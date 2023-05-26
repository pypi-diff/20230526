# Comparing `tmp/adafruit-circuitpython-itertools-2.0.4.tar.gz` & `tmp/adafruit-circuitpython-itertools-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-itertools-2.0.4.tar", last modified: Tue Nov 15 17:33:44 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-itertools-2.0.5.tar", last modified: Fri May 26 15:55:27 2023, max compression
```

## Comparing `adafruit-circuitpython-itertools-2.0.4.tar` & `adafruit-circuitpython-itertools-2.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.388536 adafruit-circuitpython-itertools-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.384536 adafruit-circuitpython-itertools-2.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.384536 adafruit-circuitpython-itertools-2.0.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.384536 adafruit-circuitpython-itertools-2.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2405 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.384536 adafruit-circuitpython-itertools-2.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2339 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/LICENSES/PSF-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-11-15 17:33:44.388536 adafruit-circuitpython-itertools-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2363 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.388536 adafruit-circuitpython-itertools-2.0.4/adafruit_circuitpython_itertools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3102 2022-11-15 17:33:44.000000 adafruit-circuitpython-itertools-2.0.4/adafruit_circuitpython_itertools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1056 2022-11-15 17:33:44.000000 adafruit-circuitpython-itertools-2.0.4/adafruit_circuitpython_itertools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 17:33:44.000000 adafruit-circuitpython-itertools-2.0.4/adafruit_circuitpython_itertools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-15 17:33:44.000000 adafruit-circuitpython-itertools-2.0.4/adafruit_circuitpython_itertools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-15 17:33:44.000000 adafruit-circuitpython-itertools-2.0.4/adafruit_circuitpython_itertools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.388536 adafruit-circuitpython-itertools-2.0.4/adafruit_itertools/
--rw-r--r--   0 runner    (1001) docker     (121)    16745 2022-11-15 17:33:36.000000 adafruit-circuitpython-itertools-2.0.4/adafruit_itertools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8759 2022-11-15 17:33:36.000000 adafruit-circuitpython-itertools-2.0.4/adafruit_itertools/adafruit_itertools_extras.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.388536 adafruit-circuitpython-itertools-2.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.388536 adafruit-circuitpython-itertools-2.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      343 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5387 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1127 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:33:44.388536 adafruit-circuitpython-itertools-2.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1724 2022-11-15 17:33:36.000000 adafruit-circuitpython-itertools-2.0.4/examples/itertools_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1186 2022-11-15 17:33:36.000000 adafruit-circuitpython-itertools-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-11-15 17:33:28.000000 adafruit-circuitpython-itertools-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 17:33:44.388536 adafruit-circuitpython-itertools-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.425567 adafruit-circuitpython-itertools-2.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.425567 adafruit-circuitpython-itertools-2.0.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.425567 adafruit-circuitpython-itertools-2.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/LICENSES/PSF-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/adafruit_circuitpython_itertools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-05-26 15:55:27.000000 adafruit-circuitpython-itertools-2.0.5/adafruit_circuitpython_itertools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-26 15:55:27.000000 adafruit-circuitpython-itertools-2.0.5/adafruit_circuitpython_itertools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:55:27.000000 adafruit-circuitpython-itertools-2.0.5/adafruit_circuitpython_itertools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 15:55:27.000000 adafruit-circuitpython-itertools-2.0.5/adafruit_circuitpython_itertools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 15:55:27.000000 adafruit-circuitpython-itertools-2.0.5/adafruit_circuitpython_itertools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/adafruit_itertools/
+-rw-r--r--   0 runner    (1001) docker     (123)    16745 2023-05-26 15:55:19.000000 adafruit-circuitpython-itertools-2.0.5/adafruit_itertools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8759 2023-05-26 15:55:19.000000 adafruit-circuitpython-itertools-2.0.5/adafruit_itertools/adafruit_itertools_extras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1724 2023-05-26 15:55:19.000000 adafruit-circuitpython-itertools-2.0.5/examples/itertools_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 15:55:19.000000 adafruit-circuitpython-itertools-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 15:55:07.000000 adafruit-circuitpython-itertools-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:55:27.429567 adafruit-circuitpython-itertools-2.0.5/setup.cfg
```

### Comparing `adafruit-circuitpython-itertools-2.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-itertools-2.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/.gitignore` & `adafruit-circuitpython-itertools-2.0.5/.gitignore`

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

### Comparing `adafruit-circuitpython-itertools-2.0.4/.pre-commit-config.yaml` & `adafruit-circuitpython-itertools-2.0.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-itertools-2.0.4/.pylintrc` & `adafruit-circuitpython-itertools-2.0.5/.pylintrc`

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

### Comparing `adafruit-circuitpython-itertools-2.0.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-itertools-2.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/LICENSE` & `adafruit-circuitpython-itertools-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-itertools-2.0.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/LICENSES/MIT.txt` & `adafruit-circuitpython-itertools-2.0.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/LICENSES/PSF-2.0.txt` & `adafruit-circuitpython-itertools-2.0.5/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-itertools-2.0.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/PKG-INFO` & `adafruit-circuitpython-itertools-2.0.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-itertools
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python's itertools for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IterTools
 Keywords: adafruit,itertools,cpython,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-itertools-2.0.4/README.rst` & `adafruit-circuitpython-itertools-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/adafruit_circuitpython_itertools.egg-info/PKG-INFO` & `adafruit-circuitpython-itertools-2.0.5/adafruit_circuitpython_itertools.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-itertools
-Version: 2.0.4
+Version: 2.0.5
 Summary: Python's itertools for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_IterTools
 Keywords: adafruit,itertools,cpython,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-itertools-2.0.4/adafruit_circuitpython_itertools.egg-info/SOURCES.txt` & `adafruit-circuitpython-itertools-2.0.5/adafruit_circuitpython_itertools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/adafruit_itertools/__init__.py` & `adafruit-circuitpython-itertools-2.0.5/adafruit_itertools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 """
 # pylint:disable=invalid-name,redefined-builtin,attribute-defined-outside-init
 # pylint:disable=stop-iteration-return,anomalous-backslash-in-string
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Itertools.git"
 
 
 def accumulate(iterable, func=lambda x, y: x + y):
     """Make an iterator that returns accumulated sums, or accumulated
     results of other binary functions (specified via the optional func
     argument). If func is supplied, it should be a function of two
```

### Comparing `adafruit-circuitpython-itertools-2.0.4/adafruit_itertools/adafruit_itertools_extras.py` & `adafruit-circuitpython-itertools-2.0.5/adafruit_itertools/adafruit_itertools_extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
   https://github.com/adafruit/circuitpython/releases
 """
 
 # pylint:disable=invalid-name,keyword-arg-before-vararg,relative-beyond-top-level
 
 import adafruit_itertools as it
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Itertools.git"
 
 
 def all_equal(iterable):
     """Returns True if all the elements are equal to each other.
 
     :param iterable: source of values
```

### Comparing `adafruit-circuitpython-itertools-2.0.4/docs/_static/favicon.ico` & `adafruit-circuitpython-itertools-2.0.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/docs/conf.py` & `adafruit-circuitpython-itertools-2.0.5/docs/conf.py`

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
 
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
```

### Comparing `adafruit-circuitpython-itertools-2.0.4/docs/index.rst` & `adafruit-circuitpython-itertools-2.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/examples/itertools_simpletest.py` & `adafruit-circuitpython-itertools-2.0.5/examples/itertools_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-itertools-2.0.4/pyproject.toml` & `adafruit-circuitpython-itertools-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-itertools"
 description = "Python's itertools for CircuitPython"
-version = "2.0.4"
+version = "2.0.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_IterTools"}
 keywords = [
     "adafruit",
```

