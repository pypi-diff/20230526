# Comparing `tmp/exergenics-etl-1.0.4.tar.gz` & `tmp/exergenics-etl-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.0.4.tar", last modified: Fri May 26 04:06:14 2023, max compression
+gzip compressed data, was "exergenics-etl-1.0.5.tar", last modified: Fri May 26 06:43:02 2023, max compression
```

## Comparing `exergenics-etl-1.0.4.tar` & `exergenics-etl-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.887457 exergenics-etl-1.0.4/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48613 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    35894 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 04:06:09.000000 exergenics-etl-1.0.4/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 04:06:14.000000 exergenics-etl-1.0.4/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 04:06:14.891457 exergenics-etl-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-26 04:06:13.000000 exergenics-etl-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48486 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35894 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 06:42:57.000000 exergenics-etl-1.0.5/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 06:43:02.000000 exergenics-etl-1.0.5/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:43:02.421196 exergenics-etl-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-26 06:43:00.000000 exergenics-etl-1.0.5/setup.py
```

### Comparing `exergenics-etl-1.0.4/LICENSE` & `exergenics-etl-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.4/app/exergenics_etl/__init__.py` & `exergenics-etl-1.0.5/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.4/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.0.5/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 0% similar despite different names*

```diff
@@ -476,17 +476,14 @@
         # Set header as column names
         df.columns = df.loc[headerRowId].values
 
         # Remove headers from values
         df.drop(labels=headerRowId, inplace=True)
         df.reset_index(inplace=True, drop=True)  # Replace and reset index
 
-        # Convert columns to best possible dtypes
-        df = df.convert_dtypes(convert_string=False, convert_boolean=False)
-
         return df
 
 
 def convertable_to_float(string: str) -> bool:
     """Checks if a given string can be converted to a float.
 
     Args:
```

### Comparing `exergenics-etl-1.0.4/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.0.5/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.4/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.0.5/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.4/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.0.5/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.4/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.0.5/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.0.4/setup.py` & `exergenics-etl-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.0.4",
+    version="v1.0.5",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

