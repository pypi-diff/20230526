# Comparing `tmp/adafruit-circuitpython-mlx90393-2.1.0.tar.gz` & `tmp/adafruit-circuitpython-mlx90393-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mlx90393-2.1.0.tar", last modified: Fri Feb 17 18:39:01 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-mlx90393-2.1.1.tar", last modified: Fri May 26 16:24:18 2023, max compression
```

## Comparing `adafruit-circuitpython-mlx90393-2.1.0.tar` & `adafruit-circuitpython-mlx90393-2.1.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.922649 adafruit-circuitpython-mlx90393-2.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.918649 adafruit-circuitpython-mlx90393-2.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.918649 adafruit-circuitpython-mlx90393-2.1.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.918649 adafruit-circuitpython-mlx90393-2.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.918649 adafruit-circuitpython-mlx90393-2.1.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-02-17 18:39:01.922649 adafruit-circuitpython-mlx90393-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.922649 adafruit-circuitpython-mlx90393-2.1.0/adafruit_circuitpython_mlx90393.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-02-17 18:39:01.000000 adafruit-circuitpython-mlx90393-2.1.0/adafruit_circuitpython_mlx90393.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-02-17 18:39:01.000000 adafruit-circuitpython-mlx90393-2.1.0/adafruit_circuitpython_mlx90393.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-17 18:39:01.000000 adafruit-circuitpython-mlx90393-2.1.0/adafruit_circuitpython_mlx90393.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-02-17 18:39:01.000000 adafruit-circuitpython-mlx90393-2.1.0/adafruit_circuitpython_mlx90393.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-17 18:39:01.000000 adafruit-circuitpython-mlx90393-2.1.0/adafruit_circuitpython_mlx90393.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    18430 2023-02-17 18:38:54.000000 adafruit-circuitpython-mlx90393-2.1.0/adafruit_mlx90393.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.922649 adafruit-circuitpython-mlx90393-2.1.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.922649 adafruit-circuitpython-mlx90393-2.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-17 18:39:01.922649 adafruit-circuitpython-mlx90393-2.1.0/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-02-17 18:38:54.000000 adafruit-circuitpython-mlx90393-2.1.0/examples/mlx90393_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-02-17 18:38:54.000000 adafruit-circuitpython-mlx90393-2.1.0/examples/mlx90393_temperature.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-02-17 18:38:54.000000 adafruit-circuitpython-mlx90393-2.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-02-17 18:38:45.000000 adafruit-circuitpython-mlx90393-2.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-17 18:39:01.922649 adafruit-circuitpython-mlx90393-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.256574 adafruit-circuitpython-mlx90393-2.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.252574 adafruit-circuitpython-mlx90393-2.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.252574 adafruit-circuitpython-mlx90393-2.1.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.252574 adafruit-circuitpython-mlx90393-2.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.256574 adafruit-circuitpython-mlx90393-2.1.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-26 16:24:18.256574 adafruit-circuitpython-mlx90393-2.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3172 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.256574 adafruit-circuitpython-mlx90393-2.1.1/adafruit_circuitpython_mlx90393.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-05-26 16:24:18.000000 adafruit-circuitpython-mlx90393-2.1.1/adafruit_circuitpython_mlx90393.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-26 16:24:18.000000 adafruit-circuitpython-mlx90393-2.1.1/adafruit_circuitpython_mlx90393.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:24:18.000000 adafruit-circuitpython-mlx90393-2.1.1/adafruit_circuitpython_mlx90393.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 16:24:18.000000 adafruit-circuitpython-mlx90393-2.1.1/adafruit_circuitpython_mlx90393.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:24:18.000000 adafruit-circuitpython-mlx90393-2.1.1/adafruit_circuitpython_mlx90393.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18430 2023-05-26 16:24:09.000000 adafruit-circuitpython-mlx90393-2.1.1/adafruit_mlx90393.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.256574 adafruit-circuitpython-mlx90393-2.1.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.256574 adafruit-circuitpython-mlx90393-2.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:24:18.256574 adafruit-circuitpython-mlx90393-2.1.1/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      717 2023-05-26 16:24:09.000000 adafruit-circuitpython-mlx90393-2.1.1/examples/mlx90393_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-26 16:24:09.000000 adafruit-circuitpython-mlx90393-2.1.1/examples/mlx90393_temperature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-26 16:24:09.000000 adafruit-circuitpython-mlx90393-2.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-26 16:23:58.000000 adafruit-circuitpython-mlx90393-2.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:24:18.256574 adafruit-circuitpython-mlx90393-2.1.1/setup.cfg
```

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mlx90393-2.1.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/.gitignore` & `adafruit-circuitpython-mlx90393-2.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/.pre-commit-config.yaml` & `adafruit-circuitpython-mlx90393-2.1.1/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/.pylintrc` & `adafruit-circuitpython-mlx90393-2.1.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mlx90393-2.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/LICENSE` & `adafruit-circuitpython-mlx90393-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mlx90393-2.1.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/LICENSES/MIT.txt` & `adafruit-circuitpython-mlx90393-2.1.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mlx90393-2.1.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/PKG-INFO` & `adafruit-circuitpython-mlx90393-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mlx90393
-Version: 2.1.0
+Version: 2.1.1
 Summary: CircuitPython driver for the MLX90393 3-axis magnetometer.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MLX90393
 Keywords: adafruit,three-axis,magnetometer,magnet,mlx90393,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/README.rst` & `adafruit-circuitpython-mlx90393-2.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/adafruit_circuitpython_mlx90393.egg-info/PKG-INFO` & `adafruit-circuitpython-mlx90393-2.1.1/adafruit_circuitpython_mlx90393.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mlx90393
-Version: 2.1.0
+Version: 2.1.1
 Summary: CircuitPython driver for the MLX90393 3-axis magnetometer.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MLX90393
 Keywords: adafruit,three-axis,magnetometer,magnet,mlx90393,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/adafruit_circuitpython_mlx90393.egg-info/SOURCES.txt` & `adafruit-circuitpython-mlx90393-2.1.1/adafruit_circuitpython_mlx90393.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/adafruit_mlx90393.py` & `adafruit-circuitpython-mlx90393-2.1.1/adafruit_mlx90393.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 try:
     from typing import Tuple
     from circuitpython_typing import ReadableBuffer
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "2.1.0"
+__version__ = "2.1.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MLX90393.git"
 
 _CMD_SB = const(0b00010000)  # Start burst mode
 _CMD_SW = const(0b00100000)  # Start wakeup on change mode
 _CMD_SM = const(0b00110000)  # Start single-measurement mode
 _CMD_RM = const(0b01000000)  # Read measurement
 _CMD_RR = const(0b01010000)  # Read register
```

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/docs/_static/favicon.ico` & `adafruit-circuitpython-mlx90393-2.1.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/docs/conf.py` & `adafruit-circuitpython-mlx90393-2.1.1/docs/conf.py`

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

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/docs/index.rst` & `adafruit-circuitpython-mlx90393-2.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/examples/mlx90393_simpletest.py` & `adafruit-circuitpython-mlx90393-2.1.1/examples/mlx90393_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/examples/mlx90393_temperature.py` & `adafruit-circuitpython-mlx90393-2.1.1/examples/mlx90393_temperature.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mlx90393-2.1.0/pyproject.toml` & `adafruit-circuitpython-mlx90393-2.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mlx90393"
 description = "CircuitPython driver for the MLX90393 3-axis magnetometer."
-version = "2.1.0"
+version = "2.1.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MLX90393"}
 keywords = [
     "adafruit",
```

