# Comparing `tmp/ccp-performance-0.3.2.tar.gz` & `tmp/ccp-performance-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-gbz19118/ccp-performance-0.3.2.tar", last modified: Thu May 25 20:37:46 2023, max compression
+gzip compressed data, was "/home/runner/work/ccp/ccp/dist/.tmp-wlwizsf7/ccp-performance-0.3.3.tar", last modified: Fri May 26 00:26:01 2023, max compression
```

## Comparing `ccp-performance-0.3.2.tar` & `ccp-performance-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    47176 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/compressor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/config/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/fluids.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/new_units.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/units.py
--rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/config/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/curve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/data_io/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/data_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/data_io/processing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/data_io/read_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/data_io/read_xl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/fo.py
--rw-r--r--   0 runner    (1001) docker     (123)    39930 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/impeller.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/plotly_theme.py
--rw-r--r--   0 runner    (1001) docker     (123)    57872 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/point.py
--rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/similarity.py
--rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/UTGCA_1231_A_1s.csv
--rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/lp-sec1-caso-a-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/lp-sec1-caso-a-head.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/normal-eff.csv
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/ccp/tests/data/normal-head.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/ccp_performance.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 20:37:46.000000 ccp-performance-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-25 20:37:36.000000 ccp-performance-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47176 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/compressor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/config/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4131 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/fluids.py
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/new_units.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/config/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/curve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/data_io/
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/data_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5068 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/data_io/processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/data_io/read_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/data_io/read_xl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/fo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39930 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/impeller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/plotly_theme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57872 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/similarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24461 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   288892 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/UTGCA_1231_A_1s.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   502046 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/lp-sec1-caso-a-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1960 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/lp-sec1-caso-a-head.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/normal-eff.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/ccp/tests/data/normal-head.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2887 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/ccp_performance.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 00:26:01.000000 ccp-performance-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-05-26 00:25:48.000000 ccp-performance-0.3.3/setup.py
```

### Comparing `ccp-performance-0.3.2/LICENSE` & `ccp-performance-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/PKG-INFO` & `ccp-performance-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.3.2
+Version: 0.3.3
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
 Project-URL: Documentation, https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/petrobras/ccp/issues
 Project-URL: Source Code, https://github.com/petrobras/ccp
```

### Comparing `ccp-performance-0.3.2/README.md` & `ccp-performance-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/__init__.py` & `ccp-performance-0.3.3/ccp/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
     _shared_library = "REFPRP64.DLL"
 
 _library_path = _path / _shared_library
 
 if not _library_path.is_file():
     _warnings.warn(f"{_library_path}.\nREFPROP not configured.")
 
-__version__ = "0.3.2"
+__version__ = "0.3.3"
 
 __version__full = (
     f"ccp: {__version__} | "
     + f'CP : {_CP.get_global_param_string("version")} | '
     + f'REFPROP : {_CP.get_global_param_string("REFPROP_version")}'
 )
```

### Comparing `ccp-performance-0.3.2/ccp/compressor.py` & `ccp-performance-0.3.3/ccp/compressor.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/config/fluids.py` & `ccp-performance-0.3.3/ccp/config/fluids.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/config/units.py` & `ccp-performance-0.3.3/ccp/config/units.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/curve.py` & `ccp-performance-0.3.3/ccp/curve.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/data_io/processing.py` & `ccp-performance-0.3.3/ccp/data_io/processing.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/data_io/read_csv.py` & `ccp-performance-0.3.3/ccp/data_io/read_csv.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/fo.py` & `ccp-performance-0.3.3/ccp/fo.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/impeller.py` & `ccp-performance-0.3.3/ccp/impeller.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/plotly_theme.py` & `ccp-performance-0.3.3/ccp/plotly_theme.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/point.py` & `ccp-performance-0.3.3/ccp/point.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/similarity.py` & `ccp-performance-0.3.3/ccp/similarity.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/state.py` & `ccp-performance-0.3.3/ccp/state.py`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/tests/data/UTGCA_1231_A_1s.csv` & `ccp-performance-0.3.3/ccp/tests/data/UTGCA_1231_A_1s.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h` & `ccp-performance-0.3.3/ccp/tests/data/UTGCA_1231_A_2019-01-01T00_00_00_2020-12-11T00_00_00_12h`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/tests/data/lp-sec1-caso-a-eff.csv` & `ccp-performance-0.3.3/ccp/tests/data/lp-sec1-caso-a-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/tests/data/lp-sec1-caso-a-head.csv` & `ccp-performance-0.3.3/ccp/tests/data/lp-sec1-caso-a-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/tests/data/normal-eff.csv` & `ccp-performance-0.3.3/ccp/tests/data/normal-eff.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp/tests/data/normal-head.csv` & `ccp-performance-0.3.3/ccp/tests/data/normal-head.csv`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/ccp_performance.egg-info/PKG-INFO` & `ccp-performance-0.3.3/ccp_performance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ccp-performance
-Version: 0.3.2
+Version: 0.3.3
 Summary: Centrifugal Compressor Performance calculation.
 Author: Raphael Timbó
 Author-email: raphaelts@petrobras.com.br
 License: Apache License 2.0
 Project-URL: Documentation, https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/
 Project-URL: Bug Tracker, https://github.com/petrobras/ccp/issues
 Project-URL: Source Code, https://github.com/petrobras/ccp
```

### Comparing `ccp-performance-0.3.2/ccp_performance.egg-info/SOURCES.txt` & `ccp-performance-0.3.3/ccp_performance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ccp-performance-0.3.2/setup.py` & `ccp-performance-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,14 +56,15 @@
     author="Raphael Timbó",
     author_email="raphaelts@petrobras.com.br",
     project_urls={
         "Documentation": "https://ccp-centrifugal-compressor-performance.readthedocs.io/en/stable/",
         "Bug Tracker": "https://github.com/petrobras/ccp/issues",
         "Source Code": "https://github.com/petrobras/ccp",
     },
+    include_package_data=True,
     package_data={"ccp.config": ["new_units.txt"], "ccp.tests.data": ["*"]},
     python_requires=">=3.6",
     install_requires=REQUIRES,
     extras_require={
         "dev": [
             "pytest",
             "pytest-cov",
```

