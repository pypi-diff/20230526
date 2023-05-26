# Comparing `tmp/adafruit-circuitpython-tc74-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-tc74-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tc74-1.0.8.tar", last modified: Tue Jun  7 16:54:26 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tc74-1.0.9.tar", last modified: Thu Jun  9 18:00:10 2022, max compression
```

## Comparing `adafruit-circuitpython-tc74-1.0.8.tar` & `adafruit-circuitpython-tc74-1.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.075656 adafruit-circuitpython-tc74-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.075656 adafruit-circuitpython-tc74-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6199 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/adafruit_circuitpython_tc74.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-06-07 16:54:25.000000 adafruit-circuitpython-tc74-1.0.8/adafruit_circuitpython_tc74.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      873 2022-06-07 16:54:26.000000 adafruit-circuitpython-tc74-1.0.8/adafruit_circuitpython_tc74.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 16:54:25.000000 adafruit-circuitpython-tc74-1.0.8/adafruit_circuitpython_tc74.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-07 16:54:25.000000 adafruit-circuitpython-tc74-1.0.8/adafruit_circuitpython_tc74.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-07 16:54:25.000000 adafruit-circuitpython-tc74-1.0.8/adafruit_circuitpython_tc74.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/adafruit_tc74.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      263 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      950 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (121)      268 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/examples/tc74_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 16:54:26.079656 adafruit-circuitpython-tc74-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-06-07 16:54:11.000000 adafruit-circuitpython-tc74-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.850387 adafruit-circuitpython-tc74-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.842387 adafruit-circuitpython-tc74-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.846387 adafruit-circuitpython-tc74-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.846387 adafruit-circuitpython-tc74-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6199 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.846387 adafruit-circuitpython-tc74-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-06-09 18:00:10.846387 adafruit-circuitpython-tc74-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2686 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.846387 adafruit-circuitpython-tc74-1.0.9/adafruit_circuitpython_tc74.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3518 2022-06-09 18:00:10.000000 adafruit-circuitpython-tc74-1.0.9/adafruit_circuitpython_tc74.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      873 2022-06-09 18:00:10.000000 adafruit-circuitpython-tc74-1.0.9/adafruit_circuitpython_tc74.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:00:10.000000 adafruit-circuitpython-tc74-1.0.9/adafruit_circuitpython_tc74.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-06-09 18:00:10.000000 adafruit-circuitpython-tc74-1.0.9/adafruit_circuitpython_tc74.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-09 18:00:10.000000 adafruit-circuitpython-tc74-1.0.9/adafruit_circuitpython_tc74.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3278 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/adafruit_tc74.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.846387 adafruit-circuitpython-tc74-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.846387 adafruit-circuitpython-tc74-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      263 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5627 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1028 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:00:10.846387 adafruit-circuitpython-tc74-1.0.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      268 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/examples/tc74_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:00:10.850387 adafruit-circuitpython-tc74-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2082 2022-06-09 17:59:55.000000 adafruit-circuitpython-tc74-1.0.9/setup.py
```

### Comparing `adafruit-circuitpython-tc74-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tc74-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-tc74-1.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-tc74-1.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/.gitignore` & `adafruit-circuitpython-tc74-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tc74-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/.pylintrc` & `adafruit-circuitpython-tc74-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tc74-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/LICENSE` & `adafruit-circuitpython-tc74-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tc74-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tc74-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tc74-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/PKG-INFO` & `adafruit-circuitpython-tc74-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tc74
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython library for the Microchip TC74 Digital Temperature Sensor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TC74
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython tc74 temperature
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-tc74-1.0.8/README.rst` & `adafruit-circuitpython-tc74-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/adafruit_circuitpython_tc74.egg-info/PKG-INFO` & `adafruit-circuitpython-tc74-1.0.9/adafruit_circuitpython_tc74.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tc74
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython library for the Microchip TC74 Digital Temperature Sensor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TC74
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython tc74 temperature
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-tc74-1.0.8/adafruit_circuitpython_tc74.egg-info/SOURCES.txt` & `adafruit-circuitpython-tc74-1.0.9/adafruit_circuitpython_tc74.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/adafruit_tc74.py` & `adafruit-circuitpython-tc74-1.0.9/adafruit_tc74.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tc74-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/docs/conf.py` & `adafruit-circuitpython-tc74-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tc74-1.0.8/docs/index.rst` & `adafruit-circuitpython-tc74-1.0.9/docs/index.rst`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     :caption: Related Products
 
     Adafruit TC74 <https://www.adafruit.com/product/4375>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_TC74/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_TC74/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-tc74-1.0.8/setup.py` & `adafruit-circuitpython-tc74-1.0.9/setup.py`

 * *Files identical despite different names*

