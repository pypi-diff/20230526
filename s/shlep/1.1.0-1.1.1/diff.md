# Comparing `tmp/shlep-1.1.0.tar.gz` & `tmp/shlep-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-1.1.0.tar", last modified: Fri May 26 06:42:46 2023, max compression
+gzip compressed data, was "shlep-1.1.1.tar", last modified: Fri May 26 06:45:47 2023, max compression
```

## Comparing `shlep-1.1.0.tar` & `shlep-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.1.0/LICENSE
--rw-r--r--   0        0        0     2221 2023-05-26 04:43:52.285127 shlep-1.1.0/README.md
--rw-r--r--   0        0        0      454 2023-05-26 06:42:46.679781 shlep-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.1.0/shlep/__init__.py
--rw-r--r--   0        0        0     3921 2023-05-26 06:41:59.127320 shlep-1.1.0/shlep/main.py
--rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 shlep-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2221 2023-05-26 04:43:52.285127 shlep-1.1.1/README.md
+-rw-r--r--   0        0        0      454 2023-05-26 06:45:47.814488 shlep-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.1.1/shlep/__init__.py
+-rw-r--r--   0        0        0     3918 2023-05-26 06:43:17.820009 shlep-1.1.1/shlep/main.py
+-rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 shlep-1.1.1/PKG-INFO
```

### Comparing `shlep-1.1.0/LICENSE` & `shlep-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-1.1.0/README.md` & `shlep-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shlep-1.1.0/shlep/main.py` & `shlep-1.1.1/shlep/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 import logging
 import os
 from pathlib import Path
 
 from pathspec import PathSpec
 
 DEFAULT_EXCLUDED = [
-    ".git/",
-    ".idea/",
-    ".pytest_cache/",
+    ".git",
+    ".idea",
+    ".pytest_cache",
 ]
 
 logger = logging.getLogger(__name__)
 
 
 def _is_excluded(base: Path, path: Path, spec: PathSpec = None):
     if not spec:
```

### Comparing `shlep-1.1.0/PKG-INFO` & `shlep-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 1.1.0
+Version: 1.1.1
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
```

