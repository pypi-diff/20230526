# Comparing `tmp/adafruit-circuitpython-lps2x-3.0.2.tar.gz` & `tmp/adafruit-circuitpython-lps2x-3.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lps2x-3.0.2.tar", last modified: Tue May 16 17:58:47 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-lps2x-3.0.3.tar", last modified: Fri May 26 16:11:55 2023, max compression
```

## Comparing `adafruit-circuitpython-lps2x-3.0.2.tar` & `adafruit-circuitpython-lps2x-3.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.520136 adafruit-circuitpython-lps2x-3.0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.520136 adafruit-circuitpython-lps2x-3.0.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.520136 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-16 17:58:47.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-16 17:58:39.000000 adafruit-circuitpython-lps2x-3.0.2/adafruit_lps2x.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5891 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-16 17:58:39.000000 adafruit-circuitpython-lps2x-3.0.2/examples/lps2x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-16 17:58:39.000000 adafruit-circuitpython-lps2x-3.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:58:29.000000 adafruit-circuitpython-lps2x-3.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:58:47.524136 adafruit-circuitpython-lps2x-3.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.284374 adafruit-circuitpython-lps2x-3.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.272374 adafruit-circuitpython-lps2x-3.0.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.276374 adafruit-circuitpython-lps2x-3.0.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.276374 adafruit-circuitpython-lps2x-3.0.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.280374 adafruit-circuitpython-lps2x-3.0.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-26 16:11:55.280374 adafruit-circuitpython-lps2x-3.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2966 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.280374 adafruit-circuitpython-lps2x-3.0.3/adafruit_circuitpython_lps2x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-05-26 16:11:55.000000 adafruit-circuitpython-lps2x-3.0.3/adafruit_circuitpython_lps2x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 16:11:55.000000 adafruit-circuitpython-lps2x-3.0.3/adafruit_circuitpython_lps2x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:11:55.000000 adafruit-circuitpython-lps2x-3.0.3/adafruit_circuitpython_lps2x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:11:55.000000 adafruit-circuitpython-lps2x-3.0.3/adafruit_circuitpython_lps2x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 16:11:55.000000 adafruit-circuitpython-lps2x-3.0.3/adafruit_circuitpython_lps2x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-26 16:11:46.000000 adafruit-circuitpython-lps2x-3.0.3/adafruit_lps2x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.280374 adafruit-circuitpython-lps2x-3.0.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.280374 adafruit-circuitpython-lps2x-3.0.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5919 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:55.280374 adafruit-circuitpython-lps2x-3.0.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-26 16:11:46.000000 adafruit-circuitpython-lps2x-3.0.3/examples/lps2x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-05-26 16:11:46.000000 adafruit-circuitpython-lps2x-3.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:11:33.000000 adafruit-circuitpython-lps2x-3.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:11:55.284374 adafruit-circuitpython-lps2x-3.0.3/setup.cfg
```

### Comparing `adafruit-circuitpython-lps2x-3.0.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-lps2x-3.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/.gitignore` & `adafruit-circuitpython-lps2x-3.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/.pre-commit-config.yaml` & `adafruit-circuitpython-lps2x-3.0.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/.pylintrc` & `adafruit-circuitpython-lps2x-3.0.3/.pylintrc`

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

### Comparing `adafruit-circuitpython-lps2x-3.0.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lps2x-3.0.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/LICENSE` & `adafruit-circuitpython-lps2x-3.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lps2x-3.0.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/LICENSES/MIT.txt` & `adafruit-circuitpython-lps2x-3.0.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lps2x-3.0.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/PKG-INFO` & `adafruit-circuitpython-lps2x-3.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lps2x
-Version: 3.0.2
+Version: 3.0.3
 Summary: Library for the ST LPS2x family of pressure sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LPS2x
 Keywords: adafruit,blinka,circuitpython,micropython,lps2x,LPS25,LPS,pressure,MEMS,barometric
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lps2x-3.0.2/README.rst` & `adafruit-circuitpython-lps2x-3.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/PKG-INFO` & `adafruit-circuitpython-lps2x-3.0.3/adafruit_circuitpython_lps2x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lps2x
-Version: 3.0.2
+Version: 3.0.3
 Summary: Library for the ST LPS2x family of pressure sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_LPS2x
 Keywords: adafruit,blinka,circuitpython,micropython,lps2x,LPS25,LPS,pressure,MEMS,barometric
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-lps2x-3.0.2/adafruit_circuitpython_lps2x.egg-info/SOURCES.txt` & `adafruit-circuitpython-lps2x-3.0.3/adafruit_circuitpython_lps2x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/adafruit_lps2x.py` & `adafruit-circuitpython-lps2x-3.0.3/adafruit_lps2x.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     https://circuitpythohn.org/downloads
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 
 """
-__version__ = "3.0.2"
+__version__ = "3.0.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LPS2X.git"
 from time import sleep
 from micropython import const
 import adafruit_bus_device.i2c_device as i2cdevice
 from adafruit_register.i2c_struct import ROUnaryStruct
 from adafruit_register.i2c_bits import RWBits, ROBits
 from adafruit_register.i2c_bit import RWBit
```

### Comparing `adafruit-circuitpython-lps2x-3.0.2/docs/_static/favicon.ico` & `adafruit-circuitpython-lps2x-3.0.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/docs/conf.py` & `adafruit-circuitpython-lps2x-3.0.3/docs/conf.py`

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

### Comparing `adafruit-circuitpython-lps2x-3.0.2/docs/index.rst` & `adafruit-circuitpython-lps2x-3.0.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/examples/lps2x_simpletest.py` & `adafruit-circuitpython-lps2x-3.0.3/examples/lps2x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lps2x-3.0.2/pyproject.toml` & `adafruit-circuitpython-lps2x-3.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-lps2x"
 description = "Library for the ST LPS2x family of pressure sensors"
-version = "3.0.2"
+version = "3.0.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_LPS2x"}
 keywords = [
     "adafruit",
```

