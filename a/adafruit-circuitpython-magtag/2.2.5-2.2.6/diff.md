# Comparing `tmp/adafruit-circuitpython-magtag-2.2.5.tar.gz` & `tmp/adafruit-circuitpython-magtag-2.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-magtag-2.2.5.tar", last modified: Thu May 18 15:38:30 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-magtag-2.2.6.tar", last modified: Fri May 26 16:11:13 2023, max compression
```

## Comparing `adafruit-circuitpython-magtag-2.2.5.tar` & `adafruit-circuitpython-magtag-2.2.6.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.731775 adafruit-circuitpython-magtag-2.2.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.723775 adafruit-circuitpython-magtag-2.2.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 15:38:30.731775 adafruit-circuitpython-magtag-2.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:38:30.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/graphics.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7326 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/magtag.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2595 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5897 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/peripherals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5858 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:38:30.727775 adafruit-circuitpython-magtag-2.2.5/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/examples/magtag_btn_sleep_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/examples/magtag_quote_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/examples/magtag_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-18 15:38:23.000000 adafruit-circuitpython-magtag-2.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-18 15:38:14.000000 adafruit-circuitpython-magtag-2.2.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:38:30.731775 adafruit-circuitpython-magtag-2.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.184265 adafruit-circuitpython-magtag-2.2.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.176265 adafruit-circuitpython-magtag-2.2.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.180265 adafruit-circuitpython-magtag-2.2.6/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.180265 adafruit-circuitpython-magtag-2.2.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.180265 adafruit-circuitpython-magtag-2.2.6/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-26 16:11:13.184265 adafruit-circuitpython-magtag-2.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.180265 adafruit-circuitpython-magtag-2.2.6/adafruit_circuitpython_magtag.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3720 2023-05-26 16:11:13.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_circuitpython_magtag.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-05-26 16:11:13.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_circuitpython_magtag.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:11:13.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_circuitpython_magtag.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 16:11:13.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_circuitpython_magtag.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:11:13.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_circuitpython_magtag.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.180265 adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3364 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/graphics.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7326 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/magtag.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2595 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5897 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/peripherals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.184265 adafruit-circuitpython-magtag-2.2.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.184265 adafruit-circuitpython-magtag-2.2.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5886 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:13.184265 adafruit-circuitpython-magtag-2.2.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/examples/magtag_btn_sleep_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/examples/magtag_quote_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/examples/magtag_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-26 16:11:04.000000 adafruit-circuitpython-magtag-2.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-26 16:10:53.000000 adafruit-circuitpython-magtag-2.2.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:11:13.184265 adafruit-circuitpython-magtag-2.2.6/setup.cfg
```

### Comparing `adafruit-circuitpython-magtag-2.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-magtag-2.2.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/.gitignore` & `adafruit-circuitpython-magtag-2.2.6/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/.pre-commit-config.yaml` & `adafruit-circuitpython-magtag-2.2.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/.pylintrc` & `adafruit-circuitpython-magtag-2.2.6/.pylintrc`

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

### Comparing `adafruit-circuitpython-magtag-2.2.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-magtag-2.2.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/LICENSE` & `adafruit-circuitpython-magtag-2.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-magtag-2.2.6/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/LICENSES/MIT.txt` & `adafruit-circuitpython-magtag-2.2.6/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/LICENSES/Unlicense.txt` & `adafruit-circuitpython-magtag-2.2.6/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/PKG-INFO` & `adafruit-circuitpython-magtag-2.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-magtag
-Version: 2.2.5
+Version: 2.2.6
 Summary: Helper library for the Adafruit MagTag
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MagTag
 Keywords: adafruit,magtag,eink,iot,esp32,espressif,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-magtag-2.2.5/README.rst` & `adafruit-circuitpython-magtag-2.2.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/PKG-INFO` & `adafruit-circuitpython-magtag-2.2.6/adafruit_circuitpython_magtag.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-magtag
-Version: 2.2.5
+Version: 2.2.6
 Summary: Helper library for the Adafruit MagTag
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_MagTag
 Keywords: adafruit,magtag,eink,iot,esp32,espressif,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-magtag-2.2.5/adafruit_circuitpython_magtag.egg-info/SOURCES.txt` & `adafruit-circuitpython-magtag-2.2.6/adafruit_circuitpython_magtag.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/graphics.py` & `adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/graphics.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from adafruit_portalbase.graphics import GraphicsBase
 
 try:
     from typing import Union, Optional, Tuple
 except ImportError:
     pass
 
-__version__ = "2.2.5"
+__version__ = "2.2.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Graphics(GraphicsBase):
     """Graphics Helper Class for the MagTag Library
 
     :param default_bg: The path to your default background image file or a hex color.
```

### Comparing `adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/magtag.py` & `adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/magtag.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 try:
     from typing import Optional, Union, Sequence, Dict, Callable, Any
     import microcontroller
     import neopixel
 except ImportError:
     pass
 
-__version__ = "2.2.5"
+__version__ = "2.2.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class MagTag(PortalBase):
     """Class representing the Adafruit MagTag.
 
     :param url: The URL of your data source. Defaults to ``None``.
```

### Comparing `adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/network.py` & `adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 try:
     from typing import Optional, Union
     import microcontroller
 except ImportError:
     pass
 
-__version__ = "2.2.5"
+__version__ = "2.2.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Network(NetworkBase):
     """Class representing the Adafruit MagTag.
 
     :param status_neopixel: The pin for the status NeoPixel. Use ``board.NEOPIXEL`` for the on-board
```

### Comparing `adafruit-circuitpython-magtag-2.2.5/adafruit_magtag/peripherals.py` & `adafruit-circuitpython-magtag-2.2.6/adafruit_magtag/peripherals.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 import board
 from digitalio import DigitalInOut, Direction, Pull
 from analogio import AnalogIn
 import neopixel
 import simpleio
 
-__version__ = "2.2.5"
+__version__ = "2.2.6"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag.git"
 
 
 class Peripherals:
     """Peripherals Helper Class for the MagTag Library"""
 
     # pylint: disable=too-many-instance-attributes, too-many-locals, too-many-branches, too-many-statements
```

### Comparing `adafruit-circuitpython-magtag-2.2.5/docs/_static/favicon.ico` & `adafruit-circuitpython-magtag-2.2.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/docs/conf.py` & `adafruit-circuitpython-magtag-2.2.6/docs/conf.py`

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

### Comparing `adafruit-circuitpython-magtag-2.2.5/docs/index.rst` & `adafruit-circuitpython-magtag-2.2.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/examples/magtag_btn_sleep_demo.py` & `adafruit-circuitpython-magtag-2.2.6/examples/magtag_btn_sleep_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/examples/magtag_quote_demo.py` & `adafruit-circuitpython-magtag-2.2.6/examples/magtag_quote_demo.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/examples/magtag_simpletest.py` & `adafruit-circuitpython-magtag-2.2.6/examples/magtag_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-magtag-2.2.5/pyproject.toml` & `adafruit-circuitpython-magtag-2.2.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-magtag"
 description = "Helper library for the Adafruit MagTag"
-version = "2.2.5"
+version = "2.2.6"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_MagTag"}
 keywords = [
     "adafruit",
```

