# Comparing `tmp/pickled_carrots-0.1.7.tar.gz` & `tmp/pickled_carrots-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-0.1.7.tar", max compression
+gzip compressed data, was "pickled_carrots-0.2.0.tar", max compression
```

## Comparing `pickled_carrots-0.1.7.tar` & `pickled_carrots-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,22 @@
--rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.1.7/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.1.7/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.1.7/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.1.7/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.1.7/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.1.7/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.1.7/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.1.7/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.1.7/pickled_carrots/plot.py
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.1.7/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0    16132 2023-05-23 22:54:44.753901 pickled_carrots-0.1.7/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     5547 2023-05-23 21:08:20.226797 pickled_carrots-0.1.7/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.1.7/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0      678 2023-05-23 23:36:02.421304 pickled_carrots-0.1.7/pickled_carrots/vinegar/tests/test_read_hsf.py
--rw-r--r--   0        0        0   138961 2023-05-23 21:02:01.777143 pickled_carrots-0.1.7/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-05-24 00:39:28.182560 pickled_carrots-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pickled_carrots-0.1.7/setup.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.2.0/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.2.0/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.2.0/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.2.0/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.2.0/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.2.0/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.2.0/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.2.0/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.2.0/pickled_carrots/plot.py
+-rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-0.2.0/pickled_carrots/resources/event_type_lookup.pickle
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.2.0/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-20 10:55:17.702165 pickled_carrots-0.2.0/pickled_carrots/vinegar/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0        0        0    13486 2023-05-24 16:56:20.344027 pickled_carrots-0.2.0/pickled_carrots/vinegar/__pycache__/core.cpython-39.pyc
+-rw-r--r--   0        0        0     5668 2023-05-24 22:08:29.557038 pickled_carrots-0.2.0/pickled_carrots/vinegar/__pycache__/event.cpython-39.pyc
+-rw-r--r--   0        0        0    17569 2023-05-26 09:34:52.131648 pickled_carrots-0.2.0/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     9239 2023-05-26 08:57:52.556544 pickled_carrots-0.2.0/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.2.0/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-0.2.0/pickled_carrots/vinegar/tests/test_read_hsf.py
+-rw-r--r--   0        0        0   138987 2023-05-24 17:57:38.942953 pickled_carrots-0.2.0/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-05-26 09:35:36.841726 pickled_carrots-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 pickled_carrots-0.2.0/setup.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.2.0/PKG-INFO
```

### Comparing `pickled_carrots-0.1.7/README.md` & `pickled_carrots-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/DPData.py` & `pickled_carrots-0.2.0/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/DPPlot.py` & `pickled_carrots-0.2.0/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/DPUtil.py` & `pickled_carrots-0.2.0/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/database.py` & `pickled_carrots-0.2.0/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/dataclass.py` & `pickled_carrots-0.2.0/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/mathutil.py` & `pickled_carrots-0.2.0/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/plot.py` & `pickled_carrots-0.2.0/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/vinegar/core.py` & `pickled_carrots-0.2.0/pickled_carrots/vinegar/core.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import hashlib
 from pickled_carrots.waveforms import HeaderLookups
 from uquake.core.stream import Stream, Trace
 from uquake.core.inventory import (Inventory, Network, Station, Channel,
                                    SystemResponse, Equipment)
 from uquake.core.event import Catalog
 from pickled_carrots.vinegar import event
+from pathlib import Path
 
 from uquake.core.logging import logger
 import numpy as np
 from pathlib import Path
 from importlib import reload
 import tarfile
 import gzip
@@ -279,19 +280,21 @@
         return evt
 
     @property
     def catalog(self):
         return Catalog(events=[self.event])
 
     @property
-    def file_bundle(self):
-        return FileBundleHandler(self.stream, self.catalog, self.inventory)
+    def usf_file(self):
+        return USFHandler(self.stream, self.catalog, self.inventory)
 
     @classmethod
     def read(cls, file_path, network, experimental=False):
+        if isinstance(file_path, Path):
+            file_path = str(file_path)
         with tempfile.NamedTemporaryFile(delete=True) as tmpfile:
             st, head = waveforms.hsf_to_obspy(file_path, print_out=False,
                                               groundmotion=False, return_head=True,
                                               experimental=experimental)
 
         # convert voltage into 32 bits integer (ADC counts)
         volt_ranges = expand_list(head['volt_range'], head['ch_descr'])
@@ -303,15 +306,15 @@
                 previous_stations.append(tr.stats.station)
             tr.data = (tr.data + volt_range) / 2 * volt_range * 2 ** 32
             tr.data.astype(int)
 
         return cls(st, head, network)
 
 
-class FileBundleHandler(object):
+class USFHandler(object):
     def __init__(self, stream, catalog, inventory):
         self.stream = stream
         self.catalog = catalog
         self.inventory = inventory
 
     def write(self, filepath):
         filepath = Path(filepath)
@@ -391,14 +394,47 @@
                     tr.stats.network = inventory[0].code
                     traces.append(tr)
 
         out_stream = Stream(traces=traces)
 
         return cls(out_stream, catalog, inventory)
 
+    def patch_using_catalog(self, catalogue_line, network):
+        event_type = event.uquake_event_from_letter_id(
+            catalogue_line['EvtType'].values[0])
+        self.catalog[0].event_type = event_type
+        if catalogue_line['WF_Modified'].values[0]:
+            evaluation_mode = 'manual'
+            if catalogue_line['Rejected'].values[0]:
+                evaluation_status = 'rejected'
+            else:
+                evaluation_status = 'final'
+        else:
+            if catalogue_line['MultiProc'].values[0]:
+                if catalogue_line['Rejected'].values[0]:
+                    evaluation_status = 'rejected'
+                else:
+                    evaluation_status = 'confirmed'
+            elif catalogue_line['RemoteProc'].values[0]:
+                if catalogue_line['Rejected'].values[0]:
+                    evaluation_status = 'rejected'
+                else:
+                    evaluation_status = 'preliminary'
+
+        for pick in self.catalog[0].picks:
+            pick.evaluation_mode = evaluation_mode
+            pick.evaluation_status = evaluation_status
+
+        self.catalog[0].evaluation_mode = evaluation_mode
+        self.catalog[0].evaluation_status = evaluation_status
+
+        trg_id = catalogue_line['TrgID'].values[0]
+
+        self.catalog[0].resource_id.id = f'esg:/{network}/{trg_id}'
+
 
 def expand_list(to_expand, expand_to):
     """
     Expand a list to match the number of elements in another list while preserving
     correspondence.
 
     :param to_expand: The list to be expanded. It should have the same number of
```

### Comparing `pickled_carrots-0.1.7/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-0.2.0/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.1.7/pickled_carrots/waveforms.py` & `pickled_carrots-0.2.0/pickled_carrots/waveforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -700,14 +700,15 @@
     # use elevation 0 if z axis for event locations is down, up if 1
     head['use_elevation'] = struct.unpack('i', h309[38:42])[0]
     # head['input_voltage'] = struct.unpack('i',h309[64:68])[0]
     # offset to the waveform data from the beginning of the hsf file
     head['data_offs'] = struct.unpack('i', h309[92:96])[0]
     head['source'] = np.array(struct.unpack('3f', h309[112:124]))
     head['evtype'] = struct.unpack('h', h309[251:253])[0]
+    print(head['evtype'])
     head['time0'] = struct.unpack('f', h309[253:257])[0]
     head['knownt0'] = struct.unpack('f', h309[302:306])[0]
     head['fs'] = struct.unpack('i', h309[42:46])[0]
     head['t0_s'] = struct.unpack('i', h309[96:100])[0]
     head['t0_us'] = struct.unpack('i', h309[100:104])[0]
     # generate datetime of t0
     head['dt'] = datetime.fromtimestamp(head['t0_s']).replace(microsecond=head['t0_us'])
```

### Comparing `pickled_carrots-0.1.7/pyproject.toml` & `pickled_carrots-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pickled_carrots"
-version = "0.1.7"
+version = "0.2.0"
 description = ""
 authors = ["pickled cattots team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 plotly = "^5.14.1"
```

### Comparing `pickled_carrots-0.1.7/setup.py` & `pickled_carrots-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['pickled_carrots', 'pickled_carrots.vinegar', 'pickled_carrots.vinegar.tests']
 
 package_data = \
-{'': ['*']}
+{'': ['*'], 'pickled_carrots': ['resources/*']}
 
 install_requires = \
 ['SQLAlchemy>=2.0.13,<3.0.0',
  'boto3>=1.26.128,<2.0.0',
  'certifi>=2022.12.7,<2023.0.0',
  'cryptography>=40.0.2,<41.0.0',
  'h5py>=3.8.0,<4.0.0',
@@ -25,15 +25,15 @@
  'pytz>=2023.3,<2024.0',
  'shapely>=2.0.1,<3.0.0',
  'statsmodels>=0.14.0,<0.15.0',
  'uquake>=1.2.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pickled-carrots',
-    'version': '0.1.7',
+    'version': '0.2.0',
     'description': '',
     'long_description': "# ESG_Research\n\nThis repository contains Python and C# code which is used for various different functions. In this document we will go through what each folder contains.\n\n__Analytics_Notebooks__\n\nThis folder contains Jupyter notebooks which have various different functionalities. More notebooks can be found on the DataShare, under Frac4/Notebooks.\n\n&nbsp;\n\n\n__ESG-dash__\n\nA dash-based dashboard for evaluating sensor quality for mining sites.\n\n&nbsp;\n\n\n__ESG__\n\nThe main module folder for our Python codes. The files within this folder are used in most of our jupyter notebooks. More details on what each file contains can be found in the folder.\n\n&nbsp;\n\n__ITG-FMC__\n\nContains the tiltmeter processing dashboard written in Python, a Fiber processing C# app, a DPA and DPA-RTA C# app, and a copy of the Stress Inversion python package (which has since been merged into the main ESG repo.\n\n&nbsp;\n\n__Scripts__\n\nContains various Python scripts which are used to automated processes such as HypoDD or noise analysis.\n\n&nbsp;\n\n__build/lib, dist, esg_das, esg_dts__\n\nPython code for processing Fiber data. \n\n&nbsp;\n\n__Miscellaneous__\n\nThere are some additional files in this folder which are related to replicated anaconda environments. The requirements.txt file can be used to create ESG's default environment.\n",
     'author': 'pickled cattots team',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pickled_carrots-0.1.7/PKG-INFO` & `pickled_carrots-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickled-carrots
-Version: 0.1.7
+Version: 0.2.0
 Summary: 
 Author: pickled cattots team
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

