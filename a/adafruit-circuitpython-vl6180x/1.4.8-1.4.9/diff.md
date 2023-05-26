# Comparing `tmp/adafruit-circuitpython-vl6180x-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-vl6180x-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-vl6180x-1.4.8.tar", last modified: Mon Aug 22 18:55:28 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-vl6180x-1.4.9.tar", last modified: Fri Aug 26 02:27:32 2022, max compression
```

## Comparing `adafruit-circuitpython-vl6180x-1.4.8.tar` & `adafruit-circuitpython-vl6180x-1.4.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.012194 adafruit-circuitpython-vl6180x-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.004194 adafruit-circuitpython-vl6180x-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.008194 adafruit-circuitpython-vl6180x-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.008194 adafruit-circuitpython-vl6180x-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.008194 adafruit-circuitpython-vl6180x-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-08-22 18:55:28.008194 adafruit-circuitpython-vl6180x-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.008194 adafruit-circuitpython-vl6180x-1.4.8/adafruit_circuitpython_vl6180x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-08-22 18:55:27.000000 adafruit-circuitpython-vl6180x-1.4.8/adafruit_circuitpython_vl6180x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-08-22 18:55:28.000000 adafruit-circuitpython-vl6180x-1.4.8/adafruit_circuitpython_vl6180x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:55:27.000000 adafruit-circuitpython-vl6180x-1.4.8/adafruit_circuitpython_vl6180x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 18:55:27.000000 adafruit-circuitpython-vl6180x-1.4.8/adafruit_circuitpython_vl6180x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-22 18:55:27.000000 adafruit-circuitpython-vl6180x-1.4.8/adafruit_circuitpython_vl6180x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    14404 2022-08-22 18:55:19.000000 adafruit-circuitpython-vl6180x-1.4.8/adafruit_vl6180x.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.008194 adafruit-circuitpython-vl6180x-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.008194 adafruit-circuitpython-vl6180x-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5478 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:55:28.008194 adafruit-circuitpython-vl6180x-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-22 18:55:19.000000 adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_calibrationtest.py
--rw-r--r--   0 runner    (1001) docker     (121)      826 2022-08-22 18:55:19.000000 adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_continuoustest.py
--rw-r--r--   0 runner    (1001) docker     (121)      945 2022-08-22 18:55:19.000000 adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_historytest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-08-22 18:55:19.000000 adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_performancetest.py
--rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-08-22 18:55:19.000000 adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-08-22 18:55:19.000000 adafruit-circuitpython-vl6180x-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-22 18:55:11.000000 adafruit-circuitpython-vl6180x-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:55:28.012194 adafruit-circuitpython-vl6180x-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.321337 adafruit-circuitpython-vl6180x-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2657 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/adafruit_circuitpython_vl6180x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3447 2022-08-26 02:27:32.000000 adafruit-circuitpython-vl6180x-1.4.9/adafruit_circuitpython_vl6180x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2022-08-26 02:27:32.000000 adafruit-circuitpython-vl6180x-1.4.9/adafruit_circuitpython_vl6180x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:27:32.000000 adafruit-circuitpython-vl6180x-1.4.9/adafruit_circuitpython_vl6180x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 02:27:32.000000 adafruit-circuitpython-vl6180x-1.4.9/adafruit_circuitpython_vl6180x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-08-26 02:27:32.000000 adafruit-circuitpython-vl6180x-1.4.9/adafruit_circuitpython_vl6180x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    14404 2022-08-26 02:27:23.000000 adafruit-circuitpython-vl6180x-1.4.9/adafruit_vl6180x.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5698 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1198 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:27:32.325337 adafruit-circuitpython-vl6180x-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      952 2022-08-26 02:27:23.000000 adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_calibrationtest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      826 2022-08-26 02:27:23.000000 adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_continuoustest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      945 2022-08-26 02:27:23.000000 adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_historytest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2022-08-26 02:27:23.000000 adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_performancetest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1357 2022-08-26 02:27:23.000000 adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1258 2022-08-26 02:27:23.000000 adafruit-circuitpython-vl6180x-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-26 02:27:15.000000 adafruit-circuitpython-vl6180x-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:27:32.329337 adafruit-circuitpython-vl6180x-1.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-vl6180x-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/.github/workflows/build.yml` & `adafruit-circuitpython-vl6180x-1.4.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/.github/workflows/release.yml` & `adafruit-circuitpython-vl6180x-1.4.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/.gitignore` & `adafruit-circuitpython-vl6180x-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-vl6180x-1.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/.pylintrc` & `adafruit-circuitpython-vl6180x-1.4.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-vl6180x-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/LICENSE` & `adafruit-circuitpython-vl6180x-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-vl6180x-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-vl6180x-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-vl6180x-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/PKG-INFO` & `adafruit-circuitpython-vl6180x-1.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vl6180x
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython library for VL6180X time of flight distance sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_VL6180X
 Keywords: adafruit,vl6180x,time,flight,distance,sensorbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/README.rst` & `adafruit-circuitpython-vl6180x-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/adafruit_circuitpython_vl6180x.egg-info/PKG-INFO` & `adafruit-circuitpython-vl6180x-1.4.9/adafruit_circuitpython_vl6180x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vl6180x
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython library for VL6180X time of flight distance sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_VL6180X
 Keywords: adafruit,vl6180x,time,flight,distance,sensorbreakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/adafruit_circuitpython_vl6180x.egg-info/SOURCES.txt` & `adafruit-circuitpython-vl6180x-1.4.9/adafruit_circuitpython_vl6180x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/adafruit_vl6180x.py` & `adafruit-circuitpython-vl6180x-1.4.9/adafruit_vl6180x.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 try:
     from typing import Optional, List
     from busio import I2C
 except ImportError:
     pass
 
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_VL6180X.git"
 
 # Registers
 _VL6180X_REG_IDENTIFICATION_MODEL_ID = const(0x000)
 
 _VL6180X_REG_SYSTEM_HISTORY_CTRL = const(0x012)
 _VL6180X_REG_SYSTEM_INTERRUPT_CONFIG = const(0x014)
```

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-vl6180x-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/docs/conf.py` & `adafruit-circuitpython-vl6180x-1.4.9/docs/conf.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -40,15 +41,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit VL6180X Library"
-copyright = "2017 Tony DiCola"
+creation_year = "2017"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Tony DiCola"
 author = "Tony DiCola"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/docs/examples.rst` & `adafruit-circuitpython-vl6180x-1.4.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/docs/index.rst` & `adafruit-circuitpython-vl6180x-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_calibrationtest.py` & `adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_calibrationtest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_continuoustest.py` & `adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_continuoustest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_historytest.py` & `adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_historytest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_performancetest.py` & `adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_performancetest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/examples/vl6180x_simpletest.py` & `adafruit-circuitpython-vl6180x-1.4.9/examples/vl6180x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl6180x-1.4.8/pyproject.toml` & `adafruit-circuitpython-vl6180x-1.4.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-vl6180x"
 description = "CircuitPython library for VL6180X time of flight distance sensor."
-version = "1.4.8"
+version = "1.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_VL6180X"}
 keywords = [
     "adafruit",
```

