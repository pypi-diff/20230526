# Comparing `tmp/FTSF-0.0.1.tar.gz` & `tmp/FTSF-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FTSF-0.0.1.tar", last modified: Fri May 26 04:46:58 2023, max compression
+gzip compressed data, was "FTSF-0.0.1.1.tar", last modified: Fri May 26 05:15:35 2023, max compression
```

## Comparing `FTSF-0.0.1.tar` & `FTSF-0.0.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 04:46:58.628268 FTSF-0.0.1/
-drwxrwxrwx   0        0        0        0 2023-05-26 04:46:58.602089 FTSF-0.0.1/FTSF.egg-info/
--rw-rw-rw-   0        0        0      632 2023-05-26 04:46:58.000000 FTSF-0.0.1/FTSF.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-26 04:46:58.000000 FTSF-0.0.1/FTSF.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 04:46:58.000000 FTSF-0.0.1/FTSF.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2023-05-26 04:46:58.000000 FTSF-0.0.1/FTSF.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2023-05-26 04:46:58.000000 FTSF-0.0.1/FTSF.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1100 2023-05-26 02:11:38.000000 FTSF-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      632 2023-05-26 04:46:58.625788 FTSF-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       11 2023-05-26 00:42:20.000000 FTSF-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 04:46:58.623040 FTSF-0.0.1/ftsf/
--rw-rw-rw-   0        0        0        0 2023-05-25 02:03:02.000000 FTSF-0.0.1/ftsf/__init__.py
--rw-rw-rw-   0        0        0     3285 2023-05-26 04:39:44.000000 FTSF-0.0.1/ftsf/backtest.py
--rw-rw-rw-   0        0        0     7953 2023-05-26 04:29:35.000000 FTSF-0.0.1/ftsf/evaluation.py
--rw-rw-rw-   0        0        0    11333 2023-05-26 01:07:23.000000 FTSF-0.0.1/ftsf/ftsf.py
--rw-rw-rw-   0        0        0     7189 2023-05-26 04:42:35.000000 FTSF-0.0.1/ftsf/model.py
--rw-rw-rw-   0        0        0        0 2023-05-25 18:39:04.000000 FTSF-0.0.1/ftsf/pipeline.py
--rw-rw-rw-   0        0        0     4486 2023-05-26 04:29:45.000000 FTSF-0.0.1/ftsf/preprocessing.py
--rw-rw-rw-   0        0        0     1873 2023-05-25 16:16:36.000000 FTSF-0.0.1/ftsf/scaler.py
-drwxrwxrwx   0        0        0        0 2023-05-26 04:46:58.625044 FTSF-0.0.1/ftsf/tests/
--rw-rw-rw-   0        0        0      629 2023-05-25 02:40:23.000000 FTSF-0.0.1/ftsf/tests/test_scaler.py
--rw-rw-rw-   0        0        0     4902 2023-05-26 04:42:22.000000 FTSF-0.0.1/ftsf/utils.py
--rw-rw-rw-   0        0        0      877 2023-05-26 02:23:53.000000 FTSF-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 04:46:58.629279 FTSF-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 05:15:35.076892 FTSF-0.0.1.1/
+drwxrwxrwx   0        0        0        0 2023-05-26 05:15:35.049480 FTSF-0.0.1.1/FTSF.egg-info/
+-rw-rw-rw-   0        0        0      634 2023-05-26 05:15:34.000000 FTSF-0.0.1.1/FTSF.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      345 2023-05-26 05:15:35.000000 FTSF-0.0.1.1/FTSF.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 05:15:34.000000 FTSF-0.0.1.1/FTSF.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-26 05:15:34.000000 FTSF-0.0.1.1/FTSF.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2023-05-26 05:15:34.000000 FTSF-0.0.1.1/FTSF.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1100 2023-05-26 02:11:38.000000 FTSF-0.0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      634 2023-05-26 05:15:35.074891 FTSF-0.0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       11 2023-05-26 00:42:20.000000 FTSF-0.0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 05:15:35.069830 FTSF-0.0.1.1/ftsf/
+-rw-rw-rw-   0        0        0        0 2023-05-25 02:03:02.000000 FTSF-0.0.1.1/ftsf/__init__.py
+-rw-rw-rw-   0        0        0     3285 2023-05-26 04:39:44.000000 FTSF-0.0.1.1/ftsf/backtest.py
+-rw-rw-rw-   0        0        0     7953 2023-05-26 04:29:35.000000 FTSF-0.0.1.1/ftsf/evaluation.py
+-rw-rw-rw-   0        0        0    11333 2023-05-26 01:07:23.000000 FTSF-0.0.1.1/ftsf/ftsf.py
+-rw-rw-rw-   0        0        0     7189 2023-05-26 04:42:35.000000 FTSF-0.0.1.1/ftsf/model.py
+-rw-rw-rw-   0        0        0        0 2023-05-25 18:39:04.000000 FTSF-0.0.1.1/ftsf/pipeline.py
+-rw-rw-rw-   0        0        0     4486 2023-05-26 04:29:45.000000 FTSF-0.0.1.1/ftsf/preprocessing.py
+-rw-rw-rw-   0        0        0     1873 2023-05-25 16:16:36.000000 FTSF-0.0.1.1/ftsf/scaler.py
+drwxrwxrwx   0        0        0        0 2023-05-26 05:15:35.071882 FTSF-0.0.1.1/ftsf/tests/
+-rw-rw-rw-   0        0        0      629 2023-05-25 02:40:23.000000 FTSF-0.0.1.1/ftsf/tests/test_scaler.py
+-rw-rw-rw-   0        0        0     4902 2023-05-26 04:42:22.000000 FTSF-0.0.1.1/ftsf/utils.py
+-rw-rw-rw-   0        0        0      819 2023-05-26 05:15:13.000000 FTSF-0.0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 05:15:35.076892 FTSF-0.0.1.1/setup.cfg
```

### Comparing `FTSF-0.0.1/FTSF.egg-info/PKG-INFO` & `FTSF-0.0.1.1/FTSF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FTSF
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Package for financial time series forecasting.
 Author-email: Nikita Safonov <sixxio@yandex.ru>
 Project-URL: Homepage, https://github.com/sixxio/ftsf
 Project-URL: Documentation, https://sixxio.github.io/ftsf/
 Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FTSF-0.0.1/LICENSE` & `FTSF-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/PKG-INFO` & `FTSF-0.0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FTSF
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: Package for financial time series forecasting.
 Author-email: Nikita Safonov <sixxio@yandex.ru>
 Project-URL: Homepage, https://github.com/sixxio/ftsf
 Project-URL: Documentation, https://sixxio.github.io/ftsf/
 Project-URL: Bug Tracker, https://github.com/sixxio/ftsf/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
```

### Comparing `FTSF-0.0.1/ftsf/backtest.py` & `FTSF-0.0.1.1/ftsf/backtest.py`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/ftsf/evaluation.py` & `FTSF-0.0.1.1/ftsf/evaluation.py`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/ftsf/ftsf.py` & `FTSF-0.0.1.1/ftsf/ftsf.py`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/ftsf/model.py` & `FTSF-0.0.1.1/ftsf/model.py`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/ftsf/preprocessing.py` & `FTSF-0.0.1.1/ftsf/preprocessing.py`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/ftsf/scaler.py` & `FTSF-0.0.1.1/ftsf/scaler.py`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/ftsf/tests/test_scaler.py` & `FTSF-0.0.1.1/ftsf/tests/test_scaler.py`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/ftsf/utils.py` & `FTSF-0.0.1.1/ftsf/utils.py`

 * *Files identical despite different names*

### Comparing `FTSF-0.0.1/pyproject.toml` & `FTSF-0.0.1.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "FTSF"
-version = "0.0.1"
+version = "0.0.1.1"
 authors = [
   { name="Nikita Safonov", email="sixxio@yandex.ru" },
 ]
 description = "Package for financial time series forecasting."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-  "requests",
-  "re",
-  "json",
-  "time",
-  "pathlib",
   "numpy",
   "pandas",
   "scikit-learn",
   "statsmodels",
   "catboost",
   "xgboost",
   "tensorflow",
```

