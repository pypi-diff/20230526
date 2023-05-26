# Comparing `tmp/shed-2023.5.1.tar.gz` & `tmp/shed-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shed-2023.5.1.tar", last modified: Tue May  2 05:28:10 2023, max compression
+gzip compressed data, was "shed-2023.5.2.tar", last modified: Fri May 26 14:54:17 2023, max compression
```

## Comparing `shed-2023.5.1.tar` & `shed-2023.5.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-02 05:27:59.000000 shed-2023.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-02 05:28:10.376080 shed-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-02 05:27:59.000000 shed-2023.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 05:28:10.376080 shed-2023.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-02 05:27:59.000000 shed-2023.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/src/shed/
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30471 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/_codemods.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 05:27:59.000000 shed-2023.5.1/src/shed/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/src/shed.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-02 05:28:10.000000 shed-2023.5.1/src/shed.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 05:28:10.376080 shed-2023.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-02 05:27:59.000000 shed-2023.5.1/tests/test_expected_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-02 05:27:59.000000 shed-2023.5.1/tests/test_shed.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-02 05:27:59.000000 shed-2023.5.1/tests/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.593455 shed-2023.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-26 14:54:01.000000 shed-2023.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-26 14:54:17.593455 shed-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-05-26 14:54:01.000000 shed-2023.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:54:17.593455 shed-2023.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-05-26 14:54:01.000000 shed-2023.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.589455 shed-2023.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.589455 shed-2023.5.2/src/shed/
+-rw-r--r--   0 runner    (1001) docker     (123)     9800 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6217 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30931 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/_codemods.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:01.000000 shed-2023.5.2/src/shed/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.589455 shed-2023.5.2/src/shed.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5070 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 14:54:17.000000 shed-2023.5.2/src/shed.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:54:17.593455 shed-2023.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1680 2023-05-26 14:54:01.000000 shed-2023.5.2/tests/test_expected_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7508 2023-05-26 14:54:01.000000 shed-2023.5.2/tests/test_shed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 14:54:01.000000 shed-2023.5.2/tests/test_suggest_different_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-26 14:54:01.000000 shed-2023.5.2/tests/test_version.py
```

### Comparing `shed-2023.5.1/LICENSE` & `shed-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shed-2023.5.1/PKG-INFO` & `shed-2023.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shed
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: `shed` canonicalises Python code.
 Home-page: https://github.com/Zac-HD/shed
 Author: Zac Hatfield-Dodds
 Author-email: zac@zhd.dev
 License: AGPL-3.0
 Project-URL: Source, https://github.com/Zac-HD/shed/
 Project-URL: Changelog, https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md
@@ -77,15 +77,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.5.1
+  rev: 2023.5.2
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.5.1/README.md` & `shed-2023.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.5.1
+  rev: 2023.5.2
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.5.1/setup.py` & `shed-2023.5.2/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         "Changelog": "https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md",
         "Funding": "https://github.com/sponsors/Zac-HD",
     },
     license="AGPL-3.0",
     description="`shed` canonicalises Python code.",
     install_requires=[
         "autoflake >= 1.4",
-        "black >= 23.1.0",
+        "black >= 23.3.0",
         "com2ann >= 0.3.0 ; python_version >= '3.8'",
         "isort >= 5.10.1",
-        "libcst >= 0.4.7",
+        "libcst >= 0.4.10",
         "pyupgrade >= 3.0.0",
     ],
     python_requires=">=3.7",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Programming Language :: Python :: 3 :: Only",
```

### Comparing `shed-2023.5.1/src/shed/__init__.py` & `shed-2023.5.2/src/shed/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,30 +17,30 @@
 import black
 import isort
 import pyupgrade._main
 from black.mode import TargetVersion
 from black.parsing import lib2to3_parse
 from isort.exceptions import FileSkipComment
 
-__version__ = "2023.5.1"
+__version__ = "2023.5.2"
 __all__ = ["shed", "docshed"]
 
 # Conditionally imported in refactor mode to reduce startup latency in the common case
 com2ann: Any = None
 _run_codemods: Any = None
 
 _version_map = {
     k: (int(k.name[2]), int(k.name[3:]))
     for k in TargetVersion
     if k.value >= TargetVersion.PY37.value
 }
 _default_min_version = min(_version_map.values())
 _SUGGESTIONS = (
     # If we fail on invalid syntax, check for detectable wrong-codeblock types
-    (r"^(>>> | In [\d+]: )", "pycon"),
+    (r"^(>>> | ?In \[\d+\]: )", "pycon"),
     (r"^Traceback \(most recent call last\):$", "python-traceback"),
 )
 
 
 class ShedSyntaxWarning(SyntaxWarning):
     """Warns that shed has been called on something with invalid syntax."""
 
@@ -92,23 +92,16 @@
                 f".{sys.version_info.minor}, so please report this as a bug."
             )
         w = ShedSyntaxWarning(msg)
         w.__cause__ = err
         if "SHED_RAISE" in os.environ:  # pragma: no cover
             raise w
         warnings.warn(w, stacklevel=_location.count(" block in ") + 2)
-        # Even if the code itself has invalid syntax, we might be able to
-        # regex-match and therefore reformat code embedded in docstrings.
-        return docshed(
-            source_code,
-            refactor=refactor,
-            first_party_imports=first_party_imports,
-            min_version=min_version,
-            _location=_location,
-        )
+        return source_code
+
     target_versions &= set(black.detect_target_versions(parsed))
     assert target_versions
     min_version = max(
         min_version,
         _version_map[min(target_versions, key=attrgetter("value"))],
     )
 
@@ -190,22 +183,14 @@
     # so we may need to re-sort its output.
     if source_code != pre_autoflake:
         source_code = run_isort()
 
     if source_code != blackened:
         source_code = black.format_str(source_code, mode=black_mode)
 
-    # Then shed.docshed (below) formats any code blocks in documentation
-    source_code = docshed(
-        source_code,
-        refactor=refactor,
-        first_party_imports=first_party_imports,
-        min_version=min_version,
-        _location=_location,
-    )
     # Remove any extra trailing whitespace
     return source_code.rstrip() + "\n"
 
 
 @functools.lru_cache()
 def docshed(
     source: str,
```

### Comparing `shed-2023.5.1/src/shed/_cli.py` & `shed-2023.5.2/src/shed/_cli.py`

 * *Files identical despite different names*

### Comparing `shed-2023.5.1/src/shed/_codemods.py` & `shed-2023.5.2/src/shed/_codemods.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # type: ignore
 """Custom LibCST-based codemods for Shed.
 
 These are mostly based on flake8, flake8-comprehensions, and some personal
 nitpicks about typing unions and literals.
 """
 
-import os
 import re
 from ast import literal_eval
 from functools import wraps
 from typing import List, Tuple, Union
 
 import libcst as cst
 import libcst.matchers as m
 from libcst.codemod import VisitorBasedCodemodCommand
 
+from . import docshed
+
 
 def leave(matcher):
     """Wrap `libcst.matchers.leave` for fixed behaviour.
 
     This works around https://github.com/Instagram/LibCST/issues/888
     by checking if the updated node matches the matcher.
     """
@@ -53,35 +54,27 @@
 ).search
 
 
 def _run_codemods(code: str, min_version: Tuple[int, int]) -> str:
     """Run all Shed fixers on a code string."""
     context = cst.codemod.CodemodContext()
 
-    # Only the native parser supports Python 3.9 and later, but for now it's
-    # only active if you set an environment variable.  Very well then:
-    var = os.environ.get("LIBCST_PARSER_TYPE")
     try:
-        os.environ["LIBCST_PARSER_TYPE"] = "native"
         mod = cst.parse_module(code)
     except cst.ParserSyntaxError:
         try:
             compile(code, "<string>", "exec")
         except SyntaxError:
             # We successfully parsed this code with lib2to3 for Black, but that
             # sometimes permits invalid syntax which libcst does not.  We'll just
             # skip refactoring here; see https://github.com/Zac-HD/shed/issues/93
             return code  # pragma: no branch  # version-dependent bug
         else:  # pragma: no cover  # This is only in case of libcst bugs
             # If the `compile()` builtin is happy, we want to crash after all.
             raise
-    finally:
-        os.environ.pop("LIBCST_PARSER_TYPE")
-        if var is not None:  # pragma: no cover  # version-dependent bug
-            os.environ["LIBCST_PARSER_TYPE"] = var
 
     if imports_hypothesis(code):  # pragma: no cover
         mod = attempt_hypothesis_codemods(context, mod)
     mod = ShedFixers(context, min_version).transform_module(mod)
     return mod.code
 
 
@@ -700,15 +693,15 @@
             return updated_node
 
         candidate_with: cst.With = updated_node
         compound_items: List[cst.WithItem] = []
         final_body: cst.BaseSuite = candidate_with.body
 
         def has_leading_comment(node: Union[cst.SimpleStatementLine, cst.With]) -> bool:
-            return any([line.comment is not None for line in node.leading_lines])
+            return any(line.comment is not None for line in node.leading_lines)
 
         header = m.AllOf(
             m.TrailingWhitespace(),
             m.MatchIfTrue(lambda h: h.comment is not None),
         )
         footer = [m.ZeroOrMore(), m.EmptyLine(comment=m.Comment()), m.ZeroOrMore()]
 
@@ -750,7 +743,27 @@
         return updated_node.with_changes(
             body=final_body,
             items=compound_items,
             # Black will only format with parens if they're there to start, so:
             lpar=cst.LeftParen(),
             rpar=cst.RightParen(),
         )
+
+    # helpers for the matchers in _docshed_docstrings
+    __first_expr_docstring = [
+        m.SimpleStatementLine(body=[m.Expr(value=m.SimpleString())]),
+        m.ZeroOrMore(m.DoNotCare()),
+    ]
+    __first_expr_docstring_in_indent = m.IndentedBlock(body=__first_expr_docstring)
+
+    @m.leave(m.FunctionDef(body=__first_expr_docstring_in_indent))
+    @m.leave(m.ClassDef(body=__first_expr_docstring_in_indent))
+    @m.leave(m.Module(body=__first_expr_docstring))
+    def _docshed_docstrings(self, _, updated_node):
+        if isinstance(updated_node, (cst.FunctionDef, cst.ClassDef)):
+            first_line = updated_node.body
+        else:
+            first_line = updated_node
+
+        string_node = first_line.body[0].body[0].value
+        new_value = docshed(string_node.value, refactor=True)
+        return updated_node.with_deep_changes(string_node, value=new_value)
```

### Comparing `shed-2023.5.1/src/shed.egg-info/PKG-INFO` & `shed-2023.5.2/src/shed.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shed
-Version: 2023.5.1
+Version: 2023.5.2
 Summary: `shed` canonicalises Python code.
 Home-page: https://github.com/Zac-HD/shed
 Author: Zac Hatfield-Dodds
 Author-email: zac@zhd.dev
 License: AGPL-3.0
 Project-URL: Source, https://github.com/Zac-HD/shed/
 Project-URL: Changelog, https://github.com/Zac-HD/shed/blob/master/CHANGELOG.md
@@ -77,15 +77,15 @@
 If you use [pre-commit](https://pre-commit.com/), you can use it with Shed by
 adding the following to your `.pre-commit-config.yaml`:
 
 ```yaml
 minimum_pre_commit_version: '2.9.0'
 repos:
 - repo: https://github.com/Zac-HD/shed
-  rev: 2023.5.1
+  rev: 2023.5.2
   hooks:
     - id: shed
       # args: [--refactor, --py39-plus]
       types_or: [python, pyi, markdown, rst]
 ```
 
 This is often considerably faster for large projects, because `pre-commit`
```

### Comparing `shed-2023.5.1/tests/test_expected_output.py` & `shed-2023.5.2/tests/test_expected_output.py`

 * *Files identical despite different names*

### Comparing `shed-2023.5.1/tests/test_shed.py` & `shed-2023.5.2/tests/test_shed.py`

 * *Files 0% similar despite different names*

```diff
@@ -110,15 +110,15 @@
 @example(source_code="@0\ndef f(): pass\n", **example_kwargs)
 @example(source_code="match 0:\n  case 0: ...\n", **example_kwargs)
 @example(source_code="try: pass\nexcept* 0: pass\n", **example_kwargs)
 @example(
     source_code="async def f(x): [[x async for x in ...] for y in ()]\n",
     **example_kwargs,
 )
-@settings(suppress_health_check=HealthCheck.all(), deadline=None)
+@settings(suppress_health_check=list(HealthCheck), deadline=None)
 def test_shed_is_idempotent(source_code, refactor, provides, min_version):
     check(source_code, refactor=refactor, min_version=min_version, provides=provides)
 
 
 def test_guesses_shed_is_first_party():
     assert _guess_first_party_modules() == frozenset(["shed"])
```

### Comparing `shed-2023.5.1/tests/test_version.py` & `shed-2023.5.2/tests/test_version.py`

 * *Files identical despite different names*

