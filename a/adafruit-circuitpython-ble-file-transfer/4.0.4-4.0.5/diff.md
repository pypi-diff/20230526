# Comparing `tmp/adafruit-circuitpython-ble-file-transfer-4.0.4.tar.gz` & `tmp/adafruit-circuitpython-ble-file-transfer-4.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-file-transfer-4.0.4.tar", last modified: Tue Nov 15 17:28:12 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-file-transfer-4.0.5.tar", last modified: Fri May 26 15:55:20 2023, max compression
```

## Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4.tar` & `adafruit-circuitpython-ble-file-transfer-4.0.5.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.344041 adafruit-circuitpython-ble-file-transfer-4.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.336041 adafruit-circuitpython-ble-file-transfer-4.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.340041 adafruit-circuitpython-ble-file-transfer-4.0.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.340041 adafruit-circuitpython-ble-file-transfer-4.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.340041 adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)    15500 2022-11-15 17:28:12.344041 adafruit-circuitpython-ble-file-transfer-4.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    14704 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    13824 2022-11-15 17:28:03.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_ble_file_transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.340041 adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_circuitpython_ble_file_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    15500 2022-11-15 17:28:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_circuitpython_ble_file_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-11-15 17:28:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_circuitpython_ble_file_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 17:28:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_circuitpython_ble_file_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-15 17:28:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_circuitpython_ble_file_transfer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-11-15 17:28:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_circuitpython_ble_file_transfer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.344041 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.344041 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5528 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      983 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      191 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:28:12.344041 adafruit-circuitpython-ble-file-transfer-4.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1522 2022-11-15 17:28:03.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/examples/ble_file_transfer_listdirs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6479 2022-11-15 17:28:03.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/examples/ble_file_transfer_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)    16538 2022-11-15 17:28:03.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/examples/ble_file_transfer_stub_server.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1267 2022-11-15 17:28:03.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-11-15 17:27:53.000000 adafruit-circuitpython-ble-file-transfer-4.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 17:28:12.344041 adafruit-circuitpython-ble-file-transfer-4.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.196634 adafruit-circuitpython-ble-file-transfer-4.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.192634 adafruit-circuitpython-ble-file-transfer-4.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.192634 adafruit-circuitpython-ble-file-transfer-4.0.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.192634 adafruit-circuitpython-ble-file-transfer-4.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.192634 adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-05-26 15:55:20.196634 adafruit-circuitpython-ble-file-transfer-4.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)    13824 2023-05-26 15:55:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_ble_file_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.192634 adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_circuitpython_ble_file_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15500 2023-05-26 15:55:20.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_circuitpython_ble_file_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 15:55:20.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_circuitpython_ble_file_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:55:20.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_circuitpython_ble_file_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 15:55:20.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_circuitpython_ble_file_transfer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 15:55:20.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_circuitpython_ble_file_transfer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.192634 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.196634 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5556 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:55:20.196634 adafruit-circuitpython-ble-file-transfer-4.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 15:55:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/examples/ble_file_transfer_listdirs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6479 2023-05-26 15:55:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/examples/ble_file_transfer_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16538 2023-05-26 15:55:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/examples/ble_file_transfer_stub_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-26 15:55:12.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-26 15:55:02.000000 adafruit-circuitpython-ble-file-transfer-4.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:55:20.196634 adafruit-circuitpython-ble-file-transfer-4.0.5/setup.cfg
```

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-file-transfer-4.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/.gitignore` & `adafruit-circuitpython-ble-file-transfer-4.0.5/.gitignore`

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

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-file-transfer-4.0.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/.pylintrc` & `adafruit-circuitpython-ble-file-transfer-4.0.5/.pylintrc`

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

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-file-transfer-4.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSE` & `adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-file-transfer-4.0.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/PKG-INFO` & `adafruit-circuitpython-ble-file-transfer-4.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-file-transfer
-Version: 4.0.4
+Version: 4.0.5
 Summary: Simple BLE Service for reading and writing files over BLE
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_File_Transfer.git
 Keywords: adafruit,blinka,circuitpython,micropython,ble_file_transfer,ble,file,transfer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/README.rst` & `adafruit-circuitpython-ble-file-transfer-4.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_ble_file_transfer.py` & `adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_ble_file_transfer.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 try:
     from typing import Optional, List
     from circuitpython_typing import WriteableBuffer, ReadableBuffer
 except ImportError:
     pass
 
-__version__ = "4.0.4"
+__version__ = "4.0.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_File_Transfer.git"
 
 CHUNK_SIZE = 490
 
 
 class FileTransferUUID(VendorUUID):
     """UUIDs with the CircuitPython base UUID."""
```

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_circuitpython_ble_file_transfer.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_circuitpython_ble_file_transfer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-file-transfer
-Version: 4.0.4
+Version: 4.0.5
 Summary: Simple BLE Service for reading and writing files over BLE
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_File_Transfer.git
 Keywords: adafruit,blinka,circuitpython,micropython,ble_file_transfer,ble,file,transfer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/adafruit_circuitpython_ble_file_transfer.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-file-transfer-4.0.5/adafruit_circuitpython_ble_file_transfer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-file-transfer-4.0.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/docs/conf.py` & `adafruit-circuitpython-ble-file-transfer-4.0.5/docs/conf.py`

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
 
 autodoc_mock_imports = ["bleak"]
```

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/docs/index.rst` & `adafruit-circuitpython-ble-file-transfer-4.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/examples/ble_file_transfer_listdirs.py` & `adafruit-circuitpython-ble-file-transfer-4.0.5/examples/ble_file_transfer_listdirs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/examples/ble_file_transfer_simpletest.py` & `adafruit-circuitpython-ble-file-transfer-4.0.5/examples/ble_file_transfer_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/examples/ble_file_transfer_stub_server.py` & `adafruit-circuitpython-ble-file-transfer-4.0.5/examples/ble_file_transfer_stub_server.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-file-transfer-4.0.4/pyproject.toml` & `adafruit-circuitpython-ble-file-transfer-4.0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ble-file-transfer"
 description = "Simple BLE Service for reading and writing files over BLE"
-version = "4.0.4"
+version = "4.0.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_File_Transfer.git"}
 keywords = [
     "adafruit",
```

