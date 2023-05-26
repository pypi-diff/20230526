# Comparing `tmp/adafruit-circuitpython-ble-eddystone-1.10.14.tar.gz` & `tmp/adafruit-circuitpython-ble-eddystone-1.10.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-eddystone-1.10.14.tar", last modified: Thu May 11 18:27:29 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-eddystone-1.10.15.tar", last modified: Fri May 26 16:22:57 2023, max compression
```

## Comparing `adafruit-circuitpython-ble-eddystone-1.10.14.tar` & `adafruit-circuitpython-ble-eddystone-1.10.15.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.020913 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/uid.py
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-11 18:27:29.000000 adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5705 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/examples/ble_eddystone_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-11 18:27:21.000000 adafruit-circuitpython-ble-eddystone-1.10.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-11 18:27:12.000000 adafruit-circuitpython-ble-eddystone-1.10.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:27:29.024913 adafruit-circuitpython-ble-eddystone-1.10.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.336492 adafruit-circuitpython-ble-eddystone-1.10.15/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.328492 adafruit-circuitpython-ble-eddystone-1.10.15/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.332492 adafruit-circuitpython-ble-eddystone-1.10.15/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.332492 adafruit-circuitpython-ble-eddystone-1.10.15/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.332492 adafruit-circuitpython-ble-eddystone-1.10.15/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-26 16:22:57.336492 adafruit-circuitpython-ble-eddystone-1.10.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3274 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.332492 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_ble_eddystone/
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-05-26 16:22:49.000000 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_ble_eddystone/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-26 16:22:49.000000 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_ble_eddystone/uid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-26 16:22:49.000000 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_ble_eddystone/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.332492 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_circuitpython_ble_eddystone.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4064 2023-05-26 16:22:57.000000 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_circuitpython_ble_eddystone.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-26 16:22:57.000000 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_circuitpython_ble_eddystone.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:22:57.000000 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_circuitpython_ble_eddystone.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 16:22:57.000000 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_circuitpython_ble_eddystone.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 16:22:57.000000 adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_circuitpython_ble_eddystone.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.336492 adafruit-circuitpython-ble-eddystone-1.10.15/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.336492 adafruit-circuitpython-ble-eddystone-1.10.15/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5733 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:57.336492 adafruit-circuitpython-ble-eddystone-1.10.15/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-26 16:22:49.000000 adafruit-circuitpython-ble-eddystone-1.10.15/examples/ble_eddystone_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-26 16:22:49.000000 adafruit-circuitpython-ble-eddystone-1.10.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-26 16:22:37.000000 adafruit-circuitpython-ble-eddystone-1.10.15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:22:57.336492 adafruit-circuitpython-ble-eddystone-1.10.15/setup.cfg
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-eddystone-1.10.15/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/.gitignore` & `adafruit-circuitpython-ble-eddystone-1.10.15/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-eddystone-1.10.15/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/.pylintrc` & `adafruit-circuitpython-ble-eddystone-1.10.15/.pylintrc`

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

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-eddystone-1.10.15/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/LICENSE` & `adafruit-circuitpython-ble-eddystone-1.10.15/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-eddystone-1.10.15/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-eddystone-1.10.15/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-eddystone-1.10.15/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/PKG-INFO` & `adafruit-circuitpython-ble-eddystone-1.10.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-eddystone
-Version: 1.10.14
+Version: 1.10.15
 Summary: CircuitPython BLE library for Google's open 'physical web' Eddystone.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone
 Keywords: adafruit,blinka,circuitpython,micropython,ble_eddystone,eddystone,ble
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/README.rst` & `adafruit-circuitpython-ble-eddystone-1.10.15/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/__init__.py` & `adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_ble_eddystone/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 import struct
 
 from adafruit_ble.advertising import Advertisement
 from adafruit_ble.advertising.standard import ServiceList, ServiceData
 from adafruit_ble.uuid import StandardUUID
 
-__version__ = "1.10.14"
+__version__ = "1.10.15"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone.git"
 
 
 class _EddystoneService:
     """Placeholder service. Not implemented."""
 
     # pylint: disable=too-few-public-methods
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/uid.py` & `adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_ble_eddystone/uid.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Static Eddystone UID advertisement. Documented by Google here:
 https://github.com/google/eddystone/tree/master/eddystone-uid
 
 """
 
 from . import EddystoneAdvertisement, EddystoneFrameStruct, EddystoneFrameBytes
 
-__version__ = "1.10.14"
+__version__ = "1.10.15"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone.git"
 
 
 class EddystoneUID(EddystoneAdvertisement):  # pylint: disable=too-few-public-methods
     """Static Eddystone unique identifier.
 
     :param bytes instance_id: instance component of the id. 10 bytes long
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_ble_eddystone/url.py` & `adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_ble_eddystone/url.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 Eddystone URL advertisement. Documented by Google here:
 https://github.com/google/eddystone/tree/master/eddystone-url
 
 """
 
 from . import EddystoneAdvertisement, EddystoneFrameStruct, EddystoneFrameBytes
 
-__version__ = "1.10.14"
+__version__ = "1.10.15"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone.git"
 
 # These prefixes are replaced with a single one-byte scheme number.
 _URL_SCHEMES = (b"http://www.", b"https://www.", b"http://", b"https://")
 
 # These common domains are replaced with a single non-printing byte.
 # Byte value is 0-6 for these with a '/' suffix.
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_circuitpython_ble_eddystone.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-eddystone
-Version: 1.10.14
+Version: 1.10.15
 Summary: CircuitPython BLE library for Google's open 'physical web' Eddystone.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone
 Keywords: adafruit,blinka,circuitpython,micropython,ble_eddystone,eddystone,ble
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/adafruit_circuitpython_ble_eddystone.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-eddystone-1.10.15/adafruit_circuitpython_ble_eddystone.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-eddystone-1.10.15/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/docs/conf.py` & `adafruit-circuitpython-ble-eddystone-1.10.15/docs/conf.py`

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
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/docs/index.rst` & `adafruit-circuitpython-ble-eddystone-1.10.15/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/examples/ble_eddystone_simpletest.py` & `adafruit-circuitpython-ble-eddystone-1.10.15/examples/ble_eddystone_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-eddystone-1.10.14/pyproject.toml` & `adafruit-circuitpython-ble-eddystone-1.10.15/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ble-eddystone"
 description = "CircuitPython BLE library for Google's open 'physical web' Eddystone."
-version = "1.10.14"
+version = "1.10.15"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Eddystone"}
 keywords = [
     "adafruit",
```

