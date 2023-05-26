# Comparing `tmp/adafruit-circuitpython-lis2mdl-2.1.8.tar.gz` & `tmp/adafruit-circuitpython-lis2mdl-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adafruit-circuitpython-lis2mdl-2.1.8.tar", last modified: Tue Mar  2 23:52:59 2021, max compression
+gzip compressed data, was "adafruit-circuitpython-lis2mdl-2.1.9.tar", last modified: Thu Apr 29 17:20:38 2021, max compression
```

## Comparing `adafruit-circuitpython-lis2mdl-2.1.8.tar` & `adafruit-circuitpython-lis2mdl-2.1.9.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:59.948017 adafruit-circuitpython-lis2mdl-2.1.8/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:59.940017 adafruit-circuitpython-lis2mdl-2.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:59.944017 adafruit-circuitpython-lis2mdl-2.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (116)     2329 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (116)     2712 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (116)      197 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (116)     1020 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (116)    16231 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (116)      162 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (116)     6147 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (116)     1102 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:59.944017 adafruit-circuitpython-lis2mdl-2.1.8/LICENSES/
--rw-r--r--   0 runner    (1001) docker     (116)    16814 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/LICENSES/CC-BY-4.0.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1108 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/LICENSES/MIT.txt
--rw-r--r--   0 runner    (1001) docker     (116)     1211 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/LICENSES/Unlicense.txt
--rw-r--r--   0 runner    (1001) docker     (116)     4259 2021-03-02 23:52:59.948017 adafruit-circuitpython-lis2mdl-2.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2703 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/README.rst
--rw-r--r--   0 runner    (1001) docker     (116)      108 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/README.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:59.944017 adafruit-circuitpython-lis2mdl-2.1.8/adafruit_circuitpython_lis2mdl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     4259 2021-03-02 23:52:59.000000 adafruit-circuitpython-lis2mdl-2.1.8/adafruit_circuitpython_lis2mdl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      860 2021-03-02 23:52:59.000000 adafruit-circuitpython-lis2mdl-2.1.8/adafruit_circuitpython_lis2mdl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-03-02 23:52:59.000000 adafruit-circuitpython-lis2mdl-2.1.8/adafruit_circuitpython_lis2mdl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       81 2021-03-02 23:52:59.000000 adafruit-circuitpython-lis2mdl-2.1.8/adafruit_circuitpython_lis2mdl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       17 2021-03-02 23:52:59.000000 adafruit-circuitpython-lis2mdl-2.1.8/adafruit_circuitpython_lis2mdl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)     7549 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/adafruit_lis2mdl.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:59.948017 adafruit-circuitpython-lis2mdl-2.1.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:59.948017 adafruit-circuitpython-lis2mdl-2.1.8/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (116)     4414 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (116)      105 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/_static/favicon.ico.license
--rw-r--r--   0 runner    (1001) docker     (116)      126 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/api.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     5596 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (116)      334 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/examples.rst.license
--rw-r--r--   0 runner    (1001) docker     (116)     1104 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (116)       96 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/docs/index.rst.license
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-03-02 23:52:59.948017 adafruit-circuitpython-lis2mdl-2.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (116)     1174 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/examples/lis2mdl_calibrate.py
--rw-r--r--   0 runner    (1001) docker     (116)     1978 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/examples/lis2mdl_compass.py
--rw-r--r--   0 runner    (1001) docker     (116)      587 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/examples/lis2mdl_interrupt.py
--rw-r--r--   0 runner    (1001) docker     (116)      458 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/examples/lis2mdl_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (116)      184 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2021-03-02 23:52:59.948017 adafruit-circuitpython-lis2mdl-2.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2060 2021-03-02 23:52:47.000000 adafruit-circuitpython-lis2mdl-2.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:20:38.747769 adafruit-circuitpython-lis2mdl-2.1.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:20:38.739769 adafruit-circuitpython-lis2mdl-2.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:20:38.743769 adafruit-circuitpython-lis2mdl-2.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2329 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2712 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    16223 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (121)      162 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     6147 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1102 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:20:38.743769 adafruit-circuitpython-lis2mdl-2.1.9/LICENSES/
+-rw-r--r--   0 runner    (1001) docker     (121)    16814 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/LICENSES/CC-BY-4.0.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/LICENSES/MIT.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1211 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/LICENSES/Unlicense.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4238 2021-04-29 17:20:38.743769 adafruit-circuitpython-lis2mdl-2.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2698 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/README.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      108 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/README.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:20:38.743769 adafruit-circuitpython-lis2mdl-2.1.9/adafruit_circuitpython_lis2mdl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     4238 2021-04-29 17:20:38.000000 adafruit-circuitpython-lis2mdl-2.1.9/adafruit_circuitpython_lis2mdl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      860 2021-04-29 17:20:38.000000 adafruit-circuitpython-lis2mdl-2.1.9/adafruit_circuitpython_lis2mdl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-04-29 17:20:38.000000 adafruit-circuitpython-lis2mdl-2.1.9/adafruit_circuitpython_lis2mdl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2021-04-29 17:20:38.000000 adafruit-circuitpython-lis2mdl-2.1.9/adafruit_circuitpython_lis2mdl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2021-04-29 17:20:38.000000 adafruit-circuitpython-lis2mdl-2.1.9/adafruit_circuitpython_lis2mdl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     8236 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/adafruit_lis2mdl.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:20:38.743769 adafruit-circuitpython-lis2mdl-2.1.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:20:38.743769 adafruit-circuitpython-lis2mdl-2.1.9/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)     4414 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/_static/favicon.ico.license
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/api.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     5596 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)      803 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/examples.rst.license
+-rw-r--r--   0 runner    (1001) docker     (121)     1256 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       96 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/docs/index.rst.license
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-04-29 17:20:38.743769 adafruit-circuitpython-lis2mdl-2.1.9/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)     1173 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/examples/lis2mdl_calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1977 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/examples/lis2mdl_compass.py
+-rw-r--r--   0 runner    (1001) docker     (121)      586 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/examples/lis2mdl_interrupt.py
+-rw-r--r--   0 runner    (1001) docker     (121)      457 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/examples/lis2mdl_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-04-29 17:20:38.747769 adafruit-circuitpython-lis2mdl-2.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2060 2021-04-29 17:20:28.000000 adafruit-circuitpython-lis2mdl-2.1.9/setup.py
```

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/.github/workflows/build.yml` & `adafruit-circuitpython-lis2mdl-2.1.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/.github/workflows/release.yml` & `adafruit-circuitpython-lis2mdl-2.1.9/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/.pre-commit-config.yaml` & `adafruit-circuitpython-lis2mdl-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/.pylintrc` & `adafruit-circuitpython-lis2mdl-2.1.9/.pylintrc`

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

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-lis2mdl-2.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/LICENSE` & `adafruit-circuitpython-lis2mdl-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/LICENSES/CC-BY-4.0.txt` & `adafruit-circuitpython-lis2mdl-2.1.9/LICENSES/CC-BY-4.0.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/LICENSES/MIT.txt` & `adafruit-circuitpython-lis2mdl-2.1.9/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/LICENSES/Unlicense.txt` & `adafruit-circuitpython-lis2mdl-2.1.9/LICENSES/Unlicense.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/PKG-INFO` & `adafruit-circuitpython-lis2mdl-2.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lis2mdl
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for LIS2MDL 3-axis magnetometer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LIS2MDL
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
@@ -60,27 +60,25 @@
             python3 -m venv .env
             source .env/bin/activate
             pip3 install adafruit-circuitpython-lis2mdl
         
         Usage Example
         =============
         
-        .. code-block:: python
+        .. code-block:: python3
         
             import time
             import board
-            import busio
             import adafruit_lis2mdl
         
-            i2c = busio.I2C(board.SCL, board.SDA)
+            i2c = board.I2C()  # uses board.SCL and board.SDA
             sensor = adafruit_lis2mdl.LIS2MDL(i2c)
         
             while True:
                 mag_x, mag_y, mag_z = sensor.magnetic
-        
                 print('Magnetometer (gauss): ({0:10.3f}, {1:10.3f}, {2:10.3f})'.format(mag_x, mag_y, mag_z))
                 print('')
                 time.sleep(1.0)
         
         
         Contributing
         ============
```

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/README.rst` & `adafruit-circuitpython-lis2mdl-2.1.9/README.rst`

 * *Files 16% similar despite different names*

```diff
@@ -52,27 +52,25 @@
     python3 -m venv .env
     source .env/bin/activate
     pip3 install adafruit-circuitpython-lis2mdl
 
 Usage Example
 =============
 
-.. code-block:: python
+.. code-block:: python3
 
     import time
     import board
-    import busio
     import adafruit_lis2mdl
 
-    i2c = busio.I2C(board.SCL, board.SDA)
+    i2c = board.I2C()  # uses board.SCL and board.SDA
     sensor = adafruit_lis2mdl.LIS2MDL(i2c)
 
     while True:
         mag_x, mag_y, mag_z = sensor.magnetic
-
         print('Magnetometer (gauss): ({0:10.3f}, {1:10.3f}, {2:10.3f})'.format(mag_x, mag_y, mag_z))
         print('')
         time.sleep(1.0)
 
 
 Contributing
 ============
```

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/adafruit_circuitpython_lis2mdl.egg-info/PKG-INFO` & `adafruit-circuitpython-lis2mdl-2.1.9/adafruit_circuitpython_lis2mdl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-lis2mdl
-Version: 2.1.8
+Version: 2.1.9
 Summary: CircuitPython library for LIS2MDL 3-axis magnetometer.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_LIS2MDL
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
@@ -60,27 +60,25 @@
             python3 -m venv .env
             source .env/bin/activate
             pip3 install adafruit-circuitpython-lis2mdl
         
         Usage Example
         =============
         
-        .. code-block:: python
+        .. code-block:: python3
         
             import time
             import board
-            import busio
             import adafruit_lis2mdl
         
-            i2c = busio.I2C(board.SCL, board.SDA)
+            i2c = board.I2C()  # uses board.SCL and board.SDA
             sensor = adafruit_lis2mdl.LIS2MDL(i2c)
         
             while True:
                 mag_x, mag_y, mag_z = sensor.magnetic
-        
                 print('Magnetometer (gauss): ({0:10.3f}, {1:10.3f}, {2:10.3f})'.format(mag_x, mag_y, mag_z))
                 print('')
                 time.sleep(1.0)
         
         
         Contributing
         ============
```

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/adafruit_circuitpython_lis2mdl.egg-info/SOURCES.txt` & `adafruit-circuitpython-lis2mdl-2.1.9/adafruit_circuitpython_lis2mdl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/adafruit_lis2mdl.py` & `adafruit-circuitpython-lis2mdl-2.1.9/adafruit_lis2mdl.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,18 @@
 * Adafruit `Triple-axis Accelerometer+Magnetometer (Compass) Board - LSM303
   <https://www.adafruit.com/product/1120>`_ (Product ID: 1120)
 * Adafruit `FLORA Accelerometer/Compass Sensor - LSM303 - v1.0
   <https://www.adafruit.com/product/1247>`_ (Product ID: 1247)
 
 **Software and Dependencies:**
 
-* Adafruit CircuitPython firmware:
+* Adafruit CircuitPython firmware for the supported boards:
   https://circuitpython.org/downloads
-* Adafruit's Bus Device library:
-  https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
-* Adafruit's Register library:
-  https://github.com/adafruit/Adafruit_CircuitPython_Register
+* Adafruit's Bus Device library: https://github.com/adafruit/Adafruit_CircuitPython_BusDevice
+* Adafruit's Register library: https://github.com/adafruit/Adafruit_CircuitPython_Register
 """
 
 from time import sleep
 from micropython import const
 from adafruit_bus_device.i2c_device import I2CDevice
 from adafruit_register.i2c_struct import UnaryStruct, ROUnaryStruct
 from adafruit_register.i2c_bit import RWBit
@@ -87,15 +85,39 @@
 _MAG_SCALE = 0.15  # 1.5 milligauss/LSB * 0.1 microtesla/milligauss
 
 
 class LIS2MDL:  # pylint: disable=too-many-instance-attributes
     """
     Driver for the LIS2MDL 3-axis magnetometer.
 
-    :param busio.I2C i2c_bus: The I2C bus the LIS2MDL is connected to.
+    :param ~busio.I2C i2c:  The I2C bus the device is connected to
+
+    **Quickstart: Importing and using the device**
+
+        Here is an example of using the :class:`LIS2MDL` class.
+        First you will need to import the libraries to use the sensor
+
+        .. code-block:: python
+
+            import board
+            import adafruit_lis2mdl
+
+        Once this is done you can define your `board.I2C` object and define your sensor object
+
+        .. code-block:: python
+
+            i2c = board.I2C()  # uses board.SCL and board.SDA
+            sensor = adafruit_lis2mdl.LIS2MDL(i2c)
+
+        Now you have access to the :attr:`magnetic` attribute
+
+        .. code-block:: python
+
+            mag_x, mag_y, mag_z = sensor.magnetic
+
 
     """
 
     _BUFFER = bytearray(6)
 
     _device_id = ROUnaryStruct(WHO_AM_I, "B")
     _int_control = UnaryStruct(INT_CRTL_REG, "B")
```

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/docs/_static/favicon.ico` & `adafruit-circuitpython-lis2mdl-2.1.9/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/docs/conf.py` & `adafruit-circuitpython-lis2mdl-2.1.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/docs/index.rst` & `adafruit-circuitpython-lis2mdl-2.1.9/docs/index.rst`

 * *Files 13% similar despite different names*

```diff
@@ -19,14 +19,16 @@
     :maxdepth: 3
 
     api
 
 .. toctree::
     :caption: Tutorials
 
+    Triple-axis Accelerometer+Magnetometer (Compass) Board - LSM303 <https://learn.adafruit.com/lsm303-accelerometer-slash-compass-breakout/downloads>
+
 .. toctree::
     :caption: Related Products
 
     Triple-axis Accelerometer+Magnetometer (Compass) Board - LSM303 <https://www.adafruit.com/product/1120>
     FLORA Accelerometer/Compass Sensor - LSM303 - v1.0 <https://www.adafruit.com/product/1247>
 
 .. toctree::
```

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/examples/lis2mdl_compass.py` & `adafruit-circuitpython-lis2mdl-2.1.9/examples/lis2mdl_compass.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 # SPDX-License-Identifier: MIT
 
 """ Display compass heading data from a calibrated magnetometer """
 
 import time
 import math
 import board
-import busio
 import adafruit_lis2mdl
 
-i2c = busio.I2C(board.SCL, board.SDA)
+i2c = board.I2C()  # uses board.SCL and board.SDA
 sensor = adafruit_lis2mdl.LIS2MDL(i2c)
 
 # You will need the calibration values from your magnetometer calibration
 # these values are in uT and are in X, Y, Z order (min and max values).
 #
 # To get these values run the lis2mdl_calibrate.py script on your device.
 # Twist the device around in 3D space while it calibrates. It will print
```

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/examples/lis2mdl_interrupt.py` & `adafruit-circuitpython-lis2mdl-2.1.9/examples/lis2mdl_interrupt.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # SPDX-FileCopyrightText: 2021 ladyada for Adafruit Industries
 # SPDX-License-Identifier: MIT
 
 import time
 import board
-import busio
 import adafruit_lis2mdl
 
-i2c = busio.I2C(board.SCL, board.SDA)
+i2c = board.I2C()  # uses board.SCL and board.SDA
 lis = adafruit_lis2mdl.LIS2MDL(i2c)
 lis.interrupt_threshold = 80
 lis.interrupt_enabled = True
 
 while True:
     x_hi, y_hi, z_hi, x_lo, y_lo, z_lo, int_triggered = lis.faults
```

### Comparing `adafruit-circuitpython-lis2mdl-2.1.8/setup.py` & `adafruit-circuitpython-lis2mdl-2.1.9/setup.py`

 * *Files identical despite different names*

