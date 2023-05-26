# Comparing `tmp/adafruit-circuitpython-as726x-2.0.8.tar.gz` & `tmp/adafruit-circuitpython-as726x-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-as726x-2.0.8.tar", last modified: Fri Feb  4 20:39:57 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-as726x-2.0.9.tar", last modified: Tue Feb 15 20:41:14 2022, max compression
```

## Comparing `adafruit-circuitpython-as726x-2.0.8.tar` & `adafruit-circuitpython-as726x-2.0.9.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.550061 adafruit-circuitpython-as726x-2.0.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.546061 adafruit-circuitpython-as726x-2.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.546061 adafruit-circuitpython-as726x-2.0.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.546061 adafruit-circuitpython-as726x-2.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      353 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.550061 adafruit-circuitpython-as726x-2.0.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-02-04 20:39:57.550061 adafruit-circuitpython-as726x-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2423 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/README.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)    19035 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/adafruit_as726x.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.550061 adafruit-circuitpython-as726x-2.0.8/adafruit_circuitpython_as726x.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3141 2022-02-04 20:39:57.000000 adafruit-circuitpython-as726x-2.0.8/adafruit_circuitpython_as726x.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      887 2022-02-04 20:39:57.000000 adafruit-circuitpython-as726x-2.0.8/adafruit_circuitpython_as726x.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-04 20:39:57.000000 adafruit-circuitpython-as726x-2.0.8/adafruit_circuitpython_as726x.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-04 20:39:57.000000 adafruit-circuitpython-as726x-2.0.8/adafruit_circuitpython_as726x.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-04 20:39:57.000000 adafruit-circuitpython-as726x-2.0.8/adafruit_circuitpython_as726x.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.550061 adafruit-circuitpython-as726x-2.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.550061 adafruit-circuitpython-as726x-2.0.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5120 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-04 20:39:57.550061 adafruit-circuitpython-as726x-2.0.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/examples/as726x_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-04 20:39:57.550061 adafruit-circuitpython-as726x-2.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-02-04 20:39:44.000000 adafruit-circuitpython-as726x-2.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.254415 adafruit-circuitpython-as726x-2.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2424 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2714 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1231 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16243 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2394 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/README.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)    20056 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/adafruit_as726x.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/adafruit_circuitpython_as726x.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3112 2022-02-15 20:41:14.000000 adafruit-circuitpython-as726x-2.0.9/adafruit_circuitpython_as726x.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      887 2022-02-15 20:41:14.000000 adafruit-circuitpython-as726x-2.0.9/adafruit_circuitpython_as726x.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-15 20:41:14.000000 adafruit-circuitpython-as726x-2.0.9/adafruit_circuitpython_as726x.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-02-15 20:41:14.000000 adafruit-circuitpython-as726x-2.0.9/adafruit_circuitpython_as726x.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-02-15 20:41:14.000000 adafruit-circuitpython-as726x-2.0.9/adafruit_circuitpython_as726x.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      265 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5120 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1044 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/examples/as726x_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-15 20:41:14.258415 adafruit-circuitpython-as726x-2.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-02-15 20:41:05.000000 adafruit-circuitpython-as726x-2.0.9/setup.py
```

### Comparing `adafruit-circuitpython-as726x-2.0.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-as726x-2.0.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/.github/workflows/build.yml` & `adafruit-circuitpython-as726x-2.0.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/.github/workflows/release.yml` & `adafruit-circuitpython-as726x-2.0.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/.pre-commit-config.yaml` & `adafruit-circuitpython-as726x-2.0.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/.pylintrc` & `adafruit-circuitpython-as726x-2.0.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-as726x-2.0.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/LICENSE` & `adafruit-circuitpython-as726x-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-as726x-2.0.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/LICENSES/MIT.txt` & `adafruit-circuitpython-as726x-2.0.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-as726x-2.0.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/PKG-INFO` & `adafruit-circuitpython-as726x-2.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-as726x
-Version: 2.0.8
+Version: 2.0.9
 Summary: CircuitPython driver for AS726x spectral sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AS726x
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit as726x light sensor hardware micropython circuitpython
 Platform: UNKNOWN
@@ -74,20 +74,17 @@
     pip3 install adafruit-circuitpython-as726x
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/as726x/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/adafruit_CircuitPython_AS726x/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-as726x-2.0.8/README.rst` & `adafruit-circuitpython-as726x-2.0.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -55,18 +55,15 @@
     pip3 install adafruit-circuitpython-as726x
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/as726x/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/adafruit_CircuitPython_AS726x/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
-
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
```

### Comparing `adafruit-circuitpython-as726x-2.0.8/adafruit_as726x.py` & `adafruit-circuitpython-as726x-2.0.9/adafruit_as726x.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,78 +27,87 @@
 
 """
 import struct
 import time
 from adafruit_bus_device.i2c_device import I2CDevice
 from micropython import const
 
-__version__ = "0.0.0-auto.0"
-__repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_AS726x.git"
+try:
+    from typing import Tuple, Optional
 
-_AS726X_ADDRESS = const(0x49)
-
-_AS726X_HW_VERSION = const(0x00)
-_AS726X_FW_VERSION = const(0x02)
-_AS726X_CONTROL_SETUP = const(0x04)
-_AS726X_INT_T = const(0x05)
-_AS726X_DEVICE_TEMP = const(0x06)
-_AS726X_LED_CONTROL = const(0x07)
+    # This is only needed for typing
+    import busio  # pylint: disable=unused-import
+except ImportError:
+    pass
+
+
+__version__: str = "0.0.0-auto.0"
+__repo__: str = "https://github.com/adafruit/Adafruit_CircuitPython_AS726x.git"
+
+_AS726X_ADDRESS: int = const(0x49)
+
+_AS726X_HW_VERSION: int = const(0x00)
+_AS726X_FW_VERSION: int = const(0x02)
+_AS726X_CONTROL_SETUP: int = const(0x04)
+_AS726X_INT_T: int = const(0x05)
+_AS726X_DEVICE_TEMP: int = const(0x06)
+_AS726X_LED_CONTROL: int = const(0x07)
 
 # for reading sensor data
-_AS7262_V_HIGH = const(0x08)
-_AS7262_V_LOW = const(0x09)
-_AS7262_B_HIGH = const(0x0A)
-_AS7262_B_LOW = const(0x0B)
-_AS7262_G_HIGH = const(0x0C)
-_AS7262_G_LOW = const(0x0D)
-_AS7262_Y_HIGH = const(0x0E)
-_AS7262_Y_LOW = const(0x0F)
-_AS7262_O_HIGH = const(0x10)
-_AS7262_O_LOW = const(0x11)
-_AS7262_R_HIGH = const(0x12)
-_AS7262_R_LOW = const(0x13)
-
-_AS7262_V_CAL = const(0x14)
-_AS7262_B_CAL = const(0x18)
-_AS7262_G_CAL = const(0x1C)
-_AS7262_Y_CAL = const(0x20)
-_AS7262_O_CAL = const(0x24)
-_AS7262_R_CAL = const(0x28)
+_AS7262_V_HIGH: int = const(0x08)
+_AS7262_V_LOW: int = const(0x09)
+_AS7262_B_HIGH: int = const(0x0A)
+_AS7262_B_LOW: int = const(0x0B)
+_AS7262_G_HIGH: int = const(0x0C)
+_AS7262_G_LOW: int = const(0x0D)
+_AS7262_Y_HIGH: int = const(0x0E)
+_AS7262_Y_LOW: int = const(0x0F)
+_AS7262_O_HIGH: int = const(0x10)
+_AS7262_O_LOW: int = const(0x11)
+_AS7262_R_HIGH: int = const(0x12)
+_AS7262_R_LOW: int = const(0x13)
+
+_AS7262_V_CAL: int = const(0x14)
+_AS7262_B_CAL: int = const(0x18)
+_AS7262_G_CAL: int = const(0x1C)
+_AS7262_Y_CAL: int = const(0x20)
+_AS7262_O_CAL: int = const(0x24)
+_AS7262_R_CAL: int = const(0x28)
 
 # hardware registers
-_AS726X_SLAVE_STATUS_REG = const(0x00)
-_AS726X_SLAVE_WRITE_REG = const(0x01)
-_AS726X_SLAVE_READ_REG = const(0x02)
-_AS726X_SLAVE_TX_VALID = const(0x02)
-_AS726X_SLAVE_RX_VALID = const(0x01)
-
-_AS7262_VIOLET = const(0x08)
-_AS7262_BLUE = const(0x0A)
-_AS7262_GREEN = const(0x0C)
-_AS7262_YELLOW = const(0x0E)
-_AS7262_ORANGE = const(0x10)
-_AS7262_RED = const(0x12)
-_AS7262_VIOLET_CALIBRATED = const(0x14)
-_AS7262_BLUE_CALIBRATED = const(0x18)
-_AS7262_GREEN_CALIBRATED = const(0x1C)
+_AS726X_SLAVE_STATUS_REG: int = const(0x00)
+_AS726X_SLAVE_WRITE_REG: int = const(0x01)
+_AS726X_SLAVE_READ_REG: int = const(0x02)
+_AS726X_SLAVE_TX_VALID: int = const(0x02)
+_AS726X_SLAVE_RX_VALID: int = const(0x01)
+
+_AS7262_VIOLET: int = const(0x08)
+_AS7262_BLUE: int = const(0x0A)
+_AS7262_GREEN: int = const(0x0C)
+_AS7262_YELLOW: int = const(0x0E)
+_AS7262_ORANGE: int = const(0x10)
+_AS7262_RED: int = const(0x12)
+_AS7262_VIOLET_CALIBRATED: int = const(0x14)
+_AS7262_BLUE_CALIBRATED: int = const(0x18)
+_AS7262_GREEN_CALIBRATED: int = const(0x1C)
 _AS7262_YELLOW_CALIBRATED = const(0x20)
-_AS7262_ORANGE_CALIBRATED = const(0x24)
-_AS7262_RED_CALIBRATED = const(0x28)
+_AS7262_ORANGE_CALIBRATED: int = const(0x24)
+_AS7262_RED_CALIBRATED: int = const(0x28)
 
-_AS726X_NUM_CHANNELS = const(6)
+_AS726X_NUM_CHANNELS: int = const(6)
 
-_COLOR_REGS = (
+_COLOR_REGS: Tuple[int, ...] = (
     _AS7262_VIOLET,
     _AS7262_BLUE,
     _AS7262_GREEN,
     _AS7262_YELLOW,
     _AS7262_ORANGE,
     _AS7262_RED,
 )
-_COLOR_REGS_CALIBRATED = (
+_COLOR_REGS_CALIBRATED: Tuple[int, ...] = (
     _AS7262_VIOLET_CALIBRATED,
     _AS7262_BLUE_CALIBRATED,
     _AS7262_GREEN_CALIBRATED,
     _AS7262_YELLOW_CALIBRATED,
     _AS7262_ORANGE_CALIBRATED,
     _AS7262_RED_CALIBRATED,
 )
@@ -109,33 +118,33 @@
 # pylint: disable=no-else-return
 # pylint: disable=inconsistent-return-statements
 
 
 class AS726x:
     """AS726x spectral sensor base class."""
 
-    MODE_0 = 0b00
+    MODE_0: int = 0b00
     """Continuously gather samples of violet, blue, green and yellow. Orange and red are skipped
        and read zero."""
 
-    MODE_1 = 0b01
+    MODE_1: int = 0b01
     """Continuously gather samples of green, yellow, orange and red. Violet and blue are skipped
        and read zero."""
 
-    MODE_2 = 0b10  # default
+    MODE_2: int = 0b10  # default
     """Continuously gather samples of all colors"""
 
-    ONE_SHOT = 0b11
+    ONE_SHOT: int = 0b11
     """Gather a single sample of all colors and then stop"""
 
-    GAIN = (1, 3.7, 16, 64)
+    GAIN: Tuple[float, ...] = (1, 3.7, 16, 64)
 
-    INDICATOR_CURRENT_LIMITS = (1, 2, 4, 8)
+    INDICATOR_CURRENT_LIMITS: Tuple[int, ...] = (1, 2, 4, 8)
 
-    DRIVER_CURRENT_LIMITS = (12.5, 25, 50, 100)
+    DRIVER_CURRENT_LIMITS: Tuple[float, ...] = (12.5, 25, 50, 100)
 
     def __init__(self):
         self._driver_led = False
         self._indicator_led = False
         self._driver_led_current = AS726x.DRIVER_CURRENT_LIMITS.index(12.5)
         self._indicator_led_current = AS726x.INDICATOR_CURRENT_LIMITS.index(1)
         self._conversion_mode = AS726x.MODE_2
@@ -159,240 +168,240 @@
             )
 
         self.integration_time = 140
         self.conversion_mode = AS726x.MODE_2
         self.gain = 64
 
     @property
-    def driver_led(self):
+    def driver_led(self) -> bool:
         """True when the driver LED is on. False otherwise."""
         return self._driver_led
 
     @driver_led.setter
-    def driver_led(self, val):
+    def driver_led(self, val: bool) -> None:
         val = bool(val)
         if self._driver_led == val:
             return
         self._driver_led = val
         enable = self._virtual_read(_AS726X_LED_CONTROL)
         enable &= ~(0x1 << 3)
         self._virtual_write(_AS726X_LED_CONTROL, enable | (val << 3))
 
     @property
-    def indicator_led(self):
+    def indicator_led(self) -> bool:
         """True when the indicator LED is on. False otherwise."""
         return self._indicator_led
 
     @indicator_led.setter
-    def indicator_led(self, val):
+    def indicator_led(self, val: bool) -> None:
         val = bool(val)
         if self._indicator_led == val:
             return
         self._indicator_led = val
         enable = self._virtual_read(_AS726X_LED_CONTROL)
         enable &= ~(0x1)
         self._virtual_write(_AS726X_LED_CONTROL, enable | val)
 
     @property
-    def driver_led_current(self):
+    def driver_led_current(self) -> float:
         """The current limit for the driver LED in milliamps. One of:
 
         - 12.5 mA
         - 25 mA
         - 50 mA
         - 100 mA"""
         return self._driver_led_current
 
     @driver_led_current.setter
-    def driver_led_current(self, val):
+    def driver_led_current(self, val: float) -> None:
         if val not in AS726x.DRIVER_CURRENT_LIMITS:
             raise ValueError("Must be 12.5, 25, 50 or 100")
         if self._driver_led_current == val:
             return
         self._driver_led_current = val
         state = self._virtual_read(_AS726X_LED_CONTROL)
         state &= ~(0x3 << 4)
         state = state | (AS726x.DRIVER_CURRENT_LIMITS.index(val) << 4)
         self._virtual_write(_AS726X_LED_CONTROL, state)
 
     @property
-    def indicator_led_current(self):
+    def indicator_led_current(self) -> int:
         """The current limit for the indicator LED in milliamps. One of:
 
         - 1 mA
         - 2 mA
         - 4 mA
         - 8 mA"""
         return self._indicator_led_current
 
     @indicator_led_current.setter
-    def indicator_led_current(self, val):
+    def indicator_led_current(self, val: int) -> None:
         if val not in AS726x.INDICATOR_CURRENT_LIMITS:
             raise ValueError("Must be 1, 2, 4 or 8")
         if self._indicator_led_current == val:
             return
         self._indicator_led_current = val
         state = self._virtual_read(_AS726X_LED_CONTROL)
         state &= ~(0x3 << 1)
         state = state | (AS726x.INDICATOR_CURRENT_LIMITS.index(val) << 4)
         self._virtual_write(_AS726X_LED_CONTROL, state)
 
     @property
-    def conversion_mode(self):
+    def conversion_mode(self) -> int:
         """The conversion mode. One of:
 
         - `MODE_0`
         - `MODE_1`
         - `MODE_2`
         - `ONE_SHOT`"""
         return self._conversion_mode
 
     @conversion_mode.setter
-    def conversion_mode(self, val):
+    def conversion_mode(self, val: int) -> None:
         val = int(val)
         assert self.MODE_0 <= val <= self.ONE_SHOT
         if self._conversion_mode == val:
             return
         self._conversion_mode = val
         state = self._virtual_read(_AS726X_CONTROL_SETUP)
         state &= ~(val << 2)
         self._virtual_write(_AS726X_CONTROL_SETUP, state | (val << 2))
 
     @property
-    def gain(self):
+    def gain(self) -> float:
         """The gain for the sensor"""
         return self._gain
 
     @gain.setter
-    def gain(self, val):
+    def gain(self, val: float) -> None:
         if val not in AS726x.GAIN:
             raise ValueError("Must be 1, 3.7, 16 or 64")
         if self._gain == val:
             return
         self._gain = val
         state = self._virtual_read(_AS726X_CONTROL_SETUP)
         state &= ~(0x3 << 4)
         state |= AS726x.GAIN.index(val) << 4
         self._virtual_write(_AS726X_CONTROL_SETUP, state)
 
     @property
-    def integration_time(self):
+    def integration_time(self) -> float:
         """The integration time in milliseconds between 2.8 and 714 ms"""
         return self._integration_time
 
     @integration_time.setter
-    def integration_time(self, val):
+    def integration_time(self, val: float) -> None:
         val = int(val)
         if not 2.8 <= val <= 714:
             raise ValueError("Out of supported range 2.8 - 714 ms")
         if self._integration_time == val:
             return
         self._integration_time = val
         self._virtual_write(_AS726X_INT_T, int(val / 2.8))
 
-    def start_measurement(self):
+    def start_measurement(self) -> None:
         """Begin a measurement.
 
         This will set the device to One Shot mode and values will
         not change after `data_ready` until :meth:`start_measurement`
         is called again or the :meth:`conversion_mode` is changed.
         """
         state = self._virtual_read(_AS726X_CONTROL_SETUP)
         state &= ~(0x02)
         self._virtual_write(_AS726X_CONTROL_SETUP, state)
 
         self.conversion_mode = self.ONE_SHOT
 
-    def read_channel(self, channel):
+    def read_channel(self, channel: int) -> int:
         """Read an individual sensor channel"""
         return (self._virtual_read(channel) << 8) | self._virtual_read(channel + 1)
 
-    def read_calibrated_value(self, channel):
+    def read_calibrated_value(self, channel: int) -> float:
         """Read a calibrated sensor channel"""
         val = bytearray(4)
         val[0] = self._virtual_read(channel)
         val[1] = self._virtual_read(channel + 1)
         val[2] = self._virtual_read(channel + 2)
         val[3] = self._virtual_read(channel + 3)
         return struct.unpack("!f", val)[0]
 
     @property
-    def data_ready(self):
+    def data_ready(self) -> bool:
         """True if the sensor has data ready to be read, False otherwise"""
         return (self._virtual_read(_AS726X_CONTROL_SETUP) >> 1) & 0x01
 
     @property
-    def temperature(self):
+    def temperature(self) -> int:
         """The temperature of the device in Celsius"""
         return self._virtual_read(_AS726X_DEVICE_TEMP)
 
     @property
-    def violet(self):
+    def violet(self) -> float:
         """Calibrated violet (450nm) value"""
         return self.read_calibrated_value(_AS7262_VIOLET_CALIBRATED)
 
     @property
-    def blue(self):
+    def blue(self) -> float:
         """Calibrated blue (500nm) value"""
         return self.read_calibrated_value(_AS7262_BLUE_CALIBRATED)
 
     @property
-    def green(self):
+    def green(self) -> float:
         """Calibrated green (550nm) value"""
         return self.read_calibrated_value(_AS7262_GREEN_CALIBRATED)
 
     @property
-    def yellow(self):
+    def yellow(self) -> float:
         """Calibrated yellow (570nm) value"""
         return self.read_calibrated_value(_AS7262_YELLOW_CALIBRATED)
 
     @property
-    def orange(self):
+    def orange(self) -> float:
         """Calibrated orange (600nm) value"""
         return self.read_calibrated_value(_AS7262_ORANGE_CALIBRATED)
 
     @property
-    def red(self):
+    def red(self) -> float:
         """Calibrated red (650nm) value"""
         return self.read_calibrated_value(_AS7262_RED_CALIBRATED)
 
     @property
-    def raw_violet(self):
+    def raw_violet(self) -> int:
         """Raw violet (450nm) 16-bit value"""
         return self.read_channel(_AS7262_VIOLET)
 
     @property
-    def raw_blue(self):
+    def raw_blue(self) -> int:
         """Raw blue (500nm) 16-bit value"""
         return self.read_channel(_AS7262_BLUE)
 
     @property
-    def raw_green(self):
+    def raw_green(self) -> int:
         """Raw green (550nm) 16-bit value"""
         return self.read_channel(_AS7262_GREEN)
 
     @property
-    def raw_yellow(self):
+    def raw_yellow(self) -> int:
         """Raw yellow (570nm) 16-bit value"""
         return self.read_channel(_AS7262_YELLOW)
 
     @property
-    def raw_orange(self):
+    def raw_orange(self) -> int:
         """Raw orange (600nm) 16-bit value"""
         return self.read_channel(_AS7262_ORANGE)
 
     @property
-    def raw_red(self):
+    def raw_red(self) -> int:
         """Raw red (650nm) 16-bit value"""
         return self.read_channel(_AS7262_RED)
 
-    def _virtual_read(self, addr):
+    def _virtual_read(self, addr: int) -> float:
         raise NotImplementedError("Must be implemented.")
 
-    def _virtual_write(self, addr, value):
+    def _virtual_write(self, addr: int, value: float) -> None:
         raise NotImplementedError("Must be implemented.")
 
 
 class AS726x_I2C(AS726x):
     """AS726x spectral sensor via I2C.
 
     :param ~busio.I2C i2c_bus: The I2C bus the AS726x is connected to
@@ -426,36 +435,36 @@
             yellow = sensor.yellow
             orange = sensor.orange
             red = sensor.red
 
 
     """
 
-    def __init__(self, i2c_bus, address=_AS726X_ADDRESS):
+    def __init__(self, i2c_bus: busio.I2C, address: int = _AS726X_ADDRESS) -> None:
         self.i2c_device = I2CDevice(i2c_bus, address)
         super().__init__()
 
-    def _read_u8(self, command):
+    def _read_u8(self, command: int) -> int:
         """read a single byte from a specified register"""
         buf = self.buf2
         buf[0] = command
         with self.i2c_device as i2c:
             i2c.write(buf, end=1)
             i2c.readinto(buf, end=1)
         return buf[0]
 
-    def __write_u8(self, command, abyte):
+    def __write_u8(self, command: int, abyte: int) -> None:
         """Write a command and 1 byte of data to the I2C device"""
         buf = self.buf2
         buf[0] = command
         buf[1] = abyte
         with self.i2c_device as i2c:
             i2c.write(buf)
 
-    def _virtual_read(self, addr):
+    def _virtual_read(self, addr: int) -> float:
         """read a virtual register"""
         while True:
             # Read slave I2C status to see if the read buffer is ready.
             status = self._read_u8(_AS726X_SLAVE_STATUS_REG)
             if (status & _AS726X_SLAVE_TX_VALID) == 0:
                 # No inbound TX pending at slave. Okay to write now.
                 break
@@ -467,15 +476,15 @@
             if (status & _AS726X_SLAVE_RX_VALID) != 0:
                 # Read data is ready.
                 break
         # Read the data to complete the operation.
         data = self._read_u8(_AS726X_SLAVE_READ_REG)
         return data
 
-    def _virtual_write(self, addr, value):
+    def _virtual_write(self, addr: int, value: float) -> None:
         """write a virtual register"""
         while True:
             # Read slave I2C status to see if the write buffer is ready.
             status = self._read_u8(_AS726X_SLAVE_STATUS_REG)
             if (status & _AS726X_SLAVE_TX_VALID) == 0:
                 break  # No inbound TX pending at slave. Okay to write now.
         # Send the virtual register address (setting bit 7 to indicate a pending write).
@@ -523,38 +532,38 @@
             yellow = sensor.yellow
             orange = sensor.orange
             red = sensor.red
 
 
     """
 
-    def __init__(self, uart):
+    def __init__(self, uart: busio.UART) -> None:
         self._uart = uart
         self._uart.baudrate = 115200
         super().__init__()
 
-    def read_channel(self, channel):
+    def read_channel(self, channel: int) -> float:
         """Read an individual sensor channel"""
         return self._virtual_read(channel)
 
-    def read_calibrated_value(self, channel):
+    def read_calibrated_value(self, channel: int) -> float:
         """Read a calibrated sensor channel"""
         return self._virtual_read(channel)
 
-    def _uart_xfer(self, cmd):
+    def _uart_xfer(self, cmd: Optional[str]) -> str:
         self._uart.reset_input_buffer()
         cmd += "\n"
         self._uart.write(cmd.encode())
         time.sleep(0.1)
         if self._uart.in_waiting:
             resp = self._uart.read(self._uart.in_waiting)
             return resp.rstrip(b" OK\n")
         return None
 
-    def _virtual_read(self, addr):
+    def _virtual_read(self, addr: int) -> float:
         if addr == _AS726X_HW_VERSION:
             # just return what is expected
             return 0x40
         elif addr == _AS726X_DEVICE_TEMP:
             return int(self._uart_xfer("ATTEMP"))
         elif addr == _AS726X_LED_CONTROL:
             LED_IND = int(self._uart_xfer("ATLED0"))
@@ -569,15 +578,15 @@
             resp = resp.decode().split(",")
             return int(resp[_COLOR_REGS.index(addr)])
         elif addr in _COLOR_REGS_CALIBRATED:
             resp = self._uart_xfer("ATCDATA")
             resp = resp.decode().split(",")
             return float(resp[_COLOR_REGS_CALIBRATED.index(addr)])
 
-    def _virtual_write(self, addr, value):
+    def _virtual_write(self, addr: int, value: float) -> None:
         if addr == _AS726X_CONTROL_SETUP:
             # check for reset
             if (value >> 7) & 0x01:
                 self._uart.write(b"ATRST\n")
                 return
             # otherwise proceed
             GAIN = (value >> 4) & 0x03
```

### Comparing `adafruit-circuitpython-as726x-2.0.8/adafruit_circuitpython_as726x.egg-info/PKG-INFO` & `adafruit-circuitpython-as726x-2.0.9/adafruit_circuitpython_as726x.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-as726x
-Version: 2.0.8
+Version: 2.0.9
 Summary: CircuitPython driver for AS726x spectral sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_AS726x
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Keywords: adafruit as726x light sensor hardware micropython circuitpython
 Platform: UNKNOWN
@@ -74,20 +74,17 @@
     pip3 install adafruit-circuitpython-as726x
 
 Documentation
 =============
 
 API documentation for this library can be found on `Read the Docs <https://docs.circuitpython.org/projects/as726x/en/latest/>`_.
 
+For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
+
 Contributing
 ============
 
 Contributions are welcome! Please read our `Code of Conduct
 <https://github.com/adafruit/adafruit_CircuitPython_AS726x/blob/main/CODE_OF_CONDUCT.md>`_
 before contributing to help this project stay welcoming.
 
-Documentation
-=============
-
-For information on building library documentation, please check out `this guide <https://learn.adafruit.com/creating-and-sharing-a-circuitpython-library/sharing-our-docs-on-readthedocs#sphinx-5-1>`_.
-
```

### Comparing `adafruit-circuitpython-as726x-2.0.8/adafruit_circuitpython_as726x.egg-info/SOURCES.txt` & `adafruit-circuitpython-as726x-2.0.9/adafruit_circuitpython_as726x.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/docs/_static/favicon.ico` & `adafruit-circuitpython-as726x-2.0.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/docs/conf.py` & `adafruit-circuitpython-as726x-2.0.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/docs/index.rst` & `adafruit-circuitpython-as726x-2.0.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/examples/as726x_simpletest.py` & `adafruit-circuitpython-as726x-2.0.9/examples/as726x_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-as726x-2.0.8/setup.py` & `adafruit-circuitpython-as726x-2.0.9/setup.py`

 * *Files identical despite different names*

