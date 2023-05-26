# Comparing `tmp/adafruit-circuitpython-ssd1675-1.2.1.tar.gz` & `tmp/adafruit-circuitpython-ssd1675-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-ssd1675-1.2.1.tar", last modified: Thu May 18 15:41:57 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-ssd1675-1.2.2.tar", last modified: Fri May 26 16:13:19 2023, max compression
```

## Comparing `adafruit-circuitpython-ssd1675-1.2.1.tar` & `adafruit-circuitpython-ssd1675-1.2.2.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.545704 adafruit-circuitpython-ssd1675-1.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.541705 adafruit-circuitpython-ssd1675-1.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.541705 adafruit-circuitpython-ssd1675-1.2.1/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.541705 adafruit-circuitpython-ssd1675-1.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.541705 adafruit-circuitpython-ssd1675-1.2.1/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-18 15:41:57.545704 adafruit-circuitpython-ssd1675-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.541705 adafruit-circuitpython-ssd1675-1.2.1/adafruit_circuitpython_ssd1675.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-18 15:41:57.000000 adafruit-circuitpython-ssd1675-1.2.1/adafruit_circuitpython_ssd1675.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-18 15:41:57.000000 adafruit-circuitpython-ssd1675-1.2.1/adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:41:57.000000 adafruit-circuitpython-ssd1675-1.2.1/adafruit_circuitpython_ssd1675.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:41:57.000000 adafruit-circuitpython-ssd1675-1.2.1/adafruit_circuitpython_ssd1675.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-18 15:41:57.000000 adafruit-circuitpython-ssd1675-1.2.1/adafruit_circuitpython_ssd1675.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-18 15:41:50.000000 adafruit-circuitpython-ssd1675-1.2.1/adafruit_ssd1675.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.545704 adafruit-circuitpython-ssd1675-1.2.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.545704 adafruit-circuitpython-ssd1675-1.2.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:41:57.545704 adafruit-circuitpython-ssd1675-1.2.1/examples/
--rwxr-xr-x   0 runner    (1001) docker     (123)   360122 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/examples/display-ruler.bmp
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/examples/display-ruler.bmp.license
--rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-18 15:41:50.000000 adafruit-circuitpython-ssd1675-1.2.1/examples/ssd1675_2.13_monochrome.py
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-18 15:41:50.000000 adafruit-circuitpython-ssd1675-1.2.1/examples/ssd1675_four_corners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-18 15:41:50.000000 adafruit-circuitpython-ssd1675-1.2.1/examples/ssd1675_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-18 15:41:50.000000 adafruit-circuitpython-ssd1675-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:41:42.000000 adafruit-circuitpython-ssd1675-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:41:57.545704 adafruit-circuitpython-ssd1675-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.279277 adafruit-circuitpython-ssd1675-1.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.271277 adafruit-circuitpython-ssd1675-1.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.275277 adafruit-circuitpython-ssd1675-1.2.2/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.275277 adafruit-circuitpython-ssd1675-1.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.275277 adafruit-circuitpython-ssd1675-1.2.2/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-26 16:13:19.279277 adafruit-circuitpython-ssd1675-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3562 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.275277 adafruit-circuitpython-ssd1675-1.2.2/adafruit_circuitpython_ssd1675.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-05-26 16:13:19.000000 adafruit-circuitpython-ssd1675-1.2.2/adafruit_circuitpython_ssd1675.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-05-26 16:13:19.000000 adafruit-circuitpython-ssd1675-1.2.2/adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:13:19.000000 adafruit-circuitpython-ssd1675-1.2.2/adafruit_circuitpython_ssd1675.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:13:19.000000 adafruit-circuitpython-ssd1675-1.2.2/adafruit_circuitpython_ssd1675.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:13:19.000000 adafruit-circuitpython-ssd1675-1.2.2/adafruit_circuitpython_ssd1675.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-05-26 16:13:11.000000 adafruit-circuitpython-ssd1675-1.2.2/adafruit_ssd1675.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.279277 adafruit-circuitpython-ssd1675-1.2.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.279277 adafruit-circuitpython-ssd1675-1.2.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5673 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1252 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:13:19.279277 adafruit-circuitpython-ssd1675-1.2.2/examples/
+-rwxr-xr-x   0 runner    (1001) docker     (123)   360122 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/examples/display-ruler.bmp
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/examples/display-ruler.bmp.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1283 2023-05-26 16:13:11.000000 adafruit-circuitpython-ssd1675-1.2.2/examples/ssd1675_2.13_monochrome.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-05-26 16:13:11.000000 adafruit-circuitpython-ssd1675-1.2.2/examples/ssd1675_four_corners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-05-26 16:13:11.000000 adafruit-circuitpython-ssd1675-1.2.2/examples/ssd1675_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-26 16:13:11.000000 adafruit-circuitpython-ssd1675-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:13:01.000000 adafruit-circuitpython-ssd1675-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:13:19.279277 adafruit-circuitpython-ssd1675-1.2.2/setup.cfg
```

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-ssd1675-1.2.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/.gitignore` & `adafruit-circuitpython-ssd1675-1.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/.pre-commit-config.yaml` & `adafruit-circuitpython-ssd1675-1.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/.pylintrc` & `adafruit-circuitpython-ssd1675-1.2.2/.pylintrc`

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

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-ssd1675-1.2.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/LICENSE` & `adafruit-circuitpython-ssd1675-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-ssd1675-1.2.2/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/LICENSES/MIT.txt` & `adafruit-circuitpython-ssd1675-1.2.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/LICENSES/Unlicense.txt` & `adafruit-circuitpython-ssd1675-1.2.2/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/PKG-INFO` & `adafruit-circuitpython-ssd1675-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1675
-Version: 1.2.1
+Version: 1.2.2
 Summary: CircuitPython `displayio` drivers for SSD1675-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1675
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1675,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/README.rst` & `adafruit-circuitpython-ssd1675-1.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/adafruit_circuitpython_ssd1675.egg-info/PKG-INFO` & `adafruit-circuitpython-ssd1675-1.2.2/adafruit_circuitpython_ssd1675.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-ssd1675
-Version: 1.2.1
+Version: 1.2.2
 Summary: CircuitPython `displayio` drivers for SSD1675-based ePaper displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SSD1675
 Keywords: adafruit,blinka,circuitpython,micropython,ssd1675,displayio,epd,epaper
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt` & `adafruit-circuitpython-ssd1675-1.2.2/adafruit_circuitpython_ssd1675.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/adafruit_ssd1675.py` & `adafruit-circuitpython-ssd1675-1.2.2/adafruit_ssd1675.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware (version 5+) for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 import displayio
 
-__version__ = "1.2.1"
+__version__ = "1.2.2"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1675.git"
 
 _START_SEQUENCE = (
     b"\x12\x80\x02"  # Software reset, 2ms delay
     b"\x74\x01\x54"  # set analog block control
     b"\x7e\x01\x3b"  # set digital block control
     b"\x01\x03\xfa\x01\x00"  # driver output control
```

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/docs/_static/favicon.ico` & `adafruit-circuitpython-ssd1675-1.2.2/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/docs/conf.py` & `adafruit-circuitpython-ssd1675-1.2.2/docs/conf.py`

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

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/docs/index.rst` & `adafruit-circuitpython-ssd1675-1.2.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/examples/display-ruler.bmp` & `adafruit-circuitpython-ssd1675-1.2.2/examples/display-ruler.bmp`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/examples/ssd1675_2.13_monochrome.py` & `adafruit-circuitpython-ssd1675-1.2.2/examples/ssd1675_2.13_monochrome.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/examples/ssd1675_four_corners.py` & `adafruit-circuitpython-ssd1675-1.2.2/examples/ssd1675_four_corners.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/examples/ssd1675_simpletest.py` & `adafruit-circuitpython-ssd1675-1.2.2/examples/ssd1675_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-ssd1675-1.2.1/pyproject.toml` & `adafruit-circuitpython-ssd1675-1.2.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-ssd1675"
 description = "CircuitPython `displayio` drivers for SSD1675-based ePaper displays"
-version = "1.2.1"
+version = "1.2.2"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SSD1675"}
 keywords = [
     "adafruit",
```

