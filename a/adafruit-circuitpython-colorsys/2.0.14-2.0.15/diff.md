# Comparing `tmp/adafruit-circuitpython-colorsys-2.0.14.tar.gz` & `tmp/adafruit-circuitpython-colorsys-2.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-colorsys-2.0.14.tar", last modified: Tue Feb  7 21:00:21 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-colorsys-2.0.15.tar", last modified: Fri May 26 16:23:56 2023, max compression
```

## Comparing `adafruit-circuitpython-colorsys-2.0.14.tar` & `adafruit-circuitpython-colorsys-2.0.15.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.211998 adafruit-circuitpython-colorsys-2.0.14/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.199998 adafruit-circuitpython-colorsys-2.0.14/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.203998 adafruit-circuitpython-colorsys-2.0.14/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.203998 adafruit-circuitpython-colorsys-2.0.14/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.207998 adafruit-circuitpython-colorsys-2.0.14/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/LICENSES/PSF-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-02-07 21:00:21.211998 adafruit-circuitpython-colorsys-2.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.207998 adafruit-circuitpython-colorsys-2.0.14/adafruit_circuitpython_colorsys.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-02-07 21:00:21.000000 adafruit-circuitpython-colorsys-2.0.14/adafruit_circuitpython_colorsys.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-02-07 21:00:21.000000 adafruit-circuitpython-colorsys-2.0.14/adafruit_circuitpython_colorsys.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 21:00:21.000000 adafruit-circuitpython-colorsys-2.0.14/adafruit_circuitpython_colorsys.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-07 21:00:21.000000 adafruit-circuitpython-colorsys-2.0.14/adafruit_circuitpython_colorsys.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-07 21:00:21.000000 adafruit-circuitpython-colorsys-2.0.14/adafruit_circuitpython_colorsys.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-02-07 21:00:13.000000 adafruit-circuitpython-colorsys-2.0.14/colorsys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.211998 adafruit-circuitpython-colorsys-2.0.14/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.211998 adafruit-circuitpython-colorsys-2.0.14/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5665 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 21:00:21.211998 adafruit-circuitpython-colorsys-2.0.14/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-02-07 21:00:13.000000 adafruit-circuitpython-colorsys-2.0.14/examples/colorsys_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-02-07 21:00:13.000000 adafruit-circuitpython-colorsys-2.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-07 21:00:02.000000 adafruit-circuitpython-colorsys-2.0.14/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 21:00:21.211998 adafruit-circuitpython-colorsys-2.0.14/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.016888 adafruit-circuitpython-colorsys-2.0.15/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.008888 adafruit-circuitpython-colorsys-2.0.15/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.012888 adafruit-circuitpython-colorsys-2.0.15/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.012888 adafruit-circuitpython-colorsys-2.0.15/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.012888 adafruit-circuitpython-colorsys-2.0.15/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12785 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/LICENSES/PSF-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-26 16:23:56.012888 adafruit-circuitpython-colorsys-2.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.012888 adafruit-circuitpython-colorsys-2.0.15/adafruit_circuitpython_colorsys.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2563 2023-05-26 16:23:55.000000 adafruit-circuitpython-colorsys-2.0.15/adafruit_circuitpython_colorsys.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-26 16:23:56.000000 adafruit-circuitpython-colorsys-2.0.15/adafruit_circuitpython_colorsys.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:23:55.000000 adafruit-circuitpython-colorsys-2.0.15/adafruit_circuitpython_colorsys.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:23:55.000000 adafruit-circuitpython-colorsys-2.0.15/adafruit_circuitpython_colorsys.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:23:55.000000 adafruit-circuitpython-colorsys-2.0.15/adafruit_circuitpython_colorsys.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3241 2023-05-26 16:23:48.000000 adafruit-circuitpython-colorsys-2.0.15/colorsys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.012888 adafruit-circuitpython-colorsys-2.0.15/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.012888 adafruit-circuitpython-colorsys-2.0.15/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.012888 adafruit-circuitpython-colorsys-2.0.15/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-26 16:23:48.000000 adafruit-circuitpython-colorsys-2.0.15/examples/colorsys_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-26 16:23:48.000000 adafruit-circuitpython-colorsys-2.0.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:23:39.000000 adafruit-circuitpython-colorsys-2.0.15/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:23:56.016888 adafruit-circuitpython-colorsys-2.0.15/setup.cfg
```

### Comparing `adafruit-circuitpython-colorsys-2.0.14/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-colorsys-2.0.15/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/.gitignore` & `adafruit-circuitpython-colorsys-2.0.15/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/.pre-commit-config.yaml` & `adafruit-circuitpython-colorsys-2.0.15/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-colorsys-2.0.14/.pylintrc` & `adafruit-circuitpython-colorsys-2.0.15/.pylintrc`

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

### Comparing `adafruit-circuitpython-colorsys-2.0.14/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-colorsys-2.0.15/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/LICENSE` & `adafruit-circuitpython-colorsys-2.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-colorsys-2.0.15/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/LICENSES/MIT.txt` & `adafruit-circuitpython-colorsys-2.0.15/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/LICENSES/PSF-2.0.txt` & `adafruit-circuitpython-colorsys-2.0.15/LICENSES/PSF-2.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/LICENSES/Unlicense.txt` & `adafruit-circuitpython-colorsys-2.0.15/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/PKG-INFO` & `adafruit-circuitpython-colorsys-2.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-colorsys
-Version: 2.0.14
+Version: 2.0.15
 Summary: CircuitPython CPython compatible libraries
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Colorsys
 Keywords: adafruit,colorsys,cpython,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-colorsys-2.0.14/README.rst` & `adafruit-circuitpython-colorsys-2.0.15/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/adafruit_circuitpython_colorsys.egg-info/PKG-INFO` & `adafruit-circuitpython-colorsys-2.0.15/adafruit_circuitpython_colorsys.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-colorsys
-Version: 2.0.14
+Version: 2.0.15
 Summary: CircuitPython CPython compatible libraries
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Colorsys
 Keywords: adafruit,colorsys,cpython,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-colorsys-2.0.14/adafruit_circuitpython_colorsys.egg-info/SOURCES.txt` & `adafruit-circuitpython-colorsys-2.0.15/adafruit_circuitpython_colorsys.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/colorsys.py` & `adafruit-circuitpython-colorsys-2.0.15/colorsys.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 try:
     from typing import Tuple
 except ImportError:
     pass
 
 
-__version__ = "2.0.14"
+__version__ = "2.0.15"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Colorsys.git"
 __all__ = ["hls_to_rgb", "hsv_to_rgb"]
 
 # Some floating point constants
 
 ONE_THIRD = 1.0 / 3.0
 ONE_SIXTH = 1.0 / 6.0
```

### Comparing `adafruit-circuitpython-colorsys-2.0.14/docs/_static/favicon.ico` & `adafruit-circuitpython-colorsys-2.0.15/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/docs/conf.py` & `adafruit-circuitpython-colorsys-2.0.15/docs/conf.py`

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

### Comparing `adafruit-circuitpython-colorsys-2.0.14/docs/index.rst` & `adafruit-circuitpython-colorsys-2.0.15/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-colorsys-2.0.14/pyproject.toml` & `adafruit-circuitpython-colorsys-2.0.15/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-colorsys"
 description = "CircuitPython CPython compatible libraries"
-version = "2.0.14"
+version = "2.0.15"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Colorsys"}
 keywords = [
     "adafruit",
```

