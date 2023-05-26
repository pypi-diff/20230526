# Comparing `tmp/adafruit-circuitpython-max31865-2.2.8.tar.gz` & `tmp/adafruit-circuitpython-max31865-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-max31865-2.2.8.tar", last modified: Tue Mar  2 23:50:21 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-max31865-2.2.9.tar", last modified: Mon Apr 26 20:23:31 2021, max compression
```

## Comparing `adafruit-circuitpython-max31865-2.2.8.tar` & `adafruit-circuitpython-max31865-2.2.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:21.020817 adafruit-circuitpython-max31865-2.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:21.016817 adafruit-circuitpython-max31865-2.2.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:21.016817 adafruit-circuitpython-max31865-2.2.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      189 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1102 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:21.016817 adafruit-circuitpython-max31865-2.2.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     3678 2021-03-02 23:50:21.020817 adafruit-circuitpython-max31865-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2276 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:21.020817 adafruit-circuitpython-max31865-2.2.8/adafruit_circuitpython_max31865.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3678 2021-03-02 23:50:20.000000 adafruit-circuitpython-max31865-2.2.8/adafruit_circuitpython_max31865.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      779 2021-03-02 23:50:20.000000 adafruit-circuitpython-max31865-2.2.8/adafruit_circuitpython_max31865.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 23:50:20.000000 adafruit-circuitpython-max31865-2.2.8/adafruit_circuitpython_max31865.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       49 2021-03-02 23:50:20.000000 adafruit-circuitpython-max31865-2.2.8/adafruit_circuitpython_max31865.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       18 2021-03-02 23:50:20.000000 adafruit-circuitpython-max31865-2.2.8/adafruit_circuitpython_max31865.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     9106 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/adafruit_max31865.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:21.020817 adafruit-circuitpython-max31865-2.2.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:21.020817 adafruit-circuitpython-max31865-2.2.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      127 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5503 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      190 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     1216 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:50:21.020817 adafruit-circuitpython-max31865-2.2.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)      997 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/examples/max31865_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      152 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 23:50:21.020817 adafruit-circuitpython-max31865-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1970 2021-03-02 23:50:08.000000 adafruit-circuitpython-max31865-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:23:31.077065 adafruit-circuitpython-max31865-2.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:23:31.073065 adafruit-circuitpython-max31865-2.2.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:23:31.073065 adafruit-circuitpython-max31865-2.2.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      189 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:23:31.073065 adafruit-circuitpython-max31865-2.2.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3678 2021-04-26 20:23:31.077065 adafruit-circuitpython-max31865-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2276 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:23:31.077065 adafruit-circuitpython-max31865-2.2.9/adafruit_circuitpython_max31865.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3678 2021-04-26 20:23:30.000000 adafruit-circuitpython-max31865-2.2.9/adafruit_circuitpython_max31865.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      779 2021-04-26 20:23:30.000000 adafruit-circuitpython-max31865-2.2.9/adafruit_circuitpython_max31865.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-26 20:23:30.000000 adafruit-circuitpython-max31865-2.2.9/adafruit_circuitpython_max31865.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-26 20:23:30.000000 adafruit-circuitpython-max31865-2.2.9/adafruit_circuitpython_max31865.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2021-04-26 20:23:30.000000 adafruit-circuitpython-max31865-2.2.9/adafruit_circuitpython_max31865.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    10261 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/adafruit_max31865.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:23:31.077065 adafruit-circuitpython-max31865-2.2.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:23:31.077065 adafruit-circuitpython-max31865-2.2.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5503 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      190 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1362 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-26 20:23:31.077065 adafruit-circuitpython-max31865-2.2.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)      977 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/examples/max31865_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-26 20:23:31.077065 adafruit-circuitpython-max31865-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1970 2021-04-26 20:23:21.000000 adafruit-circuitpython-max31865-2.2.9/setup.py
```

### Comparing `adafruit-circuitpython-max31865-2.2.8/.github/workflows/build.yml` & `adafruit-circuitpython-max31865-2.2.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/.github/workflows/release.yml` & `adafruit-circuitpython-max31865-2.2.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/.pre-commit-config.yaml` & `adafruit-circuitpython-max31865-2.2.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/.pylintrc` & `adafruit-circuitpython-max31865-2.2.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-max31865-2.2.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-max31865-2.2.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/LICENSE` & `adafruit-circuitpython-max31865-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-max31865-2.2.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/LICENSES/MIT.txt` & `adafruit-circuitpython-max31865-2.2.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-max31865-2.2.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/PKG-INFO` & `adafruit-circuitpython-max31865-2.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-max31865
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for MAX31865 thermocouple amplifier.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MAX31865
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-max31865-2.2.8/README.rst` & `adafruit-circuitpython-max31865-2.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/adafruit_circuitpython_max31865.egg-info/PKG-INFO` & `adafruit-circuitpython-max31865-2.2.9/adafruit_circuitpython_max31865.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-max31865
-Version: 2.2.8
+Version: 2.2.9
 Summary: CircuitPython library for MAX31865 thermocouple amplifier.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_MAX31865
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-max31865-2.2.8/adafruit_circuitpython_max31865.egg-info/SOURCES.txt` & `adafruit-circuitpython-max31865-2.2.9/adafruit_circuitpython_max31865.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/adafruit_max31865.py` & `adafruit-circuitpython-max31865-2.2.9/adafruit_max31865.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,16 +23,17 @@
   <https://www.adafruit.com/product/3328>`_ (Product ID: 3328)
 
 * Adafruit `PT1000 RTD Temperature Sensor Amplifier - MAX31865
   <https://www.adafruit.com/product/3648>`_ (Product ID: 3648)
 
 **Software and Dependencies:**
 
-* Adafruit CircuitPython firmware for the ESP8622 and M0-based boards:
-  https://github.com/adafruit/circuitpython/releases
+* Adafruit CircuitPython firmware for the supported boards:
+  https://circuitpython.org/downloads
+
 * Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 import math
 import time
 
 from micropython import const
 
@@ -66,15 +67,52 @@
 _MAX31865_FAULT_RTDINLOW = const(0x08)
 _MAX31865_FAULT_OVUV = const(0x04)
 _RTD_A = 3.9083e-3
 _RTD_B = -5.775e-7
 
 
 class MAX31865:
-    """Driver for the MAX31865 thermocouple amplifier."""
+    """Driver for the MAX31865 thermocouple amplifier.
+
+    :param ~busio.SPI spi: SPI device
+    :param ~digitalio.DigitalInOut cs: Chip Select
+    :param int rtd_nominal: RTD nominal value. Defaults to :const:`100`
+    :param int ref_resistor: Reference resistance. Defaults to :const:`430.0`
+    :param int wires: Number of wires. Defaults to :const:`2`
+    :param int filter_frequency: . Filter frequency. Default to :const:`60`
+
+
+    **Quickstart: Importing and using the MAX31865**
+
+        Here is an example of using the :class:`MAX31865` class.
+        First you will need to import the libraries to use the sensor
+
+        .. code-block:: python
+
+            import board
+            from digitalio import DigitalInOut, Direction
+            import adafruit_max31865
+
+        Once this is done you can define your `board.SPI` object and define your sensor object
+
+        .. code-block:: python
+
+            spi = board.SPI()
+            cs = digitalio.DigitalInOut(board.D5)  # Chip select of the MAX31865 board.
+            sensor = adafruit_max31865.MAX31865(spi, cs)
+
+
+        Now you have access to the :attr:`temperature` attribute
+
+        .. code-block:: python
+
+            temperature = sensor.temperature
+
+
+    """
 
     # Class-level buffer for reading and writing data with the sensor.
     # This reduces memory allocations but means the code is not re-entrant or
     # thread safe!
     _BUFFER = bytearray(3)
 
     def __init__(
@@ -168,15 +206,15 @@
             config |= _MAX31865_CONFIG_MODEAUTO  # Enable auto convert.
         else:
             config &= ~_MAX31865_CONFIG_MODEAUTO  # Disable auto convert.
         self._write_u8(_MAX31865_CONFIG_REG, config)
 
     @property
     def fault(self):
-        """The fault state of the sensor.  Use ``clear_faults()`` to clear the
+        """The fault state of the sensor.  Use :meth:`clear_faults` to clear the
         fault state.  Returns a 6-tuple of boolean values which indicate if any
         faults are present:
 
         - HIGHTHRESH
         - LOWTHRESH
         - REFINLOW
         - REFINHIGH
```

### Comparing `adafruit-circuitpython-max31865-2.2.8/docs/_static/favicon.ico` & `adafruit-circuitpython-max31865-2.2.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/docs/conf.py` & `adafruit-circuitpython-max31865-2.2.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-max31865-2.2.8/docs/index.rst` & `adafruit-circuitpython-max31865-2.2.9/docs/index.rst`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     :maxdepth: 3
 
     api
 
 .. toctree::
     :caption: Tutorials
 
+    Adafruit PT100 RTD Temperature Sensor Amplifier - MAX31865 Learning Guide <https://learn.adafruit.com/adafruit-max31865-rtd-pt100-amplifier>
+
 .. toctree::
     :caption: Related Products
 
     Adafruit Universal Thermocouple Amplifier MAX31856 Breakout <https://www.adafruit.com/product/3263>
 
     Adafruit PT100 RTD Temperature Sensor Amplifier - MAX31865  <https://www.adafruit.com/product/3328>
```

### Comparing `adafruit-circuitpython-max31865-2.2.8/examples/max31865_simpletest.py` & `adafruit-circuitpython-max31865-2.2.9/examples/max31865_simpletest.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 # Simple demo of the MAX31865 thermocouple amplifier.
 # Will print the temperature every second.
 import time
-
 import board
-import busio
 import digitalio
-
 import adafruit_max31865
 
 
-# Initialize SPI bus and sensor.
-spi = busio.SPI(board.SCK, MOSI=board.MOSI, MISO=board.MISO)
+# Create sensor object, communicating over the board's default SPI bus
+spi = board.SPI()
 cs = digitalio.DigitalInOut(board.D5)  # Chip select of the MAX31865 board.
 sensor = adafruit_max31865.MAX31865(spi, cs)
 # Note you can optionally provide the thermocouple RTD nominal, the reference
 # resistance, and the number of wires for the sensor (2 the default, 3, or 4)
 # with keyword args:
 # sensor = adafruit_max31865.MAX31865(spi, cs, rtd_nominal=100, ref_resistor=430.0, wires=2)
```

### Comparing `adafruit-circuitpython-max31865-2.2.8/setup.py` & `adafruit-circuitpython-max31865-2.2.9/setup.py`

 * *Files identical despite different names*

