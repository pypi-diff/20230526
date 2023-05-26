# Comparing `tmp/adafruit-circuitpython-lsm9ds1-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-lsm9ds1-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lsm9ds1-2.1.8.tar", last modified: Thu Apr 29 17:22:46 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-lsm9ds1-2.1.9.tar", last modified: Mon May 10 19:11:20 2021, max compression
```

## Comparing `adafruit-circuitpython-lsm9ds1-2.1.8.tar` & `adafruit-circuitpython-lsm9ds1-2.1.9.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:22:46.003579 adafruit-circuitpython-lsm9ds1-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:22:45.999579 adafruit-circuitpython-lsm9ds1-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:22:45.999579 adafruit-circuitpython-lsm9ds1-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (121)      211 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (121)      162 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:22:45.999579 adafruit-circuitpython-lsm9ds1-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (121)     3729 2021-04-29 17:22:46.003579 adafruit-circuitpython-lsm9ds1-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2302 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:22:45.999579 adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_circuitpython_lsm9ds1.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3729 2021-04-29 17:22:45.000000 adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_circuitpython_lsm9ds1.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      772 2021-04-29 17:22:45.000000 adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_circuitpython_lsm9ds1.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-29 17:22:45.000000 adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_circuitpython_lsm9ds1.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-04-29 17:22:45.000000 adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_circuitpython_lsm9ds1.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2021-04-29 17:22:45.000000 adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_circuitpython_lsm9ds1.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    19082 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_lsm9ds1.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:22:46.003579 adafruit-circuitpython-lsm9ds1-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:22:46.003579 adafruit-circuitpython-lsm9ds1-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (121)      126 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     5493 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:22:46.003579 adafruit-circuitpython-lsm9ds1-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/examples/lsm9ds1_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (121)      152 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-29 17:22:46.003579 adafruit-circuitpython-lsm9ds1-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-04-29 17:22:32.000000 adafruit-circuitpython-lsm9ds1-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-10 19:11:20.213816 adafruit-circuitpython-lsm9ds1-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-10 19:11:20.205816 adafruit-circuitpython-lsm9ds1-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-10 19:11:20.209816 adafruit-circuitpython-lsm9ds1-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      211 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-10 19:11:20.209816 adafruit-circuitpython-lsm9ds1-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     3729 2021-05-10 19:11:20.213816 adafruit-circuitpython-lsm9ds1-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2302 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-10 19:11:20.209816 adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_circuitpython_lsm9ds1.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3729 2021-05-10 19:11:19.000000 adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_circuitpython_lsm9ds1.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      772 2021-05-10 19:11:20.000000 adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_circuitpython_lsm9ds1.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-10 19:11:19.000000 adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_circuitpython_lsm9ds1.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-05-10 19:11:19.000000 adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_circuitpython_lsm9ds1.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-05-10 19:11:19.000000 adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_circuitpython_lsm9ds1.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    19108 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_lsm9ds1.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-10 19:11:20.213816 adafruit-circuitpython-lsm9ds1-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-10 19:11:20.213816 adafruit-circuitpython-lsm9ds1-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5493 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      188 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1197 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-10 19:11:20.213816 adafruit-circuitpython-lsm9ds1-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1619 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/examples/lsm9ds1_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      152 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-05-10 19:11:20.213816 adafruit-circuitpython-lsm9ds1-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2001 2021-05-10 19:11:07.000000 adafruit-circuitpython-lsm9ds1-2.1.9/setup.py
```

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-lsm9ds1-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-lsm9ds1-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-lsm9ds1-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/.pylintrc` & `adafruit-circuitpython-lsm9ds1-2.1.9/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lsm9ds1-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/LICENSE` & `adafruit-circuitpython-lsm9ds1-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lsm9ds1-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-lsm9ds1-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lsm9ds1-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/PKG-INFO` & `adafruit-circuitpython-lsm9ds1-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lsm9ds1
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for LSM9DS1 accelerometer, magnetometer, gyroscope.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LSM9DS1
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/README.rst` & `adafruit-circuitpython-lsm9ds1-2.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_circuitpython_lsm9ds1.egg-info/PKG-INFO` & `adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_circuitpython_lsm9ds1.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lsm9ds1
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for LSM9DS1 accelerometer, magnetometer, gyroscope.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LSM9DS1
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_circuitpython_lsm9ds1.egg-info/SOURCES.txt` & `adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_circuitpython_lsm9ds1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/adafruit_lsm9ds1.py` & `adafruit-circuitpython-lsm9ds1-2.1.9/adafruit_lsm9ds1.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,29 +15,31 @@
 * Author(s): Tony DiCola
 
 Implementation Notes
 --------------------
 
 **Hardware:**
 
-* Adafruit `9-DOF Accel/Mag/Gyro+Temp Breakout Board - LSM9DS1
+* `Adafruit 9-DOF Accel/Mag/Gyro+Temp Breakout Board - LSM9DS1
   <https://www.adafruit.com/product/3387>`_ (Product ID: 3387)
 
 **Software and Dependencies:**
 
 * Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
+
 * Adafruit's Bus Device library:
   https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
 """
 
 __version__ = "0.0.0-auto.0"
 __repo__ = "https://github.com/adafruit/Adafruit_CircuitPython_LSM9DS1.git"
 
 import time
+from math import radians
 
 try:
     import struct
 except ImportError:
     import ustruct as struct
 
 import adafruit_bus_device.i2c_device as i2c_device
@@ -298,18 +300,18 @@
         self._read_bytes(_XGTYPE, 0x80 | _LSM9DS1_REGISTER_OUT_X_L_G, 6, self._BUFFER)
         raw_x, raw_y, raw_z = struct.unpack_from("<hhh", self._BUFFER[0:6])
         return (raw_x, raw_y, raw_z)
 
     @property
     def gyro(self):
         """The gyroscope X, Y, Z axis values as a 3-tuple of
-        degrees/second values.
+        rad/s values.
         """
         raw = self.read_gyro_raw()
-        return map(lambda x: x * self._gyro_dps_digit, raw)
+        return map(lambda x: radians(x * self._gyro_dps_digit), raw)
 
     def read_temp_raw(self):
         """Read the raw temperature sensor value and return it as a 12-bit
         signed value.  If you want the temperature in nice units you probably
         want to use the temperature property!
         """
         # Read temp sensor
```

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-lsm9ds1-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/docs/conf.py` & `adafruit-circuitpython-lsm9ds1-2.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/docs/index.rst` & `adafruit-circuitpython-lsm9ds1-2.1.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/examples/lsm9ds1_simpletest.py` & `adafruit-circuitpython-lsm9ds1-2.1.9/examples/lsm9ds1_simpletest.py`

 * *Files 8% similar despite different names*

```diff
@@ -36,14 +36,14 @@
             accel_x, accel_y, accel_z
         )
     )
     print(
         "Magnetometer (gauss): ({0:0.3f},{1:0.3f},{2:0.3f})".format(mag_x, mag_y, mag_z)
     )
     print(
-        "Gyroscope (degrees/sec): ({0:0.3f},{1:0.3f},{2:0.3f})".format(
+        "Gyroscope (rad/sec): ({0:0.3f},{1:0.3f},{2:0.3f})".format(
             gyro_x, gyro_y, gyro_z
         )
     )
     print("Temperature: {0:0.3f}C".format(temp))
     # Delay for a second.
     time.sleep(1.0)
```

### Comparing `adafruit-circuitpython-lsm9ds1-2.1.8/setup.py` & `adafruit-circuitpython-lsm9ds1-2.1.9/setup.py`

 * *Files identical despite different names*

