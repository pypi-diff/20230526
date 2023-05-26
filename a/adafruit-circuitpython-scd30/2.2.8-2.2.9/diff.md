# Comparing `tmp/adafruit-circuitpython-scd30-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-scd30-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-scd30-2.2.8.tar", last modified: Fri Aug 26 02:29:01 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-scd30-2.2.9.tar", last modified: Sat Aug 27 01:03:41 2022, max compression
```

## Comparing `adafruit-circuitpython-scd30-2.2.8.tar` & `adafruit-circuitpython-scd30-2.2.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.261653 adafruit-circuitpython-scd30-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.253653 adafruit-circuitpython-scd30-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.253653 adafruit-circuitpython-scd30-2.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.257653 adafruit-circuitpython-scd30-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.257653 adafruit-circuitpython-scd30-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-08-26 02:29:01.261653 adafruit-circuitpython-scd30-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3355 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.257653 adafruit-circuitpython-scd30-2.2.8/adafruit_circuitpython_scd30.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-08-26 02:29:01.000000 adafruit-circuitpython-scd30-2.2.8/adafruit_circuitpython_scd30.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-08-26 02:29:01.000000 adafruit-circuitpython-scd30-2.2.8/adafruit_circuitpython_scd30.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:29:01.000000 adafruit-circuitpython-scd30-2.2.8/adafruit_circuitpython_scd30.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:29:01.000000 adafruit-circuitpython-scd30-2.2.8/adafruit_circuitpython_scd30.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-26 02:29:01.000000 adafruit-circuitpython-scd30-2.2.8/adafruit_circuitpython_scd30.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    11477 2022-08-26 02:28:49.000000 adafruit-circuitpython-scd30-2.2.8/adafruit_scd30.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.257653 adafruit-circuitpython-scd30-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.257653 adafruit-circuitpython-scd30-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5948 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      618 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:29:01.261653 adafruit-circuitpython-scd30-2.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      959 2022-08-26 02:28:49.000000 adafruit-circuitpython-scd30-2.2.8/examples/scd30_ft232htest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-08-26 02:28:49.000000 adafruit-circuitpython-scd30-2.2.8/examples/scd30_mcp2221test.py
--rw-r--r--   0 runner    (1001) docker     (121)      840 2022-08-26 02:28:49.000000 adafruit-circuitpython-scd30-2.2.8/examples/scd30_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-08-26 02:28:49.000000 adafruit-circuitpython-scd30-2.2.8/examples/scd30_tuning_knobs.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-08-26 02:28:49.000000 adafruit-circuitpython-scd30-2.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:28:29.000000 adafruit-circuitpython-scd30-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:29:01.261653 adafruit-circuitpython-scd30-2.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.241861 adafruit-circuitpython-scd30-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.233861 adafruit-circuitpython-scd30-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.237861 adafruit-circuitpython-scd30-2.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.237861 adafruit-circuitpython-scd30-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.237861 adafruit-circuitpython-scd30-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-08-27 01:03:41.241861 adafruit-circuitpython-scd30-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3355 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.237861 adafruit-circuitpython-scd30-2.2.9/adafruit_circuitpython_scd30.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-08-27 01:03:41.000000 adafruit-circuitpython-scd30-2.2.9/adafruit_circuitpython_scd30.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1002 2022-08-27 01:03:41.000000 adafruit-circuitpython-scd30-2.2.9/adafruit_circuitpython_scd30.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 01:03:41.000000 adafruit-circuitpython-scd30-2.2.9/adafruit_circuitpython_scd30.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-27 01:03:41.000000 adafruit-circuitpython-scd30-2.2.9/adafruit_circuitpython_scd30.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-27 01:03:41.000000 adafruit-circuitpython-scd30-2.2.9/adafruit_circuitpython_scd30.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    11947 2022-08-27 01:03:31.000000 adafruit-circuitpython-scd30-2.2.9/adafruit_scd30.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.241861 adafruit-circuitpython-scd30-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.241861 adafruit-circuitpython-scd30-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5948 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      618 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:03:41.241861 adafruit-circuitpython-scd30-2.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      959 2022-08-27 01:03:31.000000 adafruit-circuitpython-scd30-2.2.9/examples/scd30_ft232htest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-08-27 01:03:31.000000 adafruit-circuitpython-scd30-2.2.9/examples/scd30_mcp2221test.py
+-rw-r--r--   0 runner    (1001) docker     (121)      840 2022-08-27 01:03:31.000000 adafruit-circuitpython-scd30-2.2.9/examples/scd30_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1274 2022-08-27 01:03:31.000000 adafruit-circuitpython-scd30-2.2.9/examples/scd30_tuning_knobs.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1208 2022-08-27 01:03:31.000000 adafruit-circuitpython-scd30-2.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      220 2022-08-27 01:03:17.000000 adafruit-circuitpython-scd30-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 01:03:41.241861 adafruit-circuitpython-scd30-2.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-scd30-2.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-scd30-2.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-scd30-2.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-scd30-2.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/.gitignore` & `adafruit-circuitpython-scd30-2.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-scd30-2.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/.pylintrc` & `adafruit-circuitpython-scd30-2.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-scd30-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/LICENSE` & `adafruit-circuitpython-scd30-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-scd30-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-scd30-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-scd30-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/PKG-INFO` & `adafruit-circuitpython-scd30-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-scd30
-Version: 2.2.8
+Version: 2.2.9
 Summary: Helper library for the SCD30 CO2 sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SCD30
 Keywords: adafruit,blinka,circuitpython,micropython,scd30,e-CO2,CO2,air,quality
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-scd30-2.2.8/README.rst` & `adafruit-circuitpython-scd30-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/adafruit_circuitpython_scd30.egg-info/PKG-INFO` & `adafruit-circuitpython-scd30-2.2.9/adafruit_circuitpython_scd30.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-scd30
-Version: 2.2.8
+Version: 2.2.9
 Summary: Helper library for the SCD30 CO2 sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SCD30
 Keywords: adafruit,blinka,circuitpython,micropython,scd30,e-CO2,CO2,air,quality
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-scd30-2.2.8/adafruit_circuitpython_scd30.egg-info/SOURCES.txt` & `adafruit-circuitpython-scd30-2.2.9/adafruit_circuitpython_scd30.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/adafruit_scd30.py` & `adafruit-circuitpython-scd30-2.2.9/adafruit_scd30.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,16 +29,22 @@
 
 # imports
 import time
 from struct import unpack_from, unpack
 from adafruit_bus_device import i2c_device
 from micropython import const
 
+try:
+    from typing import Union, Optional
+    from circuitpython_typing import ReadableBuffer
+    from busio import I2C
+except ImportError:
+    pass
 
-__version__ = "2.2.8"
+__version__ = "2.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SCD30.git"
 SCD30_DEFAULT_ADDR = 0x61
 
 _CMD_CONTINUOUS_MEASUREMENT = const(0x0010)
 _CMD_SET_MEASUREMENT_INTERVAL = const(0x4600)
 _CMD_GET_DATA_READY = const(0x0202)
 _CMD_READ_MEASUREMENT = const(0x0300)
@@ -81,15 +87,17 @@
 
             temperature = scd.temperature
             relative_humidity = scd.relative_humidity
             co2_ppm_level = scd.CO2
 
     """
 
-    def __init__(self, i2c_bus, ambient_pressure=0, address=SCD30_DEFAULT_ADDR):
+    def __init__(
+        self, i2c_bus: I2C, ambient_pressure: int = 0, address: int = SCD30_DEFAULT_ADDR
+    ) -> None:
         if ambient_pressure != 0:
             if ambient_pressure < 700 or ambient_pressure > 1400:
                 raise AttributeError("`ambient_pressure` must be from 700-1400 mBar")
 
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
         self._buffer = bytearray(18)
         self._crc_buffer = bytearray(2)
@@ -100,38 +108,38 @@
         self.ambient_pressure = ambient_pressure
 
         # cached readings
         self._temperature = None
         self._relative_humidity = None
         self._co2 = None
 
-    def reset(self):
+    def reset(self) -> None:
         """Perform a soft reset on the sensor, restoring default values"""
         self._send_command(_CMD_SOFT_RESET)
         time.sleep(0.1)  # not mentioned by datasheet, but required to avoid IO error
 
     @property
-    def measurement_interval(self):
+    def measurement_interval(self) -> int:
         """Sets the interval between readings in seconds. The interval value must be from 2-1800
 
         .. note::
             This value will be saved and will not be reset on boot or by calling `reset`.
 
         """
 
         return self._read_register(_CMD_SET_MEASUREMENT_INTERVAL)
 
     @measurement_interval.setter
-    def measurement_interval(self, value):
+    def measurement_interval(self, value: int) -> None:
         if value < 2 or value > 1800:
             raise AttributeError("measurement_interval must be from 2-1800 seconds")
         self._send_command(_CMD_SET_MEASUREMENT_INTERVAL, value)
 
     @property
-    def self_calibration_enabled(self):
+    def self_calibration_enabled(self) -> bool:
         """Enables or disables automatic self calibration (ASC). To work correctly, the sensor must
         be on and active for 7 days after enabling ASC, and exposed to fresh air for at least 1 hour
         per day. Consult the manufacturer's documentation for more information.
 
         .. note::
             Enabling self calibration will override any values set by specifying a
             `forced_recalibration_reference`
@@ -140,131 +148,131 @@
             This value will be saved and will not be reset on boot or by calling `reset`.
 
         """
 
         return self._read_register(_CMD_AUTOMATIC_SELF_CALIBRATION) == 1
 
     @self_calibration_enabled.setter
-    def self_calibration_enabled(self, enabled):
+    def self_calibration_enabled(self, enabled: bool) -> None:
         self._send_command(_CMD_AUTOMATIC_SELF_CALIBRATION, enabled)
         if enabled:
             time.sleep(0.01)
 
     @property
-    def data_available(self):
+    def data_available(self) -> bool:
         """Check the sensor to see if new data is available"""
         return self._read_register(_CMD_GET_DATA_READY)
 
     @property
-    def ambient_pressure(self):
+    def ambient_pressure(self) -> int:
         """Specifies the ambient air pressure at the measurement location in mBar. Setting this
         value adjusts the CO2 measurement calculations to account for the air pressure's effect on
         readings. Values must be in mBar, from 700 to 1400 mBar"""
         return self._read_register(_CMD_CONTINUOUS_MEASUREMENT)
 
     @ambient_pressure.setter
-    def ambient_pressure(self, pressure_mbar):
+    def ambient_pressure(self, pressure_mbar: int) -> None:
         pressure_mbar = int(pressure_mbar)
         if pressure_mbar != 0 and (pressure_mbar > 1400 or pressure_mbar < 700):
             raise AttributeError("ambient_pressure must be from 700 to 1400 mBar")
         self._send_command(_CMD_CONTINUOUS_MEASUREMENT, pressure_mbar)
 
     @property
-    def altitude(self):
+    def altitude(self) -> int:
         """Specifies the altitude at the measurement location in meters above sea level. Setting
         this value adjusts the CO2 measurement calculations to account for the air pressure's effect
         on readings.
 
         .. note::
             This value will be saved and will not be reset on boot or by calling `reset`.
 
 
         """
         return self._read_register(_CMD_SET_ALTITUDE_COMPENSATION)
 
     @altitude.setter
-    def altitude(self, altitude):
+    def altitude(self, altitude: int) -> None:
         self._send_command(_CMD_SET_ALTITUDE_COMPENSATION, int(altitude))
 
     @property
-    def temperature_offset(self):
+    def temperature_offset(self) -> float:
         """Specifies the offset to be added to the reported measurements to account for a bias in
         the measured signal. Value is in degrees Celsius with a resolution of 0.01 degrees and a
         maximum value of 655.35 C
 
         .. note::
             This value will be saved and will not be reset on boot or by calling `reset`.
 
         """
 
         raw_offset = self._read_register(_CMD_SET_TEMPERATURE_OFFSET)
         return raw_offset / 100.0
 
     @temperature_offset.setter
-    def temperature_offset(self, offset):
+    def temperature_offset(self, offset: Union[float, int]) -> None:
         if offset > 655.35:
             raise AttributeError(
                 "Offset value must be less than or equal to 655.35 degrees Celsius"
             )
 
         self._send_command(_CMD_SET_TEMPERATURE_OFFSET, int(offset * 100))
 
     @property
-    def forced_recalibration_reference(self):
+    def forced_recalibration_reference(self) -> int:
         """Specifies the concentration of a reference source of CO2 placed in close proximity to the
         sensor. The value must be from 400 to 2000 ppm.
 
         .. note::
             Specifying a forced recalibration reference will override any calibration values
             set by Automatic Self Calibration
 
         """
         return self._read_register(_CMD_SET_FORCED_RECALIBRATION_FACTOR)
 
     @forced_recalibration_reference.setter
-    def forced_recalibration_reference(self, reference_value):
+    def forced_recalibration_reference(self, reference_value: int) -> None:
         self._send_command(_CMD_SET_FORCED_RECALIBRATION_FACTOR, reference_value)
 
     @property
-    def CO2(self):  # pylint:disable=invalid-name
+    def CO2(self) -> float:  # pylint:disable=invalid-name
         """Returns the CO2 concentration in PPM (parts per million)
 
         .. note::
             Between measurements, the most recent reading will be cached and returned.
 
         """
         if self.data_available:
             self._read_data()
         return self._co2
 
     @property
-    def temperature(self):
+    def temperature(self) -> float:
         """Returns the current temperature in degrees Celsius
 
         .. note::
             Between measurements, the most recent reading will be cached and returned.
 
         """
         if self.data_available:
             self._read_data()
         return self._temperature
 
     @property
-    def relative_humidity(self):
+    def relative_humidity(self) -> float:
         """Returns the current relative humidity in %rH.
 
         .. note::
             Between measurements, the most recent reading will be cached and returned.
 
         """
         if self.data_available:
             self._read_data()
         return self._relative_humidity
 
-    def _send_command(self, command, arguments=None):
+    def _send_command(self, command: int, arguments: Optional[int] = None) -> None:
         # if there is an argument, calculate the CRC and include it as well.
         if arguments is not None:
             self._crc_buffer[0] = arguments >> 8
             self._crc_buffer[1] = arguments & 0xFF
             self._buffer[2] = arguments >> 8
             self._buffer[3] = arguments & 0xFF
             crc = self._crc8(self._crc_buffer)
@@ -276,28 +284,28 @@
         self._buffer[0] = command >> 8
         self._buffer[1] = command & 0xFF
 
         with self.i2c_device as i2c:
             i2c.write(self._buffer, end=end_byte)
         time.sleep(0.05)  # 3ms min delay
 
-    def _read_register(self, reg_addr):
+    def _read_register(self, reg_addr: int) -> int:
         self._buffer[0] = reg_addr >> 8
         self._buffer[1] = reg_addr & 0xFF
         with self.i2c_device as i2c:
             i2c.write(self._buffer, end=2)
             # separate readinto because the SCD30 wants an i2c stop before the read
             # (non-repeated start)
             time.sleep(0.005)  # min 3 ms delay
             i2c.readinto(self._buffer, end=3)
         if not self._check_crc(self._buffer[:2], self._buffer[2]):
             raise RuntimeError("CRC check failed while reading data")
         return unpack_from(">H", self._buffer[0:2])[0]
 
-    def _read_data(self):
+    def _read_data(self) -> None:
         self._send_command(_CMD_READ_MEASUREMENT)
         with self.i2c_device as i2c:
             i2c.readinto(self._buffer)
 
         crcs_good = True
 
         for i in range(0, 18, 3):
@@ -310,19 +318,19 @@
 
         self._co2 = unpack(">f", self._buffer[0:2] + self._buffer[3:5])[0]
         self._temperature = unpack(">f", self._buffer[6:8] + self._buffer[9:11])[0]
         self._relative_humidity = unpack(
             ">f", self._buffer[12:14] + self._buffer[15:17]
         )[0]
 
-    def _check_crc(self, data_bytes, crc):
+    def _check_crc(self, data_bytes: ReadableBuffer, crc: int) -> bool:
         return crc == self._crc8(bytearray(data_bytes))
 
     @staticmethod
-    def _crc8(buffer):
+    def _crc8(buffer: bytearray) -> int:
         crc = 0xFF
         for byte in buffer:
             crc ^= byte
             for _ in range(8):
                 if crc & 0x80:
                     crc = (crc << 1) ^ 0x31
                 else:
```

### Comparing `adafruit-circuitpython-scd30-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-scd30-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/docs/conf.py` & `adafruit-circuitpython-scd30-2.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/docs/examples.rst` & `adafruit-circuitpython-scd30-2.2.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/docs/index.rst` & `adafruit-circuitpython-scd30-2.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/examples/scd30_ft232htest.py` & `adafruit-circuitpython-scd30-2.2.9/examples/scd30_ft232htest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/examples/scd30_mcp2221test.py` & `adafruit-circuitpython-scd30-2.2.9/examples/scd30_mcp2221test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/examples/scd30_simpletest.py` & `adafruit-circuitpython-scd30-2.2.9/examples/scd30_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/examples/scd30_tuning_knobs.py` & `adafruit-circuitpython-scd30-2.2.9/examples/scd30_tuning_knobs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd30-2.2.8/pyproject.toml` & `adafruit-circuitpython-scd30-2.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-scd30"
 description = "Helper library for the SCD30 CO2 sensor"
-version = "2.2.8"
+version = "2.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SCD30"}
 keywords = [
     "adafruit",
```

