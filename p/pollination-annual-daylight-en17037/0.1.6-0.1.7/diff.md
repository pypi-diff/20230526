# Comparing `tmp/pollination-annual-daylight-en17037-0.1.6.tar.gz` & `tmp/pollination-annual-daylight-en17037-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pollination-annual-daylight-en17037-0.1.6.tar", last modified: Tue May 16 11:15:31 2023, max compression
+gzip compressed data, was "dist/pollination-annual-daylight-en17037-0.1.7.tar", last modified: Fri May 26 10:49:34 2023, max compression
```

## Comparing `pollination-annual-daylight-en17037-0.1.6.tar` & `pollination-annual-daylight-en17037-0.1.7.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/.releaserc.json
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/deploy.sh
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/extras-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/pollination/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/pollination/annual_daylight_en17037/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/pollination/annual_daylight_en17037/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/pollination/annual_daylight_en17037/_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/pollination/annual_daylight_en17037/_process_epw.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/pollination/annual_daylight_en17037/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 11:14:53.000000 pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 11:15:31.000000 pollination-annual-daylight-en17037-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-16 11:14:32.000000 pollination-annual-daylight-en17037-0.1.6/tests/validation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/.releaserc.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/deploy.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/extras-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2582 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/_process_epw.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5638 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:48:46.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:49:34.000000 pollination-annual-daylight-en17037-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-26 10:48:18.000000 pollination-annual-daylight-en17037-0.1.7/tests/validation_test.py
```

### Comparing `pollination-annual-daylight-en17037-0.1.6/.github/workflows/ci.yaml` & `pollination-annual-daylight-en17037-0.1.7/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.6/.github/workflows/tests.yaml` & `pollination-annual-daylight-en17037-0.1.7/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.6/LICENSE` & `pollination-annual-daylight-en17037-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.6/PKG-INFO` & `pollination-annual-daylight-en17037-0.1.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-en17037
-Version: 0.1.6
+Version: 0.1.7
 Summary: Annual daylight EN17037 recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-en17037
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-en17037-0.1.6/pollination/annual_daylight_en17037/_postprocess.py` & `pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/_postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from pollination_dsl.dag import Inputs, GroupedDAG, task, Outputs
 from dataclasses import dataclass
-from pollination.honeybee_radiance_postprocess.post_process import AnnualDaylightEN17037Metrics
+from pollination.honeybee_radiance_postprocess.post_process import AnnualDaylightEn17037Metrics
 from pollination.honeybee_radiance_postprocess.post_process import AnnualDaylightMetrics
 
 # input/output alias
 from pollination.alias.inputs.radiancepar import daylight_thresholds_input
 from pollination.alias.inputs.schedule import schedule_csv_input
 
 
@@ -30,21 +30,21 @@
         'threshold. The default is -t 300 -lt 100 -ut 3000. The order of the keys is '
         'not important and you can include one or all of them. For instance if you only '
         'want to change the upper threshold to 2000 lux you should use -ut 2000 as '
         'the input.', default='-t 300 -lt 100 -ut 3000',
         alias=daylight_thresholds_input
     )
 
-    @task(template=AnnualDaylightEN17037Metrics)
+    @task(template=AnnualDaylightEn17037Metrics)
     def calculate_annual_metrics_en17037(
         self, folder=results, schedule=schedule
     ):
         return [
             {
-                'from': AnnualDaylightEN17037Metrics()._outputs.annual_en17037_metrics,
+                'from': AnnualDaylightEn17037Metrics()._outputs.annual_en17037_metrics,
                 'to': 'en17037'
             }
         ]
 
     @task(template=AnnualDaylightMetrics)
     def calculate_annual_metrics(
         self, folder=results, schedule=schedule, thresholds=thresholds
```

### Comparing `pollination-annual-daylight-en17037-0.1.6/pollination/annual_daylight_en17037/_process_epw.py` & `pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/_process_epw.py`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.6/pollination/annual_daylight_en17037/entry.py` & `pollination-annual-daylight-en17037-0.1.7/pollination/annual_daylight_en17037/entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,10 @@
 from pollination_dsl.dag import Inputs, DAG, task, Outputs
 from dataclasses import dataclass
 from pollination.two_phase_daylight_coefficient import TwoPhaseDaylightCoefficientEntryPoint
-from pollination.honeybee_radiance_postprocess.post_process import AnnualDaylightEN17037Metrics
-from pollination.honeybee_radiance.schedule import EPWtoDaylightHours
-from pollination.ladybug.translate import EpwToWea
 
 # input/output alias
 from pollination.alias.inputs.model import hbjson_model_grid_input
 from pollination.alias.inputs.north import north_input
 from pollination.alias.inputs.radiancepar import rad_par_annual_input, \
     daylight_thresholds_input
 from pollination.alias.inputs.grid import grid_filter_input, \
```

### Comparing `pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/PKG-INFO` & `pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pollination-annual-daylight-en17037
-Version: 0.1.6
+Version: 0.1.7
 Summary: Annual daylight EN17037 recipe for Pollination.
 Home-page: https://github.com/pollination/annual-daylight-en17037
 Author: ladybug-tools
 Author-email: info@ladybug.tools
 Maintainer: mostapha, ladybug-tools
 Maintainer-email: mostapha@ladybug.tools, info@ladybug.tools
 License: PolyForm Shield License 1.0.0, https://polyformproject.org/wp-content/uploads/2020/06/PolyForm-Shield-1.0.0.txt
```

### Comparing `pollination-annual-daylight-en17037-0.1.6/pollination_annual_daylight_en17037.egg-info/SOURCES.txt` & `pollination-annual-daylight-en17037-0.1.7/pollination_annual_daylight_en17037.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pollination-annual-daylight-en17037-0.1.6/setup.py` & `pollination-annual-daylight-en17037-0.1.7/setup.py`

 * *Files identical despite different names*

