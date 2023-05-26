# Comparing `tmp/python_equilibrium-0.5.1.tar.gz` & `tmp/python_equilibrium-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_equilibrium-0.5.1.tar", max compression
+gzip compressed data, was "python_equilibrium-0.5.2.tar", max compression
```

## Comparing `python_equilibrium-0.5.1.tar` & `python_equilibrium-0.5.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.5.1/LICENSE
--rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.5.1/README.md
--rw-r--r--   0        0        0     1661 2023-05-26 17:38:02.058474 python_equilibrium-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/AdmissionController.py
--rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/CrudResourceController.py
--rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/JsonResourceStore.py
--rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/JsonResourceStore_test.py
--rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/Namespace.py
--rw-r--r--   0        0        0    13208 2023-05-26 17:37:05.744389 python_equilibrium-0.5.1/src/equilibrium/Resource.py
--rw-r--r--   0        0        0    15825 2023-05-25 22:02:39.509291 python_equilibrium-0.5.1/src/equilibrium/ResourceContext.py
--rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/ResourceController.py
--rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/ResourceStore.py
--rw-r--r--   0        0        0     2189 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/Resource_test.py
--rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.5.1/src/equilibrium/Service.py
--rw-r--r--   0        0        0     1045 2023-05-26 17:38:02.058474 python_equilibrium-0.5.1/src/equilibrium/__init__.py
--rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.5.1/src/equilibrium/py.typed
--rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-05-16 21:13:35.338396 python_equilibrium-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1614 2023-05-19 09:27:51.784351 python_equilibrium-0.5.2/README.md
+-rw-r--r--   0        0        0     1661 2023-05-26 17:59:48.314404 python_equilibrium-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      714 2023-05-19 08:58:20.216493 python_equilibrium-0.5.2/src/equilibrium/AdmissionController.py
+-rw-r--r--   0        0        0     8461 2023-05-19 08:58:20.216493 python_equilibrium-0.5.2/src/equilibrium/CrudResourceController.py
+-rw-r--r--   0        0        0    12883 2023-05-19 08:58:20.216493 python_equilibrium-0.5.2/src/equilibrium/JsonResourceStore.py
+-rw-r--r--   0        0        0     8271 2023-05-19 08:58:20.216493 python_equilibrium-0.5.2/src/equilibrium/JsonResourceStore_test.py
+-rw-r--r--   0        0        0      607 2023-05-19 08:58:20.216493 python_equilibrium-0.5.2/src/equilibrium/Namespace.py
+-rw-r--r--   0        0        0    14850 2023-05-26 17:57:31.732913 python_equilibrium-0.5.2/src/equilibrium/Resource.py
+-rw-r--r--   0        0        0    15825 2023-05-25 22:02:39.509291 python_equilibrium-0.5.2/src/equilibrium/ResourceContext.py
+-rw-r--r--   0        0        0      482 2023-05-19 08:58:20.216493 python_equilibrium-0.5.2/src/equilibrium/ResourceController.py
+-rw-r--r--   0        0        0     4831 2023-05-19 08:58:20.216493 python_equilibrium-0.5.2/src/equilibrium/ResourceStore.py
+-rw-r--r--   0        0        0     4202 2023-05-26 17:59:04.238639 python_equilibrium-0.5.2/src/equilibrium/Resource_test.py
+-rw-r--r--   0        0        0     3028 2023-05-19 08:58:20.216493 python_equilibrium-0.5.2/src/equilibrium/Service.py
+-rw-r--r--   0        0        0     1045 2023-05-26 17:59:48.314404 python_equilibrium-0.5.2/src/equilibrium/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 21:13:35.338396 python_equilibrium-0.5.2/src/equilibrium/py.typed
+-rw-r--r--   0        0        0     2415 1970-01-01 00:00:00.000000 python_equilibrium-0.5.2/PKG-INFO
```

### Comparing `python_equilibrium-0.5.1/LICENSE` & `python_equilibrium-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/README.md` & `python_equilibrium-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/pyproject.toml` & `python_equilibrium-0.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "python-equilibrium"
-version = "0.5.1"
+version = "0.5.2"
 description = ""
 authors = ["Niklas Rosenstein <rosensteinniklas@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "equilibrium", from = "src" }]
 classifiers = []
 keywords = []
```

### Comparing `python_equilibrium-0.5.1/src/equilibrium/AdmissionController.py` & `python_equilibrium-0.5.2/src/equilibrium/AdmissionController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/src/equilibrium/CrudResourceController.py` & `python_equilibrium-0.5.2/src/equilibrium/CrudResourceController.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/src/equilibrium/JsonResourceStore.py` & `python_equilibrium-0.5.2/src/equilibrium/JsonResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/src/equilibrium/JsonResourceStore_test.py` & `python_equilibrium-0.5.2/src/equilibrium/JsonResourceStore_test.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/src/equilibrium/Namespace.py` & `python_equilibrium-0.5.2/src/equilibrium/Namespace.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/src/equilibrium/Resource.py` & `python_equilibrium-0.5.2/src/equilibrium/Resource.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,43 +11,54 @@
 from typing_extensions import Self  # 3.11+
 
 __all__ = ["Resource", "match_labels", "validate_api_version", "validate_identifier"]
 
 T = TypeVar("T")
 
 VALID_IDENTIFIER_REGEX = r"^[a-zA-Z0-9]([-a-zA-Z0-9]*[a-zA-Z0-9])?$"
-VALID_APIVERSION_REGEX = r"^[\.a-z0-9]([-\.a-z0-9]*[\.a-z0-9])?(/[\.a-z0-9]([-\.a-z0-9]*[\.a-z0-9])?)*$"
+VALID_APIVERSION_GROUP_REGEX = r"^[\.a-z0-9]([-\.a-z0-9]*[\.a-z0-9])?$"
+VALID_APIVERSION_VERSION_REGEX = r"^v[0-9]([-a-z0-9]*[a-z0-9])?$"
 
 
 class Dataclass(Protocol):
     __dataclass_fields__: Mapping[str, Any]
 
 
 def validate_identifier(s: str, name: str) -> None:
     assert isinstance(s, str), type(s)
     if not re.match(VALID_IDENTIFIER_REGEX, s):
         raise ValueError(f"invalid {name}: {s!r}")
 
 
 def validate_api_version(s: str, name: str) -> None:
     assert isinstance(s, str), type(s)
-    if not re.match(VALID_APIVERSION_REGEX, s):
-        raise ValueError(f"invalid {name}: {s!r}")
+    parts = s.split("/")
+    match parts:
+        case [group, version]:
+            if not re.match(VALID_APIVERSION_GROUP_REGEX, group):
+                raise ValueError(f"invalid {name}: {s!r}")
+            if not re.match(VALID_APIVERSION_VERSION_REGEX, version):
+                raise ValueError(f"invalid {name}: {s!r}")
+        case [version]:
+            if not re.match(VALID_APIVERSION_VERSION_REGEX, version):
+                raise ValueError(f"invalid {name}: {s!r}")
+        case _:
+            raise ValueError(f"invalid {name}: {s!r}")
 
 
 @dataclass
 class Resource(Generic[T]):
     class Error(Exception):
         pass
 
-    @dataclass
+    @dataclass(frozen=True)
     class NotFound(Error):
         uri: Resource.URI
 
-    @dataclass
+    @dataclass(frozen=True)
     class ValidationFailed(Error):
         uri: Resource.URI
         exc: Exception
 
     @dataclass
     class AdmissionFailed(Error):
         uri: Resource.URI
@@ -125,14 +136,20 @@
     GenericSpec = dict[str, Any]
     GenericState = dict[str, Any]
 
     @JsonConverter.using_classmethods(serialize="__str__", deserialize="of")
     @total_ordering
     @dataclass(frozen=True)
     class URI:
+        """
+        Represents unique resource identifiers. The `apiVersion` must consist of a `group` and a `version` formatted
+        as `group/version`. It is also acceptable to omit the `group` and have an `apiVersion` that is just a `version`.
+        The `version` component must begin with a `v` followed by a number (e.g. `v1`, `v2beta1`, `v1alpha1`, etc.).
+        """
+
         apiVersion: str
         kind: str
         namespace: str | None
         name: str
 
         def __post_init__(self) -> None:
             validate_api_version(self.apiVersion, "apiVersion")
@@ -152,22 +169,41 @@
                 return str(self) < str(other)
             else:
                 return NotImplemented
 
         @staticmethod
         def of(s: str) -> Resource.URI:
             parts = s.split("/")
-            try:
-                apiVersion = "/".join(parts[:-3])
-                kind = parts[-3]
-                namespace = parts[-2] or None
-                name = parts[-1]
-            except IndexError:
+
+            if len(parts) < 3:
                 raise ValueError(f"invalid Resource.URI: {s!r}")
-            return Resource.URI(apiVersion, kind, namespace, name)
+
+            # Determine if URI is using a `group/version` or just `version`` format.
+            try:
+                apiVersion = parts[0] + "/" + parts[1]
+                validate_api_version(apiVersion, "apiVersion component")
+                remainder = parts[2:]
+            except ValueError:
+                try:
+                    apiVersion = parts[0]
+                    validate_api_version(apiVersion, "apiVersion component")
+                    remainder = parts[1:]
+                except ValueError:
+                    raise ValueError(f"invalid Resource.URI: has invalid apiVersion component: {s!r}")
+
+            namespace: str | None
+            match remainder:
+                case [kind, namespace, name]:
+                    pass
+                case [kind, name]:
+                    namespace = None
+                case _:
+                    raise ValueError(f"invalid Resource.URI: {s!r}")
+
+            return Resource.URI(apiVersion, kind, namespace or None, name)
 
         @property
         def type(self) -> Resource.Type:
             return Resource.Type(self.apiVersion, self.kind)
 
         @property
         def locator(self) -> Resource.Locator:
```

### Comparing `python_equilibrium-0.5.1/src/equilibrium/ResourceContext.py` & `python_equilibrium-0.5.2/src/equilibrium/ResourceContext.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/src/equilibrium/ResourceStore.py` & `python_equilibrium-0.5.2/src/equilibrium/ResourceStore.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/src/equilibrium/Service.py` & `python_equilibrium-0.5.2/src/equilibrium/Service.py`

 * *Files identical despite different names*

### Comparing `python_equilibrium-0.5.1/src/equilibrium/__init__.py` & `python_equilibrium-0.5.2/src/equilibrium/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,8 +30,8 @@
     "ResourceRegistry",
     "ResourceStore",
     "ResourceTypeRegistry",
     "Service",
     "ServiceRegistry",
 ]
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
```

### Comparing `python_equilibrium-0.5.1/PKG-INFO` & `python_equilibrium-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-equilibrium
-Version: 0.5.1
+Version: 0.5.2
 Summary: 
 License: MIT
 Author: Niklas Rosenstein
 Author-email: rosensteinniklas@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

