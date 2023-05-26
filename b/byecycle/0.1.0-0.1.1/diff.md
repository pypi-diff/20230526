# Comparing `tmp/byecycle-0.1.0.tar.gz` & `tmp/byecycle-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byecycle-0.1.0.tar", last modified: Thu May 18 13:41:48 2023, max compression
+gzip compressed data, was "byecycle-0.1.1.tar", last modified: Fri May 26 08:40:07 2023, max compression
```

## Comparing `byecycle-0.1.0.tar` & `byecycle-0.1.1.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-04-04 19:18:13.300704 byecycle-0.1.0/LICENSE
--rw-r--r--   0        0        0       67 2023-05-11 20:56:47.502994 byecycle-0.1.0/README.md
--rw-r--r--   0        0        0      694 2023-05-18 13:41:48.485118 byecycle-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      129 2023-05-17 22:53:25.609403 byecycle-0.1.0/src/byecycle/__init__.py
--rw-r--r--   0        0        0     2052 2023-05-18 13:39:08.226357 byecycle-0.1.0/src/byecycle/cli.py
--rw-r--r--   0        0        0     2336 2023-05-18 11:23:50.007985 byecycle-0.1.0/src/byecycle/draw/__init__.py
--rw-r--r--   0        0        0     8151 2023-05-17 22:58:46.103839 byecycle-0.1.0/src/byecycle/graph.py
--rw-r--r--   0        0        0     1455 2023-05-17 22:21:01.575014 byecycle-0.1.0/src/byecycle/misc.py
--rw-r--r--   0        0        0        0 2023-05-11 21:22:15.360916 byecycle-0.1.0/src/byecycle/py.typed
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 byecycle-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-26 08:38:47.187985 byecycle-0.1.1/LICENSE
+-rw-r--r--   0        0        0     3530 2023-05-26 08:38:47.187985 byecycle-0.1.1/README.md
+-rw-r--r--   0        0        0     1374 2023-05-26 08:40:07.065619 byecycle-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/__init__.py
+-rw-r--r--   0        0        0     3760 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/cli.py
+-rw-r--r--   0        0        0     2350 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/draw/__init__.py
+-rw-r--r--   0        0        0     9163 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/graph.py
+-rw-r--r--   0        0        0     5141 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/misc.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/py.typed
+-rw-r--r--   0        0        0        0 2023-05-26 08:38:47.191985 byecycle-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-26 08:38:47.191985 byecycle-0.1.1/tests/test_module_imports.py
+-rw-r--r--   0        0        0     4193 1970-01-01 00:00:00.000000 byecycle-0.1.1/PKG-INFO
```

### Comparing `byecycle-0.1.0/LICENSE` & `byecycle-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `byecycle-0.1.0/src/byecycle/draw/__init__.py` & `byecycle-0.1.1/src/byecycle/draw/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from chextra import warn
 
 warn()
 
 from pathlib import Path
 
-import networkx as nx
-import matplotlib.pyplot as plt
-import matplotlib.colors as clrs
-import matplotlib.patches as ptc
+import matplotlib.colors as clrs  # type: ignore
+import matplotlib.patches as ptc  # type: ignore
+import matplotlib.pyplot as plt  # type: ignore
+import networkx as nx  # type: ignore
 
 DEFAULT_COLORS = {
     "no_cycle": "black",
     "good": "green",
     "bad": "red",
     "complicated": "yellow",
 }
 
 
-def draw_graph(package: str, g: nx.DiGraph) -> tuple[Path, Path]:
+def draw_graph(package: str, g: nx.DiGraph, draw_only_cycles: bool) -> tuple[Path, Path]:
+    """Use matplotlib to draw the import graph."""
     graph_path = Path(f"{package}.png")
     legend_path = Path(f"{package}_legend.png")
 
     all_colors = list(clrs.CSS4_COLORS)
     ratio = 0 if not g.nodes() else len(all_colors) / len(g.nodes())
     colors = {k: all_colors[int(i * ratio)] for i, k in enumerate(g.nodes())}
 
@@ -34,47 +35,41 @@
         node_shape="o",
     )
     nx.draw_networkx_edges(
         g,
         pos=layout,
         edge_color=DEFAULT_COLORS["no_cycle"],
         arrows=True,
-        edgelist=[(e_0, e_1) for e_0, e_1 in g.edges if not g[e_0][e_1]["cycle"]],
+        edgelist=[
+            (e_0, e_1)
+            for e_0, e_1 in g.edges
+            if g[e_0][e_1]["cycle"] is None and not draw_only_cycles
+        ],
     )
     nx.draw_networkx_edges(
         g,
         pos=layout,
         edge_color=DEFAULT_COLORS["good"],
         arrows=False,
-        edgelist=[
-            (e_0, e_1)
-            for e_0, e_1 in g.edges
-            if g[e_0][e_1]["cycle"] and g[e_0][e_1]["severity"] == "good"
-        ],
+        edgelist=[(e_0, e_1) for e_0, e_1 in g.edges if g[e_0][e_1]["cycle"] == "good"],
     )
     nx.draw_networkx_edges(
         g,
         pos=layout,
         edge_color=DEFAULT_COLORS["bad"],
         arrows=False,
-        edgelist=[
-            (e_0, e_1)
-            for e_0, e_1 in g.edges
-            if g[e_0][e_1]["cycle"] and g[e_0][e_1]["severity"] == "bad"
-        ],
+        edgelist=[(e_0, e_1) for e_0, e_1 in g.edges if g[e_0][e_1]["cycle"] == "bad"],
     )
     nx.draw_networkx_edges(
         g,
         pos=layout,
         edge_color=DEFAULT_COLORS["complicated"],
         arrows=False,
         edgelist=[
-            (e_0, e_1)
-            for e_0, e_1 in g.edges
-            if g[e_0][e_1]["cycle"] and g[e_0][e_1]["severity"] == "complicated"
+            (e_0, e_1) for e_0, e_1 in g.edges if g[e_0][e_1]["cycle"] == "complicated"
         ],
     )
     plt.title(f"Import graph for {package}")
     plt.savefig(str(graph_path))
     plt.show()
 
     # store legend
```

### Comparing `byecycle-0.1.0/src/byecycle/graph.py` & `byecycle-0.1.1/src/byecycle/graph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,60 +1,68 @@
 from __future__ import annotations
 
+import ast
 from collections import defaultdict
 from pathlib import Path
-import ast
 from typing import Iterable
 
-import networkx as nx
+import networkx as nx  # type: ignore
 
-from byecycle.misc import EdgeKind, ImportKind, cycle_severity, filename_to_module_path
+from byecycle.misc import EdgeKind, ImportKind, cycle_severity, path_to_module_name
 
 
 class Module:
+    """Represent a python module and the modules it imports."""
+
     _modules: list["Module"] = list()
     _sorted: bool = False
 
     def __init__(self, name: str):
         self.name: str = name
         Module._modules.append(self)
-        self.imports: dict[Module : set[ImportKind]] = defaultdict(set)
+        self.imports: dict[Module, set[ImportKind]] = defaultdict(set)
 
-    def add(self, other: "Module" | str, tags: list[ImportKind]):
+    def add(self, other: Module | str, tag: ImportKind):
         """Add an import to this Module.
 
         This method can only be called once all Modules have been instantiated.
 
         Args:
             other: A modules, either as an object or as a string that will be evaluated as
                 its longest match from all valid module names. Valid strings are fully
                 qualified import arguments, i.e. `"foo.bar"` from `import foo.bar` or
                 `"foo.bar.baz"` from `from foo.bar import baz`. If `foo.bar` is a
                 registered module with name `baz` in it, both strings would add the module
                 `foo.bar` as an import.
-            tags: Describes the kind of import, e.g. import of module `foo` has the
-                tags `typing` and `parent`, meaning it is the import of a parent module
-                within an `if typing.TYPE_CHECKING` block, which will be important
-                information once we want to visualize the severity of certain cyclic
-                imports.
+            tag: Describes the kind of import, e.g. import of module `foo` has the
+                tags `typing`, meaning it is the import of a parent module within an
+                `if typing.TYPE_CHECKING` block, which will be important information once
+                we want to visualize the severity of certain cyclic imports.
         """
         if not Module._sorted:
             # sort in descending alphabetical order, so that the longest match is found
             # first
             Module._modules.sort(key=lambda n: n.name, reverse=True)
             Module._sorted = True
 
         if isinstance(other, Module):
-            self.imports[other].update(tags)
-            return
-        if isinstance(other, str):
+            target = other
+        elif isinstance(other, str):
             for node in Module.modules():
                 if other.startswith(node.name):
-                    self.imports[node].update(tags)
-                    return
+                    target = node
+                    break
+            else:
+                # when calling this function, filter with `startswith(package)`
+                raise RuntimeError
+        else:
+            # bad parameter type
+            raise RuntimeError
+
+        self.imports[target].add(tag)
 
     def __hash__(self):
         return self.name.__hash__()
 
     def __repr__(self):
         imports = {
             k.name: v if v else "∅"
@@ -87,132 +95,135 @@
             https://discuss.python.org/t/question-understanding-imports-a-bit-better-how-are-cycles-avoided/26647/2
 
         Notes:
             This method can only be called once all Nodes have been initialised.
         """
         nodes: dict[str, Module] = {node.name: node for node in cls.modules()}
         for node in cls.modules():
-            package = node.name.rsplit(".", 1)[
-                0
-            ]  # only direct parent, not grandparents
-            if package in nodes:
-                node.add(nodes[package], ["parent"])
+            package = node.name.rsplit(".", 1)[0]  # only direct parent, not grandparents
+            if package in nodes and package != node.name:
+                node.add(nodes[package], "parent")
 
 
 class ImportVisitor(ast.NodeVisitor):
+    """Collect import statements in a module and assign them an `ImportKind` category.
+
+    Relies on a non-standard `_parent` field being present in each node which contains
+    a link to its parent node.
+    """
+
     def __init__(self):
-        self.imports: list[tuple[str, list[ImportKind]]] = []
+        self.imports: list[tuple[str, ImportKind]] = []
 
     @classmethod
-    def find_import_kinds(cls, node: ast.Import | ast.ImportFrom) -> list[ImportKind]:
-        ret: list[ImportKind] = []
-        parent: ast.AST = node.parent
-        # conditional top-level module imports
-        if isinstance(parent, ast.If) and isinstance(parent.parent, ast.Module):
-            # guarded by `if typing.TYPE_CHECKING:`
-            if isinstance(parent.test, ast.Name):
-                if parent.test.id == "TYPE_CHECKING":
-                    ret.append("typing")
-            elif isinstance(parent.test, ast.Attribute):
-                if parent.test.attr == "TYPE_CHECKING":
-                    ret.append("typing")
-            # probably guarded by `if sys.version >= (x, y, z):`, but doesn't actually
-            # matter -- anything but TYPE_CHECKING is env-dependent during runtime or
-            # too obtuse to consider (I'm not writing code that checks for `if True:`)
-            else:
-                ret.append("conditional")
-        else:
-            # test if the import happens somewhere in a function
-            current = parent
-            while hasattr(current, "parent"):
-                if isinstance(current, (ast.FunctionDef, ast.AsyncFunctionDef)):
-                    ret.append("dynamic")
-                    break
-                current = current.parent
-            else:
-                # any nodes that reach this point are treated as regular toplevel imports,
-                # like imports that happen in a class body
-                pass
-        return ret
+    def find_import_kind(cls, node: ast.Import | ast.ImportFrom) -> ImportKind:
+        parent: ast.AST = node._parent  # type: ignore[union-attr]
+        match parent:
+            case ast.If(
+                _parent=ast.Module,  # type: ignore[misc]
+                test=(ast.Name(id="TYPE_CHECKING") | ast.Attribute(attr="TYPE_CHECKING")),
+            ):
+                # guarded by `if typing.TYPE_CHECKING:`
+                return "typing"
+            case ast.If(_parent=ast.Module):  # type: ignore[misc]
+                # probably guarded by `if sys.version >= (x, y, z):`, but doesn't actually
+                # matter -- anything but TYPE_CHECKING is env-dependent during runtime or
+                # too obtuse to consider (I'm not writing code that checks for `if True:`)
+                return "conditional"
+            case ast.AST(_parent=current):  # type: ignore[misc]
+                while True:
+                    # test if the import happens somewhere in a function
+                    if isinstance(current, (ast.FunctionDef, ast.AsyncFunctionDef)):
+                        return "dynamic"
+                    try:
+                        current = current._parent
+                    except AttributeError:
+                        # any nodes that reach this point are treated as regular toplevel
+                        # imports, like imports that happen in a class body
+                        return "vanilla"
+            case _:
+                # shouldn't happen, but just in case
+                return "vanilla"
 
     def visit_Import(self, node: ast.Import):
-        kinds = self.find_import_kinds(node)
+        kind = self.find_import_kind(node)
         for alias in node.names:
-            self.imports.append((alias.name, kinds))
+            self.imports.append((alias.name, kind))
 
     def visit_ImportFrom(self, node: ast.ImportFrom):
-        kinds = self.find_import_kinds(node)
+        kind = self.find_import_kind(node)
+        # handle relative imports
+        if node.level:
+            path = node._module[: -node.level]  # type: ignore[attr-defined]
+            if node.module:
+                path.append(node.module)
+            module = ".".join(path)
+        else:
+            assert node.module is not None  # iff None when node.level > 0 # nosec
+            module = node.module
+
         for alias in node.names:
-            self.imports.append((f"{node.module}.{alias.name}", kinds))
+            self.imports.append((f"{module}.{alias.name}", kind))
 
 
 def import_map(package: str) -> list[Module]:
     """Creates a directed graph of import statements.
 
     Args:
         package: Path to the source root, e.g. "/home/dev/my_lib/src/my_lib"
 
     Returns:
         Mapping of python module names to a list of all module names that it imports
     """
-    node_data: dict[Module, list[tuple[str, list[ImportKind]]]] = {}
+    node_data: dict[Module, list[tuple[str, ImportKind]]] = {}
     package_name = Path(package).name
 
-    for path in map(str, Path(package).rglob("*")):
-        if not path.endswith(".py"):
+    # walk the project, compile all python files, collect their import statements
+    for path in Path(package).rglob("*"):
+        if not path.name.endswith(".py"):
             continue
-        name = filename_to_module_path(path, package, package_name)
+        name = path_to_module_name(str(path), package, package_name)
 
         with open(path) as f:
             ast_ = ast.parse(f.read())
+
+        # add a link to parent modules to make `Module.add_parent_imports` work
+        # and a link to their assumed module path to resolve imports
         for node in ast.walk(ast_):
             for child in ast.iter_child_nodes(node):
-                child.parent = node
-        # ast_ = AddParentLink().visit(ast_)
+                child._parent = node  # type: ignore[attr-defined]
+                child._module = (  # type: ignore[attr-defined]
+                    name.split(".") + ["."]
+                    if path.name == "__init__.py"
+                    else name.split(".")
+                )
         visitor = ImportVisitor()
         visitor.visit(ast_)
         node_data[Module(name)] = [
             (m, t) for m, t in visitor.imports if m.startswith(package_name)
         ]
     Module.add_parent_imports()
 
     # add all found imports to their respective module
-    for node, imports in node_data.items():
-        for import_, kinds in imports:
-            node.add(import_, kinds)
+    for module, imports in node_data.items():
+        for import_, kind in imports:
+            module.add(import_, kind)
 
     return [*Module.modules()]
 
 
-def build_digraph(modules: list[Module], **kwargs: dict[ImportKind, EdgeKind]) -> nx.DiGraph:
+def build_digraph(modules: list[Module], **kwargs: EdgeKind) -> nx.DiGraph:
     """Turns a module-imports-mapping into a smart graph object."""
     g = nx.DiGraph()
     g.add_nodes_from([m.name for m in modules])
     for module in modules:
         for import_, tags in module.imports.items():
-            g.add_edge(module.name, import_.name, severity=cycle_severity(tags, **kwargs))
-
+            g.add_edge(module.name, import_.name, tags=tags)
     for e_0, e_1 in g.edges():
         if g.has_edge(e_1, e_0):
-            g[e_0][e_1].update(cycle=True)
+            g[e_0][e_1]["tags"] = g[e_0][e_1]["tags"] | g[e_1][e_0]["tags"]
+            g[e_0][e_1]["cycle"] = cycle_severity(g[e_0][e_1]["tags"], **kwargs)
         else:
-            g[e_0][e_1].update(cycle=False)
-
+            g[e_0][e_1]["cycle"] = None
+    for e_0, e_1 in g.edges():
+        g[e_0][e_1]["tags"] = [*g[e_0][e_1]["tags"]]
     return g
-
-
-def solve(
-    path: str,
-    *,
-    dynamic: EdgeKind = "complicated",
-    conditional: EdgeKind = "complicated",
-    typing: EdgeKind = "skip",
-    parent: EdgeKind = "complicated",
-) -> nx.DiGraph:
-    modules = import_map(
-        path
-    )
-    return build_digraph(modules,
-        dynamic=dynamic,
-        conditional=conditional,
-        typing=typing,
-        parent=parent,)
```

