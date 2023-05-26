# Comparing `tmp/adafruit-circuitpython-oauth2-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-oauth2-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-oauth2-1.0.8.tar", last modified: Tue Jun  7 16:52:16 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-oauth2-1.0.9.tar", last modified: Thu Jun  9 17:59:29 2022, max compression
```

## Comparing `adafruit-circuitpython-oauth2-1.0.8.tar` & `adafruit-circuitpython-oauth2-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.377522 adafruit-circuitpython-oauth2-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3273 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2531 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/adafruit_circuitpython_oauth2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3273 2022-06-07 16:52:16.000000 adafruit-circuitpython-oauth2-1.0.8/adafruit_circuitpython_oauth2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      979 2022-06-07 16:52:16.000000 adafruit-circuitpython-oauth2-1.0.8/adafruit_circuitpython_oauth2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-07 16:52:16.000000 adafruit-circuitpython-oauth2-1.0.8/adafruit_circuitpython_oauth2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-07 16:52:16.000000 adafruit-circuitpython-oauth2-1.0.8/adafruit_circuitpython_oauth2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-07 16:52:16.000000 adafruit-circuitpython-oauth2-1.0.8/adafruit_circuitpython_oauth2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7294 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/adafruit_oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      895 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/examples/oauth2_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/examples/oauth2_simpletest_cpython.py
--rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/examples/oauth2_simpletest_esp32spi.py
--rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-07 16:52:16.381521 adafruit-circuitpython-oauth2-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-06-07 16:52:03.000000 adafruit-circuitpython-oauth2-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.071949 adafruit-circuitpython-oauth2-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.063948 adafruit-circuitpython-oauth2-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.063948 adafruit-circuitpython-oauth2-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.067949 adafruit-circuitpython-oauth2-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16265 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.067949 adafruit-circuitpython-oauth2-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3273 2022-06-09 17:59:29.067949 adafruit-circuitpython-oauth2-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2531 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.067949 adafruit-circuitpython-oauth2-1.0.9/adafruit_circuitpython_oauth2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3273 2022-06-09 17:59:28.000000 adafruit-circuitpython-oauth2-1.0.9/adafruit_circuitpython_oauth2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2022-06-09 17:59:29.000000 adafruit-circuitpython-oauth2-1.0.9/adafruit_circuitpython_oauth2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-09 17:59:28.000000 adafruit-circuitpython-oauth2-1.0.9/adafruit_circuitpython_oauth2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       48 2022-06-09 17:59:28.000000 adafruit-circuitpython-oauth2-1.0.9/adafruit_circuitpython_oauth2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-06-09 17:59:28.000000 adafruit-circuitpython-oauth2-1.0.9/adafruit_circuitpython_oauth2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7294 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/adafruit_oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.067949 adafruit-circuitpython-oauth2-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.067949 adafruit-circuitpython-oauth2-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5534 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      973 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-09 17:59:29.067949 adafruit-circuitpython-oauth2-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     2557 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/examples/oauth2_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2327 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/examples/oauth2_simpletest_cpython.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3083 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/examples/oauth2_simpletest_esp32spi.py
+-rw-r--r--   0 runner    (1001) docker     (121)      130 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-06-09 17:59:29.071949 adafruit-circuitpython-oauth2-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2051 2022-06-09 17:59:15.000000 adafruit-circuitpython-oauth2-1.0.9/setup.py
```

### Comparing `adafruit-circuitpython-oauth2-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-oauth2-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-oauth2-1.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-oauth2-1.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/.gitignore` & `adafruit-circuitpython-oauth2-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-oauth2-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/.pylintrc` & `adafruit-circuitpython-oauth2-1.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-oauth2-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/LICENSE` & `adafruit-circuitpython-oauth2-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-oauth2-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-oauth2-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-oauth2-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/PKG-INFO` & `adafruit-circuitpython-oauth2-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-oauth2
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython helper for OAuth2.0 authorization to access Google APIs.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_OAuth2
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython oauth2 oauth api google
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-oauth2-1.0.8/README.rst` & `adafruit-circuitpython-oauth2-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/adafruit_circuitpython_oauth2.egg-info/PKG-INFO` & `adafruit-circuitpython-oauth2-1.0.9/adafruit_circuitpython_oauth2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-oauth2
-Version: 1.0.8
+Version: 1.0.9
 Summary: CircuitPython helper for OAuth2.0 authorization to access Google APIs.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_OAuth2
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit blinka circuitpython micropython oauth2 oauth api google
 Platform: UNKNOWN
```

### Comparing `adafruit-circuitpython-oauth2-1.0.8/adafruit_circuitpython_oauth2.egg-info/SOURCES.txt` & `adafruit-circuitpython-oauth2-1.0.9/adafruit_circuitpython_oauth2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/adafruit_oauth2.py` & `adafruit-circuitpython-oauth2-1.0.9/adafruit_oauth2.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-oauth2-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/docs/conf.py` & `adafruit-circuitpython-oauth2-1.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/docs/index.rst` & `adafruit-circuitpython-oauth2-1.0.9/docs/index.rst`

 * *Files 11% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 .. toctree::
     :caption: Related Products
 
 
 .. toctree::
     :caption: Other Links
 
-    Download <https://github.com/adafruit/Adafruit_CircuitPython_OAuth2/releases/latest>
+    Download from GitHub <https://github.com/adafruit/Adafruit_CircuitPython_OAuth2/releases/latest>
+    Download Library Bundle <https://circuitpython.org/libraries>
     CircuitPython Reference Documentation <https://docs.circuitpython.org>
     CircuitPython Support Forum <https://forums.adafruit.com/viewforum.php?f=60>
     Discord Chat <https://adafru.it/discord>
     Adafruit Learning System <https://learn.adafruit.com>
     Adafruit Blog <https://blog.adafruit.com>
     Adafruit Store <https://www.adafruit.com>
```

### Comparing `adafruit-circuitpython-oauth2-1.0.8/examples/oauth2_simpletest.py` & `adafruit-circuitpython-oauth2-1.0.9/examples/oauth2_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/examples/oauth2_simpletest_cpython.py` & `adafruit-circuitpython-oauth2-1.0.9/examples/oauth2_simpletest_cpython.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/examples/oauth2_simpletest_esp32spi.py` & `adafruit-circuitpython-oauth2-1.0.9/examples/oauth2_simpletest_esp32spi.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-oauth2-1.0.8/setup.py` & `adafruit-circuitpython-oauth2-1.0.9/setup.py`

 * *Files identical despite different names*

