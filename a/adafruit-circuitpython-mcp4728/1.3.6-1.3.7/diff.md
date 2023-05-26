# Comparing `tmp/adafruit-circuitpython-mcp4728-1.3.6.tar.gz` & `tmp/adafruit-circuitpython-mcp4728-1.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mcp4728-1.3.6.tar", last modified: Thu May 18 15:13:42 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-mcp4728-1.3.7.tar", last modified: Fri May 26 16:11:12 2023, max compression
```

## Comparing `adafruit-circuitpython-mcp4728-1.3.6.tar` & `adafruit-circuitpython-mcp4728-1.3.7.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.622343 adafruit-circuitpython-mcp4728-1.3.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.618343 adafruit-circuitpython-mcp4728-1.3.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.618343 adafruit-circuitpython-mcp4728-1.3.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.618343 adafruit-circuitpython-mcp4728-1.3.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.618343 adafruit-circuitpython-mcp4728-1.3.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-18 15:13:42.622343 adafruit-circuitpython-mcp4728-1.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.618343 adafruit-circuitpython-mcp4728-1.3.6/adafruit_circuitpython_mcp4728.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-18 15:13:42.000000 adafruit-circuitpython-mcp4728-1.3.6/adafruit_circuitpython_mcp4728.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-18 15:13:42.000000 adafruit-circuitpython-mcp4728-1.3.6/adafruit_circuitpython_mcp4728.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:13:42.000000 adafruit-circuitpython-mcp4728-1.3.6/adafruit_circuitpython_mcp4728.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-18 15:13:42.000000 adafruit-circuitpython-mcp4728-1.3.6/adafruit_circuitpython_mcp4728.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:13:42.000000 adafruit-circuitpython-mcp4728-1.3.6/adafruit_circuitpython_mcp4728.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-05-18 15:13:35.000000 adafruit-circuitpython-mcp4728-1.3.6/adafruit_mcp4728.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.622343 adafruit-circuitpython-mcp4728-1.3.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.622343 adafruit-circuitpython-mcp4728-1.3.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:13:42.622343 adafruit-circuitpython-mcp4728-1.3.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-18 15:13:35.000000 adafruit-circuitpython-mcp4728-1.3.6/examples/mcp4728_generalcalltest.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-18 15:13:35.000000 adafruit-circuitpython-mcp4728-1.3.6/examples/mcp4728_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-18 15:13:35.000000 adafruit-circuitpython-mcp4728-1.3.6/examples/mcp4728_vref_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-18 15:13:35.000000 adafruit-circuitpython-mcp4728-1.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-18 15:13:26.000000 adafruit-circuitpython-mcp4728-1.3.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:13:42.622343 adafruit-circuitpython-mcp4728-1.3.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.809707 adafruit-circuitpython-mcp4728-1.3.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/adafruit_circuitpython_mcp4728.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-05-26 16:11:12.000000 adafruit-circuitpython-mcp4728-1.3.7/adafruit_circuitpython_mcp4728.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-26 16:11:12.000000 adafruit-circuitpython-mcp4728-1.3.7/adafruit_circuitpython_mcp4728.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:11:12.000000 adafruit-circuitpython-mcp4728-1.3.7/adafruit_circuitpython_mcp4728.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-26 16:11:12.000000 adafruit-circuitpython-mcp4728-1.3.7/adafruit_circuitpython_mcp4728.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:11:12.000000 adafruit-circuitpython-mcp4728-1.3.7/adafruit_circuitpython_mcp4728.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12138 2023-05-26 16:11:05.000000 adafruit-circuitpython-mcp4728-1.3.7/adafruit_mcp4728.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5901 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-26 16:11:05.000000 adafruit-circuitpython-mcp4728-1.3.7/examples/mcp4728_generalcalltest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-26 16:11:05.000000 adafruit-circuitpython-mcp4728-1.3.7/examples/mcp4728_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-05-26 16:11:05.000000 adafruit-circuitpython-mcp4728-1.3.7/examples/mcp4728_vref_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-26 16:11:05.000000 adafruit-circuitpython-mcp4728-1.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-26 16:10:56.000000 adafruit-circuitpython-mcp4728-1.3.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:11:12.813707 adafruit-circuitpython-mcp4728-1.3.7/setup.cfg
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mcp4728-1.3.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/.gitignore` & `adafruit-circuitpython-mcp4728-1.3.7/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/.pre-commit-config.yaml` & `adafruit-circuitpython-mcp4728-1.3.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/.pylintrc` & `adafruit-circuitpython-mcp4728-1.3.7/.pylintrc`

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

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mcp4728-1.3.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/LICENSE` & `adafruit-circuitpython-mcp4728-1.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mcp4728-1.3.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/LICENSES/MIT.txt` & `adafruit-circuitpython-mcp4728-1.3.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mcp4728-1.3.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/PKG-INFO` & `adafruit-circuitpython-mcp4728-1.3.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp4728
-Version: 1.3.6
+Version: 1.3.7
 Summary: Helper library for the MCP4728 I2C 12-bit Quad DAC
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP4728
 Keywords: adafruit,blinka,circuitpython,micropython,mcp4728,dac,12-bit,quad,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/README.rst` & `adafruit-circuitpython-mcp4728-1.3.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/adafruit_circuitpython_mcp4728.egg-info/PKG-INFO` & `adafruit-circuitpython-mcp4728-1.3.7/adafruit_circuitpython_mcp4728.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mcp4728
-Version: 1.3.6
+Version: 1.3.7
 Summary: Helper library for the MCP4728 I2C 12-bit Quad DAC
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MCP4728
 Keywords: adafruit,blinka,circuitpython,micropython,mcp4728,dac,12-bit,quad,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/adafruit_circuitpython_mcp4728.egg-info/SOURCES.txt` & `adafruit-circuitpython-mcp4728-1.3.7/adafruit_circuitpython_mcp4728.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/adafruit_mcp4728.py` & `adafruit-circuitpython-mcp4728-1.3.7/adafruit_mcp4728.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards: https://circuitpython.org/downloads
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 
-__version__ = "1.3.6"
+__version__ = "1.3.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MCP4728.git"
 
 from struct import pack_into
 from time import sleep
 from adafruit_bus_device import i2c_device
 
 try:
```

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/docs/_static/favicon.ico` & `adafruit-circuitpython-mcp4728-1.3.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/docs/conf.py` & `adafruit-circuitpython-mcp4728-1.3.7/docs/conf.py`

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

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/docs/examples.rst` & `adafruit-circuitpython-mcp4728-1.3.7/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/docs/index.rst` & `adafruit-circuitpython-mcp4728-1.3.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/examples/mcp4728_generalcalltest.py` & `adafruit-circuitpython-mcp4728-1.3.7/examples/mcp4728_generalcalltest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/examples/mcp4728_simpletest.py` & `adafruit-circuitpython-mcp4728-1.3.7/examples/mcp4728_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/examples/mcp4728_vref_example.py` & `adafruit-circuitpython-mcp4728-1.3.7/examples/mcp4728_vref_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mcp4728-1.3.6/pyproject.toml` & `adafruit-circuitpython-mcp4728-1.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-mcp4728"
 description = "Helper library for the MCP4728 I2C 12-bit Quad DAC"
-version = "1.3.6"
+version = "1.3.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MCP4728"}
 keywords = [
     "adafruit",
```

