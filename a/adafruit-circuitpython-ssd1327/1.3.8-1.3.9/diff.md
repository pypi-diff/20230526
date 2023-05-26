# Comparing `tmp/adafruit-circuitpython-ssd1327-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-ssd1327-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1327-1.3.8.tar", last modified: Fri Aug 26 02:30:17 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1327-1.3.9.tar", last modified: Sat Aug 27 01:02:41 2022, max compression
```

## Comparing `adafruit-circuitpython-ssd1327-1.3.8.tar` & `adafruit-circuitpython-ssd1327-1.3.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.953855 adafruit-circuitpython-ssd1327-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3780 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3015 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/adafruit_circuitpython_ssd1327.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3780 2022-08-26 02:30:17.000000 adafruit-circuitpython-ssd1327-1.3.8/adafruit_circuitpython_ssd1327.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-26 02:30:17.000000 adafruit-circuitpython-ssd1327-1.3.8/adafruit_circuitpython_ssd1327.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:30:17.000000 adafruit-circuitpython-ssd1327-1.3.8/adafruit_circuitpython_ssd1327.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:30:17.000000 adafruit-circuitpython-ssd1327-1.3.8/adafruit_circuitpython_ssd1327.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 02:30:17.000000 adafruit-circuitpython-ssd1327-1.3.8/adafruit_circuitpython_ssd1327.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2288 2022-08-26 02:30:10.000000 adafruit-circuitpython-ssd1327-1.3.8/adafruit_ssd1327.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      366 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-08-26 02:30:10.000000 adafruit-circuitpython-ssd1327-1.3.8/examples/ssd1327_gamma.py
--rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-08-26 02:30:10.000000 adafruit-circuitpython-ssd1327-1.3.8/examples/ssd1327_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-08-26 02:30:10.000000 adafruit-circuitpython-ssd1327-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:30:03.000000 adafruit-circuitpython-ssd1327-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:30:17.957855 adafruit-circuitpython-ssd1327-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.747452 adafruit-circuitpython-ssd1327-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.743452 adafruit-circuitpython-ssd1327-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.743452 adafruit-circuitpython-ssd1327-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.743452 adafruit-circuitpython-ssd1327-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.743452 adafruit-circuitpython-ssd1327-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3780 2022-08-27 01:02:41.747452 adafruit-circuitpython-ssd1327-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3015 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.747452 adafruit-circuitpython-ssd1327-1.3.9/adafruit_circuitpython_ssd1327.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3780 2022-08-27 01:02:41.000000 adafruit-circuitpython-ssd1327-1.3.9/adafruit_circuitpython_ssd1327.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-27 01:02:41.000000 adafruit-circuitpython-ssd1327-1.3.9/adafruit_circuitpython_ssd1327.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-27 01:02:41.000000 adafruit-circuitpython-ssd1327-1.3.9/adafruit_circuitpython_ssd1327.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-27 01:02:41.000000 adafruit-circuitpython-ssd1327-1.3.9/adafruit_circuitpython_ssd1327.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-27 01:02:41.000000 adafruit-circuitpython-ssd1327-1.3.9/adafruit_circuitpython_ssd1327.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2617 2022-08-27 01:02:33.000000 adafruit-circuitpython-ssd1327-1.3.9/adafruit_ssd1327.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.747452 adafruit-circuitpython-ssd1327-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.747452 adafruit-circuitpython-ssd1327-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5645 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      366 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1075 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-27 01:02:41.747452 adafruit-circuitpython-ssd1327-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1217 2022-08-27 01:02:33.000000 adafruit-circuitpython-ssd1327-1.3.9/examples/ssd1327_gamma.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1821 2022-08-27 01:02:33.000000 adafruit-circuitpython-ssd1327-1.3.9/examples/ssd1327_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1226 2022-08-27 01:02:33.000000 adafruit-circuitpython-ssd1327-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-27 01:02:23.000000 adafruit-circuitpython-ssd1327-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-27 01:02:41.747452 adafruit-circuitpython-ssd1327-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1327-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-ssd1327-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-ssd1327-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/.gitignore` & `adafruit-circuitpython-ssd1327-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1327-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/.pylintrc` & `adafruit-circuitpython-ssd1327-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1327-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/LICENSE` & `adafruit-circuitpython-ssd1327-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1327-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1327-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1327-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/PKG-INFO` & `adafruit-circuitpython-ssd1327-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1327
-Version: 1.3.8
+Version: 1.3.9
 Summary: DisplayIO driver for grayscale OLEDs drive by SSD1327
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1327
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1327,oled,grayscale,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/README.rst` & `adafruit-circuitpython-ssd1327-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/adafruit_circuitpython_ssd1327.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1327-1.3.9/adafruit_circuitpython_ssd1327.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1327
-Version: 1.3.8
+Version: 1.3.9
 Summary: DisplayIO driver for grayscale OLEDs drive by SSD1327
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1327
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1327,oled,grayscale,displayio
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/adafruit_circuitpython_ssd1327.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1327-1.3.9/adafruit_circuitpython_ssd1327.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/adafruit_ssd1327.py` & `adafruit-circuitpython-ssd1327-1.3.9/adafruit_ssd1327.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1327.git"
 
 _INIT_SEQUENCE = (
     b"\xAE\x00"  # DISPLAY_OFF
     b"\x81\x01\x80"  # set contrast control
     b"\xa0\x01\x53"  # remap memory, odd even columns, com flip and column swap
     b"\xa1\x01\x00"  # Display start line is 0
@@ -47,19 +47,27 @@
     b"\xbe\x01\x0f"  # Set vcom voltage
     b"\xbc\x01\x08"  # Set pre-charge voltage
     b"\xd5\x01\x62"  # function selection B
     b"\xfd\x01\x12"  # command unlock
     b"\xAF\x00"  # DISPLAY_ON
 )
 
+
 # pylint: disable=too-few-public-methods
 class SSD1327(displayio.Display):
-    """SSD1327 driver"""
+    """SSD1327 driver
+
+    :param ~displayio.I2CDisplay bus: The data bus the display is on
+    :param int height: (keyword-only) The height of the screen
+    :param int width: (keyword-only) The width of the screen
+    :param int rotation: (keyword-only) The rotation/orientation of the
+        screen, in degrees
+    """
 
-    def __init__(self, bus, **kwargs):
+    def __init__(self, bus: displayio.I2CDisplay, **kwargs) -> None:
         # Patch the init sequence for 32 pixel high displays.
         init_sequence = bytearray(_INIT_SEQUENCE)
         height = kwargs["height"]
         if "rotation" in kwargs and kwargs["rotation"] % 180 != 0:
             height = kwargs["width"]
         init_sequence[18] = height - 1  # patch mux ratio
         super().__init__(
```

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1327-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/docs/conf.py` & `adafruit-circuitpython-ssd1327-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/docs/index.rst` & `adafruit-circuitpython-ssd1327-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/examples/ssd1327_gamma.py` & `adafruit-circuitpython-ssd1327-1.3.9/examples/ssd1327_gamma.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/examples/ssd1327_simpletest.py` & `adafruit-circuitpython-ssd1327-1.3.9/examples/ssd1327_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1327-1.3.8/pyproject.toml` & `adafruit-circuitpython-ssd1327-1.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ssd1327"
 description = "DisplayIO driver for grayscale OLEDs drive by SSD1327"
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1327"}
 keywords = [
     "adafruit",
```

