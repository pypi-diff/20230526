# Comparing `tmp/adafruit-circuitpython-pm25-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-pm25-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pm25-2.1.8.tar", last modified: Tue Jun  7 17:04:44 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-pm25-2.1.9.tar", last modified: Thu Jun  9 18:15:09 2022, max compression
```

## Comparing `adafruit-circuitpython-pm25-2.1.8.tar` & `adafruit-circuitpython-pm25-2.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.631082 adafruit-circuitpython-pm25-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.623082 adafruit-circuitpython-pm25-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/adafruit_circuitpython_pm25.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-06-07 17:04:44.000000 adafruit-circuitpython-pm25-2.1.8/adafruit_circuitpython_pm25.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      925 2022-06-07 17:04:44.000000 adafruit-circuitpython-pm25-2.1.8/adafruit_circuitpython_pm25.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 17:04:44.000000 adafruit-circuitpython-pm25-2.1.8/adafruit_circuitpython_pm25.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-07 17:04:44.000000 adafruit-circuitpython-pm25-2.1.8/adafruit_circuitpython_pm25.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-07 17:04:44.000000 adafruit-circuitpython-pm25-2.1.8/adafruit_circuitpython_pm25.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/adafruit_pm25/
--rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/adafruit_pm25/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/adafruit_pm25/i2c.py
--rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/adafruit_pm25/uart.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      359 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5517 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1182 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 17:04:44.627082 adafruit-circuitpython-pm25-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/examples/pm25_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 17:04:44.631082 adafruit-circuitpython-pm25-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-06-07 17:04:33.000000 adafruit-circuitpython-pm25-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.274062 adafruit-circuitpython-pm25-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.270062 adafruit-circuitpython-pm25-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.270062 adafruit-circuitpython-pm25-2.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.270062 adafruit-circuitpython-pm25-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1254 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.270062 adafruit-circuitpython-pm25-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-06-09 18:15:09.274062 adafruit-circuitpython-pm25-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2678 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.274062 adafruit-circuitpython-pm25-2.1.9/adafruit_circuitpython_pm25.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3400 2022-06-09 18:15:09.000000 adafruit-circuitpython-pm25-2.1.9/adafruit_circuitpython_pm25.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      925 2022-06-09 18:15:09.000000 adafruit-circuitpython-pm25-2.1.9/adafruit_circuitpython_pm25.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 18:15:09.000000 adafruit-circuitpython-pm25-2.1.9/adafruit_circuitpython_pm25.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-06-09 18:15:09.000000 adafruit-circuitpython-pm25-2.1.9/adafruit_circuitpython_pm25.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-06-09 18:15:09.000000 adafruit-circuitpython-pm25-2.1.9/adafruit_circuitpython_pm25.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.274062 adafruit-circuitpython-pm25-2.1.9/adafruit_pm25/
+-rw-r--r--   0 runner    (1001) docker     (121)     3397 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/adafruit_pm25/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3289 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/adafruit_pm25/i2c.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2920 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/adafruit_pm25/uart.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.274062 adafruit-circuitpython-pm25-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.274062 adafruit-circuitpython-pm25-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      359 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5517 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1260 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 18:15:09.274062 adafruit-circuitpython-pm25-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2585 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/examples/pm25_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      161 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 18:15:09.274062 adafruit-circuitpython-pm25-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1929 2022-06-09 18:14:50.000000 adafruit-circuitpython-pm25-2.1.9/setup.py
```

### Comparing `adafruit-circuitpython-pm25-2.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-pm25-2.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-pm25-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-pm25-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/.gitignore` & `adafruit-circuitpython-pm25-2.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pm25-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/.pylintrc` & `adafruit-circuitpython-pm25-2.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pm25-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/LICENSE` & `adafruit-circuitpython-pm25-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pm25-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pm25-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pm25-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/PKG-INFO` & `adafruit-circuitpython-pm25-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pm25
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for PM2.5 Air Quality Sensors
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PM25
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython pm25 AQI PM2.5 Air Quality
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-pm25-2.1.8/README.rst` & `adafruit-circuitpython-pm25-2.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/adafruit_circuitpython_pm25.egg-info/PKG-INFO` & `adafruit-circuitpython-pm25-2.1.9/adafruit_circuitpython_pm25.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pm25
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for PM2.5 Air Quality Sensors
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PM25
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython pm25 AQI PM2.5 Air Quality
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-pm25-2.1.8/adafruit_circuitpython_pm25.egg-info/SOURCES.txt` & `adafruit-circuitpython-pm25-2.1.9/adafruit_circuitpython_pm25.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/adafruit_pm25/__init__.py` & `adafruit-circuitpython-pm25-2.1.9/adafruit_pm25/__init__.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/adafruit_pm25/i2c.py` & `adafruit-circuitpython-pm25-2.1.9/adafruit_pm25/i2c.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/adafruit_pm25/uart.py` & `adafruit-circuitpython-pm25-2.1.9/adafruit_pm25/uart.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pm25-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/docs/conf.py` & `adafruit-circuitpython-pm25-2.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/docs/index.rst` & `adafruit-circuitpython-pm25-2.1.9/docs/index.rst`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,16 @@
     Adafruit PMSA003I Air Quality Breakout <https://www.adafruit.com/product/4632>
 
     PM2.5 Air Quality Sensor and Breadboard Adapter Kit - PMS5003 <https://www.adafruit.com/product/3686>
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_PM25/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_PM25/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-pm25-2.1.8/examples/pm25_simpletest.py` & `adafruit-circuitpython-pm25-2.1.9/examples/pm25_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pm25-2.1.8/setup.py` & `adafruit-circuitpython-pm25-2.1.9/setup.py`

 * *Files identical despite different names*

