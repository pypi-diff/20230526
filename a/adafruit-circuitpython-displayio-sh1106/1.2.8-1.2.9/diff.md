# Comparing `tmp/adafruit-circuitpython-displayio-sh1106-1.2.8.tar.gz` & `tmp/adafruit-circuitpython-displayio-sh1106-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-displayio-sh1106-1.2.8.tar", last modified: Thu Aug 25 19:31:54 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-displayio-sh1106-1.2.9.tar", last modified: Sat Sep  3 20:37:18 2022, max compression
```

## Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8.tar` & `adafruit-circuitpython-displayio-sh1106-1.2.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.192463 adafruit-circuitpython-displayio-sh1106-1.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.192463 adafruit-circuitpython-displayio-sh1106-1.2.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_circuitpython_displayio_sh1106.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-08-25 19:31:54.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_circuitpython_displayio_sh1106.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      989 2022-08-25 19:31:54.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_circuitpython_displayio_sh1106.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-25 19:31:54.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_circuitpython_displayio_sh1106.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-08-25 19:31:54.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_circuitpython_displayio_sh1106.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-08-25 19:31:54.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_circuitpython_displayio_sh1106.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3790 2022-08-25 19:31:43.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_displayio_sh1106.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      982 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      183 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-08-25 19:31:43.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/examples/displayio_sh1106_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-08-25 19:31:43.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-25 19:31:33.000000 adafruit-circuitpython-displayio-sh1106-1.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-25 19:31:54.196463 adafruit-circuitpython-displayio-sh1106-1.2.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.423205 adafruit-circuitpython-displayio-sh1106-1.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16292 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6192 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1098 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4089 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_circuitpython_displayio_sh1106.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4890 2022-09-03 20:37:18.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_circuitpython_displayio_sh1106.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      989 2022-09-03 20:37:18.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_circuitpython_displayio_sh1106.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-03 20:37:18.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_circuitpython_displayio_sh1106.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-09-03 20:37:18.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_circuitpython_displayio_sh1106.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       26 2022-09-03 20:37:18.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_circuitpython_displayio_sh1106.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3842 2022-09-03 20:37:10.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_displayio_sh1106.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5975 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      982 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      183 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-09-03 20:37:10.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/examples/displayio_sh1106_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1278 2022-09-03 20:37:10.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-09-03 20:37:02.000000 adafruit-circuitpython-displayio-sh1106-1.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-03 20:37:18.427206 adafruit-circuitpython-displayio-sh1106-1.2.9/setup.cfg
```

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-displayio-sh1106-1.2.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-displayio-sh1106-1.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-displayio-sh1106-1.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/.gitignore` & `adafruit-circuitpython-displayio-sh1106-1.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-displayio-sh1106-1.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/.pylintrc` & `adafruit-circuitpython-displayio-sh1106-1.2.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-displayio-sh1106-1.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSE` & `adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-displayio-sh1106-1.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/PKG-INFO` & `adafruit-circuitpython-displayio-sh1106-1.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-sh1106
-Version: 1.2.8
+Version: 1.2.9
 Summary: DisplayIO compatible library for SH1106 OLED displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1106.git
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_sh1106,displayio,oled,sh1106,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/README.rst` & `adafruit-circuitpython-displayio-sh1106-1.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_circuitpython_displayio_sh1106.egg-info/PKG-INFO` & `adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_circuitpython_displayio_sh1106.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-displayio-sh1106
-Version: 1.2.8
+Version: 1.2.9
 Summary: DisplayIO compatible library for SH1106 OLED displays
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1106.git
 Keywords: adafruit,blinka,circuitpython,micropython,displayio_sh1106,displayio,oled,sh1106,display
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_circuitpython_displayio_sh1106.egg-info/SOURCES.txt` & `adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_circuitpython_displayio_sh1106.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/adafruit_displayio_sh1106.py` & `adafruit-circuitpython-displayio-sh1106-1.2.9/adafruit_displayio_sh1106.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   https://github.com/adafruit/circuitpython/releases
 
 """
 
 # imports
 import displayio
 
-__version__ = "1.2.8"
+__version__ = "1.2.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1106.git"
 
 
 # Sequence from sh1106 framebuf driver formatted for displayio init
 _INIT_SEQUENCE = (
     b"\xae\x00"  # display off, sleep mode
     b"\xd5\x01\x80"  # divide ratio/oscillator: divide by 2, fOsc (POR)
@@ -58,15 +58,15 @@
 
     :param bus: The bus that the display is connected to.
     :param int width: The width of the display. Maximum of 132
     :param int height: The height of the display. Maximum of 64
     :param int rotation: The rotation of the display. 0, 90, 180 or 270.
     """
 
-    def __init__(self, bus, **kwargs):
+    def __init__(self, bus: displayio.Fourwire, **kwargs) -> None:
         init_sequence = bytearray(_INIT_SEQUENCE)
         super().__init__(
             bus,
             init_sequence,
             **kwargs,
             color_depth=1,
             grayscale=True,
@@ -79,37 +79,37 @@
             #                upper column command = 0x10 - 0x17
             #                set page address     = 0xB0 - 0xBF (16 pages)
             SH1107_addressing=True,
         )
         self._is_awake = True  # Display starts in active state (_INIT_SEQUENCE)
 
     @property
-    def is_awake(self):
+    def is_awake(self) -> bool:
         """
         The power state of the display. (read-only)
 
         `True` if the display is active, `False` if in sleep mode.
         """
         return self._is_awake
 
-    def sleep(self):
+    def sleep(self) -> None:
         """
         Put display into sleep mode. The display uses < 5uA in sleep mode.
 
         Sleep mode does the following:
 
             1) Stops the oscillator and DC-DC circuits
             2) Stops the OLED drive
             3) Remembers display data and operation mode active prior to sleeping
             4) The MP can access (update) the built-in display RAM
         """
         if self._is_awake:
             self.bus.send(0xAE, b"")  # 0xAE = display off, sleep mode
             self._is_awake = False
 
-    def wake(self):
+    def wake(self) -> None:
         """
         Wake display from sleep mode
         """
         if not self._is_awake:
             self.bus.send(0xAF, b"")  # 0xAF = display on
             self._is_awake = True
```

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-displayio-sh1106-1.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/docs/conf.py` & `adafruit-circuitpython-displayio-sh1106-1.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/docs/index.rst` & `adafruit-circuitpython-displayio-sh1106-1.2.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/examples/displayio_sh1106_simpletest.py` & `adafruit-circuitpython-displayio-sh1106-1.2.9/examples/displayio_sh1106_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-displayio-sh1106-1.2.8/pyproject.toml` & `adafruit-circuitpython-displayio-sh1106-1.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-displayio-sh1106"
 description = "DisplayIO compatible library for SH1106 OLED displays"
-version = "1.2.8"
+version = "1.2.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_DisplayIO_SH1106.git"}
 keywords = [
     "adafruit",
```

