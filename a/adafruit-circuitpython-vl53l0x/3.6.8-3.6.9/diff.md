# Comparing `tmp/adafruit-circuitpython-vl53l0x-3.6.8.tar.gz` & `tmp/adafruit-circuitpython-vl53l0x-3.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-vl53l0x-3.6.8.tar", last modified: Mon Nov 28 18:02:23 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-vl53l0x-3.6.9.tar", last modified: Fri May 26 16:03:53 2023, max compression
```

## Comparing `adafruit-circuitpython-vl53l0x-3.6.8.tar` & `adafruit-circuitpython-vl53l0x-3.6.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.635884 adafruit-circuitpython-vl53l0x-3.6.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.631884 adafruit-circuitpython-vl53l0x-3.6.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.631884 adafruit-circuitpython-vl53l0x-3.6.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.631884 adafruit-circuitpython-vl53l0x-3.6.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1102 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.631884 adafruit-circuitpython-vl53l0x-3.6.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2022-11-28 18:02:23.635884 adafruit-circuitpython-vl53l0x-3.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.631884 adafruit-circuitpython-vl53l0x-3.6.8/adafruit_circuitpython_vl53l0x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3380 2022-11-28 18:02:23.000000 adafruit-circuitpython-vl53l0x-3.6.8/adafruit_circuitpython_vl53l0x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1086 2022-11-28 18:02:23.000000 adafruit-circuitpython-vl53l0x-3.6.8/adafruit_circuitpython_vl53l0x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:02:23.000000 adafruit-circuitpython-vl53l0x-3.6.8/adafruit_circuitpython_vl53l0x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:02:23.000000 adafruit-circuitpython-vl53l0x-3.6.8/adafruit_circuitpython_vl53l0x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:02:23.000000 adafruit-circuitpython-vl53l0x-3.6.8/adafruit_circuitpython_vl53l0x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    26792 2022-11-28 18:02:16.000000 adafruit-circuitpython-vl53l0x-3.6.8/adafruit_vl53l0x.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.635884 adafruit-circuitpython-vl53l0x-3.6.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.635884 adafruit-circuitpython-vl53l0x-3.6.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      126 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5699 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      524 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1081 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:02:23.635884 adafruit-circuitpython-vl53l0x-3.6.8/examples/
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2022-11-28 18:02:16.000000 adafruit-circuitpython-vl53l0x-3.6.8/examples/vl53l0x_multiple_sensors.py
--rw-r--r--   0 runner    (1001) docker     (122)     4252 2022-11-28 18:02:16.000000 adafruit-circuitpython-vl53l0x-3.6.8/examples/vl53l0x_multiple_sensors_continuous.py
--rw-r--r--   0 runner    (1001) docker     (122)     1589 2022-11-28 18:02:16.000000 adafruit-circuitpython-vl53l0x-3.6.8/examples/vl53l0x_simplecontinuous.py
--rw-r--r--   0 runner    (1001) docker     (122)      998 2022-11-28 18:02:16.000000 adafruit-circuitpython-vl53l0x-3.6.8/examples/vl53l0x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1258 2022-11-28 18:02:16.000000 adafruit-circuitpython-vl53l0x-3.6.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-28 18:02:08.000000 adafruit-circuitpython-vl53l0x-3.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:02:23.635884 adafruit-circuitpython-vl53l0x-3.6.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.824219 adafruit-circuitpython-vl53l0x-3.6.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.820219 adafruit-circuitpython-vl53l0x-3.6.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.820219 adafruit-circuitpython-vl53l0x-3.6.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.820219 adafruit-circuitpython-vl53l0x-3.6.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.824219 adafruit-circuitpython-vl53l0x-3.6.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-26 16:03:53.824219 adafruit-circuitpython-vl53l0x-3.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2590 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.824219 adafruit-circuitpython-vl53l0x-3.6.9/adafruit_circuitpython_vl53l0x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3380 2023-05-26 16:03:53.000000 adafruit-circuitpython-vl53l0x-3.6.9/adafruit_circuitpython_vl53l0x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 16:03:53.000000 adafruit-circuitpython-vl53l0x-3.6.9/adafruit_circuitpython_vl53l0x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:03:53.000000 adafruit-circuitpython-vl53l0x-3.6.9/adafruit_circuitpython_vl53l0x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:03:53.000000 adafruit-circuitpython-vl53l0x-3.6.9/adafruit_circuitpython_vl53l0x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:03:53.000000 adafruit-circuitpython-vl53l0x-3.6.9/adafruit_circuitpython_vl53l0x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26792 2023-05-26 16:03:46.000000 adafruit-circuitpython-vl53l0x-3.6.9/adafruit_vl53l0x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.824219 adafruit-circuitpython-vl53l0x-3.6.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.824219 adafruit-circuitpython-vl53l0x-3.6.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5727 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:03:53.824219 adafruit-circuitpython-vl53l0x-3.6.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2872 2023-05-26 16:03:46.000000 adafruit-circuitpython-vl53l0x-3.6.9/examples/vl53l0x_multiple_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-26 16:03:46.000000 adafruit-circuitpython-vl53l0x-3.6.9/examples/vl53l0x_multiple_sensors_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-05-26 16:03:46.000000 adafruit-circuitpython-vl53l0x-3.6.9/examples/vl53l0x_simplecontinuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-26 16:03:46.000000 adafruit-circuitpython-vl53l0x-3.6.9/examples/vl53l0x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-26 16:03:46.000000 adafruit-circuitpython-vl53l0x-3.6.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:03:36.000000 adafruit-circuitpython-vl53l0x-3.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:03:53.824219 adafruit-circuitpython-vl53l0x-3.6.9/setup.cfg
```

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-vl53l0x-3.6.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/.gitignore` & `adafruit-circuitpython-vl53l0x-3.6.9/.gitignore`

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

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/.pre-commit-config.yaml` & `adafruit-circuitpython-vl53l0x-3.6.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/.pylintrc` & `adafruit-circuitpython-vl53l0x-3.6.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-vl53l0x-3.6.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/LICENSE` & `adafruit-circuitpython-vl53l0x-3.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-vl53l0x-3.6.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/LICENSES/MIT.txt` & `adafruit-circuitpython-vl53l0x-3.6.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-vl53l0x-3.6.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/PKG-INFO` & `adafruit-circuitpython-vl53l0x-3.6.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vl53l0x
-Version: 3.6.8
+Version: 3.6.9
 Summary: CircuitPython library for VL53L0X time of flight distance sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_VL53L0X
 Keywords: adafruit,vl53l0x,time,flight,distance,sensorbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/README.rst` & `adafruit-circuitpython-vl53l0x-3.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/adafruit_circuitpython_vl53l0x.egg-info/PKG-INFO` & `adafruit-circuitpython-vl53l0x-3.6.9/adafruit_circuitpython_vl53l0x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vl53l0x
-Version: 3.6.8
+Version: 3.6.9
 Summary: CircuitPython library for VL53L0X time of flight distance sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_VL53L0X
 Keywords: adafruit,vl53l0x,time,flight,distance,sensorbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/adafruit_circuitpython_vl53l0x.egg-info/SOURCES.txt` & `adafruit-circuitpython-vl53l0x-3.6.9/adafruit_circuitpython_vl53l0x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/adafruit_vl53l0x.py` & `adafruit-circuitpython-vl53l0x-3.6.9/adafruit_vl53l0x.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 try:
     from typing import Optional, Tuple, Type
     from types import TracebackType
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "3.6.8"
+__version__ = "3.6.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_VL53L0X.git"
 
 # Configuration constants:
 _SYSRANGE_START = const(0x00)
 _SYSTEM_THRESH_HIGH = const(0x0C)
 _SYSTEM_THRESH_LOW = const(0x0E)
 _SYSTEM_SEQUENCE_CONFIG = const(0x01)
```

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/docs/_static/favicon.ico` & `adafruit-circuitpython-vl53l0x-3.6.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/docs/conf.py` & `adafruit-circuitpython-vl53l0x-3.6.9/docs/conf.py`

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

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/docs/examples.rst` & `adafruit-circuitpython-vl53l0x-3.6.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/docs/index.rst` & `adafruit-circuitpython-vl53l0x-3.6.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/examples/vl53l0x_multiple_sensors.py` & `adafruit-circuitpython-vl53l0x-3.6.9/examples/vl53l0x_multiple_sensors.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/examples/vl53l0x_multiple_sensors_continuous.py` & `adafruit-circuitpython-vl53l0x-3.6.9/examples/vl53l0x_multiple_sensors_continuous.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/examples/vl53l0x_simplecontinuous.py` & `adafruit-circuitpython-vl53l0x-3.6.9/examples/vl53l0x_simplecontinuous.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/examples/vl53l0x_simpletest.py` & `adafruit-circuitpython-vl53l0x-3.6.9/examples/vl53l0x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l0x-3.6.8/pyproject.toml` & `adafruit-circuitpython-vl53l0x-3.6.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-vl53l0x"
 description = "CircuitPython library for VL53L0X time of flight distance sensor."
-version = "3.6.8"
+version = "3.6.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_VL53L0X"}
 keywords = [
     "adafruit",
```

