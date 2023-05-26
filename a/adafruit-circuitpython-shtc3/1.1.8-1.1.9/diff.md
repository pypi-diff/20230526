# Comparing `tmp/adafruit-circuitpython-shtc3-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-shtc3-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-shtc3-1.1.8.tar", last modified: Mon Aug 22 18:47:32 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-shtc3-1.1.9.tar", last modified: Fri Aug 26 02:24:32 2022, max compression
```

## Comparing `adafruit-circuitpython-shtc3-1.1.8.tar` & `adafruit-circuitpython-shtc3-1.1.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.376518 adafruit-circuitpython-shtc3-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.376518 adafruit-circuitpython-shtc3-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/adafruit_circuitpython_shtc3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-08-22 18:47:32.000000 adafruit-circuitpython-shtc3-1.1.8/adafruit_circuitpython_shtc3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-22 18:47:32.000000 adafruit-circuitpython-shtc3-1.1.8/adafruit_circuitpython_shtc3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:47:32.000000 adafruit-circuitpython-shtc3-1.1.8/adafruit_circuitpython_shtc3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-22 18:47:32.000000 adafruit-circuitpython-shtc3-1.1.8/adafruit_circuitpython_shtc3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-22 18:47:32.000000 adafruit-circuitpython-shtc3-1.1.8/adafruit_circuitpython_shtc3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7880 2022-08-22 18:47:23.000000 adafruit-circuitpython-shtc3-1.1.8/adafruit_shtc3.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5653 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)      445 2022-08-22 18:47:23.000000 adafruit-circuitpython-shtc3-1.1.8/examples/shtc3_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-22 18:47:23.000000 adafruit-circuitpython-shtc3-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-22 18:47:15.000000 adafruit-circuitpython-shtc3-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:47:32.380518 adafruit-circuitpython-shtc3-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.052025 adafruit-circuitpython-shtc3-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.048025 adafruit-circuitpython-shtc3-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.048025 adafruit-circuitpython-shtc3-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.048025 adafruit-circuitpython-shtc3-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6140 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.052025 adafruit-circuitpython-shtc3-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-08-26 02:24:32.052025 adafruit-circuitpython-shtc3-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2995 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.052025 adafruit-circuitpython-shtc3-1.1.9/adafruit_circuitpython_shtc3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3784 2022-08-26 02:24:32.000000 adafruit-circuitpython-shtc3-1.1.9/adafruit_circuitpython_shtc3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      912 2022-08-26 02:24:32.000000 adafruit-circuitpython-shtc3-1.1.9/adafruit_circuitpython_shtc3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:24:32.000000 adafruit-circuitpython-shtc3-1.1.9/adafruit_circuitpython_shtc3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       93 2022-08-26 02:24:32.000000 adafruit-circuitpython-shtc3-1.1.9/adafruit_circuitpython_shtc3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2022-08-26 02:24:32.000000 adafruit-circuitpython-shtc3-1.1.9/adafruit_circuitpython_shtc3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7880 2022-08-26 02:24:22.000000 adafruit-circuitpython-shtc3-1.1.9/adafruit_shtc3.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.052025 adafruit-circuitpython-shtc3-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.052025 adafruit-circuitpython-shtc3-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5873 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:32.052025 adafruit-circuitpython-shtc3-1.1.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      445 2022-08-26 02:24:22.000000 adafruit-circuitpython-shtc3-1.1.9/examples/shtc3_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1248 2022-08-26 02:24:22.000000 adafruit-circuitpython-shtc3-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2022-08-26 02:24:12.000000 adafruit-circuitpython-shtc3-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:24:32.052025 adafruit-circuitpython-shtc3-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-shtc3-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-shtc3-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-shtc3-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-shtc3-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/.gitignore` & `adafruit-circuitpython-shtc3-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-shtc3-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/.pylintrc` & `adafruit-circuitpython-shtc3-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-shtc3-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/LICENSE` & `adafruit-circuitpython-shtc3-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-shtc3-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-shtc3-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-shtc3-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/PKG-INFO` & `adafruit-circuitpython-shtc3-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-shtc3
-Version: 1.1.8
+Version: 1.1.9
 Summary: A helper library for using the Senserion SHTC3 Humidity and Temperature Sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SHTC3
 Keywords: adafruit,blinka,circuitpython,micropython,shtc3,humidity,relative,temperature
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-shtc3-1.1.8/README.rst` & `adafruit-circuitpython-shtc3-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/adafruit_circuitpython_shtc3.egg-info/PKG-INFO` & `adafruit-circuitpython-shtc3-1.1.9/adafruit_circuitpython_shtc3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-shtc3
-Version: 1.1.8
+Version: 1.1.9
 Summary: A helper library for using the Senserion SHTC3 Humidity and Temperature Sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SHTC3
 Keywords: adafruit,blinka,circuitpython,micropython,shtc3,humidity,relative,temperature
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-shtc3-1.1.8/adafruit_circuitpython_shtc3.egg-info/SOURCES.txt` & `adafruit-circuitpython-shtc3-1.1.9/adafruit_circuitpython_shtc3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/adafruit_shtc3.py` & `adafruit-circuitpython-shtc3-1.1.9/adafruit_shtc3.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 * Adafruit's Register library:
   https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
 
 # imports
 
-__version__ = "1.1.8"
+__version__ = "1.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SHTC3.git"
 
 from struct import unpack_from
 import time
 from adafruit_bus_device import i2c_device
```

### Comparing `adafruit-circuitpython-shtc3-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-shtc3-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/docs/conf.py` & `adafruit-circuitpython-shtc3-1.1.9/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -47,15 +48,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit SHTC3 Library"
-copyright = "2020 Bryan Siepert"
+creation_year = "2020"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Bryan Siepert"
 author = "Bryan Siepert"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-shtc3-1.1.8/docs/index.rst` & `adafruit-circuitpython-shtc3-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-shtc3-1.1.8/pyproject.toml` & `adafruit-circuitpython-shtc3-1.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-shtc3"
 description = "A helper library for using the Senserion SHTC3 Humidity and Temperature Sensor"
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SHTC3"}
 keywords = [
     "adafruit",
```

