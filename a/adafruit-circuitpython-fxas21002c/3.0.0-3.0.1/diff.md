# Comparing `tmp/adafruit-circuitpython-fxas21002c-3.0.0.tar.gz` & `tmp/adafruit-circuitpython-fxas21002c-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-fxas21002c-3.0.0.tar", last modified: Thu May 11 14:41:23 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-fxas21002c-3.0.1.tar", last modified: Fri May 26 16:23:34 2023, max compression
```

## Comparing `adafruit-circuitpython-fxas21002c-3.0.0.tar` & `adafruit-circuitpython-fxas21002c-3.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:23.009912 adafruit-circuitpython-fxas21002c-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:22.997912 adafruit-circuitpython-fxas21002c-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:23.001912 adafruit-circuitpython-fxas21002c-3.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:23.001912 adafruit-circuitpython-fxas21002c-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:23.005912 adafruit-circuitpython-fxas21002c-3.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-11 14:41:23.005912 adafruit-circuitpython-fxas21002c-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:23.005912 adafruit-circuitpython-fxas21002c-3.0.0/adafruit_circuitpython_fxas21002c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-11 14:41:22.000000 adafruit-circuitpython-fxas21002c-3.0.0/adafruit_circuitpython_fxas21002c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-11 14:41:22.000000 adafruit-circuitpython-fxas21002c-3.0.0/adafruit_circuitpython_fxas21002c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:41:22.000000 adafruit-circuitpython-fxas21002c-3.0.0/adafruit_circuitpython_fxas21002c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-11 14:41:22.000000 adafruit-circuitpython-fxas21002c-3.0.0/adafruit_circuitpython_fxas21002c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-11 14:41:22.000000 adafruit-circuitpython-fxas21002c-3.0.0/adafruit_circuitpython_fxas21002c.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-11 14:41:12.000000 adafruit-circuitpython-fxas21002c-3.0.0/adafruit_fxas21002c.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:23.005912 adafruit-circuitpython-fxas21002c-3.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:23.005912 adafruit-circuitpython-fxas21002c-3.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5726 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:41:23.005912 adafruit-circuitpython-fxas21002c-3.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-11 14:41:12.000000 adafruit-circuitpython-fxas21002c-3.0.0/examples/fxas21002c_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-11 14:41:12.000000 adafruit-circuitpython-fxas21002c-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-11 14:40:55.000000 adafruit-circuitpython-fxas21002c-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:41:23.009912 adafruit-circuitpython-fxas21002c-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.164315 adafruit-circuitpython-fxas21002c-3.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.156314 adafruit-circuitpython-fxas21002c-3.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.160314 adafruit-circuitpython-fxas21002c-3.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.160314 adafruit-circuitpython-fxas21002c-3.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.160314 adafruit-circuitpython-fxas21002c-3.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-26 16:23:34.164315 adafruit-circuitpython-fxas21002c-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.160314 adafruit-circuitpython-fxas21002c-3.0.1/adafruit_circuitpython_fxas21002c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3732 2023-05-26 16:23:34.000000 adafruit-circuitpython-fxas21002c-3.0.1/adafruit_circuitpython_fxas21002c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-26 16:23:34.000000 adafruit-circuitpython-fxas21002c-3.0.1/adafruit_circuitpython_fxas21002c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:23:34.000000 adafruit-circuitpython-fxas21002c-3.0.1/adafruit_circuitpython_fxas21002c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 16:23:34.000000 adafruit-circuitpython-fxas21002c-3.0.1/adafruit_circuitpython_fxas21002c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:23:34.000000 adafruit-circuitpython-fxas21002c-3.0.1/adafruit_circuitpython_fxas21002c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7200 2023-05-26 16:23:24.000000 adafruit-circuitpython-fxas21002c-3.0.1/adafruit_fxas21002c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.164315 adafruit-circuitpython-fxas21002c-3.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.164315 adafruit-circuitpython-fxas21002c-3.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5754 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:34.164315 adafruit-circuitpython-fxas21002c-3.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-26 16:23:24.000000 adafruit-circuitpython-fxas21002c-3.0.1/examples/fxas21002c_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-26 16:23:24.000000 adafruit-circuitpython-fxas21002c-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 16:23:10.000000 adafruit-circuitpython-fxas21002c-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:23:34.164315 adafruit-circuitpython-fxas21002c-3.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-fxas21002c-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/.gitignore` & `adafruit-circuitpython-fxas21002c-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-fxas21002c-3.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/.pylintrc` & `adafruit-circuitpython-fxas21002c-3.0.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-fxas21002c-3.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/LICENSE` & `adafruit-circuitpython-fxas21002c-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-fxas21002c-3.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-fxas21002c-3.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-fxas21002c-3.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/PKG-INFO` & `adafruit-circuitpython-fxas21002c-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fxas21002c
-Version: 3.0.0
+Version: 3.0.1
 Summary: CircuitPython library for NXP FXAS21002C gyroscope.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FXAS21002C
 Keywords: adafruit,fxas21002c,gyro,gyroscope,nxp,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/README.rst` & `adafruit-circuitpython-fxas21002c-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/adafruit_circuitpython_fxas21002c.egg-info/PKG-INFO` & `adafruit-circuitpython-fxas21002c-3.0.1/adafruit_circuitpython_fxas21002c.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-fxas21002c
-Version: 3.0.0
+Version: 3.0.1
 Summary: CircuitPython library for NXP FXAS21002C gyroscope.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FXAS21002C
 Keywords: adafruit,fxas21002c,gyro,gyroscope,nxp,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/adafruit_circuitpython_fxas21002c.egg-info/SOURCES.txt` & `adafruit-circuitpython-fxas21002c-3.0.1/adafruit_circuitpython_fxas21002c.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/adafruit_fxas21002c.py` & `adafruit-circuitpython-fxas21002c-3.0.1/adafruit_fxas21002c.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     from typing import List, Tuple
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FXAS21002C.git"
 
 import adafruit_bus_device.i2c_device as i2c_dev
 from micropython import const
 
 
 # Internal constants and register values:
```

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-fxas21002c-3.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/docs/conf.py` & `adafruit-circuitpython-fxas21002c-3.0.1/docs/conf.py`

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
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
```

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/docs/index.rst` & `adafruit-circuitpython-fxas21002c-3.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/examples/fxas21002c_simpletest.py` & `adafruit-circuitpython-fxas21002c-3.0.1/examples/fxas21002c_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-fxas21002c-3.0.0/pyproject.toml` & `adafruit-circuitpython-fxas21002c-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-fxas21002c"
 description = "CircuitPython library for NXP FXAS21002C gyroscope."
-version = "3.0.0"
+version = "3.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_FXAS21002C"}
 keywords = [
     "adafruit",
```

