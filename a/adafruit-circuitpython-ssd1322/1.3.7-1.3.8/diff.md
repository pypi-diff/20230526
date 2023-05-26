# Comparing `tmp/adafruit-circuitpython-ssd1322-1.3.7.tar.gz` & `tmp/adafruit-circuitpython-ssd1322-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1322-1.3.7.tar", last modified: Thu May 18 15:19:26 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1322-1.3.8.tar", last modified: Fri May 26 16:12:50 2023, max compression
```

## Comparing `adafruit-circuitpython-ssd1322-1.3.7.tar` & `adafruit-circuitpython-ssd1322-1.3.8.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.704821 adafruit-circuitpython-ssd1322-1.3.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/adafruit_circuitpython_ssd1322.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-18 15:19:26.000000 adafruit-circuitpython-ssd1322-1.3.7/adafruit_circuitpython_ssd1322.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-18 15:19:26.000000 adafruit-circuitpython-ssd1322-1.3.7/adafruit_circuitpython_ssd1322.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:19:26.000000 adafruit-circuitpython-ssd1322-1.3.7/adafruit_circuitpython_ssd1322.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:19:26.000000 adafruit-circuitpython-ssd1322-1.3.7/adafruit_circuitpython_ssd1322.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:19:26.000000 adafruit-circuitpython-ssd1322-1.3.7/adafruit_circuitpython_ssd1322.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-18 15:19:19.000000 adafruit-circuitpython-ssd1322-1.3.7/adafruit_ssd1322.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-18 15:19:19.000000 adafruit-circuitpython-ssd1322-1.3.7/examples/ssd1322_gamma.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-18 15:19:19.000000 adafruit-circuitpython-ssd1322-1.3.7/examples/ssd1322_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-18 15:19:19.000000 adafruit-circuitpython-ssd1322-1.3.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:19:08.000000 adafruit-circuitpython-ssd1322-1.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:19:26.708821 adafruit-circuitpython-ssd1322-1.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.089813 adafruit-circuitpython-ssd1322-1.3.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.081813 adafruit-circuitpython-ssd1322-1.3.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.085813 adafruit-circuitpython-ssd1322-1.3.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.085813 adafruit-circuitpython-ssd1322-1.3.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.085813 adafruit-circuitpython-ssd1322-1.3.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-26 16:12:50.089813 adafruit-circuitpython-ssd1322-1.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.085813 adafruit-circuitpython-ssd1322-1.3.8/adafruit_circuitpython_ssd1322.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3829 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1322-1.3.8/adafruit_circuitpython_ssd1322.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1322-1.3.8/adafruit_circuitpython_ssd1322.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1322-1.3.8/adafruit_circuitpython_ssd1322.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1322-1.3.8/adafruit_circuitpython_ssd1322.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1322-1.3.8/adafruit_circuitpython_ssd1322.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4852 2023-05-26 16:12:42.000000 adafruit-circuitpython-ssd1322-1.3.8/adafruit_ssd1322.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.085813 adafruit-circuitpython-ssd1322-1.3.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.085813 adafruit-circuitpython-ssd1322-1.3.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:50.089813 adafruit-circuitpython-ssd1322-1.3.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 16:12:42.000000 adafruit-circuitpython-ssd1322-1.3.8/examples/ssd1322_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-26 16:12:42.000000 adafruit-circuitpython-ssd1322-1.3.8/examples/ssd1322_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-26 16:12:42.000000 adafruit-circuitpython-ssd1322-1.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:12:32.000000 adafruit-circuitpython-ssd1322-1.3.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:12:50.089813 adafruit-circuitpython-ssd1322-1.3.8/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1322-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/.gitignore` & `adafruit-circuitpython-ssd1322-1.3.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1322-1.3.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/.pylintrc` & `adafruit-circuitpython-ssd1322-1.3.8/.pylintrc`

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

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1322-1.3.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/LICENSE` & `adafruit-circuitpython-ssd1322-1.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1322-1.3.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1322-1.3.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1322-1.3.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/PKG-INFO` & `adafruit-circuitpython-ssd1322-1.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1322
-Version: 1.3.7
+Version: 1.3.8
 Summary: DisplayIO driver for grayscale OLEDs drive by SSD1322
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1322
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1322,oled,grayscale,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/README.rst` & `adafruit-circuitpython-ssd1322-1.3.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/adafruit_circuitpython_ssd1322.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1322-1.3.8/adafruit_circuitpython_ssd1322.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1322
-Version: 1.3.7
+Version: 1.3.8
 Summary: DisplayIO driver for grayscale OLEDs drive by SSD1322
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1322
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1322,oled,grayscale,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/adafruit_circuitpython_ssd1322.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1322-1.3.8/adafruit_circuitpython_ssd1322.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/adafruit_ssd1322.py` & `adafruit-circuitpython-ssd1322-1.3.8/adafruit_ssd1322.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython 5+ firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.3.7"
+__version__ = "1.3.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1322.git"
 
 _INIT_SEQUENCE = (
     b"\xfd\x01\x12"  # Set_Command_Lock(0x12);// Unlock Basic Commands (0x12/0x16)
     b"\xae\x00"  # Set_Display_On_Off(0x00);// Display Off (0x00/0x01)
     b"\xb3\x01\x91"  # Set_Display_Clock(0x91);// Set Clock as 80 Frames/Sec
     b"\xca\x01\x3f"  # Set_Multiplex_Ratio(0x3F);// 1/64 Duty (0x0F~0x3F)
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1322-1.3.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/docs/conf.py` & `adafruit-circuitpython-ssd1322-1.3.8/docs/conf.py`

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
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/docs/index.rst` & `adafruit-circuitpython-ssd1322-1.3.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/examples/ssd1322_gamma.py` & `adafruit-circuitpython-ssd1322-1.3.8/examples/ssd1322_gamma.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/examples/ssd1322_simpletest.py` & `adafruit-circuitpython-ssd1322-1.3.8/examples/ssd1322_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1322-1.3.7/pyproject.toml` & `adafruit-circuitpython-ssd1322-1.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ssd1322"
 description = "DisplayIO driver for grayscale OLEDs drive by SSD1322"
-version = "1.3.7"
+version = "1.3.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1322"}
 keywords = [
     "adafruit",
```

