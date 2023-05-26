# Comparing `tmp/sqlalchemy-access-2.0.1.tar.gz` & `tmp/sqlalchemy-access-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy-access-2.0.1.tar", last modified: Tue Feb  7 17:30:41 2023, max compression
+gzip compressed data, was "sqlalchemy-access-2.0.2.tar", last modified: Fri May 26 16:21:52 2023, max compression
```

## Comparing `sqlalchemy-access-2.0.1.tar` & `sqlalchemy-access-2.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-02-07 17:30:41.710818 sqlalchemy-access-2.0.1/
--rw-rw-rw-   0        0        0      563 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.1/AUTHORS
--rw-rw-rw-   0        0        0     1117 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.1/LICENSE
--rw-rw-rw-   0        0        0      489 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     4175 2023-02-07 17:30:41.710818 sqlalchemy-access-2.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     3204 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.1/README.rst
--rw-rw-rw-   0        0        0      742 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.1/README.testing.rst
--rw-rw-rw-   0        0        0      251 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      649 2023-02-07 17:30:41.710818 sqlalchemy-access-2.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1713 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-07 17:30:41.650423 sqlalchemy-access-2.0.1/sqlalchemy_access/
--rw-rw-rw-   0        0        0      523 2023-02-07 17:30:03.000000 sqlalchemy-access-2.0.1/sqlalchemy_access/__init__.py
--rw-rw-rw-   0        0        0    26363 2023-02-07 17:26:58.000000 sqlalchemy-access-2.0.1/sqlalchemy_access/base.py
--rw-rw-rw-   0        0        0     3505 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.1/sqlalchemy_access/pyodbc.py
--rw-rw-rw-   0        0        0     2195 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.1/sqlalchemy_access/requirements.py
-drwxrwxrwx   0        0        0        0 2023-02-07 17:30:41.681686 sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/
--rw-rw-rw-   0        0        0     4175 2023-02-07 17:30:40.000000 sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      572 2023-02-07 17:30:40.000000 sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-07 17:30:40.000000 sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-02-07 17:30:40.000000 sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2022-02-03 23:58:04.000000 sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       41 2023-02-07 17:30:40.000000 sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-02-07 17:30:40.000000 sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-02-07 17:30:41.710818 sqlalchemy-access-2.0.1/test/
--rw-rw-rw-   0        0        0        0 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.1/test/__init__.py
--rw-rw-rw-   0        0        0      278 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.1/test/conftest.py
--rw-rw-rw-   0        0        0      757 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.1/test/test_operator.py
--rw-rw-rw-   0        0        0    12712 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.1/test/test_suite.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:21:52.661877 sqlalchemy-access-2.0.2/
+-rw-rw-rw-   0        0        0      563 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.2/AUTHORS
+-rw-rw-rw-   0        0        0     1117 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.2/LICENSE
+-rw-rw-rw-   0        0        0      489 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     4175 2023-05-26 16:21:52.661877 sqlalchemy-access-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3204 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.2/README.rst
+-rw-rw-rw-   0        0        0      742 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.2/README.testing.rst
+-rw-rw-rw-   0        0        0      251 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      649 2023-05-26 16:21:52.661877 sqlalchemy-access-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1713 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:21:52.458704 sqlalchemy-access-2.0.2/sqlalchemy_access/
+-rw-rw-rw-   0        0        0      523 2023-05-26 16:19:47.000000 sqlalchemy-access-2.0.2/sqlalchemy_access/__init__.py
+-rw-rw-rw-   0        0        0    26451 2023-05-26 16:15:10.000000 sqlalchemy-access-2.0.2/sqlalchemy_access/base.py
+-rw-rw-rw-   0        0        0     3505 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.2/sqlalchemy_access/pyodbc.py
+-rw-rw-rw-   0        0        0     2195 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.2/sqlalchemy_access/requirements.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:21:52.583706 sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/
+-rw-rw-rw-   0        0        0     4175 2023-05-26 16:21:49.000000 sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      572 2023-05-26 16:21:49.000000 sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 16:21:49.000000 sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-05-26 16:21:49.000000 sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2022-02-03 23:58:04.000000 sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       41 2023-05-26 16:21:49.000000 sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-26 16:21:49.000000 sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 16:21:52.646251 sqlalchemy-access-2.0.2/test/
+-rw-rw-rw-   0        0        0        0 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.2/test/__init__.py
+-rw-rw-rw-   0        0        0      278 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.2/test/conftest.py
+-rw-rw-rw-   0        0        0      757 2022-02-03 23:56:47.000000 sqlalchemy-access-2.0.2/test/test_operator.py
+-rw-rw-rw-   0        0        0    12712 2023-01-30 15:16:49.000000 sqlalchemy-access-2.0.2/test/test_suite.py
```

### Comparing `sqlalchemy-access-2.0.1/AUTHORS` & `sqlalchemy-access-2.0.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/LICENSE` & `sqlalchemy-access-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/PKG-INFO` & `sqlalchemy-access-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-access
-Version: 2.0.1
+Version: 2.0.2
 Summary: MS Access for SQLAlchemy
 Home-page: https://github.com/gordthompson/sqlalchemy-access
 Author: Gord Thompson
 Author-email: gord@gordthompson.com
 License: MIT
 Project-URL: Documentation, https://github.com/gordthompson/sqlalchemy-access/wiki
 Project-URL: Source, https://github.com/gordthompson/sqlalchemy-access
```

### Comparing `sqlalchemy-access-2.0.1/README.rst` & `sqlalchemy-access-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/README.testing.rst` & `sqlalchemy-access-2.0.2/README.testing.rst`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/setup.cfg` & `sqlalchemy-access-2.0.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/setup.py` & `sqlalchemy-access-2.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/sqlalchemy_access/__init__.py` & `sqlalchemy-access-2.0.2/sqlalchemy_access/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,13 +16,13 @@
     ShortText,
     Single,
     YesNo,
 )
 
 import pyodbc
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 
 pyodbc.pooling = False  # required for Access databases with ODBC linked tables
 _registry.register(
     "access.pyodbc", "sqlalchemy_access.pyodbc", "AccessDialect_pyodbc"
 )
```

### Comparing `sqlalchemy-access-2.0.1/sqlalchemy_access/base.py` & `sqlalchemy-access-2.0.2/sqlalchemy_access/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -279,15 +279,18 @@
         If we need to store BIGINT values we can use a Decimal column. Examples here:
         https://github.com/gordthompson/sqlalchemy-access/wiki/%5Bpandas%5D-working-with-64-bit-integer-(BIGINT)-values
         """
         return LongInteger.__visit_name__
 
     def visit_BOOLEAN(self, type_, **kw):
         return YESNO.__visit_name__
-
+    
+    def visit_YESNO(self, type_, **kw):
+        return YESNO.__visit_name__
+    
     def visit_COUNTER(self, type_, **kw):
         return COUNTER.__visit_name__
 
     def visit_CURRENCY(self, type_, **kw):
         return CURRENCY.__visit_name__
 
     def visit_GUID(self, type_, **kw):
```

### Comparing `sqlalchemy-access-2.0.1/sqlalchemy_access/pyodbc.py` & `sqlalchemy-access-2.0.2/sqlalchemy_access/pyodbc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/sqlalchemy_access/requirements.py` & `sqlalchemy-access-2.0.2/sqlalchemy_access/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/PKG-INFO` & `sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-access
-Version: 2.0.1
+Version: 2.0.2
 Summary: MS Access for SQLAlchemy
 Home-page: https://github.com/gordthompson/sqlalchemy-access
 Author: Gord Thompson
 Author-email: gord@gordthompson.com
 License: MIT
 Project-URL: Documentation, https://github.com/gordthompson/sqlalchemy-access/wiki
 Project-URL: Source, https://github.com/gordthompson/sqlalchemy-access
```

### Comparing `sqlalchemy-access-2.0.1/sqlalchemy_access.egg-info/SOURCES.txt` & `sqlalchemy-access-2.0.2/sqlalchemy_access.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/test/test_operator.py` & `sqlalchemy-access-2.0.2/test/test_operator.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy-access-2.0.1/test/test_suite.py` & `sqlalchemy-access-2.0.2/test/test_suite.py`

 * *Files identical despite different names*

