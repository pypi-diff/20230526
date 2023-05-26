# Comparing `tmp/adafruit-circuitpython-dymoscale-2.0.4.tar.gz` & `tmp/adafruit-circuitpython-dymoscale-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-dymoscale-2.0.4.tar", last modified: Tue May 16 17:53:05 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-dymoscale-2.0.5.tar", last modified: Fri May 26 16:09:53 2023, max compression
```

## Comparing `adafruit-circuitpython-dymoscale-2.0.4.tar` & `adafruit-circuitpython-dymoscale-2.0.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.878676 adafruit-circuitpython-dymoscale-2.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.874676 adafruit-circuitpython-dymoscale-2.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.874676 adafruit-circuitpython-dymoscale-2.0.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.874676 adafruit-circuitpython-dymoscale-2.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.878676 adafruit-circuitpython-dymoscale-2.0.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-16 17:53:05.878676 adafruit-circuitpython-dymoscale-2.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.878676 adafruit-circuitpython-dymoscale-2.0.4/adafruit_circuitpython_dymoscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-16 17:53:05.000000 adafruit-circuitpython-dymoscale-2.0.4/adafruit_circuitpython_dymoscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-16 17:53:05.000000 adafruit-circuitpython-dymoscale-2.0.4/adafruit_circuitpython_dymoscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:53:05.000000 adafruit-circuitpython-dymoscale-2.0.4/adafruit_circuitpython_dymoscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 17:53:05.000000 adafruit-circuitpython-dymoscale-2.0.4/adafruit_circuitpython_dymoscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-16 17:53:05.000000 adafruit-circuitpython-dymoscale-2.0.4/adafruit_circuitpython_dymoscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-16 17:52:58.000000 adafruit-circuitpython-dymoscale-2.0.4/adafruit_dymoscale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.878676 adafruit-circuitpython-dymoscale-2.0.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.878676 adafruit-circuitpython-dymoscale-2.0.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5660 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:53:05.878676 adafruit-circuitpython-dymoscale-2.0.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-16 17:52:58.000000 adafruit-circuitpython-dymoscale-2.0.4/examples/dymoscale_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-16 17:52:58.000000 adafruit-circuitpython-dymoscale-2.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 17:52:49.000000 adafruit-circuitpython-dymoscale-2.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:53:05.878676 adafruit-circuitpython-dymoscale-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.612023 adafruit-circuitpython-dymoscale-2.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1098 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/adafruit_circuitpython_dymoscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-26 16:09:53.000000 adafruit-circuitpython-dymoscale-2.0.5/adafruit_circuitpython_dymoscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-26 16:09:53.000000 adafruit-circuitpython-dymoscale-2.0.5/adafruit_circuitpython_dymoscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:09:53.000000 adafruit-circuitpython-dymoscale-2.0.5/adafruit_circuitpython_dymoscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:09:53.000000 adafruit-circuitpython-dymoscale-2.0.5/adafruit_circuitpython_dymoscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 16:09:53.000000 adafruit-circuitpython-dymoscale-2.0.5/adafruit_circuitpython_dymoscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-05-26 16:09:45.000000 adafruit-circuitpython-dymoscale-2.0.5/adafruit_dymoscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-26 16:09:45.000000 adafruit-circuitpython-dymoscale-2.0.5/examples/dymoscale_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-26 16:09:45.000000 adafruit-circuitpython-dymoscale-2.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:09:35.000000 adafruit-circuitpython-dymoscale-2.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:09:53.616023 adafruit-circuitpython-dymoscale-2.0.5/setup.cfg
```

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-dymoscale-2.0.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/.gitignore` & `adafruit-circuitpython-dymoscale-2.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/.pre-commit-config.yaml` & `adafruit-circuitpython-dymoscale-2.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/.pylintrc` & `adafruit-circuitpython-dymoscale-2.0.5/.pylintrc`

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

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-dymoscale-2.0.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/LICENSE` & `adafruit-circuitpython-dymoscale-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-dymoscale-2.0.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/LICENSES/MIT.txt` & `adafruit-circuitpython-dymoscale-2.0.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-dymoscale-2.0.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/PKG-INFO` & `adafruit-circuitpython-dymoscale-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dymoscale
-Version: 2.0.4
+Version: 2.0.5
 Summary: CircuitPython interface for DYMO scales.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DymoScale
 Keywords: adafruit,blinka,circuitpython,micropython,dymoscale,dymo,scale
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/README.rst` & `adafruit-circuitpython-dymoscale-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/adafruit_circuitpython_dymoscale.egg-info/PKG-INFO` & `adafruit-circuitpython-dymoscale-2.0.5/adafruit_circuitpython_dymoscale.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-dymoscale
-Version: 2.0.4
+Version: 2.0.5
 Summary: CircuitPython interface for DYMO scales.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DymoScale
 Keywords: adafruit,blinka,circuitpython,micropython,dymoscale,dymo,scale
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/adafruit_circuitpython_dymoscale.egg-info/SOURCES.txt` & `adafruit-circuitpython-dymoscale-2.0.5/adafruit_circuitpython_dymoscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/adafruit_dymoscale.py` & `adafruit-circuitpython-dymoscale-2.0.5/adafruit_dymoscale.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 from pulseio import PulseIn
 from micropython import const
 
 OUNCES = const(0x0B)  # data in weight is in ounces
 GRAMS = const(0x02)  # data in weight is in grams
 PULSE_WIDTH = 72.5
 
-__version__ = "2.0.4"
+__version__ = "2.0.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DymoScale.git"
 
 
 # pylint: disable=too-few-public-methods
 class ScaleReading:
     """Dymo Scale Data"""
```

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/docs/_static/favicon.ico` & `adafruit-circuitpython-dymoscale-2.0.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/docs/conf.py` & `adafruit-circuitpython-dymoscale-2.0.5/docs/conf.py`

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

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/docs/index.rst` & `adafruit-circuitpython-dymoscale-2.0.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/examples/dymoscale_simpletest.py` & `adafruit-circuitpython-dymoscale-2.0.5/examples/dymoscale_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-dymoscale-2.0.4/pyproject.toml` & `adafruit-circuitpython-dymoscale-2.0.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-dymoscale"
 description = "CircuitPython interface for DYMO scales."
-version = "2.0.4"
+version = "2.0.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DymoScale"}
 keywords = [
     "adafruit",
```

