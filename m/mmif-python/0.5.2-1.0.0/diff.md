# Comparing `tmp/mmif-python-0.5.2.tar.gz` & `tmp/mmif-python-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-0.5.2.tar", last modified: Fri May 19 09:07:42 2023, max compression
+gzip compressed data, was "mmif-python-1.0.0.tar", last modified: Fri May 26 01:14:33 2023, max compression
```

## Comparing `mmif-python-0.5.2.tar` & `mmif-python-1.0.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.171131 mmif-python-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-19 09:07:13.000000 mmif-python-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-19 09:07:13.000000 mmif-python-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-19 09:07:42.171131 mmif-python-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-19 09:07:13.000000 mmif-python-0.5.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 09:07:13.000000 mmif-python-0.5.2/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-19 09:07:13.000000 mmif-python-0.5.2/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-19 09:07:41.000000 mmif-python-0.5.2/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 09:07:42.167131 mmif-python-0.5.2/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-19 09:07:42.000000 mmif-python-0.5.2/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-19 09:07:13.000000 mmif-python-0.5.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 09:07:42.171131 mmif-python-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-05-19 09:07:13.000000 mmif-python-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.534109 mmif-python-1.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-26 01:13:53.000000 mmif-python-1.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 01:13:53.000000 mmif-python-1.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 01:14:33.534109 mmif-python-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 01:13:53.000000 mmif-python-1.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 01:13:53.000000 mmif-python-1.0.0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.530109 mmif-python-1.0.0/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.530109 mmif-python-1.0.0/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:32.000000 mmif-python-1.0.0/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 01:14:32.000000 mmif-python-1.0.0/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.530109 mmif-python-1.0.0/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.530109 mmif-python-1.0.0/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 01:14:32.000000 mmif-python-1.0.0/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 01:14:32.000000 mmif-python-1.0.0/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.534109 mmif-python-1.0.0/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.534109 mmif-python-1.0.0/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 01:13:53.000000 mmif-python-1.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:14:33.534109 mmif-python-1.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-05-26 01:13:53.000000 mmif-python-1.0.0/setup.py
```

### Comparing `mmif-python-0.5.2/LICENSE` & `mmif-python-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/PKG-INFO` & `mmif-python-1.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 0.5.2
+Version: 1.0.0
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-0.5.2/mmif/res/clams.vocabulary.yaml` & `mmif-python-1.0.0/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif/res/mmif.json` & `mmif-python-1.0.0/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif/serialize/annotation.py` & `mmif-python-1.0.0/mmif/serialize/annotation.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif/serialize/mmif.py` & `mmif-python-1.0.0/mmif/serialize/mmif.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif/serialize/model.py` & `mmif-python-1.0.0/mmif/serialize/model.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif/serialize/view.py` & `mmif-python-1.0.0/mmif/serialize/view.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif/vocabulary/annotation_types.py` & `mmif-python-1.0.0/mmif/vocabulary/annotation_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif/vocabulary/base_types.py` & `mmif-python-1.0.0/mmif/vocabulary/base_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif/vocabulary/document_types.py` & `mmif-python-1.0.0/mmif/vocabulary/document_types.py`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/mmif_python.egg-info/PKG-INFO` & `mmif-python-1.0.0/mmif_python.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 0.5.2
+Version: 1.0.0
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-0.5.2/mmif_python.egg-info/SOURCES.txt` & `mmif-python-1.0.0/mmif_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmif-python-0.5.2/setup.py` & `mmif-python-1.0.0/setup.py`

 * *Files identical despite different names*

