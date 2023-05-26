# Comparing `tmp/adafruit-circuitpython-touchscreen-1.2.1.tar.gz` & `tmp/adafruit-circuitpython-touchscreen-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-touchscreen-1.2.1.tar", last modified: Mon May  1 15:02:35 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-touchscreen-1.2.2.tar", last modified: Fri May 26 16:25:50 2023, max compression
```

## Comparing `adafruit-circuitpython-touchscreen-1.2.1.tar` & `adafruit-circuitpython-touchscreen-1.2.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.582328 adafruit-circuitpython-touchscreen-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.582328 adafruit-circuitpython-touchscreen-1.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.582328 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-01 15:02:35.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6972 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/adafruit_touchscreen.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     6145 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_calibrator_built_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_orientation.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-01 15:02:27.000000 adafruit-circuitpython-touchscreen-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 15:02:17.000000 adafruit-circuitpython-touchscreen-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 15:02:35.586328 adafruit-circuitpython-touchscreen-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.270369 adafruit-circuitpython-touchscreen-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.262369 adafruit-circuitpython-touchscreen-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-26 16:25:50.270369 adafruit-circuitpython-touchscreen-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3690 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 16:25:50.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/adafruit_touchscreen.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.266369 adafruit-circuitpython-touchscreen-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:50.270369 adafruit-circuitpython-touchscreen-1.2.2/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6146 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_calibrator_built_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_orientation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-26 16:25:43.000000 adafruit-circuitpython-touchscreen-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:25:32.000000 adafruit-circuitpython-touchscreen-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:25:50.270369 adafruit-circuitpython-touchscreen-1.2.2/setup.cfg
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-touchscreen-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/.gitignore` & `adafruit-circuitpython-touchscreen-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/.pre-commit-config.yaml` & `adafruit-circuitpython-touchscreen-1.2.2/.pre-commit-config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
   - repo: https://github.com/python/black
-    rev: 22.3.0
+    rev: 23.3.0
     hooks:
       - id: black
   - repo: https://github.com/fsfe/reuse-tool
-    rev: v0.14.0
+    rev: v1.1.2
     hooks:
       - id: reuse
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.2.0
+    rev: v4.4.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.15.5
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/.pylintrc` & `adafruit-circuitpython-touchscreen-1.2.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-touchscreen-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/LICENSE` & `adafruit-circuitpython-touchscreen-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-touchscreen-1.2.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/LICENSES/MIT.txt` & `adafruit-circuitpython-touchscreen-1.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-touchscreen-1.2.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/PKG-INFO` & `adafruit-circuitpython-touchscreen-1.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-touchscreen
-Version: 1.2.1
+Version: 1.2.2
 Summary: CircuitPython library for 4-wire resistive touchscreens
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen
 Keywords: adafruit,blinka,circuitpython,micropython,touchscreen,resistive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/README.rst` & `adafruit-circuitpython-touchscreen-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO` & `adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-touchscreen
-Version: 1.2.1
+Version: 1.2.2
 Summary: CircuitPython library for 4-wire resistive touchscreens
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen
 Keywords: adafruit,blinka,circuitpython,micropython,touchscreen,resistive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt` & `adafruit-circuitpython-touchscreen-1.2.2/adafruit_circuitpython_touchscreen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/adafruit_touchscreen.py` & `adafruit-circuitpython-touchscreen-1.2.2/adafruit_touchscreen.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,29 +17,28 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen.git"
 
 from digitalio import DigitalInOut
 from analogio import AnalogIn
 
 try:
     from typing import Optional, Tuple
     from microcontroller import Pin
 except ImportError:
     pass
 
 
 def map_range(x: float, in_min: int, in_max: int, out_min: int, out_max: int) -> float:
-
     """
     Maps a number from one range to another.
 
     .. note:: This implementation handles values < in_min differently
               than arduino's map function does.
 
 
@@ -105,15 +104,14 @@
         x_resistance: Optional[int] = None,
         samples: int = 4,
         z_threshold: int = 10000,
         calibration: Optional[Tuple[Tuple[int, int], Tuple[int, int]]] = None,
         size: Optional[Tuple[int, int]] = None,
         invert_pressure: bool = True
     ) -> None:
-
         self._xm_pin = x1_pin
         self._xp_pin = x2_pin
         self._ym_pin = y1_pin
         self._yp_pin = y2_pin
         self._rx_plate = x_resistance
         self._xsamples = [0] * samples
         self._ysamples = [0] * samples
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/docs/_static/favicon.ico` & `adafruit-circuitpython-touchscreen-1.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/docs/conf.py` & `adafruit-circuitpython-touchscreen-1.2.2/docs/conf.py`

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

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/docs/index.rst` & `adafruit-circuitpython-touchscreen-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_calibrator_built_in.py` & `adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_calibrator_built_in.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 import adafruit_touchscreen
 
 
 # Operational parameters:
 DISPLAY_ROTATION = 0  # Specify 0, 90, 180, or 270 degrees
 REPL_ONLY = False  # True to disable graphics
 
+
 # pylint: disable=too-few-public-methods
 class Colors:
     """A collection of colors used for graphic objects."""
 
     BLUE_DK = 0x000060  # Screen fill
     RED = 0xFF0000  # Boundary
     WHITE = 0xFFFFFF  # Text
```

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_orientation.py` & `adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_orientation.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/examples/touchscreen_simpletest.py` & `adafruit-circuitpython-touchscreen-1.2.2/examples/touchscreen_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-touchscreen-1.2.1/pyproject.toml` & `adafruit-circuitpython-touchscreen-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-touchscreen"
 description = "CircuitPython library for 4-wire resistive touchscreens"
-version = "1.2.1"
+version = "1.2.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Touchscreen"}
 keywords = [
     "adafruit",
```

