# Comparing `tmp/adafruit-circuitpython-bh1750-1.1.7.tar.gz` & `tmp/adafruit-circuitpython-bh1750-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-bh1750-1.1.7.tar", last modified: Tue May 16 17:46:33 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-bh1750-1.1.8.tar", last modified: Fri May 26 16:08:24 2023, max compression
```

## Comparing `adafruit-circuitpython-bh1750-1.1.7.tar` & `adafruit-circuitpython-bh1750-1.1.8.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.945158 adafruit-circuitpython-bh1750-1.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-05-16 17:46:26.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_bh1750.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 17:46:33.000000 adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-16 17:46:26.000000 adafruit-circuitpython-bh1750-1.1.7/examples/bh1750_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-16 17:46:26.000000 adafruit-circuitpython-bh1750-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:46:18.000000 adafruit-circuitpython-bh1750-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:46:33.949158 adafruit-circuitpython-bh1750-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.575101 adafruit-circuitpython-bh1750-1.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     7002 2023-05-26 16:08:17.000000 adafruit-circuitpython-bh1750-1.1.8/adafruit_bh1750.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/adafruit_circuitpython_bh1750.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-26 16:08:24.000000 adafruit-circuitpython-bh1750-1.1.8/adafruit_circuitpython_bh1750.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-26 16:08:24.000000 adafruit-circuitpython-bh1750-1.1.8/adafruit_circuitpython_bh1750.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:08:24.000000 adafruit-circuitpython-bh1750-1.1.8/adafruit_circuitpython_bh1750.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:08:24.000000 adafruit-circuitpython-bh1750-1.1.8/adafruit_circuitpython_bh1750.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:08:24.000000 adafruit-circuitpython-bh1750-1.1.8/adafruit_circuitpython_bh1750.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5910 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-26 16:08:17.000000 adafruit-circuitpython-bh1750-1.1.8/examples/bh1750_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 16:08:17.000000 adafruit-circuitpython-bh1750-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:08:08.000000 adafruit-circuitpython-bh1750-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:08:24.579101 adafruit-circuitpython-bh1750-1.1.8/setup.cfg
```

### Comparing `adafruit-circuitpython-bh1750-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-bh1750-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/.gitignore` & `adafruit-circuitpython-bh1750-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/.pre-commit-config.yaml` & `adafruit-circuitpython-bh1750-1.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/.pylintrc` & `adafruit-circuitpython-bh1750-1.1.8/.pylintrc`

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

### Comparing `adafruit-circuitpython-bh1750-1.1.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-bh1750-1.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/LICENSE` & `adafruit-circuitpython-bh1750-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-bh1750-1.1.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/LICENSES/MIT.txt` & `adafruit-circuitpython-bh1750-1.1.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-bh1750-1.1.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/PKG-INFO` & `adafruit-circuitpython-bh1750-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bh1750
-Version: 1.1.7
+Version: 1.1.8
 Summary: CircuitPython library for use with the Adafruit BH1750 breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BH1750
 Keywords: adafruit,blinka,circuitpython,micropython,bh1750
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bh1750-1.1.7/README.rst` & `adafruit-circuitpython-bh1750-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/adafruit_bh1750.py` & `adafruit-circuitpython-bh1750-1.1.8/adafruit_bh1750.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
   https://circuitpython.org/downloads
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
 # imports
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BH1750.git"
 
 from time import sleep
 from struct import unpack_from
 from micropython import const
 from adafruit_bus_device import i2c_device
```

### Comparing `adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/PKG-INFO` & `adafruit-circuitpython-bh1750-1.1.8/adafruit_circuitpython_bh1750.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-bh1750
-Version: 1.1.7
+Version: 1.1.8
 Summary: CircuitPython library for use with the Adafruit BH1750 breakout
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BH1750
 Keywords: adafruit,blinka,circuitpython,micropython,bh1750
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-bh1750-1.1.7/adafruit_circuitpython_bh1750.egg-info/SOURCES.txt` & `adafruit-circuitpython-bh1750-1.1.8/adafruit_circuitpython_bh1750.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/docs/_static/favicon.ico` & `adafruit-circuitpython-bh1750-1.1.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/docs/conf.py` & `adafruit-circuitpython-bh1750-1.1.8/docs/conf.py`

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

### Comparing `adafruit-circuitpython-bh1750-1.1.7/docs/index.rst` & `adafruit-circuitpython-bh1750-1.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-bh1750-1.1.7/pyproject.toml` & `adafruit-circuitpython-bh1750-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-bh1750"
 description = "CircuitPython library for use with the Adafruit BH1750 breakout"
-version = "1.1.7"
+version = "1.1.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BH1750"}
 keywords = [
     "adafruit",
```

