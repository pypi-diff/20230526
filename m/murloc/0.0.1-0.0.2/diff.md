# Comparing `tmp/murloc-0.0.1.tar.gz` & `tmp/murloc-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "murloc-0.0.1.tar", last modified: Fri May 26 20:58:44 2023, max compression
+gzip compressed data, was "murloc-0.0.2.tar", last modified: Fri May 26 21:45:30 2023, max compression
```

## Comparing `murloc-0.0.1.tar` & `murloc-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 20:58:44.440891 murloc-0.0.1/
--rw-rw-r--   0 chris     (1000) chris     (1000)      726 2023-05-26 20:58:44.440891 murloc-0.0.1/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      435 2023-05-26 20:56:53.000000 murloc-0.0.1/README.md
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 20:58:44.439891 murloc-0.0.1/murloc/
--rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.1/murloc/__init__.py
--rw-rw-r--   0 chris     (1000) chris     (1000)     4311 2023-05-26 20:54:12.000000 murloc-0.0.1/murloc/murloc.py
-drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 20:58:44.440891 murloc-0.0.1/murloc.egg-info/
--rw-rw-r--   0 chris     (1000) chris     (1000)      726 2023-05-26 20:58:44.000000 murloc-0.0.1/murloc.egg-info/PKG-INFO
--rw-rw-r--   0 chris     (1000) chris     (1000)      174 2023-05-26 20:58:44.000000 murloc-0.0.1/murloc.egg-info/SOURCES.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-26 20:58:44.000000 murloc-0.0.1/murloc.egg-info/dependency_links.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-05-26 20:58:44.000000 murloc-0.0.1/murloc.egg-info/top_level.txt
--rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-26 20:58:44.440891 murloc-0.0.1/setup.cfg
--rw-rw-r--   0 chris     (1000) chris     (1000)      534 2023-05-26 20:57:35.000000 murloc-0.0.1/setup.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 21:45:30.158213 murloc-0.0.2/
+-rw-rw-r--   0 chris     (1000) chris     (1000)     1068 2023-05-26 21:19:51.000000 murloc-0.0.2/LICENSE
+-rw-rw-r--   0 chris     (1000) chris     (1000)      799 2023-05-26 21:45:30.158213 murloc-0.0.2/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      435 2023-05-26 21:35:46.000000 murloc-0.0.2/README.md
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 21:45:30.157213 murloc-0.0.2/murloc/
+-rw-rw-r--   0 chris     (1000) chris     (1000)       25 2023-05-26 20:30:24.000000 murloc-0.0.2/murloc/__init__.py
+-rw-rw-r--   0 chris     (1000) chris     (1000)     3972 2023-05-26 21:33:46.000000 murloc-0.0.2/murloc/murloc.py
+drwxrwxr-x   0 chris     (1000) chris     (1000)        0 2023-05-26 21:45:30.158213 murloc-0.0.2/murloc.egg-info/
+-rw-rw-r--   0 chris     (1000) chris     (1000)      799 2023-05-26 21:45:30.000000 murloc-0.0.2/murloc.egg-info/PKG-INFO
+-rw-rw-r--   0 chris     (1000) chris     (1000)      182 2023-05-26 21:45:30.000000 murloc-0.0.2/murloc.egg-info/SOURCES.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        1 2023-05-26 21:45:30.000000 murloc-0.0.2/murloc.egg-info/dependency_links.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)        7 2023-05-26 21:45:30.000000 murloc-0.0.2/murloc.egg-info/top_level.txt
+-rw-rw-r--   0 chris     (1000) chris     (1000)       38 2023-05-26 21:45:30.158213 murloc-0.0.2/setup.cfg
+-rw-rw-r--   0 chris     (1000) chris     (1000)      584 2023-05-26 21:34:41.000000 murloc-0.0.2/setup.py
```

### Comparing `murloc-0.0.1/PKG-INFO` & `murloc-0.0.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: murloc
-Version: 0.0.1
+Version: 0.0.2
 Summary: extensible api server
 Home-page: 
 Author: Chris Varga
 Author-email: 
 Keywords: extensible api server
 Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Murloc
 Extensible api server
 
 ## Example usage
 ```
 import murloc
```

### Comparing `murloc-0.0.1/murloc/murloc.py` & `murloc-0.0.2/murloc/murloc.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 #!/usr/bin/env python3
 
 import os
 import sys
 import time
-import json
 import struct
 import signal
 import socket
 import inspect
-import subprocess
 
 def init(*args, **kwargs):
     return Murloc(*args, **kwargs)
 
 class Murloc:
     def __init__(
         self,
@@ -135,26 +133,7 @@
                     self.log(f"Connection from {addr}")
                     self.handle_connection(conn, addr)
                     sys.exit(0)
                 else:
                     continue
             except:
                 break
-
-"""
-# Define server methods here.
-def hello(self, args):
-    # First parameter must be self.
-    self.log(f"'{inspect.currentframe().f_code.co_name}' called")
-    return f"args={args}"
-
-
-methods = {
-    "hello": hello,
-}
-
-
-# Main
-if __name__ == "__main__":
-    s = Murloc(methods=methods)
-    s.listen()
-"""
```

### Comparing `murloc-0.0.1/murloc.egg-info/PKG-INFO` & `murloc-0.0.2/murloc.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: murloc
-Version: 0.0.1
+Version: 0.0.2
 Summary: extensible api server
 Home-page: 
 Author: Chris Varga
 Author-email: 
 Keywords: extensible api server
 Classifier: Programming Language :: Python
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # Murloc
 Extensible api server
 
 ## Example usage
 ```
 import murloc
```

### Comparing `murloc-0.0.1/setup.py` & `murloc-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="murloc",
-    version="0.0.1",
+    version="0.0.2",
     author="Chris Varga",
     author_email="",
     description="extensible api server",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
+        "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords="extensible api server",
 )
```

