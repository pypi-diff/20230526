# Comparing `tmp/adafruit-circuitpython-simpleio-3.0.8.tar.gz` & `tmp/adafruit-circuitpython-simpleio-3.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-simpleio-3.0.8.tar", last modified: Fri Aug 26 02:49:39 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-simpleio-3.0.9.tar", last modified: Tue Nov 15 17:45:42 2022, max compression
```

## Comparing `adafruit-circuitpython-simpleio-3.0.8.tar` & `adafruit-circuitpython-simpleio-3.0.9.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.421530 adafruit-circuitpython-simpleio-3.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.417530 adafruit-circuitpython-simpleio-3.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.417530 adafruit-circuitpython-simpleio-3.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.417530 adafruit-circuitpython-simpleio-3.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.417530 adafruit-circuitpython-simpleio-3.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-08-26 02:49:39.421530 adafruit-circuitpython-simpleio-3.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.421530 adafruit-circuitpython-simpleio-3.0.8/adafruit_circuitpython_simpleio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-08-26 02:49:39.000000 adafruit-circuitpython-simpleio-3.0.8/adafruit_circuitpython_simpleio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-08-26 02:49:39.000000 adafruit-circuitpython-simpleio-3.0.8/adafruit_circuitpython_simpleio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:49:39.000000 adafruit-circuitpython-simpleio-3.0.8/adafruit_circuitpython_simpleio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:49:39.000000 adafruit-circuitpython-simpleio-3.0.8/adafruit_circuitpython_simpleio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-08-26 02:49:39.000000 adafruit-circuitpython-simpleio-3.0.8/adafruit_circuitpython_simpleio.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.421530 adafruit-circuitpython-simpleio-3.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.421530 adafruit-circuitpython-simpleio-3.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      118 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      458 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      973 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:49:39.421530 adafruit-circuitpython-simpleio-3.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-08-26 02:49:31.000000 adafruit-circuitpython-simpleio-3.0.8/examples/simpleio_map_range_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-08-26 02:49:31.000000 adafruit-circuitpython-simpleio-3.0.8/examples/simpleio_shift_in_out_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)      371 2022-08-26 02:49:31.000000 adafruit-circuitpython-simpleio-3.0.8/examples/simpleio_tone_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-08-26 02:49:31.000000 adafruit-circuitpython-simpleio-3.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:49:24.000000 adafruit-circuitpython-simpleio-3.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:49:39.421530 adafruit-circuitpython-simpleio-3.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     7929 2022-08-26 02:49:31.000000 adafruit-circuitpython-simpleio-3.0.8/simpleio.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.412498 adafruit-circuitpython-simpleio-3.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.408498 adafruit-circuitpython-simpleio-3.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.408498 adafruit-circuitpython-simpleio-3.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.408498 adafruit-circuitpython-simpleio-3.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      423 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      475 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    13069 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.408498 adafruit-circuitpython-simpleio-3.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-11-15 17:45:42.412498 adafruit-circuitpython-simpleio-3.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.408498 adafruit-circuitpython-simpleio-3.0.9/adafruit_circuitpython_simpleio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3418 2022-11-15 17:45:42.000000 adafruit-circuitpython-simpleio-3.0.9/adafruit_circuitpython_simpleio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-11-15 17:45:42.000000 adafruit-circuitpython-simpleio-3.0.9/adafruit_circuitpython_simpleio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-15 17:45:42.000000 adafruit-circuitpython-simpleio-3.0.9/adafruit_circuitpython_simpleio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-15 17:45:42.000000 adafruit-circuitpython-simpleio-3.0.9/adafruit_circuitpython_simpleio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-15 17:45:42.000000 adafruit-circuitpython-simpleio-3.0.9/adafruit_circuitpython_simpleio.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.412498 adafruit-circuitpython-simpleio-3.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.412498 adafruit-circuitpython-simpleio-3.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      118 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5392 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-15 17:45:42.412498 adafruit-circuitpython-simpleio-3.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      741 2022-11-15 17:45:34.000000 adafruit-circuitpython-simpleio-3.0.9/examples/simpleio_map_range_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1001 2022-11-15 17:45:34.000000 adafruit-circuitpython-simpleio-3.0.9/examples/simpleio_shift_in_out_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      371 2022-11-15 17:45:34.000000 adafruit-circuitpython-simpleio-3.0.9/examples/simpleio_tone_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1240 2022-11-15 17:45:34.000000 adafruit-circuitpython-simpleio-3.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-11-15 17:45:26.000000 adafruit-circuitpython-simpleio-3.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-15 17:45:42.412498 adafruit-circuitpython-simpleio-3.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     7872 2022-11-15 17:45:34.000000 adafruit-circuitpython-simpleio-3.0.9/simpleio.py
```

### Comparing `adafruit-circuitpython-simpleio-3.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-simpleio-3.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/.gitignore` & `adafruit-circuitpython-simpleio-3.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-simpleio-3.0.9/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   - repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.2.0
     hooks:
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
   - repo: https://github.com/pycqa/pylint
-    rev: v2.11.1
+    rev: v2.15.5
     hooks:
       - id: pylint
         name: pylint (library code)
         types: [python]
         args:
           - --disable=consider-using-f-string
         exclude: "^(docs/|examples/|tests/|setup.py$)"
```

### Comparing `adafruit-circuitpython-simpleio-3.0.8/.pylintrc` & `adafruit-circuitpython-simpleio-3.0.9/.pylintrc`

 * *Files 22% similar despite different names*

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
```

### Comparing `adafruit-circuitpython-simpleio-3.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-simpleio-3.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/LICENSE` & `adafruit-circuitpython-simpleio-3.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-simpleio-3.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-simpleio-3.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-simpleio-3.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/PKG-INFO` & `adafruit-circuitpython-simpleio-3.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-simpleio
-Version: 3.0.8
+Version: 3.0.9
 Summary: CircuitPython helper library to simplify hardware interactions.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SimpleIO
 Keywords: adafruit,simpleio,servo,map,range,bitwrite,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-simpleio-3.0.8/README.rst` & `adafruit-circuitpython-simpleio-3.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/adafruit_circuitpython_simpleio.egg-info/PKG-INFO` & `adafruit-circuitpython-simpleio-3.0.9/adafruit_circuitpython_simpleio.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-simpleio
-Version: 3.0.8
+Version: 3.0.9
 Summary: CircuitPython helper library to simplify hardware interactions.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SimpleIO
 Keywords: adafruit,simpleio,servo,map,range,bitwrite,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-simpleio-3.0.8/adafruit_circuitpython_simpleio.egg-info/SOURCES.txt` & `adafruit-circuitpython-simpleio-3.0.9/adafruit_circuitpython_simpleio.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,16 @@
 optional_requirements.txt
 pyproject.toml
 requirements.txt
 simpleio.py
 .github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
 .github/workflows/build.yml
 .github/workflows/failure-help-text.yml
-.github/workflows/release.yml
+.github/workflows/release_gh.yml
+.github/workflows/release_pypi.yml
 LICENSES/CC-BY-4.0.txt
 LICENSES/MIT.txt
 LICENSES/Unlicense.txt
 adafruit_circuitpython_simpleio.egg-info/PKG-INFO
 adafruit_circuitpython_simpleio.egg-info/SOURCES.txt
 adafruit_circuitpython_simpleio.egg-info/dependency_links.txt
 adafruit_circuitpython_simpleio.egg-info/requires.txt
```

### Comparing `adafruit-circuitpython-simpleio-3.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-simpleio-3.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/docs/conf.py` & `adafruit-circuitpython-simpleio-3.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/docs/index.rst` & `adafruit-circuitpython-simpleio-3.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/examples/simpleio_map_range_simpletest.py` & `adafruit-circuitpython-simpleio-3.0.9/examples/simpleio_map_range_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/examples/simpleio_shift_in_out_demo.py` & `adafruit-circuitpython-simpleio-3.0.9/examples/simpleio_shift_in_out_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-simpleio-3.0.8/pyproject.toml` & `adafruit-circuitpython-simpleio-3.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-simpleio"
 description = "CircuitPython helper library to simplify hardware interactions."
-version = "3.0.8"
+version = "3.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SimpleIO"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-simpleio-3.0.8/simpleio.py` & `adafruit-circuitpython-simpleio-3.0.9/simpleio.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     try:
         from audioio import AudioOut
     except ImportError:
         from audiopwmio import PWMAudioOut as AudioOut
 except ImportError:
     pass  # not always supported by every board!
 
-__version__ = "3.0.8"
+__version__ = "3.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SimpleIO.git"
 
 
 def tone(pin, frequency, duration=1, length=100):
     """
     Generates a square wave of the specified frequency on a pin
 
@@ -167,20 +167,17 @@
             simpleio.shift_out(data_pin, clock, valueSend)
             latchpin.value = True
             time.sleep(1.0)
     """
     if bitcount < 0 or bitcount > 32:
         raise ValueError("bitcount must be in range 0..32 inclusive")
 
-    if msb_first:
-        bitsequence = lambda: range(bitcount - 1, -1, -1)
-    else:
-        bitsequence = lambda: range(0, bitcount)
+    bitsequence = range(bitcount - 1, -1, -1) if msb_first else range(bitcount)
 
-    for i in bitsequence():
+    for i in bitsequence:
         tmpval = bool(value & (1 << i))
         data_pin.value = tmpval
         # toggle clock pin True/False
         clock.value = True
         clock.value = False
```

