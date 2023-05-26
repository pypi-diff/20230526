# Comparing `tmp/adafruit-circuitpython-funhouse-2.1.19.tar.gz` & `tmp/adafruit-circuitpython-funhouse-2.1.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-funhouse-2.1.19.tar", last modified: Tue May 16 17:54:10 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-funhouse-2.1.20.tar", last modified: Fri May 26 16:17:09 2023, max compression
```

## Comparing `adafruit-circuitpython-funhouse-2.1.19.tar` & `adafruit-circuitpython-funhouse-2.1.20.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.731292 adafruit-circuitpython-funhouse-2.1.19/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.731292 adafruit-circuitpython-funhouse-2.1.19/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.731292 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.731292 adafruit-circuitpython-funhouse-2.1.19/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 17:54:10.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4450 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7268 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6960 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/peripherals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6025 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_adafruit_io_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_simpletest.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1506 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_temperature_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-16 17:54:03.000000 adafruit-circuitpython-funhouse-2.1.19/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-16 17:53:52.000000 adafruit-circuitpython-funhouse-2.1.19/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:54:10.735292 adafruit-circuitpython-funhouse-2.1.19/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.332653 adafruit-circuitpython-funhouse-2.1.20/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.324653 adafruit-circuitpython-funhouse-2.1.20/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.328653 adafruit-circuitpython-funhouse-2.1.20/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.328653 adafruit-circuitpython-funhouse-2.1.20/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.328653 adafruit-circuitpython-funhouse-2.1.20/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-26 16:17:09.332653 adafruit-circuitpython-funhouse-2.1.20/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.328653 adafruit-circuitpython-funhouse-2.1.20/adafruit_circuitpython_funhouse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6306 2023-05-26 16:17:09.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_circuitpython_funhouse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-26 16:17:09.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_circuitpython_funhouse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:17:09.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_circuitpython_funhouse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 16:17:09.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_circuitpython_funhouse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:17:09.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_circuitpython_funhouse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.328653 adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4450 2023-05-26 16:17:01.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1835 2023-05-26 16:17:01.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7268 2023-05-26 16:17:01.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6960 2023-05-26 16:17:01.000000 adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/peripherals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.332653 adafruit-circuitpython-funhouse-2.1.20/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.332653 adafruit-circuitpython-funhouse-2.1.20/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6053 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     2221 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:17:09.332653 adafruit-circuitpython-funhouse-2.1.20/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2508 2023-05-26 16:17:01.000000 adafruit-circuitpython-funhouse-2.1.20/examples/funhouse_adafruit_io_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-26 16:17:01.000000 adafruit-circuitpython-funhouse-2.1.20/examples/funhouse_simpletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1506 2023-05-26 16:17:01.000000 adafruit-circuitpython-funhouse-2.1.20/examples/funhouse_temperature_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-26 16:17:01.000000 adafruit-circuitpython-funhouse-2.1.20/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-26 16:16:48.000000 adafruit-circuitpython-funhouse-2.1.20/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:17:09.332653 adafruit-circuitpython-funhouse-2.1.20/setup.cfg
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-funhouse-2.1.20/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/.gitignore` & `adafruit-circuitpython-funhouse-2.1.20/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/.pre-commit-config.yaml` & `adafruit-circuitpython-funhouse-2.1.20/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/.pylintrc` & `adafruit-circuitpython-funhouse-2.1.20/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -392,8 +392,8 @@
 min-public-methods=1
 
 
 [EXCEPTIONS]
 
 # Exceptions that will emit a warning when being caught. Defaults to
 # "Exception"
-overgeneral-exceptions=Exception
+overgeneral-exceptions=builtins.Exception
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-funhouse-2.1.20/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/LICENSE` & `adafruit-circuitpython-funhouse-2.1.20/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-funhouse-2.1.20/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/LICENSES/MIT.txt` & `adafruit-circuitpython-funhouse-2.1.20/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/LICENSES/Unlicense.txt` & `adafruit-circuitpython-funhouse-2.1.20/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/PKG-INFO` & `adafruit-circuitpython-funhouse-2.1.20/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-funhouse
-Version: 2.1.19
+Version: 2.1.20
 Summary: Helper library for the FunHouse board
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FunHouse
 Keywords: adafruit,funhouse,microcontroller,sensors,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/README.rst` & `adafruit-circuitpython-funhouse-2.1.20/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/PKG-INFO` & `adafruit-circuitpython-funhouse-2.1.20/adafruit_circuitpython_funhouse.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-funhouse
-Version: 2.1.19
+Version: 2.1.20
 Summary: Helper library for the FunHouse board
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_FunHouse
 Keywords: adafruit,funhouse,microcontroller,sensors,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/adafruit_circuitpython_funhouse.egg-info/SOURCES.txt` & `adafruit-circuitpython-funhouse-2.1.20/adafruit_circuitpython_funhouse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/__init__.py` & `adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 try:
     from typing import Optional, Dict, Union, Callable, Sequence, List
     from adafruit_dotstar import DotStar
 except ImportError:
     pass
 
-__version__ = "2.1.19"
+__version__ = "2.1.20"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse.git"
 
 
 class FunHouse(PortalBase):
     """Class representing the Adafruit FunHouse.
 
     :param url: The URL of your data source. Defaults to ``None``.
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/graphics.py` & `adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 * Adafruit's PortalBase library: https://github.com/adafruit/Adafruit_CircuitPython_PortalBase
 
 """
 
 import board
 from adafruit_portalbase.graphics import GraphicsBase
 
-__version__ = "2.1.19"
+__version__ = "2.1.20"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the FunHouse Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/network.py` & `adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 try:
     from typing import Optional, Union, Callable
     from adafruit_dotstar import DotStar
 except ImportError:
     pass
 
-__version__ = "2.1.19"
+__version__ = "2.1.20"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse.git"
 
 IO_MQTT_BROKER = "io.adafruit.com"
 
 
 class Network(NetworkBase):
     """Class representing the Adafruit FunHouse.
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/adafruit_funhouse/peripherals.py` & `adafruit-circuitpython-funhouse-2.1.20/adafruit_funhouse/peripherals.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 import adafruit_dotstar
 
 try:
     from typing import Optional
 except ImportError:
     pass
 
-__version__ = "2.1.19"
+__version__ = "2.1.20"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse.git"
 
 
 class Peripherals:
     """Peripherals Helper Class for the FunHouse Library
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/docs/_static/favicon.ico` & `adafruit-circuitpython-funhouse-2.1.20/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/docs/conf.py` & `adafruit-circuitpython-funhouse-2.1.20/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
 # ones.
 extensions = [
     "sphinx.ext.autodoc",
+    "sphinxcontrib.jquery",
     "sphinx.ext.intersphinx",
     "sphinx.ext.napoleon",
     "sphinx.ext.todo",
 ]
 
 # TODO: Please Read!
 # Uncomment the below if you use native CircuitPython modules such as
```

### Comparing `adafruit-circuitpython-funhouse-2.1.19/docs/examples.rst` & `adafruit-circuitpython-funhouse-2.1.20/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/docs/index.rst` & `adafruit-circuitpython-funhouse-2.1.20/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_adafruit_io_mqtt.py` & `adafruit-circuitpython-funhouse-2.1.20/examples/funhouse_adafruit_io_mqtt.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_simpletest.py` & `adafruit-circuitpython-funhouse-2.1.20/examples/funhouse_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/examples/funhouse_temperature_logger.py` & `adafruit-circuitpython-funhouse-2.1.20/examples/funhouse_temperature_logger.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-funhouse-2.1.19/pyproject.toml` & `adafruit-circuitpython-funhouse-2.1.20/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-funhouse"
 description = "Helper library for the FunHouse board"
-version = "2.1.19"
+version = "2.1.20"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_FunHouse"}
 keywords = [
     "adafruit",
```

