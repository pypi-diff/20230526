# Comparing `tmp/adafruit-circuitpython-lc709203f-2.3.0.tar.gz` & `tmp/adafruit-circuitpython-lc709203f-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lc709203f-2.3.0.tar", last modified: Mon May  1 13:48:40 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-lc709203f-2.3.1.tar", last modified: Fri May 26 16:25:22 2023, max compression
```

## Comparing `adafruit-circuitpython-lc709203f-2.3.0.tar` & `adafruit-circuitpython-lc709203f-2.3.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.563719 adafruit-circuitpython-lc709203f-2.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.563719 adafruit-circuitpython-lc709203f-2.3.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.563719 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.563719 adafruit-circuitpython-lc709203f-2.3.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-01 13:48:40.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-01 13:48:33.000000 adafruit-circuitpython-lc709203f-2.3.0/adafruit_lc709203f.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5897 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-01 13:48:33.000000 adafruit-circuitpython-lc709203f-2.3.0/examples/lc709203f_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-01 13:48:33.000000 adafruit-circuitpython-lc709203f-2.3.0/examples/lc709203f_thermistortest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-01 13:48:33.000000 adafruit-circuitpython-lc709203f-2.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-01 13:48:24.000000 adafruit-circuitpython-lc709203f-2.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 13:48:40.567719 adafruit-circuitpython-lc709203f-2.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.528039 adafruit-circuitpython-lc709203f-2.3.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/adafruit_circuitpython_lc709203f.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-26 16:25:22.000000 adafruit-circuitpython-lc709203f-2.3.1/adafruit_circuitpython_lc709203f.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 16:25:22.000000 adafruit-circuitpython-lc709203f-2.3.1/adafruit_circuitpython_lc709203f.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:25:22.000000 adafruit-circuitpython-lc709203f-2.3.1/adafruit_circuitpython_lc709203f.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-26 16:25:22.000000 adafruit-circuitpython-lc709203f-2.3.1/adafruit_circuitpython_lc709203f.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 16:25:22.000000 adafruit-circuitpython-lc709203f-2.3.1/adafruit_circuitpython_lc709203f.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9782 2023-05-26 16:25:13.000000 adafruit-circuitpython-lc709203f-2.3.1/adafruit_lc709203f.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5925 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-26 16:25:13.000000 adafruit-circuitpython-lc709203f-2.3.1/examples/lc709203f_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-26 16:25:13.000000 adafruit-circuitpython-lc709203f-2.3.1/examples/lc709203f_thermistortest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 16:25:13.000000 adafruit-circuitpython-lc709203f-2.3.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-26 16:24:59.000000 adafruit-circuitpython-lc709203f-2.3.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:25:22.532039 adafruit-circuitpython-lc709203f-2.3.1/setup.cfg
```

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-lc709203f-2.3.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/.gitignore` & `adafruit-circuitpython-lc709203f-2.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/.pre-commit-config.yaml` & `adafruit-circuitpython-lc709203f-2.3.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/.pylintrc` & `adafruit-circuitpython-lc709203f-2.3.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lc709203f-2.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/LICENSE` & `adafruit-circuitpython-lc709203f-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lc709203f-2.3.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/LICENSES/MIT.txt` & `adafruit-circuitpython-lc709203f-2.3.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lc709203f-2.3.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/PKG-INFO` & `adafruit-circuitpython-lc709203f-2.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lc709203f
-Version: 2.3.0
+Version: 2.3.1
 Summary: Library for I2C LC709203F battery status and fuel gauge
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LC709203F
 Keywords: adafruit,blinka,circuitpython,micropython,lc709203f,battery,lipoly,status,fuel,gauge,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/README.rst` & `adafruit-circuitpython-lc709203f-2.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/PKG-INFO` & `adafruit-circuitpython-lc709203f-2.3.1/adafruit_circuitpython_lc709203f.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lc709203f
-Version: 2.3.0
+Version: 2.3.1
 Summary: Library for I2C LC709203F battery status and fuel gauge
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LC709203F
 Keywords: adafruit,blinka,circuitpython,micropython,lc709203f,battery,lipoly,status,fuel,gauge,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/adafruit_circuitpython_lc709203f.egg-info/SOURCES.txt` & `adafruit-circuitpython-lc709203f-2.3.1/adafruit_circuitpython_lc709203f.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/adafruit_lc709203f.py` & `adafruit-circuitpython-lc709203f-2.3.1/adafruit_lc709203f.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
     from typing import Iterable, Optional, Tuple
     from typing_extensions import Literal
     from circuitpython_typing import ReadableBuffer
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "2.3.0"
+__version__ = "2.3.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LC709203F.git"
 
 LC709203F_I2CADDR_DEFAULT = const(0x0B)
 LC709203F_CMD_ICVERSION = const(0x11)
 LC709203F_CMD_BATTPROF = const(0x12)
 LC709203F_CMD_POWERMODE = const(0x15)
 LC709203F_CMD_APA = const(0x0B)
```

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/docs/_static/favicon.ico` & `adafruit-circuitpython-lc709203f-2.3.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/docs/conf.py` & `adafruit-circuitpython-lc709203f-2.3.1/docs/conf.py`

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

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/docs/index.rst` & `adafruit-circuitpython-lc709203f-2.3.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/examples/lc709203f_simpletest.py` & `adafruit-circuitpython-lc709203f-2.3.1/examples/lc709203f_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/examples/lc709203f_thermistortest.py` & `adafruit-circuitpython-lc709203f-2.3.1/examples/lc709203f_thermistortest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lc709203f-2.3.0/pyproject.toml` & `adafruit-circuitpython-lc709203f-2.3.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-lc709203f"
 description = "Library for I2C LC709203F battery status and fuel gauge"
-version = "2.3.0"
+version = "2.3.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LC709203F"}
 keywords = [
     "adafruit",
```

