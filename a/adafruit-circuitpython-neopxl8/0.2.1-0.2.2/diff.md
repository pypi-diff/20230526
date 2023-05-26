# Comparing `tmp/adafruit-circuitpython-neopxl8-0.2.1.tar.gz` & `tmp/adafruit-circuitpython-neopxl8-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-neopxl8-0.2.1.tar", last modified: Sat Feb  4 02:46:25 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-neopxl8-0.2.2.tar", last modified: Fri May 26 16:23:56 2023, max compression
```

## Comparing `adafruit-circuitpython-neopxl8-0.2.1.tar` & `adafruit-circuitpython-neopxl8-0.2.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.194790 adafruit-circuitpython-neopxl8-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.186791 adafruit-circuitpython-neopxl8-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.190791 adafruit-circuitpython-neopxl8-0.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.190791 adafruit-circuitpython-neopxl8-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.190791 adafruit-circuitpython-neopxl8-0.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-02-04 02:46:25.194790 adafruit-circuitpython-neopxl8-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.194790 adafruit-circuitpython-neopxl8-0.2.1/adafruit_circuitpython_neopxl8.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-02-04 02:46:25.000000 adafruit-circuitpython-neopxl8-0.2.1/adafruit_circuitpython_neopxl8.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-02-04 02:46:25.000000 adafruit-circuitpython-neopxl8-0.2.1/adafruit_circuitpython_neopxl8.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-04 02:46:25.000000 adafruit-circuitpython-neopxl8-0.2.1/adafruit_circuitpython_neopxl8.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-02-04 02:46:25.000000 adafruit-circuitpython-neopxl8-0.2.1/adafruit_circuitpython_neopxl8.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-04 02:46:25.000000 adafruit-circuitpython-neopxl8-0.2.1/adafruit_circuitpython_neopxl8.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-02-04 02:46:18.000000 adafruit-circuitpython-neopxl8-0.2.1/adafruit_neopxl8.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.194790 adafruit-circuitpython-neopxl8-0.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.194790 adafruit-circuitpython-neopxl8-0.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-04 02:46:25.194790 adafruit-circuitpython-neopxl8-0.2.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-02-04 02:46:18.000000 adafruit-circuitpython-neopxl8-0.2.1/examples/neopxl8_animations.py
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-02-04 02:46:18.000000 adafruit-circuitpython-neopxl8-0.2.1/examples/neopxl8_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-02-04 02:46:18.000000 adafruit-circuitpython-neopxl8-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-02-04 02:46:08.000000 adafruit-circuitpython-neopxl8-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-04 02:46:25.194790 adafruit-circuitpython-neopxl8-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.803240 adafruit-circuitpython-neopxl8-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.803240 adafruit-circuitpython-neopxl8-0.2.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/adafruit_circuitpython_neopxl8.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-05-26 16:23:56.000000 adafruit-circuitpython-neopxl8-0.2.2/adafruit_circuitpython_neopxl8.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 16:23:56.000000 adafruit-circuitpython-neopxl8-0.2.2/adafruit_circuitpython_neopxl8.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:23:56.000000 adafruit-circuitpython-neopxl8-0.2.2/adafruit_circuitpython_neopxl8.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 16:23:56.000000 adafruit-circuitpython-neopxl8-0.2.2/adafruit_circuitpython_neopxl8.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:23:56.000000 adafruit-circuitpython-neopxl8-0.2.2/adafruit_circuitpython_neopxl8.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 2023-05-26 16:23:48.000000 adafruit-circuitpython-neopxl8-0.2.2/adafruit_neopxl8.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5920 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1144 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1713 2023-05-26 16:23:48.000000 adafruit-circuitpython-neopxl8-0.2.2/examples/neopxl8_animations.py
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-26 16:23:48.000000 adafruit-circuitpython-neopxl8-0.2.2/examples/neopxl8_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-26 16:23:48.000000 adafruit-circuitpython-neopxl8-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 16:23:36.000000 adafruit-circuitpython-neopxl8-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:23:56.807241 adafruit-circuitpython-neopxl8-0.2.2/setup.cfg
```

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-neopxl8-0.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/.gitignore` & `adafruit-circuitpython-neopxl8-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/.pre-commit-config.yaml` & `adafruit-circuitpython-neopxl8-0.2.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/.pylintrc` & `adafruit-circuitpython-neopxl8-0.2.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-neopxl8-0.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/LICENSE` & `adafruit-circuitpython-neopxl8-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-neopxl8-0.2.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/LICENSES/MIT.txt` & `adafruit-circuitpython-neopxl8-0.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-neopxl8-0.2.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/PKG-INFO` & `adafruit-circuitpython-neopxl8-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neopxl8
-Version: 0.2.1
+Version: 0.2.2
 Summary: PIO-driven 8-way concurrent NeoPixel driver for RP2040
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_neopxl8
 Keywords: adafruit,blinka,circuitpython,micropython,neopxl8,neopixel,rp2040,rgb,rgbw,led,animation
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/README.rst` & `adafruit-circuitpython-neopxl8-0.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/adafruit_circuitpython_neopxl8.egg-info/PKG-INFO` & `adafruit-circuitpython-neopxl8-0.2.2/adafruit_circuitpython_neopxl8.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neopxl8
-Version: 0.2.1
+Version: 0.2.2
 Summary: PIO-driven 8-way concurrent NeoPixel driver for RP2040
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_neopxl8
 Keywords: adafruit,blinka,circuitpython,micropython,neopxl8,neopixel,rp2040,rgb,rgbw,led,animation
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/adafruit_circuitpython_neopxl8.egg-info/SOURCES.txt` & `adafruit-circuitpython-neopxl8-0.2.2/adafruit_circuitpython_neopxl8.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/adafruit_neopxl8.py` & `adafruit-circuitpython-neopxl8-0.2.2/adafruit_neopxl8.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 
 import struct
 import adafruit_pioasm
 import bitops
 import adafruit_pixelbuf
 import rp2pio
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NeoPxl8.git"
 
 
 _PROGRAM = """
 .program piopixl8
 top:
     mov pins, null      ; always-low part (last cycle is the 'pull ifempty' after wrap)
```

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/docs/_static/favicon.ico` & `adafruit-circuitpython-neopxl8-0.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/docs/conf.py` & `adafruit-circuitpython-neopxl8-0.2.2/docs/conf.py`

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

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/docs/index.rst` & `adafruit-circuitpython-neopxl8-0.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/examples/neopxl8_animations.py` & `adafruit-circuitpython-neopxl8-0.2.2/examples/neopxl8_animations.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/examples/neopxl8_simpletest.py` & `adafruit-circuitpython-neopxl8-0.2.2/examples/neopxl8_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopxl8-0.2.1/pyproject.toml` & `adafruit-circuitpython-neopxl8-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-neopxl8"
 description = "PIO-driven 8-way concurrent NeoPixel driver for RP2040"
-version = "0.2.1"
+version = "0.2.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_neopxl8"}
 keywords = [
     "adafruit",
```

