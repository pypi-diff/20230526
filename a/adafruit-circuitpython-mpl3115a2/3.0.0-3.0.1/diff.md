# Comparing `tmp/adafruit-circuitpython-mpl3115a2-3.0.0.tar.gz` & `tmp/adafruit-circuitpython-mpl3115a2-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mpl3115a2-3.0.0.tar", last modified: Wed Mar 15 16:11:15 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-mpl3115a2-3.0.1.tar", last modified: Fri May 26 16:26:37 2023, max compression
```

## Comparing `adafruit-circuitpython-mpl3115a2-3.0.0.tar` & `adafruit-circuitpython-mpl3115a2-3.0.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.129531 adafruit-circuitpython-mpl3115a2-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_circuitpython_mpl3115a2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-03-15 16:11:15.000000 adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_circuitpython_mpl3115a2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-15 16:11:15.000000 adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_circuitpython_mpl3115a2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 16:11:15.000000 adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_circuitpython_mpl3115a2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-03-15 16:11:15.000000 adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_circuitpython_mpl3115a2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-15 16:11:15.000000 adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_circuitpython_mpl3115a2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-03-15 16:11:07.000000 adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_mpl3115a2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5599 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-03-15 16:11:07.000000 adafruit-circuitpython-mpl3115a2-3.0.0/examples/mpl3115a2_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-03-15 16:11:07.000000 adafruit-circuitpython-mpl3115a2-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-03-15 16:10:58.000000 adafruit-circuitpython-mpl3115a2-3.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 16:11:15.133530 adafruit-circuitpython-mpl3115a2-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.938468 adafruit-circuitpython-mpl3115a2-3.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.930468 adafruit-circuitpython-mpl3115a2-3.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.934468 adafruit-circuitpython-mpl3115a2-3.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.934468 adafruit-circuitpython-mpl3115a2-3.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.934468 adafruit-circuitpython-mpl3115a2-3.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-26 16:26:37.938468 adafruit-circuitpython-mpl3115a2-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.934468 adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_circuitpython_mpl3115a2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3455 2023-05-26 16:26:37.000000 adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_circuitpython_mpl3115a2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-26 16:26:37.000000 adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_circuitpython_mpl3115a2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:26:37.000000 adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_circuitpython_mpl3115a2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:26:37.000000 adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_circuitpython_mpl3115a2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 16:26:37.000000 adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_circuitpython_mpl3115a2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11211 2023-05-26 16:26:29.000000 adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_mpl3115a2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.934468 adafruit-circuitpython-mpl3115a2-3.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.934468 adafruit-circuitpython-mpl3115a2-3.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:37.938468 adafruit-circuitpython-mpl3115a2-3.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 2023-05-26 16:26:29.000000 adafruit-circuitpython-mpl3115a2-3.0.1/examples/mpl3115a2_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-26 16:26:29.000000 adafruit-circuitpython-mpl3115a2-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:26:13.000000 adafruit-circuitpython-mpl3115a2-3.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:26:37.938468 adafruit-circuitpython-mpl3115a2-3.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mpl3115a2-3.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/.gitignore` & `adafruit-circuitpython-mpl3115a2-3.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-mpl3115a2-3.0.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/.pylintrc` & `adafruit-circuitpython-mpl3115a2-3.0.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mpl3115a2-3.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/LICENSE` & `adafruit-circuitpython-mpl3115a2-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mpl3115a2-3.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-mpl3115a2-3.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mpl3115a2-3.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/PKG-INFO` & `adafruit-circuitpython-mpl3115a2-3.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mpl3115a2
-Version: 3.0.0
+Version: 3.0.1
 Summary: CircuitPython library for MPL3115A2 barometric pressure and temperature sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MPL3115A2
 Keywords: adafruit,mpl3115a2,barometric,pressure,temperature,sensor,breakout,hardwaremicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/README.rst` & `adafruit-circuitpython-mpl3115a2-3.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_circuitpython_mpl3115a2.egg-info/PKG-INFO` & `adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_circuitpython_mpl3115a2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mpl3115a2
-Version: 3.0.0
+Version: 3.0.1
 Summary: CircuitPython library for MPL3115A2 barometric pressure and temperature sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MPL3115A2
 Keywords: adafruit,mpl3115a2,barometric,pressure,temperature,sensor,breakout,hardwaremicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_circuitpython_mpl3115a2.egg-info/SOURCES.txt` & `adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_circuitpython_mpl3115a2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/adafruit_mpl3115a2.py` & `adafruit-circuitpython-mpl3115a2-3.0.1/adafruit_mpl3115a2.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 import struct
 import time
 
 from micropython import const
 from adafruit_bus_device import i2c_device
 
 
-__version__ = "3.0.0"
+__version__ = "3.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MPL3115A2.git"
 
 
 # Internal constants:
 _MPL3115A2_ADDRESS = const(0x60)
 _MPL3115A2_REGISTER_STATUS = const(0x00)
 _MPL3115A2_REGISTER_PRESSURE_MSB = const(0x01)
```

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-mpl3115a2-3.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/docs/conf.py` & `adafruit-circuitpython-mpl3115a2-3.0.1/docs/conf.py`

 * *Files 8% similar despite different names*

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
     #'sphinx.ext.napoleon'
     "sphinx.ext.todo",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
```

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/docs/index.rst` & `adafruit-circuitpython-mpl3115a2-3.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/examples/mpl3115a2_simpletest.py` & `adafruit-circuitpython-mpl3115a2-3.0.1/examples/mpl3115a2_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mpl3115a2-3.0.0/pyproject.toml` & `adafruit-circuitpython-mpl3115a2-3.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mpl3115a2"
 description = "CircuitPython library for MPL3115A2 barometric pressure and temperature sensor."
-version = "3.0.0"
+version = "3.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MPL3115A2"}
 keywords = [
     "adafruit",
```

