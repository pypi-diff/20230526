# Comparing `tmp/fpsql-1.0.1.tar.gz` & `tmp/fpsql-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fpsql-1.0.1.tar", max compression
+gzip compressed data, was "fpsql-1.0.2.tar", max compression
```

## Comparing `fpsql-1.0.1.tar` & `fpsql-1.0.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1072 2021-11-16 19:34:41.532794 fpsql-1.0.1/LICENSE
--rw-r--r--   0        0        0      162 2023-05-17 19:07:09.401248 fpsql-1.0.1/README.md
--rw-r--r--   0        0        0      864 2023-05-17 19:05:38.885295 fpsql-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     5014 2023-05-17 19:07:39.225232 fpsql-1.0.1/src/fpsql/__init__.py
--rw-r--r--   0        0        0     1237 1970-01-01 00:00:00.000000 fpsql-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2021-11-16 19:34:41.000000 fpsql-1.0.2/LICENSE
+-rw-r--r--   0        0        0      196 2023-05-25 15:20:48.275538 fpsql-1.0.2/README.md
+-rw-r--r--   0        0        0      864 2023-05-25 15:20:56.547523 fpsql-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4946 2023-05-25 15:22:43.623334 fpsql-1.0.2/src/fpsql/__init__.py
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 fpsql-1.0.2/PKG-INFO
```

### Comparing `fpsql-1.0.1/LICENSE` & `fpsql-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fpsql-1.0.1/pyproject.toml` & `fpsql-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fpsql"
-version = "1.0.1"
+version = "1.0.2"
 authors = ["Firepup650 <firepyp650@gmail.com>"]
 description = "An easy to use SQLite package"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
```

### Comparing `fpsql-1.0.1/src/fpsql/__init__.py` & `fpsql-1.0.2/src/fpsql/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -9,25 +9,27 @@
             + pydoc.text.document(Function)
         )
         return f
 
     return decorator
 
 
-__VERSION__ = "1.0.26"
-__NEW__ = "Adds `remove_prefix` and `remove_suffix`, name mangles internal variables in `sql`, fixes a bug in `console.warn`, adds `__VERSION__`, `__NEW__`, and `__LICENSE__`, adds many aliases for interactive help."
+__VERSION__ = "1.0.2"
+__NEW__ = "Fix internal vars"
 __LICENSE__ = "MIT"
 
 
 class sql:
-    def addTable(self, tableName: str) -> None:
+    def addTable(self, tableName: str, mode: int = 0, address: str = "") -> None:
         """# Function: sql.addTable
           Adds a table to the database
         # Inputs:
           tableName: str - The name of the table to create
+          mode: int - Not yet implemented
+          address: str - Not yet implemented
 
         # Returns:
           None
 
         # Raises:
           None"""
         self.__con.execute(
@@ -138,15 +140,15 @@
             raise AttributeError("Attempted to delete from unset table")
         if self.get(name):
             self.__con.execute(
                 f"""DELETE FROM "{self.__table}" WHERE name = ?""", (name,)
             )
             self.__con.commit()
 
-    def delete_all(self) -> None:
+    def deleteAll(self) -> None:
         """# Function: sql.delete_all
           Deletes all keys from the table
         # Inputs:
           None
 
         # Returns:
           None
```

### Comparing `fpsql-1.0.1/PKG-INFO` & `fpsql-1.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fpsql
-Version: 1.0.1
+Version: 1.0.2
 Summary: An easy to use SQLite package
 Home-page: https://github.com/F1repup650/firepup650-SQL
 License: MIT
 Author: Firepup650
 Author-email: firepyp650@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -23,13 +23,15 @@
 Project-URL: Repository, https://github.com/F1repup650/firepup650-SQL
 Project-URL: Replit, https://replit.com/@Firepup650/firepup650-SQL-Package
 Description-Content-Type: text/markdown
 
 # FPSQL
 An easy to use SQLite package
 #### Change log:
+###### v.1.0.2:
+Fix internal vars
 ###### v.1.0.1:
 Actual release
 ###### v.1.0.0:
 Initial Release!
 ###### v.1.0.26:
 Mistake release :facepalm:
```

