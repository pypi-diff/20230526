# Comparing `tmp/pickled_carrots-1.0.3.tar.gz` & `tmp/pickled_carrots-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-1.0.3.tar", max compression
+gzip compressed data, was "pickled_carrots-1.0.4.tar", max compression
```

## Comparing `pickled_carrots-1.0.3.tar` & `pickled_carrots-1.0.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-1.0.3/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-1.0.3/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-1.0.3/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-1.0.3/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-1.0.3/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-1.0.3/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-1.0.3/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-1.0.3/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-1.0.3/pickled_carrots/plot.py
--rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-1.0.3/pickled_carrots/resources/event_type_lookup.pickle
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-1.0.3/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0    13845 2023-05-26 13:00:40.817419 pickled_carrots-1.0.3/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     9239 2023-05-26 08:57:52.556544 pickled_carrots-1.0.3/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-1.0.3/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-1.0.3/pickled_carrots/vinegar/tests/test_read_hsf.py
--rw-r--r--   0        0        0   138987 2023-05-24 17:57:38.942953 pickled_carrots-1.0.3/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-05-26 14:08:05.381062 pickled_carrots-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 pickled_carrots-1.0.3/setup.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-1.0.4/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-1.0.4/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-1.0.4/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-1.0.4/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-1.0.4/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-1.0.4/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-1.0.4/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-1.0.4/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-1.0.4/pickled_carrots/plot.py
+-rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-1.0.4/pickled_carrots/resources/event_type_lookup.pickle
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-1.0.4/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0    13845 2023-05-26 13:00:40.817419 pickled_carrots-1.0.4/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     9239 2023-05-26 08:57:52.556544 pickled_carrots-1.0.4/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-1.0.4/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-1.0.4/pickled_carrots/vinegar/tests/test_read_hsf.py
+-rw-r--r--   0        0        0   138987 2023-05-24 17:57:38.942953 pickled_carrots-1.0.4/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-05-26 14:18:36.274328 pickled_carrots-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 pickled_carrots-1.0.4/setup.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-1.0.4/PKG-INFO
```

### Comparing `pickled_carrots-1.0.3/README.md` & `pickled_carrots-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/DPData.py` & `pickled_carrots-1.0.4/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/DPPlot.py` & `pickled_carrots-1.0.4/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/DPUtil.py` & `pickled_carrots-1.0.4/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/database.py` & `pickled_carrots-1.0.4/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/dataclass.py` & `pickled_carrots-1.0.4/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/mathutil.py` & `pickled_carrots-1.0.4/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/plot.py` & `pickled_carrots-1.0.4/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/resources/event_type_lookup.pickle` & `pickled_carrots-1.0.4/pickled_carrots/resources/event_type_lookup.pickle`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/vinegar/core.py` & `pickled_carrots-1.0.4/pickled_carrots/vinegar/core.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/vinegar/event.py` & `pickled_carrots-1.0.4/pickled_carrots/vinegar/event.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-1.0.4/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/vinegar/tests/test_read_hsf.py` & `pickled_carrots-1.0.4/pickled_carrots/vinegar/tests/test_read_hsf.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/pickled_carrots/waveforms.py` & `pickled_carrots-1.0.4/pickled_carrots/waveforms.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-1.0.3/setup.py` & `pickled_carrots-1.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,19 +21,19 @@
  'pymongo>=4.3.3,<5.0.0',
  'pyodbc==4.0.34',
  'pyproj==3.4.1',
  'python-ternary>=1.0.8,<2.0.0',
  'pytz>=2023.3,<2024.0',
  'shapely>=2.0.1,<3.0.0',
  'statsmodels>=0.14.0,<0.15.0',
- 'uquake>=1.4.5,<2.0.0']
+ 'uquake>=1.4.6,<2.0.0']
 
 setup_kwargs = {
     'name': 'pickled-carrots',
-    'version': '1.0.3',
+    'version': '1.0.4',
     'description': '',
     'long_description': "# ESG_Research\n\nThis repository contains Python and C# code which is used for various different functions. In this document we will go through what each folder contains.\n\n__Analytics_Notebooks__\n\nThis folder contains Jupyter notebooks which have various different functionalities. More notebooks can be found on the DataShare, under Frac4/Notebooks.\n\n&nbsp;\n\n\n__ESG-dash__\n\nA dash-based dashboard for evaluating sensor quality for mining sites.\n\n&nbsp;\n\n\n__ESG__\n\nThe main module folder for our Python codes. The files within this folder are used in most of our jupyter notebooks. More details on what each file contains can be found in the folder.\n\n&nbsp;\n\n__ITG-FMC__\n\nContains the tiltmeter processing dashboard written in Python, a Fiber processing C# app, a DPA and DPA-RTA C# app, and a copy of the Stress Inversion python package (which has since been merged into the main ESG repo.\n\n&nbsp;\n\n__Scripts__\n\nContains various Python scripts which are used to automated processes such as HypoDD or noise analysis.\n\n&nbsp;\n\n__build/lib, dist, esg_das, esg_dts__\n\nPython code for processing Fiber data. \n\n&nbsp;\n\n__Miscellaneous__\n\nThere are some additional files in this folder which are related to replicated anaconda environments. The requirements.txt file can be used to create ESG's default environment.\n",
     'author': 'pickled cattots team',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pickled_carrots-1.0.3/PKG-INFO` & `pickled_carrots-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickled-carrots
-Version: 1.0.3
+Version: 1.0.4
 Summary: 
 Author: pickled cattots team
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,15 +21,15 @@
 Requires-Dist: pymongo (>=4.3.3,<5.0.0)
 Requires-Dist: pyodbc (==4.0.34)
 Requires-Dist: pyproj (==3.4.1)
 Requires-Dist: python-ternary (>=1.0.8,<2.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: shapely (>=2.0.1,<3.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
-Requires-Dist: uquake (>=1.4.5,<2.0.0)
+Requires-Dist: uquake (>=1.4.6,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ESG_Research
 
 This repository contains Python and C# code which is used for various different functions. In this document we will go through what each folder contains.
 
 __Analytics_Notebooks__
```

