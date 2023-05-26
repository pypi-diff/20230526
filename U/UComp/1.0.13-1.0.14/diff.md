# Comparing `tmp/UComp-1.0.13.tar.gz` & `tmp/UComp-1.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UComp-1.0.13.tar", last modified: Thu May 25 15:15:07 2023, max compression
+gzip compressed data, was "UComp-1.0.14.tar", last modified: Fri May 26 14:31:05 2023, max compression
```

## Comparing `UComp-1.0.13.tar` & `UComp-1.0.14.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 15:15:07.481036 UComp-1.0.13/
--rw-rw-rw-   0        0        0       76 2023-05-25 14:30:54.000000 UComp-1.0.13/MANIFEST.in
--rw-rw-rw-   0        0        0      304 2023-05-25 15:15:07.481036 UComp-1.0.13/PKG-INFO
--rw-rw-rw-   0        0        0       37 2023-05-19 10:25:10.000000 UComp-1.0.13/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 15:15:07.434179 UComp-1.0.13/UComp/
--rw-rw-rw-   0        0        0   573952 2023-05-19 09:06:21.000000 UComp-1.0.13/UComp/ETSc.pyd
--rw-rw-rw-   0        0        0  1137664 2023-05-19 08:42:47.000000 UComp-1.0.13/UComp/UCc.pyd
--rw-rw-rw-   0        0        0    18991 2023-05-25 15:14:48.000000 UComp-1.0.13/UComp/UCmodule.py
--rw-rw-rw-   0        0        0        2 2023-05-25 15:01:39.000000 UComp-1.0.13/UComp/__init__.py
--rw-rw-rw-   0        0        0 32492623 2016-06-16 16:24:20.000000 UComp-1.0.13/UComp/libopenblas.dll
-drwxrwxrwx   0        0        0        0 2023-05-25 15:15:07.481036 UComp-1.0.13/UComp.egg-info/
--rw-rw-rw-   0        0        0      304 2023-05-25 15:15:07.000000 UComp-1.0.13/UComp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2023-05-25 15:15:07.000000 UComp-1.0.13/UComp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 15:15:07.000000 UComp-1.0.13/UComp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-05-25 15:15:07.000000 UComp-1.0.13/UComp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-25 15:15:07.000000 UComp-1.0.13/UComp.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 15:15:07.481036 UComp-1.0.13/setup.cfg
--rw-rw-rw-   0        0        0      602 2023-05-25 15:15:00.000000 UComp-1.0.13/setup.py
+drwxr-xr-x   0 diego.pedregal   (501) staff       (20)        0 2023-05-26 14:31:05.479875 UComp-1.0.14/
+-rw-------   0 diego.pedregal   (501) staff       (20)      157 2023-05-26 14:30:48.000000 UComp-1.0.14/MANIFEST.in
+-rw-r--r--   0 diego.pedregal   (501) staff       (20)      294 2023-05-26 14:31:05.479585 UComp-1.0.14/PKG-INFO
+-rw-------   0 diego.pedregal   (501) staff       (20)       37 2023-05-22 14:50:53.000000 UComp-1.0.14/README.md
+drwxr-xr-x   0 diego.pedregal   (501) staff       (20)        0 2023-05-26 14:31:05.423721 UComp-1.0.14/UComp/
+-rwxr-xr-x   0 diego.pedregal   (501) staff       (20)  1451960 2023-05-26 14:15:14.000000 UComp-1.0.14/UComp/ETSc.cpython-311-darwin.so
+-rw-------   0 diego.pedregal   (501) staff       (20)   573952 2023-05-19 09:06:21.000000 UComp-1.0.14/UComp/ETSc.pyd
+-rwxr-xr-x   0 diego.pedregal   (501) staff       (20)  1631200 2023-05-26 14:18:31.000000 UComp-1.0.14/UComp/UCc.cpython-311-darwin.so
+-rw-------   0 diego.pedregal   (501) staff       (20)  1137664 2023-05-19 08:42:47.000000 UComp-1.0.14/UComp/UCc.pyd
+-rw-------   0 diego.pedregal   (501) staff       (20)    18991 2023-05-25 15:14:48.000000 UComp-1.0.14/UComp/UCmodule.py
+-rw-------   0 diego.pedregal   (501) staff       (20)        2 2023-05-25 11:12:46.000000 UComp-1.0.14/UComp/__init__.py
+-rw-------   0 diego.pedregal   (501) staff       (20) 32492623 2016-06-16 16:24:20.000000 UComp-1.0.14/UComp/libopenblas.dll
+drwxr-xr-x   0 diego.pedregal   (501) staff       (20)        0 2023-05-26 14:31:05.479207 UComp-1.0.14/UComp.egg-info/
+-rw-r--r--   0 diego.pedregal   (501) staff       (20)      294 2023-05-26 14:31:05.000000 UComp-1.0.14/UComp.egg-info/PKG-INFO
+-rw-r--r--   0 diego.pedregal   (501) staff       (20)      326 2023-05-26 14:31:05.000000 UComp-1.0.14/UComp.egg-info/SOURCES.txt
+-rw-r--r--   0 diego.pedregal   (501) staff       (20)        1 2023-05-26 14:31:05.000000 UComp-1.0.14/UComp.egg-info/dependency_links.txt
+-rw-r--r--   0 diego.pedregal   (501) staff       (20)       31 2023-05-26 14:31:05.000000 UComp-1.0.14/UComp.egg-info/requires.txt
+-rw-r--r--   0 diego.pedregal   (501) staff       (20)        6 2023-05-26 14:31:05.000000 UComp-1.0.14/UComp.egg-info/top_level.txt
+-rw-r--r--   0 diego.pedregal   (501) staff       (20)       38 2023-05-26 14:31:05.479948 UComp-1.0.14/setup.cfg
+-rw-------   0 diego.pedregal   (501) staff       (20)      602 2023-05-26 14:26:25.000000 UComp-1.0.14/setup.py
```

### Comparing `UComp-1.0.13/UComp/UCmodule.py` & `UComp-1.0.14/UComp/UCmodule.py`

 * *Files identical despite different names*

### Comparing `UComp-1.0.13/UComp/libopenblas.dll` & `UComp-1.0.14/UComp/libopenblas.dll`

 * *Files identical despite different names*

### Comparing `UComp-1.0.13/setup.py` & `UComp-1.0.14/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='UComp',
-    version='1.0.13',
+    version='1.0.14',
     author='Diego J. Pedregal',
     author_email='diego.pedregal@uclm.es',
     description='Modelling and forecasting univariate time series',
     long_description='Modelling and forecasting univariate time series',
     url='https://github.com/djpedregal/UComp',
     packages=find_packages(),
     include_package_data=True,
```

