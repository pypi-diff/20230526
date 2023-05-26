# Comparing `tmp/adafruit-circuitpython-tca9548a-0.7.0.tar.gz` & `tmp/adafruit-circuitpython-tca9548a-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tca9548a-0.7.0.tar", last modified: Mon Jan 23 20:41:52 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-tca9548a-0.7.1.tar", last modified: Fri May 26 16:23:50 2023, max compression
```

## Comparing `adafruit-circuitpython-tca9548a-0.7.0.tar` & `adafruit-circuitpython-tca9548a-0.7.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.981525 adafruit-circuitpython-tca9548a-0.7.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.973524 adafruit-circuitpython-tca9548a-0.7.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.977525 adafruit-circuitpython-tca9548a-0.7.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.977525 adafruit-circuitpython-tca9548a-0.7.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.977525 adafruit-circuitpython-tca9548a-0.7.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-01-23 20:41:52.981525 adafruit-circuitpython-tca9548a-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.981525 adafruit-circuitpython-tca9548a-0.7.0/adafruit_circuitpython_tca9548a.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-01-23 20:41:52.000000 adafruit-circuitpython-tca9548a-0.7.0/adafruit_circuitpython_tca9548a.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-01-23 20:41:52.000000 adafruit-circuitpython-tca9548a-0.7.0/adafruit_circuitpython_tca9548a.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 20:41:52.000000 adafruit-circuitpython-tca9548a-0.7.0/adafruit_circuitpython_tca9548a.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-01-23 20:41:52.000000 adafruit-circuitpython-tca9548a-0.7.0/adafruit_circuitpython_tca9548a.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-23 20:41:52.000000 adafruit-circuitpython-tca9548a-0.7.0/adafruit_circuitpython_tca9548a.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-01-23 20:41:43.000000 adafruit-circuitpython-tca9548a-0.7.0/adafruit_tca9548a.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.981525 adafruit-circuitpython-tca9548a-0.7.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.981525 adafruit-circuitpython-tca9548a-0.7.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 20:41:52.981525 adafruit-circuitpython-tca9548a-0.7.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-23 20:41:43.000000 adafruit-circuitpython-tca9548a-0.7.0/examples/pca9546a_multisensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-01-23 20:41:43.000000 adafruit-circuitpython-tca9548a-0.7.0/examples/pca9546a_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-01-23 20:41:43.000000 adafruit-circuitpython-tca9548a-0.7.0/examples/tca9548a_multisensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-01-23 20:41:43.000000 adafruit-circuitpython-tca9548a-0.7.0/examples/tca9548a_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-23 20:41:43.000000 adafruit-circuitpython-tca9548a-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-01-23 20:41:34.000000 adafruit-circuitpython-tca9548a-0.7.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 20:41:52.981525 adafruit-circuitpython-tca9548a-0.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.696739 adafruit-circuitpython-tca9548a-0.7.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.688738 adafruit-circuitpython-tca9548a-0.7.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.692738 adafruit-circuitpython-tca9548a-0.7.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.692738 adafruit-circuitpython-tca9548a-0.7.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.692738 adafruit-circuitpython-tca9548a-0.7.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-26 16:23:50.696739 adafruit-circuitpython-tca9548a-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3171 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.696739 adafruit-circuitpython-tca9548a-0.7.1/adafruit_circuitpython_tca9548a.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-05-26 16:23:50.000000 adafruit-circuitpython-tca9548a-0.7.1/adafruit_circuitpython_tca9548a.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 16:23:50.000000 adafruit-circuitpython-tca9548a-0.7.1/adafruit_circuitpython_tca9548a.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:23:50.000000 adafruit-circuitpython-tca9548a-0.7.1/adafruit_circuitpython_tca9548a.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 16:23:50.000000 adafruit-circuitpython-tca9548a-0.7.1/adafruit_circuitpython_tca9548a.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:23:50.000000 adafruit-circuitpython-tca9548a-0.7.1/adafruit_circuitpython_tca9548a.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-05-26 16:23:41.000000 adafruit-circuitpython-tca9548a-0.7.1/adafruit_tca9548a.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.696739 adafruit-circuitpython-tca9548a-0.7.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.696739 adafruit-circuitpython-tca9548a-0.7.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5794 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1176 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:50.696739 adafruit-circuitpython-tca9548a-0.7.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 16:23:41.000000 adafruit-circuitpython-tca9548a-0.7.1/examples/pca9546a_multisensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 16:23:41.000000 adafruit-circuitpython-tca9548a-0.7.1/examples/pca9546a_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-26 16:23:41.000000 adafruit-circuitpython-tca9548a-0.7.1/examples/tca9548a_multisensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 16:23:41.000000 adafruit-circuitpython-tca9548a-0.7.1/examples/tca9548a_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-26 16:23:41.000000 adafruit-circuitpython-tca9548a-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-26 16:23:29.000000 adafruit-circuitpython-tca9548a-0.7.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:23:50.696739 adafruit-circuitpython-tca9548a-0.7.1/setup.cfg
```

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tca9548a-0.7.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/.gitignore` & `adafruit-circuitpython-tca9548a-0.7.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/.pre-commit-config.yaml` & `adafruit-circuitpython-tca9548a-0.7.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/.pylintrc` & `adafruit-circuitpython-tca9548a-0.7.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tca9548a-0.7.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/LICENSE` & `adafruit-circuitpython-tca9548a-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tca9548a-0.7.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/LICENSES/MIT.txt` & `adafruit-circuitpython-tca9548a-0.7.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tca9548a-0.7.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/PKG-INFO` & `adafruit-circuitpython-tca9548a-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tca9548a
-Version: 0.7.0
+Version: 0.7.1
 Summary: CircuitPython driver for the TCA9548A I2C Multiplexer.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TCA9548A
 Keywords: adafruit,tca9548a,i2c,multiplexer,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/README.rst` & `adafruit-circuitpython-tca9548a-0.7.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/adafruit_circuitpython_tca9548a.egg-info/PKG-INFO` & `adafruit-circuitpython-tca9548a-0.7.1/adafruit_circuitpython_tca9548a.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tca9548a
-Version: 0.7.0
+Version: 0.7.1
 Summary: CircuitPython driver for the TCA9548A I2C Multiplexer.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TCA9548A
 Keywords: adafruit,tca9548a,i2c,multiplexer,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/adafruit_circuitpython_tca9548a.egg-info/SOURCES.txt` & `adafruit-circuitpython-tca9548a-0.7.1/adafruit_circuitpython_tca9548a.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/adafruit_tca9548a.py` & `adafruit-circuitpython-tca9548a-0.7.1/adafruit_tca9548a.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     from circuitpython_typing import WriteableBuffer, ReadableBuffer
     from busio import I2C
 except ImportError:
     pass
 
 _DEFAULT_ADDRESS = const(0x70)
 
-__version__ = "0.7.0"
+__version__ = "0.7.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TCA9548A.git"
 
 
 class TCA9548A_Channel:
     """Helper class to represent an output channel on the TCA9548A and take care
     of the necessary I2C commands for channel switching. This class needs to
     behave like an I2CDevice."""
```

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/docs/_static/favicon.ico` & `adafruit-circuitpython-tca9548a-0.7.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/docs/conf.py` & `adafruit-circuitpython-tca9548a-0.7.1/docs/conf.py`

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

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/docs/index.rst` & `adafruit-circuitpython-tca9548a-0.7.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/examples/pca9546a_multisensor.py` & `adafruit-circuitpython-tca9548a-0.7.1/examples/pca9546a_multisensor.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/examples/pca9546a_simpletest.py` & `adafruit-circuitpython-tca9548a-0.7.1/examples/pca9546a_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/examples/tca9548a_multisensor.py` & `adafruit-circuitpython-tca9548a-0.7.1/examples/tca9548a_multisensor.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/examples/tca9548a_simpletest.py` & `adafruit-circuitpython-tca9548a-0.7.1/examples/tca9548a_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tca9548a-0.7.0/pyproject.toml` & `adafruit-circuitpython-tca9548a-0.7.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-tca9548a"
 description = "CircuitPython driver for the TCA9548A I2C Multiplexer."
-version = "0.7.0"
+version = "0.7.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_TCA9548A"}
 keywords = [
     "adafruit",
```

