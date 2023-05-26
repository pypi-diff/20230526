# Comparing `tmp/byecycle-0.1.1.tar.gz` & `tmp/byecycle-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "byecycle-0.1.1.tar", last modified: Fri May 26 08:40:07 2023, max compression
+gzip compressed data, was "byecycle-0.1.2.tar", last modified: Fri May 26 19:25:15 2023, max compression
```

## Comparing `byecycle-0.1.1.tar` & `byecycle-0.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1069 2023-05-26 08:38:47.187985 byecycle-0.1.1/LICENSE
--rw-r--r--   0        0        0     3530 2023-05-26 08:38:47.187985 byecycle-0.1.1/README.md
--rw-r--r--   0        0        0     1374 2023-05-26 08:40:07.065619 byecycle-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      147 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/__init__.py
--rw-r--r--   0        0        0     3760 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/cli.py
--rw-r--r--   0        0        0     2350 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/draw/__init__.py
--rw-r--r--   0        0        0     9163 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/graph.py
--rw-r--r--   0        0        0     5141 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/misc.py
--rw-r--r--   0        0        0        0 2023-05-26 08:38:47.191985 byecycle-0.1.1/src/byecycle/py.typed
--rw-r--r--   0        0        0        0 2023-05-26 08:38:47.191985 byecycle-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      155 2023-05-26 08:38:47.191985 byecycle-0.1.1/tests/test_module_imports.py
--rw-r--r--   0        0        0     4193 1970-01-01 00:00:00.000000 byecycle-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-26 19:23:38.316533 byecycle-0.1.2/LICENSE
+-rw-r--r--   0        0        0     5375 2023-05-26 19:23:38.316533 byecycle-0.1.2/README.md
+-rw-r--r--   0        0        0     1569 2023-05-26 19:25:15.970280 byecycle-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      147 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/__init__.py
+-rw-r--r--   0        0        0     4064 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/cli.py
+-rw-r--r--   0        0        0     2583 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/draw/__init__.py
+-rw-r--r--   0        0        0    12094 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/graph.py
+-rw-r--r--   0        0        0     6959 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/misc.py
+-rw-r--r--   0        0        0        0 2023-05-26 19:23:38.316533 byecycle-0.1.2/src/byecycle/py.typed
+-rw-r--r--   0        0        0        0 2023-05-26 19:23:38.316533 byecycle-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-26 19:23:38.316533 byecycle-0.1.2/tests/test_module_imports.py
+-rw-r--r--   0        0        0     6038 1970-01-01 00:00:00.000000 byecycle-0.1.2/PKG-INFO
```

### Comparing `byecycle-0.1.1/LICENSE` & `byecycle-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `byecycle-0.1.1/pyproject.toml` & `byecycle-0.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "byecycle"
-version = "0.1.1"
+version = "0.1.2"
 description = "Find and expose cyclic imports in python projects."
 requires-python = ">=3.11"
 readme = "README.md"
 authors = [
     { name = "Arne Caratti", email = "arne.recknagel@hotmail.com" },
 ]
 classifiers = [
@@ -64,12 +64,27 @@
 warn_return_any = true
 warn_unused_ignores = true
 check_untyped_defs = true
 enable_incomplete_feature = [
     "Unpack",
 ]
 
+[tool.coverage.run]
+branch = true
+data_file = ".coverage/coverage_report"
+source = [
+    "byecycle",
+]
+
+[tool.coverage.paths]
+source = [
+    "src",
+]
+
+[tool.coverage.report]
+show_missing = true
+
 [tool.black]
 line-length = 90
 
 [tool.isort]
 profile = "black"
```

### Comparing `byecycle-0.1.1/src/byecycle/cli.py` & `byecycle-0.1.2/src/byecycle/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 import os.path
 from pathlib import Path
 
 import networkx as nx  # type: ignore
 import typer
 from rich import print, print_json
 
-from byecycle.graph import build_digraph, import_map
-from byecycle.misc import Edge, EdgeKind, GraphDict
+from byecycle.graph import Module, build_digraph
+from byecycle.misc import EdgeKind, GraphDict
 from byecycle.misc import _default_cycle_severity as severity
 from byecycle.misc import (
+    _Edge,
     conditional_annotation,
     draw_annotation,
     draw_only_cycles_annotation,
     dynamic_annotation,
     parent_annotation,
     rich_annotation,
     typing_annotation,
@@ -76,35 +77,41 @@
     typing: EdgeKind = severity["typing"],
     parent: EdgeKind = severity["parent"],
     vanilla: EdgeKind = severity["vanilla"],
 ) -> tuple[GraphDict, nx.DiGraph, str]:
     """Programmatic equivalent to running this package through the CLI.
 
     Args:
-        project: Either the path to a project source, or the name of an installed package
+        project: Either the path to a project source, or the name of an installed package.
+        dynamic: Severity of dynamic import cycles.
+        conditional: Severity of conditional import cycles.
+        typing: Severity of typing-only import cycles.
+        parent: Severity of parent-package-resolution related import cycles.
+        vanilla: Severity of vanilla import cycles.
+
 
     Returns:
-        A dictionary representation of the import graph
-        The actual import graph
-        The name of the package
+        A dictionary-representation of the import graph.
+        The actual import graph.
+        The name of the package.
     """
     if os.path.isdir(project):
         project_path = Path(project)
     else:
         loc = importlib.import_module(project).__file__
         if loc is None:
             raise RuntimeError(
                 f"Failed trying to resolve {project=} as a package, please pass source "
                 f"code location as proper path."
             )
         project_path = Path(loc).parent.resolve()
 
-    modules = import_map(str(project_path))
+    Module.populate(project_path)
     graph = build_digraph(
-        modules,
+        [*Module.modules()],
         dynamic=dynamic,
         conditional=conditional,
         typing=typing,
         parent=parent,
         vanilla=vanilla,
     )
     return {key: {**graph[key]} for key in graph}, graph, project_path.name
```

### Comparing `byecycle-0.1.1/src/byecycle/draw/__init__.py` & `byecycle-0.1.2/src/byecycle/draw/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,22 @@
     "good": "green",
     "bad": "red",
     "complicated": "yellow",
 }
 
 
 def draw_graph(package: str, g: nx.DiGraph, draw_only_cycles: bool) -> tuple[Path, Path]:
-    """Use matplotlib to draw the import graph."""
+    """Use matplotlib to draw the import graph.
+
+    This function also writes the drawn pictures to disk.
+
+    Returns:
+        The file location of the graph image.
+        The file location of the legend of the nodes from the graph image.
+    """
     graph_path = Path(f"{package}.png")
     legend_path = Path(f"{package}_legend.png")
 
     all_colors = list(clrs.CSS4_COLORS)
     ratio = 0 if not g.nodes() else len(all_colors) / len(g.nodes())
     colors = {k: all_colors[int(i * ratio)] for i, k in enumerate(g.nodes())}
 
@@ -64,23 +71,25 @@
         pos=layout,
         edge_color=DEFAULT_COLORS["complicated"],
         arrows=False,
         edgelist=[
             (e_0, e_1) for e_0, e_1 in g.edges if g[e_0][e_1]["cycle"] == "complicated"
         ],
     )
-    plt.title(f"Import graph for {package}")
-    plt.savefig(str(graph_path))
+    plt.axis("off")
+    plt.tight_layout()
+    plt.savefig(graph_path)
     plt.show()
 
     # store legend
-    plt.axis("off")
     plt.legend(
         loc="upper center",
         ncol=2,
         fancybox=True,
         shadow=True,
         handles=[ptc.Patch(color=c, label=l) for l, c in colors.items()],
     )
-    plt.savefig(legend_path)
+    plt.axis("off")
+    plt.tight_layout()
+    plt.savefig(legend_path, transparent=True)
 
     return graph_path, legend_path
```

### Comparing `byecycle-0.1.1/src/byecycle/graph.py` & `byecycle-0.1.2/src/byecycle/graph.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,29 @@
 from __future__ import annotations
 
 import ast
 from collections import defaultdict
 from pathlib import Path
-from typing import Iterable
+from typing import Iterable, Self, Unpack
 
 import networkx as nx  # type: ignore
 
-from byecycle.misc import EdgeKind, ImportKind, cycle_severity, path_to_module_name
+from byecycle.misc import (
+    EdgeKind,
+    ImportKind,
+    SeverityMap,
+    cycle_severity,
+    path_to_module_name,
+)
 
 
 class Module:
     """Represent a python module and the modules it imports."""
 
-    _modules: list["Module"] = list()
+    _modules: list[Module] = []
     _sorted: bool = False
 
     def __init__(self, name: str):
         self.name: str = name
         Module._modules.append(self)
         self.imports: dict[Module, set[ImportKind]] = defaultdict(set)
 
@@ -33,14 +39,17 @@
                 `"foo.bar.baz"` from `from foo.bar import baz`. If `foo.bar` is a
                 registered module with name `baz` in it, both strings would add the module
                 `foo.bar` as an import.
             tag: Describes the kind of import, e.g. import of module `foo` has the
                 tags `typing`, meaning it is the import of a parent module within an
                 `if typing.TYPE_CHECKING` block, which will be important information once
                 we want to visualize the severity of certain cyclic imports.
+
+        Raises:
+            RuntimeError: If bad arguments are passed.
         """
         if not Module._sorted:
             # sort in descending alphabetical order, so that the longest match is found
             # first
             Module._modules.sort(key=lambda n: n.name, reverse=True)
             Module._sorted = True
 
@@ -48,15 +57,16 @@
             target = other
         elif isinstance(other, str):
             for node in Module.modules():
                 if other.startswith(node.name):
                     target = node
                     break
             else:
-                # when calling this function, filter with `startswith(package)`
+                # when calling this function, filter with `startswith(package)` to avoid
+                # this exception
                 raise RuntimeError
         else:
             # bad parameter type
             raise RuntimeError
 
         self.imports[target].add(tag)
 
@@ -69,15 +79,15 @@
             for k, v in sorted(
                 self.imports.items(), key=lambda x: x[0].name, reverse=True
             )
         }
         return f"Module('{self.name}') -> {imports}"
 
     @classmethod
-    def modules(cls) -> Iterable["Module"]:
+    def modules(cls) -> Iterable[Module]:
         """Accessor for all registered modules."""
         yield from cls._modules
 
     @classmethod
     def add_parent_imports(cls):
         """Make modules with parent packages import them explicitly.
 
@@ -88,38 +98,127 @@
         Treating their reliance chain as _imports_ models this link accurately for the
         most part, but does create the impression of cycles if a parent imports names from
         a child, which is a popular pattern for simplifying/exposing a public API. As a
         consequence, these child-parent imports should be treated differently during
         analysis.
 
         See Also:
-            https://discuss.python.org/t/question-understanding-imports-a-bit-better-how-are-cycles-avoided/26647/2
+            [discuss.python.org: Partial Modules](https://discuss.python.org/t/question-understanding-imports-a-bit-better-how-are-cycles-avoided/26647/2)
+            for a technical explanation of how parent and child modules interact during
+            imports.
 
         Notes:
             This method can only be called once all Nodes have been initialised.
         """
         nodes: dict[str, Module] = {node.name: node for node in cls.modules()}
         for node in cls.modules():
             package = node.name.rsplit(".", 1)[0]  # only direct parent, not grandparents
             if package in nodes and package != node.name:
                 node.add(nodes[package], "parent")
 
+    @classmethod
+    def populate(cls, source_path: Path):
+        """Walks down a source tree and registers each python file as a [`Module`][byecycle.graph.Module].
+
+        After parsing all files recursively, all import statements in each file that
+        import a module that resolves to any of the files just recursed are listed
+        on their respective [`Module`][byecycle.graph.Module]. Additionally, some metadata from the context of the
+        import is retained. Specifically, the import-kind defintions are:
+
+        ___`vanilla`___
+
+        :   A regular import at the top-level of the module
+
+        ___`typing`___
+
+        :   Only executed during static type analyis
+
+        ___`dynamic`___
+
+        :   Scoped in a function, which might not be executed on module load
+
+        ___`conditional`___
+
+        :   In an if-block at the top-level of the module, so only maybe executed
+
+        ___`parent`___
+
+        :   Due to the module in question being a parent of the current module (in python,
+            parent modules are imported before their children)
+
+        If a module is imported multiple times in different ways, all their metadata is
+        aggregated on the same entry.
+
+        Once this method was executed, the [`Module.modules`][byecycle.graph.Module.modules]
+        class-method can called to produce all created modules.
+
+        Args:
+            source_path: Location of the source tree of the package that should be walked.
+                The `.name` attribute of this parameter is assumed to be the name of the
+                package in order to identify which imports are local imports.
+        """
+        node_data: dict[Module, list[tuple[str, ImportKind]]] = {}
+        package_name = source_path.name
+
+        # walk the project, compile all python files, collect their import statements
+        for path in source_path.rglob("*"):
+            if not path.name.endswith(".py"):
+                continue
+            name = path_to_module_name(str(path), str(source_path), package_name)
+
+            with open(path) as f:
+                ast_ = ast.parse(f.read())
+
+            # add a link to parent modules to make `Module.add_parent_imports` work
+            # and a link to their assumed module path to resolve imports
+            for node in ast.walk(ast_):
+                for child in ast.iter_child_nodes(node):
+                    child._parent = node  # type: ignore[attr-defined]
+                    child._module = (  # type: ignore[attr-defined]
+                        name.split(".") + ["."]
+                        if path.name == "__init__.py"
+                        else name.split(".")
+                    )
+            visitor = ImportVisitor()
+            visitor.visit(ast_)
+            node_data[cls(name)] = [
+                (m, t) for m, t in visitor.imports if m.startswith(package_name)
+            ]
+        cls.add_parent_imports()
+
+        # add all found imports to their respective module
+        for module, imports in node_data.items():
+            for import_, kind in imports:
+                module.add(import_, kind)
+
 
 class ImportVisitor(ast.NodeVisitor):
-    """Collect import statements in a module and assign them an `ImportKind` category.
+    """Collect import statements in a module and assign them an [`ImportKind`][byecycle.misc.ImportKind] category.
 
     Relies on a non-standard `_parent` field being present in each node which contains
     a link to its parent node.
     """
 
     def __init__(self):
         self.imports: list[tuple[str, ImportKind]] = []
 
     @classmethod
     def find_import_kind(cls, node: ast.Import | ast.ImportFrom) -> ImportKind:
+        """Find the [`ImportKind`][byecycle.misc.ImportKind] of an import statement.
+
+        A single import statement can only have a single [`ImportKind`][byecycle.misc.ImportKind].
+        This function uses information in the `ast.AST`-node to identify if it was
+        `dynamic`, `typing`, `conditional`, or `vanilla`.
+
+        Args:
+            node: Node in which the import statement takes place.
+
+        Returns:
+            The identified [`ImportKind`][byecycle.misc.ImportKind], by default `vanilla`.
+        """
         parent: ast.AST = node._parent  # type: ignore[union-attr]
         match parent:
             case ast.If(
                 _parent=ast.Module,  # type: ignore[misc]
                 test=(ast.Name(id="TYPE_CHECKING") | ast.Attribute(attr="TYPE_CHECKING")),
             ):
                 # guarded by `if typing.TYPE_CHECKING:`
@@ -161,62 +260,28 @@
             assert node.module is not None  # iff None when node.level > 0 # nosec
             module = node.module
 
         for alias in node.names:
             self.imports.append((f"{module}.{alias.name}", kind))
 
 
-def import_map(package: str) -> list[Module]:
-    """Creates a directed graph of import statements.
+def build_digraph(modules: list[Module], **kwargs: Unpack[SeverityMap]) -> nx.DiGraph:
+    """Turns a module-imports-mapping into a smart graph object.
 
     Args:
-        package: Path to the source root, e.g. "/home/dev/my_lib/src/my_lib"
+        modules: [`Module`][byecycle.graph.Module] objects that know what other local modules they import, and how.
+        **kwargs: Override the default settings for the severity of the "how" when imports
+            in local modules might cause import cycles.
 
     Returns:
-        Mapping of python module names to a list of all module names that it imports
+        A graph object which allows the kind of operations that you'd want when working
+        with graph-like structures. Every edge in the graph has a `tags` and a `cycle`
+        entry (accessible with `getitem()`) holding metadata that can help interpret how
+        much of an issue a particular cyclic import might be.
     """
-    node_data: dict[Module, list[tuple[str, ImportKind]]] = {}
-    package_name = Path(package).name
-
-    # walk the project, compile all python files, collect their import statements
-    for path in Path(package).rglob("*"):
-        if not path.name.endswith(".py"):
-            continue
-        name = path_to_module_name(str(path), package, package_name)
-
-        with open(path) as f:
-            ast_ = ast.parse(f.read())
-
-        # add a link to parent modules to make `Module.add_parent_imports` work
-        # and a link to their assumed module path to resolve imports
-        for node in ast.walk(ast_):
-            for child in ast.iter_child_nodes(node):
-                child._parent = node  # type: ignore[attr-defined]
-                child._module = (  # type: ignore[attr-defined]
-                    name.split(".") + ["."]
-                    if path.name == "__init__.py"
-                    else name.split(".")
-                )
-        visitor = ImportVisitor()
-        visitor.visit(ast_)
-        node_data[Module(name)] = [
-            (m, t) for m, t in visitor.imports if m.startswith(package_name)
-        ]
-    Module.add_parent_imports()
-
-    # add all found imports to their respective module
-    for module, imports in node_data.items():
-        for import_, kind in imports:
-            module.add(import_, kind)
-
-    return [*Module.modules()]
-
-
-def build_digraph(modules: list[Module], **kwargs: EdgeKind) -> nx.DiGraph:
-    """Turns a module-imports-mapping into a smart graph object."""
     g = nx.DiGraph()
     g.add_nodes_from([m.name for m in modules])
     for module in modules:
         for import_, tags in module.imports.items():
             g.add_edge(module.name, import_.name, tags=tags)
     for e_0, e_1 in g.edges():
         if g.has_edge(e_1, e_0):
```

### Comparing `byecycle-0.1.1/src/byecycle/misc.py` & `byecycle-0.1.2/src/byecycle/misc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 import enum
 from typing import (
     Annotated,
+    Iterable,
     Literal,
     Optional,
-    Sequence,
     TypeAlias,
     TypedDict,
     Unpack,
     cast,
 )
 
 from typer import Exit, Option
 
 from byecycle import __version__
 
-EdgeKind: TypeAlias = Literal["good", "bad", "complicated", "skip"]
 ImportKind: TypeAlias = Literal["dynamic", "conditional", "typing", "parent", "vanilla"]
+"""The types/kinds of imports that are currently recognized."""
+EdgeKind: TypeAlias = Literal["good", "bad", "complicated", "skip"]
+"""Describes an import cycle, helping with evaluating how much of an issue it could be."""
 edge_order: dict[EdgeKind, int] = {"bad": 0, "complicated": 1, "good": 2, "skip": 3}
 
 
 class ImportMetaData(TypedDict):
+    """Metadata to interpret import cycle severity."""
+
     tags: list[ImportKind]
     cycle: EdgeKind | None
 
 
 GraphDict: TypeAlias = dict[str, dict[str, ImportMetaData]]
+"""Dictionary representation of an import graph.
+
+The keys on the first level are the qualnames of importing modules, the keys on the second 
+level are the qualnames of imported modules, and the values on the second level contain
+the metadata dictionary of their keyed imports ([`ImportMetaData`][byecycle.misc.ImportMetaData]).
+Metadata consists of a `tags`-list of [`ImportKind`][byecycle.misc.ImportKind]s and a
+`cycle` which is either an [`EdgeKind`][byecycle.misc.EdgeKind] if there is a cycle, or
+`None` if there isn't.
+"""
 
 
 class SeverityMap(TypedDict, total=False):
+    """Mapping of [`ImportKind`][byecycle.misc.ImportKind]s to [`EdgeKind`][byecycle.misc.ImportKind]s."""
+
     dynamic: EdgeKind
     conditional: EdgeKind
     typing: EdgeKind
     parent: EdgeKind
     vanilla: EdgeKind
 
 
-class Edge(str, enum.Enum):
-    """Proxy of the EdgeKind type alias.
+class _Edge(str, enum.Enum):
+    """Proxy of the [`EdgeKind`][byecycle.misc.ImportKind] type alias.
 
     Necessary for typer due to https://github.com.tiangolo/typer/issues/76. I really hate
-    it.
+    it, also makes mypy sad.
     """
 
     good: EdgeKind = "good"
     bad: EdgeKind = "bad"
     complicated: EdgeKind = "complicated"
     skip: EdgeKind = "skip"
 
@@ -64,55 +79,74 @@
     "rich_annotation": "If unset, print plain ascii to the terminal.",
     "draw_annotation": "Flag which, if set, will draw the resulting import graph with matplotlib and write it to disk.",
     "draw_only_cycles_annotation": "If set, don't draw non-cyclic imports.",
     "version_annotation": "Print this package's version and exit.",
 }
 rich_annotation: TypeAlias = Annotated[bool, Option(help=help_texts["rich_annotation"])]
 draw_annotation: TypeAlias = Annotated[bool, Option(help=help_texts["draw_annotation"])]
-dynamic_annotation: TypeAlias = Annotated[Edge, Option(help=help_texts["dynamic_annotation"])]
-conditional_annotation: TypeAlias = Annotated[Edge, Option(help=help_texts["conditional_annotation"])]
-typing_annotation: TypeAlias = Annotated[Edge, Option(help=help_texts["typing_annotation"])]
-parent_annotation: TypeAlias = Annotated[Edge, Option(help=help_texts["parent_annotation"])]
-vanilla_annotation: TypeAlias = Annotated[Edge, Option(help=help_texts["vanilla_annotation"])]
+dynamic_annotation: TypeAlias = Annotated[_Edge, Option(help=help_texts["dynamic_annotation"])]
+conditional_annotation: TypeAlias = Annotated[_Edge, Option(help=help_texts["conditional_annotation"])]
+typing_annotation: TypeAlias = Annotated[_Edge, Option(help=help_texts["typing_annotation"])]
+parent_annotation: TypeAlias = Annotated[_Edge, Option(help=help_texts["parent_annotation"])]
+vanilla_annotation: TypeAlias = Annotated[_Edge, Option(help=help_texts["vanilla_annotation"])]
 draw_only_cycles_annotation: TypeAlias = Annotated[Optional[bool], Option("--draw-only-cycles", help=help_texts["draw_only_cycles_annotation"])]
 version_annotation: TypeAlias = Annotated[Optional[bool], Option("--version", callback=_print_version, is_eager=True, help=help_texts["version_annotation"])]
 # fmt: on
 
 _default_cycle_severity: SeverityMap = {
     "dynamic": "complicated",
     "conditional": "complicated",
     "typing": "skip",
     "parent": "complicated",
     "vanilla": "bad",
 }
 
 
 def cycle_severity(
-    cycles: Sequence[ImportKind] | set[ImportKind], **kwargs: Unpack[SeverityMap]
-) -> EdgeKind | None:
-    """"""
+    cycles: Iterable[ImportKind], **kwargs: Unpack[SeverityMap]
+) -> EdgeKind:
+    """Interpret import tags as to their severity if the import was part of a cycle.
+
+    Args:
+        cycles: The iterable of import-kind tags, at least one entry is expected.
+        **kwargs: Valid values are keywords equating to [`ImportKind`][byecycle.misc.ImportKind]s
+            mapping to [`EdgeKind`][byecycle.misc.ImportKind]s in order to override that
+            [`ImportKind`][byecycle.misc.ImportKind]'s severity-interpretation.
+
+    Returns:
+        A string denoting the severity of the cycle.
+    """
+    cycles = [*cycles]
     if not cycles:
-        return None  # shouldn't happen, every import has at least one ImportKind
+        raise RuntimeError("Every import statement needs at least one kind-identifier.")
     severity_map = cast(SeverityMap, {**_default_cycle_severity, **kwargs})
     cycles = [c for c in cycles if c != "vanilla"]
     if not cycles:
         return severity_map["vanilla"]
     severity = sorted((severity_map[c] for c in cycles), key=edge_order.get)  # type: ignore
     return severity[0]
 
 
 def path_to_module_name(path: str, base: str, name: str) -> str:
     """Turns a file path into a valid module name.
 
+    Just an educated guess on my part, I couldn't find an official reference. Chances are
+    that you can't know the real name of a package unless you actually install it, and
+    only projects that adhere to best practices and/or common sense regarding naming and
+    structure can be handled correctly by this function.
+
     Args:
         path: Absolute path to the file in question.
         base: Absolute path to the "source root".
         name: Name of the distribution.
 
-    Examples:
+    Returns:
+        A string in the form of an importable python module.
+
+    Example:
         ```py
         >>> # Sample call #1:
         >>> path_to_module_name(
         ...     path = "/home/me/dev/project/src/project/__init__.py"
         ...     base = "/home/me/dev/project/src/project/"
         ...     name = "project"
         ... )
```

### Comparing `byecycle-0.1.1/PKG-INFO` & `byecycle-0.1.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-Metadata-Version: 2.1
-Name: byecycle
-Version: 0.1.1
-Summary: Find and expose cyclic imports in python projects.
-Author-Email: Arne Caratti <arne.recknagel@hotmail.com>
-License: MIT
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Typing :: Typed
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.11
-Requires-Dist: networkx[default]>=3.1
-Requires-Dist: chextra>=0.1.1
-Requires-Dist: typer[all]>=0.9.0
-Requires-Dist: rich>=13.3
-Requires-Dist: matplotlib>=3.7; extra == "draw"
-Provides-Extra: draw
-Description-Content-Type: text/markdown
-
 # byecycle 🚲
 
+[![python](https://img.shields.io/pypi/pyversions/byecycle)](https://pdm.fming.dev)
+[![pyPI](https://img.shields.io/pypi/v/byecycle)](https://pypi.org/project/byecycle)
+[![docs](https://img.shields.io/badge/doc-pages-blue)](https://a-recknagel.github.io/byecycle/)
+[![pdm-managed](https://img.shields.io/badge/packaging-pdm-blueviolet)](https://pdm.fming.dev)
+[![license](https://img.shields.io/pypi/l/byecycle)](https://github.com/a-recknagel/byecycle/blob/main/LICENSE)
+[![chat](https://img.shields.io/badge/chat-gitter-mediumturquoise)](https://matrix.to/#/#chextra:gitter.im)
+
 Find and expose cyclic imports in python projects.
 
 ## Installation
 
-### From pyPI
+`byecycle` uses the build-in [ast module](https://docs.python.org/3/library/ast.html#ast.parse)
+to parse code files. As a consequence, it can only handle python code within the same
+major version (read: no support for python 1 and 2), and the same or lower minor version 
+of the python interpreter it was installed with. If `byecycle` raises `SyntaxErrors` in 
+code that you know to be working, try using a `byecycle` that is installed with the same 
+python version that can run the code in question.
 
+### From pyPI
+#### Requirements: 
  - python 3.11 or higher
+ - [pipx](https://pypa.github.io/pipx/installation/)
 ```shell
-# `pipx` might be a better choice, given that it's a global dev-tool
-pip install byecycle
+pipx install byecycle
 ```
 ---
 
 ### From Source / Dev Setup
-
+#### Requirements:
  - python 3.11 or higher
  - [pdm](https://pdm.fming.dev/)
  - git
 ```shell
 git clone https://github.com/a-recknagel/byecycle.git
 cd byecycle
 pdm install
@@ -47,18 +41,18 @@
 ## Usage
 
 ### As a Command Line Tool
 
 ```shell
 # with a path
 byecycle /home/me/dev/byecycle/src/byecycle/
-# or an installed package
+# or the name of an installed package
 byecycle byecycle
 ```
-The result will be a well-formed json string:
+The result will be a json string:
 
 ```json
 {
   "byecycle.misc": {},
   "byecycle.graph": {
     "byecycle": {
       "tags": [
@@ -167,15 +161,16 @@
       ],
       "cycle": "complicated"
     }
   }
 }
 ```
 Alternatively, you can also call the main entrypoint's core functionality as a regular
-python function which will return the result as a dictionary:
+python function. Among other things, it returns a dictionary equivalent to the CLI's json
+that you can work with:
 
 ```python
 from byecycle import run
 cycles, *_ = run("byecycle")
 # filter out imports that don't have a cycle
 for outer_k, outer_v in cycles.items():
     for inner_k, inner_v in outer_v.items():
@@ -185,17 +180,30 @@
 ```text
 byecycle.graph -> byecycle -> complicated
 byecycle.cli -> byecycle -> complicated
 byecycle -> byecycle.graph -> complicated
 byecycle -> byecycle.cli -> complicated
 ```
 
+---
+
+See the help text of `byecycle` for an explanation of tags/`ImportKind`s and 
+cycle/`EdgeKind`s. 
+
+In short, if there is a cycle, the tags of all involved imports inform
+the cycle-severity, with the highest severity winning out if multiple apply. The defaults
+can be overriden in order to isolate, filter, or highlight cycles with specific 
+tags/severities.
+
 ### To Visualize the Import Graph
 
-If you pass the `--draw` flag on your command-line-call, byecycle will create an image of
+If you pass the `--draw` flag<sup>1</sup> on your command-line-call, `byecycle` will create an image of
 the import graph instead:
 
 ```shell
 byecycle byecycle --draw
 ```
-<img src="docs/data/byecycle.png" alt="" width="320" height="240">
-<img src="docs/data/byecycle_legend.png" alt="" width="320" height="240">
+<img src="https://github.com/a-recknagel/byecycle/assets/2063412/e5e8427c-8554-4ce5-9f9f-e2e9eca40742" alt="Plot of imports in the byecycle project" width="320" height="240">
+<img src="https://github.com/a-recknagel/byecycle/assets/2063412/a00586db-e71e-4e74-94ed-0709129920b0" alt="Legend for nodes in the plot" width="320" height="240">
+
+---
+<sup>[1]<sub> Requires installation of the `draw`-extra, i.e. `pipx install "byecycle[draw]"`.</sub></sup>
```

