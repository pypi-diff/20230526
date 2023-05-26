# Comparing `tmp/adafruit-circuitpython-lifx-2.0.0.tar.gz` & `tmp/adafruit-circuitpython-lifx-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lifx-2.0.0.tar", last modified: Thu May 11 18:25:30 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-lifx-2.0.1.tar", last modified: Fri May 26 16:22:59 2023, max compression
```

## Comparing `adafruit-circuitpython-lifx-2.0.0.tar` & `adafruit-circuitpython-lifx-2.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.885089 adafruit-circuitpython-lifx-2.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.889089 adafruit-circuitpython-lifx-2.0.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.889089 adafruit-circuitpython-lifx-2.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.889089 adafruit-circuitpython-lifx-2.0.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.889089 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-11 18:25:30.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-11 18:25:23.000000 adafruit-circuitpython-lifx-2.0.0/adafruit_lifx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5345 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-11 18:25:23.000000 adafruit-circuitpython-lifx-2.0.0/examples/lifx_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-11 18:25:23.000000 adafruit-circuitpython-lifx-2.0.0/examples/lifx_simpletest_esp32s2.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-11 18:25:23.000000 adafruit-circuitpython-lifx-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-11 18:25:11.000000 adafruit-circuitpython-lifx-2.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 18:25:30.893089 adafruit-circuitpython-lifx-2.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.979853 adafruit-circuitpython-lifx-2.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.971853 adafruit-circuitpython-lifx-2.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.975853 adafruit-circuitpython-lifx-2.0.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.975853 adafruit-circuitpython-lifx-2.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.975853 adafruit-circuitpython-lifx-2.0.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-26 16:22:59.979853 adafruit-circuitpython-lifx-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3673 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.975853 adafruit-circuitpython-lifx-2.0.1/adafruit_circuitpython_lifx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-05-26 16:22:59.000000 adafruit-circuitpython-lifx-2.0.1/adafruit_circuitpython_lifx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-26 16:22:59.000000 adafruit-circuitpython-lifx-2.0.1/adafruit_circuitpython_lifx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:22:59.000000 adafruit-circuitpython-lifx-2.0.1/adafruit_circuitpython_lifx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 16:22:59.000000 adafruit-circuitpython-lifx-2.0.1/adafruit_circuitpython_lifx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 16:22:59.000000 adafruit-circuitpython-lifx-2.0.1/adafruit_circuitpython_lifx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6265 2023-05-26 16:22:52.000000 adafruit-circuitpython-lifx-2.0.1/adafruit_lifx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.975853 adafruit-circuitpython-lifx-2.0.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.975853 adafruit-circuitpython-lifx-2.0.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:59.979853 adafruit-circuitpython-lifx-2.0.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-26 16:22:52.000000 adafruit-circuitpython-lifx-2.0.1/examples/lifx_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-26 16:22:52.000000 adafruit-circuitpython-lifx-2.0.1/examples/lifx_simpletest_esp32s2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-26 16:22:52.000000 adafruit-circuitpython-lifx-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 16:22:43.000000 adafruit-circuitpython-lifx-2.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:22:59.979853 adafruit-circuitpython-lifx-2.0.1/setup.cfg
```

### Comparing `adafruit-circuitpython-lifx-2.0.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-lifx-2.0.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/.gitignore` & `adafruit-circuitpython-lifx-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/.pre-commit-config.yaml` & `adafruit-circuitpython-lifx-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/.pylintrc` & `adafruit-circuitpython-lifx-2.0.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-lifx-2.0.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lifx-2.0.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/LICENSE` & `adafruit-circuitpython-lifx-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lifx-2.0.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/LICENSES/MIT.txt` & `adafruit-circuitpython-lifx-2.0.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lifx-2.0.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/PKG-INFO` & `adafruit-circuitpython-lifx-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lifx
-Version: 2.0.0
+Version: 2.0.1
 Summary: LIFX Smart Lighting API Helper
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_lifx
 Keywords: adafruit,blinka,circuitpython,micropython,lifx
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lifx-2.0.0/README.rst` & `adafruit-circuitpython-lifx-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/PKG-INFO` & `adafruit-circuitpython-lifx-2.0.1/adafruit_circuitpython_lifx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lifx
-Version: 2.0.0
+Version: 2.0.1
 Summary: LIFX Smart Lighting API Helper
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_lifx
 Keywords: adafruit,blinka,circuitpython,micropython,lifx
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lifx-2.0.0/adafruit_circuitpython_lifx.egg-info/SOURCES.txt` & `adafruit-circuitpython-lifx-2.0.1/adafruit_circuitpython_lifx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/adafruit_lifx.py` & `adafruit-circuitpython-lifx-2.0.1/adafruit_lifx.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 or:
 
 * Adafruit_requests library:
    https://github.com/adafruit/Adafruit_CircuitPython_Requests
 
 """
 
-__version__ = "2.0.0"
+__version__ = "2.0.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_lifx.git"
 
 LIFX_URL = "https://api.lifx.com/v1/lights/"
 
 try:
     from typing import Dict, Any
     from circuitpython_typing.http import HTTPProtocol
```

### Comparing `adafruit-circuitpython-lifx-2.0.0/docs/_static/favicon.ico` & `adafruit-circuitpython-lifx-2.0.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/docs/conf.py` & `adafruit-circuitpython-lifx-2.0.1/docs/conf.py`

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
 
 
 intersphinx_mapping = {
```

### Comparing `adafruit-circuitpython-lifx-2.0.0/docs/index.rst` & `adafruit-circuitpython-lifx-2.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/examples/lifx_simpletest.py` & `adafruit-circuitpython-lifx-2.0.1/examples/lifx_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/examples/lifx_simpletest_esp32s2.py` & `adafruit-circuitpython-lifx-2.0.1/examples/lifx_simpletest_esp32s2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lifx-2.0.0/pyproject.toml` & `adafruit-circuitpython-lifx-2.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-lifx"
 description = "LIFX Smart Lighting API Helper"
-version = "2.0.0"
+version = "2.0.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_lifx"}
 keywords = [
     "adafruit",
```

