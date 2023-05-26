# Comparing `tmp/miresta-0.7.tar.gz` & `tmp/miresta-0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miresta-0.7.tar", last modified: Fri May 26 01:13:27 2023, max compression
+gzip compressed data, was "miresta-0.8.tar", last modified: Fri May 26 01:17:42 2023, max compression
```

## Comparing `miresta-0.7.tar` & `miresta-0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 01:13:27.123399 miresta-0.7/
--rw-r--r--   0 cristian  (1000) cristian  (1000)     1134 2023-05-16 14:58:24.000000 miresta-0.7/LICENSE
--rw-rw-r--   0 cristian  (1000) cristian  (1000)     1959 2023-05-26 01:13:27.123399 miresta-0.7/PKG-INFO
--rw-r--r--   0 cristian  (1000) cristian  (1000)     1146 2023-05-26 01:12:45.000000 miresta-0.7/README.md
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 01:13:27.123399 miresta-0.7/miresta/
--rw-r--r--   0 cristian  (1000) cristian  (1000)       52 2023-05-18 19:34:05.000000 miresta-0.7/miresta/__init__.py
-drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 01:13:27.123399 miresta-0.7/miresta.egg-info/
--rw-rw-r--   0 cristian  (1000) cristian  (1000)     1959 2023-05-26 01:13:27.000000 miresta-0.7/miresta.egg-info/PKG-INFO
--rw-rw-r--   0 cristian  (1000) cristian  (1000)      251 2023-05-26 01:13:27.000000 miresta-0.7/miresta.egg-info/SOURCES.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)        1 2023-05-26 01:13:27.000000 miresta-0.7/miresta.egg-info/dependency_links.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       51 2023-05-26 01:13:27.000000 miresta-0.7/miresta.egg-info/entry_points.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)        6 2023-05-26 01:13:27.000000 miresta-0.7/miresta.egg-info/requires.txt
--rw-rw-r--   0 cristian  (1000) cristian  (1000)        8 2023-05-26 01:13:27.000000 miresta-0.7/miresta.egg-info/top_level.txt
--rw-r--r--   0 cristian  (1000) cristian  (1000)       89 2023-05-18 18:16:23.000000 miresta-0.7/pyproject.toml
--rw-rw-r--   0 cristian  (1000) cristian  (1000)       38 2023-05-26 01:13:27.123399 miresta-0.7/setup.cfg
--rw-r--r--   0 cristian  (1000) cristian  (1000)     2189 2023-05-26 01:13:21.000000 miresta-0.7/setup.py
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 01:17:42.438254 miresta-0.8/
+-rw-r--r--   0 cristian  (1000) cristian  (1000)     1134 2023-05-16 14:58:24.000000 miresta-0.8/LICENSE
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)     1847 2023-05-26 01:17:42.438254 miresta-0.8/PKG-INFO
+-rw-r--r--   0 cristian  (1000) cristian  (1000)     1034 2023-05-26 01:17:30.000000 miresta-0.8/README.md
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 01:17:42.434255 miresta-0.8/miresta/
+-rw-r--r--   0 cristian  (1000) cristian  (1000)       52 2023-05-18 19:34:05.000000 miresta-0.8/miresta/__init__.py
+drwxrwxr-x   0 cristian  (1000) cristian  (1000)        0 2023-05-26 01:17:42.434255 miresta-0.8/miresta.egg-info/
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)     1847 2023-05-26 01:17:42.000000 miresta-0.8/miresta.egg-info/PKG-INFO
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)      251 2023-05-26 01:17:42.000000 miresta-0.8/miresta.egg-info/SOURCES.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)        1 2023-05-26 01:17:42.000000 miresta-0.8/miresta.egg-info/dependency_links.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       51 2023-05-26 01:17:42.000000 miresta-0.8/miresta.egg-info/entry_points.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)        6 2023-05-26 01:17:42.000000 miresta-0.8/miresta.egg-info/requires.txt
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)        8 2023-05-26 01:17:42.000000 miresta-0.8/miresta.egg-info/top_level.txt
+-rw-r--r--   0 cristian  (1000) cristian  (1000)       89 2023-05-18 18:16:23.000000 miresta-0.8/pyproject.toml
+-rw-rw-r--   0 cristian  (1000) cristian  (1000)       38 2023-05-26 01:17:42.438254 miresta-0.8/setup.cfg
+-rw-r--r--   0 cristian  (1000) cristian  (1000)     2189 2023-05-26 01:17:37.000000 miresta-0.8/setup.py
```

### Comparing `miresta-0.7/LICENSE` & `miresta-0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `miresta-0.7/PKG-INFO` & `miresta-0.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: miresta
-Version: 0.7
+Version: 0.8
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
         
-        <p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.smartick.es%2Fblog%2Fmatematicas%2Fsumas-y-restas%2Fla-resta%2F&psig=AOvVaw2XsJ-5Ec05Pur0tQ3zOvoL&ust=1685149930379000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCLjohermkf8CFQAAAAAdAAAAABAE" alt="a subtracting cat""/></p>
+        <p align="center"><img src="https://static.vecteezy.com/system/resources/previews/010/690/326/non_2x/counting-game-with-cute-cats-math-worksheet-vector.jpg" alt="a subtracting cat""/></p>
         
         ## Download and install
         
         
         If you are using `PyPI` installation it's as simple as:
         
         ```
```

### Comparing `miresta-0.7/README.md` & `miresta-0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 <!-- This are visual tags that you may add to your package at the beginning with useful information on your package --> 
 [![version](https://img.shields.io/pypi/v/pymiau?color=blue)](https://pypi.org/project/miresta/)
 [![downloads](https://img.shields.io/pypi/dw/pymiau)](https://pypi.org/project/miresta/)
 
 This package performs a subtraction between two numbers.
 
-<p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.smartick.es%2Fblog%2Fmatematicas%2Fsumas-y-restas%2Fla-resta%2F&psig=AOvVaw2XsJ-5Ec05Pur0tQ3zOvoL&ust=1685149930379000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCLjohermkf8CFQAAAAAdAAAAABAE" alt="a subtracting cat""/></p>
+<p align="center"><img src="https://static.vecteezy.com/system/resources/previews/010/690/326/non_2x/counting-game-with-cute-cats-math-worksheet-vector.jpg" alt="a subtracting cat""/></p>
 
 ## Download and install
 
 
 If you are using `PyPI` installation it's as simple as:
 
 ```
```

### Comparing `miresta-0.7/miresta.egg-info/PKG-INFO` & `miresta-0.8/miresta.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: miresta
-Version: 0.7
+Version: 0.8
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
         
-        <p align="center"><img src="https://www.google.com/url?sa=i&url=https%3A%2F%2Fwww.smartick.es%2Fblog%2Fmatematicas%2Fsumas-y-restas%2Fla-resta%2F&psig=AOvVaw2XsJ-5Ec05Pur0tQ3zOvoL&ust=1685149930379000&source=images&cd=vfe&ved=0CBEQjRxqFwoTCLjohermkf8CFQAAAAAdAAAAABAE" alt="a subtracting cat""/></p>
+        <p align="center"><img src="https://static.vecteezy.com/system/resources/previews/010/690/326/non_2x/counting-game-with-cute-cats-math-worksheet-vector.jpg" alt="a subtracting cat""/></p>
         
         ## Download and install
         
         
         If you are using `PyPI` installation it's as simple as:
         
         ```
```

### Comparing `miresta-0.7/setup.py` & `miresta-0.8/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     # CLASSIFIER
     # ######################################################################
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         ],
-    version='0.7',
+    version='0.8',
 
     # ######################################################################
     # FILES
     # ######################################################################
     package_dir={'': '.'},
     packages=setuptools.find_packages(where='.'),
```

