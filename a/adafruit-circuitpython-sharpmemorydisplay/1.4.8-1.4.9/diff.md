# Comparing `tmp/adafruit-circuitpython-sharpmemorydisplay-1.4.8.tar.gz` & `tmp/adafruit-circuitpython-sharpmemorydisplay-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-sharpmemorydisplay-1.4.8.tar", last modified: Thu May 18 15:41:37 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-sharpmemorydisplay-1.4.9.tar", last modified: Fri May 26 16:12:31 2023, max compression
```

## Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8.tar` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.396075 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.400076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:41:37.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-18 15:41:28.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_sharpmemorydisplay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5739 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/font5x8.bin.license
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-18 15:41:28.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/sharpmemorydisplay_pillow_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-18 15:41:28.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/sharpmemorydisplay_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-18 15:41:28.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:41:16.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:41:37.404076 adafruit-circuitpython-sharpmemorydisplay-1.4.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.086207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.078207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.082208 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.082208 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.086207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-26 16:12:31.086207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.086207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_circuitpython_sharpmemorydisplay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3511 2023-05-26 16:12:31.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-05-26 16:12:31.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:12:31.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_circuitpython_sharpmemorydisplay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:12:31.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_circuitpython_sharpmemorydisplay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:12:31.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_circuitpython_sharpmemorydisplay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5268 2023-05-26 16:12:23.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_sharpmemorydisplay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.086207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.086207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:31.086207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/examples/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/examples/font5x8.bin.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-26 16:12:23.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/examples/sharpmemorydisplay_pillow_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-05-26 16:12:23.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/examples/sharpmemorydisplay_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-26 16:12:23.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:12:13.000000 adafruit-circuitpython-sharpmemorydisplay-1.4.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:12:31.086207 adafruit-circuitpython-sharpmemorydisplay-1.4.9/setup.cfg
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/.gitignore` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/.pre-commit-config.yaml` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/.pylintrc` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSE` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/MIT.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/PKG-INFO` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sharpmemorydisplay
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython display control library for Sharp memory displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay
 Keywords: adafruit,sharp,memory,display,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/README.rst` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_circuitpython_sharpmemorydisplay.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-sharpmemorydisplay
-Version: 1.4.8
+Version: 1.4.9
 Summary: CircuitPython display control library for Sharp memory displays.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay
 Keywords: adafruit,sharp,memory,display,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_circuitpython_sharpmemorydisplay.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/adafruit_sharpmemorydisplay.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/adafruit_sharpmemorydisplay.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 from micropython import const
 
 try:
     import numpy
 except ImportError:
     numpy = None
 
-__version__ = "1.4.8"
+__version__ = "1.4.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay.git"
 
 _SHARPMEM_BIT_WRITECMD = const(0x80)  # in lsb
 _SHARPMEM_BIT_VCOM = const(0x40)  # in lsb
 _SHARPMEM_BIT_CLEAR = const(0x20)  # in lsb
```

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/_static/favicon.ico` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/conf.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/conf.py`

 * *Files 1% similar despite different names*

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

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/docs/index.rst` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/font5x8.bin` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/examples/font5x8.bin`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/sharpmemorydisplay_pillow_demo.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/examples/sharpmemorydisplay_pillow_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/examples/sharpmemorydisplay_simpletest.py` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/examples/sharpmemorydisplay_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-sharpmemorydisplay-1.4.8/pyproject.toml` & `adafruit-circuitpython-sharpmemorydisplay-1.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-sharpmemorydisplay"
 description = "CircuitPython display control library for Sharp memory displays."
-version = "1.4.8"
+version = "1.4.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SharpMemoryDisplay"}
 keywords = [
     "adafruit",
```

