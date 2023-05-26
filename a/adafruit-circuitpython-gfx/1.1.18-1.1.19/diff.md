# Comparing `tmp/adafruit-circuitpython-gfx-1.1.18.tar.gz` & `tmp/adafruit-circuitpython-gfx-1.1.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-gfx-1.1.18.tar", last modified: Thu May 11 14:51:25 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-gfx-1.1.19.tar", last modified: Fri May 26 16:22:34 2023, max compression
```

## Comparing `adafruit-circuitpython-gfx-1.1.18.tar` & `adafruit-circuitpython-gfx-1.1.19.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.064708 adafruit-circuitpython-gfx-1.1.18/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.060708 adafruit-circuitpython-gfx-1.1.18/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.060708 adafruit-circuitpython-gfx-1.1.18/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.060708 adafruit-circuitpython-gfx-1.1.18/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.060708 adafruit-circuitpython-gfx-1.1.18/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)    19269 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/LICENSES/CC-BY-NC-3.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-11 14:51:25.064708 adafruit-circuitpython-gfx-1.1.18/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.060708 adafruit-circuitpython-gfx-1.1.18/adafruit_circuitpython_gfx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-11 14:51:25.000000 adafruit-circuitpython-gfx-1.1.18/adafruit_circuitpython_gfx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-11 14:51:25.000000 adafruit-circuitpython-gfx-1.1.18/adafruit_circuitpython_gfx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:51:25.000000 adafruit-circuitpython-gfx-1.1.18/adafruit_circuitpython_gfx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-11 14:51:25.000000 adafruit-circuitpython-gfx-1.1.18/adafruit_circuitpython_gfx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-11 14:51:25.000000 adafruit-circuitpython-gfx-1.1.18/adafruit_circuitpython_gfx.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.060708 adafruit-circuitpython-gfx-1.1.18/adafruit_gfx/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.060708 adafruit-circuitpython-gfx-1.1.18/adafruit_gfx/fonts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-05-11 14:51:16.000000 adafruit-circuitpython-gfx-1.1.18/adafruit_gfx/fonts/gfx_standard_font_01.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19756 2023-05-11 14:51:16.000000 adafruit-circuitpython-gfx-1.1.18/adafruit_gfx/gfx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.064708 adafruit-circuitpython-gfx-1.1.18/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.064708 adafruit-circuitpython-gfx-1.1.18/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:25.064708 adafruit-circuitpython-gfx-1.1.18/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2282 2023-05-11 14:51:16.000000 adafruit-circuitpython-gfx-1.1.18/examples/gfx_ili9341_randlines.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2587 2023-05-11 14:51:16.000000 adafruit-circuitpython-gfx-1.1.18/examples/gfx_ili9341_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-11 14:51:16.000000 adafruit-circuitpython-gfx-1.1.18/examples/gfx_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-11 14:51:16.000000 adafruit-circuitpython-gfx-1.1.18/font_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-11 14:51:16.000000 adafruit-circuitpython-gfx-1.1.18/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-11 14:51:01.000000 adafruit-circuitpython-gfx-1.1.18/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:51:25.064708 adafruit-circuitpython-gfx-1.1.18/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.903859 adafruit-circuitpython-gfx-1.1.19/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.903859 adafruit-circuitpython-gfx-1.1.19/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    19269 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/LICENSES/CC-BY-NC-3.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/adafruit_circuitpython_gfx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-26 16:22:34.000000 adafruit-circuitpython-gfx-1.1.19/adafruit_circuitpython_gfx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-26 16:22:34.000000 adafruit-circuitpython-gfx-1.1.19/adafruit_circuitpython_gfx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:22:34.000000 adafruit-circuitpython-gfx-1.1.19/adafruit_circuitpython_gfx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:22:34.000000 adafruit-circuitpython-gfx-1.1.19/adafruit_circuitpython_gfx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 16:22:34.000000 adafruit-circuitpython-gfx-1.1.19/adafruit_circuitpython_gfx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/adafruit_gfx/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/adafruit_gfx/fonts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4755 2023-05-26 16:22:27.000000 adafruit-circuitpython-gfx-1.1.19/adafruit_gfx/fonts/gfx_standard_font_01.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19756 2023-05-26 16:22:27.000000 adafruit-circuitpython-gfx-1.1.19/adafruit_gfx/gfx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5424 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2282 2023-05-26 16:22:27.000000 adafruit-circuitpython-gfx-1.1.19/examples/gfx_ili9341_randlines.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2587 2023-05-26 16:22:27.000000 adafruit-circuitpython-gfx-1.1.19/examples/gfx_ili9341_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:27.000000 adafruit-circuitpython-gfx-1.1.19/examples/gfx_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8549 2023-05-26 16:22:27.000000 adafruit-circuitpython-gfx-1.1.19/font_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-26 16:22:27.000000 adafruit-circuitpython-gfx-1.1.19/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 16:22:13.000000 adafruit-circuitpython-gfx-1.1.19/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:22:34.907857 adafruit-circuitpython-gfx-1.1.19/setup.cfg
```

### Comparing `adafruit-circuitpython-gfx-1.1.18/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-gfx-1.1.19/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/.gitignore` & `adafruit-circuitpython-gfx-1.1.19/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/.pre-commit-config.yaml` & `adafruit-circuitpython-gfx-1.1.19/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/.pylintrc` & `adafruit-circuitpython-gfx-1.1.19/.pylintrc`

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

### Comparing `adafruit-circuitpython-gfx-1.1.18/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-gfx-1.1.19/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/LICENSE` & `adafruit-circuitpython-gfx-1.1.19/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-gfx-1.1.19/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/LICENSES/CC-BY-NC-3.0.txt` & `adafruit-circuitpython-gfx-1.1.19/LICENSES/CC-BY-NC-3.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/LICENSES/MIT.txt` & `adafruit-circuitpython-gfx-1.1.19/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/LICENSES/Unlicense.txt` & `adafruit-circuitpython-gfx-1.1.19/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/PKG-INFO` & `adafruit-circuitpython-gfx-1.1.19/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-gfx
-Version: 1.1.18
+Version: 1.1.19
 Summary: CircuitPython pixel graphics drawing library
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_GFX
 Keywords: adafruit,gfx,graphics,display,pixel,drawing,hardware,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-gfx-1.1.18/README.rst` & `adafruit-circuitpython-gfx-1.1.19/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/adafruit_circuitpython_gfx.egg-info/PKG-INFO` & `adafruit-circuitpython-gfx-1.1.19/adafruit_circuitpython_gfx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-gfx
-Version: 1.1.18
+Version: 1.1.19
 Summary: CircuitPython pixel graphics drawing library
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_GFX
 Keywords: adafruit,gfx,graphics,display,pixel,drawing,hardware,micropython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-gfx-1.1.18/adafruit_circuitpython_gfx.egg-info/SOURCES.txt` & `adafruit-circuitpython-gfx-1.1.19/adafruit_circuitpython_gfx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/adafruit_gfx/fonts/gfx_standard_font_01.py` & `adafruit-circuitpython-gfx-1.1.19/adafruit_gfx/fonts/gfx_standard_font_01.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/adafruit_gfx/gfx.py` & `adafruit-circuitpython-gfx-1.1.19/adafruit_gfx/gfx.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
-__version__ = "1.1.18"
+__version__ = "1.1.19"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_GFX.git"
 
 
 # pylint: disable=invalid-name
 class GFX:
     # pylint: disable=too-many-instance-attributes
     """Create an instance of the GFX drawing class.
```

### Comparing `adafruit-circuitpython-gfx-1.1.18/docs/_static/favicon.ico` & `adafruit-circuitpython-gfx-1.1.19/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/docs/conf.py` & `adafruit-circuitpython-gfx-1.1.19/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
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

### Comparing `adafruit-circuitpython-gfx-1.1.18/docs/index.rst` & `adafruit-circuitpython-gfx-1.1.19/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/examples/gfx_ili9341_randlines.py` & `adafruit-circuitpython-gfx-1.1.19/examples/gfx_ili9341_randlines.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/examples/gfx_ili9341_test.py` & `adafruit-circuitpython-gfx-1.1.19/examples/gfx_ili9341_test.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-gfx-1.1.18/font_maker.py` & `adafruit-circuitpython-gfx-1.1.19/font_maker.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Author: Jonah Yolles-Murphy on Date: 10/12/18
 
 """`TG-Modules.TG-RGB.rgb`
 a dictionary of bytes organised to create basic text, just the templates
 Author(s):Jonah Yolles-Murphy
 imspiration for base letter style from Ben Gelb"""
 
-__version__ = "1.1.18"
+__version__ = "1.1.19"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_GFX.git"
 
 
 text_dict = {
     "Height": 7,
     "Width": 5,
     "A": (0b10111111, 0b11000100, 0b11000100, 0b11000100, 0b10111111),
```

### Comparing `adafruit-circuitpython-gfx-1.1.18/pyproject.toml` & `adafruit-circuitpython-gfx-1.1.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-gfx"
 description = "CircuitPython pixel graphics drawing library"
-version = "1.1.18"
+version = "1.1.19"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_GFX"}
 keywords = [
     "adafruit",
```

