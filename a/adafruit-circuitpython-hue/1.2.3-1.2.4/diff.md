# Comparing `tmp/adafruit-circuitpython-hue-1.2.3.tar.gz` & `tmp/adafruit-circuitpython-hue-1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-hue-1.2.3.tar", last modified: Fri Aug 26 02:41:24 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-hue-1.2.4.tar", last modified: Fri May 26 15:54:34 2023, max compression
```

## Comparing `adafruit-circuitpython-hue-1.2.3.tar` & `adafruit-circuitpython-hue-1.2.4.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.620760 adafruit-circuitpython-hue-1.2.3/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.612760 adafruit-circuitpython-hue-1.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.616760 adafruit-circuitpython-hue-1.2.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.616760 adafruit-circuitpython-hue-1.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.616760 adafruit-circuitpython-hue-1.2.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-08-26 02:41:24.616760 adafruit-circuitpython-hue-1.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3506 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.616760 adafruit-circuitpython-hue-1.2.3/adafruit_circuitpython_hue.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4255 2022-08-26 02:41:24.000000 adafruit-circuitpython-hue-1.2.3/adafruit_circuitpython_hue.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-08-26 02:41:24.000000 adafruit-circuitpython-hue-1.2.3/adafruit_circuitpython_hue.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:41:24.000000 adafruit-circuitpython-hue-1.2.3/adafruit_circuitpython_hue.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      122 2022-08-26 02:41:24.000000 adafruit-circuitpython-hue-1.2.3/adafruit_circuitpython_hue.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-26 02:41:24.000000 adafruit-circuitpython-hue-1.2.3/adafruit_circuitpython_hue.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9601 2022-08-26 02:41:14.000000 adafruit-circuitpython-hue-1.2.3/adafruit_hue.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.616760 adafruit-circuitpython-hue-1.2.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.616760 adafruit-circuitpython-hue-1.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      262 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5614 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      180 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      968 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:41:24.616760 adafruit-circuitpython-hue-1.2.3/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2156 2022-08-26 02:41:14.000000 adafruit-circuitpython-hue-1.2.3/examples/hue_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1213 2022-08-26 02:41:14.000000 adafruit-circuitpython-hue-1.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-08-26 02:41:02.000000 adafruit-circuitpython-hue-1.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:41:24.620760 adafruit-circuitpython-hue-1.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.384331 adafruit-circuitpython-hue-1.2.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.376331 adafruit-circuitpython-hue-1.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.380331 adafruit-circuitpython-hue-1.2.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.380331 adafruit-circuitpython-hue-1.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.380331 adafruit-circuitpython-hue-1.2.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-26 15:54:34.384331 adafruit-circuitpython-hue-1.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.380331 adafruit-circuitpython-hue-1.2.4/adafruit_circuitpython_hue.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-05-26 15:54:34.000000 adafruit-circuitpython-hue-1.2.4/adafruit_circuitpython_hue.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-26 15:54:34.000000 adafruit-circuitpython-hue-1.2.4/adafruit_circuitpython_hue.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:54:34.000000 adafruit-circuitpython-hue-1.2.4/adafruit_circuitpython_hue.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-26 15:54:34.000000 adafruit-circuitpython-hue-1.2.4/adafruit_circuitpython_hue.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 15:54:34.000000 adafruit-circuitpython-hue-1.2.4/adafruit_circuitpython_hue.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9601 2023-05-26 15:54:26.000000 adafruit-circuitpython-hue-1.2.4/adafruit_hue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.384331 adafruit-circuitpython-hue-1.2.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.384331 adafruit-circuitpython-hue-1.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5642 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:54:34.384331 adafruit-circuitpython-hue-1.2.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-26 15:54:26.000000 adafruit-circuitpython-hue-1.2.4/examples/hue_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-26 15:54:26.000000 adafruit-circuitpython-hue-1.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-26 15:54:13.000000 adafruit-circuitpython-hue-1.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:54:34.384331 adafruit-circuitpython-hue-1.2.4/setup.cfg
```

### Comparing `adafruit-circuitpython-hue-1.2.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-hue-1.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/.gitignore` & `adafruit-circuitpython-hue-1.2.4/.gitignore`

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

### Comparing `adafruit-circuitpython-hue-1.2.3/.pre-commit-config.yaml` & `adafruit-circuitpython-hue-1.2.4/.pre-commit-config.yaml`

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

### Comparing `adafruit-circuitpython-hue-1.2.3/.pylintrc` & `adafruit-circuitpython-hue-1.2.4/.pylintrc`

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

### Comparing `adafruit-circuitpython-hue-1.2.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-hue-1.2.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/LICENSE` & `adafruit-circuitpython-hue-1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-hue-1.2.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/LICENSES/MIT.txt` & `adafruit-circuitpython-hue-1.2.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-hue-1.2.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/PKG-INFO` & `adafruit-circuitpython-hue-1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-hue
-Version: 1.2.3
+Version: 1.2.4
 Summary: CircuitPython helper library for the Philips Hue
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Hue
 Keywords: adafruit,blinka,circuitpython,micropython,hue,philips,bulb,light,bridge
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-hue-1.2.3/README.rst` & `adafruit-circuitpython-hue-1.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/adafruit_circuitpython_hue.egg-info/PKG-INFO` & `adafruit-circuitpython-hue-1.2.4/adafruit_circuitpython_hue.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-hue
-Version: 1.2.3
+Version: 1.2.4
 Summary: CircuitPython helper library for the Philips Hue
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Hue
 Keywords: adafruit,blinka,circuitpython,micropython,hue,philips,bulb,light,bridge
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-hue-1.2.3/adafruit_circuitpython_hue.egg-info/SOURCES.txt` & `adafruit-circuitpython-hue-1.2.4/adafruit_circuitpython_hue.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 adafruit_hue.py
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
 adafruit_circuitpython_hue.egg-info/PKG-INFO
 adafruit_circuitpython_hue.egg-info/SOURCES.txt
 adafruit_circuitpython_hue.egg-info/dependency_links.txt
 adafruit_circuitpython_hue.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-hue-1.2.3/adafruit_hue.py` & `adafruit-circuitpython-hue-1.2.4/adafruit_hue.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 try:
     from typing import Optional, List, Union, Sequence, Any
     from circuitpython_typing.http import HTTPProtocol
 except ImportError:
     pass
 
-__version__ = "1.2.3"
+__version__ = "1.2.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Hue.git"
 
 
 class Bridge:
     """
     HTTP Interface for interacting with a Philips Hue Bridge.
     """
```

### Comparing `adafruit-circuitpython-hue-1.2.3/docs/_static/favicon.ico` & `adafruit-circuitpython-hue-1.2.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/docs/conf.py` & `adafruit-circuitpython-hue-1.2.4/docs/conf.py`

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

### Comparing `adafruit-circuitpython-hue-1.2.3/docs/index.rst` & `adafruit-circuitpython-hue-1.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/examples/hue_simpletest.py` & `adafruit-circuitpython-hue-1.2.4/examples/hue_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-hue-1.2.3/pyproject.toml` & `adafruit-circuitpython-hue-1.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-hue"
 description = "CircuitPython helper library for the Philips Hue"
-version = "1.2.3"
+version = "1.2.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Hue"}
 keywords = [
     "adafruit",
```

