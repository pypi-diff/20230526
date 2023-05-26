# Comparing `tmp/adafruit-circuitpython-vcnl4010-0.9.5.tar.gz` & `tmp/adafruit-circuitpython-vcnl4010-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/adafruit-circuitpython-vcnl4010-0.9.5.tar", last modified: Thu Jan 23 14:37:27 2020, max compression
+gzip compressed data, was "dist/adafruit-circuitpython-vcnl4010-0.9.6.tar", last modified: Wed Feb  5 13:29:05 2020, max compression
```

## Comparing `adafruit-circuitpython-vcnl4010-0.9.5.tar` & `adafruit-circuitpython-vcnl4010-0.9.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (115)     1519 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (115)       85 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (115)    16110 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (115)       59 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (115)     5824 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (115)     1102 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (115)     3712 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     2306 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/adafruit_circuitpython_vcnl4010.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     3712 2020-01-23 14:37:25.000000 adafruit-circuitpython-vcnl4010-0.9.5/adafruit_circuitpython_vcnl4010.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)      570 2020-01-23 14:37:27.000000 adafruit-circuitpython-vcnl4010-0.9.5/adafruit_circuitpython_vcnl4010.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-23 14:37:25.000000 adafruit-circuitpython-vcnl4010-0.9.5/adafruit_circuitpython_vcnl4010.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       49 2020-01-23 14:37:25.000000 adafruit-circuitpython-vcnl4010-0.9.5/adafruit_circuitpython_vcnl4010.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       18 2020-01-23 14:37:25.000000 adafruit-circuitpython-vcnl4010-0.9.5/adafruit_circuitpython_vcnl4010.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)     9097 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/adafruit_vcnl4010.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/docs/
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/docs/_static/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (115)      127 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (115)     5249 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (115)      190 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (115)      978 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/docs/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/examples/
--rw-r--r--   0 runner    (1001) docker     (115)     1343 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/examples/vcnl4010_simpletest.py
--rw-r--r--   0 runner    (1001) docker     (115)       49 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-01-23 14:37:27.591347 adafruit-circuitpython-vcnl4010-0.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1885 2020-01-23 14:37:14.000000 adafruit-circuitpython-vcnl4010-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:29:05.533579 adafruit-circuitpython-vcnl4010-0.9.6/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:29:05.525579 adafruit-circuitpython-vcnl4010-0.9.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:29:05.529579 adafruit-circuitpython-vcnl4010-0.9.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (115)     1519 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     2598 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (115)       85 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (115)    16110 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (115)       59 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (115)     5824 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (115)     1102 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (115)     3712 2020-02-05 13:29:05.533579 adafruit-circuitpython-vcnl4010-0.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     2306 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:29:05.529579 adafruit-circuitpython-vcnl4010-0.9.6/adafruit_circuitpython_vcnl4010.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     3712 2020-02-05 13:29:05.000000 adafruit-circuitpython-vcnl4010-0.9.6/adafruit_circuitpython_vcnl4010.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)      570 2020-02-05 13:29:05.000000 adafruit-circuitpython-vcnl4010-0.9.6/adafruit_circuitpython_vcnl4010.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-02-05 13:29:05.000000 adafruit-circuitpython-vcnl4010-0.9.6/adafruit_circuitpython_vcnl4010.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       49 2020-02-05 13:29:05.000000 adafruit-circuitpython-vcnl4010-0.9.6/adafruit_circuitpython_vcnl4010.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       18 2020-02-05 13:29:05.000000 adafruit-circuitpython-vcnl4010-0.9.6/adafruit_circuitpython_vcnl4010.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)     9097 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/adafruit_vcnl4010.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:29:05.529579 adafruit-circuitpython-vcnl4010-0.9.6/docs/
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:29:05.529579 adafruit-circuitpython-vcnl4010-0.9.6/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (115)     4414 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/docs/_static/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (115)      127 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (115)     5248 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (115)      190 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (115)      978 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/docs/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-02-05 13:29:05.533579 adafruit-circuitpython-vcnl4010-0.9.6/examples/
+-rw-r--r--   0 runner    (1001) docker     (115)     1343 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/examples/vcnl4010_simpletest.py
+-rw-r--r--   0 runner    (1001) docker     (115)       49 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-02-05 13:29:05.533579 adafruit-circuitpython-vcnl4010-0.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     1885 2020-02-05 13:28:46.000000 adafruit-circuitpython-vcnl4010-0.9.6/setup.py
```

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/.github/workflows/build.yml` & `adafruit-circuitpython-vcnl4010-0.9.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/.github/workflows/release.yml` & `adafruit-circuitpython-vcnl4010-0.9.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/.pylintrc` & `adafruit-circuitpython-vcnl4010-0.9.6/.pylintrc`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/CODE_OF_CONDUCT.md` & `adafruit-circuitpython-vcnl4010-0.9.6/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/LICENSE` & `adafruit-circuitpython-vcnl4010-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/PKG-INFO` & `adafruit-circuitpython-vcnl4010-0.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vcnl4010
-Version: 0.9.5
+Version: 0.9.6
 Summary: CircuitPython library for VCNL4010 proximity and light sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_VCNL4010
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/README.rst` & `adafruit-circuitpython-vcnl4010-0.9.6/README.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/adafruit_circuitpython_vcnl4010.egg-info/PKG-INFO` & `adafruit-circuitpython-vcnl4010-0.9.6/adafruit_circuitpython_vcnl4010.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adafruit-circuitpython-vcnl4010
-Version: 0.9.5
+Version: 0.9.6
 Summary: CircuitPython library for VCNL4010 proximity and light sensor.
 Home-page: https://github.com/adafruit/Adafruit_CircuitPython_VCNL4010
 Author: Adafruit Industries
 Author-email: circuitpython@adafruit.com
 License: MIT
 Description: 
         Introduction
```

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/adafruit_circuitpython_vcnl4010.egg-info/SOURCES.txt` & `adafruit-circuitpython-vcnl4010-0.9.6/adafruit_circuitpython_vcnl4010.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/adafruit_vcnl4010.py` & `adafruit-circuitpython-vcnl4010-0.9.6/adafruit_vcnl4010.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/docs/_static/favicon.ico` & `adafruit-circuitpython-vcnl4010-0.9.6/docs/_static/favicon.ico`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/docs/conf.py` & `adafruit-circuitpython-vcnl4010-0.9.6/docs/conf.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ]
 
 # Uncomment the below if you use native CircuitPython modules such as
 # digitalio, micropython and busio. List the modules you use. Without it, the
 # autodoc module docs will fail to generate with a warning.
 # autodoc_mock_imports = ["micropython", "adafruit_bus_device"]
 
-intersphinx_mapping = {'python': ('https://docs.python.org/3.4', None),'BusDevice': ('https://circuitpython.readthedocs.io/projects/bus_device/en/latest/', None),'CircuitPython': ('https://circuitpython.readthedocs.io/en/latest/', None)}
+intersphinx_mapping = {'python': ('https://docs.python.org/3.4', None),'BusDevice': ('https://circuitpython.readthedocs.io/projects/busdevice/en/latest/', None),'CircuitPython': ('https://circuitpython.readthedocs.io/en/latest/', None)}
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ['_templates']
 
 source_suffix = '.rst'
 
 # The master toctree document.
```

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/docs/index.rst` & `adafruit-circuitpython-vcnl4010-0.9.6/docs/index.rst`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/examples/vcnl4010_simpletest.py` & `adafruit-circuitpython-vcnl4010-0.9.6/examples/vcnl4010_simpletest.py`

 * *Files identical despite different names*

### Comparing `adafruit-circuitpython-vcnl4010-0.9.5/setup.py` & `adafruit-circuitpython-vcnl4010-0.9.6/setup.py`

 * *Files identical despite different names*

