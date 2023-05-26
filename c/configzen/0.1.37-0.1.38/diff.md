# Comparing `tmp/configzen-0.1.37.tar.gz` & `tmp/configzen-0.1.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configzen-0.1.37.tar", max compression
+gzip compressed data, was "configzen-0.1.38.tar", max compression
```

## Comparing `configzen-0.1.37.tar` & `configzen-0.1.38.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.37/configzen/__init__.py
--rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.37/configzen/__main__.py
--rw-r--r--   0        0        0    58282 2023-05-26 07:03:59.357753 configzen-0.1.37/configzen/config.py
--rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.37/configzen/errors.py
--rw-r--r--   0        0        0    20832 2023-05-26 06:54:52.263087 configzen-0.1.37/configzen/processor.py
--rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.37/configzen/py.typed
--rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.37/configzen/typedefs.py
--rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.37/LICENSE
--rw-r--r--   0        0        0     1687 2023-05-26 07:04:54.911332 configzen-0.1.37/pyproject.toml
--rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.37/README.md
--rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.37/PKG-INFO
+-rw-r--r--   0        0        0      216 2023-05-17 21:14:40.122071 configzen-0.1.38/configzen/__init__.py
+-rw-r--r--   0        0        0      904 2023-05-19 14:41:10.408896 configzen-0.1.38/configzen/__main__.py
+-rw-r--r--   0        0        0    58282 2023-05-26 07:03:59.357753 configzen-0.1.38/configzen/config.py
+-rw-r--r--   0        0        0     2470 2023-05-19 16:49:24.141768 configzen-0.1.38/configzen/errors.py
+-rw-r--r--   0        0        0    20467 2023-05-26 09:17:50.644456 configzen-0.1.38/configzen/processor.py
+-rw-r--r--   0        0        0        0 2023-05-14 03:53:55.304547 configzen-0.1.38/configzen/py.typed
+-rw-r--r--   0        0        0      850 2023-05-26 07:00:32.774025 configzen-0.1.38/configzen/typedefs.py
+-rw-r--r--   0        0        0     1083 2023-04-05 18:05:38.524615 configzen-0.1.38/LICENSE
+-rw-r--r--   0        0        0     1687 2023-05-26 09:18:14.841319 configzen-0.1.38/pyproject.toml
+-rw-r--r--   0        0        0     7150 2023-05-19 22:44:45.534902 configzen-0.1.38/README.md
+-rw-r--r--   0        0        0     7841 1970-01-01 00:00:00.000000 configzen-0.1.38/PKG-INFO
```

### Comparing `configzen-0.1.37/configzen/__main__.py` & `configzen-0.1.38/configzen/__main__.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.37/configzen/config.py` & `configzen-0.1.38/configzen/config.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.37/configzen/errors.py` & `configzen-0.1.38/configzen/errors.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.37/configzen/processor.py` & `configzen-0.1.38/configzen/processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from __future__ import annotations
 
 import dataclasses
 import enum
-import pathlib
 from collections.abc import Callable
 from typing import TYPE_CHECKING, Any, ClassVar, Generic, TypedDict, TypeVar, cast
 
 from anyconfig.utils import is_dict_like, is_list_like
 
 from configzen.errors import (
     ConfigPreprocessingError,
@@ -585,22 +584,14 @@
         )
 
         if loader.resource == self.loader.resource:
             raise ConfigPreprocessingError(
                 f"{loader.resource} tried to {ctx.directive!r} on itself"
             )
 
-        if (
-            isinstance(loader.resource, pathlib.Path)
-            and not loader.resource.is_absolute()
-        ):
-            orig_resource = self.loader.resource
-            if isinstance(orig_resource, pathlib.Path) and orig_resource.is_absolute():
-                loader.resource = loader.resource.relative_to(orig_resource.parent)
-
         with loader.processor_open_resource() as reader:
             substituted = loader.load_into_dict(reader.read(), preprocess=preprocess)
 
         if substitution_route:
             substituted = at(substituted, substitution_route, loader=loader)
             if not is_dict_like(substituted):
                 raise ConfigPreprocessingError(
```

### Comparing `configzen-0.1.37/configzen/typedefs.py` & `configzen-0.1.38/configzen/typedefs.py`

 * *Files identical despite different names*

### Comparing `configzen-0.1.37/LICENSE` & `configzen-0.1.38/LICENSE`

 * *Files identical despite different names*

### Comparing `configzen-0.1.37/pyproject.toml` & `configzen-0.1.38/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "configzen"
-version = "0.1.37"
+version = "0.1.38"
 description = "The easiest way to manage configuration files in Python"
 authors = ["bswck <bswck.dev@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `configzen-0.1.37/README.md` & `configzen-0.1.38/README.md`

 * *Files identical despite different names*

### Comparing `configzen-0.1.37/PKG-INFO` & `configzen-0.1.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: configzen
-Version: 0.1.37
+Version: 0.1.38
 Summary: The easiest way to manage configuration files in Python
 License: MIT
 Author: bswck
 Author-email: bswck.dev@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

