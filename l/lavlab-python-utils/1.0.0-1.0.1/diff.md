# Comparing `tmp/lavlab-python-utils-1.0.0.tar.gz` & `tmp/lavlab-python-utils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavlab-python-utils-1.0.0.tar", last modified: Mon May 22 12:26:37 2023, max compression
+gzip compressed data, was "lavlab-python-utils-1.0.1.tar", last modified: Fri May 26 16:05:19 2023, max compression
```

## Comparing `lavlab-python-utils-1.0.0.tar` & `lavlab-python-utils-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:26:37.966412 lavlab-python-utils-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-22 12:26:37.966412 lavlab-python-utils-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 12:26:25.000000 lavlab-python-utils-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 12:26:25.000000 lavlab-python-utils-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 12:26:37.966412 lavlab-python-utils-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:26:37.962412 lavlab-python-utils-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:26:37.962412 lavlab-python-utils-1.0.0/src/lavlab/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-22 12:26:25.000000 lavlab-python-utils-1.0.0/src/lavlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-05-22 12:26:25.000000 lavlab-python-utils-1.0.0/src/lavlab/omero_asyncio.py
--rw-r--r--   0 runner    (1001) docker     (123)    19120 2023-05-22 12:26:25.000000 lavlab-python-utils-1.0.0/src/lavlab/omero_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-22 12:26:25.000000 lavlab-python-utils-1.0.0/src/lavlab/python_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 12:26:37.966412 lavlab-python-utils-1.0.0/src/lavlab_python_utils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-22 12:26:37.000000 lavlab-python-utils-1.0.0/src/lavlab_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 12:26:37.000000 lavlab-python-utils-1.0.0/src/lavlab_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 12:26:37.000000 lavlab-python-utils-1.0.0/src/lavlab_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-22 12:26:37.000000 lavlab-python-utils-1.0.0/src/lavlab_python_utils.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-22 12:26:37.000000 lavlab-python-utils-1.0.0/src/lavlab_python_utils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/src/lavlab/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/src/lavlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10652 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/src/lavlab/omero_asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19120 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/src/lavlab/omero_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-26 16:05:05.000000 lavlab-python-utils-1.0.1/src/lavlab/python_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:19.254839 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 16:05:19.000000 lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/top_level.txt
```

### Comparing `lavlab-python-utils-1.0.0/PKG-INFO` & `lavlab-python-utils-1.0.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lavlab-python-utils-1.0.0/pyproject.toml` & `lavlab-python-utils-1.0.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [project]
 name = "lavlab-python-utils"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Michael Barrett", email="mjbarrett@mcw.edu" },
 ]
 description = "LaViolette Lab utility package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   'omero-py >= 5.13.1',
   'omero-scripts >= 5.7.1',
-  'scikit-image >= 0.19.3',
-  'numpy >= 1.24.2'
+  'scikit-image >= 0.19.3'
 ]
 [project.urls]
 "Homepage" = "https://github.com/laviolette-lab/lavlab-python-utils"
 "Bug Tracker" = "https://github.com/laviolette-lab/lavlab-python-utils/issues"
```

### Comparing `lavlab-python-utils-1.0.0/src/lavlab/omero_asyncio.py` & `lavlab-python-utils-1.0.1/src/lavlab/omero_asyncio.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.0.0/src/lavlab/omero_util.py` & `lavlab-python-utils-1.0.1/src/lavlab/omero_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.0.0/src/lavlab/python_util.py` & `lavlab-python-utils-1.0.1/src/lavlab/python_util.py`

 * *Files identical despite different names*

### Comparing `lavlab-python-utils-1.0.0/src/lavlab_python_utils.egg-info/PKG-INFO` & `lavlab-python-utils-1.0.1/src/lavlab_python_utils.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavlab-python-utils
-Version: 1.0.0
+Version: 1.0.1
 Summary: LaViolette Lab utility package
 Author-email: Michael Barrett <mjbarrett@mcw.edu>
 Project-URL: Homepage, https://github.com/laviolette-lab/lavlab-python-utils
 Project-URL: Bug Tracker, https://github.com/laviolette-lab/lavlab-python-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

