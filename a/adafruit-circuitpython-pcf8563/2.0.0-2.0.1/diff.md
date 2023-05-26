# Comparing `tmp/adafruit-circuitpython-pcf8563-2.0.0.tar.gz` & `tmp/adafruit-circuitpython-pcf8563-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pcf8563-2.0.0.tar", last modified: Fri Apr 28 23:36:27 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-pcf8563-2.0.1.tar", last modified: Fri May 26 16:26:56 2023, max compression
```

## Comparing `adafruit-circuitpython-pcf8563-2.0.0.tar` & `adafruit-circuitpython-pcf8563-2.0.1.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.639472 adafruit-circuitpython-pcf8563-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.639472 adafruit-circuitpython-pcf8563-2.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.639472 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-28 23:36:27.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/pcf8563.py
--rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/api.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)    10797 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/examples/pcf8563_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-28 23:36:19.000000 adafruit-circuitpython-pcf8563-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 23:36:03.000000 adafruit-circuitpython-pcf8563-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:36:27.643472 adafruit-circuitpython-pcf8563-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.361651 adafruit-circuitpython-pcf8563-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.361651 adafruit-circuitpython-pcf8563-2.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    17023 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4846 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/adafruit_circuitpython_pcf8563.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-05-26 16:26:56.000000 adafruit-circuitpython-pcf8563-2.0.1/adafruit_circuitpython_pcf8563.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 16:26:56.000000 adafruit-circuitpython-pcf8563-2.0.1/adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:26:56.000000 adafruit-circuitpython-pcf8563-2.0.1/adafruit_circuitpython_pcf8563.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:26:56.000000 adafruit-circuitpython-pcf8563-2.0.1/adafruit_circuitpython_pcf8563.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:26:56.000000 adafruit-circuitpython-pcf8563-2.0.1/adafruit_circuitpython_pcf8563.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/adafruit_pcf8563/
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-05-26 16:26:48.000000 adafruit-circuitpython-pcf8563-2.0.1/adafruit_pcf8563/clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-26 16:26:48.000000 adafruit-circuitpython-pcf8563-2.0.1/adafruit_pcf8563/pcf8563.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3612 2023-05-26 16:26:48.000000 adafruit-circuitpython-pcf8563-2.0.1/adafruit_pcf8563/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/api.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-26 16:26:48.000000 adafruit-circuitpython-pcf8563-2.0.1/examples/pcf8563_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-26 16:26:48.000000 adafruit-circuitpython-pcf8563-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:26:38.000000 adafruit-circuitpython-pcf8563-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:26:56.365651 adafruit-circuitpython-pcf8563-2.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pcf8563-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/.gitignore` & `adafruit-circuitpython-pcf8563-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-pcf8563-2.0.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/.pylintrc` & `adafruit-circuitpython-pcf8563-2.0.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pcf8563-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/LICENSE` & `adafruit-circuitpython-pcf8563-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pcf8563-2.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-pcf8563-2.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pcf8563-2.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/PKG-INFO` & `adafruit-circuitpython-pcf8563-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcf8563
-Version: 2.0.0
+Version: 2.0.1
 Summary: CircuitPython library for PCF8563 real time clock.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PCF8563
 Keywords: adafruit,pcf8563,real,time,clock,rtc,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/README.rst` & `adafruit-circuitpython-pcf8563-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/PKG-INFO` & `adafruit-circuitpython-pcf8563-2.0.1/adafruit_circuitpython_pcf8563.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcf8563
-Version: 2.0.0
+Version: 2.0.1
 Summary: CircuitPython library for PCF8563 real time clock.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PCF8563
 Keywords: adafruit,pcf8563,real,time,clock,rtc,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt` & `adafruit-circuitpython-pcf8563-2.0.1/adafruit_circuitpython_pcf8563.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/clock.py` & `adafruit-circuitpython-pcf8563-2.0.1/adafruit_pcf8563/clock.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 **Notes:**
 
 #. Datasheet: http://cache.nxp.com/documents/data_sheet/PCF8563.pdf
 """
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PCF8563.git"
 
 import time
 
 from adafruit_bus_device.i2c_device import I2CDevice
 from adafruit_register import i2c_bit
 from adafruit_register import i2c_bits
```

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/pcf8563.py` & `adafruit-circuitpython-pcf8563-2.0.1/adafruit_pcf8563/pcf8563.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 #. Milliseconds are not supported by this RTC.
 #. The alarm does not support seconds. It will always fire on full minutes.
 #. This RTC has a single timer. The class Timer implements the interface to timer-specfic registers.
 #. The class Clock implements the configuration of the clkout-pin.
 #. Datasheet: http://cache.nxp.com/documents/data_sheet/PCF8563.pdf
 """
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PCF8563.git"
 
 import time
 
 from adafruit_bus_device.i2c_device import I2CDevice
 from adafruit_register import i2c_bit
 from adafruit_register import i2c_bcd_alarm
```

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/adafruit_pcf8563/timer.py` & `adafruit-circuitpython-pcf8563-2.0.1/adafruit_pcf8563/timer.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 **Notes:**
 
 #. Datasheet: http://cache.nxp.com/documents/data_sheet/PCF8563.pdf
 """
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PCF8563.git"
 
 import time
 
 from adafruit_bus_device.i2c_device import I2CDevice
 from adafruit_register import i2c_bit
 from adafruit_register import i2c_bits
```

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-pcf8563-2.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/docs/conf.py` & `adafruit-circuitpython-pcf8563-2.0.1/docs/conf.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,20 @@
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
-extensions = ["sphinx.ext.autodoc", "sphinx.ext.todo", "sphinx.ext.intersphinx"]
+extensions = [
+    "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
+    "sphinx.ext.todo",
+    "sphinx.ext.intersphinx",
+]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 autodoc_mock_imports = ["adafruit_bus_device", "adafruit_register"]
 
 # Add any paths that contain templates here, relative to this directory.
```

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/docs/index.rst` & `adafruit-circuitpython-pcf8563-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/examples/pcf8563_simpletest.py` & `adafruit-circuitpython-pcf8563-2.0.1/examples/pcf8563_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8563-2.0.0/pyproject.toml` & `adafruit-circuitpython-pcf8563-2.0.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pcf8563"
 description = "CircuitPython library for PCF8563 real time clock."
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_PCF8563"}
 keywords = [
     "adafruit",
```

