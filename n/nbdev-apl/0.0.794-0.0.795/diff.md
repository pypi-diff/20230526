# Comparing `tmp/nbdev-apl-0.0.794.tar.gz` & `tmp/nbdev-apl-0.0.795.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdev-apl-0.0.794.tar", last modified: Thu May 25 13:16:45 2023, max compression
+gzip compressed data, was "nbdev-apl-0.0.795.tar", last modified: Fri May 26 01:47:42 2023, max compression
```

## Comparing `nbdev-apl-0.0.794.tar` & `nbdev-apl-0.0.795.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:16:45.048032 nbdev-apl-0.0.794/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-25 13:06:49.000000 nbdev-apl-0.0.794/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 13:06:49.000000 nbdev-apl-0.0.794/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-25 13:16:45.044032 nbdev-apl-0.0.794/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-25 13:06:49.000000 nbdev-apl-0.0.794/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:16:45.044032 nbdev-apl-0.0.794/nbdev_apl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/nbdev_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-25 13:06:49.000000 nbdev-apl-0.0.794/nbdev_apl/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/nbdev_apl/_nbdev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 13:16:45.044032 nbdev-apl-0.0.794/nbdev_apl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/nbdev_apl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-25 13:16:45.000000 nbdev-apl-0.0.794/nbdev_apl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/nbdev_apl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/nbdev_apl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/nbdev_apl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/nbdev_apl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/nbdev_apl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-25 13:16:44.000000 nbdev-apl-0.0.794/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 13:16:45.048032 nbdev-apl-0.0.794/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-25 13:06:49.000000 nbdev-apl-0.0.794/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:47:42.541698 nbdev-apl-0.0.795/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-26 01:32:54.000000 nbdev-apl-0.0.795/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-26 01:32:54.000000 nbdev-apl-0.0.795/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-26 01:47:42.537698 nbdev-apl-0.0.795/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 01:32:54.000000 nbdev-apl-0.0.795/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:47:42.537698 nbdev-apl-0.0.795/nbdev_apl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-26 01:32:54.000000 nbdev-apl-0.0.795/nbdev_apl/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl/_nbdev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:47:42.537698 nbdev-apl-0.0.795/nbdev_apl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/nbdev_apl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-26 01:47:42.000000 nbdev-apl-0.0.795/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:47:42.541698 nbdev-apl-0.0.795/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-26 01:32:54.000000 nbdev-apl-0.0.795/setup.py
```

### Comparing `nbdev-apl-0.0.794/LICENSE` & `nbdev-apl-0.0.795/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.794/PKG-INFO` & `nbdev-apl-0.0.795/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.794
+Version: 0.0.795
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.794/nbdev_apl/_modidx.py` & `nbdev-apl-0.0.795/nbdev_apl/_modidx.py`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.794/nbdev_apl.egg-info/PKG-INFO` & `nbdev-apl-0.0.795/nbdev_apl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.794
+Version: 0.0.795
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.794/settings.ini` & `nbdev-apl-0.0.795/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 user = fastai
 description = nbdev docs lookup for numpy
 keywords = nbdev fastai python
 author = Jeremy Howard
 author_email = info@fast.ai
 copyright = fast.ai, inc
 branch = master
-version = 0.0.794
+version = 0.0.795
 min_python = 3.6
 audience = Developers
 language = English
 license = apache2
 status = 2
 lib_path = nbdev_apl
 nbs_path = .
```

### Comparing `nbdev-apl-0.0.794/setup.py` & `nbdev-apl-0.0.795/setup.py`

 * *Files identical despite different names*

