# Comparing `tmp/phap-2.1.2.tar.gz` & `tmp/phap-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phap-2.1.2.tar", last modified: Wed May 24 05:10:22 2023, max compression
+gzip compressed data, was "phap-2.2.0.tar", last modified: Fri May 26 05:18:43 2023, max compression
```

## Comparing `phap-2.1.2.tar` & `phap-2.2.0.tar`

### file list

```diff
@@ -1,23 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 05:10:22.360830 phap-2.1.2/
--rw-rw-rw-   0        0        0     1069 2023-04-23 14:27:33.000000 phap-2.1.2/LICENSE
--rw-rw-rw-   0        0        0     1710 2023-05-24 05:10:22.360830 phap-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      913 2023-05-24 05:09:53.000000 phap-2.1.2/README.md
--rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-2.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 05:10:22.368834 phap-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1639 2023-05-24 05:10:02.000000 phap-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:10:22.280833 phap-2.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-24 05:10:22.328843 phap-2.1.2/src/numalgo/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:04:59.000000 phap-2.1.2/src/numalgo/__init__.py
--rw-rw-rw-   0        0        0      450 2023-05-23 14:04:59.000000 phap-2.1.2/src/numalgo/deskcheck.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:10:22.344829 phap-2.1.2/src/phap.egg-info/
--rw-rw-rw-   0        0        0     1710 2023-05-24 05:10:22.000000 phap-2.1.2/src/phap.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      335 2023-05-24 05:10:22.000000 phap-2.1.2/src/phap.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 05:10:22.000000 phap-2.1.2/src/phap.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-24 05:10:22.000000 phap-2.1.2/src/phap.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-24 05:10:22.352850 phap-2.1.2/src/stralgo/
--rw-rw-rw-   0        0        0        0 2022-03-11 23:01:04.000000 phap-2.1.2/src/stralgo/__init__.py
--rw-rw-rw-   0        0        0      972 2023-02-20 00:51:10.000000 phap-2.1.2/src/stralgo/base.py
-drwxrwxrwx   0        0        0        0 2023-05-24 05:10:22.360830 phap-2.1.2/src/stralgo/hash/
--rw-rw-rw-   0        0        0      212 2023-05-23 14:04:59.000000 phap-2.1.2/src/stralgo/hash/__init__.py
--rw-rw-rw-   0        0        0      460 2023-02-20 00:51:14.000000 phap-2.1.2/src/stralgo/hash/sha.py
--rw-rw-rw-   0        0        0      175 2023-05-23 14:04:59.000000 phap-2.1.2/src/stralgo/json.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:43.595527 phap-2.2.0/
+-rw-rw-rw-   0        0        0     1069 2023-05-25 04:31:47.000000 phap-2.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1710 2023-05-26 05:18:43.594530 phap-2.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      913 2023-05-26 05:17:32.000000 phap-2.2.0/README.md
+-rw-rw-rw-   0        0        0       86 2022-03-12 07:02:40.000000 phap-2.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 05:18:43.595527 phap-2.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1639 2023-05-26 05:17:43.000000 phap-2.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:43.523921 phap-2.2.0/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:43.572921 phap-2.2.0/src/numalgo/
+-rw-rw-rw-   0        0        0        0 2023-05-25 04:35:10.000000 phap-2.2.0/src/numalgo/__init__.py
+-rw-rw-rw-   0        0        0      452 2023-05-25 05:00:13.000000 phap-2.2.0/src/numalgo/deskcheck.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:43.581511 phap-2.2.0/src/phap.egg-info/
+-rw-rw-rw-   0        0        0     1710 2023-05-26 05:18:43.000000 phap-2.2.0/src/phap.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      398 2023-05-26 05:18:43.000000 phap-2.2.0/src/phap.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 05:18:43.000000 phap-2.2.0/src/phap.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-05-26 05:18:43.000000 phap-2.2.0/src/phap.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:43.585518 phap-2.2.0/src/stralgo/
+-rw-rw-rw-   0        0        0        0 2022-03-11 23:01:04.000000 phap-2.2.0/src/stralgo/__init__.py
+-rw-rw-rw-   0        0        0      972 2023-02-20 00:51:10.000000 phap-2.2.0/src/stralgo/base.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:43.589529 phap-2.2.0/src/stralgo/hash/
+-rw-rw-rw-   0        0        0      212 2023-05-25 04:35:10.000000 phap-2.2.0/src/stralgo/hash/__init__.py
+-rw-rw-rw-   0        0        0      460 2023-02-20 00:51:14.000000 phap-2.2.0/src/stralgo/hash/sha.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:18:43.593529 phap-2.2.0/src/stralgo/hash/sm/
+-rw-rw-rw-   0        0        0       26 2023-05-26 05:17:05.000000 phap-2.2.0/src/stralgo/hash/sm/__init__.py
+-rw-rw-rw-   0        0        0     6937 2023-05-26 05:16:45.000000 phap-2.2.0/src/stralgo/hash/sm/sm3libs.py
+-rw-rw-rw-   0        0        0      175 2023-05-25 04:35:10.000000 phap-2.2.0/src/stralgo/json.py
```

### Comparing `phap-2.1.2/LICENSE` & `phap-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `phap-2.1.2/PKG-INFO` & `phap-2.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 2.1.2
+Version: 2.2.0
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,15 +31,15 @@
 # Versions
 ## Stable
 + v0.1.0 (stralgo)
 + v1.1.1 (stralgo)
 + v2.1.2
 
 ## Latest Version
-+ v2.1.2
++ v2.2.0
 
 # Build
 ## Precondition
 + Install git and make tools
 + Install Python(the version 3.9 or the version 3.11)
 + Clone source code from source repository
 #### ```git clone git@github.com:DashBing/phap.git```
```

### Comparing `phap-2.1.2/README.md` & `phap-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Versions
 ## Stable
 + v0.1.0 (stralgo)
 + v1.1.1 (stralgo)
 + v2.1.2
 
 ## Latest Version
-+ v2.1.2
++ v2.2.0
 
 # Build
 ## Precondition
 + Install git and make tools
 + Install Python(the version 3.9 or the version 3.11)
 + Clone source code from source repository
 #### ```git clone git@github.com:DashBing/phap.git```
```

### Comparing `phap-2.1.2/setup.py` & `phap-2.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="phap",
-    version="2.1.2",  #版本
+    version="2.2.0",  #版本
     author="DashBing",
     author_email="mcbbkf@outlook.com",
     description="Programing Helpful Algorithm Package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     #scripts=[],
     url="https://github.com/DashBing/phap/",
```

### Comparing `phap-2.1.2/src/phap.egg-info/PKG-INFO` & `phap-2.2.0/src/phap.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: phap
-Version: 2.1.2
+Version: 2.2.0
 Summary: Programing Helpful Algorithm Package
 Home-page: https://github.com/DashBing/phap/
 Author: DashBing
 Author-email: mcbbkf@outlook.com
 Project-URL: Github, https://github.com/DashBing/phap/
 Project-URL: Old Project Version(stralgo), https://pypi.org/project/stralgo/
 Classifier: Development Status :: 5 - Production/Stable
@@ -31,15 +31,15 @@
 # Versions
 ## Stable
 + v0.1.0 (stralgo)
 + v1.1.1 (stralgo)
 + v2.1.2
 
 ## Latest Version
-+ v2.1.2
++ v2.2.0
 
 # Build
 ## Precondition
 + Install git and make tools
 + Install Python(the version 3.9 or the version 3.11)
 + Clone source code from source repository
 #### ```git clone git@github.com:DashBing/phap.git```
```

### Comparing `phap-2.1.2/src/stralgo/base.py` & `phap-2.2.0/src/stralgo/base.py`

 * *Files identical despite different names*

