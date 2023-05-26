# Comparing `tmp/adafruit-circuitpython-neopixel-spi-1.0.6.tar.gz` & `tmp/adafruit-circuitpython-neopixel-spi-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-neopixel-spi-1.0.6.tar", last modified: Fri Apr 28 23:01:04 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-neopixel-spi-1.0.7.tar", last modified: Fri May 26 16:25:00 2023, max compression
```

## Comparing `adafruit-circuitpython-neopixel-spi-1.0.6.tar` & `adafruit-circuitpython-neopixel-spi-1.0.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.950276 adafruit-circuitpython-neopixel-spi-1.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.950276 adafruit-circuitpython-neopixel-spi-1.0.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-28 23:01:04.000000 adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-28 23:00:56.000000 adafruit-circuitpython-neopixel-spi-1.0.6/examples/neopixel_spi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-04-28 23:00:56.000000 adafruit-circuitpython-neopixel-spi-1.0.6/neopixel_spi.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-28 23:00:56.000000 adafruit-circuitpython-neopixel-spi-1.0.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-28 23:00:44.000000 adafruit-circuitpython-neopixel-spi-1.0.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 23:01:04.954276 adafruit-circuitpython-neopixel-spi-1.0.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.058662 adafruit-circuitpython-neopixel-spi-1.0.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.054662 adafruit-circuitpython-neopixel-spi-1.0.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.054662 adafruit-circuitpython-neopixel-spi-1.0.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.054662 adafruit-circuitpython-neopixel-spi-1.0.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.054662 adafruit-circuitpython-neopixel-spi-1.0.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-26 16:25:00.058662 adafruit-circuitpython-neopixel-spi-1.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.054662 adafruit-circuitpython-neopixel-spi-1.0.7/adafruit_circuitpython_neopixel_spi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-26 16:25:00.000000 adafruit-circuitpython-neopixel-spi-1.0.7/adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-26 16:25:00.000000 adafruit-circuitpython-neopixel-spi-1.0.7/adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:25:00.000000 adafruit-circuitpython-neopixel-spi-1.0.7/adafruit_circuitpython_neopixel_spi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:25:00.000000 adafruit-circuitpython-neopixel-spi-1.0.7/adafruit_circuitpython_neopixel_spi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 16:25:00.000000 adafruit-circuitpython-neopixel-spi-1.0.7/adafruit_circuitpython_neopixel_spi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.054662 adafruit-circuitpython-neopixel-spi-1.0.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.058662 adafruit-circuitpython-neopixel-spi-1.0.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:25:00.058662 adafruit-circuitpython-neopixel-spi-1.0.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-26 16:24:52.000000 adafruit-circuitpython-neopixel-spi-1.0.7/examples/neopixel_spi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-26 16:24:52.000000 adafruit-circuitpython-neopixel-spi-1.0.7/neopixel_spi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-26 16:24:52.000000 adafruit-circuitpython-neopixel-spi-1.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:24:43.000000 adafruit-circuitpython-neopixel-spi-1.0.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:25:00.058662 adafruit-circuitpython-neopixel-spi-1.0.7/setup.cfg
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-neopixel-spi-1.0.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/.gitignore` & `adafruit-circuitpython-neopixel-spi-1.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/.pre-commit-config.yaml` & `adafruit-circuitpython-neopixel-spi-1.0.7/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/.pylintrc` & `adafruit-circuitpython-neopixel-spi-1.0.7/.pylintrc`

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

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-neopixel-spi-1.0.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/LICENSE` & `adafruit-circuitpython-neopixel-spi-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-neopixel-spi-1.0.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/MIT.txt` & `adafruit-circuitpython-neopixel-spi-1.0.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-neopixel-spi-1.0.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/PKG-INFO` & `adafruit-circuitpython-neopixel-spi-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neopixel-spi
-Version: 1.0.6
+Version: 1.0.7
 Summary: SPI driven CircuitPython driver for neopixels.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel_SPI
 Keywords: adafruit,blinka,circuitpython,micropython,neopixel_spi,neopixel
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/README.rst` & `adafruit-circuitpython-neopixel-spi-1.0.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO` & `adafruit-circuitpython-neopixel-spi-1.0.7/adafruit_circuitpython_neopixel_spi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neopixel-spi
-Version: 1.0.6
+Version: 1.0.7
 Summary: SPI driven CircuitPython driver for neopixels.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel_SPI
 Keywords: adafruit,blinka,circuitpython,micropython,neopixel_spi,neopixel
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt` & `adafruit-circuitpython-neopixel-spi-1.0.7/adafruit_circuitpython_neopixel_spi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/docs/_static/favicon.ico` & `adafruit-circuitpython-neopixel-spi-1.0.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/docs/conf.py` & `adafruit-circuitpython-neopixel-spi-1.0.7/docs/conf.py`

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

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/docs/index.rst` & `adafruit-circuitpython-neopixel-spi-1.0.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/examples/neopixel_spi_simpletest.py` & `adafruit-circuitpython-neopixel-spi-1.0.7/examples/neopixel_spi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/neopixel_spi.py` & `adafruit-circuitpython-neopixel-spi-1.0.7/neopixel_spi.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     from busio import SPI
 except ImportError:
     pass
 
 import adafruit_pixelbuf
 from adafruit_bus_device.spi_device import SPIDevice
 
-__version__ = "1.0.6"
+__version__ = "1.0.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel_SPI.git"
 
 # Pixel color order constants
 RGB: str = "RGB"
 """Red Green Blue"""
 GRB: str = "GRB"
 """Green Red Blue"""
```

### Comparing `adafruit-circuitpython-neopixel-spi-1.0.6/pyproject.toml` & `adafruit-circuitpython-neopixel-spi-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-neopixel-spi"
 description = "SPI driven CircuitPython driver for neopixels."
-version = "1.0.6"
+version = "1.0.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel_SPI"}
 keywords = [
     "adafruit",
```

