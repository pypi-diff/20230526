# Comparing `tmp/adafruit-circuitpython-displayio-sh1107-1.5.8.tar.gz` & `tmp/adafruit-circuitpython-displayio-sh1107-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-displayio-sh1107-1.5.8.tar", last modified: Fri Aug 26 02:11:26 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-displayio-sh1107-1.5.9.tar", last modified: Sun Sep  4 02:33:01 2022, max compression
```

## Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8.tar` & `adafruit-circuitpython-displayio-sh1107-1.5.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.743916 adafruit-circuitpython-displayio-sh1107-1.5.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.731916 adafruit-circuitpython-displayio-sh1107-1.5.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.735916 adafruit-circuitpython-displayio-sh1107-1.5.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.735916 adafruit-circuitpython-displayio-sh1107-1.5.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16247 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.739916 adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-08-26 02:11:26.743916 adafruit-circuitpython-displayio-sh1107-1.5.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3925 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.739916 adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_circuitpython_displayio_sh1107.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-08-26 02:11:26.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_circuitpython_displayio_sh1107.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-08-26 02:11:26.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_circuitpython_displayio_sh1107.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:11:26.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_circuitpython_displayio_sh1107.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-26 02:11:26.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_circuitpython_displayio_sh1107.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-26 02:11:26.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_circuitpython_displayio_sh1107.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     7773 2022-08-26 02:11:18.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_displayio_sh1107.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.739916 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.743916 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5848 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:11:26.743916 adafruit-circuitpython-displayio-sh1107-1.5.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     4197 2022-08-26 02:11:18.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/examples/displayio_sh1107_game_of_life.py
--rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-08-26 02:11:18.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/examples/displayio_sh1107_mono_128x128_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     2659 2022-08-26 02:11:18.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/examples/displayio_sh1107_random_motion.py
--rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-08-26 02:11:18.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/examples/displayio_sh1107_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-08-26 02:11:18.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:11:10.000000 adafruit-circuitpython-displayio-sh1107-1.5.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:11:26.743916 adafruit-circuitpython-displayio-sh1107-1.5.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.766032 adafruit-circuitpython-displayio-sh1107-1.5.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.758032 adafruit-circuitpython-displayio-sh1107-1.5.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.762032 adafruit-circuitpython-displayio-sh1107-1.5.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.762032 adafruit-circuitpython-displayio-sh1107-1.5.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16247 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1103 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.762032 adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-09-04 02:33:01.766032 adafruit-circuitpython-displayio-sh1107-1.5.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3925 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.762032 adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_circuitpython_displayio_sh1107.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-09-04 02:33:01.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_circuitpython_displayio_sh1107.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1121 2022-09-04 02:33:01.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_circuitpython_displayio_sh1107.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-04 02:33:01.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_circuitpython_displayio_sh1107.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-04 02:33:01.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_circuitpython_displayio_sh1107.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-04 02:33:01.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_circuitpython_displayio_sh1107.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     7932 2022-09-04 02:32:51.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_displayio_sh1107.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.762032 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.762032 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5848 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-04 02:33:01.766032 adafruit-circuitpython-displayio-sh1107-1.5.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     4197 2022-09-04 02:32:51.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/examples/displayio_sh1107_game_of_life.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2833 2022-09-04 02:32:51.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/examples/displayio_sh1107_mono_128x128_test.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2659 2022-09-04 02:32:51.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/examples/displayio_sh1107_random_motion.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2299 2022-09-04 02:32:51.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/examples/displayio_sh1107_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1235 2022-09-04 02:32:51.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-04 02:32:38.000000 adafruit-circuitpython-displayio-sh1107-1.5.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-04 02:33:01.766032 adafruit-circuitpython-displayio-sh1107-1.5.9/setup.cfg
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-displayio-sh1107-1.5.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/.github/workflows/build.yml` & `adafruit-circuitpython-displayio-sh1107-1.5.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/.github/workflows/release.yml` & `adafruit-circuitpython-displayio-sh1107-1.5.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/.gitignore` & `adafruit-circuitpython-displayio-sh1107-1.5.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/.pre-commit-config.yaml` & `adafruit-circuitpython-displayio-sh1107-1.5.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/.pylintrc` & `adafruit-circuitpython-displayio-sh1107-1.5.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-displayio-sh1107-1.5.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSE` & `adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSES/MIT.txt` & `adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-displayio-sh1107-1.5.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/PKG-INFO` & `adafruit-circuitpython-displayio-sh1107-1.5.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-sh1107
-Version: 1.5.8
+Version: 1.5.9
 Summary: Support for the SH1107 OLED display driver IC
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1107
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_sh1107,display,oled
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/README.rst` & `adafruit-circuitpython-displayio-sh1107-1.5.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_circuitpython_displayio_sh1107.egg-info/PKG-INFO` & `adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_circuitpython_displayio_sh1107.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-sh1107
-Version: 1.5.8
+Version: 1.5.9
 Summary: Support for the SH1107 OLED display driver IC
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1107
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_sh1107,display,oled
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_circuitpython_displayio_sh1107.egg-info/SOURCES.txt` & `adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_circuitpython_displayio_sh1107.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/adafruit_displayio_sh1107.py` & `adafruit-circuitpython-displayio-sh1107-1.5.9/adafruit_displayio_sh1107.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,15 +26,20 @@
 
 """
 
 import sys
 import displayio
 from micropython import const
 
-__version__ = "1.5.8"
+try:
+    from typing import Union
+except ImportError:
+    pass
+
+__version__ = "1.5.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1107.git"
 
 
 DISPLAY_OFFSET_ADAFRUIT_FEATHERWING_OLED_4650 = const(0x60)
 """
 The hardware display offset to use when configuring the SH1107 for the
 `Adafruit Featherwing 128x64 OLED <https://www.adafruit.com/product/4650>`_.
@@ -137,19 +142,19 @@
         This will be dependent on the OLED display and two displays with the
         same dimensions could have different offsets. This defaults to
         `DISPLAY_OFFSET_ADAFRUIT_FEATHERWING_OLED_4650`
     """
 
     def __init__(
         self,
-        bus,
-        display_offset=DISPLAY_OFFSET_ADAFRUIT_FEATHERWING_OLED_4650,
-        rotation=0,
+        bus: Union[displayio.I2CDisplay, displayio.FourWire],
+        display_offset: int = DISPLAY_OFFSET_ADAFRUIT_FEATHERWING_OLED_4650,
+        rotation: int = 0,
         **kwargs
-    ):
+    ) -> None:
         rotation = (rotation + _ROTATION_OFFSET) % 360
         if rotation in (0, 180):
             multiplex = kwargs["width"] - 1
         else:
             multiplex = kwargs["height"] - 1
         init_sequence = bytearray(_INIT_SEQUENCE)
         init_sequence[16] = multiplex
@@ -170,39 +175,39 @@
             #                upper column command = 0x10 - 0x17
             #                set page address     = 0xB0 - 0xBF (16 pages)
             SH1107_addressing=True,
         )
         self._is_awake = True  # Display starts in active state (_INIT_SEQUENCE)
 
     @property
-    def is_awake(self):
+    def is_awake(self) -> bool:
         """
         The power state of the display. (read-only)
 
         `True` if the display is active, `False` if in sleep mode.
 
         :type: bool
         """
         return self._is_awake
 
-    def sleep(self):
+    def sleep(self) -> None:
         """
         Put display into sleep mode. The display uses < 5uA in sleep mode
 
         Sleep mode does the following:
 
             1) Stops the oscillator and DC-DC circuits
             2) Stops the OLED drive
             3) Remembers display data and operation mode active prior to sleeping
             4) The MP can access (update) the built-in display RAM
         """
         if self._is_awake:
             self.bus.send(0xAE, b"")  # 0xAE = display off, sleep mode
             self._is_awake = False
 
-    def wake(self):
+    def wake(self) -> None:
         """
         Wake display from sleep mode
         """
         if not self._is_awake:
             self.bus.send(0xAF, b"")  # 0xAF = display on
             self._is_awake = True
```

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/docs/_static/favicon.ico` & `adafruit-circuitpython-displayio-sh1107-1.5.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/docs/conf.py` & `adafruit-circuitpython-displayio-sh1107-1.5.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/docs/index.rst` & `adafruit-circuitpython-displayio-sh1107-1.5.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/examples/displayio_sh1107_game_of_life.py` & `adafruit-circuitpython-displayio-sh1107-1.5.9/examples/displayio_sh1107_game_of_life.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/examples/displayio_sh1107_mono_128x128_test.py` & `adafruit-circuitpython-displayio-sh1107-1.5.9/examples/displayio_sh1107_mono_128x128_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/examples/displayio_sh1107_random_motion.py` & `adafruit-circuitpython-displayio-sh1107-1.5.9/examples/displayio_sh1107_random_motion.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/examples/displayio_sh1107_simpletest.py` & `adafruit-circuitpython-displayio-sh1107-1.5.9/examples/displayio_sh1107_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1107-1.5.8/pyproject.toml` & `adafruit-circuitpython-displayio-sh1107-1.5.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-displayio-sh1107"
 description = "Support for the SH1107 OLED display driver IC"
-version = "1.5.8"
+version = "1.5.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1107"}
 keywords = [
     "adafruit",
```

