# Comparing `tmp/adafruit-circuitpython-vl53l1x-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-vl53l1x-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-vl53l1x-1.1.8.tar", last modified: Mon Nov 28 18:05:05 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-vl53l1x-1.1.9.tar", last modified: Thu Dec 15 19:58:10 2022, max compression
```

## Comparing `adafruit-circuitpython-vl53l1x-1.1.8.tar` & `adafruit-circuitpython-vl53l1x-1.1.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.058743 adafruit-circuitpython-vl53l1x-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.050742 adafruit-circuitpython-vl53l1x-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.054743 adafruit-circuitpython-vl53l1x-1.1.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (122)      880 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.054743 adafruit-circuitpython-vl53l1x-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (122)      479 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (122)      423 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (122)      475 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (122)     1648 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (122)     1239 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (122)    13069 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (122)      388 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (122)     6753 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (122)     1104 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.054743 adafruit-circuitpython-vl53l1x-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (122)    16814 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1108 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1211 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (122)     4179 2022-11-28 18:05:05.054743 adafruit-circuitpython-vl53l1x-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     3405 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      188 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.054743 adafruit-circuitpython-vl53l1x-1.1.8/adafruit_circuitpython_vl53l1x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     4179 2022-11-28 18:05:05.000000 adafruit-circuitpython-vl53l1x-1.1.8/adafruit_circuitpython_vl53l1x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1013 2022-11-28 18:05:05.000000 adafruit-circuitpython-vl53l1x-1.1.8/adafruit_circuitpython_vl53l1x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-28 18:05:05.000000 adafruit-circuitpython-vl53l1x-1.1.8/adafruit_circuitpython_vl53l1x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       61 2022-11-28 18:05:05.000000 adafruit-circuitpython-vl53l1x-1.1.8/adafruit_circuitpython_vl53l1x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       17 2022-11-28 18:05:05.000000 adafruit-circuitpython-vl53l1x-1.1.8/adafruit_circuitpython_vl53l1x.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    13632 2022-11-28 18:04:57.000000 adafruit-circuitpython-vl53l1x-1.1.8/adafruit_vl53l1x.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.054743 adafruit-circuitpython-vl53l1x-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.054743 adafruit-circuitpython-vl53l1x-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (122)      105 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (122)      267 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     6014 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      414 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)     1066 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (122)      189 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (122)      123 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-28 18:05:05.054743 adafruit-circuitpython-vl53l1x-1.1.8/examples/
--rwxr-xr-x   0 runner    (1001) docker     (122)     2704 2022-11-28 18:04:57.000000 adafruit-circuitpython-vl53l1x-1.1.8/examples/vl53l1x_set_address_multiple_sensors.py
--rw-r--r--   0 runner    (1001) docker     (122)     1285 2022-11-28 18:04:57.000000 adafruit-circuitpython-vl53l1x-1.1.8/examples/vl53l1x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (122)      108 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1228 2022-11-28 18:04:57.000000 adafruit-circuitpython-vl53l1x-1.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)      158 2022-11-28 18:04:51.000000 adafruit-circuitpython-vl53l1x-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-28 18:05:05.058743 adafruit-circuitpython-vl53l1x-1.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.614844 adafruit-circuitpython-vl53l1x-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.606844 adafruit-circuitpython-vl53l1x-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.610844 adafruit-circuitpython-vl53l1x-1.1.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.610844 adafruit-circuitpython-vl53l1x-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13069 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.610844 adafruit-circuitpython-vl53l1x-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2022-12-15 19:58:10.614844 adafruit-circuitpython-vl53l1x-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.610844 adafruit-circuitpython-vl53l1x-1.1.9/adafruit_circuitpython_vl53l1x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2022-12-15 19:58:10.000000 adafruit-circuitpython-vl53l1x-1.1.9/adafruit_circuitpython_vl53l1x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2022-12-15 19:58:10.000000 adafruit-circuitpython-vl53l1x-1.1.9/adafruit_circuitpython_vl53l1x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-15 19:58:10.000000 adafruit-circuitpython-vl53l1x-1.1.9/adafruit_circuitpython_vl53l1x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2022-12-15 19:58:10.000000 adafruit-circuitpython-vl53l1x-1.1.9/adafruit_circuitpython_vl53l1x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2022-12-15 19:58:10.000000 adafruit-circuitpython-vl53l1x-1.1.9/adafruit_circuitpython_vl53l1x.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13685 2022-12-15 19:57:59.000000 adafruit-circuitpython-vl53l1x-1.1.9/adafruit_vl53l1x.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.614844 adafruit-circuitpython-vl53l1x-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.614844 adafruit-circuitpython-vl53l1x-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6014 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-15 19:58:10.614844 adafruit-circuitpython-vl53l1x-1.1.9/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2704 2022-12-15 19:57:59.000000 adafruit-circuitpython-vl53l1x-1.1.9/examples/vl53l1x_set_address_multiple_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2022-12-15 19:57:59.000000 adafruit-circuitpython-vl53l1x-1.1.9/examples/vl53l1x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1228 2022-12-15 19:57:59.000000 adafruit-circuitpython-vl53l1x-1.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2022-12-15 19:57:46.000000 adafruit-circuitpython-vl53l1x-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-15 19:58:10.614844 adafruit-circuitpython-vl53l1x-1.1.9/setup.cfg
```

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-vl53l1x-1.1.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/.gitignore` & `adafruit-circuitpython-vl53l1x-1.1.9/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 _build
 
 # This file results from running `pip -e install .` in a local repository
 *.egg-info
 
 # Virtual environment-specific files
 .env
+.venv
 
 # MacOS-specific files
 *.DS_Store
 
 # IDE-specific files
 .idea
 .vscode
```

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-vl53l1x-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/.pylintrc` & `adafruit-circuitpython-vl53l1x-1.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-vl53l1x-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/LICENSE` & `adafruit-circuitpython-vl53l1x-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-vl53l1x-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-vl53l1x-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-vl53l1x-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/PKG-INFO` & `adafruit-circuitpython-vl53l1x-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vl53l1x
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython module for interacting with the VL53L1X distance sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_VL53L1X.git
 Keywords: adafruit,blinka,circuitpython,micropython,vl53l1x,distance,ToF
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/README.rst` & `adafruit-circuitpython-vl53l1x-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/adafruit_circuitpython_vl53l1x.egg-info/PKG-INFO` & `adafruit-circuitpython-vl53l1x-1.1.9/adafruit_circuitpython_vl53l1x.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vl53l1x
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython module for interacting with the VL53L1X distance sensor.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_VL53L1X.git
 Keywords: adafruit,blinka,circuitpython,micropython,vl53l1x,distance,ToF
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/adafruit_circuitpython_vl53l1x.egg-info/SOURCES.txt` & `adafruit-circuitpython-vl53l1x-1.1.9/adafruit_circuitpython_vl53l1x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/adafruit_vl53l1x.py` & `adafruit-circuitpython-vl53l1x-1.1.9/adafruit_vl53l1x.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 """
 
 import time
 import struct
 from adafruit_bus_device import i2c_device
 from micropython import const
 
-# imports__version__ = "1.1.8"
+# imports__version__ = "1.1.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_VL53L1X.git"
 
 _VL53L1X_I2C_SLAVE_DEVICE_ADDRESS = const(0x0001)
 _VL53L1X_VHV_CONFIG__TIMEOUT_MACROP_LOOP_BOUND = const(0x0008)
 _GPIO_HV_MUX__CTRL = const(0x0030)
 _GPIO__TIO_HV_STATUS = const(0x0031)
 _PHASECAL_CONFIG__TIMEOUT_MACROP = const(0x004B)
@@ -233,15 +233,16 @@
         return False
 
     @property
     def timing_budget(self):
         """Ranging duration in milliseconds. Increasing the timing budget
         increases the maximum distance the device can range and improves
         the repeatability error. However, average power consumption augments
-        accordingly. ms = 15 (short mode only), 20, 33, 50, 100, 200, 500."""
+        accordingly. ms = 15 (short mode only), 20, 33, 50, 100, 200, 500.
+        Defaults to 50."""
         return self._timing_budget
 
     @timing_budget.setter
     def timing_budget(self, val):
         reg_vals = None
         mode = self.distance_mode
         if mode == 1:
@@ -260,15 +261,15 @@
     def _interrupt_polarity(self):
         int_pol = self._read_register(_GPIO_HV_MUX__CTRL)[0] & 0x10
         int_pol = (int_pol >> 4) & 0x01
         return 0 if int_pol else 1
 
     @property
     def distance_mode(self):
-        """The distance mode. 1=short, 2=long."""
+        """The distance mode. 1=short (up to 136cm) , 2=long (up to 360cm)."""
         mode = self._read_register(_PHASECAL_CONFIG__TIMEOUT_MACROP)[0]
         if mode == 0x14:
             return 1  # short distance
         if mode == 0x0A:
             return 2  # long distance
         return None  # unknown
```

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-vl53l1x-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/docs/conf.py` & `adafruit-circuitpython-vl53l1x-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/docs/index.rst` & `adafruit-circuitpython-vl53l1x-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/examples/vl53l1x_set_address_multiple_sensors.py` & `adafruit-circuitpython-vl53l1x-1.1.9/examples/vl53l1x_set_address_multiple_sensors.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/examples/vl53l1x_simpletest.py` & `adafruit-circuitpython-vl53l1x-1.1.9/examples/vl53l1x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vl53l1x-1.1.8/pyproject.toml` & `adafruit-circuitpython-vl53l1x-1.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-vl53l1x"
 description = "CircuitPython module for interacting with the VL53L1X distance sensor."
-version = "1.1.8"
+version = "1.1.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_VL53L1X.git"}
 keywords = [
     "adafruit",
```

