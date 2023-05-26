# Comparing `tmp/adafruit-circuitpython-mmc56x3-1.0.4.tar.gz` & `tmp/adafruit-circuitpython-mmc56x3-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mmc56x3-1.0.4.tar", last modified: Mon Nov 28 18:09:55 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-mmc56x3-1.0.5.tar", last modified: Fri May 26 15:57:29 2023, max compression
```

## Comparing `adafruit-circuitpython-mmc56x3-1.0.4.tar` & `adafruit-circuitpython-mmc56x3-1.0.5.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.702850 adafruit-circuitpython-mmc56x3-1.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.694851 adafruit-circuitpython-mmc56x3-1.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.698850 adafruit-circuitpython-mmc56x3-1.0.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.698850 adafruit-circuitpython-mmc56x3-1.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.698850 adafruit-circuitpython-mmc56x3-1.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4119 2022-11-28 18:09:55.702850 adafruit-circuitpython-mmc56x3-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3365 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.698850 adafruit-circuitpython-mmc56x3-1.0.4/adafruit_circuitpython_mmc56x3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4119 2022-11-28 18:09:55.000000 adafruit-circuitpython-mmc56x3-1.0.4/adafruit_circuitpython_mmc56x3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      995 2022-11-28 18:09:55.000000 adafruit-circuitpython-mmc56x3-1.0.4/adafruit_circuitpython_mmc56x3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:09:55.000000 adafruit-circuitpython-mmc56x3-1.0.4/adafruit_circuitpython_mmc56x3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       93 2022-11-28 18:09:55.000000 adafruit-circuitpython-mmc56x3-1.0.4/adafruit_circuitpython_mmc56x3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:09:55.000000 adafruit-circuitpython-mmc56x3-1.0.4/adafruit_circuitpython_mmc56x3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6966 2022-11-28 18:09:43.000000 adafruit-circuitpython-mmc56x3-1.0.4/adafruit_mmc56x3.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.702850 adafruit-circuitpython-mmc56x3-1.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.702850 adafruit-circuitpython-mmc56x3-1.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      267 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     6066 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      973 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:09:55.702850 adafruit-circuitpython-mmc56x3-1.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      621 2022-11-28 18:09:43.000000 adafruit-circuitpython-mmc56x3-1.0.4/examples/mmc56x3_continuous.py
--rw-r--r--   0 runner    (1001) docker     (122)      640 2022-11-28 18:09:43.000000 adafruit-circuitpython-mmc56x3-1.0.4/examples/mmc56x3_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2022-11-28 18:09:43.000000 adafruit-circuitpython-mmc56x3-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      190 2022-11-28 18:09:15.000000 adafruit-circuitpython-mmc56x3-1.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:09:55.702850 adafruit-circuitpython-mmc56x3-1.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.455910 adafruit-circuitpython-mmc56x3-1.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.447910 adafruit-circuitpython-mmc56x3-1.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.451910 adafruit-circuitpython-mmc56x3-1.0.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.451910 adafruit-circuitpython-mmc56x3-1.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.451910 adafruit-circuitpython-mmc56x3-1.0.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-26 15:57:29.455910 adafruit-circuitpython-mmc56x3-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.455910 adafruit-circuitpython-mmc56x3-1.0.5/adafruit_circuitpython_mmc56x3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-26 15:57:29.000000 adafruit-circuitpython-mmc56x3-1.0.5/adafruit_circuitpython_mmc56x3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 15:57:29.000000 adafruit-circuitpython-mmc56x3-1.0.5/adafruit_circuitpython_mmc56x3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:57:29.000000 adafruit-circuitpython-mmc56x3-1.0.5/adafruit_circuitpython_mmc56x3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 15:57:29.000000 adafruit-circuitpython-mmc56x3-1.0.5/adafruit_circuitpython_mmc56x3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 15:57:29.000000 adafruit-circuitpython-mmc56x3-1.0.5/adafruit_circuitpython_mmc56x3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6966 2023-05-26 15:57:19.000000 adafruit-circuitpython-mmc56x3-1.0.5/adafruit_mmc56x3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.455910 adafruit-circuitpython-mmc56x3-1.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.455910 adafruit-circuitpython-mmc56x3-1.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6094 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:29.455910 adafruit-circuitpython-mmc56x3-1.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 15:57:19.000000 adafruit-circuitpython-mmc56x3-1.0.5/examples/mmc56x3_continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 15:57:19.000000 adafruit-circuitpython-mmc56x3-1.0.5/examples/mmc56x3_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-26 15:57:19.000000 adafruit-circuitpython-mmc56x3-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 15:57:03.000000 adafruit-circuitpython-mmc56x3-1.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:57:29.455910 adafruit-circuitpython-mmc56x3-1.0.5/setup.cfg
```

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mmc56x3-1.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/.gitignore` & `adafruit-circuitpython-mmc56x3-1.0.5/.gitignore`

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

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/.pre-commit-config.yaml` & `adafruit-circuitpython-mmc56x3-1.0.5/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/.pylintrc` & `adafruit-circuitpython-mmc56x3-1.0.5/.pylintrc`

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

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mmc56x3-1.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/LICENSE` & `adafruit-circuitpython-mmc56x3-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mmc56x3-1.0.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/LICENSES/MIT.txt` & `adafruit-circuitpython-mmc56x3-1.0.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mmc56x3-1.0.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/PKG-INFO` & `adafruit-circuitpython-mmc56x3-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mmc56x3
-Version: 1.0.4
+Version: 1.0.5
 Summary: Magnetometer sensor library
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MMC56x3.git
 Keywords: adafruit,blinka,circuitpython,micropython,mmc56x3,mmc5603,mmc5613,magnetometer,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/README.rst` & `adafruit-circuitpython-mmc56x3-1.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/adafruit_circuitpython_mmc56x3.egg-info/PKG-INFO` & `adafruit-circuitpython-mmc56x3-1.0.5/adafruit_circuitpython_mmc56x3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mmc56x3
-Version: 1.0.4
+Version: 1.0.5
 Summary: Magnetometer sensor library
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MMC56x3.git
 Keywords: adafruit,blinka,circuitpython,micropython,mmc56x3,mmc5603,mmc5613,magnetometer,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/adafruit_circuitpython_mmc56x3.egg-info/SOURCES.txt` & `adafruit-circuitpython-mmc56x3-1.0.5/adafruit_circuitpython_mmc56x3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/adafruit_mmc56x3.py` & `adafruit-circuitpython-mmc56x3-1.0.5/adafruit_mmc56x3.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 try:
     from typing import Tuple
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.0.4"
+__version__ = "1.0.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MMC56x3.git"
 
 _MMC5603_I2CADDR_DEFAULT: int = const(0x30)  # Default I2C address
 _MMC5603_CHIP_ID = const(0x10)
 
 _MMC5603_OUT_X_L = const(0x00)  # Register that starts the mag data out
 _MMC5603_OUT_TEMP = const(0x09)  # Register that contains temp reading
```

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/docs/_static/favicon.ico` & `adafruit-circuitpython-mmc56x3-1.0.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/docs/conf.py` & `adafruit-circuitpython-mmc56x3-1.0.5/docs/conf.py`

 * *Files 0% similar despite different names*

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

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/docs/index.rst` & `adafruit-circuitpython-mmc56x3-1.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/examples/mmc56x3_continuous.py` & `adafruit-circuitpython-mmc56x3-1.0.5/examples/mmc56x3_continuous.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/examples/mmc56x3_simpletest.py` & `adafruit-circuitpython-mmc56x3-1.0.5/examples/mmc56x3_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mmc56x3-1.0.4/pyproject.toml` & `adafruit-circuitpython-mmc56x3-1.0.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mmc56x3"
 description = "Magnetometer sensor library"
-version = "1.0.4"
+version = "1.0.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MMC56x3.git"}
 keywords = [
     "adafruit",
```

