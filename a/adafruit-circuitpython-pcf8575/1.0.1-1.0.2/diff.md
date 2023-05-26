# Comparing `tmp/adafruit-circuitpython-pcf8575-1.0.1.tar.gz` & `tmp/adafruit-circuitpython-pcf8575-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pcf8575-1.0.1.tar", last modified: Mon Nov 28 18:08:48 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pcf8575-1.0.2.tar", last modified: Fri May 26 15:57:07 2023, max compression
```

## Comparing `adafruit-circuitpython-pcf8575-1.0.1.tar` & `adafruit-circuitpython-pcf8575-1.0.2.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.814555 adafruit-circuitpython-pcf8575-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.802555 adafruit-circuitpython-pcf8575-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.810555 adafruit-circuitpython-pcf8575-1.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.810555 adafruit-circuitpython-pcf8575-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1254 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      405 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1098 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.810555 adafruit-circuitpython-pcf8575-1.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4076 2022-11-28 18:08:48.814555 adafruit-circuitpython-pcf8575-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3292 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      182 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.810555 adafruit-circuitpython-pcf8575-1.0.1/adafruit_circuitpython_pcf8575.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4076 2022-11-28 18:08:48.000000 adafruit-circuitpython-pcf8575-1.0.1/adafruit_circuitpython_pcf8575.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1062 2022-11-28 18:08:48.000000 adafruit-circuitpython-pcf8575-1.0.1/adafruit_circuitpython_pcf8575.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:08:48.000000 adafruit-circuitpython-pcf8575-1.0.1/adafruit_circuitpython_pcf8575.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:08:48.000000 adafruit-circuitpython-pcf8575-1.0.1/adafruit_circuitpython_pcf8575.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:08:48.000000 adafruit-circuitpython-pcf8575-1.0.1/adafruit_circuitpython_pcf8575.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     6971 2022-11-28 18:08:38.000000 adafruit-circuitpython-pcf8575-1.0.1/adafruit_pcf8575.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.814555 adafruit-circuitpython-pcf8575-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.814555 adafruit-circuitpython-pcf8575-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      267 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     5979 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1049 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      183 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:08:48.814555 adafruit-circuitpython-pcf8575-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (122)      549 2022-11-28 18:08:38.000000 adafruit-circuitpython-pcf8575-1.0.1/examples/pcf8575_blink16outputs.py
--rw-r--r--   0 runner    (1001) docker     (122)      764 2022-11-28 18:08:38.000000 adafruit-circuitpython-pcf8575-1.0.1/examples/pcf8575_buttonled.py
--rw-r--r--   0 runner    (1001) docker     (122)      620 2022-11-28 18:08:38.000000 adafruit-circuitpython-pcf8575-1.0.1/examples/pcf8575_read16inputs.py
--rw-r--r--   0 runner    (1001) docker     (122)      649 2022-11-28 18:08:38.000000 adafruit-circuitpython-pcf8575-1.0.1/examples/pcf8575_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1572 2022-11-28 18:08:38.000000 adafruit-circuitpython-pcf8575-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      240 2022-11-28 18:08:28.000000 adafruit-circuitpython-pcf8575-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:08:48.814555 adafruit-circuitpython-pcf8575-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.687458 adafruit-circuitpython-pcf8575-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.679458 adafruit-circuitpython-pcf8575-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.683458 adafruit-circuitpython-pcf8575-1.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.683458 adafruit-circuitpython-pcf8575-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.683458 adafruit-circuitpython-pcf8575-1.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-26 15:57:07.683458 adafruit-circuitpython-pcf8575-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3292 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.683458 adafruit-circuitpython-pcf8575-1.0.2/adafruit_circuitpython_pcf8575.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-05-26 15:57:07.000000 adafruit-circuitpython-pcf8575-1.0.2/adafruit_circuitpython_pcf8575.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-26 15:57:07.000000 adafruit-circuitpython-pcf8575-1.0.2/adafruit_circuitpython_pcf8575.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:57:07.000000 adafruit-circuitpython-pcf8575-1.0.2/adafruit_circuitpython_pcf8575.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 15:57:07.000000 adafruit-circuitpython-pcf8575-1.0.2/adafruit_circuitpython_pcf8575.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 15:57:07.000000 adafruit-circuitpython-pcf8575-1.0.2/adafruit_circuitpython_pcf8575.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6971 2023-05-26 15:57:00.000000 adafruit-circuitpython-pcf8575-1.0.2/adafruit_pcf8575.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.683458 adafruit-circuitpython-pcf8575-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.683458 adafruit-circuitpython-pcf8575-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6007 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:57:07.683458 adafruit-circuitpython-pcf8575-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-26 15:57:00.000000 adafruit-circuitpython-pcf8575-1.0.2/examples/pcf8575_blink16outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-26 15:57:00.000000 adafruit-circuitpython-pcf8575-1.0.2/examples/pcf8575_buttonled.py
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-05-26 15:57:00.000000 adafruit-circuitpython-pcf8575-1.0.2/examples/pcf8575_read16inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-26 15:57:00.000000 adafruit-circuitpython-pcf8575-1.0.2/examples/pcf8575_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-26 15:57:00.000000 adafruit-circuitpython-pcf8575-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 15:56:48.000000 adafruit-circuitpython-pcf8575-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:57:07.687458 adafruit-circuitpython-pcf8575-1.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pcf8575-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/.gitignore` & `adafruit-circuitpython-pcf8575-1.0.2/.gitignore`

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

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-pcf8575-1.0.2/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/.pylintrc` & `adafruit-circuitpython-pcf8575-1.0.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pcf8575-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/LICENSE` & `adafruit-circuitpython-pcf8575-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pcf8575-1.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-pcf8575-1.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pcf8575-1.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/PKG-INFO` & `adafruit-circuitpython-pcf8575-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcf8575
-Version: 1.0.1
+Version: 1.0.2
 Summary: CircuitPython library for Adafruit PCF8575 GPIO expander
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PCF8575
 Keywords: adafruit,blinka,circuitpython,micropython,pcf8575,pcf8575,i2c,gpio,expander,python,library
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/README.rst` & `adafruit-circuitpython-pcf8575-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/adafruit_circuitpython_pcf8575.egg-info/PKG-INFO` & `adafruit-circuitpython-pcf8575-1.0.2/adafruit_circuitpython_pcf8575.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcf8575
-Version: 1.0.1
+Version: 1.0.2
 Summary: CircuitPython library for Adafruit PCF8575 GPIO expander
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_PCF8575
 Keywords: adafruit,blinka,circuitpython,micropython,pcf8575,pcf8575,i2c,gpio,expander,python,library
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/adafruit_circuitpython_pcf8575.egg-info/SOURCES.txt` & `adafruit-circuitpython-pcf8575-1.0.2/adafruit_circuitpython_pcf8575.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/adafruit_pcf8575.py` & `adafruit-circuitpython-pcf8575-1.0.2/adafruit_pcf8575.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     pass
 
 
 from adafruit_bus_device.i2c_device import I2CDevice
 from micropython import const
 import digitalio
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_PCF8575.git"
 
 PCF8575_I2CADDR_DEFAULT: int = const(0x20)  # Default I2C address
 
 
 class PCF8575:
     """Interface library for PCF8575 GPIO expanders
```

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-pcf8575-1.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/docs/conf.py` & `adafruit-circuitpython-pcf8575-1.0.2/docs/conf.py`

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

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/docs/index.rst` & `adafruit-circuitpython-pcf8575-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/examples/pcf8575_blink16outputs.py` & `adafruit-circuitpython-pcf8575-1.0.2/examples/pcf8575_blink16outputs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/examples/pcf8575_buttonled.py` & `adafruit-circuitpython-pcf8575-1.0.2/examples/pcf8575_buttonled.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/examples/pcf8575_read16inputs.py` & `adafruit-circuitpython-pcf8575-1.0.2/examples/pcf8575_read16inputs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/examples/pcf8575_simpletest.py` & `adafruit-circuitpython-pcf8575-1.0.2/examples/pcf8575_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcf8575-1.0.1/pyproject.toml` & `adafruit-circuitpython-pcf8575-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-pcf8575"
 description = "CircuitPython library for Adafruit PCF8575 GPIO expander"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_PCF8575"}
 keywords = [
     "adafruit",
```

