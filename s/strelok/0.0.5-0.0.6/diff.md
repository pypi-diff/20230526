# Comparing `tmp/strelok-0.0.5.tar.gz` & `tmp/strelok-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strelok-0.0.5.tar", last modified: Fri May 26 02:25:39 2023, max compression
+gzip compressed data, was "strelok-0.0.6.tar", last modified: Fri May 26 03:33:29 2023, max compression
```

## Comparing `strelok-0.0.5.tar` & `strelok-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:25:39.307133 strelok-0.0.5/
--rw-r--r--   0 juliusriel   (501) staff       (20)    15310 2023-05-26 02:25:39.306957 strelok-0.0.5/PKG-INFO
--rw-r--r--   0 juliusriel   (501) staff       (20)    14635 2023-05-26 02:23:48.000000 strelok-0.0.5/README.rst
--rw-r--r--   0 juliusriel   (501) staff       (20)       38 2023-05-26 02:25:39.307172 strelok-0.0.5/setup.cfg
--rw-r--r--   0 juliusriel   (501) staff       (20)      964 2023-05-26 02:24:43.000000 strelok-0.0.5/setup.py
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:25:39.306210 strelok-0.0.5/strelok/
--rw-r--r--   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:13:50.000000 strelok-0.0.5/strelok/__init__.py
--rw-r--r--   0 juliusriel   (501) staff       (20)    13597 2023-05-26 02:16:29.000000 strelok-0.0.5/strelok/feat.py
-drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 02:25:39.306779 strelok-0.0.5/strelok.egg-info/
--rw-r--r--   0 juliusriel   (501) staff       (20)    15310 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/PKG-INFO
--rw-r--r--   0 juliusriel   (501) staff       (20)      209 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/SOURCES.txt
--rw-r--r--   0 juliusriel   (501) staff       (20)        1 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/dependency_links.txt
--rw-r--r--   0 juliusriel   (501) staff       (20)       37 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/requires.txt
--rw-r--r--   0 juliusriel   (501) staff       (20)        8 2023-05-26 02:25:39.000000 strelok-0.0.5/strelok.egg-info/top_level.txt
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 03:33:29.542636 strelok-0.0.6/
+-rw-r--r--   0 juliusriel   (501) staff       (20)    15310 2023-05-26 03:33:29.542094 strelok-0.0.6/PKG-INFO
+-rw-r--r--   0 juliusriel   (501) staff       (20)    14635 2023-05-26 02:23:48.000000 strelok-0.0.6/README.rst
+-rw-r--r--   0 juliusriel   (501) staff       (20)       38 2023-05-26 03:33:29.542683 strelok-0.0.6/setup.cfg
+-rw-r--r--   0 juliusriel   (501) staff       (20)      951 2023-05-26 03:33:11.000000 strelok-0.0.6/setup.py
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 03:33:29.541333 strelok-0.0.6/strelok/
+-rw-r--r--   0 juliusriel   (501) staff       (20)        0 2023-05-24 08:13:50.000000 strelok-0.0.6/strelok/__init__.py
+-rw-r--r--   0 juliusriel   (501) staff       (20)    13597 2023-05-26 02:16:29.000000 strelok-0.0.6/strelok/feat.py
+drwxr-xr-x   0 juliusriel   (501) staff       (20)        0 2023-05-26 03:33:29.541904 strelok-0.0.6/strelok.egg-info/
+-rw-r--r--   0 juliusriel   (501) staff       (20)    15310 2023-05-26 03:33:29.000000 strelok-0.0.6/strelok.egg-info/PKG-INFO
+-rw-r--r--   0 juliusriel   (501) staff       (20)      209 2023-05-26 03:33:29.000000 strelok-0.0.6/strelok.egg-info/SOURCES.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)        1 2023-05-26 03:33:29.000000 strelok-0.0.6/strelok.egg-info/dependency_links.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)       27 2023-05-26 03:33:29.000000 strelok-0.0.6/strelok.egg-info/requires.txt
+-rw-r--r--   0 juliusriel   (501) staff       (20)        8 2023-05-26 03:33:29.000000 strelok-0.0.6/strelok.egg-info/top_level.txt
```

### Comparing `strelok-0.0.5/PKG-INFO` & `strelok-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strelok
-Version: 0.0.5
+Version: 0.0.6
 Summary: Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models
 Author: Julius Riel
 Author-email: julius.riel@icloud.com
 License: UNKNOWN
 Keywords: strelok,feature,selection,machine learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `strelok-0.0.5/README.rst` & `strelok-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `strelok-0.0.5/setup.py` & `strelok-0.0.6/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r') as f:
     long_description = f.read()
 
 setup(
     name="strelok",
-    version="0.0.5",
+    version="0.0.6",
     author="Julius Riel",
     author_email="julius.riel@icloud.com",
     description="Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models",
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    install_requires=['numpy', 'pandas', 'sklearn', 'scipy', 'itertools'],
+    install_requires=['numpy', 'pandas', 'sklearn', 'scipy'],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     keywords="strelok, feature, selection, machine learning",
```

### Comparing `strelok-0.0.5/strelok/feat.py` & `strelok-0.0.6/strelok/feat.py`

 * *Files identical despite different names*

### Comparing `strelok-0.0.5/strelok.egg-info/PKG-INFO` & `strelok-0.0.6/strelok.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strelok
-Version: 0.0.5
+Version: 0.0.6
 Summary: Strelok is a simple Python package that provides FEAT, a feature engineering automation toolkit. With a focus on simplicity, it offers user definable pipelines to streamline the feature engineering process and improve the performance of machine learning models
 Author: Julius Riel
 Author-email: julius.riel@icloud.com
 License: UNKNOWN
 Keywords: strelok,feature,selection,machine learning
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

