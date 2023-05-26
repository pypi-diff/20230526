# Comparing `tmp/adafruit-circuitpython-vl53l4cd-1.1.4.tar.gz` & `tmp/adafruit-circuitpython-vl53l4cd-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-vl53l4cd-1.1.4.tar", last modified: Mon Nov 28 18:02:57 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-vl53l4cd-1.1.5.tar", last modified: Fri May 26 16:05:58 2023, max compression
```

## Comparing `adafruit-circuitpython-vl53l4cd-1.1.4.tar` & `adafruit-circuitpython-vl53l4cd-1.1.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.049826 adafruit-circuitpython-vl53l4cd-1.1.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4202 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3422 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_circuitpython_vl53l4cd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4202 2022-11-28 18:02:57.000000 adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_circuitpython_vl53l4cd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1021 2022-11-28 18:02:57.000000 adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_circuitpython_vl53l4cd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:02:57.000000 adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_circuitpython_vl53l4cd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:02:57.000000 adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_circuitpython_vl53l4cd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-28 18:02:57.000000 adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_circuitpython_vl53l4cd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    16104 2022-11-28 18:02:49.000000 adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_vl53l4cd.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     6000 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      418 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1068 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     2742 2022-11-28 18:02:49.000000 adafruit-circuitpython-vl53l4cd-1.1.4/examples/vl53l4cd_set_address_multiple_sensors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1320 2022-11-28 18:02:49.000000 adafruit-circuitpython-vl53l4cd-1.1.4/examples/vl53l4cd_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2022-11-28 18:02:49.000000 adafruit-circuitpython-vl53l4cd-1.1.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-28 18:02:39.000000 adafruit-circuitpython-vl53l4cd-1.1.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:02:57.053826 adafruit-circuitpython-vl53l4cd-1.1.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.204200 adafruit-circuitpython-vl53l4cd-1.1.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.196200 adafruit-circuitpython-vl53l4cd-1.1.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.200199 adafruit-circuitpython-vl53l4cd-1.1.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.200199 adafruit-circuitpython-vl53l4cd-1.1.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.200199 adafruit-circuitpython-vl53l4cd-1.1.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-26 16:05:58.204200 adafruit-circuitpython-vl53l4cd-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3422 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.200199 adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_circuitpython_vl53l4cd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-26 16:05:58.000000 adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_circuitpython_vl53l4cd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 16:05:58.000000 adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_circuitpython_vl53l4cd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:05:58.000000 adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_circuitpython_vl53l4cd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:05:58.000000 adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_circuitpython_vl53l4cd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:05:58.000000 adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_circuitpython_vl53l4cd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16104 2023-05-26 16:05:50.000000 adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_vl53l4cd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.200199 adafruit-circuitpython-vl53l4cd-1.1.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.204200 adafruit-circuitpython-vl53l4cd-1.1.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6028 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:58.204200 adafruit-circuitpython-vl53l4cd-1.1.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-26 16:05:50.000000 adafruit-circuitpython-vl53l4cd-1.1.5/examples/vl53l4cd_set_address_multiple_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-26 16:05:50.000000 adafruit-circuitpython-vl53l4cd-1.1.5/examples/vl53l4cd_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2023-05-26 16:05:50.000000 adafruit-circuitpython-vl53l4cd-1.1.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:05:41.000000 adafruit-circuitpython-vl53l4cd-1.1.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:05:58.204200 adafruit-circuitpython-vl53l4cd-1.1.5/setup.cfg
```

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-vl53l4cd-1.1.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/.gitignore` & `adafruit-circuitpython-vl53l4cd-1.1.5/.gitignore`

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

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/.pre-commit-config.yaml` & `adafruit-circuitpython-vl53l4cd-1.1.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/.pylintrc` & `adafruit-circuitpython-vl53l4cd-1.1.5/.pylintrc`

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

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-vl53l4cd-1.1.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/LICENSE` & `adafruit-circuitpython-vl53l4cd-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-vl53l4cd-1.1.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/LICENSES/MIT.txt` & `adafruit-circuitpython-vl53l4cd-1.1.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-vl53l4cd-1.1.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/PKG-INFO` & `adafruit-circuitpython-vl53l4cd-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vl53l4cd
-Version: 1.1.4
+Version: 1.1.5
 Summary: CircuitPython helper library for the VL53L4CD time of flight distance sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_VL53L4CD.git
 Keywords: adafruit,blinka,circuitpython,micropython,vl53l4cd,distance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/README.rst` & `adafruit-circuitpython-vl53l4cd-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_circuitpython_vl53l4cd.egg-info/PKG-INFO` & `adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_circuitpython_vl53l4cd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vl53l4cd
-Version: 1.1.4
+Version: 1.1.5
 Summary: CircuitPython helper library for the VL53L4CD time of flight distance sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_VL53L4CD.git
 Keywords: adafruit,blinka,circuitpython,micropython,vl53l4cd,distance
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_circuitpython_vl53l4cd.egg-info/SOURCES.txt` & `adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_circuitpython_vl53l4cd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/adafruit_vl53l4cd.py` & `adafruit-circuitpython-vl53l4cd-1.1.5/adafruit_vl53l4cd.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 """
 
 import time
 import struct
 from adafruit_bus_device import i2c_device
 from micropython import const
 
-__version__ = "1.1.4"
+__version__ = "1.1.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_VL53L4CD.git"
 
 _VL53L4CD_SOFT_RESET = const(0x0000)
 _VL53L4CD_I2C_SLAVE_DEVICE_ADDRESS = const(0x0001)
 _VL53L4CD_VHV_CONFIG_TIMEOUT_MACROP_LOOP_BOUND = const(0x0008)
 _VL53L4CD_XTALK_PLANE_OFFSET_KCPS = const(0x0016)
 _VL53L4CD_XTALK_X_PLANE_GRADIENT_KCPS = const(0x0018)
```

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/docs/_static/favicon.ico` & `adafruit-circuitpython-vl53l4cd-1.1.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/docs/conf.py` & `adafruit-circuitpython-vl53l4cd-1.1.5/docs/conf.py`

 * *Files 0% similar despite different names*

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

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/docs/index.rst` & `adafruit-circuitpython-vl53l4cd-1.1.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/examples/vl53l4cd_set_address_multiple_sensors.py` & `adafruit-circuitpython-vl53l4cd-1.1.5/examples/vl53l4cd_set_address_multiple_sensors.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/examples/vl53l4cd_simpletest.py` & `adafruit-circuitpython-vl53l4cd-1.1.5/examples/vl53l4cd_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l4cd-1.1.4/pyproject.toml` & `adafruit-circuitpython-vl53l4cd-1.1.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-vl53l4cd"
 description = "CircuitPython helper library for the VL53L4CD time of flight distance sensor."
-version = "1.1.4"
+version = "1.1.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_VL53L4CD.git"}
 keywords = [
     "adafruit",
```

