# Comparing `tmp/adafruit-circuitpython-tlv493d-2.0.1.tar.gz` & `tmp/adafruit-circuitpython-tlv493d-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tlv493d-2.0.1.tar", last modified: Mon Nov 28 18:05:33 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tlv493d-2.0.2.tar", last modified: Fri May 26 15:56:23 2023, max compression
```

## Comparing `adafruit-circuitpython-tlv493d-2.0.1.tar` & `adafruit-circuitpython-tlv493d-2.0.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.852029 adafruit-circuitpython-tlv493d-2.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.848029 adafruit-circuitpython-tlv493d-2.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.848029 adafruit-circuitpython-tlv493d-2.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.848029 adafruit-circuitpython-tlv493d-2.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6147 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.852029 adafruit-circuitpython-tlv493d-2.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2022-11-28 18:05:33.852029 adafruit-circuitpython-tlv493d-2.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2894 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.852029 adafruit-circuitpython-tlv493d-2.0.1/adafruit_circuitpython_tlv493d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     3669 2022-11-28 18:05:33.000000 adafruit-circuitpython-tlv493d-2.0.1/adafruit_circuitpython_tlv493d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      964 2022-11-28 18:05:33.000000 adafruit-circuitpython-tlv493d-2.0.1/adafruit_circuitpython_tlv493d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:05:33.000000 adafruit-circuitpython-tlv493d-2.0.1/adafruit_circuitpython_tlv493d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:05:33.000000 adafruit-circuitpython-tlv493d-2.0.1/adafruit_circuitpython_tlv493d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:05:33.000000 adafruit-circuitpython-tlv493d-2.0.1/adafruit_circuitpython_tlv493d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     5564 2022-11-28 18:05:24.000000 adafruit-circuitpython-tlv493d-2.0.1/adafruit_tlv493d.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.852029 adafruit-circuitpython-tlv493d-2.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.852029 adafruit-circuitpython-tlv493d-2.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      266 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5894 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1191 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)       96 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:33.852029 adafruit-circuitpython-tlv493d-2.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      407 2022-11-28 18:05:24.000000 adafruit-circuitpython-tlv493d-2.0.1/examples/tlv493d_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1236 2022-11-28 18:05:24.000000 adafruit-circuitpython-tlv493d-2.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:05:15.000000 adafruit-circuitpython-tlv493d-2.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:05:33.852029 adafruit-circuitpython-tlv493d-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.215841 adafruit-circuitpython-tlv493d-2.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.207841 adafruit-circuitpython-tlv493d-2.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.211841 adafruit-circuitpython-tlv493d-2.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.211841 adafruit-circuitpython-tlv493d-2.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.211841 adafruit-circuitpython-tlv493d-2.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-26 15:56:23.215841 adafruit-circuitpython-tlv493d-2.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2894 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.211841 adafruit-circuitpython-tlv493d-2.0.2/adafruit_circuitpython_tlv493d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-05-26 15:56:23.000000 adafruit-circuitpython-tlv493d-2.0.2/adafruit_circuitpython_tlv493d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 15:56:23.000000 adafruit-circuitpython-tlv493d-2.0.2/adafruit_circuitpython_tlv493d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:56:23.000000 adafruit-circuitpython-tlv493d-2.0.2/adafruit_circuitpython_tlv493d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 15:56:23.000000 adafruit-circuitpython-tlv493d-2.0.2/adafruit_circuitpython_tlv493d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 15:56:23.000000 adafruit-circuitpython-tlv493d-2.0.2/adafruit_circuitpython_tlv493d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-05-26 15:56:15.000000 adafruit-circuitpython-tlv493d-2.0.2/adafruit_tlv493d.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.215841 adafruit-circuitpython-tlv493d-2.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.215841 adafruit-circuitpython-tlv493d-2.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5922 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:56:23.215841 adafruit-circuitpython-tlv493d-2.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-26 15:56:15.000000 adafruit-circuitpython-tlv493d-2.0.2/examples/tlv493d_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-26 15:56:15.000000 adafruit-circuitpython-tlv493d-2.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 15:56:02.000000 adafruit-circuitpython-tlv493d-2.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:56:23.215841 adafruit-circuitpython-tlv493d-2.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tlv493d-2.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/.gitignore` & `adafruit-circuitpython-tlv493d-2.0.2/.gitignore`

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

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-tlv493d-2.0.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/.pylintrc` & `adafruit-circuitpython-tlv493d-2.0.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tlv493d-2.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/LICENSE` & `adafruit-circuitpython-tlv493d-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tlv493d-2.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-tlv493d-2.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tlv493d-2.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/PKG-INFO` & `adafruit-circuitpython-tlv493d-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tlv493d
-Version: 2.0.1
+Version: 2.0.2
 Summary: CircuitPython helper library for the TLV493D 3-axis magnetometer
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TLV493D
 Keywords: adafruit,blinka,circuitpython,micropython,tlv493d,tlv,sensor,magnetometer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/README.rst` & `adafruit-circuitpython-tlv493d-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/adafruit_circuitpython_tlv493d.egg-info/PKG-INFO` & `adafruit-circuitpython-tlv493d-2.0.2/adafruit_circuitpython_tlv493d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tlv493d
-Version: 2.0.1
+Version: 2.0.2
 Summary: CircuitPython helper library for the TLV493D 3-axis magnetometer
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_TLV493D
 Keywords: adafruit,blinka,circuitpython,micropython,tlv493d,tlv,sensor,magnetometer
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/adafruit_circuitpython_tlv493d.egg-info/SOURCES.txt` & `adafruit-circuitpython-tlv493d-2.0.2/adafruit_circuitpython_tlv493d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/adafruit_tlv493d.py` & `adafruit-circuitpython-tlv493d-2.0.2/adafruit_tlv493d.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 try:
     from typing import Tuple
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "2.0.1"
+__version__ = "2.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_TLV493D.git"
 
 _TLV493D_DEFAULT_ADDRESS = const(0x5E)
 
 
 class TLV493D:
     """Driver for the TLV493D 3-axis Magnetometer.
```

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-tlv493d-2.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/docs/conf.py` & `adafruit-circuitpython-tlv493d-2.0.2/docs/conf.py`

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

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/docs/index.rst` & `adafruit-circuitpython-tlv493d-2.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tlv493d-2.0.1/pyproject.toml` & `adafruit-circuitpython-tlv493d-2.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-tlv493d"
 description = "CircuitPython helper library for the TLV493D 3-axis magnetometer"
-version = "2.0.1"
+version = "2.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_TLV493D"}
 keywords = [
     "adafruit",
```

