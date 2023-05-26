# Comparing `tmp/adafruit-circuitpython-ssd1331-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-ssd1331-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1331-1.3.8.tar", last modified: Thu May 18 15:19:52 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1331-1.3.9.tar", last modified: Fri May 26 16:13:13 2023, max compression
```

## Comparing `adafruit-circuitpython-ssd1331-1.3.8.tar` & `adafruit-circuitpython-ssd1331-1.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.419428 adafruit-circuitpython-ssd1331-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.407428 adafruit-circuitpython-ssd1331-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.411428 adafruit-circuitpython-ssd1331-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.415428 adafruit-circuitpython-ssd1331-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.415428 adafruit-circuitpython-ssd1331-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-18 15:19:52.419428 adafruit-circuitpython-ssd1331-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.415428 adafruit-circuitpython-ssd1331-1.3.8/adafruit_circuitpython_ssd1331.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-18 15:19:52.000000 adafruit-circuitpython-ssd1331-1.3.8/adafruit_circuitpython_ssd1331.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-18 15:19:52.000000 adafruit-circuitpython-ssd1331-1.3.8/adafruit_circuitpython_ssd1331.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:19:52.000000 adafruit-circuitpython-ssd1331-1.3.8/adafruit_circuitpython_ssd1331.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-18 15:19:52.000000 adafruit-circuitpython-ssd1331-1.3.8/adafruit_circuitpython_ssd1331.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:19:52.000000 adafruit-circuitpython-ssd1331-1.3.8/adafruit_circuitpython_ssd1331.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-05-18 15:19:42.000000 adafruit-circuitpython-ssd1331-1.3.8/adafruit_ssd1331.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.415428 adafruit-circuitpython-ssd1331-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.419428 adafruit-circuitpython-ssd1331-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5711 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:19:52.419428 adafruit-circuitpython-ssd1331-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-18 15:19:42.000000 adafruit-circuitpython-ssd1331-1.3.8/examples/ssd1331_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-18 15:19:42.000000 adafruit-circuitpython-ssd1331-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-18 15:19:29.000000 adafruit-circuitpython-ssd1331-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:19:52.419428 adafruit-circuitpython-ssd1331-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.168934 adafruit-circuitpython-ssd1331-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.156934 adafruit-circuitpython-ssd1331-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.160934 adafruit-circuitpython-ssd1331-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.160934 adafruit-circuitpython-ssd1331-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.160934 adafruit-circuitpython-ssd1331-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-26 16:13:13.168934 adafruit-circuitpython-ssd1331-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.164934 adafruit-circuitpython-ssd1331-1.3.9/adafruit_circuitpython_ssd1331.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-05-26 16:13:13.000000 adafruit-circuitpython-ssd1331-1.3.9/adafruit_circuitpython_ssd1331.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 16:13:13.000000 adafruit-circuitpython-ssd1331-1.3.9/adafruit_circuitpython_ssd1331.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:13:13.000000 adafruit-circuitpython-ssd1331-1.3.9/adafruit_circuitpython_ssd1331.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 16:13:13.000000 adafruit-circuitpython-ssd1331-1.3.9/adafruit_circuitpython_ssd1331.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:13:13.000000 adafruit-circuitpython-ssd1331-1.3.9/adafruit_circuitpython_ssd1331.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1902 2023-05-26 16:13:04.000000 adafruit-circuitpython-ssd1331-1.3.9/adafruit_ssd1331.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.164934 adafruit-circuitpython-ssd1331-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.164934 adafruit-circuitpython-ssd1331-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:13.164934 adafruit-circuitpython-ssd1331-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-05-26 16:13:04.000000 adafruit-circuitpython-ssd1331-1.3.9/examples/ssd1331_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-05-26 16:13:04.000000 adafruit-circuitpython-ssd1331-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 16:12:50.000000 adafruit-circuitpython-ssd1331-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:13:13.168934 adafruit-circuitpython-ssd1331-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1331-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/.gitignore` & `adafruit-circuitpython-ssd1331-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1331-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/.pylintrc` & `adafruit-circuitpython-ssd1331-1.3.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1331-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/LICENSE` & `adafruit-circuitpython-ssd1331-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1331-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1331-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1331-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/PKG-INFO` & `adafruit-circuitpython-ssd1331-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1331
-Version: 1.3.8
+Version: 1.3.9
 Summary: displayio driver for SSD1331 TFT-LCD displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1331
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1331,display,tft,lcd,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/README.rst` & `adafruit-circuitpython-ssd1331-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/adafruit_circuitpython_ssd1331.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1331-1.3.9/adafruit_circuitpython_ssd1331.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1331
-Version: 1.3.8
+Version: 1.3.9
 Summary: displayio driver for SSD1331 TFT-LCD displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1331
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1331,display,tft,lcd,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/adafruit_circuitpython_ssd1331.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1331-1.3.9/adafruit_circuitpython_ssd1331.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/adafruit_ssd1331.py` & `adafruit-circuitpython-ssd1331-1.3.9/adafruit_ssd1331.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1331.git"
 
 _INIT_SEQUENCE = (
     b"\xAE\x00"  # _DISPLAYOFF
     b"\xA0\x01\x72"  # _SETREMAP (RGB)
     b"\xA1\x01\x00"  # _STARTLINE
     b"\xA2\x01\x00"  # _DISPLAYOFFSET
```

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1331-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/docs/conf.py` & `adafruit-circuitpython-ssd1331-1.3.9/docs/conf.py`

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

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/docs/index.rst` & `adafruit-circuitpython-ssd1331-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/examples/ssd1331_simpletest.py` & `adafruit-circuitpython-ssd1331-1.3.9/examples/ssd1331_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1331-1.3.8/pyproject.toml` & `adafruit-circuitpython-ssd1331-1.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ssd1331"
 description = "displayio driver for SSD1331 TFT-LCD displays."
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1331"}
 keywords = [
     "adafruit",
```

