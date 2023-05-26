# Comparing `tmp/adafruit-circuitpython-msa301-1.3.1.tar.gz` & `tmp/adafruit-circuitpython-msa301-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-msa301-1.3.1.tar", last modified: Mon Nov 28 18:09:07 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-msa301-1.3.2.tar", last modified: Fri May 26 15:57:12 2023, max compression
```

## Comparing `adafruit-circuitpython-msa301-1.3.1.tar` & `adafruit-circuitpython-msa301-1.3.2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.337348 adafruit-circuitpython-msa301-1.3.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.333348 adafruit-circuitpython-msa301-1.3.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.333348 adafruit-circuitpython-msa301-1.3.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.333348 adafruit-circuitpython-msa301-1.3.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.333348 adafruit-circuitpython-msa301-1.3.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3633 2022-11-28 18:09:07.337348 adafruit-circuitpython-msa301-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2866 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.337348 adafruit-circuitpython-msa301-1.3.1/adafruit_circuitpython_msa301.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3633 2022-11-28 18:09:07.000000 adafruit-circuitpython-msa301-1.3.1/adafruit_circuitpython_msa301.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1018 2022-11-28 18:09:07.000000 adafruit-circuitpython-msa301-1.3.1/adafruit_circuitpython_msa301.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:09:07.000000 adafruit-circuitpython-msa301-1.3.1/adafruit_circuitpython_msa301.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:09:07.000000 adafruit-circuitpython-msa301-1.3.1/adafruit_circuitpython_msa301.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2022-11-28 18:09:07.000000 adafruit-circuitpython-msa301-1.3.1/adafruit_circuitpython_msa301.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11821 2022-11-28 18:08:58.000000 adafruit-circuitpython-msa301-1.3.1/adafruit_msa3xx.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.337348 adafruit-circuitpython-msa301-1.3.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.337348 adafruit-circuitpython-msa301-1.3.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      265 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5879 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      368 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1268 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:07.337348 adafruit-circuitpython-msa301-1.3.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (122)      392 2022-11-28 18:08:58.000000 adafruit-circuitpython-msa301-1.3.1/examples/msa301_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      428 2022-11-28 18:08:58.000000 adafruit-circuitpython-msa301-1.3.1/examples/msa301_tap_example.py
--rw-r--r--   0 runner    (1001) docker     (122)      392 2022-11-28 18:08:58.000000 adafruit-circuitpython-msa301-1.3.1/examples/msa311_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1227 2022-11-28 18:08:58.000000 adafruit-circuitpython-msa301-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:08:47.000000 adafruit-circuitpython-msa301-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:09:07.337348 adafruit-circuitpython-msa301-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.671265 adafruit-circuitpython-msa301-1.3.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.667265 adafruit-circuitpython-msa301-1.3.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.667265 adafruit-circuitpython-msa301-1.3.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.667265 adafruit-circuitpython-msa301-1.3.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.667265 adafruit-circuitpython-msa301-1.3.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-26 15:57:12.671265 adafruit-circuitpython-msa301-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2866 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.667265 adafruit-circuitpython-msa301-1.3.2/adafruit_circuitpython_msa301.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-26 15:57:12.000000 adafruit-circuitpython-msa301-1.3.2/adafruit_circuitpython_msa301.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-05-26 15:57:12.000000 adafruit-circuitpython-msa301-1.3.2/adafruit_circuitpython_msa301.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:57:12.000000 adafruit-circuitpython-msa301-1.3.2/adafruit_circuitpython_msa301.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 15:57:12.000000 adafruit-circuitpython-msa301-1.3.2/adafruit_circuitpython_msa301.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 15:57:12.000000 adafruit-circuitpython-msa301-1.3.2/adafruit_circuitpython_msa301.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11821 2023-05-26 15:57:05.000000 adafruit-circuitpython-msa301-1.3.2/adafruit_msa3xx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.671265 adafruit-circuitpython-msa301-1.3.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.671265 adafruit-circuitpython-msa301-1.3.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5907 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:12.671265 adafruit-circuitpython-msa301-1.3.2/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      392 2023-05-26 15:57:05.000000 adafruit-circuitpython-msa301-1.3.2/examples/msa301_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 15:57:05.000000 adafruit-circuitpython-msa301-1.3.2/examples/msa301_tap_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-26 15:57:05.000000 adafruit-circuitpython-msa301-1.3.2/examples/msa311_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-26 15:57:05.000000 adafruit-circuitpython-msa301-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 15:56:52.000000 adafruit-circuitpython-msa301-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:57:12.671265 adafruit-circuitpython-msa301-1.3.2/setup.cfg
```

### Comparing `adafruit-circuitpython-msa301-1.3.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-msa301-1.3.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/.gitignore` & `adafruit-circuitpython-msa301-1.3.2/.gitignore`

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

### Comparing `adafruit-circuitpython-msa301-1.3.1/.pre-commit-config.yaml` & `adafruit-circuitpython-msa301-1.3.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-msa301-1.3.1/.pylintrc` & `adafruit-circuitpython-msa301-1.3.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-msa301-1.3.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-msa301-1.3.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/LICENSE` & `adafruit-circuitpython-msa301-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-msa301-1.3.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/LICENSES/MIT.txt` & `adafruit-circuitpython-msa301-1.3.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-msa301-1.3.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/PKG-INFO` & `adafruit-circuitpython-msa301-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-msa301
-Version: 1.3.1
+Version: 1.3.2
 Summary: CircuitPython library for the MSA301/MSA311 Accelerometers
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MSA301
 Keywords: adafruit,blinka,circuitpython,micropython,msa301,msa311,accelerometer,msa
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-msa301-1.3.1/README.rst` & `adafruit-circuitpython-msa301-1.3.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/adafruit_circuitpython_msa301.egg-info/PKG-INFO` & `adafruit-circuitpython-msa301-1.3.2/adafruit_circuitpython_msa301.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-msa301
-Version: 1.3.1
+Version: 1.3.2
 Summary: CircuitPython library for the MSA301/MSA311 Accelerometers
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MSA301
 Keywords: adafruit,blinka,circuitpython,micropython,msa301,msa311,accelerometer,msa
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-msa301-1.3.1/adafruit_circuitpython_msa301.egg-info/SOURCES.txt` & `adafruit-circuitpython-msa301-1.3.2/adafruit_circuitpython_msa301.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/adafruit_msa3xx.py` & `adafruit-circuitpython-msa301-1.3.2/adafruit_msa3xx.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
   https://circuitpython.org/downloads
 * Adafruit's Bus Device library:
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library:
   https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 
-__version__ = "1.3.1"
+__version__ = "1.3.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MSA301.git"
 
 from micropython import const
 from adafruit_register.i2c_struct import Struct, ROUnaryStruct
 from adafruit_register.i2c_bit import RWBit
 from adafruit_register.i2c_bits import RWBits
 import adafruit_bus_device.i2c_device as i2cdevice
```

### Comparing `adafruit-circuitpython-msa301-1.3.1/docs/_static/favicon.ico` & `adafruit-circuitpython-msa301-1.3.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/docs/conf.py` & `adafruit-circuitpython-msa301-1.3.2/docs/conf.py`

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

### Comparing `adafruit-circuitpython-msa301-1.3.1/docs/index.rst` & `adafruit-circuitpython-msa301-1.3.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-msa301-1.3.1/pyproject.toml` & `adafruit-circuitpython-msa301-1.3.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-msa301"
 description = "CircuitPython library for the MSA301/MSA311 Accelerometers"
-version = "1.3.1"
+version = "1.3.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MSA301"}
 keywords = [
     "adafruit",
```

