# Comparing `tmp/adafruit-circuitpython-mma8451-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-mma8451-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-mma8451-1.3.8.tar", last modified: Mon Nov 15 18:57:22 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-mma8451-1.3.9.tar", last modified: Wed Dec 29 22:45:09 2021, max compression
```

## Comparing `adafruit-circuitpython-mma8451-1.3.8.tar` & `adafruit-circuitpython-mma8451-1.3.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.303148 adafruit-circuitpython-mma8451-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.303148 adafruit-circuitpython-mma8451-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3619 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2775 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/adafruit_circuitpython_mma8451.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3619 2021-11-15 18:57:21.000000 adafruit-circuitpython-mma8451-1.3.8/adafruit_circuitpython_mma8451.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      894 2021-11-15 18:57:22.000000 adafruit-circuitpython-mma8451-1.3.8/adafruit_circuitpython_mma8451.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 18:57:21.000000 adafruit-circuitpython-mma8451-1.3.8/adafruit_circuitpython_mma8451.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-15 18:57:21.000000 adafruit-circuitpython-mma8451-1.3.8/adafruit_circuitpython_mma8451.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-11-15 18:57:21.000000 adafruit-circuitpython-mma8451-1.3.8/adafruit_circuitpython_mma8451.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     8878 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/adafruit_mma8451.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5327 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/examples/mma8451_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      159 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 18:57:22.307148 adafruit-circuitpython-mma8451-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1960 2021-11-15 18:57:04.000000 adafruit-circuitpython-mma8451-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.380656 adafruit-circuitpython-mma8451-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.376656 adafruit-circuitpython-mma8451-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.376656 adafruit-circuitpython-mma8451-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.376656 adafruit-circuitpython-mma8451-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.376656 adafruit-circuitpython-mma8451-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3619 2021-12-29 22:45:09.380656 adafruit-circuitpython-mma8451-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2775 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.376656 adafruit-circuitpython-mma8451-1.3.9/adafruit_circuitpython_mma8451.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3619 2021-12-29 22:45:09.000000 adafruit-circuitpython-mma8451-1.3.9/adafruit_circuitpython_mma8451.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      894 2021-12-29 22:45:09.000000 adafruit-circuitpython-mma8451-1.3.9/adafruit_circuitpython_mma8451.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-29 22:45:09.000000 adafruit-circuitpython-mma8451-1.3.9/adafruit_circuitpython_mma8451.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-29 22:45:09.000000 adafruit-circuitpython-mma8451-1.3.9/adafruit_circuitpython_mma8451.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-12-29 22:45:09.000000 adafruit-circuitpython-mma8451-1.3.9/adafruit_circuitpython_mma8451.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8820 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/adafruit_mma8451.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.376656 adafruit-circuitpython-mma8451-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.380656 adafruit-circuitpython-mma8451-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5327 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1165 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-29 22:45:09.380656 adafruit-circuitpython-mma8451-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2683 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/examples/mma8451_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      159 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-12-29 22:45:09.380656 adafruit-circuitpython-mma8451-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1960 2021-12-29 22:44:59.000000 adafruit-circuitpython-mma8451-1.3.9/setup.py
```

### Comparing `adafruit-circuitpython-mma8451-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-mma8451-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-mma8451-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-mma8451-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-mma8451-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/.pylintrc` & `adafruit-circuitpython-mma8451-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-mma8451-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/LICENSE` & `adafruit-circuitpython-mma8451-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-mma8451-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-mma8451-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-mma8451-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/PKG-INFO` & `adafruit-circuitpython-mma8451-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mma8451
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for MMA8451 3-axis accelerometer..
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MMA8451
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit mma8451 axis accelerometer breakout hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-mma8451-1.3.8/README.rst` & `adafruit-circuitpython-mma8451-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/adafruit_circuitpython_mma8451.egg-info/PKG-INFO` & `adafruit-circuitpython-mma8451-1.3.9/adafruit_circuitpython_mma8451.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-mma8451
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for MMA8451 3-axis accelerometer..
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MMA8451
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit mma8451 axis accelerometer breakout hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-mma8451-1.3.8/adafruit_circuitpython_mma8451.egg-info/SOURCES.txt` & `adafruit-circuitpython-mma8451-1.3.9/adafruit_circuitpython_mma8451.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/adafruit_mma8451.py` & `adafruit-circuitpython-mma8451-1.3.9/adafruit_mma8451.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,18 +24,15 @@
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
 * Adafruit's Bus Device library:
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 
 """
-try:
-    import struct
-except ImportError:
-    import ustruct as struct
+import struct
 
 from micropython import const
 
 from adafruit_bus_device import i2c_device
 
 
 __version__ = "0.0.0-auto.0"
```

### Comparing `adafruit-circuitpython-mma8451-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-mma8451-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/docs/conf.py` & `adafruit-circuitpython-mma8451-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/docs/index.rst` & `adafruit-circuitpython-mma8451-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/examples/mma8451_simpletest.py` & `adafruit-circuitpython-mma8451-1.3.9/examples/mma8451_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-mma8451-1.3.8/setup.py` & `adafruit-circuitpython-mma8451-1.3.9/setup.py`

 * *Files identical despite different names*

