# Comparing `tmp/adafruit-circuitpython-pcd8544-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-pcd8544-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pcd8544-1.2.8.tar", last modified: Tue Jun  7 17:00:59 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pcd8544-1.2.9.tar", last modified: Thu Jun  9 18:11:13 2022, max compression
```

## Comparing `adafruit-circuitpython-pcd8544-1.2.8.tar` & `adafruit-circuitpython-pcd8544-1.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.870602 adafruit-circuitpython-pcd8544-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/adafruit_circuitpython_pcd8544.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-06-07 17:00:59.000000 adafruit-circuitpython-pcd8544-1.2.8/adafruit_circuitpython_pcd8544.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      926 2022-06-07 17:00:59.000000 adafruit-circuitpython-pcd8544-1.2.8/adafruit_circuitpython_pcd8544.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:00:59.000000 adafruit-circuitpython-pcd8544-1.2.8/adafruit_circuitpython_pcd8544.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-07 17:00:59.000000 adafruit-circuitpython-pcd8544-1.2.8/adafruit_circuitpython_pcd8544.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-07 17:00:59.000000 adafruit-circuitpython-pcd8544-1.2.8/adafruit_circuitpython_pcd8544.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4661 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/adafruit_pcd8544.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      894 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/examples/pcd8544_pillow_demo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/examples/pcd8544_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:00:59.874601 adafruit-circuitpython-pcd8544-1.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-06-07 17:00:45.000000 adafruit-circuitpython-pcd8544-1.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.143389 adafruit-circuitpython-pcd8544-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2465 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/adafruit_circuitpython_pcd8544.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-06-09 18:11:13.000000 adafruit-circuitpython-pcd8544-1.2.9/adafruit_circuitpython_pcd8544.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      926 2022-06-09 18:11:13.000000 adafruit-circuitpython-pcd8544-1.2.9/adafruit_circuitpython_pcd8544.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:11:13.000000 adafruit-circuitpython-pcd8544-1.2.9/adafruit_circuitpython_pcd8544.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-09 18:11:13.000000 adafruit-circuitpython-pcd8544-1.2.9/adafruit_circuitpython_pcd8544.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-06-09 18:11:13.000000 adafruit-circuitpython-pcd8544-1.2.9/adafruit_circuitpython_pcd8544.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4661 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/adafruit_pcd8544.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5532 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1970 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/examples/pcd8544_pillow_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2112 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/examples/pcd8544_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:11:13.147389 adafruit-circuitpython-pcd8544-1.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1961 2022-06-09 18:11:00.000000 adafruit-circuitpython-pcd8544-1.2.9/setup.py
```

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pcd8544-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-pcd8544-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-pcd8544-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/.gitignore` & `adafruit-circuitpython-pcd8544-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pcd8544-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/.pylintrc` & `adafruit-circuitpython-pcd8544-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pcd8544-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/LICENSE` & `adafruit-circuitpython-pcd8544-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pcd8544-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pcd8544-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pcd8544-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/PKG-INFO` & `adafruit-circuitpython-pcd8544-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcd8544
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython display control library for Nokia PCD8544 monochrome displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PCD8544
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit display nokia pcd8544 monochrome displays hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/README.rst` & `adafruit-circuitpython-pcd8544-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/adafruit_circuitpython_pcd8544.egg-info/PKG-INFO` & `adafruit-circuitpython-pcd8544-1.2.9/adafruit_circuitpython_pcd8544.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pcd8544
-Version: 1.2.8
+Version: 1.2.9
 Summary: CircuitPython display control library for Nokia PCD8544 monochrome displays.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PCD8544
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit display nokia pcd8544 monochrome displays hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/adafruit_circuitpython_pcd8544.egg-info/SOURCES.txt` & `adafruit-circuitpython-pcd8544-1.2.9/adafruit_circuitpython_pcd8544.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/adafruit_pcd8544.py` & `adafruit-circuitpython-pcd8544-1.2.9/adafruit_pcd8544.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pcd8544-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/docs/conf.py` & `adafruit-circuitpython-pcd8544-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/docs/index.rst` & `adafruit-circuitpython-pcd8544-1.2.9/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -25,15 +25,16 @@
 
 .. toctree::
     :caption: Related Products
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_PCD8544/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_PCD8544/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/examples/pcd8544_pillow_demo.py` & `adafruit-circuitpython-pcd8544-1.2.9/examples/pcd8544_pillow_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/examples/pcd8544_simpletest.py` & `adafruit-circuitpython-pcd8544-1.2.9/examples/pcd8544_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pcd8544-1.2.8/setup.py` & `adafruit-circuitpython-pcd8544-1.2.9/setup.py`

 * *Files identical despite different names*

