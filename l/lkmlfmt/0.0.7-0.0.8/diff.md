# Comparing `tmp/lkmlfmt-0.0.7.tar.gz` & `tmp/lkmlfmt-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lkmlfmt-0.0.7.tar", max compression
+gzip compressed data, was "lkmlfmt-0.0.8.tar", max compression
```

## Comparing `lkmlfmt-0.0.7.tar` & `lkmlfmt-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,14 @@
--rw-r--r--   0        0        0     2582 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/README.md
--rw-r--r--   0        0        0       53 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/__init__.py
--rw-r--r--   0        0        0       70 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/__main__.py
--rw-r--r--   0        0        0     2738 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/command.py
--rw-r--r--   0        0        0      100 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/exception.py
--rw-r--r--   0        0        0    11547 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/formatter.py
--rw-r--r--   0        0        0      757 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/lkml.lark
--rw-r--r--   0        0        0       64 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/logger.py
--rw-r--r--   0        0        0     2292 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/parser.py
--rw-r--r--   0        0        0     4251 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/lkmlfmt/template.py
--rw-r--r--   0        0        0      534 2023-05-22 14:48:35.496985 lkmlfmt-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 lkmlfmt-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2582 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/README.md
+-rw-r--r--   0        0        0       53 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/__init__.py
+-rw-r--r--   0        0        0       70 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/__main__.py
+-rw-r--r--   0        0        0     2738 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/command.py
+-rw-r--r--   0        0        0      100 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/exception.py
+-rw-r--r--   0        0        0    11592 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/formatter.py
+-rw-r--r--   0        0        0      757 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/lkml.lark
+-rw-r--r--   0        0        0       64 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/logger.py
+-rw-r--r--   0        0        0     2292 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/parser.py
+-rw-r--r--   0        0        0        0 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/py.typed
+-rw-r--r--   0        0        0     4251 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/lkmlfmt/template.py
+-rw-r--r--   0        0        0      534 2023-05-26 13:51:34.430199 lkmlfmt-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2987 1970-01-01 00:00:00.000000 lkmlfmt-0.0.8/PKG-INFO
```

### Comparing `lkmlfmt-0.0.7/README.md` & `lkmlfmt-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.7/lkmlfmt/command.py` & `lkmlfmt-0.0.8/lkmlfmt/command.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.7/lkmlfmt/formatter.py` & `lkmlfmt-0.0.8/lkmlfmt/formatter.py`

 * *Files 0% similar despite different names*

```diff
@@ -98,15 +98,17 @@
 {value}
 {self.fmt_indent()};;"""
 
         # sql_xxx: ... ;; or expression_xxx: ... ;;
         with self.indent():
             # https://docs.python.org/3/library/functions.html#property
             Line.prefix = property(  # type: ignore
-                lambda s: " " * INDENT_WIDTH * (s.depth[0] + self.curr_indent)
+                lambda s: " "
+                * INDENT_WIDTH
+                * (s.depth[0] + s.depth[1] + self.curr_indent)
             )
             if key.startswith("sql"):
                 formatted = self._try_plugins(value, "fmt_sql")
                 if formatted is not None:
                     value = formatted
                 else:
                     value = self._fmt_sql(value)
```

### Comparing `lkmlfmt-0.0.7/lkmlfmt/lkml.lark` & `lkmlfmt-0.0.8/lkmlfmt/lkml.lark`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.7/lkmlfmt/parser.py` & `lkmlfmt-0.0.8/lkmlfmt/parser.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.7/lkmlfmt/template.py` & `lkmlfmt-0.0.8/lkmlfmt/template.py`

 * *Files identical despite different names*

### Comparing `lkmlfmt-0.0.7/pyproject.toml` & `lkmlfmt-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lkmlfmt"
-version = "0.0.7"
+version = "0.0.8"
 description = ""
 authors = ["dr666m1 <skndr666m1@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.scripts]
 lkmlfmt = "lkmlfmt.command:run"
```

### Comparing `lkmlfmt-0.0.7/PKG-INFO` & `lkmlfmt-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lkmlfmt
-Version: 0.0.7
+Version: 0.0.8
 Summary: 
 Author: dr666m1
 Author-email: skndr666m1@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
```

