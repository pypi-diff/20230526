# Comparing `tmp/adafruit-circuitpython-ble-beacon-1.0.1.tar.gz` & `tmp/adafruit-circuitpython-ble-beacon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-beacon-1.0.1.tar", last modified: Wed Sep 21 23:58:59 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-beacon-1.0.2.tar", last modified: Fri May 26 15:51:40 2023, max compression
```

## Comparing `adafruit-circuitpython-ble-beacon-1.0.1.tar` & `adafruit-circuitpython-ble-beacon-1.0.2.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2728 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1654 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6753 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3227 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      187 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5467 2022-09-21 23:58:51.000000 adafruit-circuitpython-ble-beacon-1.0.1/adafruit_ble_beacon.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/adafruit_circuitpython_ble_beacon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4007 2022-09-21 23:58:59.000000 adafruit-circuitpython-ble-beacon-1.0.1/adafruit_circuitpython_ble_beacon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-09-21 23:58:59.000000 adafruit-circuitpython-ble-beacon-1.0.1/adafruit_circuitpython_ble_beacon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 23:58:59.000000 adafruit-circuitpython-ble-beacon-1.0.1/adafruit_circuitpython_ble_beacon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-09-21 23:58:59.000000 adafruit-circuitpython-ble-beacon-1.0.1/adafruit_circuitpython_ble_beacon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-09-21 23:58:59.000000 adafruit-circuitpython-ble-beacon-1.0.1/adafruit_circuitpython_ble_beacon.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5912 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      976 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 23:58:59.435623 adafruit-circuitpython-ble-beacon-1.0.1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      603 2022-09-21 23:58:51.000000 adafruit-circuitpython-ble-beacon-1.0.1/examples/ble_beacon_sendtest.py
--rw-r--r--   0 runner    (1001) docker     (121)      661 2022-09-21 23:58:51.000000 adafruit-circuitpython-ble-beacon-1.0.1/examples/ble_beacon_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-09-21 23:58:51.000000 adafruit-circuitpython-ble-beacon-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      239 2022-09-21 23:58:40.000000 adafruit-circuitpython-ble-beacon-1.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-21 23:58:59.439623 adafruit-circuitpython-ble-beacon-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.481826 adafruit-circuitpython-ble-beacon-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.465826 adafruit-circuitpython-ble-beacon-1.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.473826 adafruit-circuitpython-ble-beacon-1.0.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.473826 adafruit-circuitpython-ble-beacon-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.473826 adafruit-circuitpython-ble-beacon-1.0.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-26 15:51:40.481826 adafruit-circuitpython-ble-beacon-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3227 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5467 2023-05-26 15:51:32.000000 adafruit-circuitpython-ble-beacon-1.0.2/adafruit_ble_beacon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.477826 adafruit-circuitpython-ble-beacon-1.0.2/adafruit_circuitpython_ble_beacon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-05-26 15:51:40.000000 adafruit-circuitpython-ble-beacon-1.0.2/adafruit_circuitpython_ble_beacon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-05-26 15:51:40.000000 adafruit-circuitpython-ble-beacon-1.0.2/adafruit_circuitpython_ble_beacon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:51:40.000000 adafruit-circuitpython-ble-beacon-1.0.2/adafruit_circuitpython_ble_beacon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 15:51:40.000000 adafruit-circuitpython-ble-beacon-1.0.2/adafruit_circuitpython_ble_beacon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 15:51:40.000000 adafruit-circuitpython-ble-beacon-1.0.2/adafruit_circuitpython_ble_beacon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.477826 adafruit-circuitpython-ble-beacon-1.0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.481826 adafruit-circuitpython-ble-beacon-1.0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:51:40.481826 adafruit-circuitpython-ble-beacon-1.0.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 15:51:32.000000 adafruit-circuitpython-ble-beacon-1.0.2/examples/ble_beacon_sendtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-26 15:51:32.000000 adafruit-circuitpython-ble-beacon-1.0.2/examples/ble_beacon_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-26 15:51:32.000000 adafruit-circuitpython-ble-beacon-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 15:51:22.000000 adafruit-circuitpython-ble-beacon-1.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:51:40.481826 adafruit-circuitpython-ble-beacon-1.0.2/setup.cfg
```

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-beacon-1.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/.gitignore` & `adafruit-circuitpython-ble-beacon-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-beacon-1.0.2/.pre-commit-config.yaml`

 * *Files 9% similar despite different names*

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
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string,duplicate-code
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/.pylintrc` & `adafruit-circuitpython-ble-beacon-1.0.2/.pylintrc`

 * *Files 24% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
 jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
-load-plugins=
+load-plugins=pylint.extensions.no_self_use
 
 # Pickle collected data for later comparisons.
 persistent=yes
 
 # Specify a configuration file.
 #rcfile=
 
@@ -50,16 +50,16 @@
 # option multiple times (only on the command line, not in the configuration
 # file where it should appear only once).You can also use "--disable=all" to
 # disable everything first and then reenable specific checks. For example, if
 # you want to run only the similarities checker, you can use "--disable=all
 # --enable=similarities". If you want to run only the classes checker, but have
 # no Warning level messages displayed, use"--disable=all --enable=classes
 # --disable=W"
-# disable=import-error,print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,pointless-string-statement,unspecified-encoding
+# disable=import-error,raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,deprecated-str-translate-call
+disable=raw-checker-failed,bad-inline-option,locally-disabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,import-error,pointless-string-statement,unspecified-encoding
 
 # Enable the message, report, category or checker with the given id(s). You can
 # either give multiple identifier separated by comma (,) or put this option
 # multiple time (only on the command line, not in the configuration file where
 # it should appear only once). See also the "--disable" option for examples.
 enable=
 
@@ -221,20 +221,14 @@
 
 # Maximum number of characters on a single line.
 max-line-length=100
 
 # Maximum number of lines in a module
 max-module-lines=1000
 
-# List of optional constructs for which whitespace checking is disabled. `dict-
-# separator` is used to allow tabulation in dicts, etc.: {1  : 1,\n222: 2}.
-# `trailing-comma` allows a space between comma and closing bracket: (a, ).
-# `empty-line` allows space-only lines.
-no-space-check=trailing-comma,dict-separator
-
 # Allow the body of a class to be on the same line as the declaration if body
 # contains single statement.
 single-line-class-stmt=no
 
 # Allow the body of an if to be on the same line as the test if there is no
 # else.
 single-line-if-stmt=no
@@ -253,81 +247,53 @@
 
 # Minimum lines number of a similarity.
 min-similarity-lines=12
 
 
 [BASIC]
 
-# Naming hint for argument names
-argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct argument names
 argument-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for attribute names
-attr-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct attribute names
 attr-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Bad variable names which should always be refused, separated by a comma
 bad-names=foo,bar,baz,toto,tutu,tata
 
-# Naming hint for class attribute names
-class-attribute-name-hint=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
-
 # Regular expression matching correct class attribute names
 class-attribute-rgx=([A-Za-z_][A-Za-z0-9_]{2,30}|(__.*__))$
 
-# Naming hint for class names
-# class-name-hint=[A-Z_][a-zA-Z0-9]+$
-class-name-hint=[A-Z_][a-zA-Z0-9_]+$
-
 # Regular expression matching correct class names
 # class-rgx=[A-Z_][a-zA-Z0-9]+$
 class-rgx=[A-Z_][a-zA-Z0-9_]+$
 
-# Naming hint for constant names
-const-name-hint=(([A-Z_][A-Z0-9_]*)|(__.*__))$
-
 # Regular expression matching correct constant names
 const-rgx=(([A-Z_][A-Z0-9_]*)|(__.*__))$
 
 # Minimum line length for functions/classes that require docstrings, shorter
 # ones are exempt.
 docstring-min-length=-1
 
-# Naming hint for function names
-function-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct function names
 function-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 # Good variable names which should always be accepted, separated by a comma
 # good-names=i,j,k,ex,Run,_
 good-names=r,g,b,w,i,j,k,n,x,y,z,ex,ok,Run,_
 
 # Include a hint for the correct naming format with invalid-name
 include-naming-hint=no
 
-# Naming hint for inline iteration names
-inlinevar-name-hint=[A-Za-z_][A-Za-z0-9_]*$
-
 # Regular expression matching correct inline iteration names
 inlinevar-rgx=[A-Za-z_][A-Za-z0-9_]*$
 
-# Naming hint for method names
-method-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct method names
 method-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
-# Naming hint for module names
-module-name-hint=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
-
 # Regular expression matching correct module names
 module-rgx=(([a-z_][a-z0-9_]*)|([A-Z][a-zA-Z0-9]+))$
 
 # Colon-delimited sets of names that determine each other's naming style when
 # the name regexes allow several styles.
 name-group=
 
@@ -335,17 +301,14 @@
 # not require a docstring.
 no-docstring-rgx=^_
 
 # List of decorators that produce properties, such as abc.abstractproperty. Add
 # to this list to register other decorators that produce valid properties.
 property-classes=abc.abstractproperty
 
-# Naming hint for variable names
-variable-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
-
 # Regular expression matching correct variable names
 variable-rgx=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
 
 
 [IMPORTS]
 
 # Allow wildcard imports from modules that define __all__.
@@ -429,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-beacon-1.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/LICENSE` & `adafruit-circuitpython-ble-beacon-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-beacon-1.0.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-beacon-1.0.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-beacon-1.0.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/PKG-INFO` & `adafruit-circuitpython-ble-beacon-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-beacon
-Version: 1.0.1
+Version: 1.0.2
 Summary: BLE Location Beacon for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/tekktrik/Adafruit_CircuitPython_BLE_Beacon
 Keywords: adafruit,blinka,circuitpython,micropython,ble-beacon,ble,beacon,location,proximity,distance,ibeacon
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/README.rst` & `adafruit-circuitpython-ble-beacon-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/adafruit_ble_beacon.py` & `adafruit-circuitpython-ble-beacon-1.0.2/adafruit_ble_beacon.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from adafruit_ble.advertising import Advertisement, AdvertisingDataField
 
 try:
     from typing import Optional, Union, Type, Tuple, Sequence
 except ImportError:
     pass
 
-__version__ = "1.0.1"
+__version__ = "1.0.2"
 __repo__ = "https://github.com/tekktrik/Adafruit_CircuitPython_BLE_Beacon.git"
 
 
 _MANUFACTURING_DATA_ADT = const(0xFF)
 
 _APPLE_COMPANY_ID = const(0x004C)
 _IBEACON_TYPE = const(0x02)
```

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/adafruit_circuitpython_ble_beacon.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-beacon-1.0.2/adafruit_circuitpython_ble_beacon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-beacon
-Version: 1.0.1
+Version: 1.0.2
 Summary: BLE Location Beacon for CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/tekktrik/Adafruit_CircuitPython_BLE_Beacon
 Keywords: adafruit,blinka,circuitpython,micropython,ble-beacon,ble,beacon,location,proximity,distance,ibeacon
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/adafruit_circuitpython_ble_beacon.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-beacon-1.0.2/adafruit_circuitpython_ble_beacon.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_ble_beacon.py
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_ble_beacon.egg-info/PKG-INFO
 adafruit_circuitpython_ble_beacon.egg-info/SOURCES.txt
 adafruit_circuitpython_ble_beacon.egg-info/dependency_links.txt
 adafruit_circuitpython_ble_beacon.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-beacon-1.0.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/docs/conf.py` & `adafruit-circuitpython-ble-beacon-1.0.2/docs/conf.py`

 * *Files 3% similar despite different names*

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

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/docs/index.rst` & `adafruit-circuitpython-ble-beacon-1.0.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/examples/ble_beacon_sendtest.py` & `adafruit-circuitpython-ble-beacon-1.0.2/examples/ble_beacon_sendtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/examples/ble_beacon_simpletest.py` & `adafruit-circuitpython-ble-beacon-1.0.2/examples/ble_beacon_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-beacon-1.0.1/pyproject.toml` & `adafruit-circuitpython-ble-beacon-1.0.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ble-beacon"
 description = "BLE Location Beacon for CircuitPython"
-version = "1.0.1"
+version = "1.0.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/tekktrik/Adafruit_CircuitPython_BLE_Beacon"}
 keywords = [
     "adafruit",
```

