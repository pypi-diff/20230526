# Comparing `tmp/miresta-0.3.tar.gz` & `tmp/miresta-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miresta-0.3.tar", last modified: Fri May 26 00:55:59 2023, max compression
+gzip compressed data, was "miresta-0.5.tar", last modified: Fri May 26 00:59:37 2023, max compression
```

## Comparing `miresta-0.3.tar` & `miresta-0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 00:55:59.260155 miresta-0.3/
--rw-r--r--   0 cristian  (1000) cristian  (1000)     1134 2023-05-16 14:58:24.000000 miresta-0.3/LICENSE
--rw-rw-r--   0 cristian  (1000) cristian  (1000)     1743 2023-05-26 00:55:59.256155 miresta-0.3/PKG-INFO
--rw-r--r--   0 cristian  (1000) cristian  (1000)     1002 2023-05-26 00:55:31.000000 miresta-0.3/README.md
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 00:55:59.256155 miresta-0.3/miresta/
--rw-r--r--   0 cristian  (1000) cristian  (1000)       52 2023-05-18 19:34:05.000000 miresta-0.3/miresta/__init__.py
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 00:55:59.256155 miresta-0.3/miresta.egg-info/
--rw-rw-r--   0 cristian  (1000) cristian  (1000)     1743 2023-05-26 00:55:59.000000 miresta-0.3/miresta.egg-info/PKG-INFO
--rw-rw-r--   0 cristian  (1000) cristian  (1000)      251 2023-05-26 00:55:59.000000 miresta-0.3/miresta.egg-info/SOURCES.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)        1 2023-05-26 00:55:59.000000 miresta-0.3/miresta.egg-info/dependency_links.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       51 2023-05-26 00:55:59.000000 miresta-0.3/miresta.egg-info/entry_points.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)        6 2023-05-26 00:55:59.000000 miresta-0.3/miresta.egg-info/requires.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)        8 2023-05-26 00:55:59.000000 miresta-0.3/miresta.egg-info/top_level.txt
--rw-r--r--   0 cristian  (1000) cristian  (1000)       89 2023-05-18 18:16:23.000000 miresta-0.3/pyproject.toml
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       38 2023-05-26 00:55:59.260155 miresta-0.3/setup.cfg
--rw-r--r--   0 cristian  (1000) cristian  (1000)     2189 2023-05-26 00:55:49.000000 miresta-0.3/setup.py
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 00:59:37.610451 miresta-0.5/
+-rw-r--r--   0 cristian  (1000) cristian  (1000)     1134 2023-05-16 14:58:24.000000 miresta-0.5/LICENSE
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)     1756 2023-05-26 00:59:37.610451 miresta-0.5/PKG-INFO
+-rw-r--r--   0 cristian  (1000) cristian  (1000)     1015 2023-05-26 00:57:38.000000 miresta-0.5/README.md
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 00:59:37.606450 miresta-0.5/miresta/
+-rw-r--r--   0 cristian  (1000) cristian  (1000)       52 2023-05-18 19:34:05.000000 miresta-0.5/miresta/__init__.py
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 00:59:37.610451 miresta-0.5/miresta.egg-info/
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)     1756 2023-05-26 00:59:37.000000 miresta-0.5/miresta.egg-info/PKG-INFO
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)      251 2023-05-26 00:59:37.000000 miresta-0.5/miresta.egg-info/SOURCES.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)        1 2023-05-26 00:59:37.000000 miresta-0.5/miresta.egg-info/dependency_links.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       51 2023-05-26 00:59:37.000000 miresta-0.5/miresta.egg-info/entry_points.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)        6 2023-05-26 00:59:37.000000 miresta-0.5/miresta.egg-info/requires.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)        8 2023-05-26 00:59:37.000000 miresta-0.5/miresta.egg-info/top_level.txt
+-rw-r--r--   0 cristian  (1000) cristian  (1000)       89 2023-05-18 18:16:23.000000 miresta-0.5/pyproject.toml
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       38 2023-05-26 00:59:37.610451 miresta-0.5/setup.cfg
+-rw-r--r--   0 cristian  (1000) cristian  (1000)     2189 2023-05-26 00:59:31.000000 miresta-0.5/setup.py
```

### Comparing `miresta-0.3/LICENSE` & `miresta-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `miresta-0.3/PKG-INFO` & `miresta-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: miresta
-Version: 0.3
+Version: 0.5
 Summary: This package performs a subtraction
 Home-page: https://pypi.org/project/miresta
 Author: Diana Carolina Zapata Zuluaga
 Author-email: dianac.zapata@udea.edu.co
 License: MIT
 Description: # miresta
         
         <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
         [![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/miresta/)
         [![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/miresta/)
         
         This package performs a subtraction between two numbers.
         
-        <p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.cokitos.com%2Fsumas-y-restas-con-el-gato-tom%2F&psig=AOvVaw04zWHvV8ITAnHDRUqTvzye&ust=1685148891291000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCICpsPrikf8CFQAAAAAdAAAAABAE" alt="Logo""/></p>
+        <p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.cokitos.com%2Fsumas-y-restas-con-el-gato-tom%2F&psig=AOvVaw04zWHvV8ITAnHDRUqTvzye&ust=1685148891291000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCICpsPrikf8CFQAAAAAdAAAAABAE" alt="a subtracting cat""/></p>
         
         ## Download and install
         
         
         If you are using `PyPI` installation it's as simple as:
         
         ```
```

### Comparing `miresta-0.3/README.md` & `miresta-0.5/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
 [![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/miresta/)
 [![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/miresta/)
 
 This package performs a subtraction between two numbers.
 
-<p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.cokitos.com%2Fsumas-y-restas-con-el-gato-tom%2F&psig=AOvVaw04zWHvV8ITAnHDRUqTvzye&ust=1685148891291000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCICpsPrikf8CFQAAAAAdAAAAABAE" alt="Logo""/></p>
+<p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.cokitos.com%2Fsumas-y-restas-con-el-gato-tom%2F&psig=AOvVaw04zWHvV8ITAnHDRUqTvzye&ust=1685148891291000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCICpsPrikf8CFQAAAAAdAAAAABAE" alt="a subtracting cat""/></p>
 
 ## Download and install
 
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
```

### Comparing `miresta-0.3/miresta.egg-info/PKG-INFO` & `miresta-0.5/miresta.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: miresta
-Version: 0.3
+Version: 0.5
 Summary: This package performs a subtraction
 Home-page: https://pypi.org/project/miresta
 Author: Diana Carolina Zapata Zuluaga
 Author-email: dianac.zapata@udea.edu.co
 License: MIT
 Description: # miresta
         
         <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
         [![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/miresta/)
         [![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/miresta/)
         
         This package performs a subtraction between two numbers.
         
-        <p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.cokitos.com%2Fsumas-y-restas-con-el-gato-tom%2F&psig=AOvVaw04zWHvV8ITAnHDRUqTvzye&ust=1685148891291000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCICpsPrikf8CFQAAAAAdAAAAABAE" alt="Logo""/></p>
+        <p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.cokitos.com%2Fsumas-y-restas-con-el-gato-tom%2F&psig=AOvVaw04zWHvV8ITAnHDRUqTvzye&ust=1685148891291000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCICpsPrikf8CFQAAAAAdAAAAABAE" alt="a subtracting cat""/></p>
         
         ## Download and install
         
         
         If you are using `PyPI` installation it's as simple as:
         
         ```
```

### Comparing `miresta-0.3/setup.py` & `miresta-0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.3',
+    version='0.5',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

