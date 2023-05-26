# Comparing `tmp/adafruit-circuitpython-si5351-1.4.0.tar.gz` & `tmp/adafruit-circuitpython-si5351-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-si5351-1.4.0.tar", last modified: Thu May 11 14:14:37 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-si5351-1.4.1.tar", last modified: Fri May 26 16:18:18 2023, max compression
```

## Comparing `adafruit-circuitpython-si5351-1.4.0.tar` & `adafruit-circuitpython-si5351-1.4.1.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.720312 adafruit-circuitpython-si5351-1.4.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/adafruit_circuitpython_si5351.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-11 14:14:37.000000 adafruit-circuitpython-si5351-1.4.0/adafruit_circuitpython_si5351.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-11 14:14:37.000000 adafruit-circuitpython-si5351-1.4.0/adafruit_circuitpython_si5351.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-11 14:14:37.000000 adafruit-circuitpython-si5351-1.4.0/adafruit_circuitpython_si5351.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-11 14:14:37.000000 adafruit-circuitpython-si5351-1.4.0/adafruit_circuitpython_si5351.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-11 14:14:37.000000 adafruit-circuitpython-si5351-1.4.0/adafruit_circuitpython_si5351.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    21666 2023-05-11 14:14:29.000000 adafruit-circuitpython-si5351-1.4.0/adafruit_si5351.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5490 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-11 14:14:29.000000 adafruit-circuitpython-si5351-1.4.0/examples/si5351_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-11 14:14:29.000000 adafruit-circuitpython-si5351-1.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-11 14:14:18.000000 adafruit-circuitpython-si5351-1.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-11 14:14:37.724312 adafruit-circuitpython-si5351-1.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.694891 adafruit-circuitpython-si5351-1.4.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.686891 adafruit-circuitpython-si5351-1.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.690891 adafruit-circuitpython-si5351-1.4.1/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.690891 adafruit-circuitpython-si5351-1.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.690891 adafruit-circuitpython-si5351-1.4.1/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-26 16:18:18.694891 adafruit-circuitpython-si5351-1.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2554 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.690891 adafruit-circuitpython-si5351-1.4.1/adafruit_circuitpython_si5351.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-05-26 16:18:18.000000 adafruit-circuitpython-si5351-1.4.1/adafruit_circuitpython_si5351.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-26 16:18:18.000000 adafruit-circuitpython-si5351-1.4.1/adafruit_circuitpython_si5351.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:18:18.000000 adafruit-circuitpython-si5351-1.4.1/adafruit_circuitpython_si5351.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 16:18:18.000000 adafruit-circuitpython-si5351-1.4.1/adafruit_circuitpython_si5351.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:18:18.000000 adafruit-circuitpython-si5351-1.4.1/adafruit_circuitpython_si5351.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    21666 2023-05-26 16:18:10.000000 adafruit-circuitpython-si5351-1.4.1/adafruit_si5351.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.690891 adafruit-circuitpython-si5351-1.4.1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.694891 adafruit-circuitpython-si5351-1.4.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:18:18.694891 adafruit-circuitpython-si5351-1.4.1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-05-26 16:18:10.000000 adafruit-circuitpython-si5351-1.4.1/examples/si5351_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-26 16:18:10.000000 adafruit-circuitpython-si5351-1.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-26 16:18:00.000000 adafruit-circuitpython-si5351-1.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:18:18.694891 adafruit-circuitpython-si5351-1.4.1/setup.cfg
```

### Comparing `adafruit-circuitpython-si5351-1.4.0/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-si5351-1.4.1/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/.gitignore` & `adafruit-circuitpython-si5351-1.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/.pre-commit-config.yaml` & `adafruit-circuitpython-si5351-1.4.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/.pylintrc` & `adafruit-circuitpython-si5351-1.4.1/.pylintrc`

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

### Comparing `adafruit-circuitpython-si5351-1.4.0/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-si5351-1.4.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/LICENSE` & `adafruit-circuitpython-si5351-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-si5351-1.4.1/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/LICENSES/MIT.txt` & `adafruit-circuitpython-si5351-1.4.1/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/LICENSES/Unlicense.txt` & `adafruit-circuitpython-si5351-1.4.1/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/PKG-INFO` & `adafruit-circuitpython-si5351-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si5351
-Version: 1.4.0
+Version: 1.4.1
 Summary: CircuitPython library for SI5351 clock generator module.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI5351
 Keywords: adafruit,si5351,clock,generator,module,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si5351-1.4.0/README.rst` & `adafruit-circuitpython-si5351-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/adafruit_circuitpython_si5351.egg-info/PKG-INFO` & `adafruit-circuitpython-si5351-1.4.1/adafruit_circuitpython_si5351.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si5351
-Version: 1.4.0
+Version: 1.4.1
 Summary: CircuitPython library for SI5351 clock generator module.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI5351
 Keywords: adafruit,si5351,clock,generator,module,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si5351-1.4.0/adafruit_circuitpython_si5351.egg-info/SOURCES.txt` & `adafruit-circuitpython-si5351-1.4.1/adafruit_circuitpython_si5351.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/adafruit_si5351.py` & `adafruit-circuitpython-si5351-1.4.1/adafruit_si5351.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 try:
     import typing  # pylint: disable=unused-import
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.4.0"
+__version__ = "1.4.1"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SI5351.git"
 
 
 # Internal constants:
 _SI5351_ADDRESS = const(0x60)  # Assumes ADDR pin = low
 _SI5351_READBIT = const(0x01)
 _SI5351_CRYSTAL_FREQUENCY = 25000000.0  # Fixed 25mhz crystal on board.
```

### Comparing `adafruit-circuitpython-si5351-1.4.0/docs/_static/favicon.ico` & `adafruit-circuitpython-si5351-1.4.1/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/docs/conf.py` & `adafruit-circuitpython-si5351-1.4.1/docs/conf.py`

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
     "sphinx.ext.todo",
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
```

### Comparing `adafruit-circuitpython-si5351-1.4.0/docs/index.rst` & `adafruit-circuitpython-si5351-1.4.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/examples/si5351_simpletest.py` & `adafruit-circuitpython-si5351-1.4.1/examples/si5351_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si5351-1.4.0/pyproject.toml` & `adafruit-circuitpython-si5351-1.4.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-si5351"
 description = "CircuitPython library for SI5351 clock generator module."
-version = "1.4.0"
+version = "1.4.1"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SI5351"}
 keywords = [
     "adafruit",
```

