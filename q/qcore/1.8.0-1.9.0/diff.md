# Comparing `tmp/qcore-1.8.0.tar.gz` & `tmp/qcore-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcore-1.8.0.tar", last modified: Wed Apr 20 00:45:38 2022, max compression
+gzip compressed data, was "qcore-1.9.0.tar", last modified: Fri May 26 03:43:20 2023, max compression
```

## Comparing `qcore-1.8.0.tar` & `qcore-1.9.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 00:45:38.653431 qcore-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    10173 2022-04-20 00:45:33.000000 qcore-1.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     7459 2022-04-20 00:45:38.653431 qcore-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5289 2022-04-20 00:45:33.000000 qcore-1.8.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-04-20 00:45:33.000000 qcore-1.8.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 00:45:38.649431 qcore-1.8.0/qcore/
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      708 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14009 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/asserts.py
--rw-r--r--   0 runner    (1001) docker     (121)     3694 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/asserts.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1324 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/caching.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    13654 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/caching.py
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/caching.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     4105 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     1143 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/debug.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/decorators.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     9662 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1743 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/disallow_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (121)       37 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/disallow_inheritance.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12142 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     2253 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/enum.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     2190 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/errors.py
--rw-r--r--   0 runner    (1001) docker     (121)      608 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (121)      803 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/events.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    12913 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     2075 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/events.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1938 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/helpers.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     8569 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     2201 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/helpers.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1992 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/inspectable_class.py
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/inspectable_class.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/inspection.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     6722 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/inspection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1201 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/inspection.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1218 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/microtime.pxd
--rw-r--r--   0 runner    (1001) docker     (121)     5585 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/microtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     1417 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/microtime.pyi
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     4533 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/testing.pyi
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 00:45:38.653431 qcore-1.8.0/qcore/tests/
--rw-r--r--   0 runner    (1001) docker     (121)    10350 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_asserts.py
--rw-r--r--   0 runner    (1001) docker     (121)    16822 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_caching.py
--rw-r--r--   0 runner    (1001) docker     (121)     2876 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_debug.py
--rw-r--r--   0 runner    (1001) docker     (121)    11356 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)      222 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_disallow_inheritance.py
--rw-r--r--   0 runner    (1001) docker     (121)    10545 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_enum.py
--rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)     7879 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_events.py
--rw-r--r--   0 runner    (1001) docker     (121)     1720 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_examples.py
--rw-r--r--   0 runner    (1001) docker     (121)     6334 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     4806 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_inspectable_class.py
--rw-r--r--   0 runner    (1001) docker     (121)     5652 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_inspection.py
--rw-r--r--   0 runner    (1001) docker     (121)     1766 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_microtime.py
--rw-r--r--   0 runner    (1001) docker     (121)     3703 2022-04-20 00:45:33.000000 qcore-1.8.0/qcore/tests/test_testing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-20 00:45:38.649431 qcore-1.8.0/qcore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     7459 2022-04-20 00:45:38.000000 qcore-1.8.0/qcore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-04-20 00:45:38.000000 qcore-1.8.0/qcore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-20 00:45:38.000000 qcore-1.8.0/qcore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-20 00:45:38.000000 qcore-1.8.0/qcore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-04-20 00:45:38.000000 qcore-1.8.0/qcore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-20 00:45:38.653431 qcore-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2227 2022-04-20 00:45:33.000000 qcore-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:20.008219 qcore-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10173 2023-05-26 03:43:16.000000 qcore-1.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-26 03:43:20.008219 qcore-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5281 2023-05-26 03:43:16.000000 qcore-1.9.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 03:43:16.000000 qcore-1.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:20.008219 qcore-1.9.0/qcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14001 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/asserts.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/caching.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    13638 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/caching.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/debug.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/decorators.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9646 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/disallow_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/disallow_inheritance.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12134 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/enum.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2190 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/events.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12889 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1890 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/helpers.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/helpers.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1984 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspectable_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspectable_class.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspection.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/inspection.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/microtime.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7318 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/microtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/microtime.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4518 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/testing.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:20.008219 qcore-1.9.0/qcore/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_asserts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16772 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11328 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_disallow_inheritance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10545 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6302 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_inspectable_class.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5557 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_inspection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4825 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_microtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-05-26 03:43:16.000000 qcore-1.9.0/qcore/tests/test_testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:43:20.008219 qcore-1.9.0/qcore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5947 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 03:43:19.000000 qcore-1.9.0/qcore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 03:43:20.008219 qcore-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-26 03:43:16.000000 qcore-1.9.0/setup.py
```

### Comparing `qcore-1.8.0/LICENSE` & `qcore-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/PKG-INFO` & `qcore-1.9.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,206 +1,206 @@
 Metadata-Version: 2.1
 Name: qcore
-Version: 1.8.0
+Version: 1.9.0
 Summary: Quora's core utility library
 Home-page: https://github.com/quora/qcore
 Author: Quora, Inc.
 Author-email: asynq@quora.com
 License: Apache Software License
-Description: *****
-        qcore
-        *****
-        
-        ``qcore`` is a library of common utility functions used at Quora. It is used to
-        abstract out common functionality for other Quora libraries like `asynq <https://github.com/quora/asynq>`_.
-        
-        Its component modules are discussed below. See the docstrings in the code
-        itself for more detail.
-        
-        qcore.asserts
-        -------------
-        
-        When a normal Python assert fails, it only indicates that there was a failure,
-        not what the bad values were that caused the assert to fail. This module
-        provides rich assertion helpers that automatically produce better error
-        messages. For example:
-        
-        .. code-block:: python
-        
-            >>> from qcore.asserts import assert_eq
-            >>> assert 5 == 2 * 2
-            Traceback (most recent call last):
-              File "<stdin>", line 1, in <module>
-            AssertionError
-            >>> assert_eq(5, 2 * 2)
-            Traceback (most recent call last):
-              File "<stdin>", line 1, in <module>
-              File "qcore/asserts.py", line 82, in assert_eq
-                assert expected == actual, _assert_fail_message(message, expected, actual, '!=', extra)
-            AssertionError: 5 != 4
-        
-        Similar methods are provided by the standard library's ``unittest`` package,
-        but those are tied to the ``TestCase`` class instead of being standalone
-        functions.
-        
-        qcore.caching
-        -------------
-        
-        This provides helpers for caching data. Some examples include:
-        
-        .. code-block:: python
-        
-            from qcore.caching import cached_per_instance, lazy_constant
-        
-            @lazy_constant
-            def some_function():
-                # this will only be executed the first time some_function() is called;
-                # afterwards it will be cached
-                return expensive_computation()
-        
-            class SomeClass(object):
-                @cached_per_instance()
-                def some_method(self, a, b):
-                    # for any instance of SomeClass, this will only be executed once
-                    return expensive_computation(a, b)
-        
-        qcore.debug
-        -----------
-        
-        This module provides some helpers useful for debugging Python. Among others, it
-        includes the ``@qcore.debug.trace()`` decorator, which can be used to trace
-        every time a function is called.
-        
-        qcore.decorators
-        ----------------
-        
-        This module provides an abstraction for class-based decorators that supports
-        transparently decorating functions, methods, classmethods, and staticmethods
-        while also providing the option to add additional custom attributes. For
-        example, it could be used to provide a caching decorator that adds a ``.dirty``
-        attribute to decorated functions to dirty their cache:
-        
-        .. code-block:: python
-        
-            from qcore.decorators import DecoratorBase, DecoratorBinder, decorate
-        
-            class CacheDecoratorBinder(DecoratorBinder):
-                def dirty(self, *args):
-                    if self.instance is None:
-                        return self.decorator.dirty(*args)
-                    else:
-                        return self.decorator.dirty(self.instance, *args)
-        
-            class CacheDecorator(DecoratorBase):
-                binder_cls = CacheDecoratorBinder
-        
-                def __init__(self, *args):
-                    super().__init__(*args)
-                    self._cache = {}
-        
-                def dirty(self, *args):
-                    try:
-                        del self._cache[args]
-                    except KeyError:
-                        pass
-        
-                def __call__(self, *args):
-                    try:
-                        return self._cache[args]
-                    except KeyError:
-                        value = self.fn(*args)
-                        self._cache[args] = value
-                        return value
-        
-            cached = decorate(CacheDecorator)
-        
-        qcore.enum
-        ----------
-        
-        This module provides an abstraction for defining enums. You can define an enum
-        as follows:
-        
-        .. code-block:: python
-        
-            from qcore.enum import Enum
-        
-            class Color(Enum):
-                red = 1
-                green = 2
-                blue = 3
-        
-        qcore.errors
-        ------------
-        
-        This module provides some commonly useful exception classes and helpers for
-        reraising exceptions from a different place.
-        
-        qcore.events
-        ------------
-        
-        This provides an abstraction for registering events and running callbacks.
-        Example usage:
-        
-        .. code-block:: python
-        
-            >>> from qcore.events import EventHook
-            >>> event = EventHook()
-            >>> def callback():
-            ...     print('callback called')
-            ...
-            >>> event.subscribe(callback)
-            >>> event.trigger()
-            callback called
-        
-        qcore.helpers
-        -------------
-        
-        This provides a number of small helper functions.
-        
-        qcore.inspectable_class
-        -----------------------
-        
-        This provides a base class that automatically provides hashing, equality
-        checks, and a readable ``repr()`` result. Example usage:
-        
-        .. code-block:: python
-        
-            >>> from qcore.inspectable_class import InspectableClass
-            >>> class Pair(InspectableClass):
-            ...     def __init__(self, a, b):
-            ...         self.a = a
-            ...         self.b = b
-            ...
-            >>> Pair(1, 2)
-            Pair(a=1, b=2)
-            >>> Pair(1, 2) == Pair(1, 2)
-            True
-        
-        qcore.inspection
-        ----------------
-        
-        This provides functionality similar to the standard ``inspect`` module. Among
-        others, it includes the ``get_original_fn`` function, which extracts the
-        underlying function from a ``qcore.decorators``-decorated object.
-        
-        qcore.microtime
-        ---------------
-        
-        This includes helpers for dealing with time, represented as an integer number
-        of microseconds since the Unix epoch.
-        
-        qcore.testing
-        -------------
-        
-        This provides helpers to use in unit tests. Among others, it provides an
-        ``Anything`` object that compares equal to any other Python object.
-        
 Keywords: quora core common utility
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+*****
+qcore
+*****
+
+``qcore`` is a library of common utility functions used at Quora. It is used to
+abstract out common functionality for other Quora libraries like `asynq <https://github.com/quora/asynq>`_.
+
+Its component modules are discussed below. See the docstrings in the code
+itself for more detail.
+
+qcore.asserts
+-------------
+
+When a normal Python assert fails, it only indicates that there was a failure,
+not what the bad values were that caused the assert to fail. This module
+provides rich assertion helpers that automatically produce better error
+messages. For example:
+
+.. code-block:: python
+
+    >>> from qcore.asserts import assert_eq
+    >>> assert 5 == 2 * 2
+    Traceback (most recent call last):
+      File "<stdin>", line 1, in <module>
+    AssertionError
+    >>> assert_eq(5, 2 * 2)
+    Traceback (most recent call last):
+      File "<stdin>", line 1, in <module>
+      File "qcore/asserts.py", line 82, in assert_eq
+        assert expected == actual, _assert_fail_message(message, expected, actual, '!=', extra)
+    AssertionError: 5 != 4
+
+Similar methods are provided by the standard library's ``unittest`` package,
+but those are tied to the ``TestCase`` class instead of being standalone
+functions.
+
+qcore.caching
+-------------
+
+This provides helpers for caching data. Some examples include:
+
+.. code-block:: python
+
+    from qcore.caching import cached_per_instance, lazy_constant
+
+    @lazy_constant
+    def some_function():
+        # this will only be executed the first time some_function() is called;
+        # afterwards it will be cached
+        return expensive_computation()
+
+    class SomeClass:
+        @cached_per_instance()
+        def some_method(self, a, b):
+            # for any instance of SomeClass, this will only be executed once
+            return expensive_computation(a, b)
+
+qcore.debug
+-----------
+
+This module provides some helpers useful for debugging Python. Among others, it
+includes the ``@qcore.debug.trace()`` decorator, which can be used to trace
+every time a function is called.
+
+qcore.decorators
+----------------
+
+This module provides an abstraction for class-based decorators that supports
+transparently decorating functions, methods, classmethods, and staticmethods
+while also providing the option to add additional custom attributes. For
+example, it could be used to provide a caching decorator that adds a ``.dirty``
+attribute to decorated functions to dirty their cache:
+
+.. code-block:: python
+
+    from qcore.decorators import DecoratorBase, DecoratorBinder, decorate
+
+    class CacheDecoratorBinder(DecoratorBinder):
+        def dirty(self, *args):
+            if self.instance is None:
+                return self.decorator.dirty(*args)
+            else:
+                return self.decorator.dirty(self.instance, *args)
+
+    class CacheDecorator(DecoratorBase):
+        binder_cls = CacheDecoratorBinder
+
+        def __init__(self, *args):
+            super().__init__(*args)
+            self._cache = {}
+
+        def dirty(self, *args):
+            try:
+                del self._cache[args]
+            except KeyError:
+                pass
+
+        def __call__(self, *args):
+            try:
+                return self._cache[args]
+            except KeyError:
+                value = self.fn(*args)
+                self._cache[args] = value
+                return value
+
+    cached = decorate(CacheDecorator)
+
+qcore.enum
+----------
+
+This module provides an abstraction for defining enums. You can define an enum
+as follows:
+
+.. code-block:: python
+
+    from qcore.enum import Enum
+
+    class Color(Enum):
+        red = 1
+        green = 2
+        blue = 3
+
+qcore.errors
+------------
+
+This module provides some commonly useful exception classes and helpers for
+reraising exceptions from a different place.
+
+qcore.events
+------------
+
+This provides an abstraction for registering events and running callbacks.
+Example usage:
+
+.. code-block:: python
+
+    >>> from qcore.events import EventHook
+    >>> event = EventHook()
+    >>> def callback():
+    ...     print('callback called')
+    ...
+    >>> event.subscribe(callback)
+    >>> event.trigger()
+    callback called
+
+qcore.helpers
+-------------
+
+This provides a number of small helper functions.
+
+qcore.inspectable_class
+-----------------------
+
+This provides a base class that automatically provides hashing, equality
+checks, and a readable ``repr()`` result. Example usage:
+
+.. code-block:: python
+
+    >>> from qcore.inspectable_class import InspectableClass
+    >>> class Pair(InspectableClass):
+    ...     def __init__(self, a, b):
+    ...         self.a = a
+    ...         self.b = b
+    ...
+    >>> Pair(1, 2)
+    Pair(a=1, b=2)
+    >>> Pair(1, 2) == Pair(1, 2)
+    True
+
+qcore.inspection
+----------------
+
+This provides functionality similar to the standard ``inspect`` module. Among
+others, it includes the ``get_original_fn`` function, which extracts the
+underlying function from a ``qcore.decorators``-decorated object.
+
+qcore.microtime
+---------------
+
+This includes helpers for dealing with time, represented as an integer number
+of microseconds since the Unix epoch.
+
+qcore.testing
+-------------
+
+This provides helpers to use in unit tests. Among others, it provides an
+``Anything`` object that compares equal to any other Python object.
```

### Comparing `qcore-1.8.0/README.rst` & `qcore-1.9.0/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
     @lazy_constant
     def some_function():
         # this will only be executed the first time some_function() is called;
         # afterwards it will be cached
         return expensive_computation()
 
-    class SomeClass(object):
+    class SomeClass:
         @cached_per_instance()
         def some_method(self, a, b):
             # for any instance of SomeClass, this will only be executed once
             return expensive_computation(a, b)
 
 qcore.debug
 -----------
```

### Comparing `qcore-1.8.0/qcore/__init__.py` & `qcore-1.9.0/qcore/__init__.py`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/__init__.pyi` & `qcore-1.9.0/qcore/__init__.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/asserts.py` & `qcore-1.9.0/qcore/asserts.py`

 * *Files 1% similar despite different names*

```diff
@@ -309,15 +309,15 @@
 
 def assert_raises(fn, *expected_exception_types):
     """Raises an AssertionError if calling fn does not raise one of the expected_exception-types."""
     with AssertRaises(*expected_exception_types):
         fn()
 
 
-class AssertRaises(object):
+class AssertRaises:
     """With-context that asserts that the code within the context raises the specified exception."""
 
     def __init__(self, *expected_exception_types, **kwargs):
         # when you don't specify the exception expected, it's easy to write buggy tests that appear
         # to pass but actually throw an exception different from the expected one
         assert (
             len(expected_exception_types) >= 1
```

### Comparing `qcore-1.8.0/qcore/asserts.pyi` & `qcore-1.9.0/qcore/asserts.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 def assert_unordered_list_eq(
     expected: Iterable[Any], actual: Iterable[Any], message: Optional[str] = ...
 ) -> None: ...
 def assert_raises(
     fn: Callable[[], Any], *expected_exception_types: Type[BaseException]
 ) -> None: ...
 
-class AssertRaises(object):
+class AssertRaises:
     expected_exception_types: Set[Type[BaseException]]
     expected_exception_found: Any
     extra: Optional[str]
     def __init__(
         self,
         *expected_exception_types: Type[BaseException],
         extra: Optional[object] = ...,
```

### Comparing `qcore-1.8.0/qcore/caching.pxd` & `qcore-1.9.0/qcore/caching.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 from . cimport helpers
 
 
 cdef object miss
 cdef object not_computed
 
 
-cdef class LazyConstant(object):
+cdef class LazyConstant:
     cdef public object value_provider
     cdef public object value
 
     cpdef get_value(self)
     cpdef compute(self)
     cpdef clear(self)
 
 
-cdef class LRUCache(object):
+cdef class LRUCache:
     cdef int _capacity
     cdef object _item_evicted
     cdef object _dict
 
     cpdef get_capacity(self)
     cpdef get(self, key, default=?)
     cpdef clear(self, omit_item_evicted=?)
```

### Comparing `qcore-1.8.0/qcore/caching.py` & `qcore-1.9.0/qcore/caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 miss = helpers.miss
 not_computed = helpers.MarkerObject("not_computed @ qcore.caching")
 globals()["miss"] = miss
 globals()["not_computed"] = not_computed
 
 
-class LazyConstant(object):
+class LazyConstant:
     """
     Describes lazy or rarely changing value.
 
     Normally used to cache lazy / rarely changing values that are re-computed
     only on demand (e.g. in case a particular event is raised).
 
     """
@@ -118,15 +118,15 @@
         else:
             return self.value
 
     def clear(self):
         self.value = not_computed
 
 
-class LRUCache(object):
+class LRUCache:
     """A dictionary-like object that stores only a certain number of items, and
     discards its least recently used item when full.
 
     >>> cache = LRUCache(3)
     >>> cache['A'] = 0
     >>> cache['B'] = 1
     >>> cache['C'] = 2
```

### Comparing `qcore-1.8.0/qcore/caching.pyi` & `qcore-1.9.0/qcore/caching.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/debug.py` & `qcore-1.9.0/qcore/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                 raise
 
         return new_fn
 
     return decorate
 
 
-class DebugCounter(object):
+class DebugCounter:
     def __init__(self, name, value=0):
         self.name = name
         self.value = value
         self.last_dump_time = 0
         counters[name] = self
 
     def increment(self, increment_by=1):
```

### Comparing `qcore-1.8.0/qcore/debug.pyi` & `qcore-1.9.0/qcore/debug.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 counters: Dict[str, DebugCounter]
 
 def trace(
     enter: bool = ..., exit: bool = ...
 ) -> Callable[[_CallableT], _CallableT]: ...
 
-class DebugCounter(object):
+class DebugCounter:
     def __init__(self, name: str, value: int = ...) -> None: ...
     def increment(self: _SelfT, increment_by: int = ...) -> _SelfT: ...
     def decrement(self: _SelfT, decrement_by: int = ...) -> _SelfT: ...
     def dump(self: _SelfT) -> _SelfT: ...
     def dump_if(
         self: _SelfT, predicate: Callable[[_SelfT], bool], and_break: bool = ...
     ) -> _SelfT: ...
```

### Comparing `qcore-1.8.0/qcore/decorators.pxd` & `qcore-1.9.0/qcore/decorators.pxd`

 * *Files 12% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import cython
 
 
-cdef class DecoratorBase(object):
+cdef class DecoratorBase:
     cdef public object fn
     cdef public object type
 
     cpdef str name(self)
     cpdef bint is_decorator(self) except -1
 
-cdef class DecoratorBinder(object):
+cdef class DecoratorBinder:
     cdef public DecoratorBase decorator
     cdef public object instance
 
     cpdef str name(self)
     cpdef bint is_decorator(self) except -1
```

### Comparing `qcore-1.8.0/qcore/decorators.py` & `qcore-1.9.0/qcore/decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import inspect
 import sys
 import time
 
 from . import inspection
 
 
-class DecoratorBinder(object):
+class DecoratorBinder:
     def __init__(self, decorator, instance=None):
         self.decorator = decorator
         self.instance = instance
 
     def name(self):
         return self.decorator.name()
 
@@ -103,15 +103,15 @@
             and self.instance == other.instance
         )
 
     DecoratorBinder.__eq__ = __eq__
     del __eq__
 
 
-class DecoratorBase(object):
+class DecoratorBase:
     binder_cls = DecoratorBinder
 
     def __init__(self, fn):
         if hasattr(fn, "__func__"):  # Class method, static method
             self.type = type(fn)
             fn = fn.__func__
         elif hasattr(fn, "is_decorator"):  # Decorator
```

### Comparing `qcore-1.8.0/qcore/decorators.pyi` & `qcore-1.9.0/qcore/decorators.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/disallow_inheritance.py` & `qcore-1.9.0/qcore/disallow_inheritance.py`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/enum.py` & `qcore-1.9.0/qcore/enum.py`

 * *Files 0% similar despite different names*

```diff
@@ -367,15 +367,15 @@
 class IntEnum(int, Enum):
     """Enum subclass that offers more compatibility with int."""
 
     def __repr__(self):
         return Enum.__repr__(self)
 
 
-class EnumValueGenerator(object):
+class EnumValueGenerator:
     def __init__(self, start=1):
         self._next_value = start
 
     def reset(self, start=1):
         self._next_value = start
 
     def next(self):
```

### Comparing `qcore-1.8.0/qcore/enum.pyi` & `qcore-1.9.0/qcore/enum.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -66,12 +66,12 @@
     def __contains__(self, item: SupportsInt) -> bool: ...
     def __or__(self: _FlagsT, other: SupportsInt) -> _FlagsT: ...
     def __and__(self: _FlagsT, other: SupportsInt) -> _FlagsT: ...
     def __xor__(self: _FlagsT, other: SupportsInt) -> _FlagsT: ...
 
 class IntEnum(int, Enum): ...
 
-class EnumValueGenerator(object):
+class EnumValueGenerator:
     def __init__(self, start: int = ...) -> None: ...
     def reset(self, start: int = ...) -> None: ...
     def next(self) -> int: ...
     def __call__(self) -> int: ...
```

### Comparing `qcore-1.8.0/qcore/errors.py` & `qcore-1.9.0/qcore/errors.py`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/errors.pyi` & `qcore-1.9.0/qcore/errors.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/events.pxd` & `qcore-1.9.0/qcore/events.pxd`

 * *Files 3% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-cdef class EventHook(object):
+cdef class EventHook:
     cdef list handlers
 
 
 cdef class SinkingEventHook(EventHook):
     pass
 
 cdef SinkingEventHook sinking_event_hook
 
 
-cdef class EventInterceptor(object):
+cdef class EventInterceptor:
     cdef object source
     cdef dict events
```

### Comparing `qcore-1.8.0/qcore/events.py` & `qcore-1.9.0/qcore/events.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import inspect
 
 from .enum import EnumType, EnumBase
 from .errors import prepare_for_reraise, reraise
 
 
-class EventHook(object):
+class EventHook:
     """This type allows to implement event pattern.
 
     Allowed operations on EventHook objects:
 
     * hook.subscribe(handler)  # subscribe
     * hook.unsubscribe(handler)  # unsubscribe (requires O(handlerCount)!)
     * hook(...)  # invokes all event handlers
@@ -159,15 +159,15 @@
         return "SinkingEventHook()"
 
 
 sinking_event_hook = SinkingEventHook()
 globals()["sinking_event_hook"] = sinking_event_hook
 
 
-class EventInterceptor(object):
+class EventInterceptor:
     """A context object helping to temporarily intercept
     a set of events on an object exposing a set of event hooks.
 
     """
 
     def __init__(self, source, **events):
         """
@@ -191,15 +191,15 @@
         """Stops event interception."""
         source = self.source
         for name, handler in self.events.items():
             hook = getattr(source, name)
             hook.unsubscribe(handler)
 
 
-class EventHub(object):
+class EventHub:
     """Provides named event hooks on demand.
 
     Use properties (or keys) of this object to access
     named event hooks created on demand (i.e. on the first
     access attempt).
 
     """
```

### Comparing `qcore-1.8.0/qcore/events.pyi` & `qcore-1.9.0/qcore/events.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Type, TypeVar
 from types import TracebackType
 
 _HandlerT = Callable[..., Any]
 
-class EventHook(object):
+class EventHook:
     def __init__(self, handlers: Optional[List[_HandlerT]] = ...) -> None: ...
     def subscribe(self, handler: _HandlerT) -> None: ...
     def unsubscribe(self, handler: _HandlerT) -> None: ...
     def safe_trigger(self, *args: Any) -> None: ...
     def trigger(self, *args: Any) -> None: ...
     def __call__(self, *args: Any) -> None: ...
     def __contains__(self, item: _HandlerT) -> bool: ...
     def __iter__(self) -> Iterator[_HandlerT]: ...
 
 class SinkingEventHook(EventHook): ...
 
 sinking_event_hook: SinkingEventHook
 
-class EventInterceptor(object):
+class EventInterceptor:
     source: object
     events: Dict[str, _HandlerT]
     def __init__(self, source: object, **events: _HandlerT) -> None: ...
     def __enter__(self) -> None: ...
     def __exit__(
         self,
         typ: Optional[Type[BaseException]],
         value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None: ...
 
 _HubT = TypeVar("_HubT", bound=EventHub)
 
-class EventHub(object):
+class EventHub:
     def __init__(self, source: Optional[Dict[Any, Any]] = ...) -> None: ...
     def on(self: _HubT, event: object, handler: _HandlerT) -> _HubT: ...
     def off(self: _HubT, event: object, handler: _HandlerT) -> _HubT: ...
     def trigger(self: _HubT, event: object, *args: Any) -> _HubT: ...
     def safe_trigger(self: _HubT, event: object, *args: Any) -> _HubT: ...
     def get_or_create(self, event: object) -> EventHook: ...
     def __getattr__(self, key: str) -> EventHook: ...
```

### Comparing `qcore-1.8.0/qcore/helpers.pxd` & `qcore-1.9.0/qcore/helpers.pxd`

 * *Files 13% similar despite different names*

```diff
@@ -17,56 +17,56 @@
 
 
 cdef list empty_list
 cdef tuple empty_tuple
 cdef dict empty_dict
 
 
-cdef class MarkerObject(object):
+cdef class MarkerObject:
     cpdef unicode name
 
 cdef MarkerObject none
 cdef MarkerObject miss
 cdef MarkerObject same
 cdef MarkerObject unspecified
 
 
-cdef class EmptyContext(object):
+cdef class EmptyContext:
     cpdef __enter__(self)
     cpdef __exit__(self, exc_type, exc_val, exc_tb)
 
 cdef EmptyContext empty_context
 
 
-cdef class CythonCachedHashWrapper(object):
+cdef class CythonCachedHashWrapper:
     cdef object _value
     cdef int _hash
 
     cpdef object value(self)
     cpdef object hash(self)
 
 cdef object CachedHashWrapper
 
 
 cdef class _ScopedValueOverrideContext(object)  # Forward declaration
 
-cdef class ScopedValue(object):
+cdef class ScopedValue:
     cdef object _value
 
     cpdef object get(self)
     cpdef set(self, object value)
     cpdef object override(self, object value)
 
-cdef class _ScopedValueOverrideContext(object):
+cdef class _ScopedValueOverrideContext:
     cdef ScopedValue _target
     cdef object _value
     cdef object _old_value
 
 
-cdef class _PropertyOverrideContext(object):
+cdef class _PropertyOverrideContext:
     cdef object _target
     cdef object _property_name
     cdef object _value
     cdef object _old_value
 
 cdef object override  # Alias of PropertyOverrideContext
```

### Comparing `qcore-1.8.0/qcore/helpers.py` & `qcore-1.9.0/qcore/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     return True
 
 
 def false_fn():
     return False
 
 
-class MarkerObject(object):
+class MarkerObject:
     """Replaces None in cases when None value is also expected.
     Used mainly by caches to describe a cache miss.
 
     """
 
     def __init__(self, name):
         if isinstance(name, bytes):
@@ -66,30 +66,30 @@
 unspecified = MarkerObject("unspecified")
 globals()["none"] = none
 globals()["miss"] = miss
 globals()["same"] = same
 globals()["unspecified"] = unspecified
 
 
-class EmptyContext(object):
+class EmptyContext:
     def __enter__(self):
         pass
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         pass
 
     def __repr__(self):
         return "qcore.empty_context"
 
 
 empty_context = EmptyContext()
 globals()["empty_context"] = empty_context
 
 
-class CythonCachedHashWrapper(object):
+class CythonCachedHashWrapper:
     def __init__(self, value):
         self._value = value
         self._hash = hash(value)
 
     def value(self):
         return self._value
 
@@ -146,15 +146,15 @@
         def __hash__(self):
             return self._hash
 
     CachedHashWrapper = PythonCachedHashWrapper
     globals()["CachedHashWrapper"] = PythonCachedHashWrapper
 
 
-class ScopedValue(object):
+class ScopedValue:
     def __init__(self, default):
         self._value = default
 
     def get(self):
         return self._value
 
     def set(self, value):
@@ -174,29 +174,29 @@
     def __str__(self):
         return "ScopedValue(%s)" % (self._value,)
 
     def __repr__(self):
         return "ScopedValue(%r)" % (self._value,)
 
 
-class _ScopedValueOverrideContext(object):
+class _ScopedValueOverrideContext:
     def __init__(self, target, value):
         self._target = target
         self._value = value
         self._old_value = None
 
     def __enter__(self):
         self._old_value = self._target._value
         self._target._value = self._value
 
     def __exit__(self, exc_type, exc_value, tb):
         self._target._value = self._old_value
 
 
-class _PropertyOverrideContext(object):
+class _PropertyOverrideContext:
     def __init__(self, target, property_name, value):
         self._target = target
         self._property_name = property_name
         self._value = value
         self._old_value = None
 
     def __enter__(self):
```

### Comparing `qcore-1.8.0/qcore/helpers.pyi` & `qcore-1.9.0/qcore/helpers.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -20,24 +20,24 @@
 empty_tuple: Tuple[Any, ...]
 empty_list: List[Any]
 empty_dict: Dict[Any, Any]
 
 def true_fn() -> bool: ...
 def false_fn() -> bool: ...
 
-class MarkerObject(object):
+class MarkerObject:
     name: Text
     def __init__(self, name: Text) -> None: ...
 
 none: MarkerObject
 miss: MarkerObject
 same: MarkerObject
 unspecified: MarkerObject
 
-class EmptyContext(object):
+class EmptyContext:
     def __enter__(self) -> None: ...
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
     ) -> None: ...
@@ -55,15 +55,15 @@
 class ScopedValue(Generic[_T]):
     def __init__(self, default: _T) -> None: ...
     def get(self) -> _T: ...
     def set(self, value: _T) -> None: ...
     def override(self, value: _T) -> ContextManager[None]: ...
     def __call__(self) -> _T: ...
 
-class _PropertyOverrideContext(object):
+class _PropertyOverrideContext:
     def __init__(self, target: object, property_name: str, value: object) -> None: ...
     def __enter__(self) -> None: ...
     def __exit__(
         self,
         exc_type: Optional[Type[BaseException]],
         exc_val: Optional[BaseException],
         exc_tb: Optional[TracebackType],
```

### Comparing `qcore-1.8.0/qcore/inspectable_class.py` & `qcore-1.9.0/qcore/inspectable_class.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 """
 
 Provides a base class overriding some useful dunder methods.
 
 """
 
 
-class InspectableClass(object):
+class InspectableClass:
     """Class that provides commonly useful dunder methods.
 
     This creates a useful repr/str representation, implements equality checking, and provides
     hashing.
 
     """
```

### Comparing `qcore-1.8.0/qcore/inspection.pxd` & `qcore-1.9.0/qcore/inspection.pxd`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/inspection.py` & `qcore-1.9.0/qcore/inspection.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 """
 
 Code inspection helpers.
 
 """
 
+from collections import namedtuple
 import functools
 import inspect
 import sys
 
 
 def get_original_fn(fn):
     """Gets the very original function of a decorated one."""
@@ -115,14 +116,20 @@
         else:
             result += ","
         result += str(k) + "=" + repr(v)
     result += ")"
     return result
 
 
+if sys.version_info >= (3, 10):
+    ArgSpec = namedtuple("ArgSpec", "args varargs keywords defaults")
+else:
+    ArgSpec = inspect.ArgSpec
+
+
 def getargspec(func):
     """Variation of inspect.getargspec that works for more functions.
 
     This function works for Cythonized, non-cpdef functions, which expose argspec information but
     are not accepted by getargspec. It also works for Python 3 functions that use annotations, which
     are simply ignored. However, keyword-only arguments are not supported.
 
@@ -133,15 +140,15 @@
     try:
         code = func.__code__
     except AttributeError:
         raise TypeError("{!r} is not a Python function".format(func))
     if hasattr(code, "co_kwonlyargcount") and code.co_kwonlyargcount > 0:
         raise ValueError("keyword-only arguments are not supported by getargspec()")
     args, varargs, varkw = inspect.getargs(code)
-    return inspect.ArgSpec(args, varargs, varkw, func.__defaults__)
+    return ArgSpec(args, varargs, varkw, func.__defaults__)
 
 
 def is_cython_or_generator(fn):
     """Returns whether this function is either a generator function or a Cythonized function."""
     if hasattr(fn, "__func__"):
         fn = fn.__func__  # Class method, static method
     if inspect.isgeneratorfunction(fn):
```

### Comparing `qcore-1.8.0/qcore/inspection.pyi` & `qcore-1.9.0/qcore/inspection.pyi`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/microtime.pxd` & `qcore-1.9.0/qcore/microtime.pxd`

 * *Files 6% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 
 cdef object _time_offset
 
 cpdef inline object get_time_offset()
 cpdef inline object set_time_offset(object offset)
 cpdef inline object add_time_offset(object offset)
 
-cdef class TimeOffset(object):
+cdef class TimeOffset:
     cdef object offset
 
 
 cpdef object utime()
 cpdef object true_utime()
 
-# NOTE(alex): Can't cpdef this because fo nested function
+# NOTE: Can't cpdef this because of nested function.
 #
 # cpdef execute_with_timeout(fn, tuple args=?, dict kwargs=?, timeout=?,
 #         bool fail_if_no_timer=?,
 #         signal_type=?,
 #         timer_type=?,
 #         timeout_exception_cls=?)
```

### Comparing `qcore-1.8.0/qcore/microtime.py` & `qcore-1.9.0/qcore/microtime.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,141 +10,198 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
 
-Helpers for dealing with time.
+Helpers for dealing with sub-second time.
 
-Assume that time is represented as an integer of microseconds.
+Here, time is represented as an integer of microseconds, a.k.a. "Utime".
 
 """
 
 __all__ = [
+    "DAY",
+    "HOUR",
     "MICROSECOND",
     "MILLISECOND",
-    "SECOND",
     "MINUTE",
-    "HOUR",
-    "DAY",
+    "MONTH_APPROXIMATE",
+    "SECOND",
     "WEEK",
     "YEAR_APPROXIMATE",
-    "MONTH_APPROXIMATE",
-    "utime_delta",
+    "TimeOffset",
+    "Utime",
+    "add_time_offset",
+    "datetime_as_utime",
+    "execute_with_timeout",
+    "format_utime_as_iso_8601",
     "get_time_offset",
     "set_time_offset",
-    "add_time_offset",
-    "TimeOffset",
-    "utime",
     "true_utime",
-    "execute_with_timeout",
-    "Utime",
+    "utime",
+    "utime_as_datetime",
+    "utime_delta",
 ]
 
-from functools import wraps
+
 import signal
-from time import time as _time
+from functools import wraps
+from time import time as _time_in_seconds
+from datetime import datetime, timezone
 from typing import NewType
 
 from . import inspection
 from .helpers import none, empty_tuple, empty_dict
 from .errors import TimeoutError, NotSupportedError
 
+
 Utime = NewType("Utime", int)
 
 
 MICROSECOND = 1
 MILLISECOND = MICROSECOND * 1000
 SECOND = MILLISECOND * 1000
 MINUTE = SECOND * 60
 HOUR = MINUTE * 60
 DAY = HOUR * 24
 WEEK = DAY * 7
 YEAR_APPROXIMATE = int(DAY * 365.25)
 MONTH_APPROXIMATE = int(YEAR_APPROXIMATE // 12)
 
-_time_offset = 0  # In microseconds (us)
 
+_offset_utime = 0  # type: Utime
 
-def _keyword_arguments_only(fn):
-    @wraps(fn)
-    def new_fn(**kwargs):
-        return fn(**kwargs)
 
-    return new_fn
-
-
-@_keyword_arguments_only
-def utime_delta(days=0, hours=0, minutes=0, seconds=0):
+def utime_delta(*, days=0, hours=0, minutes=0, seconds=0):
     """Gets time delta in microseconds.
 
     Note: Do NOT use this function without keyword arguments.
     It will become much-much harder to add extra time ranges later if positional arguments are used.
 
     """
     return (days * DAY) + (hours * HOUR) + (minutes * MINUTE) + (seconds * SECOND)
 
 
 def get_time_offset():
     """Gets the offset applied to time() function result in microseconds."""
-    global _time_offset
-    return _time_offset
+    global _offset_utime
+    return _offset_utime
 
 
 def set_time_offset(offset):
     """Sets the offset applied to time() function result in microseconds."""
-    global _time_offset
-    _time_offset = int(offset)
+    global _offset_utime
+    _offset_utime = int(offset)
 
 
 def add_time_offset(offset):
     """Adds specified number of microseconds to the offset applied to time() function result."""
-    global _time_offset
-    _time_offset += int(offset)
+    global _offset_utime
+    _offset_utime += int(offset)
 
 
-class TimeOffset(object):
+class TimeOffset:
     """Temporarily applies specified offset (in microseconds) to time() function result."""
 
     def __init__(self, offset):
         self.offset = int(offset)
 
     def __enter__(self):
-        global _time_offset
-        _time_offset += self.offset
+        global _offset_utime
+        _offset_utime += self.offset
 
     def __exit__(self, typ, value, traceback):
-        global _time_offset
-        _time_offset -= self.offset
+        global _offset_utime
+        _offset_utime -= self.offset
 
 
 def utime():
     """Gets current time in microseconds from the epoch time w/applied offset."""
-    return _time_offset + int(_time() * 1000000)
+    return _offset_utime + int(_time_in_seconds() * SECOND)
 
 
 def true_utime():
     """Gets current time in microseconds from the epoch time."""
-    return int(_time() * 1000000)
+    return int(_time_in_seconds() * SECOND)
+
+
+# ===================================================
+# Conversions to/from PY Date-Time
+# ===================================================
+
+
+def utime_as_datetime(utime, *, tz=timezone.utc):
+    """Get Python datetime instance for the given microseconds time.
+
+    This time refers to an absolute moment, given as microseconds from Unix Epoch.
+
+    """
+    return datetime.fromtimestamp(utime / SECOND, tz=tz)
+
+
+def datetime_as_utime(dt):
+    """Get the microseconds time for given Python datetime instance.
+
+    This time refers to an absolute moment, given as microseconds from Unix Epoch.
+
+    """
+    return int(dt.timestamp() * SECOND)
+
+
+# ===================================================
+# Conversions to/from ISO 8601 Date-Time
+# ===================================================
+
+
+def format_utime_as_iso_8601(utime, *, sep="T", drop_subseconds=False, tz=timezone.utc):
+    """Get ISO 8601 Time string for the given microseconds time.
+
+    Example output for the default UTC timezone:
+    "2022-10-31T18:02:03.123456+00:00"
+
+    """
+    timespec = "seconds" if drop_subseconds else "auto"
+    return utime_as_datetime(utime, tz=tz).isoformat(sep=sep, timespec=timespec)
+
+
+# datetime.fromisoformat() is new in Python 3.7.
+if hasattr(datetime, "fromisoformat"):
+
+    def iso_8601_as_utime(iso_datetime):
+        """Get the microseconds time for given ISO 8601 Time string.
+
+        Example input:
+        "2022-11-01T01:02:03.123456+07:00"
+
+        """
+        return datetime_as_utime(datetime.fromisoformat(iso_datetime))
+
+    __all__.append("iso_8601_as_utime")
+
+
+# ===================================================
+# Timeout API
+# ===================================================
 
 
 # Windows compatibility stuff
-_default_signal_type = signal.SIGALRM if hasattr(signal, "SIGALRM") else None
-_default_timer_type = signal.ITIMER_REAL if hasattr(signal, "ITIMER_REAL") else None
+_DEFAULT_SIGNAL_TYPE = signal.SIGALRM if hasattr(signal, "SIGALRM") else None
+_DEFAULT_TIMER_TYPE = signal.ITIMER_REAL if hasattr(signal, "ITIMER_REAL") else None
 
 
 def execute_with_timeout(
     fn,
     args=None,
     kwargs=None,
     timeout=None,
     fail_if_no_timer=True,
-    signal_type=_default_signal_type,
-    timer_type=_default_timer_type,
+    signal_type=_DEFAULT_SIGNAL_TYPE,
+    timer_type=_DEFAULT_TIMER_TYPE,
     timeout_exception_cls=TimeoutError,
 ):
     """
     Executes specified function with timeout. Uses SIGALRM to interrupt it.
 
     :type fn: function
     :param fn: function to execute
```

### Comparing `qcore-1.8.0/qcore/microtime.pyi` & `qcore-1.9.0/qcore/microtime.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import sys
+from datetime import datetime, timezone, tzinfo
 from typing import (
     Any,
     Callable,
     Iterable,
     Mapping,
     NewType,
     Optional,
@@ -28,28 +30,56 @@
 def utime_delta(
     *, days: int = ..., hours: int = ..., minutes: int = ..., seconds: int = ...
 ) -> Utime: ...
 def get_time_offset() -> Utime: ...
 def set_time_offset(offset: SupportsInt) -> None: ...
 def add_time_offset(offset: SupportsInt) -> None: ...
 
-class TimeOffset(object):
+class TimeOffset:
     """Temporarily applies specified offset (in microseconds) to time() function result."""
 
     def __init__(self, offset: SupportsInt) -> None: ...
     def __enter__(self) -> None: ...
     def __exit__(
         self,
         typ: Optional[Type[BaseException]],
         value: Optional[BaseException],
         traceback: Optional[TracebackType],
     ) -> None: ...
 
 def utime() -> Utime: ...
 def true_utime() -> Utime: ...
+
+# ===================================================
+# Conversions to/from PY Date-Time
+# ===================================================
+
+def utime_as_datetime(utime: Utime, *, tz: tzinfo = timezone.utc) -> datetime: ...
+def datetime_as_utime(dt: datetime) -> Utime: ...
+
+# ===================================================
+# Conversions to/from ISO 8601 Date-Time
+# ===================================================
+
+def format_utime_as_iso_8601(
+    utime: Utime,
+    *,
+    sep: str = "T",
+    drop_subseconds: bool = False,
+    tz: tzinfo = timezone.utc,
+) -> str: ...
+
+# datetime.fromisoformat() is new in Python 3.7.
+if sys.version_info >= (3, 7):
+    def iso_8601_as_utime(iso_datetime: str) -> Utime: ...
+
+# ===================================================
+# Timeout API
+# ===================================================
+
 def execute_with_timeout(
     fn: Callable[..., _T],
     args: Optional[Iterable[Any]] = ...,
     kwargs: Optional[Mapping[str, Any]] = ...,
     timeout: Optional[float] = ...,
     fail_if_no_timer: bool = ...,
     signal_type: int = ...,
```

### Comparing `qcore-1.8.0/qcore/testing.py` & `qcore-1.9.0/qcore/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
 
 import functools
 import inspect
 
 TEST_PREFIX = "test"
 
 
-class _Anything(object):
+class _Anything:
     def __eq__(self, other):
         return True
 
     def __ne__(self, other):
         return False
 
     def __repr__(self):
@@ -63,15 +63,15 @@
     def __hash__(self):
         return 0
 
 
 Anything = _Anything()
 
 
-class GreaterEq(object):
+class GreaterEq:
     """Greater than or equal to some value.
 
     For example, assert_eq(GreaterEq(2), 3) and assert_eq(GreaterEq(2), 2) succeed,
     while assert_eq(GreaterEq(3), 2) fails.
     Useful if only equality asserts are supported or if we need to
     check inequality in a subfield as part of an assert_eq on an object that contains it.
     """
@@ -119,14 +119,15 @@
         return decorate_class(func_or_class)
     else:
         assert False, "Must be used as a function or class decorator"
 
 
 def decorate_all_test_methods(decorator):
     """Decorator to apply another decorator to all test methods of a class."""
+
     # in python 3, unbound methods are just functions, so we also need to check for functions
     def predicate(member):
         return inspect.ismethod(member) or inspect.isfunction(member)
 
     def wrapper(cls):
         for name, m in inspect.getmembers(cls, predicate):
             if name.startswith(TEST_PREFIX):
```

### Comparing `qcore-1.8.0/qcore/tests/test_asserts.py` & `qcore-1.9.0/qcore/tests/test_asserts.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,15 +222,15 @@
     pass
 
 
 class SpecificException2(Exception):
     pass
 
 
-class TestAssertRaises(object):
+class TestAssertRaises:
     def test_handles_specific_exceptions(self):
         with AssertRaises(SpecificException, SpecificException2):
             raise SpecificException("foo")
 
     def test_handles_any_exceptions(self):
         with AssertRaises(Exception):
             raise Exception("foo")
```

### Comparing `qcore-1.8.0/qcore/tests/test_caching.py` & `qcore-1.9.0/qcore/tests/test_caching.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 import threading
 
 from unittest import mock
 from unittest.mock import MagicMock, call
 import pickle
 
 
-class TestLazyConstant(object):
+class TestLazyConstant:
     def test_decorator(self):
         self.is_computed = False
 
         @lazy_constant
         def test_function():
             assert_is(
                 False, self.is_computed, "test_function has been called more than once"
@@ -78,15 +78,15 @@
         assert_eq(42, lazy_constant.compute())
         assert self.is_called, "test_function has not been called"
         self.is_called = False
         assert_eq(42, lazy_constant.compute())
         assert self.is_called, "test_function has not been called"
 
 
-class TestThreadLocalLazyConstant(object):
+class TestThreadLocalLazyConstant:
     def test_thread_locality(self):
         lazy_constant = ThreadLocalLazyConstant(threading.current_thread)
         results = []
         lock = threading.RLock()
 
         def execute():
             with lock:
@@ -123,15 +123,15 @@
         assert self.is_called, "test_function has not been called"
         self.is_called = False
 
         assert_eq(42, lazy_constant.compute())
         assert self.is_called, "test_function has not been called"
 
 
-class TestLRUCache(object):
+class TestLRUCache:
     def test_deletion(self):
         # Zero capacity cache is not allowed
         with AssertRaises(ValueError):
             c = LRUCache(0)
 
         # Capacity = 1
         c = LRUCache(1)
@@ -273,15 +273,14 @@
         c.clear()
         self._check_order([], c)
         assert_eq(3, on_evict.call_count)
         assert_eq([call(0, "a"), call(1, "b"), call(2, "c")], on_evict.call_args_list)
 
 
 def test_lru_cache():
-
     calls = []
 
     @lru_cache(maxsize=3)
     def cube(n):
         calls.append(n)
         return n * n * n
 
@@ -341,15 +340,15 @@
     cube.clear()
     assert_eq(27, cube(3))
     assert_eq([1, 2, 3], calls)
     assert_eq(27, cube(1))
     assert_eq([1, 2, 3], calls)
 
 
-class TestClass(object):
+class TestClass:
     # not hashable
     __hash__ = None  # type: ignore
 
     def __init__(self, val):
         self.val = val
         self.x = 0
 
@@ -426,22 +425,21 @@
     assert_eq(2, object3.x)
     object3.with_variable_kwargs(k2=2)
     assert_eq(4, object3.x)
     object3.with_variable_kwargs(k1=2, k2=2)
     assert_eq(8, object3.x)
 
 
-class PickleTestClass(object):
+class PickleTestClass:
     @cached_per_instance()
     def f(self, x):
         return x
 
 
 def test_cached_per_instance_pickling():
-
     # make sure cached stuff doesn't appear in the pickled representation
 
     obj = PickleTestClass()
     obj.attr = "spam"
     assert_eq(set(), set(PickleTestClass.f.__cached_per_instance_cache__.keys()))
     obj.f("my hovercraft is full of eels")
     assert_eq({id(obj)}, set(PickleTestClass.f.__cached_per_instance_cache__.keys()))
@@ -457,15 +455,15 @@
         {id(obj), id(restored)},
         set(PickleTestClass.f.__cached_per_instance_cache__.keys()),
     )
     assert_eq("spam", obj.attr)
 
     # make sure we can use this with a custom __getstate__
 
-    class X(object):
+    class X:
         @cached_per_instance()
         def f(self, x):
             return x
 
         def __getstate__(self):
             return {}
```

### Comparing `qcore-1.8.0/qcore/tests/test_debug.py` & `qcore-1.9.0/qcore/tests/test_debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
     counter.decrement(3)
     assert_eq("DebugCounter('test_debug_counter', value=2)", str(counter))
     assert_eq("DebugCounter('test_debug_counter', value=2)", repr(counter))
 
 
 def test_bool_by_mask():
-    class MaskObject(object):
+    class MaskObject:
         def __init__(self):
             self.TEST_MASK_1 = False
             self.TEST_MASK_2 = True
 
     m = MaskObject()
     assert_is(True, get_bool_by_mask(m, "ABC"))
     assert_is(False, get_bool_by_mask(m, "TEST_MASK"))
```

### Comparing `qcore-1.8.0/qcore/tests/test_decorators.py` & `qcore-1.9.0/qcore/tests/test_decorators.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 
 @deprecated("Deprecated.")
 def deprecated_fn():
     pass
 
 
 @deprecated("Deprecated.")
-class DeprecatedClass(object):
+class DeprecatedClass:
     pass
 
 
 def test_deprecated():
     fn = deprecated_fn
     fn.__doc__.startswith("Deprecated")
 
@@ -66,15 +66,15 @@
 
 
 @retry(Exception)
 def retry_it():
     pass
 
 
-class TestRetry(object):
+class TestRetry:
     def create_generator_function(self, exception_type, max_tries):
         fn_body = mock.Mock()
         fn_body.return_value = range(3)
 
         @retry(exception_type, max_tries=max_tries)
         def any_function(*args, **kwargs):
             for it in fn_body(*args, **kwargs):
@@ -175,23 +175,21 @@
 
     def test_retry_preserves_argspec(self):
         def fn(foo, bar, baz=None, **kwargs):
             pass
 
         decorated = retry(Exception)(fn)
 
-        assert_eq(
-            inspect.getargspec(fn), inspect.getargspec(get_original_fn(decorated))
-        )
+        assert_eq(inspect.signature(fn), inspect.signature(get_original_fn(decorated)))
 
 
 def test_decorator_of_context_manager():
     data = []
 
-    class Context(object):
+    class Context:
         "Dummy context"
 
         def __init__(self, key):
             self.key = key
 
         def __enter__(self):
             data.append("enter %s" % self.key)
@@ -207,15 +205,15 @@
 
     assert_eq("Dummy context", decorator.__doc__)
 
     decorated()
 
     assert_eq(["enter maras", "inside maras", "exit maras"], data)
 
-    class NoDocString(object):
+    class NoDocString:
         def __enter__(self):
             pass
 
         def __exit__(self, *args):
             pass
 
     assert_eq(
@@ -286,15 +284,15 @@
 @cached
 def f(a, b):
     global i
     i += 1
     return a + b + i
 
 
-class CachedMethods(object):
+class CachedMethods:
     @cached
     def f(self, a, b):
         global i
         i += 1
         return a + b + i
 
     @cached
@@ -322,15 +320,15 @@
     def __str__(self):
         return "CachedMethods()"
 
     def __repr__(self):
         return str(self)
 
 
-class TestDecorators(object):
+class TestDecorators:
     def setup(self):
         global i
         i = 0
 
     def test_cached(self):
         global i
         instance = CachedMethods()
@@ -364,16 +362,18 @@
     def test_decorator_str_and_repr(self):
         cases = [
             (f, "@cached test_decorators.f"),
             (CachedMethods().f, "<@cached test_decorators.f bound to CachedMethods()>"),
             (CachedMethods.f, "<@cached test_decorators.f unbound>"),
             (
                 CachedMethods.cached_classmethod,
-                "<@cached test_decorators.cached_classmethod bound to <class "
-                "'test_decorators.CachedMethods'>>",
+                (
+                    "<@cached test_decorators.cached_classmethod bound to <class "
+                    "'test_decorators.CachedMethods'>>"
+                ),
             ),
             (
                 CachedMethods.cached_staticmethod,
                 "@cached test_decorators.cached_staticmethod",
             ),
         ]
         for method, expected in cases:
```

### Comparing `qcore-1.8.0/qcore/tests/test_enum.py` & `qcore-1.9.0/qcore/tests/test_enum.py`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/tests/test_errors.py` & `qcore-1.9.0/qcore/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/tests/test_events.py` & `qcore-1.9.0/qcore/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/tests/test_examples.py` & `qcore-1.9.0/qcore/tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/qcore/tests/test_helpers.py` & `qcore-1.9.0/qcore/tests/test_helpers.py`

 * *Files 8% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             raise NotImplementedError()
     except NotImplementedError:
         pass
     assert_eq(v(), "a")
 
 
 def test_override():
-    class TestObject(object):
+    class TestObject:
         def __init__(self):
             self.v = None
 
     o = TestObject()
     o.v = "a"
 
     with qcore.override(o, "v", "b"):
@@ -117,15 +117,15 @@
     assert_eq(1, g.hi)
     assert_eq(2, g.hello)
     assert_eq(6, g._hi)
     assert_eq(7, g._hello)
     assert_ne(g.__code__, f.__code__)
     assert_ne(g.__name__, f.__name__)
 
-    class A(object):
+    class A:
         pass
 
     a1 = A()
     a1._hey = 0
     a1.hi = 1
     a1.hello = 2
     a1._hi = 3
@@ -159,15 +159,15 @@
     assert_eq(1, a2.hi)
     assert_eq(2, a2.hello)
     assert_eq(6, a2._hi)
     assert_eq(7, a2._hello)
 
 
 def test_cached_hash_wrapper():
-    class TestClass(object):
+    class TestClass:
         pass
 
     w1a = qcore.CachedHashWrapper(TestClass())
     w1b = qcore.CachedHashWrapper(w1a())
     w2a = qcore.CachedHashWrapper(TestClass())
 
     print("w1a", w1a)
@@ -232,15 +232,15 @@
 def test_ellipsis():
     assert_eq("abcdef", qcore.ellipsis("abcdef", 0))
     assert_eq("abcdef", qcore.ellipsis("abcdef", 10))
     assert_eq("ab...", qcore.ellipsis("abcdef", 5))
 
 
 def test_safe_representation():
-    class TestObject(object):
+    class TestObject:
         """A test object that has neither __str__ nor __repr__."""
 
         def __str__(self):
             return NotImplementedError()
 
         def __repr__(self):
             return NotImplementedError()
```

### Comparing `qcore-1.8.0/qcore/tests/test_inspectable_class.py` & `qcore-1.9.0/qcore/tests/test_inspectable_class.py`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 class ObjectWithSlots(InspectableClass):
     __slots__ = ("oid",)
 
     def __init__(self, oid):
         self.oid = oid
 
 
-class TestObjectWithDictComparison(object):
+class TestObjectWithDictComparison:
     def _check_repr_and_str(self, expected, obj):
         assert_eq(expected, repr(obj))
         assert_eq(expected, str(obj))
 
     def test_compare_objects(self):
         assert_eq(SimpleObjectWithDictComparison(), SimpleObjectWithDictComparison())
         assert_eq(
```

### Comparing `qcore-1.8.0/qcore/tests/test_inspection.py` & `qcore-1.9.0/qcore/tests/test_inspection.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,33 +10,32 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import qcore
 from qcore.asserts import assert_eq, assert_ne, assert_unordered_list_eq, AssertRaises
-import inspect
 
 
-class NonCython(object):
+class NonCython:
     pass
 
 
 class InheritFromCython(qcore.caching.LazyConstant):
     pass
 
 
 def test_is_cython_class():
     if qcore.caching.__file__.endswith(".so"):
         assert qcore.inspection.is_cython_class(qcore.caching.LazyConstant)
     assert not qcore.inspection.is_cython_class(NonCython)
     assert not qcore.inspection.is_cython_class(InheritFromCython)
 
 
-class A(object):
+class A:
     pass
 
 
 class B(A):
     pass
 
 
@@ -62,60 +61,55 @@
 
 
 def fun_with_args(a, b, c, d="e", **f):
     pass
 
 
 def test_getargspec():
-    empty = inspect.ArgSpec(args=[], varargs=None, keywords=None, defaults=None)
+    empty = qcore.inspection.ArgSpec(
+        args=[], varargs=None, keywords=None, defaults=None
+    )
     assert_eq(empty, qcore.inspection.getargspec(test_get_subclass_tree))
     assert_eq(empty, qcore.inspection.getargspec(qcore.inspection.lazy_stack))
 
-    emptymethod = inspect.ArgSpec(
+    emptymethod = qcore.inspection.ArgSpec(
         args=["self"], varargs=None, keywords=None, defaults=None
     )
     assert_eq(emptymethod, qcore.inspection.getargspec(X.myinstancemethod))
     assert_eq(emptymethod, qcore.inspection.getargspec(X().myinstancemethod))
 
-    emptyclsmethod = inspect.ArgSpec(
+    emptyclsmethod = qcore.inspection.ArgSpec(
         args=["cls"], varargs=None, keywords=None, defaults=None
     )
     assert_eq(emptyclsmethod, qcore.inspection.getargspec(X.myclassmethod))
 
-    spec = inspect.ArgSpec(
+    spec = qcore.inspection.ArgSpec(
         args=["a", "b", "c", "d"], varargs=None, keywords="f", defaults=("e",)
     )
     assert_eq(spec, qcore.inspection.getargspec(fun_with_args))
 
 
-try:
-    exec(
-        """
 def fun_with_annotations(a: int, b: str, *args) -> None:
     pass
 
 
 def fun_with_kwonly_args(a=1, *, b, c=3):
     pass
-"""
-    )
-except SyntaxError:
-    pass
-else:
 
-    def test_getargspec_py3_only():
-        spec = inspect.ArgSpec(
-            args=["a", "b"], varargs="args", keywords=None, defaults=None
-        )
-        assert_eq(spec, qcore.inspection.getargspec(fun_with_annotations))
-        with AssertRaises(ValueError):
-            qcore.inspection.getargspec(fun_with_kwonly_args)
+
+def test_getargspec_py3_only():
+    spec = qcore.inspection.ArgSpec(
+        args=["a", "b"], varargs="args", keywords=None, defaults=None
+    )
+    assert_eq(spec, qcore.inspection.getargspec(fun_with_annotations))
+    with AssertRaises(ValueError):
+        qcore.inspection.getargspec(fun_with_kwonly_args)
 
 
-class X(object):
+class X:
     @classmethod
     def myclassmethod(cls):
         pass
 
     def myinstancemethod(self):
         pass
 
@@ -125,15 +119,15 @@
     def myclassmethod(cls):
         pass
 
     def myinstancemethod(self):
         pass
 
 
-class BoolConversionFails(object):
+class BoolConversionFails:
     def method(self):
         pass
 
     def __nonzero__(self):
         raise TypeError("Cannot convert %s to bool" % self)
 
     __bool__ = __nonzero__
@@ -156,15 +150,15 @@
     assert not qcore.inspection.is_classmethod(OldStyle.myinstancemethod)
     assert not qcore.inspection.is_classmethod(OldStyle().myinstancemethod)
     # this throws an error if you do "not im_self"
     assert not qcore.inspection.is_classmethod(BoolConversionFails().method)
 
 
 def test_get_function_call_str():
-    class TestObject(object):
+    class TestObject:
         """A test object containing no __str__ implementation."""
 
         def __str__(self):
             raise NotImplementedError()
 
         def __repr__(self):
             return "test"
```

### Comparing `qcore-1.8.0/qcore/tests/test_testing.py` & `qcore-1.9.0/qcore/tests/test_testing.py`

 * *Files 11% similar despite different names*

```diff
@@ -61,25 +61,25 @@
     @disabled
     def fn():
         pass
 
     _check_disabled(fn)
 
     @disabled
-    class TestCls(object):
+    class TestCls:
         def test_method(self):
             return marker
 
         def normal_method(self):
             return marker
 
     _check_disabled(TestCls().test_method)
     assert_is(marker, TestCls().normal_method())
 
-    class TestCls2(object):
+    class TestCls2:
         def test_method(self):
             return marker
 
         @disabled
         def test_method_disabled(self):
             return marker
 
@@ -104,15 +104,15 @@
 
 
 def decorator(method):
     return marker
 
 
 def _get_decoratable_class():
-    class Cls(object):
+    class Cls:
         pass
 
     Cls.normal_method = normal_method
 
     test_method = lambda self: None
     setattr(Cls, test_method_name, test_method)
     assert_eq(test_method.__get__(None, Cls), getattr(Cls, test_method_name))
```

### Comparing `qcore-1.8.0/qcore.egg-info/PKG-INFO` & `qcore-1.9.0/qcore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,206 +1,206 @@
 Metadata-Version: 2.1
 Name: qcore
-Version: 1.8.0
+Version: 1.9.0
 Summary: Quora's core utility library
 Home-page: https://github.com/quora/qcore
 Author: Quora, Inc.
 Author-email: asynq@quora.com
 License: Apache Software License
-Description: *****
-        qcore
-        *****
-        
-        ``qcore`` is a library of common utility functions used at Quora. It is used to
-        abstract out common functionality for other Quora libraries like `asynq <https://github.com/quora/asynq>`_.
-        
-        Its component modules are discussed below. See the docstrings in the code
-        itself for more detail.
-        
-        qcore.asserts
-        -------------
-        
-        When a normal Python assert fails, it only indicates that there was a failure,
-        not what the bad values were that caused the assert to fail. This module
-        provides rich assertion helpers that automatically produce better error
-        messages. For example:
-        
-        .. code-block:: python
-        
-            >>> from qcore.asserts import assert_eq
-            >>> assert 5 == 2 * 2
-            Traceback (most recent call last):
-              File "<stdin>", line 1, in <module>
-            AssertionError
-            >>> assert_eq(5, 2 * 2)
-            Traceback (most recent call last):
-              File "<stdin>", line 1, in <module>
-              File "qcore/asserts.py", line 82, in assert_eq
-                assert expected == actual, _assert_fail_message(message, expected, actual, '!=', extra)
-            AssertionError: 5 != 4
-        
-        Similar methods are provided by the standard library's ``unittest`` package,
-        but those are tied to the ``TestCase`` class instead of being standalone
-        functions.
-        
-        qcore.caching
-        -------------
-        
-        This provides helpers for caching data. Some examples include:
-        
-        .. code-block:: python
-        
-            from qcore.caching import cached_per_instance, lazy_constant
-        
-            @lazy_constant
-            def some_function():
-                # this will only be executed the first time some_function() is called;
-                # afterwards it will be cached
-                return expensive_computation()
-        
-            class SomeClass(object):
-                @cached_per_instance()
-                def some_method(self, a, b):
-                    # for any instance of SomeClass, this will only be executed once
-                    return expensive_computation(a, b)
-        
-        qcore.debug
-        -----------
-        
-        This module provides some helpers useful for debugging Python. Among others, it
-        includes the ``@qcore.debug.trace()`` decorator, which can be used to trace
-        every time a function is called.
-        
-        qcore.decorators
-        ----------------
-        
-        This module provides an abstraction for class-based decorators that supports
-        transparently decorating functions, methods, classmethods, and staticmethods
-        while also providing the option to add additional custom attributes. For
-        example, it could be used to provide a caching decorator that adds a ``.dirty``
-        attribute to decorated functions to dirty their cache:
-        
-        .. code-block:: python
-        
-            from qcore.decorators import DecoratorBase, DecoratorBinder, decorate
-        
-            class CacheDecoratorBinder(DecoratorBinder):
-                def dirty(self, *args):
-                    if self.instance is None:
-                        return self.decorator.dirty(*args)
-                    else:
-                        return self.decorator.dirty(self.instance, *args)
-        
-            class CacheDecorator(DecoratorBase):
-                binder_cls = CacheDecoratorBinder
-        
-                def __init__(self, *args):
-                    super().__init__(*args)
-                    self._cache = {}
-        
-                def dirty(self, *args):
-                    try:
-                        del self._cache[args]
-                    except KeyError:
-                        pass
-        
-                def __call__(self, *args):
-                    try:
-                        return self._cache[args]
-                    except KeyError:
-                        value = self.fn(*args)
-                        self._cache[args] = value
-                        return value
-        
-            cached = decorate(CacheDecorator)
-        
-        qcore.enum
-        ----------
-        
-        This module provides an abstraction for defining enums. You can define an enum
-        as follows:
-        
-        .. code-block:: python
-        
-            from qcore.enum import Enum
-        
-            class Color(Enum):
-                red = 1
-                green = 2
-                blue = 3
-        
-        qcore.errors
-        ------------
-        
-        This module provides some commonly useful exception classes and helpers for
-        reraising exceptions from a different place.
-        
-        qcore.events
-        ------------
-        
-        This provides an abstraction for registering events and running callbacks.
-        Example usage:
-        
-        .. code-block:: python
-        
-            >>> from qcore.events import EventHook
-            >>> event = EventHook()
-            >>> def callback():
-            ...     print('callback called')
-            ...
-            >>> event.subscribe(callback)
-            >>> event.trigger()
-            callback called
-        
-        qcore.helpers
-        -------------
-        
-        This provides a number of small helper functions.
-        
-        qcore.inspectable_class
-        -----------------------
-        
-        This provides a base class that automatically provides hashing, equality
-        checks, and a readable ``repr()`` result. Example usage:
-        
-        .. code-block:: python
-        
-            >>> from qcore.inspectable_class import InspectableClass
-            >>> class Pair(InspectableClass):
-            ...     def __init__(self, a, b):
-            ...         self.a = a
-            ...         self.b = b
-            ...
-            >>> Pair(1, 2)
-            Pair(a=1, b=2)
-            >>> Pair(1, 2) == Pair(1, 2)
-            True
-        
-        qcore.inspection
-        ----------------
-        
-        This provides functionality similar to the standard ``inspect`` module. Among
-        others, it includes the ``get_original_fn`` function, which extracts the
-        underlying function from a ``qcore.decorators``-decorated object.
-        
-        qcore.microtime
-        ---------------
-        
-        This includes helpers for dealing with time, represented as an integer number
-        of microseconds since the Unix epoch.
-        
-        qcore.testing
-        -------------
-        
-        This provides helpers to use in unit tests. Among others, it provides an
-        ``Anything`` object that compares equal to any other Python object.
-        
 Keywords: quora core common utility
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/x-rst
+License-File: LICENSE
+
+*****
+qcore
+*****
+
+``qcore`` is a library of common utility functions used at Quora. It is used to
+abstract out common functionality for other Quora libraries like `asynq <https://github.com/quora/asynq>`_.
+
+Its component modules are discussed below. See the docstrings in the code
+itself for more detail.
+
+qcore.asserts
+-------------
+
+When a normal Python assert fails, it only indicates that there was a failure,
+not what the bad values were that caused the assert to fail. This module
+provides rich assertion helpers that automatically produce better error
+messages. For example:
+
+.. code-block:: python
+
+    >>> from qcore.asserts import assert_eq
+    >>> assert 5 == 2 * 2
+    Traceback (most recent call last):
+      File "<stdin>", line 1, in <module>
+    AssertionError
+    >>> assert_eq(5, 2 * 2)
+    Traceback (most recent call last):
+      File "<stdin>", line 1, in <module>
+      File "qcore/asserts.py", line 82, in assert_eq
+        assert expected == actual, _assert_fail_message(message, expected, actual, '!=', extra)
+    AssertionError: 5 != 4
+
+Similar methods are provided by the standard library's ``unittest`` package,
+but those are tied to the ``TestCase`` class instead of being standalone
+functions.
+
+qcore.caching
+-------------
+
+This provides helpers for caching data. Some examples include:
+
+.. code-block:: python
+
+    from qcore.caching import cached_per_instance, lazy_constant
+
+    @lazy_constant
+    def some_function():
+        # this will only be executed the first time some_function() is called;
+        # afterwards it will be cached
+        return expensive_computation()
+
+    class SomeClass:
+        @cached_per_instance()
+        def some_method(self, a, b):
+            # for any instance of SomeClass, this will only be executed once
+            return expensive_computation(a, b)
+
+qcore.debug
+-----------
+
+This module provides some helpers useful for debugging Python. Among others, it
+includes the ``@qcore.debug.trace()`` decorator, which can be used to trace
+every time a function is called.
+
+qcore.decorators
+----------------
+
+This module provides an abstraction for class-based decorators that supports
+transparently decorating functions, methods, classmethods, and staticmethods
+while also providing the option to add additional custom attributes. For
+example, it could be used to provide a caching decorator that adds a ``.dirty``
+attribute to decorated functions to dirty their cache:
+
+.. code-block:: python
+
+    from qcore.decorators import DecoratorBase, DecoratorBinder, decorate
+
+    class CacheDecoratorBinder(DecoratorBinder):
+        def dirty(self, *args):
+            if self.instance is None:
+                return self.decorator.dirty(*args)
+            else:
+                return self.decorator.dirty(self.instance, *args)
+
+    class CacheDecorator(DecoratorBase):
+        binder_cls = CacheDecoratorBinder
+
+        def __init__(self, *args):
+            super().__init__(*args)
+            self._cache = {}
+
+        def dirty(self, *args):
+            try:
+                del self._cache[args]
+            except KeyError:
+                pass
+
+        def __call__(self, *args):
+            try:
+                return self._cache[args]
+            except KeyError:
+                value = self.fn(*args)
+                self._cache[args] = value
+                return value
+
+    cached = decorate(CacheDecorator)
+
+qcore.enum
+----------
+
+This module provides an abstraction for defining enums. You can define an enum
+as follows:
+
+.. code-block:: python
+
+    from qcore.enum import Enum
+
+    class Color(Enum):
+        red = 1
+        green = 2
+        blue = 3
+
+qcore.errors
+------------
+
+This module provides some commonly useful exception classes and helpers for
+reraising exceptions from a different place.
+
+qcore.events
+------------
+
+This provides an abstraction for registering events and running callbacks.
+Example usage:
+
+.. code-block:: python
+
+    >>> from qcore.events import EventHook
+    >>> event = EventHook()
+    >>> def callback():
+    ...     print('callback called')
+    ...
+    >>> event.subscribe(callback)
+    >>> event.trigger()
+    callback called
+
+qcore.helpers
+-------------
+
+This provides a number of small helper functions.
+
+qcore.inspectable_class
+-----------------------
+
+This provides a base class that automatically provides hashing, equality
+checks, and a readable ``repr()`` result. Example usage:
+
+.. code-block:: python
+
+    >>> from qcore.inspectable_class import InspectableClass
+    >>> class Pair(InspectableClass):
+    ...     def __init__(self, a, b):
+    ...         self.a = a
+    ...         self.b = b
+    ...
+    >>> Pair(1, 2)
+    Pair(a=1, b=2)
+    >>> Pair(1, 2) == Pair(1, 2)
+    True
+
+qcore.inspection
+----------------
+
+This provides functionality similar to the standard ``inspect`` module. Among
+others, it includes the ``get_original_fn`` function, which extracts the
+underlying function from a ``qcore.decorators``-decorated object.
+
+qcore.microtime
+---------------
+
+This includes helpers for dealing with time, represented as an integer number
+of microseconds since the Unix epoch.
+
+qcore.testing
+-------------
+
+This provides helpers to use in unit tests. Among others, it provides an
+``Anything`` object that compares equal to any other Python object.
```

### Comparing `qcore-1.8.0/qcore.egg-info/SOURCES.txt` & `qcore-1.9.0/qcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qcore-1.8.0/setup.py` & `qcore-1.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 DATA_FILES = (
     ["py.typed"]
     + ["%s.pxd" % module for module in CYTHON_MODULES]
     + [os.path.relpath(f, "qcore/") for f in glob.glob("qcore/*.pyi")]
 )
 
 
-VERSION = "1.8.0"
+VERSION = "1.9.0"
 
 
 EXTENSIONS = [
     Extension("qcore.%s" % module, ["qcore/%s.py" % module])
     for module in CYTHON_MODULES
 ]
 
@@ -58,19 +58,19 @@
         long_description=long_description,
         long_description_content_type="text/x-rst",
         url="https://github.com/quora/qcore",
         license="Apache Software License",
         classifiers=[
             "License :: OSI Approved :: Apache Software License",
             "Programming Language :: Python",
-            "Programming Language :: Python :: 3.6",
             "Programming Language :: Python :: 3.7",
             "Programming Language :: Python :: 3.8",
             "Programming Language :: Python :: 3.9",
             "Programming Language :: Python :: 3.10",
+            "Programming Language :: Python :: 3.11",
         ],
         keywords="quora core common utility",
         packages=["qcore", "qcore.tests"],
         package_data={"qcore": DATA_FILES},
         ext_modules=EXTENSIONS,
         setup_requires=["Cython"],
         install_requires=["Cython"],
```

