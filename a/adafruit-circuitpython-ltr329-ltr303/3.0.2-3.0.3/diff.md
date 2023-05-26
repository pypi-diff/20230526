# Comparing `tmp/adafruit-circuitpython-ltr329-ltr303-3.0.2.tar.gz` & `tmp/adafruit-circuitpython-ltr329-ltr303-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ltr329-ltr303-3.0.2.tar", last modified: Mon Nov 28 18:10:23 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ltr329-ltr303-3.0.3.tar", last modified: Fri May 26 15:57:26 2023, max compression
```

## Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2.tar` & `adafruit-circuitpython-ltr329-ltr303-3.0.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.649791 adafruit-circuitpython-ltr329-ltr303-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.641790 adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.645790 adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.645790 adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.645790 adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4226 2022-11-28 18:10:23.649791 adafruit-circuitpython-ltr329-ltr303-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3431 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.645790 adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_circuitpython_ltr329_ltr303.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4226 2022-11-28 18:10:23.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_circuitpython_ltr329_ltr303.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1093 2022-11-28 18:10:23.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_circuitpython_ltr329_ltr303.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:10:23.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_circuitpython_ltr329_ltr303.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-28 18:10:23.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_circuitpython_ltr329_ltr303.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       23 2022-11-28 18:10:23.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_circuitpython_ltr329_ltr303.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     8246 2022-11-28 18:10:14.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_ltr329_ltr303.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.645790 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.645790 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      273 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      186 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1029 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:10:23.645790 adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     3347 2022-11-28 18:10:14.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/ltr303_advancedtest.py
--rw-r--r--   0 runner    (1001) docker     (122)      584 2022-11-28 18:10:14.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/ltr303_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)     2556 2022-11-28 18:10:14.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/ltr329_advancedtest.py
--rw-r--r--   0 runner    (1001) docker     (122)      584 2022-11-28 18:10:14.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/ltr329_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2022-11-28 18:10:14.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      272 2022-11-28 18:10:05.000000 adafruit-circuitpython-ltr329-ltr303-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:10:23.649791 adafruit-circuitpython-ltr329-ltr303-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.451299 adafruit-circuitpython-ltr329-ltr303-3.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.447299 adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.447299 adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.447299 adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.447299 adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-26 15:57:26.451299 adafruit-circuitpython-ltr329-ltr303-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.447299 adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_circuitpython_ltr329_ltr303.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4226 2023-05-26 15:57:26.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_circuitpython_ltr329_ltr303.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-26 15:57:26.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_circuitpython_ltr329_ltr303.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:57:26.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_circuitpython_ltr329_ltr303.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 15:57:26.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_circuitpython_ltr329_ltr303.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 15:57:26.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_circuitpython_ltr329_ltr303.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8246 2023-05-26 15:57:19.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_ltr329_ltr303.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.451299 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.451299 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:26.451299 adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-26 15:57:19.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/ltr303_advancedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-26 15:57:19.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/ltr303_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-26 15:57:19.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/ltr329_advancedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-26 15:57:19.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/ltr329_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-26 15:57:19.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 15:57:10.000000 adafruit-circuitpython-ltr329-ltr303-3.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:57:26.451299 adafruit-circuitpython-ltr329-ltr303-3.0.3/setup.cfg
```

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/.gitignore` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/.gitignore`

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

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/.pre-commit-config.yaml` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/.pylintrc` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/.pylintrc`

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

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSE` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSES/MIT.txt` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/PKG-INFO` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ltr329-ltr303
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python driver for LTR-329/303 light sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LTR329_LTR303
 Keywords: adafruit,blinka,circuitpython,micropython,ltr329,LTR-329,LTR329,LTR-303,ltr303,LRT303,light,lux,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/README.rst` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_circuitpython_ltr329_ltr303.egg-info/PKG-INFO` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_circuitpython_ltr329_ltr303.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ltr329-ltr303
-Version: 3.0.2
+Version: 3.0.3
 Summary: Python driver for LTR-329/303 light sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LTR329_LTR303
 Keywords: adafruit,blinka,circuitpython,micropython,ltr329,LTR-329,LTR329,LTR-303,ltr303,LRT303,light,lux,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_circuitpython_ltr329_ltr303.egg-info/SOURCES.txt` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_circuitpython_ltr329_ltr303.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/adafruit_ltr329_ltr303.py` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/adafruit_ltr329_ltr303.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 try:
     from typing import Tuple
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LTR329_LTR303.git"
 
 _LTR329_I2CADDR_DEFAULT: int = const(0x29)  # Default I2C address
 
 # These registers on both LTR-329 and LTR-303
 _LTR329_REG_ALS_CONTR = const(0x80)
 _LTR329_REG_ALS_MEASRATE = const(0x85)
```

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/_static/favicon.ico` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/conf.py` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/conf.py`

 * *Files 1% similar despite different names*

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

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/docs/index.rst` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/ltr303_advancedtest.py` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/ltr303_advancedtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/ltr303_simpletest.py` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/ltr303_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/ltr329_advancedtest.py` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/ltr329_advancedtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/examples/ltr329_simpletest.py` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/examples/ltr329_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ltr329-ltr303-3.0.2/pyproject.toml` & `adafruit-circuitpython-ltr329-ltr303-3.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ltr329-ltr303"
 description = "Python driver for LTR-329/303 light sensors"
-version = "3.0.2"
+version = "3.0.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LTR329_LTR303"}
 keywords = [
     "adafruit",
```

