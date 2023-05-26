# Comparing `tmp/adafruit-circuitpython-typing-1.9.3.tar.gz` & `tmp/adafruit-circuitpython-typing-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-typing-1.9.3.tar", last modified: Thu May 18 15:43:02 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-typing-1.9.4.tar", last modified: Fri May 26 16:15:30 2023, max compression
```

## Comparing `adafruit-circuitpython-typing-1.9.3.tar` & `adafruit-circuitpython-typing-1.9.4.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.623424 adafruit-circuitpython-typing-1.9.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.615424 adafruit-circuitpython-typing-1.9.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.619424 adafruit-circuitpython-typing-1.9.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.619424 adafruit-circuitpython-typing-1.9.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.619424 adafruit-circuitpython-typing-1.9.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-18 15:43:02.623424 adafruit-circuitpython-typing-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.619424 adafruit-circuitpython-typing-1.9.3/adafruit_circuitpython_typing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-18 15:43:02.000000 adafruit-circuitpython-typing-1.9.3/adafruit_circuitpython_typing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-18 15:43:02.000000 adafruit-circuitpython-typing-1.9.3/adafruit_circuitpython_typing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:43:02.000000 adafruit-circuitpython-typing-1.9.3/adafruit_circuitpython_typing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-18 15:43:02.000000 adafruit-circuitpython-typing-1.9.3/adafruit_circuitpython_typing.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-18 15:43:02.000000 adafruit-circuitpython-typing-1.9.3/adafruit_circuitpython_typing.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.619424 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/
--rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/device_drivers.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/io.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/led.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/pil.py
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/pwmio.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/circuitpython_typing/socket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.623424 adafruit-circuitpython-typing-1.9.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.623424 adafruit-circuitpython-typing-1.9.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     6078 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:43:02.623424 adafruit-circuitpython-typing-1.9.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/examples/typing_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-18 15:42:54.000000 adafruit-circuitpython-typing-1.9.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-18 15:42:45.000000 adafruit-circuitpython-typing-1.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:43:02.623424 adafruit-circuitpython-typing-1.9.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.597676 adafruit-circuitpython-typing-1.9.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.597676 adafruit-circuitpython-typing-1.9.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.597676 adafruit-circuitpython-typing-1.9.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/adafruit_circuitpython_typing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-05-26 16:15:30.000000 adafruit-circuitpython-typing-1.9.4/adafruit_circuitpython_typing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-05-26 16:15:30.000000 adafruit-circuitpython-typing-1.9.4/adafruit_circuitpython_typing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:15:30.000000 adafruit-circuitpython-typing-1.9.4/adafruit_circuitpython_typing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 16:15:30.000000 adafruit-circuitpython-typing-1.9.4/adafruit_circuitpython_typing.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-26 16:15:30.000000 adafruit-circuitpython-typing-1.9.4/adafruit_circuitpython_typing.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/
+-rw-r--r--   0 runner    (1001) docker     (123)     5514 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/device_drivers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1124 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/led.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/pil.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/pwmio.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     4360 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/circuitpython_typing/socket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     6106 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/examples/typing_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-26 16:15:23.000000 adafruit-circuitpython-typing-1.9.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-26 16:15:13.000000 adafruit-circuitpython-typing-1.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:15:30.601676 adafruit-circuitpython-typing-1.9.4/setup.cfg
```

### Comparing `adafruit-circuitpython-typing-1.9.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-typing-1.9.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/.gitignore` & `adafruit-circuitpython-typing-1.9.4/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/.pre-commit-config.yaml` & `adafruit-circuitpython-typing-1.9.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/.pylintrc` & `adafruit-circuitpython-typing-1.9.4/.pylintrc`

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

### Comparing `adafruit-circuitpython-typing-1.9.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-typing-1.9.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/LICENSE` & `adafruit-circuitpython-typing-1.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-typing-1.9.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/LICENSES/MIT.txt` & `adafruit-circuitpython-typing-1.9.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-typing-1.9.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/PKG-INFO` & `adafruit-circuitpython-typing-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-typing
-Version: 1.9.3
+Version: 1.9.4
 Summary: Types needed for type annotation that are not in `typing`
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Typing
 Keywords: adafruit,blinka,circuitpython,micropython,circuitpython_typing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-typing-1.9.3/README.rst` & `adafruit-circuitpython-typing-1.9.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/adafruit_circuitpython_typing.egg-info/PKG-INFO` & `adafruit-circuitpython-typing-1.9.4/adafruit_circuitpython_typing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-typing
-Version: 1.9.3
+Version: 1.9.4
 Summary: Types needed for type annotation that are not in `typing`
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Typing
 Keywords: adafruit,blinka,circuitpython,micropython,circuitpython_typing
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-typing-1.9.3/adafruit_circuitpython_typing.egg-info/SOURCES.txt` & `adafruit-circuitpython-typing-1.9.4/adafruit_circuitpython_typing.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/circuitpython_typing/__init__.py` & `adafruit-circuitpython-typing-1.9.4/circuitpython_typing/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 Types needed for type annotation that are not in `typing`
 
 
 * Author(s): Alec Delaney, Dan Halbert, Randy Hudson
 """
 
-__version__ = "1.9.3"
+__version__ = "1.9.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_Typing.git"
 
 import array
 from typing import Union, Optional
 from typing_extensions import Protocol, TypeAlias  # Safety import for Python 3.7
 
 # Lists below are alphabetized.
```

### Comparing `adafruit-circuitpython-typing-1.9.3/circuitpython_typing/device_drivers.py` & `adafruit-circuitpython-typing-1.9.4/circuitpython_typing/device_drivers.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/circuitpython_typing/http.py` & `adafruit-circuitpython-typing-1.9.4/circuitpython_typing/http.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/circuitpython_typing/io.py` & `adafruit-circuitpython-typing-1.9.4/circuitpython_typing/io.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/circuitpython_typing/led.py` & `adafruit-circuitpython-typing-1.9.4/circuitpython_typing/led.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/circuitpython_typing/pil.py` & `adafruit-circuitpython-typing-1.9.4/circuitpython_typing/pil.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/circuitpython_typing/pwmio.py` & `adafruit-circuitpython-typing-1.9.4/circuitpython_typing/pwmio.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/circuitpython_typing/socket.py` & `adafruit-circuitpython-typing-1.9.4/circuitpython_typing/socket.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/docs/_static/favicon.ico` & `adafruit-circuitpython-typing-1.9.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/docs/conf.py` & `adafruit-circuitpython-typing-1.9.4/docs/conf.py`

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

### Comparing `adafruit-circuitpython-typing-1.9.3/docs/index.rst` & `adafruit-circuitpython-typing-1.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-typing-1.9.3/pyproject.toml` & `adafruit-circuitpython-typing-1.9.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-typing"
 description = "Types needed for type annotation that are not in `typing`"
-version = "1.9.3"
+version = "1.9.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Typing"}
 keywords = [
     "adafruit",
```

