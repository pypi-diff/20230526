# Comparing `tmp/adafruit-circuitpython-waveform-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-waveform-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-waveform-1.3.8.tar", last modified: Mon Nov 15 19:11:11 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-waveform-1.3.9.tar", last modified: Tue Jan 11 19:02:43 2022, max compression
```

## Comparing `adafruit-circuitpython-waveform-1.3.8.tar` & `adafruit-circuitpython-waveform-1.3.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.707959 adafruit-circuitpython-waveform-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.703959 adafruit-circuitpython-waveform-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.703959 adafruit-circuitpython-waveform-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      886 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.703959 adafruit-circuitpython-waveform-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2422 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.703959 adafruit-circuitpython-waveform-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2021-11-15 19:11:11.707959 adafruit-circuitpython-waveform-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2565 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.707959 adafruit-circuitpython-waveform-1.3.8/adafruit_circuitpython_waveform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3434 2021-11-15 19:11:11.000000 adafruit-circuitpython-waveform-1.3.8/adafruit_circuitpython_waveform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      954 2021-11-15 19:11:11.000000 adafruit-circuitpython-waveform-1.3.8/adafruit_circuitpython_waveform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-15 19:11:11.000000 adafruit-circuitpython-waveform-1.3.8/adafruit_circuitpython_waveform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2021-11-15 19:11:11.000000 adafruit-circuitpython-waveform-1.3.8/adafruit_circuitpython_waveform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.707959 adafruit-circuitpython-waveform-1.3.8/adafruit_waveform/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/adafruit_waveform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      790 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/adafruit_waveform/sine.py
--rw-r--r--   0 runner    (1001) docker     (121)      686 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/adafruit_waveform/square.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.707959 adafruit-circuitpython-waveform-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.707959 adafruit-circuitpython-waveform-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      187 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5119 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      334 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      901 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-15 19:11:11.707959 adafruit-circuitpython-waveform-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      515 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/examples/waveform_sine_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      521 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/examples/waveform_square_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      102 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-15 19:11:11.707959 adafruit-circuitpython-waveform-1.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2021-11-15 19:10:59.000000 adafruit-circuitpython-waveform-1.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.737050 adafruit-circuitpython-waveform-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.733050 adafruit-circuitpython-waveform-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.733050 adafruit-circuitpython-waveform-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      886 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.733050 adafruit-circuitpython-waveform-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2422 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      353 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.733050 adafruit-circuitpython-waveform-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-01-11 19:02:43.737050 adafruit-circuitpython-waveform-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2565 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.733050 adafruit-circuitpython-waveform-1.3.9/adafruit_circuitpython_waveform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3434 2022-01-11 19:02:43.000000 adafruit-circuitpython-waveform-1.3.9/adafruit_circuitpython_waveform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      954 2022-01-11 19:02:43.000000 adafruit-circuitpython-waveform-1.3.9/adafruit_circuitpython_waveform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-11 19:02:43.000000 adafruit-circuitpython-waveform-1.3.9/adafruit_circuitpython_waveform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-01-11 19:02:43.000000 adafruit-circuitpython-waveform-1.3.9/adafruit_circuitpython_waveform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.733050 adafruit-circuitpython-waveform-1.3.9/adafruit_waveform/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/adafruit_waveform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      790 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/adafruit_waveform/sine.py
+-rw-r--r--   0 runner    (1001) docker     (121)      686 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/adafruit_waveform/square.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.737050 adafruit-circuitpython-waveform-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.737050 adafruit-circuitpython-waveform-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      187 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5119 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      901 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-11 19:02:43.737050 adafruit-circuitpython-waveform-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      515 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/examples/waveform_sine_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      521 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/examples/waveform_square_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      102 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-11 19:02:43.737050 adafruit-circuitpython-waveform-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-01-11 19:02:34.000000 adafruit-circuitpython-waveform-1.3.9/setup.py
```

### Comparing `adafruit-circuitpython-waveform-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-waveform-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-waveform-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-waveform-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-waveform-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/.pylintrc` & `adafruit-circuitpython-waveform-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-waveform-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/LICENSE` & `adafruit-circuitpython-waveform-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-waveform-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-waveform-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-waveform-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/PKG-INFO` & `adafruit-circuitpython-waveform-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-waveform
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for generating simple waveforms for audio.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Waveform
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit haptic waveform signal audio rtttl sine squarewave hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-waveform-1.3.8/README.rst` & `adafruit-circuitpython-waveform-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/adafruit_circuitpython_waveform.egg-info/PKG-INFO` & `adafruit-circuitpython-waveform-1.3.9/adafruit_circuitpython_waveform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-waveform
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for generating simple waveforms for audio.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_Waveform
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit haptic waveform signal audio rtttl sine squarewave hardware micropython circuitpython
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-waveform-1.3.8/adafruit_circuitpython_waveform.egg-info/SOURCES.txt` & `adafruit-circuitpython-waveform-1.3.9/adafruit_circuitpython_waveform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/adafruit_waveform/sine.py` & `adafruit-circuitpython-waveform-1.3.9/adafruit_waveform/sine.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/adafruit_waveform/square.py` & `adafruit-circuitpython-waveform-1.3.9/adafruit_waveform/square.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-waveform-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/docs/conf.py` & `adafruit-circuitpython-waveform-1.3.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/docs/index.rst` & `adafruit-circuitpython-waveform-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/examples/waveform_sine_simpletest.py` & `adafruit-circuitpython-waveform-1.3.9/examples/waveform_sine_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/examples/waveform_square_simpletest.py` & `adafruit-circuitpython-waveform-1.3.9/examples/waveform_square_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-waveform-1.3.8/setup.py` & `adafruit-circuitpython-waveform-1.3.9/setup.py`

 * *Files identical despite different names*

