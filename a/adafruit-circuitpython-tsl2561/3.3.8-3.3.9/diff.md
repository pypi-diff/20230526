# Comparing `tmp/adafruit-circuitpython-tsl2561-3.3.8.tar.gz` & `tmp/adafruit-circuitpython-tsl2561-3.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tsl2561-3.3.8.tar", last modified: Fri Feb  4 20:35:44 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tsl2561-3.3.9.tar", last modified: Fri Apr  1 20:05:53 2022, max compression
```

## Comparing `adafruit-circuitpython-tsl2561-3.3.8.tar` & `adafruit-circuitpython-tsl2561-3.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.779270 adafruit-circuitpython-tsl2561-3.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2593 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/adafruit_circuitpython_tsl2561.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3313 2022-02-04 20:35:44.000000 adafruit-circuitpython-tsl2561-3.3.8/adafruit_circuitpython_tsl2561.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-02-04 20:35:44.000000 adafruit-circuitpython-tsl2561-3.3.8/adafruit_circuitpython_tsl2561.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:35:44.000000 adafruit-circuitpython-tsl2561-3.3.8/adafruit_circuitpython_tsl2561.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-02-04 20:35:44.000000 adafruit-circuitpython-tsl2561-3.3.8/adafruit_circuitpython_tsl2561.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-02-04 20:35:44.000000 adafruit-circuitpython-tsl2561-3.3.8/adafruit_circuitpython_tsl2561.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     9001 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/adafruit_tsl2561.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5635 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/examples/tsl2561_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:35:44.783270 adafruit-circuitpython-tsl2561-3.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-02-04 20:35:33.000000 adafruit-circuitpython-tsl2561-3.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.160185 adafruit-circuitpython-tsl2561-3.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1113 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/adafruit_circuitpython_tsl2561.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-04-01 20:05:53.000000 adafruit-circuitpython-tsl2561-3.3.9/adafruit_circuitpython_tsl2561.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2022-04-01 20:05:53.000000 adafruit-circuitpython-tsl2561-3.3.9/adafruit_circuitpython_tsl2561.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-01 20:05:53.000000 adafruit-circuitpython-tsl2561-3.3.9/adafruit_circuitpython_tsl2561.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-04-01 20:05:53.000000 adafruit-circuitpython-tsl2561-3.3.9/adafruit_circuitpython_tsl2561.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-04-01 20:05:53.000000 adafruit-circuitpython-tsl2561-3.3.9/adafruit_circuitpython_tsl2561.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8999 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/adafruit_tsl2561.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5635 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1183 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-01 20:05:53.156185 adafruit-circuitpython-tsl2561-3.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1458 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/examples/tsl2561_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-01 20:05:53.160185 adafruit-circuitpython-tsl2561-3.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2022-04-01 20:05:41.000000 adafruit-circuitpython-tsl2561-3.3.9/setup.py
```

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tsl2561-3.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-tsl2561-3.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-tsl2561-3.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tsl2561-3.3.9/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # SPDX-FileCopyrightText: 2020 Diego Elio Pettenò
 #
 # SPDX-License-Identifier: Unlicense
 
 repos:
 -   repo: https://github.com/python/black
-    rev: 20.8b1
+    rev: 22.3.0
     hooks:
     - id: black
 -   repo: https://github.com/fsfe/reuse-tool
     rev: v0.12.1
     hooks:
     - id: reuse
 -   repo: https://github.com/pre-commit/pre-commit-hooks
```

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/.pylintrc` & `adafruit-circuitpython-tsl2561-3.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tsl2561-3.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/LICENSE` & `adafruit-circuitpython-tsl2561-3.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tsl2561-3.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tsl2561-3.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tsl2561-3.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/PKG-INFO` & `adafruit-circuitpython-tsl2561-3.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tsl2561
-Version: 3.3.8
+Version: 3.3.9
 Summary: CircuitPython library for TSL2561 Light Sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TSL2561
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit tsl2561 light sensor hardware micropython circuitpython
 Platform: UNKNOWN
@@ -85,20 +85,17 @@
     3294.37
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/tsl2561/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_CircuitPython_TSL2561/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/README.rst` & `adafruit-circuitpython-tsl2561-3.3.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -66,18 +66,15 @@
     3294.37
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/tsl2561/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_CircuitPython_TSL2561/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/adafruit_circuitpython_tsl2561.egg-info/PKG-INFO` & `adafruit-circuitpython-tsl2561-3.3.9/adafruit_circuitpython_tsl2561.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tsl2561
-Version: 3.3.8
+Version: 3.3.9
 Summary: CircuitPython library for TSL2561 Light Sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TSL2561
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit tsl2561 light sensor hardware micropython circuitpython
 Platform: UNKNOWN
@@ -85,20 +85,17 @@
     3294.37
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/tsl2561/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/Adafruit_CircuitPython_CircuitPython_TSL2561/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/adafruit_circuitpython_tsl2561.egg-info/SOURCES.txt` & `adafruit-circuitpython-tsl2561-3.3.9/adafruit_circuitpython_tsl2561.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/adafruit_tsl2561.py` & `adafruit-circuitpython-tsl2561-3.3.9/adafruit_tsl2561.py`

 * *Files 1% similar despite different names*

```diff
@@ -225,15 +225,15 @@
             return None
         if ch0 > _CLIP_THRESHOLD[self.integration_time]:
             return None
         if ch1 > _CLIP_THRESHOLD[self.integration_time]:
             return None
         ratio = ch1 / ch0
         if 0 <= ratio <= 0.50:
-            lux = 0.0304 * ch0 - 0.062 * ch0 * ratio ** 1.4
+            lux = 0.0304 * ch0 - 0.062 * ch0 * ratio**1.4
         elif ratio <= 0.61:
             lux = 0.0224 * ch0 - 0.031 * ch1
         elif ratio <= 0.80:
             lux = 0.0128 * ch0 - 0.0153 * ch1
         elif ratio <= 1.30:
             lux = 0.00146 * ch0 - 0.00112 * ch1
         else:
```

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tsl2561-3.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/docs/conf.py` & `adafruit-circuitpython-tsl2561-3.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/docs/index.rst` & `adafruit-circuitpython-tsl2561-3.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/examples/tsl2561_simpletest.py` & `adafruit-circuitpython-tsl2561-3.3.9/examples/tsl2561_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tsl2561-3.3.8/setup.py` & `adafruit-circuitpython-tsl2561-3.3.9/setup.py`

 * *Files identical despite different names*

