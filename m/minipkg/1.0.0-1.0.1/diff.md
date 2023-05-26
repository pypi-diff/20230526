# Comparing `tmp/minipkg-1.0.0.tar.gz` & `tmp/minipkg-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minipkg-1.0.0.tar", last modified: Fri May 26 16:17:33 2023, max compression
+gzip compressed data, was "minipkg-1.0.1.tar", last modified: Fri May 26 17:32:22 2023, max compression
```

## Comparing `minipkg-1.0.0.tar` & `minipkg-1.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 16:17:33.379109 minipkg-1.0.0/
--rw-rw-rw-   0        0        0     1359 2023-05-24 05:25:07.000000 minipkg-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     1189 2023-05-26 16:17:33.375111 minipkg-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1972 2023-05-26 15:44:24.000000 minipkg-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 16:17:33.370113 minipkg-1.0.0/minipkg.egg-info/
--rw-rw-rw-   0        0        0     1189 2023-05-26 16:17:33.000000 minipkg-1.0.0/minipkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-05-26 16:17:33.000000 minipkg-1.0.0/minipkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 16:17:33.000000 minipkg-1.0.0/minipkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 16:17:33.000000 minipkg-1.0.0/minipkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 16:17:33.000000 minipkg-1.0.0/minipkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    13388 2023-05-26 16:07:16.000000 minipkg-1.0.0/minipy.py
--rw-rw-rw-   0        0        0      104 2023-05-24 03:36:59.000000 minipkg-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 16:17:33.379109 minipkg-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1297 2023-05-26 15:52:11.000000 minipkg-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:32:22.062166 minipkg-1.0.1/
+-rw-rw-rw-   0        0        0     1359 2023-05-24 05:25:07.000000 minipkg-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     1189 2023-05-26 17:32:22.062166 minipkg-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1972 2023-05-26 15:44:24.000000 minipkg-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 17:32:22.062166 minipkg-1.0.1/minipkg.egg-info/
+-rw-rw-rw-   0        0        0     1189 2023-05-26 17:32:21.000000 minipkg-1.0.1/minipkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      205 2023-05-26 17:32:21.000000 minipkg-1.0.1/minipkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:32:21.000000 minipkg-1.0.1/minipkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 17:32:21.000000 minipkg-1.0.1/minipkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 17:32:21.000000 minipkg-1.0.1/minipkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13388 2023-05-26 16:07:16.000000 minipkg-1.0.1/minipy.py
+-rw-rw-rw-   0        0        0      104 2023-05-24 03:36:59.000000 minipkg-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 17:32:22.062166 minipkg-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1297 2023-05-26 17:31:19.000000 minipkg-1.0.1/setup.py
```

### Comparing `minipkg-1.0.0/LICENSE` & `minipkg-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `minipkg-1.0.0/PKG-INFO` & `minipkg-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minipkg
-Version: 1.0.0
+Version: 1.0.1
 Summary: All the power of Python...in the palm of your hand.
 Author: Omer Drkić
 Author-email: omerdrkic2501@gmail.com
 License: Boost Software License 1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Framework :: Jupyter
```

### Comparing `minipkg-1.0.0/README.md` & `minipkg-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `minipkg-1.0.0/minipkg.egg-info/PKG-INFO` & `minipkg-1.0.1/minipkg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minipkg
-Version: 1.0.0
+Version: 1.0.1
 Summary: All the power of Python...in the palm of your hand.
 Author: Omer Drkić
 Author-email: omerdrkic2501@gmail.com
 License: Boost Software License 1.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Framework :: Jupyter
```

### Comparing `minipkg-1.0.0/minipy.py` & `minipkg-1.0.1/minipy.py`

 * *Files identical despite different names*

### Comparing `minipkg-1.0.0/setup.py` & `minipkg-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ﻿from setuptools import setup
 
 setup(
   name = "minipkg",
-  version = "1.0.0",
+  version = "1.0.1",
   description = "All the power of Python...in the palm of your hand.",
   long_description = "miniPkg is a package that implements a module named miniPy, programmed by Omer Drkić that adds loads of new features and makes Python easier to use. It adds some extension to the 'math' library and to the actual Python environment, as well as some useful data manipulation tools.",
   author = "Omer Drkić",
   author_email = "omerdrkic2501@gmail.com",
   py_modules = [
     "minipy"
   ],
```

