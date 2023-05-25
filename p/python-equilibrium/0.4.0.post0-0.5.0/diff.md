# Comparing `tmp/python_equilibrium-0.4.0.post0.tar.gz` & `tmp/python_equilibrium-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.4.0.post0.tar", max compression
+gzip compressed data, was "python_equilibrium-0.5.0.tar", max compression
```

## Comparing `python_equilibrium-0.4.0.post0.tar` & `python_equilibrium-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.4.0.post0/LICENSE
--rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.4.0.post0/README.md
--rw-r--r--   0        0        0     1615 2023-05-19 09:28:12.252441 python_equilibrium-0.4.0.post0/pyproject.toml
--rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/AdmissionController.py
--rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/CrudResourceController.py
--rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/JsonResourceStore.py
--rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/JsonResourceStore_test.py
--rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/Namespace.py
--rw-r--r--   0        0        0    13234 2023-05-16 21:15:49.967795 python_equilibrium-0.4.0.post0/src/equilibrium/Resource.py
--rw-r--r--   0        0        0    15427 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/ResourceContext.py
--rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/ResourceController.py
--rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/ResourceStore.py
--rw-r--r--   0        0        0     2189 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/Resource_test.py
--rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.4.0.post0/src/equilibrium/Service.py
--rw-r--r--   0        0        0     1051 2023-05-19 09:28:12.252441 python_equilibrium-0.4.0.post0/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.4.0.post0/src/equilibrium/py.typed
--rw-r--r--   0        0        0     2343 1970-01-01 00:00:00.000000 python_equilibrium-0.4.0.post0/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.5.0/LICENSE
+-rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.5.0/README.md
+-rw-r--r--   0        0        0     1661 2023-05-25 22:03:29.008781 python_equilibrium-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/AdmissionController.py
+-rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/CrudResourceController.py
+-rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/JsonResourceStore.py
+-rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/Namespace.py
+-rw-r--r--   0        0        0    13234 2023-05-16 21:15:49.967795 python_equilibrium-0.5.0/src/equilibrium/Resource.py
+-rw-r--r--   0        0        0    15825 2023-05-25 22:02:39.509291 python_equilibrium-0.5.0/src/equilibrium/ResourceContext.py
+-rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/ResourceController.py
+-rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/ResourceStore.py
+-rw-r--r--   0        0        0     2189 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/Resource_test.py
+-rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.5.0/src/equilibrium/Service.py
+-rw-r--r--   0        0        0     1045 2023-05-25 22:03:29.008781 python_equilibrium-0.5.0/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.5.0/src/equilibrium/py.typed
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.5.0/PKG-INFO
```

### Comparing `python_equilibrium-0.4.0.post0/LICENSE` & `python_equilibrium-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/README.md` & `python_equilibrium-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/pyproject.toml` & `python_equilibrium-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.4.0.post0"
+version = "0.5.0"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/NiklasRosenstein/python-equilibrium/issues"
 # Documentation = ""
-# Homepage = ""
+Homepage = "https://github.com/NiklasRosenstein/python-equilibrium"
 Repository = "https://github.com/NiklasRosenstein/python-equilibrium"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 "databind.json" = "^4.2.5"
 pyyaml = "^6.0"
 types-pyyaml = "^6.0.12.9"
```

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/AdmissionController.py` & `python_equilibrium-0.5.0/src/equilibrium/AdmissionController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/CrudResourceController.py` & `python_equilibrium-0.5.0/src/equilibrium/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/JsonResourceStore.py` & `python_equilibrium-0.5.0/src/equilibrium/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/JsonResourceStore_test.py` & `python_equilibrium-0.5.0/src/equilibrium/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/Namespace.py` & `python_equilibrium-0.5.0/src/equilibrium/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/Resource.py` & `python_equilibrium-0.5.0/src/equilibrium/Resource.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/ResourceContext.py` & `python_equilibrium-0.5.0/src/equilibrium/ResourceContext.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,16 +140,29 @@
         if resource_type.apiVersion not in self._resource_types:
             return False
         return resource_type.kind in self._resource_types[resource_type.apiVersion]
 
     def register(self, spec_type: type[Resource.Spec]) -> None:
         self._resource_types.setdefault(spec_type.API_VERSION, {})[spec_type.KIND] = spec_type
 
-    def get(self, resource_type: Resource.Type) -> type[Resource.Spec] | None:
-        return self._resource_types.get(resource_type.apiVersion, {}).get(resource_type.kind)
+    @overload
+    def get(self, resource_type: Resource.Type) -> type[Resource.Spec]:
+        ...
+
+    @overload
+    def get(self, resource_type: Resource.Type, default: T) -> type[Resource.Spec] | T:
+        ...
+
+    def get(self, resource_type: Resource.Type, default: T | NotSet = NotSet.Value) -> type[Resource.Spec] | T:
+        try:
+            return self._resource_types.get(resource_type.apiVersion, {})[resource_type.kind]
+        except KeyError:
+            if default is NotSet.Value:
+                raise KeyError(resource_type)
+            return default
 
 
 class ServiceRegistry(Service.Provider):
     def __init__(self, resources: ResourceStore) -> None:
         self._resources = resources
         self._services: dict[Resource.Type, dict[Service.Id, Service]] = {}
```

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/ResourceStore.py` & `python_equilibrium-0.5.0/src/equilibrium/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/Resource_test.py` & `python_equilibrium-0.5.0/src/equilibrium/Resource_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/Service.py` & `python_equilibrium-0.5.0/src/equilibrium/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.4.0.post0/src/equilibrium/__init__.py` & `python_equilibrium-0.5.0/src/equilibrium/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     "ResourceRegistry",
     "ResourceStore",
     "ResourceTypeRegistry",
     "Service",
     "ServiceRegistry",
 ]
 
-__version__ = "0.4.0.post0"
+__version__ = "0.5.0"
```

### Comparing `python_equilibrium-0.4.0.post0/PKG-INFO` & `python_equilibrium-0.5.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.4.0.post0
+Version: 0.5.0
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: databind.json (>=4.2.5,<5.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
 Requires-Dist: types-pyyaml (>=6.0.12.9,<7.0.0.0)
 Project-URL: Bug Tracker, https://github.com/NiklasRosenstein/python-equilibrium/issues
+Project-URL: Homepage, https://github.com/NiklasRosenstein/python-equilibrium
 Project-URL: Repository, https://github.com/NiklasRosenstein/python-equilibrium
 Description-Content-Type: text/markdown
 
 # equilibrium
 
 > __Equilibrium__ _(noun)_: A state in which opposing forces or influences are balanced, resulting in a stable system
 > that does not undergo significant changes. In a broader sense, equilibrium can refer to a state of mental or emotional
```

