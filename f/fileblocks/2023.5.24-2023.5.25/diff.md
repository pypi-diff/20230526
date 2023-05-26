# Comparing `tmp/fileblocks-2023.5.24.tar.gz` & `tmp/fileblocks-2023.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fileblocks-2023.5.24.tar", last modified: Fri May 26 01:11:58 2023, max compression
+gzip compressed data, was "fileblocks-2023.5.25.tar", last modified: Fri May 26 01:23:48 2023, max compression
```

## Comparing `fileblocks-2023.5.24.tar` & `fileblocks-2023.5.25.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:11:58.925907 fileblocks-2023.5.24/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 01:11:46.000000 fileblocks-2023.5.24/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-26 01:11:58.921907 fileblocks-2023.5.24/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-26 01:11:46.000000 fileblocks-2023.5.24/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:11:58.921907 fileblocks-2023.5.24/fbi/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 01:11:46.000000 fileblocks-2023.5.24/fbi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 01:11:46.000000 fileblocks-2023.5.24/fbi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-26 01:11:46.000000 fileblocks-2023.5.24/fbi/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:11:58.921907 fileblocks-2023.5.24/fileblocks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-26 01:11:58.000000 fileblocks-2023.5.24/fileblocks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 01:11:58.000000 fileblocks-2023.5.24/fileblocks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:11:58.000000 fileblocks-2023.5.24/fileblocks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 01:11:58.000000 fileblocks-2023.5.24/fileblocks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 01:11:58.000000 fileblocks-2023.5.24/fileblocks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-26 01:11:58.000000 fileblocks-2023.5.24/fileblocks.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:11:58.925907 fileblocks-2023.5.24/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 01:11:46.000000 fileblocks-2023.5.24/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:23:48.661488 fileblocks-2023.5.25/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-26 01:23:48.661488 fileblocks-2023.5.25/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:23:48.657488 fileblocks-2023.5.25/fbi/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/fbi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/fbi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/fbi/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:23:48.661488 fileblocks-2023.5.25/fileblocks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3426 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-26 01:23:48.000000 fileblocks-2023.5.25/fileblocks.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:23:48.661488 fileblocks-2023.5.25/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-26 01:23:35.000000 fileblocks-2023.5.25/setup.py
```

### Comparing `fileblocks-2023.5.24/LICENSE` & `fileblocks-2023.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `fileblocks-2023.5.24/PKG-INFO` & `fileblocks-2023.5.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileblocks
-Version: 2023.5.24
+Version: 2023.5.25
 Summary: Walk the line, Byte by Byte Analysis
 Home-page: https://github.com/jblukach/fbi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fileblocks-2023.5.24/README.md` & `fileblocks-2023.5.25/README.md`

 * *Files identical despite different names*

### Comparing `fileblocks-2023.5.24/fbi/cli.py` & `fileblocks-2023.5.25/fbi/cli.py`

 * *Files identical despite different names*

### Comparing `fileblocks-2023.5.24/fileblocks.egg-info/PKG-INFO` & `fileblocks-2023.5.25/fileblocks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileblocks
-Version: 2023.5.24
+Version: 2023.5.25
 Summary: Walk the line, Byte by Byte Analysis
 Home-page: https://github.com/jblukach/fbi
 Author: John Lukach
 Author-email: hello@lukach.io
 License: Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `fileblocks-2023.5.24/setup.py` & `fileblocks-2023.5.25/setup.py`

 * *Files identical despite different names*

