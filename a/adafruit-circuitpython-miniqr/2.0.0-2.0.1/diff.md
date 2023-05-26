# Comparing `tmp/adafruit-circuitpython-miniqr-2.0.0.tar.gz` & `tmp/adafruit-circuitpython-miniqr-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-miniqr-2.0.0.tar", last modified: Thu May 11 14:23:51 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-miniqr-2.0.1.tar", last modified: Fri May 26 16:15:52 2023, max compression
```

## Comparing `adafruit-circuitpython-miniqr-2.0.0.tar` & `adafruit-circuitpython-miniqr-2.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.520213 adafruit-circuitpython-miniqr-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.516213 adafruit-circuitpython-miniqr-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.516213 adafruit-circuitpython-miniqr-2.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.516213 adafruit-circuitpython-miniqr-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.516213 adafruit-circuitpython-miniqr-2.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-11 14:23:51.520213 adafruit-circuitpython-miniqr-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.520213 adafruit-circuitpython-miniqr-2.0.0/adafruit_circuitpython_miniqr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-11 14:23:51.000000 adafruit-circuitpython-miniqr-2.0.0/adafruit_circuitpython_miniqr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-11 14:23:51.000000 adafruit-circuitpython-miniqr-2.0.0/adafruit_circuitpython_miniqr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:23:51.000000 adafruit-circuitpython-miniqr-2.0.0/adafruit_circuitpython_miniqr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-11 14:23:51.000000 adafruit-circuitpython-miniqr-2.0.0/adafruit_circuitpython_miniqr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 14:23:51.000000 adafruit-circuitpython-miniqr-2.0.0/adafruit_circuitpython_miniqr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-05-11 14:23:42.000000 adafruit-circuitpython-miniqr-2.0.0/adafruit_miniqr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.520213 adafruit-circuitpython-miniqr-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.520213 adafruit-circuitpython-miniqr-2.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5631 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:23:51.520213 adafruit-circuitpython-miniqr-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-11 14:23:42.000000 adafruit-circuitpython-miniqr-2.0.0/examples/miniqr_displaytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-11 14:23:42.000000 adafruit-circuitpython-miniqr-2.0.0/examples/miniqr_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-11 14:23:42.000000 adafruit-circuitpython-miniqr-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:23:29.000000 adafruit-circuitpython-miniqr-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:23:51.520213 adafruit-circuitpython-miniqr-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.927005 adafruit-circuitpython-miniqr-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.923005 adafruit-circuitpython-miniqr-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.923005 adafruit-circuitpython-miniqr-2.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.923005 adafruit-circuitpython-miniqr-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.927005 adafruit-circuitpython-miniqr-2.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-26 16:15:52.927005 adafruit-circuitpython-miniqr-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.927005 adafruit-circuitpython-miniqr-2.0.1/adafruit_circuitpython_miniqr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3400 2023-05-26 16:15:52.000000 adafruit-circuitpython-miniqr-2.0.1/adafruit_circuitpython_miniqr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-26 16:15:52.000000 adafruit-circuitpython-miniqr-2.0.1/adafruit_circuitpython_miniqr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:15:52.000000 adafruit-circuitpython-miniqr-2.0.1/adafruit_circuitpython_miniqr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 16:15:52.000000 adafruit-circuitpython-miniqr-2.0.1/adafruit_circuitpython_miniqr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:15:52.000000 adafruit-circuitpython-miniqr-2.0.1/adafruit_circuitpython_miniqr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    20120 2023-05-26 16:15:45.000000 adafruit-circuitpython-miniqr-2.0.1/adafruit_miniqr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.927005 adafruit-circuitpython-miniqr-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.927005 adafruit-circuitpython-miniqr-2.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:52.927005 adafruit-circuitpython-miniqr-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-26 16:15:45.000000 adafruit-circuitpython-miniqr-2.0.1/examples/miniqr_displaytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 16:15:45.000000 adafruit-circuitpython-miniqr-2.0.1/examples/miniqr_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-26 16:15:45.000000 adafruit-circuitpython-miniqr-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:15:34.000000 adafruit-circuitpython-miniqr-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:15:52.927005 adafruit-circuitpython-miniqr-2.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-miniqr-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-miniqr-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/.gitignore` & `adafruit-circuitpython-miniqr-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-miniqr-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/.pylintrc` & `adafruit-circuitpython-miniqr-2.0.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-miniqr-2.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-miniqr-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/LICENSE` & `adafruit-circuitpython-miniqr-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-miniqr-2.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-miniqr-2.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-miniqr-2.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/PKG-INFO` & `adafruit-circuitpython-miniqr-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-miniqr
-Version: 2.0.0
+Version: 2.0.1
 Summary: A non-hardware dependant miniature QR generator library. All native Python!
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_miniQR
 Keywords: adafruit,software,miniqr,qr,generator,python,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-miniqr-2.0.0/README.rst` & `adafruit-circuitpython-miniqr-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/adafruit_circuitpython_miniqr.egg-info/PKG-INFO` & `adafruit-circuitpython-miniqr-2.0.1/adafruit_circuitpython_miniqr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-miniqr
-Version: 2.0.0
+Version: 2.0.1
 Summary: A non-hardware dependant miniature QR generator library. All native Python!
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_miniQR
 Keywords: adafruit,software,miniqr,qr,generator,python,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-miniqr-2.0.0/adafruit_circuitpython_miniqr.egg-info/SOURCES.txt` & `adafruit-circuitpython-miniqr-2.0.1/adafruit_circuitpython_miniqr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/adafruit_miniqr.py` & `adafruit-circuitpython-miniqr-2.0.1/adafruit_miniqr.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 * Python 3
 
 """
 
 # imports
 import math
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_miniQR.git"
 
 # Consts!
 M = 0
 L = 1
 H = 2
 Q = 3
```

### Comparing `adafruit-circuitpython-miniqr-2.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-miniqr-2.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/docs/conf.py` & `adafruit-circuitpython-miniqr-2.0.1/docs/conf.py`

 * *Files 4% similar despite different names*

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

### Comparing `adafruit-circuitpython-miniqr-2.0.0/docs/index.rst` & `adafruit-circuitpython-miniqr-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/examples/miniqr_displaytest.py` & `adafruit-circuitpython-miniqr-2.0.1/examples/miniqr_displaytest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/examples/miniqr_simpletest.py` & `adafruit-circuitpython-miniqr-2.0.1/examples/miniqr_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-miniqr-2.0.0/pyproject.toml` & `adafruit-circuitpython-miniqr-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-miniqr"
 description = "A non-hardware dependant miniature QR generator library. All native Python!"
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_miniQR"}
 keywords = [
     "adafruit",
```

