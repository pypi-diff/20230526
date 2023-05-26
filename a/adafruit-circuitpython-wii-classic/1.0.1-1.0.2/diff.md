# Comparing `tmp/adafruit-circuitpython-wii-classic-1.0.1.tar.gz` & `tmp/adafruit-circuitpython-wii-classic-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-wii-classic-1.0.1.tar", last modified: Mon Apr 10 14:22:39 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-wii-classic-1.0.2.tar", last modified: Fri May 26 16:24:32 2023, max compression
```

## Comparing `adafruit-circuitpython-wii-classic-1.0.1.tar` & `adafruit-circuitpython-wii-classic-1.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.291741 adafruit-circuitpython-wii-classic-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.291741 adafruit-circuitpython-wii-classic-1.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-10 14:22:39.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-04-10 14:22:30.000000 adafruit-circuitpython-wii-classic-1.0.1/adafruit_wii_classic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    77052 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-04-10 14:22:30.000000 adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic_displayio_visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-04-10 14:22:30.000000 adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-04-10 14:22:30.000000 adafruit-circuitpython-wii-classic-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-04-10 14:22:22.000000 adafruit-circuitpython-wii-classic-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 14:22:39.295741 adafruit-circuitpython-wii-classic-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.924703 adafruit-circuitpython-wii-classic-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.920703 adafruit-circuitpython-wii-classic-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.920703 adafruit-circuitpython-wii-classic-1.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.920703 adafruit-circuitpython-wii-classic-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.924703 adafruit-circuitpython-wii-classic-1.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-26 16:24:32.924703 adafruit-circuitpython-wii-classic-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4093 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.924703 adafruit-circuitpython-wii-classic-1.0.2/adafruit_circuitpython_wii_classic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-26 16:24:32.000000 adafruit-circuitpython-wii-classic-1.0.2/adafruit_circuitpython_wii_classic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-26 16:24:32.000000 adafruit-circuitpython-wii-classic-1.0.2/adafruit_circuitpython_wii_classic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:24:32.000000 adafruit-circuitpython-wii-classic-1.0.2/adafruit_circuitpython_wii_classic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:24:32.000000 adafruit-circuitpython-wii-classic-1.0.2/adafruit_circuitpython_wii_classic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 16:24:32.000000 adafruit-circuitpython-wii-classic-1.0.2/adafruit_circuitpython_wii_classic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7046 2023-05-26 16:24:24.000000 adafruit-circuitpython-wii-classic-1.0.2/adafruit_wii_classic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.924703 adafruit-circuitpython-wii-classic-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.924703 adafruit-circuitpython-wii-classic-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6055 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:32.924703 adafruit-circuitpython-wii-classic-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    77052 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/examples/wii_classic.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/examples/wii_classic.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5724 2023-05-26 16:24:24.000000 adafruit-circuitpython-wii-classic-1.0.2/examples/wii_classic_displayio_visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1007 2023-05-26 16:24:24.000000 adafruit-circuitpython-wii-classic-1.0.2/examples/wii_classic_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-26 16:24:24.000000 adafruit-circuitpython-wii-classic-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-26 16:24:14.000000 adafruit-circuitpython-wii-classic-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:24:32.924703 adafruit-circuitpython-wii-classic-1.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-wii-classic-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/.gitignore` & `adafruit-circuitpython-wii-classic-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-wii-classic-1.0.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/.pylintrc` & `adafruit-circuitpython-wii-classic-1.0.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-wii-classic-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/LICENSE` & `adafruit-circuitpython-wii-classic-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-wii-classic-1.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-wii-classic-1.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-wii-classic-1.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/PKG-INFO` & `adafruit-circuitpython-wii-classic-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wii-classic
-Version: 1.0.1
+Version: 1.0.2
 Summary: CircuitPython library for Nintendo Wii Classic controllers.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wii_Classic
 Keywords: adafruit,blinka,circuitpython,micropython,wii_classic,wii,classic,remote,control
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/README.rst` & `adafruit-circuitpython-wii-classic-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/PKG-INFO` & `adafruit-circuitpython-wii-classic-1.0.2/adafruit_circuitpython_wii_classic.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-wii-classic
-Version: 1.0.1
+Version: 1.0.2
 Summary: CircuitPython library for Nintendo Wii Classic controllers.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Wii_Classic
 Keywords: adafruit,blinka,circuitpython,micropython,wii_classic,wii,classic,remote,control
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/adafruit_circuitpython_wii_classic.egg-info/SOURCES.txt` & `adafruit-circuitpython-wii-classic-1.0.2/adafruit_circuitpython_wii_classic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/adafruit_wii_classic.py` & `adafruit-circuitpython-wii-classic-1.0.2/adafruit_wii_classic.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 try:
     import typing  # pylint: disable=unused-import
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Wii_Classic.git"
 
 _I2C_INIT_DELAY = 0.1
 
 
 class Wii_Classic:
     """Class which provides interface to Nintendo Wii Classic controller.
```

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-wii-classic-1.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/docs/conf.py` & `adafruit-circuitpython-wii-classic-1.0.2/docs/conf.py`

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

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/docs/index.rst` & `adafruit-circuitpython-wii-classic-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic.bmp` & `adafruit-circuitpython-wii-classic-1.0.2/examples/wii_classic.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic_displayio_visualizer.py` & `adafruit-circuitpython-wii-classic-1.0.2/examples/wii_classic_displayio_visualizer.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/examples/wii_classic_simpletest.py` & `adafruit-circuitpython-wii-classic-1.0.2/examples/wii_classic_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-wii-classic-1.0.1/pyproject.toml` & `adafruit-circuitpython-wii-classic-1.0.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-wii-classic"
 description = "CircuitPython library for Nintendo Wii Classic controllers."
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Wii_Classic"}
 keywords = [
     "adafruit",
```

