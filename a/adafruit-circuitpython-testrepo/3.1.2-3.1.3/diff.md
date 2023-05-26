# Comparing `tmp/adafruit-circuitpython-testrepo-3.1.2.tar.gz` & `tmp/adafruit-circuitpython-testrepo-3.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-testrepo-3.1.2.tar", last modified: Fri Jan 20 02:36:55 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-testrepo-3.1.3.tar", last modified: Fri May 26 16:24:12 2023, max compression
```

## Comparing `adafruit-circuitpython-testrepo-3.1.2.tar` & `adafruit-circuitpython-testrepo-3.1.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.407532 adafruit-circuitpython-testrepo-3.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.411532 adafruit-circuitpython-testrepo-3.1.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.411532 adafruit-circuitpython-testrepo-3.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.patch-test-file
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.411532 adafruit-circuitpython-testrepo-3.1.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/adafruit_circuitpython_testrepo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-01-20 02:36:55.000000 adafruit-circuitpython-testrepo-3.1.2/adafruit_circuitpython_testrepo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-01-20 02:36:55.000000 adafruit-circuitpython-testrepo-3.1.2/adafruit_circuitpython_testrepo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 02:36:55.000000 adafruit-circuitpython-testrepo-3.1.2/adafruit_circuitpython_testrepo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-01-20 02:36:55.000000 adafruit-circuitpython-testrepo-3.1.2/adafruit_circuitpython_testrepo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-20 02:36:55.000000 adafruit-circuitpython-testrepo-3.1.2/adafruit_circuitpython_testrepo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-01-20 02:36:47.000000 adafruit-circuitpython-testrepo-3.1.2/adafruit_testrepo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5447 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-01-20 02:36:47.000000 adafruit-circuitpython-testrepo-3.1.2/examples/testrepo_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-01-20 02:36:47.000000 adafruit-circuitpython-testrepo-3.1.2/examples/testrepo_simpletest_two.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/examples/testrepo_test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:47.000000 adafruit-circuitpython-testrepo-3.1.2/examples/testrepo_test/thing.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-01-20 02:36:47.000000 adafruit-circuitpython-testrepo-3.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-20 02:36:40.000000 adafruit-circuitpython-testrepo-3.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 02:36:55.415531 adafruit-circuitpython-testrepo-3.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-01-20 02:36:47.000000 adafruit-circuitpython-testrepo-3.1.2/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.013700 adafruit-circuitpython-testrepo-3.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.005700 adafruit-circuitpython-testrepo-3.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.009700 adafruit-circuitpython-testrepo-3.1.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.009700 adafruit-circuitpython-testrepo-3.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.patch-test-file
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.009700 adafruit-circuitpython-testrepo-3.1.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-26 16:24:12.013700 adafruit-circuitpython-testrepo-3.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.009700 adafruit-circuitpython-testrepo-3.1.3/adafruit_circuitpython_testrepo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-26 16:24:11.000000 adafruit-circuitpython-testrepo-3.1.3/adafruit_circuitpython_testrepo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-26 16:24:12.000000 adafruit-circuitpython-testrepo-3.1.3/adafruit_circuitpython_testrepo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:24:11.000000 adafruit-circuitpython-testrepo-3.1.3/adafruit_circuitpython_testrepo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-26 16:24:11.000000 adafruit-circuitpython-testrepo-3.1.3/adafruit_circuitpython_testrepo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:24:11.000000 adafruit-circuitpython-testrepo-3.1.3/adafruit_circuitpython_testrepo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-05-26 16:24:03.000000 adafruit-circuitpython-testrepo-3.1.3/adafruit_testrepo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.013700 adafruit-circuitpython-testrepo-3.1.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.013700 adafruit-circuitpython-testrepo-3.1.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.013700 adafruit-circuitpython-testrepo-3.1.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-26 16:24:03.000000 adafruit-circuitpython-testrepo-3.1.3/examples/testrepo_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-26 16:24:03.000000 adafruit-circuitpython-testrepo-3.1.3/examples/testrepo_simpletest_two.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.013700 adafruit-circuitpython-testrepo-3.1.3/examples/testrepo_test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:03.000000 adafruit-circuitpython-testrepo-3.1.3/examples/testrepo_test/thing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-05-26 16:24:03.000000 adafruit-circuitpython-testrepo-3.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-26 16:23:51.000000 adafruit-circuitpython-testrepo-3.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:24:12.013700 adafruit-circuitpython-testrepo-3.1.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:12.013700 adafruit-circuitpython-testrepo-3.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 16:24:03.000000 adafruit-circuitpython-testrepo-3.1.3/tests/test.py
```

### Comparing `adafruit-circuitpython-testrepo-3.1.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-testrepo-3.1.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/.gitignore` & `adafruit-circuitpython-testrepo-3.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/.pre-commit-config.yaml` & `adafruit-circuitpython-testrepo-3.1.3/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

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
           - --disable=consider-using-f-string,duplicate-code
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-testrepo-3.1.2/.pylintrc` & `adafruit-circuitpython-testrepo-3.1.3/.pylintrc`

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

### Comparing `adafruit-circuitpython-testrepo-3.1.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-testrepo-3.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/LICENSE` & `adafruit-circuitpython-testrepo-3.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-testrepo-3.1.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/LICENSES/MIT.txt` & `adafruit-circuitpython-testrepo-3.1.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-testrepo-3.1.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/PKG-INFO` & `adafruit-circuitpython-testrepo-3.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-testrepo
-Version: 3.1.2
+Version: 3.1.3
 Summary: CircuitPython test library
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TestRepo
 Keywords: adafruit,blinka,circuitpython,micropython,test
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-testrepo-3.1.2/README.rst` & `adafruit-circuitpython-testrepo-3.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/adafruit_circuitpython_testrepo.egg-info/PKG-INFO` & `adafruit-circuitpython-testrepo-3.1.3/adafruit_circuitpython_testrepo.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-testrepo
-Version: 3.1.2
+Version: 3.1.3
 Summary: CircuitPython test library
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TestRepo
 Keywords: adafruit,blinka,circuitpython,micropython,test
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-testrepo-3.1.2/adafruit_circuitpython_testrepo.egg-info/SOURCES.txt` & `adafruit-circuitpython-testrepo-3.1.3/adafruit_circuitpython_testrepo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/adafruit_testrepo.py` & `adafruit-circuitpython-testrepo-3.1.3/adafruit_testrepo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/docs/_static/favicon.ico` & `adafruit-circuitpython-testrepo-3.1.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/docs/conf.py` & `adafruit-circuitpython-testrepo-3.1.3/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
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

### Comparing `adafruit-circuitpython-testrepo-3.1.2/docs/index.rst` & `adafruit-circuitpython-testrepo-3.1.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-testrepo-3.1.2/pyproject.toml` & `adafruit-circuitpython-testrepo-3.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-testrepo"
 description = "CircuitPython test library"
-version = "3.1.2"
+version = "3.1.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_TestRepo"}
 keywords = [
     "adafruit",
```

