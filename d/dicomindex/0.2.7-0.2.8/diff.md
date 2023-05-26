# Comparing `tmp/dicomindex-0.2.7.tar.gz` & `tmp/dicomindex-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicomindex-0.2.7.tar", max compression
+gzip compressed data, was "dicomindex-0.2.8.tar", max compression
```

## Comparing `dicomindex-0.2.7.tar` & `dicomindex-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0        0 2023-04-24 12:37:10.935914 dicomindex-0.2.7/dicomindex/__init__.py
--rw-r--r--   0        0        0     3577 2023-05-19 18:10:28.453258 dicomindex-0.2.7/dicomindex/cli.py
--rw-r--r--   0        0        0      552 2023-05-15 18:44:04.167863 dicomindex-0.2.7/dicomindex/core.py
--rw-r--r--   0        0        0     2128 2023-05-24 09:13:50.175910 dicomindex-0.2.7/dicomindex/dataset.py
--rw-r--r--   0        0        0      186 2023-05-15 18:44:04.167863 dicomindex-0.2.7/dicomindex/exceptions.py
--rw-r--r--   0        0        0     4380 2023-05-01 10:43:16.779259 dicomindex-0.2.7/dicomindex/fields.py
--rw-r--r--   0        0        0     2410 2023-05-19 18:10:28.453258 dicomindex-0.2.7/dicomindex/iterators.py
--rw-r--r--   0        0        0      138 2023-05-01 11:02:04.380560 dicomindex-0.2.7/dicomindex/logs.py
--rw-r--r--   0        0        0     9942 2023-05-15 18:44:04.167863 dicomindex-0.2.7/dicomindex/orm.py
--rw-r--r--   0        0        0      766 2023-05-15 18:44:04.167863 dicomindex-0.2.7/dicomindex/persistence.py
--rw-r--r--   0        0        0     9483 2023-05-24 09:13:50.335911 dicomindex-0.2.7/dicomindex/processing.py
--rw-r--r--   0        0        0     1850 2023-05-22 13:39:59.156988 dicomindex-0.2.7/dicomindex/statistics.py
--rw-r--r--   0        0        0     4279 2023-05-23 13:07:30.546035 dicomindex-0.2.7/dicomindex/threading.py
--rw-r--r--   0        0        0     2377 2023-05-01 10:55:22.033601 dicomindex-0.2.7/dicomindex/types.py
--rw-r--r--   0        0        0      655 2023-05-24 09:14:38.796362 dicomindex-0.2.7/pyproject.toml
--rw-r--r--   0        0        0      866 2023-05-24 09:14:47.253791 dicomindex-0.2.7/setup.py
--rw-r--r--   0        0        0      622 2023-05-24 09:14:47.254003 dicomindex-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 08:31:31.490764 dicomindex-0.2.8/dicomindex/__init__.py
+-rw-r--r--   0        0        0     3577 2023-05-26 08:31:31.490764 dicomindex-0.2.8/dicomindex/cli.py
+-rw-r--r--   0        0        0      552 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/core.py
+-rw-r--r--   0        0        0     2128 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/dataset.py
+-rw-r--r--   0        0        0      186 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/exceptions.py
+-rw-r--r--   0        0        0     4380 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/fields.py
+-rw-r--r--   0        0        0     2410 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/iterators.py
+-rw-r--r--   0        0        0      138 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/logs.py
+-rw-r--r--   0        0        0     9942 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/orm.py
+-rw-r--r--   0        0        0      766 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/persistence.py
+-rw-r--r--   0        0        0     9483 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/processing.py
+-rw-r--r--   0        0        0     1850 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/statistics.py
+-rw-r--r--   0        0        0     4279 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/threading.py
+-rw-r--r--   0        0        0     2377 2023-05-26 08:31:31.494764 dicomindex-0.2.8/dicomindex/types.py
+-rw-r--r--   0        0        0      638 2023-05-26 08:31:31.494764 dicomindex-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 dicomindex-0.2.8/PKG-INFO
```

### Comparing `dicomindex-0.2.7/dicomindex/cli.py` & `dicomindex-0.2.8/dicomindex/cli.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/core.py` & `dicomindex-0.2.8/dicomindex/core.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/dataset.py` & `dicomindex-0.2.8/dicomindex/dataset.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/fields.py` & `dicomindex-0.2.8/dicomindex/fields.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/iterators.py` & `dicomindex-0.2.8/dicomindex/iterators.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/orm.py` & `dicomindex-0.2.8/dicomindex/orm.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/persistence.py` & `dicomindex-0.2.8/dicomindex/persistence.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/processing.py` & `dicomindex-0.2.8/dicomindex/processing.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/statistics.py` & `dicomindex-0.2.8/dicomindex/statistics.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/threading.py` & `dicomindex-0.2.8/dicomindex/threading.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/dicomindex/types.py` & `dicomindex-0.2.8/dicomindex/types.py`

 * *Files identical despite different names*

### Comparing `dicomindex-0.2.7/pyproject.toml` & `dicomindex-0.2.8/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "dicomindex"
-version = "0.2.7"
-description = "Index dicom files into patient->study->series->instance"
+version = "0.2.8"
+description = "Index dicom files into sqlite database"
 authors = ["sjoerdk <sjoerd.kerkstra@radboudumc.nl>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 pydicom = "^2.3.1"
 SQLAlchemy = "^2.0.10"
```

### Comparing `dicomindex-0.2.7/PKG-INFO` & `dicomindex-0.2.8/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: dicomindex
-Version: 0.2.7
-Summary: Index dicom files into patient->study->series->instance
+Version: 0.2.8
+Summary: Index dicom files into sqlite database
 License: MIT
 Author: sjoerdk
 Author-email: sjoerd.kerkstra@radboudumc.nl
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: SQLAlchemy (>=2.0.10,<3.0.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: pydicom (>=2.3.1,<3.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
```

