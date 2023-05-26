# Comparing `tmp/adafruit-circuitpython-ens160-1.0.3.tar.gz` & `tmp/adafruit-circuitpython-ens160-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ens160-1.0.3.tar", last modified: Thu May 18 15:35:32 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ens160-1.0.4.tar", last modified: Fri May 26 16:09:59 2023, max compression
```

## Comparing `adafruit-circuitpython-ens160-1.0.3.tar` & `adafruit-circuitpython-ens160-1.0.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.803602 adafruit-circuitpython-ens160-1.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.803602 adafruit-circuitpython-ens160-1.0.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.803602 adafruit-circuitpython-ens160-1.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.803602 adafruit-circuitpython-ens160-1.0.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:35:32.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-18 15:35:25.000000 adafruit-circuitpython-ens160-1.0.3/adafruit_ens160.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6057 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-18 15:35:25.000000 adafruit-circuitpython-ens160-1.0.3/examples/ens160_advancedtest.py
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-18 15:35:25.000000 adafruit-circuitpython-ens160-1.0.3/examples/ens160_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-18 15:35:25.000000 adafruit-circuitpython-ens160-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-18 15:35:17.000000 adafruit-circuitpython-ens160-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:35:32.807602 adafruit-circuitpython-ens160-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.879176 adafruit-circuitpython-ens160-1.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.871176 adafruit-circuitpython-ens160-1.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.875176 adafruit-circuitpython-ens160-1.0.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.875176 adafruit-circuitpython-ens160-1.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.875176 adafruit-circuitpython-ens160-1.0.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-26 16:09:59.879176 adafruit-circuitpython-ens160-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.875176 adafruit-circuitpython-ens160-1.0.4/adafruit_circuitpython_ens160.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4199 2023-05-26 16:09:59.000000 adafruit-circuitpython-ens160-1.0.4/adafruit_circuitpython_ens160.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 16:09:59.000000 adafruit-circuitpython-ens160-1.0.4/adafruit_circuitpython_ens160.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:09:59.000000 adafruit-circuitpython-ens160-1.0.4/adafruit_circuitpython_ens160.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 16:09:59.000000 adafruit-circuitpython-ens160-1.0.4/adafruit_circuitpython_ens160.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:09:59.000000 adafruit-circuitpython-ens160-1.0.4/adafruit_circuitpython_ens160.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-05-26 16:09:52.000000 adafruit-circuitpython-ens160-1.0.4/adafruit_ens160.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.879176 adafruit-circuitpython-ens160-1.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.879176 adafruit-circuitpython-ens160-1.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6085 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:59.879176 adafruit-circuitpython-ens160-1.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-26 16:09:52.000000 adafruit-circuitpython-ens160-1.0.4/examples/ens160_advancedtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-26 16:09:52.000000 adafruit-circuitpython-ens160-1.0.4/examples/ens160_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-05-26 16:09:52.000000 adafruit-circuitpython-ens160-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-26 16:09:41.000000 adafruit-circuitpython-ens160-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:09:59.879176 adafruit-circuitpython-ens160-1.0.4/setup.cfg
```

### Comparing `adafruit-circuitpython-ens160-1.0.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ens160-1.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/.gitignore` & `adafruit-circuitpython-ens160-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/.pre-commit-config.yaml` & `adafruit-circuitpython-ens160-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/.pylintrc` & `adafruit-circuitpython-ens160-1.0.4/.pylintrc`

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

### Comparing `adafruit-circuitpython-ens160-1.0.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ens160-1.0.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/LICENSE` & `adafruit-circuitpython-ens160-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ens160-1.0.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/LICENSES/MIT.txt` & `adafruit-circuitpython-ens160-1.0.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ens160-1.0.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/PKG-INFO` & `adafruit-circuitpython-ens160-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ens160
-Version: 1.0.3
+Version: 1.0.4
 Summary: CircuitPython / Python library for ScioSense ENS160 digital multi-gas sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ENS160
 Keywords: adafruit,blinka,circuitpython,micropython,ens160,ens160,python,circuitpython,gas,tvoc,eco2,mox,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ens160-1.0.3/README.rst` & `adafruit-circuitpython-ens160-1.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/PKG-INFO` & `adafruit-circuitpython-ens160-1.0.4/adafruit_circuitpython_ens160.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ens160
-Version: 1.0.3
+Version: 1.0.4
 Summary: CircuitPython / Python library for ScioSense ENS160 digital multi-gas sensor
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ENS160
 Keywords: adafruit,blinka,circuitpython,micropython,ens160,ens160,python,circuitpython,gas,tvoc,eco2,mox,sensor
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ens160-1.0.3/adafruit_circuitpython_ens160.egg-info/SOURCES.txt` & `adafruit-circuitpython-ens160-1.0.4/adafruit_circuitpython_ens160.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/adafruit_ens160.py` & `adafruit-circuitpython-ens160-1.0.4/adafruit_ens160.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 try:
     from typing import Dict, Optional, Union, List
     from typing_extensions import Literal
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ENS160.git"
 
 
 ENS160_I2CADDR_DEFAULT: int = const(0x53)  # Default I2C address
 
 _ENS160_REG_PARTID = const(0x00)
 _ENS160_REG_OPMODE = const(0x10)
```

### Comparing `adafruit-circuitpython-ens160-1.0.3/docs/_static/favicon.ico` & `adafruit-circuitpython-ens160-1.0.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/docs/conf.py` & `adafruit-circuitpython-ens160-1.0.4/docs/conf.py`

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

### Comparing `adafruit-circuitpython-ens160-1.0.3/docs/index.rst` & `adafruit-circuitpython-ens160-1.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/examples/ens160_advancedtest.py` & `adafruit-circuitpython-ens160-1.0.4/examples/ens160_advancedtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/examples/ens160_simpletest.py` & `adafruit-circuitpython-ens160-1.0.4/examples/ens160_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ens160-1.0.3/pyproject.toml` & `adafruit-circuitpython-ens160-1.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ens160"
 description = "CircuitPython / Python library for ScioSense ENS160 digital multi-gas sensor"
-version = "1.0.3"
+version = "1.0.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ENS160"}
 keywords = [
     "adafruit",
```

