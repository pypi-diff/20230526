# Comparing `tmp/adafruit-circuitpython-acep7in-0.8.2.tar.gz` & `tmp/adafruit-circuitpython-acep7in-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-acep7in-0.8.2.tar", last modified: Thu May 18 15:27:51 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-acep7in-0.8.3.tar", last modified: Fri May 26 16:07:12 2023, max compression
```

## Comparing `adafruit-circuitpython-acep7in-0.8.2.tar` & `adafruit-circuitpython-acep7in-0.8.3.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.948572 adafruit-circuitpython-acep7in-0.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-18 15:27:44.000000 adafruit-circuitpython-acep7in-0.8.2/adafruit_acep7in.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/adafruit_circuitpython_acep7in.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-18 15:27:51.000000 adafruit-circuitpython-acep7in-0.8.2/adafruit_circuitpython_acep7in.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-18 15:27:51.000000 adafruit-circuitpython-acep7in-0.8.2/adafruit_circuitpython_acep7in.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:27:51.000000 adafruit-circuitpython-acep7in-0.8.2/adafruit_circuitpython_acep7in.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 15:27:51.000000 adafruit-circuitpython-acep7in-0.8.2/adafruit_circuitpython_acep7in.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:27:51.000000 adafruit-circuitpython-acep7in-0.8.2/adafruit_circuitpython_acep7in.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-18 15:27:44.000000 adafruit-circuitpython-acep7in-0.8.2/examples/acep7in_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)   921926 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/examples/display-ruler-720p.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/examples/display-ruler-720p.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-18 15:27:44.000000 adafruit-circuitpython-acep7in-0.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-18 15:27:35.000000 adafruit-circuitpython-acep7in-0.8.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:27:51.952572 adafruit-circuitpython-acep7in-0.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.462299 adafruit-circuitpython-acep7in-0.8.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.458299 adafruit-circuitpython-acep7in-0.8.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.458299 adafruit-circuitpython-acep7in-0.8.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.458299 adafruit-circuitpython-acep7in-0.8.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.458299 adafruit-circuitpython-acep7in-0.8.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-26 16:07:12.462299 adafruit-circuitpython-acep7in-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2595 2023-05-26 16:07:05.000000 adafruit-circuitpython-acep7in-0.8.3/adafruit_acep7in.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.462299 adafruit-circuitpython-acep7in-0.8.3/adafruit_circuitpython_acep7in.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-26 16:07:12.000000 adafruit-circuitpython-acep7in-0.8.3/adafruit_circuitpython_acep7in.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-26 16:07:12.000000 adafruit-circuitpython-acep7in-0.8.3/adafruit_circuitpython_acep7in.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:07:12.000000 adafruit-circuitpython-acep7in-0.8.3/adafruit_circuitpython_acep7in.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 16:07:12.000000 adafruit-circuitpython-acep7in-0.8.3/adafruit_circuitpython_acep7in.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:07:12.000000 adafruit-circuitpython-acep7in-0.8.3/adafruit_circuitpython_acep7in.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.462299 adafruit-circuitpython-acep7in-0.8.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.462299 adafruit-circuitpython-acep7in-0.8.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5968 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:12.462299 adafruit-circuitpython-acep7in-0.8.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-26 16:07:05.000000 adafruit-circuitpython-acep7in-0.8.3/examples/acep7in_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   921926 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/examples/display-ruler-720p.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/examples/display-ruler-720p.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-26 16:07:05.000000 adafruit-circuitpython-acep7in-0.8.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 16:06:52.000000 adafruit-circuitpython-acep7in-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:07:12.462299 adafruit-circuitpython-acep7in-0.8.3/setup.cfg
```

### Comparing `adafruit-circuitpython-acep7in-0.8.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-acep7in-0.8.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/.gitignore` & `adafruit-circuitpython-acep7in-0.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/.pre-commit-config.yaml` & `adafruit-circuitpython-acep7in-0.8.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/.pylintrc` & `adafruit-circuitpython-acep7in-0.8.3/.pylintrc`

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

### Comparing `adafruit-circuitpython-acep7in-0.8.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-acep7in-0.8.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/LICENSE` & `adafruit-circuitpython-acep7in-0.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-acep7in-0.8.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/LICENSES/MIT.txt` & `adafruit-circuitpython-acep7in-0.8.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-acep7in-0.8.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/PKG-INFO` & `adafruit-circuitpython-acep7in-0.8.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-acep7in
-Version: 0.8.2
+Version: 0.8.3
 Summary: Driver for 7.3" 7-color (aka ACeP) epaper display
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ACeP7in
 Keywords: adafruit,blinka,circuitpython,micropython,acep7in,epd,acep
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-acep7in-0.8.2/README.rst` & `adafruit-circuitpython-acep7in-0.8.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/adafruit_acep7in.py` & `adafruit-circuitpython-acep7in-0.8.3/adafruit_acep7in.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 
 """
 
 import displayio
 
-__version__ = "0.8.2"
+__version__ = "0.8.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ACeP7In.git"
 
 _START_SEQUENCE = (
     b"\xaa\x06\x49\x55\x20\x08\x09\x18"  # CMDH
     b"\x01\x06\x3F\x00\x32\x2A\x0E\x2A"  # power setting PWRR
     b"\x00\x02\x5f\x69"  # panel setting (PSR)
     b"\x03\x04\x00\x54\x00\x44"  # POFS
```

### Comparing `adafruit-circuitpython-acep7in-0.8.2/adafruit_circuitpython_acep7in.egg-info/PKG-INFO` & `adafruit-circuitpython-acep7in-0.8.3/adafruit_circuitpython_acep7in.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-acep7in
-Version: 0.8.2
+Version: 0.8.3
 Summary: Driver for 7.3" 7-color (aka ACeP) epaper display
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ACeP7in
 Keywords: adafruit,blinka,circuitpython,micropython,acep7in,epd,acep
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-acep7in-0.8.2/adafruit_circuitpython_acep7in.egg-info/SOURCES.txt` & `adafruit-circuitpython-acep7in-0.8.3/adafruit_circuitpython_acep7in.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/docs/_static/favicon.ico` & `adafruit-circuitpython-acep7in-0.8.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/docs/conf.py` & `adafruit-circuitpython-acep7in-0.8.3/docs/conf.py`

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

### Comparing `adafruit-circuitpython-acep7in-0.8.2/docs/index.rst` & `adafruit-circuitpython-acep7in-0.8.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/examples/acep7in_simpletest.py` & `adafruit-circuitpython-acep7in-0.8.3/examples/acep7in_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/examples/display-ruler-720p.bmp` & `adafruit-circuitpython-acep7in-0.8.3/examples/display-ruler-720p.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-acep7in-0.8.2/pyproject.toml` & `adafruit-circuitpython-acep7in-0.8.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-acep7in"
 description = "Driver for 7.3\" 7-color (aka ACeP) epaper display"
-version = "0.8.2"
+version = "0.8.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ACeP7in"}
 keywords = [
     "adafruit",
```

