# Comparing `tmp/adafruit-circuitpython-tsc2007-1.0.6.tar.gz` & `tmp/adafruit-circuitpython-tsc2007-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tsc2007-1.0.6.tar", last modified: Mon Nov 28 18:05:26 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tsc2007-1.0.7.tar", last modified: Fri May 26 15:56:18 2023, max compression
```

## Comparing `adafruit-circuitpython-tsc2007-1.0.6.tar` & `adafruit-circuitpython-tsc2007-1.0.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.690346 adafruit-circuitpython-tsc2007-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.686346 adafruit-circuitpython-tsc2007-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.686346 adafruit-circuitpython-tsc2007-1.0.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.686346 adafruit-circuitpython-tsc2007-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.686346 adafruit-circuitpython-tsc2007-1.0.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4700 2022-11-28 18:05:26.690346 adafruit-circuitpython-tsc2007-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3937 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.686346 adafruit-circuitpython-tsc2007-1.0.6/adafruit_circuitpython_tsc2007.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4700 2022-11-28 18:05:26.000000 adafruit-circuitpython-tsc2007-1.0.6/adafruit_circuitpython_tsc2007.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      964 2022-11-28 18:05:26.000000 adafruit-circuitpython-tsc2007-1.0.6/adafruit_circuitpython_tsc2007.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:05:26.000000 adafruit-circuitpython-tsc2007-1.0.6/adafruit_circuitpython_tsc2007.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:05:26.000000 adafruit-circuitpython-tsc2007-1.0.6/adafruit_circuitpython_tsc2007.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:05:26.000000 adafruit-circuitpython-tsc2007-1.0.6/adafruit_circuitpython_tsc2007.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3409 2022-11-28 18:05:17.000000 adafruit-circuitpython-tsc2007-1.0.6/adafruit_tsc2007.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.690346 adafruit-circuitpython-tsc2007-1.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.690346 adafruit-circuitpython-tsc2007-1.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      267 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1074 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:26.690346 adafruit-circuitpython-tsc2007-1.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      798 2022-11-28 18:05:17.000000 adafruit-circuitpython-tsc2007-1.0.6/examples/tsc2007_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1217 2022-11-28 18:05:17.000000 adafruit-circuitpython-tsc2007-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-28 18:05:10.000000 adafruit-circuitpython-tsc2007-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:05:26.690346 adafruit-circuitpython-tsc2007-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.894206 adafruit-circuitpython-tsc2007-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3937 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/adafruit_circuitpython_tsc2007.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-05-26 15:56:18.000000 adafruit-circuitpython-tsc2007-1.0.7/adafruit_circuitpython_tsc2007.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 15:56:18.000000 adafruit-circuitpython-tsc2007-1.0.7/adafruit_circuitpython_tsc2007.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:56:18.000000 adafruit-circuitpython-tsc2007-1.0.7/adafruit_circuitpython_tsc2007.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 15:56:18.000000 adafruit-circuitpython-tsc2007-1.0.7/adafruit_circuitpython_tsc2007.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 15:56:18.000000 adafruit-circuitpython-tsc2007-1.0.7/adafruit_circuitpython_tsc2007.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3409 2023-05-26 15:56:11.000000 adafruit-circuitpython-tsc2007-1.0.7/adafruit_tsc2007.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-26 15:56:11.000000 adafruit-circuitpython-tsc2007-1.0.7/examples/tsc2007_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-26 15:56:11.000000 adafruit-circuitpython-tsc2007-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 15:55:59.000000 adafruit-circuitpython-tsc2007-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:56:18.898206 adafruit-circuitpython-tsc2007-1.0.7/setup.cfg
```

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tsc2007-1.0.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/.gitignore` & `adafruit-circuitpython-tsc2007-1.0.7/.gitignore`

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

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/.pre-commit-config.yaml` & `adafruit-circuitpython-tsc2007-1.0.7/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/.pylintrc` & `adafruit-circuitpython-tsc2007-1.0.7/.pylintrc`

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

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tsc2007-1.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/LICENSE` & `adafruit-circuitpython-tsc2007-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tsc2007-1.0.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/LICENSES/MIT.txt` & `adafruit-circuitpython-tsc2007-1.0.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tsc2007-1.0.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/PKG-INFO` & `adafruit-circuitpython-tsc2007-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tsc2007
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python library for TSC2007 resistive touch screen driver
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TSC2007.git
 Keywords: adafruit,blinka,circuitpython,micropython,tsc2007,touch,resistive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/README.rst` & `adafruit-circuitpython-tsc2007-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/adafruit_circuitpython_tsc2007.egg-info/PKG-INFO` & `adafruit-circuitpython-tsc2007-1.0.7/adafruit_circuitpython_tsc2007.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tsc2007
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python library for TSC2007 resistive touch screen driver
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TSC2007.git
 Keywords: adafruit,blinka,circuitpython,micropython,tsc2007,touch,resistive
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/adafruit_circuitpython_tsc2007.egg-info/SOURCES.txt` & `adafruit-circuitpython-tsc2007-1.0.7/adafruit_circuitpython_tsc2007.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/adafruit_tsc2007.py` & `adafruit-circuitpython-tsc2007-1.0.7/adafruit_tsc2007.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 """
 
 
 import digitalio
 from adafruit_bus_device import i2c_device
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TSC2007.git"
 
 TSC2007_MEASURE_TEMP0 = 0
 TSC2007_MEASURE_AUX = 2
 TSC2007_MEASURE_TEMP1 = 4
 TSC2007_ACTIVATE_X = 8
 TSC2007_ACTIVATE_Y = 9
```

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/docs/_static/favicon.ico` & `adafruit-circuitpython-tsc2007-1.0.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/docs/conf.py` & `adafruit-circuitpython-tsc2007-1.0.7/docs/conf.py`

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

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/docs/index.rst` & `adafruit-circuitpython-tsc2007-1.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/examples/tsc2007_simpletest.py` & `adafruit-circuitpython-tsc2007-1.0.7/examples/tsc2007_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsc2007-1.0.6/pyproject.toml` & `adafruit-circuitpython-tsc2007-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-tsc2007"
 description = "Python library for TSC2007 resistive touch screen driver"
-version = "1.0.6"
+version = "1.0.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_TSC2007.git"}
 keywords = [
     "adafruit",
```

