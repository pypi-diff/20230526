# Comparing `tmp/adafruit-circuitpython-si1145-1.1.7.tar.gz` & `tmp/adafruit-circuitpython-si1145-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-si1145-1.1.7.tar", last modified: Mon Nov 28 18:07:59 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-si1145-1.1.8.tar", last modified: Fri May 26 15:56:49 2023, max compression
```

## Comparing `adafruit-circuitpython-si1145-1.1.7.tar` & `adafruit-circuitpython-si1145-1.1.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.507484 adafruit-circuitpython-si1145-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.499484 adafruit-circuitpython-si1145-1.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.503484 adafruit-circuitpython-si1145-1.1.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.503484 adafruit-circuitpython-si1145-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.507484 adafruit-circuitpython-si1145-1.1.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2022-11-28 18:07:59.507484 adafruit-circuitpython-si1145-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.507484 adafruit-circuitpython-si1145-1.1.7/adafruit_circuitpython_si1145.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4102 2022-11-28 18:07:59.000000 adafruit-circuitpython-si1145-1.1.7/adafruit_circuitpython_si1145.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      957 2022-11-28 18:07:59.000000 adafruit-circuitpython-si1145-1.1.7/adafruit_circuitpython_si1145.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:07:59.000000 adafruit-circuitpython-si1145-1.1.7/adafruit_circuitpython_si1145.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:07:59.000000 adafruit-circuitpython-si1145-1.1.7/adafruit_circuitpython_si1145.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 18:07:59.000000 adafruit-circuitpython-si1145-1.1.7/adafruit_circuitpython_si1145.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5878 2022-11-28 18:07:51.000000 adafruit-circuitpython-si1145-1.1.7/adafruit_si1145.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.507484 adafruit-circuitpython-si1145-1.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.507484 adafruit-circuitpython-si1145-1.1.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5982 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1069 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:07:59.507484 adafruit-circuitpython-si1145-1.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      668 2022-11-28 18:07:51.000000 adafruit-circuitpython-si1145-1.1.7/examples/si1145_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1277 2022-11-28 18:07:51.000000 adafruit-circuitpython-si1145-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:07:42.000000 adafruit-circuitpython-si1145-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:07:59.511484 adafruit-circuitpython-si1145-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.401705 adafruit-circuitpython-si1145-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.393705 adafruit-circuitpython-si1145-1.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.397705 adafruit-circuitpython-si1145-1.1.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.397705 adafruit-circuitpython-si1145-1.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.397705 adafruit-circuitpython-si1145-1.1.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-26 15:56:49.401705 adafruit-circuitpython-si1145-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.397705 adafruit-circuitpython-si1145-1.1.8/adafruit_circuitpython_si1145.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-26 15:56:49.000000 adafruit-circuitpython-si1145-1.1.8/adafruit_circuitpython_si1145.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-26 15:56:49.000000 adafruit-circuitpython-si1145-1.1.8/adafruit_circuitpython_si1145.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:56:49.000000 adafruit-circuitpython-si1145-1.1.8/adafruit_circuitpython_si1145.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 15:56:49.000000 adafruit-circuitpython-si1145-1.1.8/adafruit_circuitpython_si1145.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 15:56:49.000000 adafruit-circuitpython-si1145-1.1.8/adafruit_circuitpython_si1145.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5878 2023-05-26 15:56:40.000000 adafruit-circuitpython-si1145-1.1.8/adafruit_si1145.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.401705 adafruit-circuitpython-si1145-1.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.401705 adafruit-circuitpython-si1145-1.1.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:49.401705 adafruit-circuitpython-si1145-1.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-26 15:56:40.000000 adafruit-circuitpython-si1145-1.1.8/examples/si1145_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-26 15:56:40.000000 adafruit-circuitpython-si1145-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 15:56:30.000000 adafruit-circuitpython-si1145-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:56:49.401705 adafruit-circuitpython-si1145-1.1.8/setup.cfg
```

### Comparing `adafruit-circuitpython-si1145-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-si1145-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/.gitignore` & `adafruit-circuitpython-si1145-1.1.8/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-si1145-1.1.7/.pre-commit-config.yaml` & `adafruit-circuitpython-si1145-1.1.8/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

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
           - --disable=consider-using-f-string,duplicate-code
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-si1145-1.1.7/.pylintrc` & `adafruit-circuitpython-si1145-1.1.8/.pylintrc`

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

### Comparing `adafruit-circuitpython-si1145-1.1.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-si1145-1.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/LICENSE` & `adafruit-circuitpython-si1145-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-si1145-1.1.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/LICENSES/MIT.txt` & `adafruit-circuitpython-si1145-1.1.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-si1145-1.1.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/PKG-INFO` & `adafruit-circuitpython-si1145-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si1145
-Version: 1.1.7
+Version: 1.1.8
 Summary: CircuitPython helper library for the SI1145 Digital UV Index IR Visible Light Sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI1145.git
 Keywords: adafruit,blinka,circuitpython,micropython,si1145,ultraviolet,,infrared,,visible,,light
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si1145-1.1.7/README.rst` & `adafruit-circuitpython-si1145-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/adafruit_circuitpython_si1145.egg-info/PKG-INFO` & `adafruit-circuitpython-si1145-1.1.8/adafruit_circuitpython_si1145.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si1145
-Version: 1.1.7
+Version: 1.1.8
 Summary: CircuitPython helper library for the SI1145 Digital UV Index IR Visible Light Sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI1145.git
 Keywords: adafruit,blinka,circuitpython,micropython,si1145,ultraviolet,,infrared,,visible,,light
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si1145-1.1.7/adafruit_circuitpython_si1145.egg-info/SOURCES.txt` & `adafruit-circuitpython-si1145-1.1.8/adafruit_circuitpython_si1145.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/adafruit_si1145.py` & `adafruit-circuitpython-si1145-1.1.8/adafruit_si1145.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     from typing import Tuple, Union
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SI1145.git"
 
 # Registers
 _DEFAULT_ADDRESS = const(0x60)
 _PART_ID = const(0x00)
 _HW_KEY = const(0x07)
 _COEFF_0 = const(0x13)
```

### Comparing `adafruit-circuitpython-si1145-1.1.7/docs/_static/favicon.ico` & `adafruit-circuitpython-si1145-1.1.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/docs/conf.py` & `adafruit-circuitpython-si1145-1.1.8/docs/conf.py`

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
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-si1145-1.1.7/docs/index.rst` & `adafruit-circuitpython-si1145-1.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/examples/si1145_simpletest.py` & `adafruit-circuitpython-si1145-1.1.8/examples/si1145_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si1145-1.1.7/pyproject.toml` & `adafruit-circuitpython-si1145-1.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-si1145"
 description = "CircuitPython helper library for the SI1145 Digital UV Index IR Visible Light Sensor"
-version = "1.1.7"
+version = "1.1.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SI1145.git"}
 keywords = [
     "adafruit",
```

