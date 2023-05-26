# Comparing `tmp/cubic-spline-0.1.0.tar.gz` & `tmp/cubic-spline-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cubic-spline-0.1.0.tar", last modified: Fri May 26 18:17:38 2023, max compression
+gzip compressed data, was "cubic-spline-0.1.1.tar", last modified: Fri May 26 18:36:52 2023, max compression
```

## Comparing `cubic-spline-0.1.0.tar` & `cubic-spline-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 18:17:38.239974 cubic-spline-0.1.0/
--rw-rw-rw-   0        0        0     1085 2023-05-19 12:22:20.000000 cubic-spline-0.1.0/LICENSE
--rw-rw-rw-   0        0        0     2622 2023-05-26 18:17:38.239974 cubic-spline-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     2115 2023-05-19 12:23:30.000000 cubic-spline-0.1.0/README.md
--rw-rw-rw-   0        0        0      600 2023-05-26 18:15:15.000000 cubic-spline-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 18:17:38.239974 cubic-spline-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 18:17:38.168425 cubic-spline-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 18:17:38.208727 cubic-spline-0.1.0/src/cubic_spline/
--rw-rw-rw-   0        0        0      122 2023-05-22 20:37:47.000000 cubic-spline-0.1.0/src/cubic_spline/__init__.py
--rw-rw-rw-   0        0        0     6087 2023-05-26 16:10:14.000000 cubic-spline-0.1.0/src/cubic_spline/cubic_spline.py
--rw-rw-rw-   0        0        0     3435 2023-05-19 12:23:31.000000 cubic-spline-0.1.0/src/cubic_spline/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:17:38.224353 cubic-spline-0.1.0/src/cubic_spline.egg-info/
--rw-rw-rw-   0        0        0     2622 2023-05-26 18:17:38.000000 cubic-spline-0.1.0/src/cubic_spline.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      280 2023-05-26 18:17:38.000000 cubic-spline-0.1.0/src/cubic_spline.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 18:17:38.000000 cubic-spline-0.1.0/src/cubic_spline.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-26 18:17:38.000000 cubic-spline-0.1.0/src/cubic_spline.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 18:36:52.038401 cubic-spline-0.1.1/
+-rw-rw-rw-   0        0        0     1085 2023-05-19 12:22:20.000000 cubic-spline-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0     2622 2023-05-26 18:36:52.022774 cubic-spline-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2115 2023-05-26 18:29:55.000000 cubic-spline-0.1.1/README.md
+-rw-rw-rw-   0        0        0      600 2023-05-26 18:33:09.000000 cubic-spline-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 18:36:52.038401 cubic-spline-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 18:36:51.967374 cubic-spline-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 18:36:51.998612 cubic-spline-0.1.1/src/cubic_spline/
+-rw-rw-rw-   0        0        0      122 2023-05-22 20:37:47.000000 cubic-spline-0.1.1/src/cubic_spline/__init__.py
+-rw-rw-rw-   0        0        0     6087 2023-05-26 16:10:14.000000 cubic-spline-0.1.1/src/cubic_spline/cubic_spline.py
+-rw-rw-rw-   0        0        0     3435 2023-05-19 12:23:31.000000 cubic-spline-0.1.1/src/cubic_spline/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:36:52.022774 cubic-spline-0.1.1/src/cubic_spline.egg-info/
+-rw-rw-rw-   0        0        0     2622 2023-05-26 18:36:51.000000 cubic-spline-0.1.1/src/cubic_spline.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      280 2023-05-26 18:36:51.000000 cubic-spline-0.1.1/src/cubic_spline.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 18:36:51.000000 cubic-spline-0.1.1/src/cubic_spline.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-26 18:36:51.000000 cubic-spline-0.1.1/src/cubic_spline.egg-info/top_level.txt
```

### Comparing `cubic-spline-0.1.0/LICENSE` & `cubic-spline-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cubic-spline-0.1.0/PKG-INFO` & `cubic-spline-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubic-spline
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cubic spline interpolation with Numba compatibility
 Author-email: Harrison Snell <harrison.snell23@gmail.com>
 Project-URL: Homepage, https://github.com/hwsnell/Cubic-Spline
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -24,14 +24,14 @@
 ```
 
 ## Installation
 
 `cubic_spline` runs on NumPy and Numba. The pacakge was developed with Python 3.9 with NumPy version 1.21 and Numba version 0.55. To install run the following command
 
 ```
-pip install cubic_spline
+pip install cubic-spline
 ```
 
 
 ## Using the Pacakge
 
 `cubic_spline.py` and `tools.py` are the necessary files for carrying out cubic interpolation. Users will normally only need to interact with `cubic_spline` as it contains the high level wrapper functions. The other files, `vfi_demo` and `firm_engine`, provide an application of this cubic interpolation package to a heterogeneous firm optimization problem. `firm_engine` requires the SSJ pacakge to be installed. `vfi_demo` is a notebook that walks through the canonical lumpy investment problem with value function iteration making use of the `cubic_spline` methods.
```

### Comparing `cubic-spline-0.1.0/README.md` & `cubic-spline-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,14 @@
 ```
 
 ## Installation
 
 `cubic_spline` runs on NumPy and Numba. The pacakge was developed with Python 3.9 with NumPy version 1.21 and Numba version 0.55. To install run the following command
 
 ```
-pip install cubic_spline
+pip install cubic-spline
 ```
 
 
 ## Using the Pacakge
 
 `cubic_spline.py` and `tools.py` are the necessary files for carrying out cubic interpolation. Users will normally only need to interact with `cubic_spline` as it contains the high level wrapper functions. The other files, `vfi_demo` and `firm_engine`, provide an application of this cubic interpolation package to a heterogeneous firm optimization problem. `firm_engine` requires the SSJ pacakge to be installed. `vfi_demo` is a notebook that walks through the canonical lumpy investment problem with value function iteration making use of the `cubic_spline` methods.
```

### Comparing `cubic-spline-0.1.0/pyproject.toml` & `cubic-spline-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     "numba>=0.55.1"
 ]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "cubic-spline"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Harrison Snell", email="harrison.snell23@gmail.com" },
 ]
 description = "Cubic spline interpolation with Numba compatibility"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `cubic-spline-0.1.0/src/cubic_spline/cubic_spline.py` & `cubic-spline-0.1.1/src/cubic_spline/cubic_spline.py`

 * *Files identical despite different names*

### Comparing `cubic-spline-0.1.0/src/cubic_spline/tools.py` & `cubic-spline-0.1.1/src/cubic_spline/tools.py`

 * *Files identical despite different names*

### Comparing `cubic-spline-0.1.0/src/cubic_spline.egg-info/PKG-INFO` & `cubic-spline-0.1.1/src/cubic_spline.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cubic-spline
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cubic spline interpolation with Numba compatibility
 Author-email: Harrison Snell <harrison.snell23@gmail.com>
 Project-URL: Homepage, https://github.com/hwsnell/Cubic-Spline
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -24,14 +24,14 @@
 ```
 
 ## Installation
 
 `cubic_spline` runs on NumPy and Numba. The pacakge was developed with Python 3.9 with NumPy version 1.21 and Numba version 0.55. To install run the following command
 
 ```
-pip install cubic_spline
+pip install cubic-spline
 ```
 
 
 ## Using the Pacakge
 
 `cubic_spline.py` and `tools.py` are the necessary files for carrying out cubic interpolation. Users will normally only need to interact with `cubic_spline` as it contains the high level wrapper functions. The other files, `vfi_demo` and `firm_engine`, provide an application of this cubic interpolation package to a heterogeneous firm optimization problem. `firm_engine` requires the SSJ pacakge to be installed. `vfi_demo` is a notebook that walks through the canonical lumpy investment problem with value function iteration making use of the `cubic_spline` methods.
```

