# Comparing `tmp/adafruit-circuitpython-sht31d-2.3.8.tar.gz` & `tmp/adafruit-circuitpython-sht31d-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-sht31d-2.3.8.tar", last modified: Wed Dec 29 21:19:40 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-sht31d-2.3.9.tar", last modified: Mon Jan  3 20:59:54 2022, max compression
```

## Comparing `adafruit-circuitpython-sht31d-2.3.8.tar` & `adafruit-circuitpython-sht31d-2.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.035848 adafruit-circuitpython-sht31d-2.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4107 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/adafruit_circuitpython_sht31d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4966 2021-12-29 21:19:39.000000 adafruit-circuitpython-sht31d-2.3.8/adafruit_circuitpython_sht31d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      951 2021-12-29 21:19:39.000000 adafruit-circuitpython-sht31d-2.3.8/adafruit_circuitpython_sht31d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-29 21:19:39.000000 adafruit-circuitpython-sht31d-2.3.8/adafruit_circuitpython_sht31d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-29 21:19:39.000000 adafruit-circuitpython-sht31d-2.3.8/adafruit_circuitpython_sht31d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-12-29 21:19:39.000000 adafruit-circuitpython-sht31d-2.3.8/adafruit_circuitpython_sht31d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    12625 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/adafruit_sht31d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      125 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5595 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      567 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1029 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/examples/sht31d_periodic_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/examples/sht31d_simple_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/examples/sht31d_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-29 21:19:40.039847 adafruit-circuitpython-sht31d-2.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1981 2021-12-29 21:19:28.000000 adafruit-circuitpython-sht31d-2.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.758933 adafruit-circuitpython-sht31d-2.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.754932 adafruit-circuitpython-sht31d-2.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.754932 adafruit-circuitpython-sht31d-2.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.754932 adafruit-circuitpython-sht31d-2.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.754932 adafruit-circuitpython-sht31d-2.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-01-03 20:59:54.758933 adafruit-circuitpython-sht31d-2.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4107 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.758933 adafruit-circuitpython-sht31d-2.3.9/adafruit_circuitpython_sht31d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4966 2022-01-03 20:59:54.000000 adafruit-circuitpython-sht31d-2.3.9/adafruit_circuitpython_sht31d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      951 2022-01-03 20:59:54.000000 adafruit-circuitpython-sht31d-2.3.9/adafruit_circuitpython_sht31d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 20:59:54.000000 adafruit-circuitpython-sht31d-2.3.9/adafruit_circuitpython_sht31d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-01-03 20:59:54.000000 adafruit-circuitpython-sht31d-2.3.9/adafruit_circuitpython_sht31d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-01-03 20:59:54.000000 adafruit-circuitpython-sht31d-2.3.9/adafruit_circuitpython_sht31d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    12631 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/adafruit_sht31d.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.758933 adafruit-circuitpython-sht31d-2.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.758933 adafruit-circuitpython-sht31d-2.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5595 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      567 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 20:59:54.758933 adafruit-circuitpython-sht31d-2.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1029 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/examples/sht31d_periodic_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/examples/sht31d_simple_mode.py
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/examples/sht31d_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-03 20:59:54.758933 adafruit-circuitpython-sht31d-2.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1981 2022-01-03 20:59:41.000000 adafruit-circuitpython-sht31d-2.3.9/setup.py
```

### Comparing `adafruit-circuitpython-sht31d-2.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-sht31d-2.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-sht31d-2.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-sht31d-2.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-sht31d-2.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/.pylintrc` & `adafruit-circuitpython-sht31d-2.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-sht31d-2.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/LICENSE` & `adafruit-circuitpython-sht31d-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-sht31d-2.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-sht31d-2.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-sht31d-2.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/PKG-INFO` & `adafruit-circuitpython-sht31d-2.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sht31d
-Version: 2.3.8
+Version: 2.3.9
 Summary: CircuitPython library for SHT31-D temperature and humidity sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SHT31-D
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit sht31d sht31-d temperature humidity sensorhardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-sht31d-2.3.8/README.rst` & `adafruit-circuitpython-sht31d-2.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/adafruit_circuitpython_sht31d.egg-info/PKG-INFO` & `adafruit-circuitpython-sht31d-2.3.9/adafruit_circuitpython_sht31d.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sht31d
-Version: 2.3.8
+Version: 2.3.9
 Summary: CircuitPython library for SHT31-D temperature and humidity sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_SHT31-D
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit sht31d sht31-d temperature humidity sensorhardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-sht31d-2.3.8/adafruit_circuitpython_sht31d.egg-info/SOURCES.txt` & `adafruit-circuitpython-sht31d-2.3.9/adafruit_circuitpython_sht31d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/adafruit_sht31d.py` & `adafruit-circuitpython-sht31d-2.3.9/adafruit_sht31d.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,18 +111,18 @@
 def _crc(data):
     crc = 0xFF
     for byte in data:
         crc ^= byte
         for _ in range(8):
             if crc & 0x80:
                 crc <<= 1
-                crc ^= 0x131
+                crc ^= 0x31
             else:
                 crc <<= 1
-    return crc
+    return crc & 0xFF
 
 
 def _unpack(data):
     length = len(data)
     crc = [None] * (length // 3)
     word = [None] * (length // 3)
     for i in range(length // 6):
```

### Comparing `adafruit-circuitpython-sht31d-2.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-sht31d-2.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/docs/conf.py` & `adafruit-circuitpython-sht31d-2.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/docs/examples.rst` & `adafruit-circuitpython-sht31d-2.3.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/docs/index.rst` & `adafruit-circuitpython-sht31d-2.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/examples/sht31d_periodic_mode.py` & `adafruit-circuitpython-sht31d-2.3.9/examples/sht31d_periodic_mode.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/examples/sht31d_simple_mode.py` & `adafruit-circuitpython-sht31d-2.3.9/examples/sht31d_simple_mode.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/examples/sht31d_simpletest.py` & `adafruit-circuitpython-sht31d-2.3.9/examples/sht31d_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sht31d-2.3.8/setup.py` & `adafruit-circuitpython-sht31d-2.3.9/setup.py`

 * *Files identical despite different names*

