# Comparing `tmp/playmolecule-1.8.2.tar.gz` & `tmp/playmolecule-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "playmolecule-1.8.2.tar", last modified: Thu May 25 08:10:05 2023, max compression
+gzip compressed data, was "playmolecule-1.8.3.tar", last modified: Fri May 26 09:55:41 2023, max compression
```

## Comparing `playmolecule-1.8.2.tar` & `playmolecule-1.8.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:10:05.255429 playmolecule-1.8.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-25 08:09:42.000000 playmolecule-1.8.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 08:09:42.000000 playmolecule-1.8.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-25 08:10:05.251428 playmolecule-1.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-25 08:09:42.000000 playmolecule-1.8.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:10:05.255429 playmolecule-1.8.2/playmolecule/
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/_test_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-25 08:10:05.255429 playmolecule-1.8.2/playmolecule/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (123)    32574 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/devutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/jsonlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/local.py
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/logging.ini
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/playqueue.py
--rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-25 08:09:42.000000 playmolecule-1.8.2/playmolecule/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:10:05.251428 playmolecule-1.8.2/playmolecule.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-25 08:10:05.000000 playmolecule-1.8.2/playmolecule.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-25 08:10:05.000000 playmolecule-1.8.2/playmolecule.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:10:05.000000 playmolecule-1.8.2/playmolecule.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 08:10:04.000000 playmolecule-1.8.2/playmolecule.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-25 08:10:05.000000 playmolecule-1.8.2/playmolecule.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-25 08:10:05.000000 playmolecule-1.8.2/playmolecule.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-25 08:09:42.000000 playmolecule-1.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 08:10:05.255429 playmolecule-1.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-25 08:09:42.000000 playmolecule-1.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 08:10:05.251428 playmolecule-1.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-25 08:09:42.000000 playmolecule-1.8.2/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-25 08:09:42.000000 playmolecule-1.8.2/tests/test_app_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-25 08:09:42.000000 playmolecule-1.8.2/tests/test_datacenter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:55:41.419762 playmolecule-1.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-26 09:55:19.000000 playmolecule-1.8.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 09:55:19.000000 playmolecule-1.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 09:55:41.419762 playmolecule-1.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 09:55:19.000000 playmolecule-1.8.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:55:41.419762 playmolecule-1.8.3/playmolecule/
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/_test_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 09:55:41.419762 playmolecule-1.8.3/playmolecule/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24631 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32601 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/devutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32171 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9766 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/jsonlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6392 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/playqueue.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33414 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3707 2023-05-26 09:55:19.000000 playmolecule-1.8.3/playmolecule/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:55:41.419762 playmolecule-1.8.3/playmolecule.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 09:55:41.000000 playmolecule-1.8.3/playmolecule.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-26 09:55:19.000000 playmolecule-1.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:55:41.419762 playmolecule-1.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 09:55:19.000000 playmolecule-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:55:41.419762 playmolecule-1.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 09:55:19.000000 playmolecule-1.8.3/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-26 09:55:19.000000 playmolecule-1.8.3/tests/test_app_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4083 2023-05-26 09:55:19.000000 playmolecule-1.8.3/tests/test_datacenter.py
```

### Comparing `playmolecule-1.8.2/LICENSE.md` & `playmolecule-1.8.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/PKG-INFO` & `playmolecule-1.8.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.2
+Version: 1.8.3
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.2/playmolecule/__init__.py` & `playmolecule-1.8.3/playmolecule/__init__.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/_test_funcs.py` & `playmolecule-1.8.3/playmolecule/_test_funcs.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/config.py` & `playmolecule-1.8.3/playmolecule/config.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/datacenter.py` & `playmolecule-1.8.3/playmolecule/datacenter.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/devutils.py` & `playmolecule-1.8.3/playmolecule/devutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -537,14 +537,15 @@
     import datetime
     import shutil
     from unittest import mock
     import json
     import yaml
     import traceback
     import logging
+    from shlex import split
 
     # Import the module/function of the app to call
     pieces = func.split(".")
     top_module = pieces[0]
     module_name = ".".join(pieces[:-1])
     module = importlib.import_module(module_name)
     func = getattr(module, pieces[-1])
@@ -560,15 +561,15 @@
         return
 
     if token is None:
         if input_json is not None:
             with open(input_json, "r") as f:
                 params = json.load(f)
         else:
-            cli_arg = cli_arg_str.split()
+            cli_arg = split(cli_arg_str)
             print("Parsing arguments", cli_arg)
             # The parser really likes to kill the app when failing to parse... This mock.patch prevents it
             with mock.patch("sys.exit") as m:
                 appargs, unknownargs = parser.parse_known_args(cli_arg)
                 if len(unknownargs):
                     # Otherwise throw an error for unknown arguments
                     parser.print_help()
```

### Comparing `playmolecule-1.8.2/playmolecule/job.py` & `playmolecule-1.8.3/playmolecule/job.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/jsonlogger.py` & `playmolecule-1.8.3/playmolecule/jsonlogger.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/local.py` & `playmolecule-1.8.3/playmolecule/local.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/playqueue.py` & `playmolecule-1.8.3/playmolecule/playqueue.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/session.py` & `playmolecule-1.8.3/playmolecule/session.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule/utils.py` & `playmolecule-1.8.3/playmolecule/utils.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/playmolecule.egg-info/PKG-INFO` & `playmolecule-1.8.3/playmolecule.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: playmolecule
-Version: 1.8.2
+Version: 1.8.3
 Summary: PlayMolecule python API
 Author-email: Acellera <info@acellera.com>
 Project-URL: Homepage, https://github.com/Acellera/playmolecule-python-api
 Project-URL: Bug Tracker, https://github.com/Acellera/playmolecule-python-api/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.8
```

### Comparing `playmolecule-1.8.2/playmolecule.egg-info/SOURCES.txt` & `playmolecule-1.8.3/playmolecule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/pyproject.toml` & `playmolecule-1.8.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/tests/test.py` & `playmolecule-1.8.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/tests/test_app_wrapper.py` & `playmolecule-1.8.3/tests/test_app_wrapper.py`

 * *Files identical despite different names*

### Comparing `playmolecule-1.8.2/tests/test_datacenter.py` & `playmolecule-1.8.3/tests/test_datacenter.py`

 * *Files identical despite different names*

