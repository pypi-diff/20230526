# Comparing `tmp/adafruit-circuitpython-apds9960-3.1.7.tar.gz` & `tmp/adafruit-circuitpython-apds9960-3.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-apds9960-3.1.7.tar", last modified: Tue May 16 17:44:47 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-apds9960-3.1.8.tar", last modified: Fri May 26 16:16:28 2023, max compression
```

## Comparing `adafruit-circuitpython-apds9960-3.1.7.tar` & `adafruit-circuitpython-apds9960-3.1.8.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.400189 adafruit-circuitpython-apds9960-3.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.392189 adafruit-circuitpython-apds9960-3.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-05-16 17:44:47.400189 adafruit-circuitpython-apds9960-3.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35503 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/apds9960.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/colorutility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 17:44:47.000000 adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.396189 adafruit-circuitpython-apds9960-3.1.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:44:47.400189 adafruit-circuitpython-apds9960-3.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_color_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_gesture_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_proximity_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 17:44:38.000000 adafruit-circuitpython-apds9960-3.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:44:25.000000 adafruit-circuitpython-apds9960-3.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:44:47.400189 adafruit-circuitpython-apds9960-3.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.546946 adafruit-circuitpython-apds9960-3.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.538946 adafruit-circuitpython-apds9960-3.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.542946 adafruit-circuitpython-apds9960-3.1.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.542946 adafruit-circuitpython-apds9960-3.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.542946 adafruit-circuitpython-apds9960-3.1.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-05-26 16:16:28.546946 adafruit-circuitpython-apds9960-3.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9125 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.542946 adafruit-circuitpython-apds9960-3.1.8/adafruit_apds9960/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-26 16:16:20.000000 adafruit-circuitpython-apds9960-3.1.8/adafruit_apds9960/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35503 2023-05-26 16:16:20.000000 adafruit-circuitpython-apds9960-3.1.8/adafruit_apds9960/apds9960.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-26 16:16:20.000000 adafruit-circuitpython-apds9960-3.1.8/adafruit_apds9960/colorutility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.542946 adafruit-circuitpython-apds9960-3.1.8/adafruit_circuitpython_apds9960.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9910 2023-05-26 16:16:28.000000 adafruit-circuitpython-apds9960-3.1.8/adafruit_circuitpython_apds9960.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 16:16:28.000000 adafruit-circuitpython-apds9960-3.1.8/adafruit_circuitpython_apds9960.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:16:28.000000 adafruit-circuitpython-apds9960-3.1.8/adafruit_circuitpython_apds9960.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:16:28.000000 adafruit-circuitpython-apds9960-3.1.8/adafruit_circuitpython_apds9960.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:16:28.000000 adafruit-circuitpython-apds9960-3.1.8/adafruit_circuitpython_apds9960.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.546946 adafruit-circuitpython-apds9960-3.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.546946 adafruit-circuitpython-apds9960-3.1.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:28.546946 adafruit-circuitpython-apds9960-3.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 16:16:20.000000 adafruit-circuitpython-apds9960-3.1.8/examples/apds9960_color_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-26 16:16:20.000000 adafruit-circuitpython-apds9960-3.1.8/examples/apds9960_gesture_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      928 2023-05-26 16:16:20.000000 adafruit-circuitpython-apds9960-3.1.8/examples/apds9960_proximity_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-26 16:16:20.000000 adafruit-circuitpython-apds9960-3.1.8/examples/apds9960_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-26 16:16:20.000000 adafruit-circuitpython-apds9960-3.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:16:08.000000 adafruit-circuitpython-apds9960-3.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:16:28.546946 adafruit-circuitpython-apds9960-3.1.8/setup.cfg
```

### Comparing `adafruit-circuitpython-apds9960-3.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-apds9960-3.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/.gitignore` & `adafruit-circuitpython-apds9960-3.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/.pre-commit-config.yaml` & `adafruit-circuitpython-apds9960-3.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/.pylintrc` & `adafruit-circuitpython-apds9960-3.1.8/.pylintrc`

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

### Comparing `adafruit-circuitpython-apds9960-3.1.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-apds9960-3.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/LICENSE` & `adafruit-circuitpython-apds9960-3.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-apds9960-3.1.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/LICENSES/MIT.txt` & `adafruit-circuitpython-apds9960-3.1.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-apds9960-3.1.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/PKG-INFO` & `adafruit-circuitpython-apds9960-3.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-apds9960
-Version: 3.1.7
+Version: 3.1.8
 Summary: CircuitPython driver for APSD9960 Gesture breakout board
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_APDS9960
 Keywords: adafruit,apsd9960,gesture,color,proximity,light,sensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-apds9960-3.1.7/README.rst` & `adafruit-circuitpython-apds9960-3.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/apds9960.py` & `adafruit-circuitpython-apds9960-3.1.8/adafruit_apds9960/apds9960.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 try:
     # Only used for typing
     from typing import Tuple
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "3.1.7"
+__version__ = "3.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_APDS9960.git"
 
 # Only one address is possible for the APDS9960, no alternates are available
 _APDS9960_I2C_ADDRESS = const(0x39)
 _DEVICE_ID = const(0xAB)
 
 # APDS9960_RAM        = const(0x00)
```

### Comparing `adafruit-circuitpython-apds9960-3.1.7/adafruit_apds9960/colorutility.py` & `adafruit-circuitpython-apds9960-3.1.8/adafruit_apds9960/colorutility.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ====================================================
 
 Helper functions for color calculations
 
 * Author(s): Michael McWethy
 """
 
-__version__ = "3.1.7"
+__version__ = "3.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_APDS9960.git"
 
 
 def calculate_color_temperature(r: int, g: int, b: int) -> float:
     """Converts the raw R/G/B values to color temperature in degrees Kelvin"""
 
     #  1. Map RGB values to their XYZ counterparts.
```

### Comparing `adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/PKG-INFO` & `adafruit-circuitpython-apds9960-3.1.8/adafruit_circuitpython_apds9960.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-apds9960
-Version: 3.1.7
+Version: 3.1.8
 Summary: CircuitPython driver for APSD9960 Gesture breakout board
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_APDS9960
 Keywords: adafruit,apsd9960,gesture,color,proximity,light,sensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-apds9960-3.1.7/adafruit_circuitpython_apds9960.egg-info/SOURCES.txt` & `adafruit-circuitpython-apds9960-3.1.8/adafruit_circuitpython_apds9960.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/docs/_static/favicon.ico` & `adafruit-circuitpython-apds9960-3.1.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/docs/conf.py` & `adafruit-circuitpython-apds9960-3.1.8/docs/conf.py`

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
     "sphinx.ext.viewcode",
 ]
 
 # Mock out micropython ourselves so that we can make const a lambda.
 import imp
```

### Comparing `adafruit-circuitpython-apds9960-3.1.7/docs/examples.rst` & `adafruit-circuitpython-apds9960-3.1.8/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/docs/index.rst` & `adafruit-circuitpython-apds9960-3.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_color_simpletest.py` & `adafruit-circuitpython-apds9960-3.1.8/examples/apds9960_color_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_gesture_simpletest.py` & `adafruit-circuitpython-apds9960-3.1.8/examples/apds9960_gesture_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/examples/apds9960_proximity_simpletest.py` & `adafruit-circuitpython-apds9960-3.1.8/examples/apds9960_proximity_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-apds9960-3.1.7/pyproject.toml` & `adafruit-circuitpython-apds9960-3.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-apds9960"
 description = "CircuitPython driver for APSD9960 Gesture breakout board"
-version = "3.1.7"
+version = "3.1.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_APDS9960"}
 keywords = [
     "adafruit",
```

