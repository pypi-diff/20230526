# Comparing `tmp/adafruit-circuitpython-pct2075-1.1.8.tar.gz` & `tmp/adafruit-circuitpython-pct2075-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-pct2075-1.1.8.tar", last modified: Tue Mar  2 23:52:51 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-pct2075-1.1.9.tar", last modified: Fri Apr 16 19:38:13 2021, max compression
```

## Comparing `adafruit-circuitpython-pct2075-1.1.8.tar` & `adafruit-circuitpython-pct2075-1.1.9.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:51.296741 adafruit-circuitpython-pct2075-1.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:51.292741 adafruit-circuitpython-pct2075-1.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:51.292741 adafruit-circuitpython-pct2075-1.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      197 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6199 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:51.292741 adafruit-circuitpython-pct2075-1.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4258 2021-03-02 23:52:51.296741 adafruit-circuitpython-pct2075-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2730 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:51.296741 adafruit-circuitpython-pct2075-1.1.8/adafruit_circuitpython_pct2075.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4258 2021-03-02 23:52:50.000000 adafruit-circuitpython-pct2075-1.1.8/adafruit_circuitpython_pct2075.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      816 2021-03-02 23:52:51.000000 adafruit-circuitpython-pct2075-1.1.8/adafruit_circuitpython_pct2075.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 23:52:50.000000 adafruit-circuitpython-pct2075-1.1.8/adafruit_circuitpython_pct2075.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       81 2021-03-02 23:52:50.000000 adafruit-circuitpython-pct2075-1.1.8/adafruit_circuitpython_pct2075.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-03-02 23:52:50.000000 adafruit-circuitpython-pct2075-1.1.8/adafruit_circuitpython_pct2075.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     6135 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/adafruit_pct2075.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:51.296741 adafruit-circuitpython-pct2075-1.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:51.296741 adafruit-circuitpython-pct2075-1.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      266 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5674 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      328 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)      971 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:51.296741 adafruit-circuitpython-pct2075-1.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      592 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/examples/pct2075_high_temp_alert_example.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      317 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/examples/pct2075_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      184 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 23:52:51.296741 adafruit-circuitpython-pct2075-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2096 2021-03-02 23:52:38.000000 adafruit-circuitpython-pct2075-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 19:38:13.473050 adafruit-circuitpython-pct2075-1.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 19:38:13.469050 adafruit-circuitpython-pct2075-1.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 19:38:13.469050 adafruit-circuitpython-pct2075-1.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6199 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1104 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 19:38:13.469050 adafruit-circuitpython-pct2075-1.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4258 2021-04-16 19:38:13.473050 adafruit-circuitpython-pct2075-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2730 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 19:38:13.469050 adafruit-circuitpython-pct2075-1.1.9/adafruit_circuitpython_pct2075.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4258 2021-04-16 19:38:13.000000 adafruit-circuitpython-pct2075-1.1.9/adafruit_circuitpython_pct2075.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      816 2021-04-16 19:38:13.000000 adafruit-circuitpython-pct2075-1.1.9/adafruit_circuitpython_pct2075.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-16 19:38:13.000000 adafruit-circuitpython-pct2075-1.1.9/adafruit_circuitpython_pct2075.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-04-16 19:38:13.000000 adafruit-circuitpython-pct2075-1.1.9/adafruit_circuitpython_pct2075.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-04-16 19:38:13.000000 adafruit-circuitpython-pct2075-1.1.9/adafruit_circuitpython_pct2075.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     6992 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/adafruit_pct2075.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 19:38:13.473050 adafruit-circuitpython-pct2075-1.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 19:38:13.473050 adafruit-circuitpython-pct2075-1.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      266 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5674 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      461 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)      971 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-16 19:38:13.473050 adafruit-circuitpython-pct2075-1.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      592 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/examples/pct2075_high_temp_alert_example.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      317 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/examples/pct2075_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-16 19:38:13.473050 adafruit-circuitpython-pct2075-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2096 2021-04-16 19:37:58.000000 adafruit-circuitpython-pct2075-1.1.9/setup.py
```

### Comparing `adafruit-circuitpython-pct2075-1.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-pct2075-1.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-pct2075-1.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-pct2075-1.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/.pylintrc` & `adafruit-circuitpython-pct2075-1.1.9/.pylintrc`

 * *Files 1% similar despite different names*

```diff
@@ -18,16 +18,15 @@
 ignore-patterns=
 
 # Python code to execute, usually for sys.path manipulation such as
 # pygtk.require().
 #init-hook=
 
 # Use multiple processes to speed up Pylint.
-# jobs=1
-jobs=2
+jobs=1
 
 # List of plugins (as comma separated values of python modules names) to load,
 # usually to register additional checkers.
 load-plugins=
 
 # Pickle collected data for later comparisons.
 persistent=yes
@@ -249,15 +248,15 @@
 # Ignore docstrings when computing similarities.
 ignore-docstrings=yes
 
 # Ignore imports when computing similarities.
 ignore-imports=yes
 
 # Minimum lines number of a similarity.
-min-similarity-lines=4
+min-similarity-lines=12
 
 
 [BASIC]
 
 # Naming hint for argument names
 argument-name-hint=(([a-z][a-z0-9_]{2,30})|(_[a-z0-9_]*))$
```

### Comparing `adafruit-circuitpython-pct2075-1.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-pct2075-1.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/LICENSE` & `adafruit-circuitpython-pct2075-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-pct2075-1.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-pct2075-1.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-pct2075-1.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/PKG-INFO` & `adafruit-circuitpython-pct2075-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pct2075
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for the NXP PCT2075 Digital Temperature Sensor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PCT2075
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-pct2075-1.1.8/README.rst` & `adafruit-circuitpython-pct2075-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/adafruit_circuitpython_pct2075.egg-info/PKG-INFO` & `adafruit-circuitpython-pct2075-1.1.9/adafruit_circuitpython_pct2075.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-pct2075
-Version: 1.1.8
+Version: 1.1.9
 Summary: CircuitPython library for the NXP PCT2075 Digital Temperature Sensor
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_PCT2075
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: Introduction
         ============
```

### Comparing `adafruit-circuitpython-pct2075-1.1.8/adafruit_circuitpython_pct2075.egg-info/SOURCES.txt` & `adafruit-circuitpython-pct2075-1.1.9/adafruit_circuitpython_pct2075.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/adafruit_pct2075.py` & `adafruit-circuitpython-pct2075-1.1.9/adafruit_pct2075.py`

 * *Files 18% similar despite different names*

```diff
@@ -12,20 +12,20 @@
 * Author(s): Bryan Siepert
 
 Implementation Notes
 --------------------
 
 **Hardware:**
 
-* Adafruit PCT2075 Breakout: https://www.adafruit.com/products/4369
+* Adafruit PCT2075 Temperature Sensor Breakout: https://www.adafruit.com/products/4369
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
-  https://github.com/adafruit/circuitpython/releases
+  https://circuitpython.org/downloads
 
 
 
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 * Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 
@@ -63,28 +63,55 @@
 
 
 # pylint: enable=too-few-public-methods
 
 
 class PCT2075:
     """Driver for the PCT2075 Digital Temperature Sensor and Thermal Watchdog.
+
     :param ~busio.I2C i2c_bus: The I2C bus the PCT2075 is connected to.
-    :param address: The I2C device address for the sensor. Default is ``0x37``.
+    :param address: The I2C device address for the sensor. Default is :const:`0x37`
+
+    **Quickstart: Importing and using the PCT2075 temperature sensor**
+
+        Here is one way of importing the `PCT2075` class so you can use it with the name ``pct``.
+        First you will need to import the libraries to use the sensor
+
+        .. code-block:: python
+
+            import busio
+            import board
+            import adafruit_pct2075
+
+        Once this is done you can define your `busio.I2C` object and define your sensor object
+
+        .. code-block:: python
+
+            i2c = busio.I2C(board.SCL, board.SDA)
+            pct = adafruit_pct2075.PCT2075(i2c)
+
+        Now you have access to the temperature using the attribute :attr:`temperature`.
+
+        .. code-block:: python
+
+            temperature = pct.temperature
+
     """
 
     def __init__(self, i2c_bus, address=PCT2075_DEFAULT_ADDRESS):
         self.i2c_device = i2cdevice.I2CDevice(i2c_bus, address)
 
     _temperature = ROUnaryStruct(PCT2075_REGISTER_TEMP, ">h")
     mode = RWBit(PCT2075_REGISTER_CONFIG, 1, register_width=1)
-    """Sets the alert mode. In comparitor mode, the sensor acts like a thermostat and will activate
+    """Sets the alert mode. In comparator mode, the sensor acts like a thermostat and will activate
     the INT pin according to `high_temp_active_high` when an alert is triggered. The INT pin will be
-    deactiveated when the temperature falls below `temperature_hysteresis`. In interrupt mode the
-    INT pin is activated once when a temperature fault is detected, and once more when the
-    temperature falls below `temperature_hysteresis`. In interrupt mode, the alert is cleared by
+    deactivated when the temperature falls below :attr:`temperature_hysteresis`.
+    In interrupt mode the INT pin is activated once when a temperature fault
+    is detected, and once more when the     temperature falls below
+    :attr:`temperature_hysteresis`. In interrupt mode, the alert is cleared by
     reading a property"""
 
     shutdown = RWBit(PCT2075_REGISTER_CONFIG, 0, 1)
     """Set to True to turn off the temperature measurement circuitry in the sensor. While shut down
     the configurations properties can still be read or written but the temperature will not be
     measured"""
     _fault_queue_length = RWBits(2, PCT2075_REGISTER_CONFIG, 3, register_width=1)
@@ -93,32 +120,36 @@
     _idle_time = RWBits(5, PCT2075_REGISTER_TIDLE, 0, register_width=1)
     high_temp_active_high = RWBit(PCT2075_REGISTER_CONFIG, 2, register_width=1)
     """Sets the alert polarity. When False the INT pin will be tied to ground when an alert is
     triggered. If set to True it will be disconnected from ground when an alert is triggered."""
 
     @property
     def temperature(self):
-        """Returns the current temperature in degress celsius. Resolution is 0.125 degrees C"""
+        """Returns the current temperature in degrees Celsius.
+        Resolution is 0.125 degrees Celsius"""
         return (self._temperature >> 5) * 0.125
 
     @property
     def high_temperature_threshold(self):
         """The temperature in degrees celsius that will trigger an alert on the INT pin if it is
-        exceeded. Resolution is 0.5 degrees C."""
+        exceeded. Resolution is 0.5 degrees Celsius"""
         return (self._high_temperature_threshold >> 7) * 0.5
 
     @high_temperature_threshold.setter
     def high_temperature_threshold(self, value):
         self._high_temperature_threshold = int(value * 2) << 7
 
     @property
     def temperature_hysteresis(self):
-        """The temperature hysteresis value defines the bottom of the temperature range in degrees
-        C in which the temperature is still considered high". `temperature_hysteresis` must be
-        lower than `high_temperature_threshold`. Resolution is 0.5 degrees C.
+        """The temperature hysteresis value defines the bottom
+        of the temperature range in degrees Celsius in which
+        the temperature is still considered high.
+        :attr:`temperature_hysteresis` must be lower than
+        :attr:`high_temperature_threshold`.
+        Resolution is 0.5 degrees Celsius
         """
         return (self._temp_hysteresis >> 7) * 0.5
 
     @temperature_hysteresis.setter
     def temperature_hysteresis(self, value):
         if value >= self.high_temperature_threshold:
             raise ValueError(
@@ -126,16 +157,16 @@
             )
         self._temp_hysteresis = int(value * 2) << 7
 
     @property
     def faults_to_alert(self):
         """The number of consecutive high temperature faults required to raise an alert. An fault
         is tripped each time the sensor measures the temperature to be greater than
-        `high_temperature_threshold`. The rate at which the sensor measures the temperature
-        is defined by `delay_between_measurements`.
+        :attr:`high_temperature_threshold`. The rate at which the sensor measures the temperature
+        is defined by :attr:`delay_between_measurements`.
         """
 
         return self._fault_queue_length
 
     @faults_to_alert.setter
     def faults_to_alert(self, value):
         if value > 4 or value < 1:
```

### Comparing `adafruit-circuitpython-pct2075-1.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-pct2075-1.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/docs/conf.py` & `adafruit-circuitpython-pct2075-1.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/docs/index.rst` & `adafruit-circuitpython-pct2075-1.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/examples/pct2075_high_temp_alert_example.py` & `adafruit-circuitpython-pct2075-1.1.9/examples/pct2075_high_temp_alert_example.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-pct2075-1.1.8/setup.py` & `adafruit-circuitpython-pct2075-1.1.9/setup.py`

 * *Files identical despite different names*

