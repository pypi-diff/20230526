# Comparing `tmp/adafruit-circuitpython-neotrellis-1.3.3.tar.gz` & `tmp/adafruit-circuitpython-neotrellis-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-neotrellis-1.3.3.tar", last modified: Thu May 18 15:15:24 2023, max compression
+gzip compressed data, was "adafruit-circuitpython-neotrellis-1.3.4.tar", last modified: Fri May 26 16:12:02 2023, max compression
```

## Comparing `adafruit-circuitpython-neotrellis-1.3.3.tar` & `adafruit-circuitpython-neotrellis-1.3.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.428101 adafruit-circuitpython-neotrellis-1.3.3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.416101 adafruit-circuitpython-neotrellis-1.3.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.420101 adafruit-circuitpython-neotrellis-1.3.3/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.420101 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/release_gh.yml
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.github/workflows/release_pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    13069 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.420101 adafruit-circuitpython-neotrellis-1.3.3/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-18 15:15:24.428101 adafruit-circuitpython-neotrellis-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.424101 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-18 15:15:24.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.424101 adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/multitrellis.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3621 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/neotrellis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.424101 adafruit-circuitpython-neotrellis-1.3.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.424101 adafruit-circuitpython-neotrellis-1.3.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     5931 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 15:15:24.428101 adafruit-circuitpython-neotrellis-1.3.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/examples/neotrellis_multitrellis_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/examples/neotrellis_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-18 15:15:14.000000 adafruit-circuitpython-neotrellis-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-18 15:14:58.000000 adafruit-circuitpython-neotrellis-1.3.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 15:15:24.428101 adafruit-circuitpython-neotrellis-1.3.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.125518 adafruit-circuitpython-neotrellis-1.3.4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.113518 adafruit-circuitpython-neotrellis-1.3.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.117518 adafruit-circuitpython-neotrellis-1.3.4/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.117518 adafruit-circuitpython-neotrellis-1.3.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.github/workflows/release_gh.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.github/workflows/release_pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    13078 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.117518 adafruit-circuitpython-neotrellis-1.3.4/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (123)    16814 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-26 16:12:02.125518 adafruit-circuitpython-neotrellis-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.121518 adafruit-circuitpython-neotrellis-1.3.4/adafruit_circuitpython_neotrellis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3584 2023-05-26 16:12:02.000000 adafruit-circuitpython-neotrellis-1.3.4/adafruit_circuitpython_neotrellis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-26 16:12:02.000000 adafruit-circuitpython-neotrellis-1.3.4/adafruit_circuitpython_neotrellis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:12:02.000000 adafruit-circuitpython-neotrellis-1.3.4/adafruit_circuitpython_neotrellis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 16:12:02.000000 adafruit-circuitpython-neotrellis-1.3.4/adafruit_circuitpython_neotrellis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 16:12:02.000000 adafruit-circuitpython-neotrellis-1.3.4/adafruit_circuitpython_neotrellis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.121518 adafruit-circuitpython-neotrellis-1.3.4/adafruit_neotrellis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 16:11:52.000000 adafruit-circuitpython-neotrellis-1.3.4/adafruit_neotrellis/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4259 2023-05-26 16:11:52.000000 adafruit-circuitpython-neotrellis-1.3.4/adafruit_neotrellis/multitrellis.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3621 2023-05-26 16:11:52.000000 adafruit-circuitpython-neotrellis-1.3.4/adafruit_neotrellis/neotrellis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.121518 adafruit-circuitpython-neotrellis-1.3.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.121518 adafruit-circuitpython-neotrellis-1.3.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:12:02.125518 adafruit-circuitpython-neotrellis-1.3.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-05-26 16:11:52.000000 adafruit-circuitpython-neotrellis-1.3.4/examples/neotrellis_multitrellis_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-26 16:11:52.000000 adafruit-circuitpython-neotrellis-1.3.4/examples/neotrellis_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-26 16:11:52.000000 adafruit-circuitpython-neotrellis-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 16:11:39.000000 adafruit-circuitpython-neotrellis-1.3.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:12:02.125518 adafruit-circuitpython-neotrellis-1.3.4/setup.cfg
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-neotrellis-1.3.4/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/.gitignore` & `adafruit-circuitpython-neotrellis-1.3.4/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/.pre-commit-config.yaml` & `adafruit-circuitpython-neotrellis-1.3.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/.pylintrc` & `adafruit-circuitpython-neotrellis-1.3.4/.pylintrc`

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

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-neotrellis-1.3.4/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/LICENSE` & `adafruit-circuitpython-neotrellis-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-neotrellis-1.3.4/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/LICENSES/MIT.txt` & `adafruit-circuitpython-neotrellis-1.3.4/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/LICENSES/Unlicense.txt` & `adafruit-circuitpython-neotrellis-1.3.4/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/PKG-INFO` & `adafruit-circuitpython-neotrellis-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neotrellis
-Version: 1.3.3
+Version: 1.3.4
 Summary: CircuitPython library for using Adafruit NeoTrellis.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoTrellis
 Keywords: adafruit,neotrellis,neopixel,trellis,led,rgbsensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/README.rst` & `adafruit-circuitpython-neotrellis-1.3.4/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/PKG-INFO` & `adafruit-circuitpython-neotrellis-1.3.4/adafruit_circuitpython_neotrellis.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-neotrellis
-Version: 1.3.3
+Version: 1.3.4
 Summary: CircuitPython library for using Adafruit NeoTrellis.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_NeoTrellis
 Keywords: adafruit,neotrellis,neopixel,trellis,led,rgbsensor,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/adafruit_circuitpython_neotrellis.egg-info/SOURCES.txt` & `adafruit-circuitpython-neotrellis-1.3.4/adafruit_circuitpython_neotrellis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/multitrellis.py` & `adafruit-circuitpython-neotrellis-1.3.4/adafruit_neotrellis/multitrellis.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit Seesaw CircuitPython library
   https://github.com/adafruit/Adafruit_CircuitPython_seesaw/releases
 """
 
-__version__ = "1.3.3"
+__version__ = "1.3.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_neotrellis.git"
 
 
 from time import sleep
 from micropython import const
 from adafruit_seesaw.keypad import KeyEvent
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/adafruit_neotrellis/neotrellis.py` & `adafruit-circuitpython-neotrellis-1.3.4/adafruit_neotrellis/neotrellis.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 * Adafruit CircuitPython firmware for the supported boards:
   https://github.com/adafruit/circuitpython/releases
 
 * Adafruit Seesaw CircuitPython library
   https://github.com/adafruit/Adafruit_CircuitPython_seesaw/releases
 """
 
-__version__ = "1.3.3"
+__version__ = "1.3.4"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_neotrellis.git"
 
 from time import sleep
 from micropython import const
 from adafruit_seesaw.keypad import Keypad, KeyEvent
 from adafruit_seesaw.neopixel import NeoPixel, GRB
```

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/docs/_static/favicon.ico` & `adafruit-circuitpython-neotrellis-1.3.4/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/docs/conf.py` & `adafruit-circuitpython-neotrellis-1.3.4/docs/conf.py`

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

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/docs/index.rst` & `adafruit-circuitpython-neotrellis-1.3.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/examples/neotrellis_multitrellis_simpletest.py` & `adafruit-circuitpython-neotrellis-1.3.4/examples/neotrellis_multitrellis_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/examples/neotrellis_simpletest.py` & `adafruit-circuitpython-neotrellis-1.3.4/examples/neotrellis_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-neotrellis-1.3.3/pyproject.toml` & `adafruit-circuitpython-neotrellis-1.3.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-neotrellis"
 description = "CircuitPython library for using Adafruit NeoTrellis."
-version = "1.3.3"
+version = "1.3.4"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_NeoTrellis"}
 keywords = [
     "adafruit",
```

