# Comparing `tmp/adafruit-circuitpython-thermistor-3.4.7.tar.gz` & `tmp/adafruit-circuitpython-thermistor-3.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-thermistor-3.4.7.tar", last modified: Fri Aug 26 02:33:57 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-thermistor-3.4.8.tar", last modified: Fri May 26 16:04:46 2023, max compression
```

## Comparing `adafruit-circuitpython-thermistor-3.4.7.tar` & `adafruit-circuitpython-thermistor-3.4.8.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.473220 adafruit-circuitpython-thermistor-3.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3900 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3111 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/adafruit_circuitpython_thermistor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3900 2022-08-26 02:33:57.000000 adafruit-circuitpython-thermistor-3.4.7/adafruit_circuitpython_thermistor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      947 2022-08-26 02:33:57.000000 adafruit-circuitpython-thermistor-3.4.7/adafruit_circuitpython_thermistor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:33:57.000000 adafruit-circuitpython-thermistor-3.4.7/adafruit_circuitpython_thermistor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:33:57.000000 adafruit-circuitpython-thermistor-3.4.7/adafruit_circuitpython_thermistor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       20 2022-08-26 02:33:57.000000 adafruit-circuitpython-thermistor-3.4.7/adafruit_circuitpython_thermistor.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4531 2022-08-26 02:33:49.000000 adafruit-circuitpython-thermistor-3.4.7/adafruit_thermistor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5603 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      194 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1202 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      834 2022-08-26 02:33:49.000000 adafruit-circuitpython-thermistor-3.4.7/examples/thermistor_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1246 2022-08-26 02:33:49.000000 adafruit-circuitpython-thermistor-3.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:33:41.000000 adafruit-circuitpython-thermistor-3.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:33:57.477220 adafruit-circuitpython-thermistor-3.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.693308 adafruit-circuitpython-thermistor-3.4.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.685307 adafruit-circuitpython-thermistor-3.4.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.689308 adafruit-circuitpython-thermistor-3.4.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.689308 adafruit-circuitpython-thermistor-3.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.689308 adafruit-circuitpython-thermistor-3.4.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-26 16:04:46.693308 adafruit-circuitpython-thermistor-3.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.689308 adafruit-circuitpython-thermistor-3.4.8/adafruit_circuitpython_thermistor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3900 2023-05-26 16:04:46.000000 adafruit-circuitpython-thermistor-3.4.8/adafruit_circuitpython_thermistor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-26 16:04:46.000000 adafruit-circuitpython-thermistor-3.4.8/adafruit_circuitpython_thermistor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:04:46.000000 adafruit-circuitpython-thermistor-3.4.8/adafruit_circuitpython_thermistor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:04:46.000000 adafruit-circuitpython-thermistor-3.4.8/adafruit_circuitpython_thermistor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:04:46.000000 adafruit-circuitpython-thermistor-3.4.8/adafruit_circuitpython_thermistor.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-26 16:04:39.000000 adafruit-circuitpython-thermistor-3.4.8/adafruit_thermistor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.689308 adafruit-circuitpython-thermistor-3.4.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.689308 adafruit-circuitpython-thermistor-3.4.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:04:46.693308 adafruit-circuitpython-thermistor-3.4.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 16:04:39.000000 adafruit-circuitpython-thermistor-3.4.8/examples/thermistor_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-26 16:04:39.000000 adafruit-circuitpython-thermistor-3.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:04:30.000000 adafruit-circuitpython-thermistor-3.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:04:46.693308 adafruit-circuitpython-thermistor-3.4.8/setup.cfg
```

### Comparing `adafruit-circuitpython-thermistor-3.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-thermistor-3.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/.gitignore` & `adafruit-circuitpython-thermistor-3.4.8/.gitignore`

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

### Comparing `adafruit-circuitpython-thermistor-3.4.7/.pre-commit-config.yaml` & `adafruit-circuitpython-thermistor-3.4.8/.pre-commit-config.yaml`

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
-    rev: v2.11.1
+    rev: v2.17.4
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-thermistor-3.4.7/.pylintrc` & `adafruit-circuitpython-thermistor-3.4.8/.pylintrc`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
+# SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: Unlicense
 
 [MASTER]
 
 # A comma-separated list of package or module names from where C extensions may
 # be loaded. Extensions are loading into the active Python interpreter and may
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
-disable=print-statement,parameter-unpacking,unpacking-in-except,old-raise-syntax,backtick,long-suffix,old-ne-operator,old-octal-literal,import-star-module-level,raw-checker-failed,bad-inline-option,locally-disabled,locally-enabled,file-ignored,suppressed-message,useless-suppression,deprecated-pragma,apply-builtin,basestring-builtin,buffer-builtin,cmp-builtin,coerce-builtin,execfile-builtin,file-builtin,long-builtin,raw_input-builtin,reduce-builtin,standarderror-builtin,unicode-builtin,xrange-builtin,coerce-method,delslice-method,getslice-method,setslice-method,no-absolute-import,old-division,dict-iter-method,dict-view-method,next-method-called,metaclass-assignment,indexing-exception,raising-string,reload-builtin,oct-method,hex-method,nonzero-method,cmp-method,input-builtin,round-builtin,intern-builtin,unichr-builtin,map-builtin-not-iterating,zip-builtin-not-iterating,range-builtin-not-iterating,filter-builtin-not-iterating,using-cmp-argument,eq-without-hash,div-method,idiv-method,rdiv-method,exception-message-attribute,invalid-str-codec,sys-max-int,bad-python3-import,deprecated-string-function,deprecated-str-translate-call,import-error,bad-continuation,unspecified-encoding
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

### Comparing `adafruit-circuitpython-thermistor-3.4.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-thermistor-3.4.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/LICENSE` & `adafruit-circuitpython-thermistor-3.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-thermistor-3.4.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/LICENSES/MIT.txt` & `adafruit-circuitpython-thermistor-3.4.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-thermistor-3.4.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/PKG-INFO` & `adafruit-circuitpython-thermistor-3.4.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-thermistor
-Version: 3.4.7
+Version: 3.4.8
 Summary: CircuitPython library for Thermistor thermal resistor temperature sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Thermistor
 Keywords: adafruit,thermal,resistor,temperature,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-thermistor-3.4.7/README.rst` & `adafruit-circuitpython-thermistor-3.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/adafruit_circuitpython_thermistor.egg-info/PKG-INFO` & `adafruit-circuitpython-thermistor-3.4.8/adafruit_circuitpython_thermistor.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-thermistor
-Version: 3.4.7
+Version: 3.4.8
 Summary: CircuitPython library for Thermistor thermal resistor temperature sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Thermistor
 Keywords: adafruit,thermal,resistor,temperature,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-thermistor-3.4.7/adafruit_circuitpython_thermistor.egg-info/SOURCES.txt` & `adafruit-circuitpython-thermistor-3.4.8/adafruit_circuitpython_thermistor.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_thermistor.py
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
 adafruit_circuitpython_thermistor.egg-info/PKG-INFO
 adafruit_circuitpython_thermistor.egg-info/SOURCES.txt
 adafruit_circuitpython_thermistor.egg-info/dependency_links.txt
 adafruit_circuitpython_thermistor.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-thermistor-3.4.7/adafruit_thermistor.py` & `adafruit-circuitpython-thermistor-3.4.8/adafruit_thermistor.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 try:
     import typing  # pylint: disable=unused-import
     import microcontroller
 except ImportError:
     pass
 
-__version__ = "3.4.7"
+__version__ = "3.4.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Thermistor.git"
 
 
 class Thermistor:
     """
     :param ~microcontroller.Pin pin: Analog pin used for the thermistor
     :param int series_resistor: resistance in series between you analog input and the
```

### Comparing `adafruit-circuitpython-thermistor-3.4.7/docs/_static/favicon.ico` & `adafruit-circuitpython-thermistor-3.4.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/docs/conf.py` & `adafruit-circuitpython-thermistor-3.4.8/docs/conf.py`

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
     "sphinx.ext.viewcode",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
```

### Comparing `adafruit-circuitpython-thermistor-3.4.7/docs/index.rst` & `adafruit-circuitpython-thermistor-3.4.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/examples/thermistor_simpletest.py` & `adafruit-circuitpython-thermistor-3.4.8/examples/thermistor_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-thermistor-3.4.7/pyproject.toml` & `adafruit-circuitpython-thermistor-3.4.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-thermistor"
 description = "CircuitPython library for Thermistor thermal resistor temperature sensor."
-version = "3.4.7"
+version = "3.4.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Thermistor"}
 keywords = [
     "adafruit",
```

