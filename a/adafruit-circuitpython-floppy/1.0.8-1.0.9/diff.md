# Comparing `tmp/adafruit-circuitpython-floppy-1.0.8.tar.gz` & `tmp/adafruit-circuitpython-floppy-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-floppy-1.0.8.tar", last modified: Thu May 18 15:36:15 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-floppy-1.0.9.tar", last modified: Fri May 26 16:16:51 2023, max compression
```

## Comparing `adafruit-circuitpython-floppy-1.0.8.tar` & `adafruit-circuitpython-floppy-1.0.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.675026 adafruit-circuitpython-floppy-1.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.683026 adafruit-circuitpython-floppy-1.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.687026 adafruit-circuitpython-floppy-1.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.687026 adafruit-circuitpython-floppy-1.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.691027 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-18 15:36:15.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-18 15:36:07.000000 adafruit-circuitpython-floppy-1.0.8/adafruit_floppy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-18 15:36:07.000000 adafruit-circuitpython-floppy-1.0.8/examples/floppy_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-18 15:36:07.000000 adafruit-circuitpython-floppy-1.0.8/examples/floppy_vfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-18 15:36:07.000000 adafruit-circuitpython-floppy-1.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-18 15:35:53.000000 adafruit-circuitpython-floppy-1.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:36:15.695027 adafruit-circuitpython-floppy-1.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.404267 adafruit-circuitpython-floppy-1.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.400267 adafruit-circuitpython-floppy-1.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.400267 adafruit-circuitpython-floppy-1.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.400267 adafruit-circuitpython-floppy-1.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.400267 adafruit-circuitpython-floppy-1.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-26 16:16:51.404267 adafruit-circuitpython-floppy-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.404267 adafruit-circuitpython-floppy-1.0.9/adafruit_circuitpython_floppy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-26 16:16:51.000000 adafruit-circuitpython-floppy-1.0.9/adafruit_circuitpython_floppy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 16:16:51.000000 adafruit-circuitpython-floppy-1.0.9/adafruit_circuitpython_floppy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:16:51.000000 adafruit-circuitpython-floppy-1.0.9/adafruit_circuitpython_floppy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 16:16:51.000000 adafruit-circuitpython-floppy-1.0.9/adafruit_circuitpython_floppy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:16:51.000000 adafruit-circuitpython-floppy-1.0.9/adafruit_circuitpython_floppy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    10099 2023-05-26 16:16:43.000000 adafruit-circuitpython-floppy-1.0.9/adafruit_floppy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.404267 adafruit-circuitpython-floppy-1.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.404267 adafruit-circuitpython-floppy-1.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:16:51.404267 adafruit-circuitpython-floppy-1.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-26 16:16:43.000000 adafruit-circuitpython-floppy-1.0.9/examples/floppy_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-26 16:16:43.000000 adafruit-circuitpython-floppy-1.0.9/examples/floppy_vfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-26 16:16:43.000000 adafruit-circuitpython-floppy-1.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-26 16:16:33.000000 adafruit-circuitpython-floppy-1.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:16:51.404267 adafruit-circuitpython-floppy-1.0.9/setup.cfg
```

### Comparing `adafruit-circuitpython-floppy-1.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-floppy-1.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/.gitignore` & `adafruit-circuitpython-floppy-1.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-floppy-1.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/.pylintrc` & `adafruit-circuitpython-floppy-1.0.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-floppy-1.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-floppy-1.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/LICENSE` & `adafruit-circuitpython-floppy-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-floppy-1.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-floppy-1.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-floppy-1.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/PKG-INFO` & `adafruit-circuitpython-floppy-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-floppy
-Version: 1.0.8
+Version: 1.0.9
 Summary: Access floppy drives from CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Floppy
 Keywords: adafruit,floppy,drive,storage,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-floppy-1.0.8/README.rst` & `adafruit-circuitpython-floppy-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/PKG-INFO` & `adafruit-circuitpython-floppy-1.0.9/adafruit_circuitpython_floppy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-floppy
-Version: 1.0.8
+Version: 1.0.9
 Summary: Access floppy drives from CircuitPython
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_Floppy
 Keywords: adafruit,floppy,drive,storage,hardware,micropythoncircuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-floppy-1.0.8/adafruit_circuitpython_floppy.egg-info/SOURCES.txt` & `adafruit-circuitpython-floppy-1.0.9/adafruit_circuitpython_floppy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/adafruit_floppy.py` & `adafruit-circuitpython-floppy-1.0.9/adafruit_floppy.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     import typing
     import microcontroller
     import circuitpython_typing  # pylint: disable=unused-import
 except ImportError:
     pass
 
 
-__version__ = "1.0.8"
+__version__ = "1.0.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_floppy.git"
 
 
 def _optionaldigitalinout(
     maybe_pin: typing.Optional[microcontroller.Pin],
 ) -> typing.Optional[DigitalInOut]:
     return None if maybe_pin is None else DigitalInOut(maybe_pin)
```

### Comparing `adafruit-circuitpython-floppy-1.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-floppy-1.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/docs/conf.py` & `adafruit-circuitpython-floppy-1.0.9/docs/conf.py`

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

### Comparing `adafruit-circuitpython-floppy-1.0.8/docs/index.rst` & `adafruit-circuitpython-floppy-1.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/examples/floppy_simpletest.py` & `adafruit-circuitpython-floppy-1.0.9/examples/floppy_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/examples/floppy_vfs.py` & `adafruit-circuitpython-floppy-1.0.9/examples/floppy_vfs.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-floppy-1.0.8/pyproject.toml` & `adafruit-circuitpython-floppy-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-floppy"
 description = "Access floppy drives from CircuitPython"
-version = "1.0.8"
+version = "1.0.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_Floppy"}
 keywords = [
     "adafruit",
```

