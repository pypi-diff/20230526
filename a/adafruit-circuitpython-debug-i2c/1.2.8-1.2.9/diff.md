# Comparing `tmp/adafruit-circuitpython-debug-i2c-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-debug-i2c-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-debug-i2c-1.2.8.tar", last modified: Wed Feb 16 14:16:36 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-debug-i2c-1.2.9.tar", last modified: Fri Feb 18 19:17:48 2022, max compression
```

## Comparing `adafruit-circuitpython-debug-i2c-1.2.8.tar` & `adafruit-circuitpython-debug-i2c-1.2.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.086943 adafruit-circuitpython-debug-i2c-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.078942 adafruit-circuitpython-debug-i2c-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.082942 adafruit-circuitpython-debug-i2c-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.082942 adafruit-circuitpython-debug-i2c-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.082942 adafruit-circuitpython-debug-i2c-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-02-16 14:16:36.086943 adafruit-circuitpython-debug-i2c-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.086943 adafruit-circuitpython-debug-i2c-1.2.8/adafruit_circuitpython_debug_i2c.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4165 2022-02-16 14:16:35.000000 adafruit-circuitpython-debug-i2c-1.2.8/adafruit_circuitpython_debug_i2c.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      908 2022-02-16 14:16:35.000000 adafruit-circuitpython-debug-i2c-1.2.8/adafruit_circuitpython_debug_i2c.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-16 14:16:35.000000 adafruit-circuitpython-debug-i2c-1.2.8/adafruit_circuitpython_debug_i2c.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-02-16 14:16:35.000000 adafruit-circuitpython-debug-i2c-1.2.8/adafruit_circuitpython_debug_i2c.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-02-16 14:16:35.000000 adafruit-circuitpython-debug-i2c-1.2.8/adafruit_circuitpython_debug_i2c.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     6462 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/adafruit_debug_i2c.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.086943 adafruit-circuitpython-debug-i2c-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.086943 adafruit-circuitpython-debug-i2c-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5450 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      192 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      898 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-16 14:16:36.086943 adafruit-circuitpython-debug-i2c-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/examples/debug_i2c_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-16 14:16:36.086943 adafruit-circuitpython-debug-i2c-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1904 2022-02-16 14:16:25.000000 adafruit-circuitpython-debug-i2c-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.482915 adafruit-circuitpython-debug-i2c-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.478915 adafruit-circuitpython-debug-i2c-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.478915 adafruit-circuitpython-debug-i2c-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.478915 adafruit-circuitpython-debug-i2c-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.478915 adafruit-circuitpython-debug-i2c-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-02-18 19:17:48.482915 adafruit-circuitpython-debug-i2c-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3457 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.478915 adafruit-circuitpython-debug-i2c-1.2.9/adafruit_circuitpython_debug_i2c.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4190 2022-02-18 19:17:48.000000 adafruit-circuitpython-debug-i2c-1.2.9/adafruit_circuitpython_debug_i2c.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      908 2022-02-18 19:17:48.000000 adafruit-circuitpython-debug-i2c-1.2.9/adafruit_circuitpython_debug_i2c.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-18 19:17:48.000000 adafruit-circuitpython-debug-i2c-1.2.9/adafruit_circuitpython_debug_i2c.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-02-18 19:17:48.000000 adafruit-circuitpython-debug-i2c-1.2.9/adafruit_circuitpython_debug_i2c.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-02-18 19:17:48.000000 adafruit-circuitpython-debug-i2c-1.2.9/adafruit_circuitpython_debug_i2c.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6462 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/adafruit_debug_i2c.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.482915 adafruit-circuitpython-debug-i2c-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.482915 adafruit-circuitpython-debug-i2c-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      268 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5450 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      192 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      898 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-18 19:17:48.482915 adafruit-circuitpython-debug-i2c-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/examples/debug_i2c_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      156 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-18 19:17:48.482915 adafruit-circuitpython-debug-i2c-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-02-18 19:17:38.000000 adafruit-circuitpython-debug-i2c-1.2.9/setup.py
```

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-debug-i2c-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-debug-i2c-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-debug-i2c-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-debug-i2c-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/.pylintrc` & `adafruit-circuitpython-debug-i2c-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-debug-i2c-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/LICENSE` & `adafruit-circuitpython-debug-i2c-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-debug-i2c-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-debug-i2c-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-debug-i2c-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/PKG-INFO` & `adafruit-circuitpython-debug-i2c-1.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-debug-i2c
-Version: 1.2.8
+Version: 1.2.9
 Summary: Wrapper library for debugging I2C.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Debug_I2C
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython debug_i2c i2c debug
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-debug_i2c/badge/?version=latest
```

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/README.rst` & `adafruit-circuitpython-debug-i2c-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/adafruit_circuitpython_debug_i2c.egg-info/PKG-INFO` & `adafruit-circuitpython-debug-i2c-1.2.9/adafruit_circuitpython_debug_i2c.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-debug-i2c
-Version: 1.2.8
+Version: 1.2.9
 Summary: Wrapper library for debugging I2C.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Debug_I2C
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython debug_i2c i2c debug
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: System :: Hardware
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7.0
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 Introduction
 ============
 
 .. image:: https://readthedocs.org/projects/adafruit-circuitpython-debug_i2c/badge/?version=latest
```

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/adafruit_circuitpython_debug_i2c.egg-info/SOURCES.txt` & `adafruit-circuitpython-debug-i2c-1.2.9/adafruit_circuitpython_debug_i2c.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/adafruit_debug_i2c.py` & `adafruit-circuitpython-debug-i2c-1.2.9/adafruit_debug_i2c.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-debug-i2c-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/docs/conf.py` & `adafruit-circuitpython-debug-i2c-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/docs/index.rst` & `adafruit-circuitpython-debug-i2c-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/examples/debug_i2c_simpletest.py` & `adafruit-circuitpython-debug-i2c-1.2.9/examples/debug_i2c_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-debug-i2c-1.2.8/setup.py` & `adafruit-circuitpython-debug-i2c-1.2.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,16 @@
     long_description=long_description,
     long_description_content_type="text/x-rst",
     # The project's main homepage.
     url="https://github.com/adafruit/Adafruit_CircuitPython_Debug_I2C",
     # Author details
     author="Adafruit Industries",
     author_email="circuitpython@adafruit.com",
-    install_requires=["Adafruit-Blinka>=6.20.4", "adafruit-circuitpython-typing"],
+    python_requires=">=3.7.0",
+    install_requires=["Adafruit-Blinka>=7.0.0", "adafruit-circuitpython-typing"],
     # Choose your license
     license="MIT",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Libraries",
```

