# Comparing `tmp/adafruit-circuitpython-focaltouch-1.4.7.tar.gz` & `tmp/adafruit-circuitpython-focaltouch-1.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-focaltouch-1.4.7.tar", last modified: Tue May 16 17:54:04 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-focaltouch-1.4.8.tar", last modified: Fri May 26 16:16:51 2023, max compression
```

## Comparing `adafruit-circuitpython-focaltouch-1.4.7.tar` & `adafruit-circuitpython-focaltouch-1.4.8.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.085727 adafruit-circuitpython-focaltouch-1.4.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.081727 adafruit-circuitpython-focaltouch-1.4.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.081727 adafruit-circuitpython-focaltouch-1.4.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.081727 adafruit-circuitpython-focaltouch-1.4.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.085727 adafruit-circuitpython-focaltouch-1.4.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-16 17:54:04.085727 adafruit-circuitpython-focaltouch-1.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.085727 adafruit-circuitpython-focaltouch-1.4.7/adafruit_circuitpython_focaltouch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-16 17:54:04.000000 adafruit-circuitpython-focaltouch-1.4.7/adafruit_circuitpython_focaltouch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-16 17:54:04.000000 adafruit-circuitpython-focaltouch-1.4.7/adafruit_circuitpython_focaltouch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:54:04.000000 adafruit-circuitpython-focaltouch-1.4.7/adafruit_circuitpython_focaltouch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-16 17:54:04.000000 adafruit-circuitpython-focaltouch-1.4.7/adafruit_circuitpython_focaltouch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 17:54:04.000000 adafruit-circuitpython-focaltouch-1.4.7/adafruit_circuitpython_focaltouch.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     5629 2023-05-16 17:53:55.000000 adafruit-circuitpython-focaltouch-1.4.7/adafruit_focaltouch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.085727 adafruit-circuitpython-focaltouch-1.4.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.085727 adafruit-circuitpython-focaltouch-1.4.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:04.085727 adafruit-circuitpython-focaltouch-1.4.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-16 17:53:55.000000 adafruit-circuitpython-focaltouch-1.4.7/examples/focaltouch_paint_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-16 17:53:55.000000 adafruit-circuitpython-focaltouch-1.4.7/examples/focaltouch_print_touches.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-16 17:53:55.000000 adafruit-circuitpython-focaltouch-1.4.7/examples/focaltouch_print_touches_with_irq.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-16 17:53:55.000000 adafruit-circuitpython-focaltouch-1.4.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-16 17:53:44.000000 adafruit-circuitpython-focaltouch-1.4.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:54:04.085727 adafruit-circuitpython-focaltouch-1.4.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.331114 adafruit-circuitpython-focaltouch-1.4.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.331114 adafruit-circuitpython-focaltouch-1.4.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:16:51.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5629 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/adafruit_focaltouch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_paint_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_print_touches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_print_touches_with_irq.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 16:16:44.000000 adafruit-circuitpython-focaltouch-1.4.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:16:35.000000 adafruit-circuitpython-focaltouch-1.4.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:16:51.335114 adafruit-circuitpython-focaltouch-1.4.8/setup.cfg
```

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-focaltouch-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/.gitignore` & `adafruit-circuitpython-focaltouch-1.4.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/.pre-commit-config.yaml` & `adafruit-circuitpython-focaltouch-1.4.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/.pylintrc` & `adafruit-circuitpython-focaltouch-1.4.8/.pylintrc`

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

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-focaltouch-1.4.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/LICENSE` & `adafruit-circuitpython-focaltouch-1.4.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-focaltouch-1.4.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/LICENSES/MIT.txt` & `adafruit-circuitpython-focaltouch-1.4.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-focaltouch-1.4.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/PKG-INFO` & `adafruit-circuitpython-focaltouch-1.4.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-focaltouch
-Version: 1.4.7
+Version: 1.4.8
 Summary: CircuitPython Focaltouch library for capacitive touch displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Focaltouch
 Keywords: adafruit,focaltouch,capacitive,touch,screen,display,touchscreenhardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/README.rst` & `adafruit-circuitpython-focaltouch-1.4.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/adafruit_circuitpython_focaltouch.egg-info/PKG-INFO` & `adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-focaltouch
-Version: 1.4.7
+Version: 1.4.8
 Summary: CircuitPython Focaltouch library for capacitive touch displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Focaltouch
 Keywords: adafruit,focaltouch,capacitive,touch,screen,display,touchscreenhardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/adafruit_circuitpython_focaltouch.egg-info/SOURCES.txt` & `adafruit-circuitpython-focaltouch-1.4.8/adafruit_circuitpython_focaltouch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/adafruit_focaltouch.py` & `adafruit-circuitpython-focaltouch-1.4.8/adafruit_focaltouch.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
   https://github.com/adafruit/circuitpython/releases
 * Adafruit's Bus Device library (when using I2C/SPI):
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
 # imports
 
-__version__ = "1.4.7"
+__version__ = "1.4.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FocalTouch.git"
 
 import struct
 
 from adafruit_bus_device.i2c_device import I2CDevice
 
 from micropython import const
```

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/docs/_static/favicon.ico` & `adafruit-circuitpython-focaltouch-1.4.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/docs/conf.py` & `adafruit-circuitpython-focaltouch-1.4.8/docs/conf.py`

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

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/docs/index.rst` & `adafruit-circuitpython-focaltouch-1.4.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/examples/focaltouch_paint_simpletest.py` & `adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_paint_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/examples/focaltouch_print_touches.py` & `adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_print_touches.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/examples/focaltouch_print_touches_with_irq.py` & `adafruit-circuitpython-focaltouch-1.4.8/examples/focaltouch_print_touches_with_irq.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-focaltouch-1.4.7/pyproject.toml` & `adafruit-circuitpython-focaltouch-1.4.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-focaltouch"
 description = "CircuitPython Focaltouch library for capacitive touch displays."
-version = "1.4.7"
+version = "1.4.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Focaltouch"}
 keywords = [
     "adafruit",
```

