# Comparing `tmp/pollination-annual-daylight-en17037-0.1.7.tar.gz` & `tmp/pollination-annual-daylight-en17037-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-annual-daylight-en17037-0.1.7.tar", last modified: Fri May 26 10:49:34 2023, max compression
+gzip compressed data, was "dist/pollination-annual-daylight-en17037-0.1.8.tar", last modified: Fri May 26 11:01:02 2023, max compression
```

## Comparing `pollination-annual-daylight-en17037-0.1.7.tar` & `pollination-annual-daylight-en17037-0.1.8.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/_process_epw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:48:46.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/_process_epw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6679 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:00:17.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:01:02.000000 pollination-annual-daylight-en17037-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 10:59:51.000000 pollination-annual-daylight-en17037-0.1.8/tests/validation_test.py
```

### Comparing `pollination-annual-daylight-en17037-0.1.7/.github/workflows/ci.yaml` & `pollination-annual-daylight-en17037-0.1.8/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.7/.github/workflows/tests.yaml` & `pollination-annual-daylight-en17037-0.1.8/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.7/LICENSE` & `pollination-annual-daylight-en17037-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.7/PKG-INFO` & `pollination-annual-daylight-en17037-0.1.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-en17037
-Version: 0.1.7
+Version: 0.1.8
 Summary: Annual daylight EN17037 recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-en17037
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/_postprocess.py` & `pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/_postprocess.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/_process_epw.py` & `pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/_process_epw.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/entry.py` & `pollination-annual-daylight-en17037-0.1.8/pollination/annual_daylight_en17037/entry.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 # input/output alias
 from pollination.alias.inputs.model import hbjson_model_grid_input
 from pollination.alias.inputs.north import north_input
 from pollination.alias.inputs.radiancepar import rad_par_annual_input, \
     daylight_thresholds_input
 from pollination.alias.inputs.grid import grid_filter_input, \
     min_sensor_count_input, cpu_count
-from pollination.alias.outputs.daylight import annual_daylight_results
+from pollination.alias.outputs.daylight import annual_daylight_results, \
+    daylight_autonomy_results, continuous_daylight_autonomy_results, \
+    udi_results, udi_lower_results, udi_upper_results
 
 from ._process_epw import AnnualDaylightEN17037ProcessEPW
 from ._postprocess import AnnualDaylightEN17037PostProcess
 
 
 @dataclass
 class AnnualDaylightEN17037EntryPoint(DAG):
@@ -141,7 +143,34 @@
     )
 
     metrics = Outputs.folder(
         source='metrics', description='Annual daylight metrics folder. These '
         'metrics are the usual annual daylight metrics with the daylight '
         'hours occupancy schedule.'
     )
+
+    da = Outputs.folder(
+        source='metrics/da', description='Daylight autonomy results.',
+        alias=daylight_autonomy_results
+    )
+
+    cda = Outputs.folder(
+        source='metrics/cda', description='Continuous daylight autonomy results.',
+        alias=continuous_daylight_autonomy_results
+    )
+
+    udi = Outputs.folder(
+        source='metrics/udi', description='Useful daylight illuminance results.',
+        alias=udi_results
+    )
+
+    udi_lower = Outputs.folder(
+        source='metrics/udi_lower', description='Results for the percent of time that '
+        'is below the lower threshold of useful daylight illuminance.',
+        alias=udi_lower_results
+    )
+
+    udi_upper = Outputs.folder(
+        source='metrics/udi_upper', description='Results for the percent of time that '
+        'is above the upper threshold of useful daylight illuminance.',
+        alias=udi_upper_results
+    )
```

### Comparing `pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/PKG-INFO` & `pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-en17037
-Version: 0.1.7
+Version: 0.1.8
 Summary: Annual daylight EN17037 recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-en17037
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/SOURCES.txt` & `pollination-annual-daylight-en17037-0.1.8/pollination_annual_daylight_en17037.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.7/setup.py` & `pollination-annual-daylight-en17037-0.1.8/setup.py`

 * *Files identical despite different names*

