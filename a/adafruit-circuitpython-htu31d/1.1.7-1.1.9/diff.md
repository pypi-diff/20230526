# Comparing `tmp/adafruit-circuitpython-htu31d-1.1.7.tar.gz` & `tmp/adafruit-circuitpython-htu31d-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-htu31d-1.1.7.tar", last modified: Mon Aug 22 18:40:15 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-htu31d-1.1.9.tar", last modified: Wed Sep 28 00:34:30 2022, max compression
```

## Comparing `adafruit-circuitpython-htu31d-1.1.7.tar` & `adafruit-circuitpython-htu31d-1.1.9.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.716177 adafruit-circuitpython-htu31d-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.708177 adafruit-circuitpython-htu31d-1.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.712177 adafruit-circuitpython-htu31d-1.1.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.712177 adafruit-circuitpython-htu31d-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.712177 adafruit-circuitpython-htu31d-1.1.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-08-22 18:40:15.716177 adafruit-circuitpython-htu31d-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.712177 adafruit-circuitpython-htu31d-1.1.7/adafruit_circuitpython_htu31d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-08-22 18:40:15.000000 adafruit-circuitpython-htu31d-1.1.7/adafruit_circuitpython_htu31d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      958 2022-08-22 18:40:15.000000 adafruit-circuitpython-htu31d-1.1.7/adafruit_circuitpython_htu31d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:40:15.000000 adafruit-circuitpython-htu31d-1.1.7/adafruit_circuitpython_htu31d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 18:40:15.000000 adafruit-circuitpython-htu31d-1.1.7/adafruit_circuitpython_htu31d.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 18:40:15.000000 adafruit-circuitpython-htu31d-1.1.7/adafruit_circuitpython_htu31d.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7769 2022-08-22 18:40:05.000000 adafruit-circuitpython-htu31d-1.1.7/adafruit_htu31d.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.716177 adafruit-circuitpython-htu31d-1.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.716177 adafruit-circuitpython-htu31d-1.1.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5636 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      443 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:40:15.716177 adafruit-circuitpython-htu31d-1.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      745 2022-08-22 18:40:05.000000 adafruit-circuitpython-htu31d-1.1.7/examples/htu31d_setting_resolutions.py
--rw-r--r--   0 runner    (1001) docker     (121)      616 2022-08-22 18:40:05.000000 adafruit-circuitpython-htu31d-1.1.7/examples/htu31d_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-08-22 18:40:05.000000 adafruit-circuitpython-htu31d-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-22 18:39:52.000000 adafruit-circuitpython-htu31d-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:40:15.716177 adafruit-circuitpython-htu31d-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.976750 adafruit-circuitpython-htu31d-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.972750 adafruit-circuitpython-htu31d-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.972750 adafruit-circuitpython-htu31d-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.972750 adafruit-circuitpython-htu31d-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1087 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.972750 adafruit-circuitpython-htu31d-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-09-28 00:34:30.976750 adafruit-circuitpython-htu31d-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3107 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.972750 adafruit-circuitpython-htu31d-1.1.9/adafruit_circuitpython_htu31d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3883 2022-09-28 00:34:30.000000 adafruit-circuitpython-htu31d-1.1.9/adafruit_circuitpython_htu31d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      958 2022-09-28 00:34:30.000000 adafruit-circuitpython-htu31d-1.1.9/adafruit_circuitpython_htu31d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-28 00:34:30.000000 adafruit-circuitpython-htu31d-1.1.9/adafruit_circuitpython_htu31d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       84 2022-09-28 00:34:30.000000 adafruit-circuitpython-htu31d-1.1.9/adafruit_circuitpython_htu31d.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-09-28 00:34:30.000000 adafruit-circuitpython-htu31d-1.1.9/adafruit_circuitpython_htu31d.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8229 2022-09-28 00:34:21.000000 adafruit-circuitpython-htu31d-1.1.9/adafruit_htu31d.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.976750 adafruit-circuitpython-htu31d-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.976750 adafruit-circuitpython-htu31d-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      443 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1076 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-28 00:34:30.976750 adafruit-circuitpython-htu31d-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      745 2022-09-28 00:34:21.000000 adafruit-circuitpython-htu31d-1.1.9/examples/htu31d_setting_resolutions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      616 2022-09-28 00:34:21.000000 adafruit-circuitpython-htu31d-1.1.9/examples/htu31d_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1243 2022-09-28 00:34:21.000000 adafruit-circuitpython-htu31d-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-09-28 00:34:12.000000 adafruit-circuitpython-htu31d-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-28 00:34:30.976750 adafruit-circuitpython-htu31d-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-htu31d-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-htu31d-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/.github/workflows/build.yml` & `adafruit-circuitpython-htu31d-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/.github/workflows/release.yml` & `adafruit-circuitpython-htu31d-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/.gitignore` & `adafruit-circuitpython-htu31d-1.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/.pre-commit-config.yaml` & `adafruit-circuitpython-htu31d-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/.pylintrc` & `adafruit-circuitpython-htu31d-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-htu31d-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/LICENSE` & `adafruit-circuitpython-htu31d-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-htu31d-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/LICENSES/MIT.txt` & `adafruit-circuitpython-htu31d-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-htu31d-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/PKG-INFO` & `adafruit-circuitpython-htu31d-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-htu31d
-Version: 1.1.7
+Version: 1.1.9
 Summary: Python library for TE HTU31D temperature and humidity sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTU31D
 Keywords: adafruit,blinka,circuitpython,micropython,htu31d,temperature,humidity,sensor,te
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-htu31d-1.1.7/README.rst` & `adafruit-circuitpython-htu31d-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/adafruit_circuitpython_htu31d.egg-info/PKG-INFO` & `adafruit-circuitpython-htu31d-1.1.9/adafruit_circuitpython_htu31d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-htu31d
-Version: 1.1.7
+Version: 1.1.9
 Summary: Python library for TE HTU31D temperature and humidity sensors
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_HTU31D
 Keywords: adafruit,blinka,circuitpython,micropython,htu31d,temperature,humidity,sensor,te
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-htu31d-1.1.7/adafruit_circuitpython_htu31d.egg-info/SOURCES.txt` & `adafruit-circuitpython-htu31d-1.1.9/adafruit_circuitpython_htu31d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/adafruit_htu31d.py` & `adafruit-circuitpython-htu31d-1.1.9/adafruit_htu31d.py`

 * *Files 11% similar despite different names*

```diff
@@ -31,15 +31,22 @@
 """
 
 import time
 import struct
 from adafruit_bus_device import i2c_device
 from micropython import const
 
-__version__ = "1.1.7"
+try:
+    from typing import Tuple
+    from typing_extensions import Literal
+    from busio import I2C
+except ImportError:
+    pass
+
+__version__ = "1.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_HTU31D.git"
 
 _HTU31D_DEFAULT_ADDR = const(0x40)  # HTU31D default I2C Address
 _HTU31D_SECONDARY_ADDR = const(0x41)  # HTU31D alternate I2C Address
 _HTU31D_ADDRESSES = (_HTU31D_DEFAULT_ADDR, _HTU31D_SECONDARY_ADDR)
 
 _HTU31D_READSERIAL = const(0x0A)  # Read Out of Serial Register
@@ -85,71 +92,71 @@
 
             temperature = htu.temperature
             relative_humidity = htu.relative_humidity
 
 
     """
 
-    def __init__(self, i2c_bus, address=_HTU31D_DEFAULT_ADDR):
+    def __init__(self, i2c_bus: I2C, address: int = _HTU31D_DEFAULT_ADDR) -> None:
         if address not in _HTU31D_ADDRESSES:
-            raise ValueError("Invalid address: 0x%x" % (address))
+            raise ValueError(f"Invalid address: {address:#x}")
         self.i2c_device = i2c_device.I2CDevice(i2c_bus, address)
         self._conversion_command = _HTU31D_CONVERSION
         self._buffer = bytearray(6)
         self.reset()
 
     @property
-    def serial_number(self):
+    def serial_number(self) -> int:
         """The unique 32-bit serial number"""
         self._buffer[0] = _HTU31D_READSERIAL
         with self.i2c_device as i2c:
             i2c.write_then_readinto(self._buffer, self._buffer, out_end=1, in_end=4)
         ser = struct.unpack(">I", self._buffer[0:4])
-        return ser
+        return ser[0]
 
-    def reset(self):
+    def reset(self) -> None:
         """Perform a soft reset of the sensor, resetting all settings to their power-on defaults"""
         self._conversion_command = _HTU31D_CONVERSION
         self._buffer[0] = _HTU31D_SOFTRESET
         with self.i2c_device as i2c:
             i2c.write(self._buffer, end=1)
         time.sleep(0.015)
 
     @property
-    def heater(self):
+    def heater(self) -> bool:
         """The current sensor heater mode"""
         return self._heater
 
     @heater.setter
-    def heater(self, new_mode):
-        # check its a boolean
-        if not new_mode in (True, False):
+    def heater(self, new_mode: bool) -> None:
+        # check it is a boolean
+        if not isinstance(new_mode, bool):
             raise AttributeError("Heater mode must be boolean")
         # cache the mode
         self._heater = new_mode
         # decide the command!
         if new_mode:
             self._buffer[0] = _HTU31D_HEATERON
         else:
             self._buffer[0] = _HTU31D_HEATEROFF
         with self.i2c_device as i2c:
             i2c.write(self._buffer, end=1)
 
     @property
-    def relative_humidity(self):
+    def relative_humidity(self) -> float:
         """The current relative humidity in % rH"""
         return self.measurements[1]
 
     @property
-    def temperature(self):
+    def temperature(self) -> float:
         """The current temperature in degrees Celsius"""
         return self.measurements[0]
 
     @property
-    def measurements(self):
+    def measurements(self) -> Tuple[float, float]:
         """both `temperature` and `relative_humidity`, read simultaneously"""
 
         temperature = None
         humidity = None
 
         self._buffer[0] = self._conversion_command
         with self.i2c_device as i2c:
@@ -179,65 +186,69 @@
         # repeat above steps for humidity data
         humidity = 100 * humidity / 65535.0
         humidity = max(min(humidity, 100), 0)
 
         return (temperature, humidity)
 
     @property
-    def humidity_resolution(self):
+    def humidity_resolution(self) -> Literal["0.020%", "0.014%", "0.010%", "0.007%"]:
         """The current relative humidity resolution in % rH.
 
         Possibles values:
 
             * "0.020%"
             * "0.014%"
             * "0.010%"
             * "0.007%"
 
         """
 
         return _HTU31D_HUMIDITY_RES[self._conversion_command >> 4 & 3]
 
     @humidity_resolution.setter
-    def humidity_resolution(self, value):
+    def humidity_resolution(
+        self, value: Literal["0.020%", "0.014%", "0.010%", "0.007%"]
+    ) -> None:
         if value not in _HTU31D_HUMIDITY_RES:
             raise ValueError(
-                "Humidity resolution must be one of: {}".format(_HTU31D_HUMIDITY_RES)
+                f"Humidity resolution must be one of: {_HTU31D_HUMIDITY_RES}"
             )
         register = self._conversion_command & 0xCF
         hum_res = _HTU31D_HUMIDITY_RES.index(value)
         self._conversion_command = register | hum_res << 4
 
     @property
-    def temp_resolution(self):
+    def temp_resolution(self) -> Literal["0.040", "0.025", "0.016", "0.012"]:
         """The current temperature resolution in Celsius.
 
         Possibles values:
 
             * "0.040"
             * "0.025"
             * "0.016"
             * "0.012"
 
         """
 
         return _HTU31D_TEMP_RES[self._conversion_command >> 2 & 3]
 
     @temp_resolution.setter
-    def temp_resolution(self, value):
+    def temp_resolution(
+        self, value: Literal["0.040", "0.025", "0.016", "0.012"]
+    ) -> None:
         if value not in _HTU31D_TEMP_RES:
             raise ValueError(
-                "Temperature resolution must be one of: {}".format(_HTU31D_TEMP_RES)
+                f"Temperature resolution must be one of: {_HTU31D_TEMP_RES}"
             )
         register = self._conversion_command & 0xF3
         temp_res = _HTU31D_TEMP_RES.index(value)
         self._conversion_command = register | temp_res << 2
 
     @staticmethod
-    def _crc(value):
+    def _crc(value) -> int:
         polynom = 0x988000  # x^8 + x^5 + x^4 + 1
         msb = 0x800000
         mask = 0xFF8000
         result = value << 8  # Pad with zeros as specified in spec
 
         while msb != 0x80:
             # Check if msb of current value is 1 and apply XOR mask
```

### Comparing `adafruit-circuitpython-htu31d-1.1.7/docs/_static/favicon.ico` & `adafruit-circuitpython-htu31d-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/docs/conf.py` & `adafruit-circuitpython-htu31d-1.1.9/docs/conf.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2017 Scott Shawcroft, written for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -46,15 +47,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit HTU31D Library"
-copyright = "2021 ladyada"
+creation_year = "2021"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " ladyada"
 author = "ladyada"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-htu31d-1.1.7/docs/index.rst` & `adafruit-circuitpython-htu31d-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/examples/htu31d_setting_resolutions.py` & `adafruit-circuitpython-htu31d-1.1.9/examples/htu31d_setting_resolutions.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/examples/htu31d_simpletest.py` & `adafruit-circuitpython-htu31d-1.1.9/examples/htu31d_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-htu31d-1.1.7/pyproject.toml` & `adafruit-circuitpython-htu31d-1.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-htu31d"
 description = "Python library for TE HTU31D temperature and humidity sensors"
-version = "1.1.7"
+version = "1.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_HTU31D"}
 keywords = [
     "adafruit",
```

