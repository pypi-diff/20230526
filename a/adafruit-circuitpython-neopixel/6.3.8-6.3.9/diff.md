# Comparing `tmp/adafruit-circuitpython-neopixel-6.3.8.tar.gz` & `tmp/adafruit-circuitpython-neopixel-6.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-neopixel-6.3.8.tar", last modified: Fri Jan 20 18:29:10 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-neopixel-6.3.9.tar", last modified: Fri May 26 16:05:38 2023, max compression
```

## Comparing `adafruit-circuitpython-neopixel-6.3.8.tar` & `adafruit-circuitpython-neopixel-6.3.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.473460 adafruit-circuitpython-neopixel-6.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/adafruit_circuitpython_neopixel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-01-20 18:29:10.000000 adafruit-circuitpython-neopixel-6.3.8/adafruit_circuitpython_neopixel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-01-20 18:29:10.000000 adafruit-circuitpython-neopixel-6.3.8/adafruit_circuitpython_neopixel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-20 18:29:10.000000 adafruit-circuitpython-neopixel-6.3.8/adafruit_circuitpython_neopixel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-01-20 18:29:10.000000 adafruit-circuitpython-neopixel-6.3.8/adafruit_circuitpython_neopixel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-20 18:29:10.000000 adafruit-circuitpython-neopixel-6.3.8/adafruit_circuitpython_neopixel.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-01-20 18:29:02.000000 adafruit-circuitpython-neopixel-6.3.8/examples/neopixel_pixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-01-20 18:29:02.000000 adafruit-circuitpython-neopixel-6.3.8/examples/neopixel_rainbowio_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-01-20 18:29:02.000000 adafruit-circuitpython-neopixel-6.3.8/examples/neopixel_rpi_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-01-20 18:29:02.000000 adafruit-circuitpython-neopixel-6.3.8/examples/neopixel_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-01-20 18:29:02.000000 adafruit-circuitpython-neopixel-6.3.8/neopixel.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-01-20 18:29:02.000000 adafruit-circuitpython-neopixel-6.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-01-20 18:28:52.000000 adafruit-circuitpython-neopixel-6.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-20 18:29:10.477460 adafruit-circuitpython-neopixel-6.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.584894 adafruit-circuitpython-neopixel-6.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.580894 adafruit-circuitpython-neopixel-6.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.580894 adafruit-circuitpython-neopixel-6.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.580894 adafruit-circuitpython-neopixel-6.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.580894 adafruit-circuitpython-neopixel-6.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-26 16:05:38.584894 adafruit-circuitpython-neopixel-6.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.580894 adafruit-circuitpython-neopixel-6.3.9/adafruit_circuitpython_neopixel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5958 2023-05-26 16:05:38.000000 adafruit-circuitpython-neopixel-6.3.9/adafruit_circuitpython_neopixel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 16:05:38.000000 adafruit-circuitpython-neopixel-6.3.9/adafruit_circuitpython_neopixel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:05:38.000000 adafruit-circuitpython-neopixel-6.3.9/adafruit_circuitpython_neopixel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 16:05:38.000000 adafruit-circuitpython-neopixel-6.3.9/adafruit_circuitpython_neopixel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 16:05:38.000000 adafruit-circuitpython-neopixel-6.3.9/adafruit_circuitpython_neopixel.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.584894 adafruit-circuitpython-neopixel-6.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.584894 adafruit-circuitpython-neopixel-6.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5454 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:05:38.584894 adafruit-circuitpython-neopixel-6.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-05-26 16:05:30.000000 adafruit-circuitpython-neopixel-6.3.9/examples/neopixel_pixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 16:05:30.000000 adafruit-circuitpython-neopixel-6.3.9/examples/neopixel_rainbowio_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-26 16:05:30.000000 adafruit-circuitpython-neopixel-6.3.9/examples/neopixel_rpi_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-26 16:05:30.000000 adafruit-circuitpython-neopixel-6.3.9/examples/neopixel_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-05-26 16:05:30.000000 adafruit-circuitpython-neopixel-6.3.9/neopixel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-26 16:05:30.000000 adafruit-circuitpython-neopixel-6.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 16:05:20.000000 adafruit-circuitpython-neopixel-6.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:05:38.584894 adafruit-circuitpython-neopixel-6.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-neopixel-6.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-neopixel-6.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/.gitignore` & `adafruit-circuitpython-neopixel-6.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-neopixel-6.3.9/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-neopixel-6.3.8/.pylintrc` & `adafruit-circuitpython-neopixel-6.3.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-neopixel-6.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-neopixel-6.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/LICENSE` & `adafruit-circuitpython-neopixel-6.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-neopixel-6.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-neopixel-6.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-neopixel-6.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/PKG-INFO` & `adafruit-circuitpython-neopixel-6.3.9/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neopixel
-Version: 6.3.8
+Version: 6.3.9
 Summary: CircuitPython library for NeoPixel LEDs.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel
 Keywords: adafruit,neopixel,rgb,rgbw,led,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -124,14 +124,40 @@
 
     import board
     import neopixel
 
     pixel = neopixel.NeoPixel(board.D0, 1, pixel_order=neopixel.RGBW)
     pixel[0] = (30, 0, 20, 10)
 
+Setup for sudo-less usage on Raspberry Pi boards
+================================================
+1. Enable both SPI and Serial port hardware (Serial interface). Do it by ``raspi-config`` tool or manually by adding
+
+   ::
+
+      dtparam=spi=on
+      enable_uart=1
+
+   to the ``/boot/config.txt``
+
+2. Reboot the Pi to apply the changes - the hardware setup takes place during boot.
+3. Connect LED's DIN to ``GPIO10`` (physical pin 19)
+
+When initializing the ``NeoPixel`` object **always** do it with ``board.D10`` (GPIO10)
+
+.. code-block:: python
+
+    import board
+    import neopixel
+
+    DATA_PIN = board.D10
+    pixel = neopixel.NeoPixel(DATA_PIN, ...)
+
+Now you can execute the code using ``python`` without ``sudo``
+
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/neopixel/en/latest/>`_.
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-neopixel-6.3.8/README.rst` & `adafruit-circuitpython-neopixel-6.3.9/README.rst`

 * *Files 11% similar despite different names*

```diff
@@ -106,14 +106,40 @@
 
     import board
     import neopixel
 
     pixel = neopixel.NeoPixel(board.D0, 1, pixel_order=neopixel.RGBW)
     pixel[0] = (30, 0, 20, 10)
 
+Setup for sudo-less usage on Raspberry Pi boards
+================================================
+1. Enable both SPI and Serial port hardware (Serial interface). Do it by ``raspi-config`` tool or manually by adding
+
+   ::
+
+      dtparam=spi=on
+      enable_uart=1
+
+   to the ``/boot/config.txt``
+
+2. Reboot the Pi to apply the changes - the hardware setup takes place during boot.
+3. Connect LED's DIN to ``GPIO10`` (physical pin 19)
+
+When initializing the ``NeoPixel`` object **always** do it with ``board.D10`` (GPIO10)
+
+.. code-block:: python
+
+    import board
+    import neopixel
+
+    DATA_PIN = board.D10
+    pixel = neopixel.NeoPixel(DATA_PIN, ...)
+
+Now you can execute the code using ``python`` without ``sudo``
+
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/neopixel/en/latest/>`_.
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-neopixel-6.3.8/adafruit_circuitpython_neopixel.egg-info/PKG-INFO` & `adafruit-circuitpython-neopixel-6.3.9/adafruit_circuitpython_neopixel.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neopixel
-Version: 6.3.8
+Version: 6.3.9
 Summary: CircuitPython library for NeoPixel LEDs.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel
 Keywords: adafruit,neopixel,rgb,rgbw,led,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
@@ -124,14 +124,40 @@
 
     import board
     import neopixel
 
     pixel = neopixel.NeoPixel(board.D0, 1, pixel_order=neopixel.RGBW)
     pixel[0] = (30, 0, 20, 10)
 
+Setup for sudo-less usage on Raspberry Pi boards
+================================================
+1. Enable both SPI and Serial port hardware (Serial interface). Do it by ``raspi-config`` tool or manually by adding
+
+   ::
+
+      dtparam=spi=on
+      enable_uart=1
+
+   to the ``/boot/config.txt``
+
+2. Reboot the Pi to apply the changes - the hardware setup takes place during boot.
+3. Connect LED's DIN to ``GPIO10`` (physical pin 19)
+
+When initializing the ``NeoPixel`` object **always** do it with ``board.D10`` (GPIO10)
+
+.. code-block:: python
+
+    import board
+    import neopixel
+
+    DATA_PIN = board.D10
+    pixel = neopixel.NeoPixel(DATA_PIN, ...)
+
+Now you can execute the code using ``python`` without ``sudo``
+
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/neopixel/en/latest/>`_.
 
 For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-neopixel-6.3.8/adafruit_circuitpython_neopixel.egg-info/SOURCES.txt` & `adafruit-circuitpython-neopixel-6.3.9/adafruit_circuitpython_neopixel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-neopixel-6.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/docs/conf.py` & `adafruit-circuitpython-neopixel-6.3.9/docs/conf.py`

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
     "sphinx.ext.viewcode",
 ]
 
 autodoc_mock_imports = ["neopixel_write"]
 
 intersphinx_mapping = {
```

### Comparing `adafruit-circuitpython-neopixel-6.3.8/docs/index.rst` & `adafruit-circuitpython-neopixel-6.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/examples/neopixel_pixel.py` & `adafruit-circuitpython-neopixel-6.3.9/examples/neopixel_pixel.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/examples/neopixel_rainbowio_simpletest.py` & `adafruit-circuitpython-neopixel-6.3.9/examples/neopixel_rainbowio_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/examples/neopixel_rpi_simpletest.py` & `adafruit-circuitpython-neopixel-6.3.9/examples/neopixel_rpi_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/examples/neopixel_simpletest.py` & `adafruit-circuitpython-neopixel-6.3.9/examples/neopixel_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neopixel-6.3.8/neopixel.py` & `adafruit-circuitpython-neopixel-6.3.9/neopixel.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     from typing import Optional, Type
     from types import TracebackType
     import microcontroller
 except ImportError:
     pass
 
 
-__version__ = "6.3.8"
+__version__ = "6.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel.git"
 
 
 # Pixel color order constants
 RGB = "RGB"
 """Red Green Blue"""
 GRB = "GRB"
```

### Comparing `adafruit-circuitpython-neopixel-6.3.8/pyproject.toml` & `adafruit-circuitpython-neopixel-6.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-neopixel"
 description = "CircuitPython library for NeoPixel LEDs."
-version = "6.3.8"
+version = "6.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_NeoPixel"}
 keywords = [
     "adafruit",
```

