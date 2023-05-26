# Comparing `tmp/adafruit-circuitpython-ble-creation-0.9.5.tar.gz` & `tmp/adafruit-circuitpython-ble-creation-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ble-creation-0.9.5.tar", last modified: Thu May 18 15:30:25 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ble-creation-0.9.6.tar", last modified: Fri May 26 16:08:25 2023, max compression
```

## Comparing `adafruit-circuitpython-ble-creation-0.9.5.tar` & `adafruit-circuitpython-ble-creation-0.9.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.993791 adafruit-circuitpython-ble-creation-0.9.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.989791 adafruit-circuitpython-ble-creation-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.989791 adafruit-circuitpython-ble-creation-0.9.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.989791 adafruit-circuitpython-ble-creation-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.989791 adafruit-circuitpython-ble-creation-0.9.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-18 15:30:25.993791 adafruit-circuitpython-ble-creation-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-18 15:30:16.000000 adafruit-circuitpython-ble-creation-0.9.5/adafruit_ble_creation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.989791 adafruit-circuitpython-ble-creation-0.9.5/adafruit_circuitpython_ble_creation.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-18 15:30:25.000000 adafruit-circuitpython-ble-creation-0.9.5/adafruit_circuitpython_ble_creation.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-18 15:30:25.000000 adafruit-circuitpython-ble-creation-0.9.5/adafruit_circuitpython_ble_creation.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:30:25.000000 adafruit-circuitpython-ble-creation-0.9.5/adafruit_circuitpython_ble_creation.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-18 15:30:25.000000 adafruit-circuitpython-ble-creation-0.9.5/adafruit_circuitpython_ble_creation.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-18 15:30:25.000000 adafruit-circuitpython-ble-creation-0.9.5/adafruit_circuitpython_ble_creation.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.993791 adafruit-circuitpython-ble-creation-0.9.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.993791 adafruit-circuitpython-ble-creation-0.9.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5807 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:30:25.993791 adafruit-circuitpython-ble-creation-0.9.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-18 15:30:16.000000 adafruit-circuitpython-ble-creation-0.9.5/examples/ble_creation_advertise.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-18 15:30:16.000000 adafruit-circuitpython-ble-creation-0.9.5/examples/ble_creation_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-18 15:30:16.000000 adafruit-circuitpython-ble-creation-0.9.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-18 15:30:02.000000 adafruit-circuitpython-ble-creation-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:30:25.993791 adafruit-circuitpython-ble-creation-0.9.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.744086 adafruit-circuitpython-ble-creation-0.9.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.736086 adafruit-circuitpython-ble-creation-0.9.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.740085 adafruit-circuitpython-ble-creation-0.9.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.740085 adafruit-circuitpython-ble-creation-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.740085 adafruit-circuitpython-ble-creation-0.9.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-26 16:08:25.744086 adafruit-circuitpython-ble-creation-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-05-26 16:08:18.000000 adafruit-circuitpython-ble-creation-0.9.6/adafruit_ble_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.740085 adafruit-circuitpython-ble-creation-0.9.6/adafruit_circuitpython_ble_creation.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-05-26 16:08:25.000000 adafruit-circuitpython-ble-creation-0.9.6/adafruit_circuitpython_ble_creation.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-26 16:08:25.000000 adafruit-circuitpython-ble-creation-0.9.6/adafruit_circuitpython_ble_creation.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:08:25.000000 adafruit-circuitpython-ble-creation-0.9.6/adafruit_circuitpython_ble_creation.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 16:08:25.000000 adafruit-circuitpython-ble-creation-0.9.6/adafruit_circuitpython_ble_creation.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 16:08:25.000000 adafruit-circuitpython-ble-creation-0.9.6/adafruit_circuitpython_ble_creation.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.740085 adafruit-circuitpython-ble-creation-0.9.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.744086 adafruit-circuitpython-ble-creation-0.9.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5835 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:08:25.744086 adafruit-circuitpython-ble-creation-0.9.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-26 16:08:18.000000 adafruit-circuitpython-ble-creation-0.9.6/examples/ble_creation_advertise.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-26 16:08:18.000000 adafruit-circuitpython-ble-creation-0.9.6/examples/ble_creation_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-05-26 16:08:18.000000 adafruit-circuitpython-ble-creation-0.9.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-26 16:08:09.000000 adafruit-circuitpython-ble-creation-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:08:25.744086 adafruit-circuitpython-ble-creation-0.9.6/setup.cfg
```

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ble-creation-0.9.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/.gitignore` & `adafruit-circuitpython-ble-creation-0.9.6/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/.pre-commit-config.yaml` & `adafruit-circuitpython-ble-creation-0.9.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/.pylintrc` & `adafruit-circuitpython-ble-creation-0.9.6/.pylintrc`

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

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ble-creation-0.9.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/LICENSE` & `adafruit-circuitpython-ble-creation-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ble-creation-0.9.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/LICENSES/MIT.txt` & `adafruit-circuitpython-ble-creation-0.9.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ble-creation-0.9.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/PKG-INFO` & `adafruit-circuitpython-ble-creation-0.9.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-creation
-Version: 0.9.5
+Version: 0.9.6
 Summary: Friendlier device discovery using Creation IDs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Creation
 Keywords: adafruit,blinka,circuitpython,micropython,ble_creation
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/README.rst` & `adafruit-circuitpython-ble-creation-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/adafruit_ble_creation.py` & `adafruit-circuitpython-ble-creation-0.9.6/adafruit_ble_creation.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 )
 from adafruit_ble.advertising.adafruit import (
     MANUFACTURING_DATA_ADT,
     ADAFRUIT_COMPANY_ID,
 )
 from micropython import const
 
-__version__ = "0.9.5"
+__version__ = "0.9.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Creation.git"
 
 # Color packets are 1 (and radio), broadcastnet is 3.
 _DEVICE_FRIEND_DATA_ID = const(0x0004)
 
 
 # pylint: disable=too-few-public-methods
```

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/adafruit_circuitpython_ble_creation.egg-info/PKG-INFO` & `adafruit-circuitpython-ble-creation-0.9.6/adafruit_circuitpython_ble_creation.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ble-creation
-Version: 0.9.5
+Version: 0.9.6
 Summary: Friendlier device discovery using Creation IDs
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_BLE_Creation
 Keywords: adafruit,blinka,circuitpython,micropython,ble_creation
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/adafruit_circuitpython_ble_creation.egg-info/SOURCES.txt` & `adafruit-circuitpython-ble-creation-0.9.6/adafruit_circuitpython_ble_creation.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/docs/_static/favicon.ico` & `adafruit-circuitpython-ble-creation-0.9.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/docs/conf.py` & `adafruit-circuitpython-ble-creation-0.9.6/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
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

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/docs/index.rst` & `adafruit-circuitpython-ble-creation-0.9.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/examples/ble_creation_advertise.py` & `adafruit-circuitpython-ble-creation-0.9.6/examples/ble_creation_advertise.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/examples/ble_creation_simpletest.py` & `adafruit-circuitpython-ble-creation-0.9.6/examples/ble_creation_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ble-creation-0.9.5/pyproject.toml` & `adafruit-circuitpython-ble-creation-0.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ble-creation"
 description = "Friendlier device discovery using Creation IDs"
-version = "0.9.5"
+version = "0.9.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_BLE_Creation"}
 keywords = [
     "adafruit",
```

