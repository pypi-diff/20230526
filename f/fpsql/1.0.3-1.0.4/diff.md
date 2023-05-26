# Comparing `tmp/fpsql-1.0.3.tar.gz` & `tmp/fpsql-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpsql-1.0.3.tar", max compression
+gzip compressed data, was "fpsql-1.0.4.tar", max compression
```

## Comparing `fpsql-1.0.3.tar` & `fpsql-1.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2021-11-16 19:34:41.000000 fpsql-1.0.3/LICENSE
--rw-r--r--   0        0        0      237 2023-05-26 01:32:44.492420 fpsql-1.0.3/README.md
--rw-r--r--   0        0        0      864 2023-05-26 01:32:33.264432 fpsql-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     4946 2023-05-25 15:22:43.623334 fpsql-1.0.3/src/fpsql/__init__.py
--rw-r--r--   0        0        0      500 2023-05-26 01:31:58.196469 fpsql-1.0.3/src/fpsql/__init__.pyi
--rw-r--r--   0        0        0        0 2023-05-26 01:31:02.620528 fpsql-1.0.3/src/fpsql/py.typed
--rw-r--r--   0        0        0     1264 1970-01-01 00:00:00.000000 fpsql-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-11-16 19:34:41.000000 fpsql-1.0.4/LICENSE
+-rw-r--r--   0        0        0      278 2023-05-26 02:00:04.970677 fpsql-1.0.4/README.md
+-rw-r--r--   0        0        0      864 2023-05-26 01:59:56.442686 fpsql-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4956 2023-05-26 02:02:22.638531 fpsql-1.0.4/src/fpsql/__init__.py
+-rw-r--r--   0        0        0      513 2023-05-26 02:00:39.094641 fpsql-1.0.4/src/fpsql/__init__.pyi
+-rw-r--r--   0        0        0        0 2023-05-26 01:31:02.620528 fpsql-1.0.4/src/fpsql/py.typed
+-rw-r--r--   0        0        0     1305 1970-01-01 00:00:00.000000 fpsql-1.0.4/PKG-INFO
```

### Comparing `fpsql-1.0.3/LICENSE` & `fpsql-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fpsql-1.0.3/pyproject.toml` & `fpsql-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fpsql"
-version = "1.0.3"
+version = "1.0.4"
 authors = ["Firepup650 <firepyp650@gmail.com>"]
 description = "An easy to use SQLite package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `fpsql-1.0.3/src/fpsql/__init__.py` & `fpsql-1.0.4/src/fpsql/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Firepup650's SQL Package"""
+from typing import Any
 import sqlite3, ast, pydoc
 
 
 def alias(Function):
     def decorator(f):
         f.__doc__ = (
             "This method is an alias of the following method:\n\n"
@@ -68,22 +69,22 @@
         # Returns:
           None
 
         # Raises:
           None"""
         self.__table = tableName
 
-    def get(self, name: str) -> object or None:
+    def get(self, name: str) -> Any:
         """# Function: sql.get
           Gets the value of a key
         # Inputs:
           name: str - The name of the key to retrieve
 
         # Returns:
-          object or None - If the key exists, return it's value, otherwise, return `None`
+          Any - If the key exists, return it's value (casted), otherwise, return `None`
 
         # Raises:
           AttributeError - If the table is unset"""
         if not self.__table:
             raise AttributeError("Attempted to read from unset table")
         cur = self.__con.execute(
             f"""SELECT value FROM "{self.__table}" WHERE name = ?""", (name,)
```

### Comparing `fpsql-1.0.3/PKG-INFO` & `fpsql-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpsql
-Version: 1.0.3
+Version: 1.0.4
 Summary: An easy to use SQLite package
 Home-page: https://github.com/F1repup650/firepup650-SQL
 License: MIT
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,14 +22,16 @@
 Project-URL: Repository, https://github.com/F1repup650/firepup650-SQL
 Project-URL: Replit, https://replit.com/@Firepup650/firepup650-SQL-Package
 Description-Content-Type: text/markdown
 
 # FPSQL
 An easy to use SQLite package
 #### Change log:
+###### v.1.0.4:
+Fix all mypy stub issues
 ###### v.1.0.3:
 Provide a mypy stub file
 ###### v.1.0.2:
 Fix internal vars
 ###### v.1.0.1:
 Actual release
 ###### v.1.0.0:
```

