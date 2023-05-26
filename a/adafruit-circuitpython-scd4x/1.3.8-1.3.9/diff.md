# Comparing `tmp/adafruit-circuitpython-scd4x-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-scd4x-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-scd4x-1.3.8.tar", last modified: Mon Nov 28 18:27:52 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-scd4x-1.3.9.tar", last modified: Fri May 26 15:56:53 2023, max compression
```

## Comparing `adafruit-circuitpython-scd4x-1.3.8.tar` & `adafruit-circuitpython-scd4x-1.3.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.092400 adafruit-circuitpython-scd4x-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3775 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/adafruit_circuitpython_scd4x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4541 2022-11-28 18:27:52.000000 adafruit-circuitpython-scd4x-1.3.8/adafruit_circuitpython_scd4x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      981 2022-11-28 18:27:52.000000 adafruit-circuitpython-scd4x-1.3.8/adafruit_circuitpython_scd4x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:27:52.000000 adafruit-circuitpython-scd4x-1.3.8/adafruit_circuitpython_scd4x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:27:52.000000 adafruit-circuitpython-scd4x-1.3.8/adafruit_circuitpython_scd4x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2022-11-28 18:27:52.000000 adafruit-circuitpython-scd4x-1.3.8/adafruit_circuitpython_scd4x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    13322 2022-11-28 18:27:44.000000 adafruit-circuitpython-scd4x-1.3.8/adafruit_scd4x.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      265 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5984 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      184 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      972 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      722 2022-11-28 18:27:44.000000 adafruit-circuitpython-scd4x-1.3.8/examples/scd4x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1774 2022-11-28 18:27:44.000000 adafruit-circuitpython-scd4x-1.3.8/examples/scd4x_tuning_knobs.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1246 2022-11-28 18:27:44.000000 adafruit-circuitpython-scd4x-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-28 18:27:37.000000 adafruit-circuitpython-scd4x-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:27:52.096400 adafruit-circuitpython-scd4x-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.906529 adafruit-circuitpython-scd4x-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 15:56:53.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13322 2023-05-26 15:56:47.000000 adafruit-circuitpython-scd4x-1.3.9/adafruit_scd4x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6012 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-26 15:56:47.000000 adafruit-circuitpython-scd4x-1.3.9/examples/scd4x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-26 15:56:47.000000 adafruit-circuitpython-scd4x-1.3.9/examples/scd4x_tuning_knobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-26 15:56:47.000000 adafruit-circuitpython-scd4x-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 15:56:38.000000 adafruit-circuitpython-scd4x-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:56:53.910529 adafruit-circuitpython-scd4x-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-scd4x-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-scd4x-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/.gitignore` & `adafruit-circuitpython-scd4x-1.3.9/.gitignore`

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

### Comparing `adafruit-circuitpython-scd4x-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-scd4x-1.3.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-scd4x-1.3.8/.pylintrc` & `adafruit-circuitpython-scd4x-1.3.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-scd4x-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-scd4x-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/LICENSE` & `adafruit-circuitpython-scd4x-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-scd4x-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-scd4x-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-scd4x-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/PKG-INFO` & `adafruit-circuitpython-scd4x-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-scd4x
-Version: 1.3.8
+Version: 1.3.9
 Summary: Driver for Sensirion SCD4X CO2 sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SCD4X.git
 Keywords: adafruit,blinka,circuitpython,micropython,scd4x,CO2,humidity,temperature,sensor,SCD40,SCD41
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-scd4x-1.3.8/README.rst` & `adafruit-circuitpython-scd4x-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/adafruit_circuitpython_scd4x.egg-info/PKG-INFO` & `adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-scd4x
-Version: 1.3.8
+Version: 1.3.9
 Summary: Driver for Sensirion SCD4X CO2 sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SCD4X.git
 Keywords: adafruit,blinka,circuitpython,micropython,scd4x,CO2,humidity,temperature,sensor,SCD40,SCD41
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-scd4x-1.3.8/adafruit_circuitpython_scd4x.egg-info/SOURCES.txt` & `adafruit-circuitpython-scd4x-1.3.9/adafruit_circuitpython_scd4x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/adafruit_scd4x.py` & `adafruit-circuitpython-scd4x-1.3.9/adafruit_scd4x.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     from typing import Tuple, Union
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SCD4X.git"
 
 SCD4X_DEFAULT_ADDR = 0x62
 _SCD4X_REINIT = const(0x3646)
 _SCD4X_FACTORYRESET = const(0x3632)
 _SCD4X_FORCEDRECAL = const(0x362F)
 _SCD4X_SELFTEST = const(0x3639)
```

### Comparing `adafruit-circuitpython-scd4x-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-scd4x-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/docs/conf.py` & `adafruit-circuitpython-scd4x-1.3.9/docs/conf.py`

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

### Comparing `adafruit-circuitpython-scd4x-1.3.8/docs/index.rst` & `adafruit-circuitpython-scd4x-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/examples/scd4x_simpletest.py` & `adafruit-circuitpython-scd4x-1.3.9/examples/scd4x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/examples/scd4x_tuning_knobs.py` & `adafruit-circuitpython-scd4x-1.3.9/examples/scd4x_tuning_knobs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-scd4x-1.3.8/pyproject.toml` & `adafruit-circuitpython-scd4x-1.3.9/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-scd4x"
 description = "Driver for Sensirion SCD4X CO2 sensor"
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SCD4X.git"}
 keywords = [
     "adafruit",
```

