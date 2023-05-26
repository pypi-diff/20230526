# Comparing `tmp/luisy-1.2.1.tar.gz` & `tmp/luisy-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luisy-1.2.1.tar", last modified: Fri Mar  3 13:43:55 2023, max compression
+gzip compressed data, was "luisy-1.2.2.tar", last modified: Fri May 26 11:43:23 2023, max compression
```

## Comparing `luisy-1.2.1.tar` & `luisy-1.2.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:43:55.770730 luisy-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-03-03 13:43:28.000000 luisy-1.2.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-03-03 13:43:55.770730 luisy-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-03-03 13:43:28.000000 luisy-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:43:55.770730 luisy-1.2.1/luisy/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/code_inspection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/default_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/file_system.py
--rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/hashes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/luigi_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/targets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:43:55.770730 luisy-1.2.1/luisy/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/tasks/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-03 13:43:28.000000 luisy-1.2.1/luisy/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-03 13:43:55.770730 luisy-1.2.1/luisy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-03-03 13:43:55.000000 luisy-1.2.1/luisy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-03 13:43:55.000000 luisy-1.2.1/luisy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-03 13:43:55.000000 luisy-1.2.1/luisy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-03 13:43:55.000000 luisy-1.2.1/luisy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-03-03 13:43:55.000000 luisy-1.2.1/luisy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-03 13:43:55.000000 luisy-1.2.1/luisy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-03-03 13:43:55.770730 luisy-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-03-03 13:43:28.000000 luisy-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:43:23.743646 luisy-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-05-26 11:42:51.000000 luisy-1.2.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-26 11:43:23.743646 luisy-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-05-26 11:42:51.000000 luisy-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:43:23.743646 luisy-1.2.2/luisy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20141 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/code_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7585 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/default_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/file_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20428 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12409 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/luigi_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6446 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:43:23.743646 luisy-1.2.2/luisy/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6942 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/tasks/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6196 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-26 11:42:51.000000 luisy-1.2.2/luisy/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:43:23.743646 luisy-1.2.2/luisy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-26 11:43:23.000000 luisy-1.2.2/luisy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-26 11:43:23.000000 luisy-1.2.2/luisy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:43:23.000000 luisy-1.2.2/luisy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 11:43:23.000000 luisy-1.2.2/luisy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 11:43:23.000000 luisy-1.2.2/luisy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 11:43:23.000000 luisy-1.2.2/luisy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-26 11:43:23.747646 luisy-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-05-26 11:42:51.000000 luisy-1.2.2/setup.py
```

### Comparing `luisy-1.2.1/LICENSE.txt` & `luisy-1.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/PKG-INFO` & `luisy-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luisy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Framework to build data pipelines
 Author: Robert Bosch GmbH
 License: Apache-2.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
```

### Comparing `luisy-1.2.1/README.md` & `luisy-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/__init__.py` & `luisy-1.2.2/luisy/__init__.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/cli.py` & `luisy-1.2.2/luisy/cli.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/code_inspection.py` & `luisy-1.2.2/luisy/code_inspection.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/config.py` & `luisy-1.2.2/luisy/config.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/decorators.py` & `luisy-1.2.2/luisy/decorators.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/default_params.py` & `luisy-1.2.2/luisy/default_params.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/file_system.py` & `luisy-1.2.2/luisy/file_system.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/hashes.py` & `luisy-1.2.2/luisy/hashes.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/helpers.py` & `luisy-1.2.2/luisy/helpers.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/luigi_interface.py` & `luisy-1.2.2/luisy/luigi_interface.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/targets.py` & `luisy-1.2.2/luisy/targets.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/tasks/base.py` & `luisy-1.2.2/luisy/tasks/base.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/testing.py` & `luisy-1.2.2/luisy/testing.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy/visualize.py` & `luisy-1.2.2/luisy/visualize.py`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/luisy.egg-info/PKG-INFO` & `luisy-1.2.2/luisy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luisy
-Version: 1.2.1
+Version: 1.2.2
 Summary: Framework to build data pipelines
 Author: Robert Bosch GmbH
 License: Apache-2.0
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 License-File: LICENSE.txt
```

### Comparing `luisy-1.2.1/luisy.egg-info/SOURCES.txt` & `luisy-1.2.2/luisy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luisy-1.2.1/setup.py` & `luisy-1.2.2/setup.py`

 * *Files identical despite different names*

