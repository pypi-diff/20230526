# Comparing `tmp/adafruit-circuitpython-onewire-2.0.4.tar.gz` & `tmp/adafruit-circuitpython-onewire-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-onewire-2.0.4.tar", last modified: Wed Jan 11 01:17:44 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-onewire-2.0.5.tar", last modified: Fri May 26 16:04:41 2023, max compression
```

## Comparing `adafruit-circuitpython-onewire-2.0.4.tar` & `adafruit-circuitpython-onewire-2.0.5.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.600422 adafruit-circuitpython-onewire-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.596422 adafruit-circuitpython-onewire-2.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.596422 adafruit-circuitpython-onewire-2.0.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.596422 adafruit-circuitpython-onewire-2.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.596422 adafruit-circuitpython-onewire-2.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-01-11 01:17:44.600422 adafruit-circuitpython-onewire-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.596422 adafruit-circuitpython-onewire-2.0.4/adafruit_circuitpython_onewire.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-01-11 01:17:44.000000 adafruit-circuitpython-onewire-2.0.4/adafruit_circuitpython_onewire.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-01-11 01:17:44.000000 adafruit-circuitpython-onewire-2.0.4/adafruit_circuitpython_onewire.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-11 01:17:44.000000 adafruit-circuitpython-onewire-2.0.4/adafruit_circuitpython_onewire.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-01-11 01:17:44.000000 adafruit-circuitpython-onewire-2.0.4/adafruit_circuitpython_onewire.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-11 01:17:44.000000 adafruit-circuitpython-onewire-2.0.4/adafruit_circuitpython_onewire.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.600422 adafruit-circuitpython-onewire-2.0.4/adafruit_onewire/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:36.000000 adafruit-circuitpython-onewire-2.0.4/adafruit_onewire/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-01-11 01:17:36.000000 adafruit-circuitpython-onewire-2.0.4/adafruit_onewire/bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-01-11 01:17:36.000000 adafruit-circuitpython-onewire-2.0.4/adafruit_onewire/device.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.600422 adafruit-circuitpython-onewire-2.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.600422 adafruit-circuitpython-onewire-2.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-11 01:17:44.600422 adafruit-circuitpython-onewire-2.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-01-11 01:17:36.000000 adafruit-circuitpython-onewire-2.0.4/examples/onewire_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-11 01:17:36.000000 adafruit-circuitpython-onewire-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-01-11 01:17:22.000000 adafruit-circuitpython-onewire-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-11 01:17:44.600422 adafruit-circuitpython-onewire-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.805729 adafruit-circuitpython-onewire-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.801729 adafruit-circuitpython-onewire-2.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.801729 adafruit-circuitpython-onewire-2.0.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.801729 adafruit-circuitpython-onewire-2.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.801729 adafruit-circuitpython-onewire-2.0.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-26 16:04:41.805729 adafruit-circuitpython-onewire-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.801729 adafruit-circuitpython-onewire-2.0.5/adafruit_circuitpython_onewire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-05-26 16:04:41.000000 adafruit-circuitpython-onewire-2.0.5/adafruit_circuitpython_onewire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-26 16:04:41.000000 adafruit-circuitpython-onewire-2.0.5/adafruit_circuitpython_onewire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:04:41.000000 adafruit-circuitpython-onewire-2.0.5/adafruit_circuitpython_onewire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-26 16:04:41.000000 adafruit-circuitpython-onewire-2.0.5/adafruit_circuitpython_onewire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:04:41.000000 adafruit-circuitpython-onewire-2.0.5/adafruit_circuitpython_onewire.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.805729 adafruit-circuitpython-onewire-2.0.5/adafruit_onewire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:34.000000 adafruit-circuitpython-onewire-2.0.5/adafruit_onewire/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-05-26 16:04:34.000000 adafruit-circuitpython-onewire-2.0.5/adafruit_onewire/bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2735 2023-05-26 16:04:34.000000 adafruit-circuitpython-onewire-2.0.5/adafruit_onewire/device.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.805729 adafruit-circuitpython-onewire-2.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.805729 adafruit-circuitpython-onewire-2.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5716 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:41.805729 adafruit-circuitpython-onewire-2.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 16:04:34.000000 adafruit-circuitpython-onewire-2.0.5/examples/onewire_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-26 16:04:34.000000 adafruit-circuitpython-onewire-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 16:04:24.000000 adafruit-circuitpython-onewire-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:04:41.805729 adafruit-circuitpython-onewire-2.0.5/setup.cfg
```

### Comparing `adafruit-circuitpython-onewire-2.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-onewire-2.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/.gitignore` & `adafruit-circuitpython-onewire-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/.pre-commit-config.yaml` & `adafruit-circuitpython-onewire-2.0.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-onewire-2.0.4/.pylintrc` & `adafruit-circuitpython-onewire-2.0.5/.pylintrc`

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

### Comparing `adafruit-circuitpython-onewire-2.0.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-onewire-2.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/LICENSE` & `adafruit-circuitpython-onewire-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-onewire-2.0.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/LICENSES/MIT.txt` & `adafruit-circuitpython-onewire-2.0.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-onewire-2.0.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/PKG-INFO` & `adafruit-circuitpython-onewire-2.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-onewire
-Version: 2.0.4
+Version: 2.0.5
 Summary: CircuitPython OneWire helper library for 1-wire bus devices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_OneWire
 Keywords: adafruit,onewire,dallas,1-wire,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-onewire-2.0.4/README.rst` & `adafruit-circuitpython-onewire-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/adafruit_circuitpython_onewire.egg-info/PKG-INFO` & `adafruit-circuitpython-onewire-2.0.5/adafruit_circuitpython_onewire.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-onewire
-Version: 2.0.4
+Version: 2.0.5
 Summary: CircuitPython OneWire helper library for 1-wire bus devices.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_OneWire
 Keywords: adafruit,onewire,dallas,1-wire,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-onewire-2.0.4/adafruit_circuitpython_onewire.egg-info/SOURCES.txt` & `adafruit-circuitpython-onewire-2.0.5/adafruit_circuitpython_onewire.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/adafruit_onewire/bus.py` & `adafruit-circuitpython-onewire-2.0.5/adafruit_onewire/bus.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ====================================================
 
 Provide access to a 1-Wire bus.
 
 * Author(s): Carter Nelson
 """
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_OneWire.git"
 
 import onewireio
 from micropython import const
 
 try:
     from typing import Optional, List, Tuple
```

### Comparing `adafruit-circuitpython-onewire-2.0.4/adafruit_onewire/device.py` & `adafruit-circuitpython-onewire-2.0.5/adafruit_onewire/device.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ====================================================
 
 Provides access to a single device on the 1-Wire bus.
 
 * Author(s): Carter Nelson
 """
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_OneWire.git"
 
 try:
     from typing import Optional, Type
     from circuitpython_typing import ReadableBuffer, WriteableBuffer
     from types import TracebackType
     from adafruit_onewire.bus import OneWireBus, OneWireAddress
```

### Comparing `adafruit-circuitpython-onewire-2.0.4/docs/_static/favicon.ico` & `adafruit-circuitpython-onewire-2.0.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/docs/conf.py` & `adafruit-circuitpython-onewire-2.0.5/docs/conf.py`

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

### Comparing `adafruit-circuitpython-onewire-2.0.4/docs/index.rst` & `adafruit-circuitpython-onewire-2.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/examples/onewire_simpletest.py` & `adafruit-circuitpython-onewire-2.0.5/examples/onewire_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-onewire-2.0.4/pyproject.toml` & `adafruit-circuitpython-onewire-2.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-onewire"
 description = "CircuitPython OneWire helper library for 1-wire bus devices."
-version = "2.0.4"
+version = "2.0.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_OneWire"}
 keywords = [
     "adafruit",
```

