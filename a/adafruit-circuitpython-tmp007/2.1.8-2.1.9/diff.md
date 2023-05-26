# Comparing `tmp/adafruit-circuitpython-tmp007-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-tmp007-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-tmp007-2.1.8.tar", last modified: Tue Jun  7 17:07:15 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-tmp007-2.1.9.tar", last modified: Thu Jun  9 18:19:38 2022, max compression
```

## Comparing `adafruit-circuitpython-tmp007-2.1.8.tar` & `adafruit-circuitpython-tmp007-2.1.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.606135 adafruit-circuitpython-tmp007-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.606135 adafruit-circuitpython-tmp007-2.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/adafruit_circuitpython_tmp007.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-06-07 17:07:15.000000 adafruit-circuitpython-tmp007-2.1.8/adafruit_circuitpython_tmp007.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-06-07 17:07:15.000000 adafruit-circuitpython-tmp007-2.1.8/adafruit_circuitpython_tmp007.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:07:15.000000 adafruit-circuitpython-tmp007-2.1.8/adafruit_circuitpython_tmp007.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-07 17:07:15.000000 adafruit-circuitpython-tmp007-2.1.8/adafruit_circuitpython_tmp007.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 17:07:15.000000 adafruit-circuitpython-tmp007-2.1.8/adafruit_circuitpython_tmp007.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/adafruit_tmp007.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5551 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      939 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/examples/tmp007_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:07:15.610135 adafruit-circuitpython-tmp007-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-06-07 17:07:05.000000 adafruit-circuitpython-tmp007-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.504078 adafruit-circuitpython-tmp007-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1080 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2391 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/adafruit_circuitpython_tmp007.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3147 2022-06-09 18:19:38.000000 adafruit-circuitpython-tmp007-2.1.9/adafruit_circuitpython_tmp007.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-06-09 18:19:38.000000 adafruit-circuitpython-tmp007-2.1.9/adafruit_circuitpython_tmp007.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:19:38.000000 adafruit-circuitpython-tmp007-2.1.9/adafruit_circuitpython_tmp007.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-09 18:19:38.000000 adafruit-circuitpython-tmp007-2.1.9/adafruit_circuitpython_tmp007.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-09 18:19:38.000000 adafruit-circuitpython-tmp007-2.1.9/adafruit_circuitpython_tmp007.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5920 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/adafruit_tmp007.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5551 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/examples/tmp007_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:19:38.508078 adafruit-circuitpython-tmp007-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1880 2022-06-09 18:19:23.000000 adafruit-circuitpython-tmp007-2.1.9/setup.py
```

### Comparing `adafruit-circuitpython-tmp007-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-tmp007-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-tmp007-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-tmp007-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/.gitignore` & `adafruit-circuitpython-tmp007-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-tmp007-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/.pylintrc` & `adafruit-circuitpython-tmp007-2.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-tmp007-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/LICENSE` & `adafruit-circuitpython-tmp007-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-tmp007-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-tmp007-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-tmp007-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/PKG-INFO` & `adafruit-circuitpython-tmp007-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tmp007
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for TMP007 contactless IR thermometer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TMP007
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit contactless ir thermometer temperature tmp007 hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-tmp007-2.1.8/README.rst` & `adafruit-circuitpython-tmp007-2.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/adafruit_circuitpython_tmp007.egg-info/PKG-INFO` & `adafruit-circuitpython-tmp007-2.1.9/adafruit_circuitpython_tmp007.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-tmp007
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for TMP007 contactless IR thermometer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_TMP007
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit contactless ir thermometer temperature tmp007 hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-tmp007-2.1.8/adafruit_circuitpython_tmp007.egg-info/SOURCES.txt` & `adafruit-circuitpython-tmp007-2.1.9/adafruit_circuitpython_tmp007.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/adafruit_tmp007.py` & `adafruit-circuitpython-tmp007-2.1.9/adafruit_tmp007.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-tmp007-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/docs/conf.py` & `adafruit-circuitpython-tmp007-2.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/docs/index.rst` & `adafruit-circuitpython-tmp007-2.1.9/docs/index.rst`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,16 @@
     :caption: Related Products
 
     <https://www.adafruit.com/product/2023>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_TMP007/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_TMP007/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-tmp007-2.1.8/examples/tmp007_simpletest.py` & `adafruit-circuitpython-tmp007-2.1.9/examples/tmp007_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-tmp007-2.1.8/setup.py` & `adafruit-circuitpython-tmp007-2.1.9/setup.py`

 * *Files identical despite different names*

