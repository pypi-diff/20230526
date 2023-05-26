# Comparing `tmp/adafruit-circuitpython-aw9523-1.1.6.tar.gz` & `tmp/adafruit-circuitpython-aw9523-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-aw9523-1.1.6.tar", last modified: Tue May 16 17:45:55 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-aw9523-1.1.7.tar", last modified: Fri May 26 16:07:26 2023, max compression
```

## Comparing `adafruit-circuitpython-aw9523-1.1.6.tar` & `adafruit-circuitpython-aw9523-1.1.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.549676 adafruit-circuitpython-aw9523-1.1.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.549676 adafruit-circuitpython-aw9523-1.1.6/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.549676 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.549676 adafruit-circuitpython-aw9523-1.1.6/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_aw9523.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-16 17:45:55.000000 adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5966 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_constant_current_leds.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_read_all_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_set_all_outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-16 17:45:48.000000 adafruit-circuitpython-aw9523-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:45:38.000000 adafruit-circuitpython-aw9523-1.1.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:45:55.553676 adafruit-circuitpython-aw9523-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.539834 adafruit-circuitpython-aw9523-1.1.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.527833 adafruit-circuitpython-aw9523-1.1.7/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.531833 adafruit-circuitpython-aw9523-1.1.7/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.531833 adafruit-circuitpython-aw9523-1.1.7/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.535833 adafruit-circuitpython-aw9523-1.1.7/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-26 16:07:26.539834 adafruit-circuitpython-aw9523-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     9368 2023-05-26 16:07:18.000000 adafruit-circuitpython-aw9523-1.1.7/adafruit_aw9523.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.535833 adafruit-circuitpython-aw9523-1.1.7/adafruit_circuitpython_aw9523.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-26 16:07:26.000000 adafruit-circuitpython-aw9523-1.1.7/adafruit_circuitpython_aw9523.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 16:07:26.000000 adafruit-circuitpython-aw9523-1.1.7/adafruit_circuitpython_aw9523.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:07:26.000000 adafruit-circuitpython-aw9523-1.1.7/adafruit_circuitpython_aw9523.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 16:07:26.000000 adafruit-circuitpython-aw9523-1.1.7/adafruit_circuitpython_aw9523.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 16:07:26.000000 adafruit-circuitpython-aw9523-1.1.7/adafruit_circuitpython_aw9523.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.535833 adafruit-circuitpython-aw9523-1.1.7/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.535833 adafruit-circuitpython-aw9523-1.1.7/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:07:26.535833 adafruit-circuitpython-aw9523-1.1.7/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-26 16:07:18.000000 adafruit-circuitpython-aw9523-1.1.7/examples/aw9523_constant_current_leds.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-26 16:07:18.000000 adafruit-circuitpython-aw9523-1.1.7/examples/aw9523_read_all_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-26 16:07:18.000000 adafruit-circuitpython-aw9523-1.1.7/examples/aw9523_set_all_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-26 16:07:18.000000 adafruit-circuitpython-aw9523-1.1.7/examples/aw9523_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-26 16:07:18.000000 adafruit-circuitpython-aw9523-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:07:07.000000 adafruit-circuitpython-aw9523-1.1.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:07:26.539834 adafruit-circuitpython-aw9523-1.1.7/setup.cfg
```

### Comparing `adafruit-circuitpython-aw9523-1.1.6/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-aw9523-1.1.7/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/.gitignore` & `adafruit-circuitpython-aw9523-1.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/.pre-commit-config.yaml` & `adafruit-circuitpython-aw9523-1.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/.pylintrc` & `adafruit-circuitpython-aw9523-1.1.7/.pylintrc`

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

### Comparing `adafruit-circuitpython-aw9523-1.1.6/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-aw9523-1.1.7/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/LICENSE` & `adafruit-circuitpython-aw9523-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-aw9523-1.1.7/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/LICENSES/MIT.txt` & `adafruit-circuitpython-aw9523-1.1.7/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/LICENSES/Unlicense.txt` & `adafruit-circuitpython-aw9523-1.1.7/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/PKG-INFO` & `adafruit-circuitpython-aw9523-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-aw9523
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python library for AW9523 GPIO expander and LED driver
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AW9523
 Keywords: adafruit,blinka,circuitpython,micropython,aw9523,gpio,expander,led,constant-,current,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-aw9523-1.1.6/README.rst` & `adafruit-circuitpython-aw9523-1.1.7/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/adafruit_aw9523.py` & `adafruit-circuitpython-aw9523-1.1.7/adafruit_aw9523.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 
 try:
     from typing import Optional
     from busio import I2C
 except ImportError:
     pass
 
-__version__ = "1.1.6"
+__version__ = "1.1.7"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AW9523.git"
 
 _AW9523_DEFAULT_ADDR = const(0x58)
 _AW9523_REG_CHIPID = const(0x10)  # Register for hardcode chip ID
 _AW9523_REG_SOFTRESET = const(0x7F)  # Register for soft resetting
 _AW9523_REG_INPUT0 = const(0x00)  # Register for reading input values
 _AW9523_REG_OUTPUT0 = const(0x02)  # Register for writing output values
```

### Comparing `adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/PKG-INFO` & `adafruit-circuitpython-aw9523-1.1.7/adafruit_circuitpython_aw9523.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-aw9523
-Version: 1.1.6
+Version: 1.1.7
 Summary: Python library for AW9523 GPIO expander and LED driver
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_AW9523
 Keywords: adafruit,blinka,circuitpython,micropython,aw9523,gpio,expander,led,constant-,current,i2c
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-aw9523-1.1.6/adafruit_circuitpython_aw9523.egg-info/SOURCES.txt` & `adafruit-circuitpython-aw9523-1.1.7/adafruit_circuitpython_aw9523.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/docs/_static/favicon.ico` & `adafruit-circuitpython-aw9523-1.1.7/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/docs/conf.py` & `adafruit-circuitpython-aw9523-1.1.7/docs/conf.py`

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

### Comparing `adafruit-circuitpython-aw9523-1.1.6/docs/index.rst` & `adafruit-circuitpython-aw9523-1.1.7/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_constant_current_leds.py` & `adafruit-circuitpython-aw9523-1.1.7/examples/aw9523_constant_current_leds.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/examples/aw9523_simpletest.py` & `adafruit-circuitpython-aw9523-1.1.7/examples/aw9523_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-aw9523-1.1.6/pyproject.toml` & `adafruit-circuitpython-aw9523-1.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-aw9523"
 description = "Python library for AW9523 GPIO expander and LED driver"
-version = "1.1.6"
+version = "1.1.7"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_AW9523"}
 keywords = [
     "adafruit",
```

