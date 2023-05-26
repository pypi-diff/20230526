# Comparing `tmp/configzen-0.1.38.tar.gz` & `tmp/configzen-0.1.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.38.tar", max compression
+gzip compressed data, was "configzen-0.1.39.tar", max compression
```

## Comparing `configzen-0.1.38.tar` & `configzen-0.1.39.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.38/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.38/configzen/__main__.py
--rw-r--r--   0        0        0    58282 2023-05-26 07:03:59.357753 configzen-0.1.38/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.38/configzen/errors.py
--rw-r--r--   0        0        0    20467 2023-05-26 09:17:50.644456 configzen-0.1.38/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.38/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.38/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.38/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-26 09:18:14.841319 configzen-0.1.38/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.38/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.38/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.39/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.39/configzen/__main__.py
+-rw-r--r--   0        0        0    58387 2023-05-26 09:30:03.180364 configzen-0.1.39/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.39/configzen/errors.py
+-rw-r--r--   0        0        0    20675 2023-05-26 09:30:03.156364 configzen-0.1.39/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.39/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.39/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.39/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-26 09:30:23.047340 configzen-0.1.39/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.39/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.39/PKG-INFO
```

### Comparing `configzen-0.1.38/configzen/__main__.py` & `configzen-0.1.39/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.38/configzen/config.py` & `configzen-0.1.39/configzen/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,14 +432,15 @@
     ValueError
     """
 
     _resource: NormalizedResourceT
     processor_class: type[Processor[ConfigModelT]]
     ac_parser: str | None
     create_if_missing: bool
+    relative: bool = False
     allowed_url_schemes: set[str]
     use_pydantic_json: bool = True
     global_load_options: dict[str, Any] = {}
     global_dump_options: dict[str, Any] = {
         # These are usually desirable for configuration files.
         # If you want to change them, you can do so by monkey-patching
         # these variables. You can also change `load_options` and
@@ -515,14 +516,16 @@
         if (
             isinstance(resource, (str, os.PathLike))
             and not (
                 isinstance(resource, str)
                 and urllib.parse.urlparse(str(resource)).scheme in _URL_SCHEMES
             )
         ):
+            if resource.startwsith("."):
+                self.relative = True
             resource = pathlib.Path(resource)
 
         self.resource = resource
         self.create_if_missing = create_if_missing
         self.use_pydantic_json = kwargs.pop("use_pydantic_json", True)
         self.default_kwargs = kwargs.pop(
             "default_kwargs", self.predefined_default_kwargs.copy()
```

### Comparing `configzen-0.1.38/configzen/errors.py` & `configzen-0.1.39/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.38/configzen/processor.py` & `configzen-0.1.39/configzen/processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import copy
 import dataclasses
 import enum
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
 
 from anyconfig.utils import is_dict_like, is_list_like
 
@@ -584,15 +585,20 @@
         )
 
         if loader.resource == self.loader.resource:
             raise ConfigPreprocessingError(
                 f"{loader.resource} tried to {ctx.directive!r} on itself"
             )
 
-        with loader.processor_open_resource() as reader:
+        actual_loader = loader
+        if loader.relative:
+            actual_loader = copy.copy(loader)
+            actual_loader.resource = self.loader.resource.parent / loader.resource
+
+        with actual_loader.processor_open_resource() as reader:
             substituted = loader.load_into_dict(reader.read(), preprocess=preprocess)
 
         if substitution_route:
             substituted = at(substituted, substitution_route, loader=loader)
             if not is_dict_like(substituted):
                 raise ConfigPreprocessingError(
                     f"imported item {substitution_route!r} "
```

### Comparing `configzen-0.1.38/configzen/typedefs.py` & `configzen-0.1.39/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.38/LICENSE` & `configzen-0.1.39/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.38/pyproject.toml` & `configzen-0.1.39/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.38"
+version = "0.1.39"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.38/README.md` & `configzen-0.1.39/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.38/PKG-INFO` & `configzen-0.1.39/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.38
+Version: 0.1.39
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

