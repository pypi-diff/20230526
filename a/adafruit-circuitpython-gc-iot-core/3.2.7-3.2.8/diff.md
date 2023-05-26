# Comparing `tmp/adafruit-circuitpython-gc-iot-core-3.2.7.tar.gz` & `tmp/adafruit-circuitpython-gc-iot-core-3.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-gc-iot-core-3.2.7.tar", last modified: Tue May 16 17:54:59 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-gc-iot-core-3.2.8.tar", last modified: Fri May 26 16:10:17 2023, max compression
```

## Comparing `adafruit-circuitpython-gc-iot-core-3.2.7.tar` & `adafruit-circuitpython-gc-iot-core-3.2.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.187920 adafruit-circuitpython-gc-iot-core-3.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.183920 adafruit-circuitpython-gc-iot-core-3.2.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.183920 adafruit-circuitpython-gc-iot-core-3.2.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.183920 adafruit-circuitpython-gc-iot-core-3.2.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.183920 adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/Apache-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-16 17:54:59.187920 adafruit-circuitpython-gc-iot-core-3.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.187920 adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_circuitpython_gc_iot_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-16 17:54:59.000000 adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_circuitpython_gc_iot_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-16 17:54:59.000000 adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_circuitpython_gc_iot_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:54:59.000000 adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_circuitpython_gc_iot_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-16 17:54:59.000000 adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_circuitpython_gc_iot_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-16 17:54:59.000000 adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_circuitpython_gc_iot_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-05-16 17:54:52.000000 adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_gc_iot_core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.187920 adafruit-circuitpython-gc-iot-core-3.2.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.187920 adafruit-circuitpython-gc-iot-core-3.2.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:59.187920 adafruit-circuitpython-gc-iot-core-3.2.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-16 17:54:52.000000 adafruit-circuitpython-gc-iot-core-3.2.7/examples/gc_iot_core_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-16 17:54:52.000000 adafruit-circuitpython-gc-iot-core-3.2.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-16 17:54:42.000000 adafruit-circuitpython-gc-iot-core-3.2.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:54:59.187920 adafruit-circuitpython-gc-iot-core-3.2.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.953078 adafruit-circuitpython-gc-iot-core-3.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.949078 adafruit-circuitpython-gc-iot-core-3.2.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.949078 adafruit-circuitpython-gc-iot-core-3.2.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.949078 adafruit-circuitpython-gc-iot-core-3.2.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.953078 adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/Apache-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-26 16:10:17.953078 adafruit-circuitpython-gc-iot-core-3.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.953078 adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_circuitpython_gc_iot_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3923 2023-05-26 16:10:17.000000 adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_circuitpython_gc_iot_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-26 16:10:17.000000 adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_circuitpython_gc_iot_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:10:17.000000 adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_circuitpython_gc_iot_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-26 16:10:17.000000 adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_circuitpython_gc_iot_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 16:10:17.000000 adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_circuitpython_gc_iot_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16048 2023-05-26 16:10:10.000000 adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_gc_iot_core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.953078 adafruit-circuitpython-gc-iot-core-3.2.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.953078 adafruit-circuitpython-gc-iot-core-3.2.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:10:17.953078 adafruit-circuitpython-gc-iot-core-3.2.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-05-26 16:10:10.000000 adafruit-circuitpython-gc-iot-core-3.2.8/examples/gc_iot_core_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-26 16:10:10.000000 adafruit-circuitpython-gc-iot-core-3.2.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-26 16:09:56.000000 adafruit-circuitpython-gc-iot-core-3.2.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:10:17.953078 adafruit-circuitpython-gc-iot-core-3.2.8/setup.cfg
```

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-gc-iot-core-3.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/.gitignore` & `adafruit-circuitpython-gc-iot-core-3.2.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/.pre-commit-config.yaml` & `adafruit-circuitpython-gc-iot-core-3.2.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/.pylintrc` & `adafruit-circuitpython-gc-iot-core-3.2.8/.pylintrc`

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

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-gc-iot-core-3.2.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/LICENSE` & `adafruit-circuitpython-gc-iot-core-3.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/Apache-2.0.txt` & `adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/Apache-2.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/MIT.txt` & `adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-gc-iot-core-3.2.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/PKG-INFO` & `adafruit-circuitpython-gc-iot-core-3.2.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-gc-iot-core
-Version: 3.2.7
+Version: 3.2.8
 Summary: Google Cloud IoT Core Client for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_GC_IOT_CORE
 Keywords: adafruit,blinka,circuitpython,micropython,gc_iot_core,gcs,,google,cloud,platform,,cloud,,iot,,core
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/README.rst` & `adafruit-circuitpython-gc-iot-core-3.2.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_circuitpython_gc_iot_core.egg-info/PKG-INFO` & `adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_circuitpython_gc_iot_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-gc-iot-core
-Version: 3.2.7
+Version: 3.2.8
 Summary: Google Cloud IoT Core Client for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_GC_IOT_CORE
 Keywords: adafruit,blinka,circuitpython,micropython,gc_iot_core,gcs,,google,cloud,platform,,cloud,,iot,,core
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_circuitpython_gc_iot_core.egg-info/SOURCES.txt` & `adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_circuitpython_gc_iot_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/adafruit_gc_iot_core.py` & `adafruit-circuitpython-gc-iot-core-3.2.8/adafruit_gc_iot_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 except ImportError:
     pass
 
 import adafruit_logging as logging
 from adafruit_jwt import JWT
 import rtc
 
-__version__ = "3.2.7"
+__version__ = "3.2.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_GC_IOT_Core.git"
 
 
 class MQTT_API_ERROR(Exception):
     """Exception raised on MQTT API return-code errors."""
 
     # pylint: disable=unnecessary-pass
```

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/docs/_static/favicon.ico` & `adafruit-circuitpython-gc-iot-core-3.2.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/docs/conf.py` & `adafruit-circuitpython-gc-iot-core-3.2.8/docs/conf.py`

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
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
```

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/docs/index.rst` & `adafruit-circuitpython-gc-iot-core-3.2.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/examples/gc_iot_core_simpletest.py` & `adafruit-circuitpython-gc-iot-core-3.2.8/examples/gc_iot_core_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gc-iot-core-3.2.7/pyproject.toml` & `adafruit-circuitpython-gc-iot-core-3.2.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-gc-iot-core"
 description = "Google Cloud IoT Core Client for CircuitPython"
-version = "3.2.7"
+version = "3.2.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_GC_IOT_CORE"}
 keywords = [
     "adafruit",
```

