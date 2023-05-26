# Comparing `tmp/python_equilibrium-0.5.0.tar.gz` & `tmp/python_equilibrium-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.5.0.tar", max compression
+gzip compressed data, was "python_equilibrium-0.5.1.tar", max compression
```

## Comparing `python_equilibrium-0.5.0.tar` & `python_equilibrium-0.5.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.5.0/LICENSE
--rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.5.0/README.md
--rw-r--r--   0        0        0     1661 2023-05-25 22:03:29.008781 python_equilibrium-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/AdmissionController.py
--rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/CrudResourceController.py
--rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/JsonResourceStore.py
--rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/JsonResourceStore_test.py
--rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/Namespace.py
--rw-r--r--   0        0        0    13234 2023-05-16 21:15:49.967795 python_equilibrium-0.5.0/src/equilibrium/Resource.py
--rw-r--r--   0        0        0    15825 2023-05-25 22:02:39.509291 python_equilibrium-0.5.0/src/equilibrium/ResourceContext.py
--rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/ResourceController.py
--rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/ResourceStore.py
--rw-r--r--   0        0        0     2189 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/Resource_test.py
--rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/Service.py
--rw-r--r--   0        0        0     1045 2023-05-25 22:03:29.008781 python_equilibrium-0.5.0/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.5.0/src/equilibrium/py.typed
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.5.1/LICENSE
+-rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.5.1/README.md
+-rw-r--r--   0        0        0     1661 2023-05-26 17:38:02.058474 python_equilibrium-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/AdmissionController.py
+-rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/CrudResourceController.py
+-rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/JsonResourceStore.py
+-rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/Namespace.py
+-rw-r--r--   0        0        0    13208 2023-05-26 17:37:05.744389 python_equilibrium-0.5.1/src/equilibrium/Resource.py
+-rw-r--r--   0        0        0    15825 2023-05-25 22:02:39.509291 python_equilibrium-0.5.1/src/equilibrium/ResourceContext.py
+-rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/ResourceController.py
+-rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/ResourceStore.py
+-rw-r--r--   0        0        0     2189 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/Resource_test.py
+-rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/Service.py
+-rw-r--r--   0        0        0     1045 2023-05-26 17:38:02.058474 python_equilibrium-0.5.1/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.5.1/src/equilibrium/py.typed
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.5.1/PKG-INFO
```

### Comparing `python_equilibrium-0.5.0/LICENSE` & `python_equilibrium-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/README.md` & `python_equilibrium-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/pyproject.toml` & `python_equilibrium-0.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.5.0"
+version = "0.5.1"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_equilibrium-0.5.0/src/equilibrium/AdmissionController.py` & `python_equilibrium-0.5.1/src/equilibrium/AdmissionController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/CrudResourceController.py` & `python_equilibrium-0.5.1/src/equilibrium/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/JsonResourceStore.py` & `python_equilibrium-0.5.1/src/equilibrium/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/JsonResourceStore_test.py` & `python_equilibrium-0.5.1/src/equilibrium/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/Namespace.py` & `python_equilibrium-0.5.1/src/equilibrium/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/Resource.py` & `python_equilibrium-0.5.1/src/equilibrium/Resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,19 @@
 
 
 @dataclass
 class Resource(Generic[T]):
     class Error(Exception):
         pass
 
-    @dataclass(frozen=True)
+    @dataclass
     class NotFound(Error):
         uri: Resource.URI
 
-    @dataclass(frozen=True)
+    @dataclass
     class ValidationFailed(Error):
         uri: Resource.URI
         exc: Exception
 
     @dataclass
     class AdmissionFailed(Error):
         uri: Resource.URI
```

### Comparing `python_equilibrium-0.5.0/src/equilibrium/ResourceContext.py` & `python_equilibrium-0.5.1/src/equilibrium/ResourceContext.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/ResourceStore.py` & `python_equilibrium-0.5.1/src/equilibrium/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/Resource_test.py` & `python_equilibrium-0.5.1/src/equilibrium/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/Service.py` & `python_equilibrium-0.5.1/src/equilibrium/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.0/src/equilibrium/__init__.py` & `python_equilibrium-0.5.1/src/equilibrium/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     "ResourceRegistry",
     "ResourceStore",
     "ResourceTypeRegistry",
     "Service",
     "ServiceRegistry",
 ]
 
-__version__ = "0.5.0"
+__version__ = "0.5.1"
```

### Comparing `python_equilibrium-0.5.0/PKG-INFO` & `python_equilibrium-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.5.0
+Version: 0.5.1
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

