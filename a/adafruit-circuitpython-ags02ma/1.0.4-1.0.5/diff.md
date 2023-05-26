# Comparing `tmp/adafruit-circuitpython-ags02ma-1.0.4.tar.gz` & `tmp/adafruit-circuitpython-ags02ma-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ags02ma-1.0.4.tar", last modified: Mon Apr 24 14:44:38 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ags02ma-1.0.5.tar", last modified: Fri May 26 16:24:44 2023, max compression
```

## Comparing `adafruit-circuitpython-ags02ma-1.0.4.tar` & `adafruit-circuitpython-ags02ma-1.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.604179 adafruit-circuitpython-ags02ma-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-04-24 14:44:29.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_ags02ma.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-24 14:44:38.000000 adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.608178 adafruit-circuitpython-ags02ma-1.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5979 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-04-24 14:44:29.000000 adafruit-circuitpython-ags02ma-1.0.4/examples/ags02ma_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-24 14:44:29.000000 adafruit-circuitpython-ags02ma-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-24 14:44:13.000000 adafruit-circuitpython-ags02ma-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 14:44:38.612179 adafruit-circuitpython-ags02ma-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.630806 adafruit-circuitpython-ags02ma-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.626805 adafruit-circuitpython-ags02ma-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.626805 adafruit-circuitpython-ags02ma-1.0.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.626805 adafruit-circuitpython-ags02ma-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.630806 adafruit-circuitpython-ags02ma-1.0.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-26 16:24:44.630806 adafruit-circuitpython-ags02ma-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3275 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-26 16:24:36.000000 adafruit-circuitpython-ags02ma-1.0.5/adafruit_ags02ma.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.630806 adafruit-circuitpython-ags02ma-1.0.5/adafruit_circuitpython_ags02ma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-05-26 16:24:44.000000 adafruit-circuitpython-ags02ma-1.0.5/adafruit_circuitpython_ags02ma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 16:24:44.000000 adafruit-circuitpython-ags02ma-1.0.5/adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:24:44.000000 adafruit-circuitpython-ags02ma-1.0.5/adafruit_circuitpython_ags02ma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:24:44.000000 adafruit-circuitpython-ags02ma-1.0.5/adafruit_circuitpython_ags02ma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:24:44.000000 adafruit-circuitpython-ags02ma-1.0.5/adafruit_circuitpython_ags02ma.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.630806 adafruit-circuitpython-ags02ma-1.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.630806 adafruit-circuitpython-ags02ma-1.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:44.630806 adafruit-circuitpython-ags02ma-1.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 16:24:36.000000 adafruit-circuitpython-ags02ma-1.0.5/examples/ags02ma_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 16:24:36.000000 adafruit-circuitpython-ags02ma-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 16:24:26.000000 adafruit-circuitpython-ags02ma-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:24:44.630806 adafruit-circuitpython-ags02ma-1.0.5/setup.cfg
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ags02ma-1.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/.gitignore` & `adafruit-circuitpython-ags02ma-1.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/.pre-commit-config.yaml` & `adafruit-circuitpython-ags02ma-1.0.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/.pylintrc` & `adafruit-circuitpython-ags02ma-1.0.5/.pylintrc`

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

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ags02ma-1.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/LICENSE` & `adafruit-circuitpython-ags02ma-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ags02ma-1.0.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/LICENSES/MIT.txt` & `adafruit-circuitpython-ags02ma-1.0.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ags02ma-1.0.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/PKG-INFO` & `adafruit-circuitpython-ags02ma-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ags02ma
-Version: 1.0.4
+Version: 1.0.5
 Summary: CircuitPython / Python library for AGS02MA gas sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AGS02MA
 Keywords: adafruit,blinka,circuitpython,micropython,ags02ma,tvoc,gas,resistance,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/README.rst` & `adafruit-circuitpython-ags02ma-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/adafruit_ags02ma.py` & `adafruit-circuitpython-ags02ma-1.0.5/adafruit_ags02ma.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     pass
 
 import time
 import struct
 from micropython import const
 from adafruit_bus_device import i2c_device
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AGS02MA.git"
 
 AGS02MA_I2CADDR_DEFAULT: int = const(0x1A)  # Default I2C address
 _AGS02MA_TVOCSTAT_REG = const(0x00)
 _AGS02MA_VERSION_REG = const(0x11)
 _AGS02MA_GASRES_REG = const(0x20)
 _AGS02MA_SETADDR_REG = const(0x21)
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/PKG-INFO` & `adafruit-circuitpython-ags02ma-1.0.5/adafruit_circuitpython_ags02ma.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ags02ma
-Version: 1.0.4
+Version: 1.0.5
 Summary: CircuitPython / Python library for AGS02MA gas sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AGS02MA
 Keywords: adafruit,blinka,circuitpython,micropython,ags02ma,tvoc,gas,resistance,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt` & `adafruit-circuitpython-ags02ma-1.0.5/adafruit_circuitpython_ags02ma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/docs/_static/favicon.ico` & `adafruit-circuitpython-ags02ma-1.0.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/docs/conf.py` & `adafruit-circuitpython-ags02ma-1.0.5/docs/conf.py`

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

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/docs/index.rst` & `adafruit-circuitpython-ags02ma-1.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/examples/ags02ma_simpletest.py` & `adafruit-circuitpython-ags02ma-1.0.5/examples/ags02ma_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ags02ma-1.0.4/pyproject.toml` & `adafruit-circuitpython-ags02ma-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ags02ma"
 description = "CircuitPython / Python library for AGS02MA gas sensor"
-version = "1.0.4"
+version = "1.0.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AGS02MA"}
 keywords = [
     "adafruit",
```

