# Comparing `tmp/adafruit-circuitpython-displayio-ssd1306-1.6.0.tar.gz` & `tmp/adafruit-circuitpython-displayio-ssd1306-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-displayio-ssd1306-1.6.0.tar", last modified: Mon Feb 27 19:53:27 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-displayio-ssd1306-1.6.1.tar", last modified: Fri May 26 16:24:16 2023, max compression
```

## Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0.tar` & `adafruit-circuitpython-displayio-ssd1306-1.6.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.665422 adafruit-circuitpython-displayio-ssd1306-1.6.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.653421 adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.661422 adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.661422 adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.661422 adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-02-27 19:53:27.665422 adafruit-circuitpython-displayio-ssd1306-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.661422 adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_circuitpython_displayio_ssd1306.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-02-27 19:53:27.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_circuitpython_displayio_ssd1306.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-02-27 19:53:27.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_circuitpython_displayio_ssd1306.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 19:53:27.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_circuitpython_displayio_ssd1306.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-27 19:53:27.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_circuitpython_displayio_ssd1306.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-02-27 19:53:27.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_circuitpython_displayio_ssd1306.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-02-27 19:53:20.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_displayio_ssd1306.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.661422 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.661422 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5735 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 19:53:27.665422 adafruit-circuitpython-displayio-ssd1306-1.6.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-02-27 19:53:20.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/examples/displayio_ssd1306_64x32_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-02-27 19:53:20.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/examples/displayio_ssd1306_featherwing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-02-27 19:53:20.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/examples/displayio_ssd1306_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-02-27 19:53:20.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-02-27 19:53:12.000000 adafruit-circuitpython-displayio-ssd1306-1.6.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 19:53:27.665422 adafruit-circuitpython-displayio-ssd1306-1.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.651362 adafruit-circuitpython-displayio-ssd1306-1.6.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.643362 adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.647362 adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.647362 adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.647362 adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-26 16:24:16.651362 adafruit-circuitpython-displayio-ssd1306-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3268 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.647362 adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_circuitpython_displayio_ssd1306.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4056 2023-05-26 16:24:16.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_circuitpython_displayio_ssd1306.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-26 16:24:16.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_circuitpython_displayio_ssd1306.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:24:16.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_circuitpython_displayio_ssd1306.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:24:16.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_circuitpython_displayio_ssd1306.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 16:24:16.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_circuitpython_displayio_ssd1306.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-26 16:24:09.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_displayio_ssd1306.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.651362 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.651362 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5763 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:16.651362 adafruit-circuitpython-displayio-ssd1306-1.6.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1735 2023-05-26 16:24:09.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/examples/displayio_ssd1306_64x32_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-05-26 16:24:09.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/examples/displayio_ssd1306_featherwing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-26 16:24:09.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/examples/displayio_ssd1306_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-26 16:24:09.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:24:00.000000 adafruit-circuitpython-displayio-ssd1306-1.6.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:24:16.651362 adafruit-circuitpython-displayio-ssd1306-1.6.1/setup.cfg
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/.gitignore` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/.pre-commit-config.yaml` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/.pylintrc` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSE` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSES/MIT.txt` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/PKG-INFO` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-ssd1306
-Version: 1.6.0
+Version: 1.6.1
 Summary: DisplayIO driver for SSD1306 monochrome displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SSD1306
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_ssd1306,displayio,ssd1306,oled
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/README.rst` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_circuitpython_displayio_ssd1306.egg-info/PKG-INFO` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_circuitpython_displayio_ssd1306.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-ssd1306
-Version: 1.6.0
+Version: 1.6.1
 Summary: DisplayIO driver for SSD1306 monochrome displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SSD1306
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_ssd1306,displayio,ssd1306,oled
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_circuitpython_displayio_ssd1306.egg-info/SOURCES.txt` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_circuitpython_displayio_ssd1306.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/adafruit_displayio_ssd1306.py` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/adafruit_displayio_ssd1306.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import displayio
 
 try:
     from typing import Union
 except ImportError:
     pass
 
-__version__ = "1.6.0"
+__version__ = "1.6.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SSD1306.git"
 
 # Sequence from page 19 here: https://cdn-shop.adafruit.com/datasheets/UG-2864HSWEG01+user+guide.pdf
 _INIT_SEQUENCE = (
     b"\xAE\x00"  # DISPLAY_OFF
     b"\x20\x01\x00"  # Set memory addressing to horizontal mode.
     b"\x81\x01\xcf"  # set contrast control
```

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/_static/favicon.ico` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/conf.py` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/conf.py`

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

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/docs/index.rst` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/examples/displayio_ssd1306_64x32_simpletest.py` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/examples/displayio_ssd1306_64x32_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/examples/displayio_ssd1306_featherwing.py` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/examples/displayio_ssd1306_featherwing.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/examples/displayio_ssd1306_simpletest.py` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/examples/displayio_ssd1306_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-ssd1306-1.6.0/pyproject.toml` & `adafruit-circuitpython-displayio-ssd1306-1.6.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-displayio-ssd1306"
 description = "DisplayIO driver for SSD1306 monochrome displays"
-version = "1.6.0"
+version = "1.6.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SSD1306"}
 keywords = [
     "adafruit",
```

