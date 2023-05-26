# Comparing `tmp/adafruit-circuitpython-esp32s2tft-1.1.7.tar.gz` & `tmp/adafruit-circuitpython-esp32s2tft-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-esp32s2tft-1.1.7.tar", last modified: Tue May 16 17:53:19 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-esp32s2tft-1.1.8.tar", last modified: Fri May 26 16:09:58 2023, max compression
```

## Comparing `adafruit-circuitpython-esp32s2tft-1.1.7.tar` & `adafruit-circuitpython-esp32s2tft-1.1.8.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.078368 adafruit-circuitpython-esp32s2tft-1.1.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.074368 adafruit-circuitpython-esp32s2tft-1.1.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.074368 adafruit-circuitpython-esp32s2tft-1.1.7/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.074368 adafruit-circuitpython-esp32s2tft-1.1.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.074368 adafruit-circuitpython-esp32s2tft-1.1.7/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-16 17:53:19.078368 adafruit-circuitpython-esp32s2tft-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.078368 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_circuitpython_esp32s2tft.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-16 17:53:19.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_circuitpython_esp32s2tft.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-16 17:53:19.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_circuitpython_esp32s2tft.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:53:19.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_circuitpython_esp32s2tft.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-16 17:53:19.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_circuitpython_esp32s2tft.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-16 17:53:19.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_circuitpython_esp32s2tft.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.078368 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4708 2023-05-16 17:53:11.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1856 2023-05-16 17:53:11.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-16 17:53:11.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2468 2023-05-16 17:53:11.000000 adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/peripherals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.078368 adafruit-circuitpython-esp32s2tft-1.1.7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.078368 adafruit-circuitpython-esp32s2tft-1.1.7/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6014 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:19.078368 adafruit-circuitpython-esp32s2tft-1.1.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-16 17:53:11.000000 adafruit-circuitpython-esp32s2tft-1.1.7/examples/esp32s2tft_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-16 17:53:11.000000 adafruit-circuitpython-esp32s2tft-1.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 17:52:58.000000 adafruit-circuitpython-esp32s2tft-1.1.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:53:19.078368 adafruit-circuitpython-esp32s2tft-1.1.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.633569 adafruit-circuitpython-esp32s2tft-1.1.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3633 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_circuitpython_esp32s2tft.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4407 2023-05-26 16:09:58.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_circuitpython_esp32s2tft.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-26 16:09:58.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_circuitpython_esp32s2tft.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:09:58.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_circuitpython_esp32s2tft.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 16:09:58.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_circuitpython_esp32s2tft.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:09:58.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_circuitpython_esp32s2tft.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4708 2023-05-26 16:09:51.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1856 2023-05-26 16:09:51.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-05-26 16:09:51.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2468 2023-05-26 16:09:51.000000 adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/peripherals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6042 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-05-26 16:09:51.000000 adafruit-circuitpython-esp32s2tft-1.1.8/examples/esp32s2tft_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-26 16:09:51.000000 adafruit-circuitpython-esp32s2tft-1.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 16:09:41.000000 adafruit-circuitpython-esp32s2tft-1.1.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:09:58.637569 adafruit-circuitpython-esp32s2tft-1.1.8/setup.cfg
```

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-esp32s2tft-1.1.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/.gitignore` & `adafruit-circuitpython-esp32s2tft-1.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/.pre-commit-config.yaml` & `adafruit-circuitpython-esp32s2tft-1.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/.pylintrc` & `adafruit-circuitpython-esp32s2tft-1.1.8/.pylintrc`

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

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-esp32s2tft-1.1.8/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/LICENSE` & `adafruit-circuitpython-esp32s2tft-1.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-esp32s2tft-1.1.8/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/LICENSES/MIT.txt` & `adafruit-circuitpython-esp32s2tft-1.1.8/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/LICENSES/Unlicense.txt` & `adafruit-circuitpython-esp32s2tft-1.1.8/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/PKG-INFO` & `adafruit-circuitpython-esp32s2tft-1.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32s2tft
-Version: 1.1.7
+Version: 1.1.8
 Summary: Helper library for the Adafruit ESP32-S2 TFT Feather
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32S2TFT
 Keywords: adafruit,esp32,esp32s2,tft,espressif,feather,hardwaremicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/README.rst` & `adafruit-circuitpython-esp32s2tft-1.1.8/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_circuitpython_esp32s2tft.egg-info/PKG-INFO` & `adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_circuitpython_esp32s2tft.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-esp32s2tft
-Version: 1.1.7
+Version: 1.1.8
 Summary: Helper library for the Adafruit ESP32-S2 TFT Feather
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_ESP32S2TFT
 Keywords: adafruit,esp32,esp32s2,tft,espressif,feather,hardwaremicropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_circuitpython_esp32s2tft.egg-info/SOURCES.txt` & `adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_circuitpython_esp32s2tft.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/__init__.py` & `adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 
 try:
     from typing import Optional, Dict, Union, Callable, Sequence, List
     from neopixel import NeoPixel
 except ImportError:
     pass
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32S2TFT.git"
 
 
 class ESP32S2TFT(PortalBase):
     """Class representing the Adafruit ESP32-S2 TFT Feather.
 
     :param url: The URL of your data source. Defaults to ``None``.
```

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/graphics.py` & `adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/graphics.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 * Adafruit's PortalBase library: https://github.com/adafruit/Adafruit_CircuitPython_PortalBase
 
 """
 
 import board
 from adafruit_portalbase.graphics import GraphicsBase
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32S2TFT.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the ESP32S2TFT Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/network.py` & `adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     from typing import Optional, Union, Callable
     from neopixel import NeoPixel
     from adafruit_io.adafruit_io import IO_MQTT
     import adafruit_minimqtt.adafruit_minimqtt as MQTT
 except ImportError:
     pass
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32S2TFT.git"
 
 IO_MQTT_BROKER = "io.adafruit.com"
 
 
 class Network(NetworkBase):
     """Network Helper Class for the ESP32S2TFT Library
```

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/adafruit_esp32s2tft/peripherals.py` & `adafruit-circuitpython-esp32s2tft-1.1.8/adafruit_esp32s2tft/peripherals.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 """
 
 import board
 from digitalio import DigitalInOut, Direction, Pull
 import neopixel
 
 
-__version__ = "1.1.7"
+__version__ = "1.1.8"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32S2TFT.git"
 
 
 class Peripherals:
     """Peripherals Helper Class for the ESP32S2TFT Library
```

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/docs/_static/favicon.ico` & `adafruit-circuitpython-esp32s2tft-1.1.8/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/docs/conf.py` & `adafruit-circuitpython-esp32s2tft-1.1.8/docs/conf.py`

 * *Files 0% similar despite different names*

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

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/docs/index.rst` & `adafruit-circuitpython-esp32s2tft-1.1.8/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/examples/esp32s2tft_simpletest.py` & `adafruit-circuitpython-esp32s2tft-1.1.8/examples/esp32s2tft_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-esp32s2tft-1.1.7/pyproject.toml` & `adafruit-circuitpython-esp32s2tft-1.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-esp32s2tft"
 description = "Helper library for the Adafruit ESP32-S2 TFT Feather"
-version = "1.1.7"
+version = "1.1.8"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_ESP32S2TFT"}
 keywords = [
     "adafruit",
```

