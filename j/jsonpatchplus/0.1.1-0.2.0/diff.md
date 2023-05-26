# Comparing `tmp/jsonpatchplus-0.1.1.tar.gz` & `tmp/jsonpatchplus-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonpatchplus-0.1.1.tar", last modified: Fri May 26 02:41:02 2023, max compression
+gzip compressed data, was "jsonpatchplus-0.2.0.tar", last modified: Fri May 26 08:27:02 2023, max compression
```

## Comparing `jsonpatchplus-0.1.1.tar` & `jsonpatchplus-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.340405 jsonpatchplus-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 02:41:02.340405 jsonpatchplus-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 02:41:02.340405 jsonpatchplus-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.336405 jsonpatchplus-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.336405 jsonpatchplus-0.1.1/src/jsonpatchplus/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.340405 jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/jsonpatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/jsonpatchplus.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.336405 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:27:02.690194 jsonpatchplus-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 08:27:02.690194 jsonpatchplus-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 08:27:02.690194 jsonpatchplus-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:27:02.690194 jsonpatchplus-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:27:02.690194 jsonpatchplus-0.2.0/src/jsonpatchplus/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:27:02.690194 jsonpatchplus-0.2.0/src/jsonpatchplus/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/loaders/jsonpatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/loaders/jsonpatchplus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:27:02.690194 jsonpatchplus-0.2.0/src/jsonpatchplus/preprocessors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/preprocessors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/preprocessors/jsonpath.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-26 08:26:52.000000 jsonpatchplus-0.2.0/src/jsonpatchplus/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:27:02.690194 jsonpatchplus-0.2.0/src/jsonpatchplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 08:27:02.000000 jsonpatchplus-0.2.0/src/jsonpatchplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-26 08:27:02.000000 jsonpatchplus-0.2.0/src/jsonpatchplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:27:02.000000 jsonpatchplus-0.2.0/src/jsonpatchplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 08:27:02.000000 jsonpatchplus-0.2.0/src/jsonpatchplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 08:27:02.000000 jsonpatchplus-0.2.0/src/jsonpatchplus.egg-info/top_level.txt
```

### Comparing `jsonpatchplus-0.1.1/LICENSE` & `jsonpatchplus-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonpatchplus-0.1.1/PKG-INFO` & `jsonpatchplus-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonpatchplus
-Version: 0.1.1
+Version: 0.2.0
 Summary: JsonPatch+
 Author-email: Elmer Nocon <elmernocon@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Elmer Nocon
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsonpatchplus-0.1.1/src/jsonpatchplus/ctypes.py` & `jsonpatchplus-0.2.0/src/jsonpatchplus/ctypes.py`

 * *Files identical despite different names*

### Comparing `jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/jsonpatch.py` & `jsonpatchplus-0.2.0/src/jsonpatchplus/loaders/jsonpatch.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,30 @@
-import json
+from pathlib import Path
+
+import yaml
 
 from ..ctypes import (
     StringOrFilePath,
     JsonPatchDocument,
     JsonPatchDocumentLoader,
 )
 from ..exceptions import JsonPatchInvalidError
 
 
 class Loader:
     def __call__(self, s_or_fp: StringOrFilePath, /, **kwargs) -> JsonPatchDocument:
-        if isinstance(s_or_fp, (bytes, str)):
-            result = json.loads(s_or_fp, **kwargs)
-        else:
-            result = json.load(s_or_fp, **kwargs)
+        if not isinstance(s_or_fp, (bytes, str)):
+            kwargs.setdefault("encoding", "utf-8")
+            kwargs.setdefault("errors", "ignore")
+            s_or_fp = Path(s_or_fp).read_text(**kwargs)
+
+        if not isinstance(s_or_fp, str):
+            raise JsonPatchInvalidError()
+
+        result = yaml.safe_load(s_or_fp)
 
         if not isinstance(result, list):
             raise JsonPatchInvalidError()
 
         return result
 
     @property
```

### Comparing `jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/jsonpatchplus.py` & `jsonpatchplus-0.2.0/src/jsonpatchplus/loaders/jsonpatchplus.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import json
 
 import yaml
 from pathlib import Path
-from typing import List
+from typing import List, Optional
 
 from ..ctypes import (
     StringOrFilePath,
     JsonDocument,
     JsonPatch,
     JsonPatchDocument,
     JsonPatchDocumentLoader,
     JsonPatchPreprocessor,
 )
-from ..exceptions import JsonPatchInvalidError
+from ..exceptions import JsonDocumentMissing, JsonPatchInvalidError
 
 
 class Expansion:
     def __init__(
         self, /, *, tag: str, patch: JsonPatch, expansions: List[JsonPatch]
     ) -> None:
         self.tag = tag
@@ -33,24 +33,27 @@
 
 
 class Loader:
     def __init__(
         self,
         /,
         *,
-        doc: JsonDocument,
         preprocessors: List[JsonPatchPreprocessor],
+        doc: Optional[JsonDocument] = None,
         **kwargs,
     ) -> None:
         self.doc = doc
         self.preprocessors = preprocessors
 
         self.expansions: List[Expansion] = []
 
     def __call__(self, s_or_fp: StringOrFilePath, /, **kwargs) -> JsonPatchDocument:
+        if not self.doc:
+            raise JsonDocumentMissing()
+
         self.expansions = []
 
         if not isinstance(s_or_fp, (bytes, str)):
             kwargs.setdefault("encoding", "utf-8")
             kwargs.setdefault("errors", "ignore")
             s_or_fp = Path(s_or_fp).read_text(**kwargs)
```

### Comparing `jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/PKG-INFO` & `jsonpatchplus-0.2.0/src/jsonpatchplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonpatchplus
-Version: 0.1.1
+Version: 0.2.0
 Summary: JsonPatch+
 Author-email: Elmer Nocon <elmernocon@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Elmer Nocon
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

