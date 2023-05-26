# Comparing `tmp/adafruit-circuitpython-si4713-1.3.8.tar.gz` & `tmp/adafruit-circuitpython-si4713-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-si4713-1.3.8.tar", last modified: Mon Aug 22 18:47:50 2022, max compression
+gzip compressed data, was "adafruit-circuitpython-si4713-1.3.9.tar", last modified: Fri Aug 26 02:24:38 2022, max compression
```

## Comparing `adafruit-circuitpython-si4713-1.3.8.tar` & `adafruit-circuitpython-si4713-1.3.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.525933 adafruit-circuitpython-si4713-1.3.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.521932 adafruit-circuitpython-si4713-1.3.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.521932 adafruit-circuitpython-si4713-1.3.8/.github/PULL_REQUEST_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.521932 adafruit-circuitpython-si4713-1.3.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/.github/workflows/failure-help-text.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.525933 adafruit-circuitpython-si4713-1.3.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-08-22 18:47:50.525933 adafruit-circuitpython-si4713-1.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.525933 adafruit-circuitpython-si4713-1.3.8/adafruit_circuitpython_si4713.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-08-22 18:47:50.000000 adafruit-circuitpython-si4713-1.3.8/adafruit_circuitpython_si4713.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      919 2022-08-22 18:47:50.000000 adafruit-circuitpython-si4713-1.3.8/adafruit_circuitpython_si4713.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 18:47:50.000000 adafruit-circuitpython-si4713-1.3.8/adafruit_circuitpython_si4713.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-22 18:47:50.000000 adafruit-circuitpython-si4713-1.3.8/adafruit_circuitpython_si4713.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-22 18:47:50.000000 adafruit-circuitpython-si4713-1.3.8/adafruit_circuitpython_si4713.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    23256 2022-08-22 18:47:41.000000 adafruit-circuitpython-si4713-1.3.8/adafruit_si4713.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.525933 adafruit-circuitpython-si4713-1.3.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.525933 adafruit-circuitpython-si4713-1.3.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5286 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/index.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 18:47:50.525933 adafruit-circuitpython-si4713-1.3.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-08-22 18:47:41.000000 adafruit-circuitpython-si4713-1.3.8/examples/si4713_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/optional_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-08-22 18:47:41.000000 adafruit-circuitpython-si4713-1.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-22 18:47:29.000000 adafruit-circuitpython-si4713-1.3.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-22 18:47:50.525933 adafruit-circuitpython-si4713-1.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.186913 adafruit-circuitpython-si4713-1.3.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.178913 adafruit-circuitpython-si4713-1.3.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.182913 adafruit-circuitpython-si4713-1.3.9/.github/PULL_REQUEST_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      880 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.182913 adafruit-circuitpython-si4713-1.3.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2535 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/.github/workflows/failure-help-text.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2966 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1648 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1239 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16248 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.182913 adafruit-circuitpython-si4713-1.3.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-08-26 02:24:38.186913 adafruit-circuitpython-si4713-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2586 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.182913 adafruit-circuitpython-si4713-1.3.9/adafruit_circuitpython_si4713.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3352 2022-08-26 02:24:38.000000 adafruit-circuitpython-si4713-1.3.9/adafruit_circuitpython_si4713.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      919 2022-08-26 02:24:38.000000 adafruit-circuitpython-si4713-1.3.9/adafruit_circuitpython_si4713.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-26 02:24:38.000000 adafruit-circuitpython-si4713-1.3.9/adafruit_circuitpython_si4713.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-08-26 02:24:38.000000 adafruit-circuitpython-si4713-1.3.9/adafruit_circuitpython_si4713.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-26 02:24:38.000000 adafruit-circuitpython-si4713-1.3.9/adafruit_circuitpython_si4713.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    23256 2022-08-26 02:24:29.000000 adafruit-circuitpython-si4713-1.3.9/adafruit_si4713.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.182913 adafruit-circuitpython-si4713-1.3.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.186913 adafruit-circuitpython-si4713-1.3.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      125 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5506 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      186 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/index.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-26 02:24:38.186913 adafruit-circuitpython-si4713-1.3.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     3247 2022-08-26 02:24:29.000000 adafruit-circuitpython-si4713-1.3.9/examples/si4713_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/optional_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1233 2022-08-26 02:24:29.000000 adafruit-circuitpython-si4713-1.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-08-26 02:24:20.000000 adafruit-circuitpython-si4713-1.3.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-26 02:24:38.186913 adafruit-circuitpython-si4713-1.3.9/setup.cfg
```

### Comparing `adafruit-circuitpython-si4713-1.3.8/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md` & `adafruit-circuitpython-si4713-1.3.9/.github/PULL_REQUEST_TEMPLATE/adafruit_circuitpython_pr.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/.github/workflows/build.yml` & `adafruit-circuitpython-si4713-1.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/.github/workflows/release.yml` & `adafruit-circuitpython-si4713-1.3.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/.gitignore` & `adafruit-circuitpython-si4713-1.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/.pre-commit-config.yaml` & `adafruit-circuitpython-si4713-1.3.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/.pylintrc` & `adafruit-circuitpython-si4713-1.3.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-si4713-1.3.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/LICENSE` & `adafruit-circuitpython-si4713-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-si4713-1.3.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/LICENSES/MIT.txt` & `adafruit-circuitpython-si4713-1.3.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-si4713-1.3.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/PKG-INFO` & `adafruit-circuitpython-si4713-1.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si4713
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for SI4713 FM RDS transmitter.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI4713
 Keywords: adafruit,si4713,fm,rds,transmitter,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si4713-1.3.8/README.rst` & `adafruit-circuitpython-si4713-1.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/adafruit_circuitpython_si4713.egg-info/PKG-INFO` & `adafruit-circuitpython-si4713-1.3.9/adafruit_circuitpython_si4713.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-si4713
-Version: 1.3.8
+Version: 1.3.9
 Summary: CircuitPython library for SI4713 FM RDS transmitter.
 Author-email: Adafruit Industries <circuitpython@adafruit.com>
 License: MIT
 Project-URL: Homepage, https://github.com/adafruit/Adafruit_CircuitPython_SI4713
 Keywords: adafruit,si4713,fm,rds,transmitter,breakout,hardware,micropython,circuitpython
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
```

### Comparing `adafruit-circuitpython-si4713-1.3.8/adafruit_circuitpython_si4713.egg-info/SOURCES.txt` & `adafruit-circuitpython-si4713-1.3.9/adafruit_circuitpython_si4713.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/adafruit_si4713.py` & `adafruit-circuitpython-si4713-1.3.9/adafruit_si4713.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     import struct
 except ImportError:
     import ustruct as struct
 
 from adafruit_bus_device import i2c_device
 
 
-__version__ = "1.3.8"
+__version__ = "1.3.9"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_SI4713.git"
 
 
 # Internal constants:
 _SI4710_ADDR0 = const(0x11)  # if SEN is = const(low)
 _SI4710_ADDR1 = const(0x63)  # if SEN is high, default
 _SI4710_STATUS_CTS = const(0x80)
```

### Comparing `adafruit-circuitpython-si4713-1.3.8/docs/_static/favicon.ico` & `adafruit-circuitpython-si4713-1.3.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/docs/conf.py` & `adafruit-circuitpython-si4713-1.3.9/docs/conf.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 #
 # SPDX-License-Identifier: MIT
 
 import os
 import sys
+import datetime
 
 sys.path.insert(0, os.path.abspath(".."))
 
 # -- General configuration ------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
@@ -40,15 +41,22 @@
 source_suffix = ".rst"
 
 # The master toctree document.
 master_doc = "index"
 
 # General information about the project.
 project = "Adafruit SI4713 Library"
-copyright = "2017 Tony DiCola"
+creation_year = "2017"
+current_year = str(datetime.datetime.now().year)
+year_duration = (
+    current_year
+    if current_year == creation_year
+    else creation_year + " - " + current_year
+)
+copyright = year_duration + " Tony DiCola"
 author = "Tony DiCola"
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
```

### Comparing `adafruit-circuitpython-si4713-1.3.8/docs/index.rst` & `adafruit-circuitpython-si4713-1.3.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/examples/si4713_simpletest.py` & `adafruit-circuitpython-si4713-1.3.9/examples/si4713_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-si4713-1.3.8/pyproject.toml` & `adafruit-circuitpython-si4713-1.3.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     "wheel",
     "setuptools-scm",
 ]
 
 [project]
 name = "adafruit-circuitpython-si4713"
 description = "CircuitPython library for SI4713 FM RDS transmitter."
-version = "1.3.8"
+version = "1.3.9"
 readme = "README.rst"
 authors = [
     {name = "Adafruit Industries", email = "circuitpython@adafruit.com"}
 ]
 urls = {Homepage = "https://github.com/adafruit/Adafruit_CircuitPython_SI4713"}
 keywords = [
     "adafruit",
```

