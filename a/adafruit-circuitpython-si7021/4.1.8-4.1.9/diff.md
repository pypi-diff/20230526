# Comparing `tmp/adafruit-circuitpython-si7021-4.1.8.tar.gz` & `tmp/adafruit-circuitpython-si7021-4.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-si7021-4.1.8.tar", last modified: Thu May 18 15:41:38 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-si7021-4.1.9.tar", last modified: Fri May 26 16:17:55 2023, max compression
```

## Comparing `adafruit-circuitpython-si7021-4.1.8.tar` & `adafruit-circuitpython-si7021-4.1.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.572077 adafruit-circuitpython-si7021-4.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.564077 adafruit-circuitpython-si7021-4.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.568077 adafruit-circuitpython-si7021-4.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.568077 adafruit-circuitpython-si7021-4.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.568077 adafruit-circuitpython-si7021-4.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-18 15:41:38.572077 adafruit-circuitpython-si7021-4.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.568077 adafruit-circuitpython-si7021-4.1.8/adafruit_circuitpython_si7021.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-18 15:41:38.000000 adafruit-circuitpython-si7021-4.1.8/adafruit_circuitpython_si7021.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-18 15:41:38.000000 adafruit-circuitpython-si7021-4.1.8/adafruit_circuitpython_si7021.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:41:38.000000 adafruit-circuitpython-si7021-4.1.8/adafruit_circuitpython_si7021.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 15:41:38.000000 adafruit-circuitpython-si7021-4.1.8/adafruit_circuitpython_si7021.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:41:38.000000 adafruit-circuitpython-si7021-4.1.8/adafruit_circuitpython_si7021.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.568077 adafruit-circuitpython-si7021-4.1.8/adafruit_si7021/
--rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-05-18 15:41:31.000000 adafruit-circuitpython-si7021-4.1.8/adafruit_si7021/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-18 15:41:31.000000 adafruit-circuitpython-si7021-4.1.8/adafruit_si7021/i2c_bits.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.568077 adafruit-circuitpython-si7021-4.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.568077 adafruit-circuitpython-si7021-4.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:38.568077 adafruit-circuitpython-si7021-4.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-18 15:41:31.000000 adafruit-circuitpython-si7021-4.1.8/examples/si7021_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-18 15:41:31.000000 adafruit-circuitpython-si7021-4.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-18 15:41:22.000000 adafruit-circuitpython-si7021-4.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:41:38.572077 adafruit-circuitpython-si7021-4.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.470894 adafruit-circuitpython-si7021-4.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.470894 adafruit-circuitpython-si7021-4.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/adafruit_circuitpython_si7021.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4100 2023-05-26 16:17:55.000000 adafruit-circuitpython-si7021-4.1.9/adafruit_circuitpython_si7021.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-26 16:17:55.000000 adafruit-circuitpython-si7021-4.1.9/adafruit_circuitpython_si7021.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:17:55.000000 adafruit-circuitpython-si7021-4.1.9/adafruit_circuitpython_si7021.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:17:55.000000 adafruit-circuitpython-si7021-4.1.9/adafruit_circuitpython_si7021.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:17:55.000000 adafruit-circuitpython-si7021-4.1.9/adafruit_circuitpython_si7021.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/adafruit_si7021/
+-rw-r--r--   0 runner    (1001) docker     (123)     9760 2023-05-26 16:17:48.000000 adafruit-circuitpython-si7021-4.1.9/adafruit_si7021/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4471 2023-05-26 16:17:48.000000 adafruit-circuitpython-si7021-4.1.9/adafruit_si7021/i2c_bits.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5749 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-26 16:17:48.000000 adafruit-circuitpython-si7021-4.1.9/examples/si7021_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-05-26 16:17:48.000000 adafruit-circuitpython-si7021-4.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:17:38.000000 adafruit-circuitpython-si7021-4.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:17:55.474894 adafruit-circuitpython-si7021-4.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-si7021-4.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-si7021-4.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/.gitignore` & `adafruit-circuitpython-si7021-4.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-si7021-4.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/.pylintrc` & `adafruit-circuitpython-si7021-4.1.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-si7021-4.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-si7021-4.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/LICENSE` & `adafruit-circuitpython-si7021-4.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-si7021-4.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-si7021-4.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-si7021-4.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/PKG-INFO` & `adafruit-circuitpython-si7021-4.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si7021
-Version: 4.1.8
+Version: 4.1.9
 Summary: CircuitPython library for SI7021 Temperature and Humidity Sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI7021
 Keywords: adafruit,si7021,temperature,humidity,sensorbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si7021-4.1.8/README.rst` & `adafruit-circuitpython-si7021-4.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/adafruit_circuitpython_si7021.egg-info/PKG-INFO` & `adafruit-circuitpython-si7021-4.1.9/adafruit_circuitpython_si7021.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si7021
-Version: 4.1.8
+Version: 4.1.9
 Summary: CircuitPython library for SI7021 Temperature and Humidity Sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI7021
 Keywords: adafruit,si7021,temperature,humidity,sensorbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si7021-4.1.8/adafruit_circuitpython_si7021.egg-info/SOURCES.txt` & `adafruit-circuitpython-si7021-4.1.9/adafruit_circuitpython_si7021.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/adafruit_si7021/__init__.py` & `adafruit-circuitpython-si7021-4.1.9/adafruit_si7021/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     from typing import Optional, Tuple
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "4.1.8"
+__version__ = "4.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SI7021.git"
 
 HUMIDITY = const(0xF5)
 TEMPERATURE = const(0xF3)
 WRITE_HEATER_LEVEL = const(0x51)
 READ_HEATER_LEVEL = const(0x11)
 WRITE_HEATER_ENABLE = const(0xE6)
```

### Comparing `adafruit-circuitpython-si7021-4.1.8/adafruit_si7021/i2c_bits.py` & `adafruit-circuitpython-si7021-4.1.9/adafruit_si7021/i2c_bits.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-si7021-4.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/docs/conf.py` & `adafruit-circuitpython-si7021-4.1.9/docs/conf.py`

 * *Files 1% similar despite different names*

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
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
```

### Comparing `adafruit-circuitpython-si7021-4.1.8/docs/index.rst` & `adafruit-circuitpython-si7021-4.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/examples/si7021_simpletest.py` & `adafruit-circuitpython-si7021-4.1.9/examples/si7021_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si7021-4.1.8/pyproject.toml` & `adafruit-circuitpython-si7021-4.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-si7021"
 description = "CircuitPython library for SI7021 Temperature and Humidity Sensor."
-version = "4.1.8"
+version = "4.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SI7021"}
 keywords = [
     "adafruit",
```

