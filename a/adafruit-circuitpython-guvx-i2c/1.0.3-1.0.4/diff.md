# Comparing `tmp/adafruit-circuitpython-guvx-i2c-1.0.3.tar.gz` & `tmp/adafruit-circuitpython-guvx-i2c-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-guvx-i2c-1.0.3.tar", last modified: Mon Nov 28 18:12:47 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-guvx-i2c-1.0.4.tar", last modified: Fri May 26 15:57:56 2023, max compression
```

## Comparing `adafruit-circuitpython-guvx-i2c-1.0.3.tar` & `adafruit-circuitpython-guvx-i2c-1.0.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.486445 adafruit-circuitpython-guvx-i2c-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.478445 adafruit-circuitpython-guvx-i2c-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.478445 adafruit-circuitpython-guvx-i2c-1.0.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.482445 adafruit-circuitpython-guvx-i2c-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.482445 adafruit-circuitpython-guvx-i2c-1.0.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4225 2022-11-28 18:12:47.486445 adafruit-circuitpython-guvx-i2c-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3436 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.482445 adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_circuitpython_guvx_i2c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4225 2022-11-28 18:12:47.000000 adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_circuitpython_guvx_i2c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1037 2022-11-28 18:12:47.000000 adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_circuitpython_guvx_i2c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:12:47.000000 adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_circuitpython_guvx_i2c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-28 18:12:47.000000 adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_circuitpython_guvx_i2c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2022-11-28 18:12:47.000000 adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_circuitpython_guvx_i2c.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     7996 2022-11-28 18:12:37.000000 adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_guvx_i2c.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.482445 adafruit-circuitpython-guvx-i2c-1.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.482445 adafruit-circuitpython-guvx-i2c-1.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      268 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      192 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1031 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:12:47.486445 adafruit-circuitpython-guvx-i2c-1.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      975 2022-11-28 18:12:37.000000 adafruit-circuitpython-guvx-i2c-1.0.3/examples/guva_c32sm_fulltest.py
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2022-11-28 18:12:37.000000 adafruit-circuitpython-guvx-i2c-1.0.3/examples/guvb_c31sm_fulltest.py
--rw-r--r--   0 runner    (1001) docker     (122)      502 2022-11-28 18:12:37.000000 adafruit-circuitpython-guvx-i2c-1.0.3/examples/guvb_c31sm_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      142 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1585 2022-11-28 18:12:37.000000 adafruit-circuitpython-guvx-i2c-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      272 2022-11-28 18:12:27.000000 adafruit-circuitpython-guvx-i2c-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:12:47.486445 adafruit-circuitpython-guvx-i2c-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.808317 adafruit-circuitpython-guvx-i2c-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.800317 adafruit-circuitpython-guvx-i2c-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.800317 adafruit-circuitpython-guvx-i2c-1.0.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.800317 adafruit-circuitpython-guvx-i2c-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.804317 adafruit-circuitpython-guvx-i2c-1.0.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-26 15:57:56.808317 adafruit-circuitpython-guvx-i2c-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.804317 adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_circuitpython_guvx_i2c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4225 2023-05-26 15:57:56.000000 adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_circuitpython_guvx_i2c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-26 15:57:56.000000 adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_circuitpython_guvx_i2c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:57:56.000000 adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_circuitpython_guvx_i2c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 15:57:56.000000 adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_circuitpython_guvx_i2c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 15:57:56.000000 adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_circuitpython_guvx_i2c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-05-26 15:57:47.000000 adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_guvx_i2c.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.804317 adafruit-circuitpython-guvx-i2c-1.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.804317 adafruit-circuitpython-guvx-i2c-1.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:56.804317 adafruit-circuitpython-guvx-i2c-1.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-26 15:57:47.000000 adafruit-circuitpython-guvx-i2c-1.0.4/examples/guva_c32sm_fulltest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-26 15:57:47.000000 adafruit-circuitpython-guvx-i2c-1.0.4/examples/guvb_c31sm_fulltest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-26 15:57:47.000000 adafruit-circuitpython-guvx-i2c-1.0.4/examples/guvb_c31sm_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-26 15:57:47.000000 adafruit-circuitpython-guvx-i2c-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 15:57:36.000000 adafruit-circuitpython-guvx-i2c-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:57:56.808317 adafruit-circuitpython-guvx-i2c-1.0.4/setup.cfg
```

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-guvx-i2c-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/.gitignore` & `adafruit-circuitpython-guvx-i2c-1.0.4/.gitignore`

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

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/.pre-commit-config.yaml` & `adafruit-circuitpython-guvx-i2c-1.0.4/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/.pylintrc` & `adafruit-circuitpython-guvx-i2c-1.0.4/.pylintrc`

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

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-guvx-i2c-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/LICENSE` & `adafruit-circuitpython-guvx-i2c-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-guvx-i2c-1.0.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/LICENSES/MIT.txt` & `adafruit-circuitpython-guvx-i2c-1.0.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-guvx-i2c-1.0.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/PKG-INFO` & `adafruit-circuitpython-guvx-i2c-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-guvx-i2c
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python drivers for the GUVA-C32SM and GUVB-C31SM I2C UV sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_GUVX_I2C
 Keywords: adafruit,blinka,circuitpython,micropython,guvx_i2c,UVA,UVB,Python,driver,I2C,GUVA,GUVB
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/README.rst` & `adafruit-circuitpython-guvx-i2c-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_circuitpython_guvx_i2c.egg-info/PKG-INFO` & `adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_circuitpython_guvx_i2c.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-guvx-i2c
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python drivers for the GUVA-C32SM and GUVB-C31SM I2C UV sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_GUVX_I2C
 Keywords: adafruit,blinka,circuitpython,micropython,guvx_i2c,UVA,UVB,Python,driver,I2C,GUVA,GUVB
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_circuitpython_guvx_i2c.egg-info/SOURCES.txt` & `adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_circuitpython_guvx_i2c.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/adafruit_guvx_i2c.py` & `adafruit-circuitpython-guvx-i2c-1.0.4/adafruit_guvx_i2c.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 try:
     import typing  # pylint: disable=unused-import
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_GUVX_I2C.git"
 
 
 _GUVXI2C_I2CADDR_DEFAULT: int = const(0x39)  # Default I2C address
 _GUVXI2C_CHIP_ID = const(0x62)
 
 _GUVXI2C_REG_CHIPID = const(0x00)
```

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/docs/_static/favicon.ico` & `adafruit-circuitpython-guvx-i2c-1.0.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/docs/conf.py` & `adafruit-circuitpython-guvx-i2c-1.0.4/docs/conf.py`

 * *Files 1% similar despite different names*

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

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/docs/index.rst` & `adafruit-circuitpython-guvx-i2c-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/examples/guva_c32sm_fulltest.py` & `adafruit-circuitpython-guvx-i2c-1.0.4/examples/guva_c32sm_fulltest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/examples/guvb_c31sm_fulltest.py` & `adafruit-circuitpython-guvx-i2c-1.0.4/examples/guvb_c31sm_fulltest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-guvx-i2c-1.0.3/pyproject.toml` & `adafruit-circuitpython-guvx-i2c-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-guvx-i2c"
 description = "Python drivers for the GUVA-C32SM and GUVB-C31SM I2C UV sensors"
-version = "1.0.3"
+version = "1.0.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_GUVX_I2C"}
 keywords = [
     "adafruit",
```

