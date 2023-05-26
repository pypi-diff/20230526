# Comparing `tmp/adafruit-circuitpython-datetime-1.2.4.tar.gz` & `tmp/adafruit-circuitpython-datetime-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-datetime-1.2.4.tar", last modified: Tue May 16 17:49:05 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-datetime-1.2.5.tar", last modified: Fri May 26 16:09:14 2023, max compression
```

## Comparing `adafruit-circuitpython-datetime-1.2.4.tar` & `adafruit-circuitpython-datetime-1.2.5.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.987288 adafruit-circuitpython-datetime-1.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSES/Python-2.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-16 17:49:05.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)    60298 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/adafruit_datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5772 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/examples/datetime_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/examples/datetime_time.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/examples/datetime_timedelta.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-16 17:48:50.000000 adafruit-circuitpython-datetime-1.2.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 17:49:05.991288 adafruit-circuitpython-datetime-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)    49197 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/tests/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-05-16 17:48:58.000000 adafruit-circuitpython-datetime-1.2.4/tests/test_time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.694663 adafruit-circuitpython-datetime-1.2.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.686663 adafruit-circuitpython-datetime-1.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13925 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/LICENSES/Python-2.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/adafruit_circuitpython_datetime.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 2023-05-26 16:09:14.000000 adafruit-circuitpython-datetime-1.2.5/adafruit_circuitpython_datetime.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-05-26 16:09:14.000000 adafruit-circuitpython-datetime-1.2.5/adafruit_circuitpython_datetime.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:09:14.000000 adafruit-circuitpython-datetime-1.2.5/adafruit_circuitpython_datetime.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 16:09:14.000000 adafruit-circuitpython-datetime-1.2.5/adafruit_circuitpython_datetime.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 16:09:14.000000 adafruit-circuitpython-datetime-1.2.5/adafruit_circuitpython_datetime.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60298 2023-05-26 16:09:07.000000 adafruit-circuitpython-datetime-1.2.5/adafruit_datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5800 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1443 2023-05-26 16:09:07.000000 adafruit-circuitpython-datetime-1.2.5/examples/datetime_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 16:09:07.000000 adafruit-circuitpython-datetime-1.2.5/examples/datetime_time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-26 16:09:07.000000 adafruit-circuitpython-datetime-1.2.5/examples/datetime_timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-26 16:09:07.000000 adafruit-circuitpython-datetime-1.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 16:08:58.000000 adafruit-circuitpython-datetime-1.2.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:09:14.694663 adafruit-circuitpython-datetime-1.2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:09:14.690663 adafruit-circuitpython-datetime-1.2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    18478 2023-05-26 16:09:07.000000 adafruit-circuitpython-datetime-1.2.5/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49197 2023-05-26 16:09:07.000000 adafruit-circuitpython-datetime-1.2.5/tests/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14919 2023-05-26 16:09:07.000000 adafruit-circuitpython-datetime-1.2.5/tests/test_time.py
```

### Comparing `adafruit-circuitpython-datetime-1.2.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-datetime-1.2.5/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/.gitignore` & `adafruit-circuitpython-datetime-1.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/.pre-commit-config.yaml` & `adafruit-circuitpython-datetime-1.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/.pylintrc` & `adafruit-circuitpython-datetime-1.2.5/.pylintrc`

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

### Comparing `adafruit-circuitpython-datetime-1.2.4/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-datetime-1.2.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/LICENSE` & `adafruit-circuitpython-datetime-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-datetime-1.2.5/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/LICENSES/MIT.txt` & `adafruit-circuitpython-datetime-1.2.5/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/LICENSES/Python-2.0.txt` & `adafruit-circuitpython-datetime-1.2.5/LICENSES/Python-2.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/LICENSES/Unlicense.txt` & `adafruit-circuitpython-datetime-1.2.5/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/PKG-INFO` & `adafruit-circuitpython-datetime-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-datetime
-Version: 1.2.4
+Version: 1.2.5
 Summary: Subset of CPython datetime module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_datetime
 Keywords: adafruit,blinka,circuitpython,micropython,datetime,date,time,timedelta,tzinfo,timezone
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-datetime-1.2.4/README.rst` & `adafruit-circuitpython-datetime-1.2.5/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/PKG-INFO` & `adafruit-circuitpython-datetime-1.2.5/adafruit_circuitpython_datetime.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-datetime
-Version: 1.2.4
+Version: 1.2.5
 Summary: Subset of CPython datetime module
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_datetime
 Keywords: adafruit,blinka,circuitpython,micropython,datetime,date,time,timedelta,tzinfo,timezone
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-datetime-1.2.4/adafruit_circuitpython_datetime.egg-info/SOURCES.txt` & `adafruit-circuitpython-datetime-1.2.5/adafruit_circuitpython_datetime.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/adafruit_datetime.py` & `adafruit-circuitpython-datetime-1.2.5/adafruit_datetime.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 from micropython import const
 
 try:
     from typing import Any, Union, Optional, Tuple, Sequence, List
 except ImportError:
     pass
 
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DateTime.git"
 
 # Constants
 MINYEAR = const(1)
 MAXYEAR = const(9999)
 _MAXORDINAL = const(3652059)
 _DI400Y = const(146097)
```

### Comparing `adafruit-circuitpython-datetime-1.2.4/docs/_static/favicon.ico` & `adafruit-circuitpython-datetime-1.2.5/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/docs/conf.py` & `adafruit-circuitpython-datetime-1.2.5/docs/conf.py`

 * *Files 4% similar despite different names*

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

### Comparing `adafruit-circuitpython-datetime-1.2.4/docs/index.rst` & `adafruit-circuitpython-datetime-1.2.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/examples/datetime_simpletest.py` & `adafruit-circuitpython-datetime-1.2.5/examples/datetime_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/examples/datetime_time.py` & `adafruit-circuitpython-datetime-1.2.5/examples/datetime_time.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/examples/datetime_timedelta.py` & `adafruit-circuitpython-datetime-1.2.5/examples/datetime_timedelta.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/pyproject.toml` & `adafruit-circuitpython-datetime-1.2.5/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-datetime"
 description = "Subset of CPython datetime module"
-version = "1.2.4"
+version = "1.2.5"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_datetime"}
 keywords = [
     "adafruit",
```

### Comparing `adafruit-circuitpython-datetime-1.2.4/tests/test_date.py` & `adafruit-circuitpython-datetime-1.2.5/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/tests/test_datetime.py` & `adafruit-circuitpython-datetime-1.2.5/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-datetime-1.2.4/tests/test_time.py` & `adafruit-circuitpython-datetime-1.2.5/tests/test_time.py`

 * *Files identical despite different names*

