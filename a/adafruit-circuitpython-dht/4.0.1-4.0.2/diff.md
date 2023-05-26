# Comparing `tmp/adafruit-circuitpython-dht-4.0.1.tar.gz` & `tmp/adafruit-circuitpython-dht-4.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-dht-4.0.1.tar", last modified: Tue May 16 15:50:06 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-dht-4.0.2.tar", last modified: Fri May 26 16:18:39 2023, max compression
```

## Comparing `adafruit-circuitpython-dht-4.0.1.tar` & `adafruit-circuitpython-dht-4.0.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.895501 adafruit-circuitpython-dht-4.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.891501 adafruit-circuitpython-dht-4.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.891501 adafruit-circuitpython-dht-4.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.891501 adafruit-circuitpython-dht-4.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.895501 adafruit-circuitpython-dht-4.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-16 15:50:06.895501 adafruit-circuitpython-dht-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.895501 adafruit-circuitpython-dht-4.0.1/adafruit_circuitpython_dht.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-16 15:50:06.000000 adafruit-circuitpython-dht-4.0.1/adafruit_circuitpython_dht.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-16 15:50:06.000000 adafruit-circuitpython-dht-4.0.1/adafruit_circuitpython_dht.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 15:50:06.000000 adafruit-circuitpython-dht-4.0.1/adafruit_circuitpython_dht.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 15:50:06.000000 adafruit-circuitpython-dht-4.0.1/adafruit_circuitpython_dht.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 15:50:06.000000 adafruit-circuitpython-dht-4.0.1/adafruit_circuitpython_dht.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-16 15:49:58.000000 adafruit-circuitpython-dht-4.0.1/adafruit_dht.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.895501 adafruit-circuitpython-dht-4.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.895501 adafruit-circuitpython-dht-4.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 15:50:06.895501 adafruit-circuitpython-dht-4.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-16 15:49:58.000000 adafruit-circuitpython-dht-4.0.1/examples/dht_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-16 15:49:58.000000 adafruit-circuitpython-dht-4.0.1/examples/dht_time_calibration_advance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-16 15:49:58.000000 adafruit-circuitpython-dht-4.0.1/examples/dht_to_led_display.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 15:49:58.000000 adafruit-circuitpython-dht-4.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 15:49:48.000000 adafruit-circuitpython-dht-4.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 15:50:06.895501 adafruit-circuitpython-dht-4.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.114633 adafruit-circuitpython-dht-4.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/adafruit_circuitpython_dht.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5625 2023-05-26 16:18:39.000000 adafruit-circuitpython-dht-4.0.2/adafruit_circuitpython_dht.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-26 16:18:39.000000 adafruit-circuitpython-dht-4.0.2/adafruit_circuitpython_dht.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:18:39.000000 adafruit-circuitpython-dht-4.0.2/adafruit_circuitpython_dht.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:18:39.000000 adafruit-circuitpython-dht-4.0.2/adafruit_circuitpython_dht.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 16:18:39.000000 adafruit-circuitpython-dht-4.0.2/adafruit_circuitpython_dht.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11693 2023-05-26 16:18:31.000000 adafruit-circuitpython-dht-4.0.2/adafruit_dht.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-26 16:18:31.000000 adafruit-circuitpython-dht-4.0.2/examples/dht_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-26 16:18:31.000000 adafruit-circuitpython-dht-4.0.2/examples/dht_time_calibration_advance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-26 16:18:31.000000 adafruit-circuitpython-dht-4.0.2/examples/dht_to_led_display.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:18:31.000000 adafruit-circuitpython-dht-4.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:18:22.000000 adafruit-circuitpython-dht-4.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:18:39.118633 adafruit-circuitpython-dht-4.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-dht-4.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-dht-4.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/.gitignore` & `adafruit-circuitpython-dht-4.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-dht-4.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/.pylintrc` & `adafruit-circuitpython-dht-4.0.2/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -392,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-dht-4.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-dht-4.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/LICENSE` & `adafruit-circuitpython-dht-4.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-dht-4.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-dht-4.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-dht-4.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/PKG-INFO` & `adafruit-circuitpython-dht-4.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dht
-Version: 4.0.1
+Version: 4.0.2
 Summary: CircuitPython support for DHT11 and DHT22 type temperature/humidity devices
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DHT
 Keywords: adafruit,dht,hardware,sensors,temperature,humidity,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dht-4.0.1/README.rst` & `adafruit-circuitpython-dht-4.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/adafruit_circuitpython_dht.egg-info/PKG-INFO` & `adafruit-circuitpython-dht-4.0.2/adafruit_circuitpython_dht.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dht
-Version: 4.0.1
+Version: 4.0.2
 Summary: CircuitPython support for DHT11 and DHT22 type temperature/humidity devices
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DHT
 Keywords: adafruit,dht,hardware,sensors,temperature,humidity,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dht-4.0.1/adafruit_circuitpython_dht.egg-info/SOURCES.txt` & `adafruit-circuitpython-dht-4.0.2/adafruit_circuitpython_dht.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/adafruit_dht.py` & `adafruit-circuitpython-dht-4.0.2/adafruit_dht.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 try:
     # Used only for typing
     from typing import Union
     from microcontroller import Pin
 except ImportError:
     pass
 
-__version__ = "4.0.1"
+__version__ = "4.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DHT.git"
 
 
 class DHTBase:
     """base support for DHT11 and DHT22 devices
 
     :param bool dht11: True if device is DHT11, otherwise DHT22.
```

### Comparing `adafruit-circuitpython-dht-4.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-dht-4.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/docs/conf.py` & `adafruit-circuitpython-dht-4.0.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
 ]
 
 autodoc_mock_imports = ["pulseio"]
 
 intersphinx_mapping = {
```

### Comparing `adafruit-circuitpython-dht-4.0.1/docs/examples.rst` & `adafruit-circuitpython-dht-4.0.2/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/docs/index.rst` & `adafruit-circuitpython-dht-4.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/examples/dht_simpletest.py` & `adafruit-circuitpython-dht-4.0.2/examples/dht_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/examples/dht_time_calibration_advance.py` & `adafruit-circuitpython-dht-4.0.2/examples/dht_time_calibration_advance.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/examples/dht_to_led_display.py` & `adafruit-circuitpython-dht-4.0.2/examples/dht_to_led_display.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dht-4.0.1/pyproject.toml` & `adafruit-circuitpython-dht-4.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-dht"
 description = "CircuitPython support for DHT11 and DHT22 type temperature/humidity devices"
-version = "4.0.1"
+version = "4.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DHT"}
 keywords = [
     "adafruit",
```

