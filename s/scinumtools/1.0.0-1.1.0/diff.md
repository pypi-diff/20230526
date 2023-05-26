# Comparing `tmp/scinumtools-1.0.0.tar.gz` & `tmp/scinumtools-1.1.0.tar.gz`

## Comparing `scinumtools-1.0.0.tar` & `scinumtools-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 scinumtools-1.0.0/requirements.txt
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.0.0/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.0.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/data/CachingClass.py
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/data/__init__.py
--rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/stats/StopwatchClass.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/stats/__init__.py
--rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/structs/CollectorClass.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/structs/ParameterClass.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.0.0/src/scinumtools/structs/__init__.py
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.0.0/tests/cached_data.npy
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 scinumtools-1.0.0/tests/test_data.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.0.0/tests/test_stats.py
--rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.0.0/tests/test_struct.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.0.0/.gitignore
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.0.0/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 scinumtools-1.1.0/requirements.txt
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 scinumtools-1.1.0/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 scinumtools-1.1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/data/CachingClass.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/data/PlottingClass.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/data/__init__.py
+-rw-r--r--   0        0        0     2606 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/stats/StopwatchClass.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/stats/__init__.py
+-rw-r--r--   0        0        0     5397 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/structs/CollectorClass.py
+-rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/structs/ParameterClass.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 scinumtools-1.1.0/src/scinumtools/structs/__init__.py
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 scinumtools-1.1.0/tests/cached_data.npy
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 scinumtools-1.1.0/tests/test_data.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 scinumtools-1.1.0/tests/test_stats.py
+-rw-r--r--   0        0        0     3986 2020-02-02 00:00:00.000000 scinumtools-1.1.0/tests/test_struct.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 scinumtools-1.1.0/.gitignore
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 scinumtools-1.1.0/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 scinumtools-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 scinumtools-1.1.0/PKG-INFO
```

### Comparing `scinumtools-1.0.0/.github/workflows/python-publish.yml` & `scinumtools-1.1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `scinumtools-1.0.0/src/scinumtools/stats/StopwatchClass.py` & `scinumtools-1.1.0/src/scinumtools/stats/StopwatchClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.0.0/src/scinumtools/structs/CollectorClass.py` & `scinumtools-1.1.0/src/scinumtools/structs/CollectorClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.0.0/src/scinumtools/structs/ParameterClass.py` & `scinumtools-1.1.0/src/scinumtools/structs/ParameterClass.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.0.0/tests/test_stats.py` & `scinumtools-1.1.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.0.0/tests/test_struct.py` & `scinumtools-1.1.0/tests/test_struct.py`

 * *Files identical despite different names*

### Comparing `scinumtools-1.0.0/.gitignore` & `scinumtools-1.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `scinumtools-1.0.0/pyproject.toml` & `scinumtools-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "scinumtools"
-version = "1.0.0"
+version = "1.1.0"
 authors = [
   { name="Ondrej Pego Jaura", email="vrtulka23@pm.me" },
 ]
 description = "Set of most frequently used tools for a rapid numerical code development in Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `scinumtools-1.0.0/PKG-INFO` & `scinumtools-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scinumtools
-Version: 1.0.0
+Version: 1.1.0
 Summary: Set of most frequently used tools for a rapid numerical code development in Python.
 Project-URL: Homepage, https://github.com/vrtulka23/scinumtools
 Project-URL: Bug Tracker, https://github.com/vrtulka23/scinumtools/issues
 Author-email: Ondrej Pego Jaura <vrtulka23@pm.me>
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

