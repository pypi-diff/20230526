# Comparing `tmp/adafruit-circuitpython-framebuf-1.6.2.tar.gz` & `tmp/adafruit-circuitpython-framebuf-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-framebuf-1.6.2.tar", last modified: Thu May 18 15:44:06 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-framebuf-1.6.3.tar", last modified: Fri May 26 16:22:53 2023, max compression
```

## Comparing `adafruit-circuitpython-framebuf-1.6.2.tar` & `adafruit-circuitpython-framebuf-1.6.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.751575 adafruit-circuitpython-framebuf-1.6.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-18 15:44:06.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    23905 2023-05-18 15:43:59.000000 adafruit-circuitpython-framebuf-1.6.2/adafruit_framebuf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.755575 adafruit-circuitpython-framebuf-1.6.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5661 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/examples/font5x8.bin
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/examples/font5x8.bin.license
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-18 15:43:59.000000 adafruit-circuitpython-framebuf-1.6.2/examples/framebuf_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-18 15:43:59.000000 adafruit-circuitpython-framebuf-1.6.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-18 15:43:50.000000 adafruit-circuitpython-framebuf-1.6.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:44:06.759575 adafruit-circuitpython-framebuf-1.6.2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-05-18 15:43:59.000000 adafruit-circuitpython-framebuf-1.6.2/utils/font_to_bin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.115454 adafruit-circuitpython-framebuf-1.6.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.107453 adafruit-circuitpython-framebuf-1.6.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.111454 adafruit-circuitpython-framebuf-1.6.3/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.111454 adafruit-circuitpython-framebuf-1.6.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.111454 adafruit-circuitpython-framebuf-1.6.3/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-26 16:22:53.115454 adafruit-circuitpython-framebuf-1.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.111454 adafruit-circuitpython-framebuf-1.6.3/adafruit_circuitpython_framebuf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-05-26 16:22:53.000000 adafruit-circuitpython-framebuf-1.6.3/adafruit_circuitpython_framebuf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-26 16:22:53.000000 adafruit-circuitpython-framebuf-1.6.3/adafruit_circuitpython_framebuf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:22:53.000000 adafruit-circuitpython-framebuf-1.6.3/adafruit_circuitpython_framebuf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:22:53.000000 adafruit-circuitpython-framebuf-1.6.3/adafruit_circuitpython_framebuf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:22:53.000000 adafruit-circuitpython-framebuf-1.6.3/adafruit_circuitpython_framebuf.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    23905 2023-05-26 16:22:45.000000 adafruit-circuitpython-framebuf-1.6.3/adafruit_framebuf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.111454 adafruit-circuitpython-framebuf-1.6.3/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.115454 adafruit-circuitpython-framebuf-1.6.3/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.115454 adafruit-circuitpython-framebuf-1.6.3/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/examples/font5x8.bin
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/examples/font5x8.bin.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-26 16:22:45.000000 adafruit-circuitpython-framebuf-1.6.3/examples/framebuf_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-26 16:22:45.000000 adafruit-circuitpython-framebuf-1.6.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:22:36.000000 adafruit-circuitpython-framebuf-1.6.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:22:53.115454 adafruit-circuitpython-framebuf-1.6.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:22:53.115454 adafruit-circuitpython-framebuf-1.6.3/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)    38224 2023-05-26 16:22:45.000000 adafruit-circuitpython-framebuf-1.6.3/utils/font_to_bin.py
```

### Comparing `adafruit-circuitpython-framebuf-1.6.2/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-framebuf-1.6.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/.gitignore` & `adafruit-circuitpython-framebuf-1.6.3/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/.pre-commit-config.yaml` & `adafruit-circuitpython-framebuf-1.6.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/.pylintrc` & `adafruit-circuitpython-framebuf-1.6.3/.pylintrc`

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

### Comparing `adafruit-circuitpython-framebuf-1.6.2/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-framebuf-1.6.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/LICENSE` & `adafruit-circuitpython-framebuf-1.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-framebuf-1.6.3/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/LICENSES/MIT.txt` & `adafruit-circuitpython-framebuf-1.6.3/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/LICENSES/Unlicense.txt` & `adafruit-circuitpython-framebuf-1.6.3/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/PKG-INFO` & `adafruit-circuitpython-framebuf-1.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-framebuf
-Version: 1.6.2
+Version: 1.6.3
 Summary: CircuitPython frambuf module, based on the Python frambuf module.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_framebuf
 Keywords: adafruit,display,framebuf,framebuffer,software,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-framebuf-1.6.2/README.rst` & `adafruit-circuitpython-framebuf-1.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/PKG-INFO` & `adafruit-circuitpython-framebuf-1.6.3/adafruit_circuitpython_framebuf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-framebuf
-Version: 1.6.2
+Version: 1.6.3
 Summary: CircuitPython frambuf module, based on the Python frambuf module.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_framebuf
 Keywords: adafruit,display,framebuf,framebuffer,software,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-framebuf-1.6.2/adafruit_circuitpython_framebuf.egg-info/SOURCES.txt` & `adafruit-circuitpython-framebuf-1.6.3/adafruit_circuitpython_framebuf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/adafruit_framebuf.py` & `adafruit-circuitpython-framebuf-1.6.3/adafruit_framebuf.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 """
 
-__version__ = "1.6.2"
+__version__ = "1.6.3"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_framebuf.git"
 
 import os
 import struct
 
 # Framebuf format constants:
 MVLSB = 0  # Single bit displays (like SSD1306 OLED)
```

### Comparing `adafruit-circuitpython-framebuf-1.6.2/docs/_static/favicon.ico` & `adafruit-circuitpython-framebuf-1.6.3/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/docs/conf.py` & `adafruit-circuitpython-framebuf-1.6.3/docs/conf.py`

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

### Comparing `adafruit-circuitpython-framebuf-1.6.2/docs/index.rst` & `adafruit-circuitpython-framebuf-1.6.3/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/examples/font5x8.bin` & `adafruit-circuitpython-framebuf-1.6.3/examples/font5x8.bin`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/examples/framebuf_simpletest.py` & `adafruit-circuitpython-framebuf-1.6.3/examples/framebuf_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-framebuf-1.6.2/pyproject.toml` & `adafruit-circuitpython-framebuf-1.6.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-framebuf"
 description = "CircuitPython frambuf module, based on the Python frambuf module."
-version = "1.6.2"
+version = "1.6.3"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_framebuf"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-framebuf-1.6.2/utils/font_to_bin.py` & `adafruit-circuitpython-framebuf-1.6.3/utils/font_to_bin.py`

 * *Files identical despite different names*

