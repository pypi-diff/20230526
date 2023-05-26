# Comparing `tmp/wtisdk-1.1.tar.gz` & `tmp/wtisdk-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wtisdk-1.1.tar", last modified: Fri May 26 20:12:31 2023, max compression
+gzip compressed data, was "wtisdk-1.2.tar", last modified: Fri May 26 20:16:23 2023, max compression
```

## Comparing `wtisdk-1.1.tar` & `wtisdk-1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:12:31.892651 wtisdk-1.1/
--rw-r--r--   0 MTeke1     (502) staff       (20)     2123 2023-05-26 20:12:31.892511 wtisdk-1.1/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      648 2023-05-26 20:12:23.000000 wtisdk-1.1/README.md
--rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-05-26 20:12:31.892708 wtisdk-1.1/setup.cfg
--rw-r--r--   0 MTeke1     (502) staff       (20)     2152 2023-05-26 20:09:14.000000 wtisdk-1.1/setup.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:12:31.890735 wtisdk-1.1/wtisdk/
--rw-r--r--   0 MTeke1     (502) staff       (20)       28 2023-05-26 20:01:08.000000 wtisdk-1.1/wtisdk/__init__.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:12:31.892203 wtisdk-1.1/wtisdk/tests/
--rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-05-26 17:07:10.000000 wtisdk-1.1/wtisdk/tests/__init__.py
--rw-r--r--   0 MTeke1     (502) staff       (20)      714 2023-05-26 19:17:23.000000 wtisdk-1.1/wtisdk/tests/test_wtisdk.py
--rw-r--r--   0 MTeke1     (502) staff       (20)    37138 2023-05-26 19:02:26.000000 wtisdk-1.1/wtisdk/wtisdk.py
-drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:12:31.891922 wtisdk-1.1/wtisdk.egg-info/
--rw-r--r--   0 MTeke1     (502) staff       (20)     2123 2023-05-26 20:12:31.000000 wtisdk-1.1/wtisdk.egg-info/PKG-INFO
--rw-r--r--   0 MTeke1     (502) staff       (20)      256 2023-05-26 20:12:31.000000 wtisdk-1.1/wtisdk.egg-info/SOURCES.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-05-26 20:12:31.000000 wtisdk-1.1/wtisdk.egg-info/dependency_links.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)       17 2023-05-26 20:12:31.000000 wtisdk-1.1/wtisdk.egg-info/requires.txt
--rw-r--r--   0 MTeke1     (502) staff       (20)        7 2023-05-26 20:12:31.000000 wtisdk-1.1/wtisdk.egg-info/top_level.txt
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:16:23.736906 wtisdk-1.2/
+-rw-r--r--   0 MTeke1     (502) staff       (20)     2123 2023-05-26 20:16:23.736718 wtisdk-1.2/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)      648 2023-05-26 20:13:15.000000 wtisdk-1.2/README.md
+-rw-r--r--   0 MTeke1     (502) staff       (20)       38 2023-05-26 20:16:23.737001 wtisdk-1.2/setup.cfg
+-rw-r--r--   0 MTeke1     (502) staff       (20)     2152 2023-05-26 20:16:17.000000 wtisdk-1.2/setup.py
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:16:23.734009 wtisdk-1.2/wtisdk/
+-rw-r--r--   0 MTeke1     (502) staff       (20)       35 2023-05-26 20:16:12.000000 wtisdk-1.2/wtisdk/__init__.py
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:16:23.736211 wtisdk-1.2/wtisdk/tests/
+-rw-r--r--   0 MTeke1     (502) staff       (20)        0 2023-05-26 17:07:10.000000 wtisdk-1.2/wtisdk/tests/__init__.py
+-rw-r--r--   0 MTeke1     (502) staff       (20)      714 2023-05-26 19:17:23.000000 wtisdk-1.2/wtisdk/tests/test_wtisdk.py
+-rw-r--r--   0 MTeke1     (502) staff       (20)    37138 2023-05-26 19:02:26.000000 wtisdk-1.2/wtisdk/wtisdk.py
+drwxr-xr-x   0 MTeke1     (502) staff       (20)        0 2023-05-26 20:16:23.735914 wtisdk-1.2/wtisdk.egg-info/
+-rw-r--r--   0 MTeke1     (502) staff       (20)     2123 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/PKG-INFO
+-rw-r--r--   0 MTeke1     (502) staff       (20)      256 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/SOURCES.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        1 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/dependency_links.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)       17 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/requires.txt
+-rw-r--r--   0 MTeke1     (502) staff       (20)        7 2023-05-26 20:16:23.000000 wtisdk-1.2/wtisdk.egg-info/top_level.txt
```

### Comparing `wtisdk-1.1/PKG-INFO` & `wtisdk-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.1
+Version: 1.2
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Description: 
                                 WTI SDK: Python SDK for interacting with WTI devices
```

### Comparing `wtisdk-1.1/README.md` & `wtisdk-1.2/README.md`

 * *Files identical despite different names*

### Comparing `wtisdk-1.1/setup.py` & `wtisdk-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='wtisdk',
-    version='1.1',
+    version='1.2',
     author='Melih Teke',
     author_email='me@mteke.com',
     description='WTI SDK for interacting with WTI devices',
     long_description='''
                         WTI SDK: Python SDK for interacting with WTI devices
 
                         The WTI SDK is a powerful Python library that enables developers to easily interact with WTI devices, providing a comprehensive set of functions for managing and controlling operational and configuration aspects.
```

### Comparing `wtisdk-1.1/wtisdk/tests/test_wtisdk.py` & `wtisdk-1.2/wtisdk/tests/test_wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.1/wtisdk/wtisdk.py` & `wtisdk-1.2/wtisdk/wtisdk.py`

 * *Files identical despite different names*

### Comparing `wtisdk-1.1/wtisdk.egg-info/PKG-INFO` & `wtisdk-1.2/wtisdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wtisdk
-Version: 1.1
+Version: 1.2
 Summary: WTI SDK for interacting with WTI devices
 Home-page: https://github.com/melihteke/wtisdk
 Author: Melih Teke
 Author-email: me@mteke.com
 License: UNKNOWN
 Description: 
                                 WTI SDK: Python SDK for interacting with WTI devices
```

