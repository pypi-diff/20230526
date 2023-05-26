# Comparing `tmp/pickled_carrots-0.2.1.tar.gz` & `tmp/pickled_carrots-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pickled_carrots-0.2.1.tar", max compression
+gzip compressed data, was "pickled_carrots-0.3.0.tar", max compression
```

## Comparing `pickled_carrots-0.2.1.tar` & `pickled_carrots-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,19 @@
--rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.2.1/README.md
--rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.2.1/pickled_carrots/DPData.py
--rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.2.1/pickled_carrots/DPPlot.py
--rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.2.1/pickled_carrots/DPUtil.py
--rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.2.1/pickled_carrots/__init__.py
--rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.2.1/pickled_carrots/database.py
--rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.2.1/pickled_carrots/dataclass.py
--rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.2.1/pickled_carrots/mathutil.py
--rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.2.1/pickled_carrots/plot.py
--rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-0.2.1/pickled_carrots/resources/event_type_lookup.pickle
--rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.2.1/pickled_carrots/vinegar/__init__.py
--rw-r--r--   0        0        0      192 2023-05-20 10:55:17.702165 pickled_carrots-0.2.1/pickled_carrots/vinegar/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0    13486 2023-05-24 16:56:20.344027 pickled_carrots-0.2.1/pickled_carrots/vinegar/__pycache__/core.cpython-39.pyc
--rw-r--r--   0        0        0     5668 2023-05-24 22:08:29.557038 pickled_carrots-0.2.1/pickled_carrots/vinegar/__pycache__/event.cpython-39.pyc
--rw-r--r--   0        0        0    17488 2023-05-26 09:41:49.479048 pickled_carrots-0.2.1/pickled_carrots/vinegar/core.py
--rw-r--r--   0        0        0     9239 2023-05-26 08:57:52.556544 pickled_carrots-0.2.1/pickled_carrots/vinegar/event.py
--rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.2.1/pickled_carrots/vinegar/inventory.py
--rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-0.2.1/pickled_carrots/vinegar/tests/test_read_hsf.py
--rw-r--r--   0        0        0   138987 2023-05-24 17:57:38.942953 pickled_carrots-0.2.1/pickled_carrots/waveforms.py
--rw-r--r--   0        0        0      678 2023-05-26 09:41:55.979350 pickled_carrots-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 pickled_carrots-0.2.1/setup.py
--rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1309 2023-05-19 17:43:26.854143 pickled_carrots-0.3.0/README.md
+-rw-r--r--   0        0        0    43329 2023-05-19 18:09:07.525014 pickled_carrots-0.3.0/pickled_carrots/DPData.py
+-rw-r--r--   0        0        0    89223 2023-05-19 18:09:07.461011 pickled_carrots-0.3.0/pickled_carrots/DPPlot.py
+-rw-r--r--   0        0        0    44076 2023-05-19 18:09:07.521014 pickled_carrots-0.3.0/pickled_carrots/DPUtil.py
+-rw-r--r--   0        0        0      464 2023-05-19 18:09:07.477012 pickled_carrots-0.3.0/pickled_carrots/__init__.py
+-rw-r--r--   0        0        0    90206 2023-05-19 18:09:07.517014 pickled_carrots-0.3.0/pickled_carrots/database.py
+-rw-r--r--   0        0        0    22267 2023-05-19 18:09:07.549015 pickled_carrots-0.3.0/pickled_carrots/dataclass.py
+-rw-r--r--   0        0        0    32719 2023-05-19 18:09:07.541015 pickled_carrots-0.3.0/pickled_carrots/mathutil.py
+-rw-r--r--   0        0        0    36342 2023-05-19 18:09:07.473012 pickled_carrots-0.3.0/pickled_carrots/plot.py
+-rwxr-xr-x   0        0        0     1034 2023-05-24 14:49:39.883632 pickled_carrots-0.3.0/pickled_carrots/resources/event_type_lookup.pickle
+-rw-r--r--   0        0        0       19 2023-05-20 10:55:16.214096 pickled_carrots-0.3.0/pickled_carrots/vinegar/__init__.py
+-rw-r--r--   0        0        0    12335 2023-05-26 12:26:44.670893 pickled_carrots-0.3.0/pickled_carrots/vinegar/core.py
+-rw-r--r--   0        0        0     9239 2023-05-26 08:57:52.556544 pickled_carrots-0.3.0/pickled_carrots/vinegar/event.py
+-rw-r--r--   0        0        0     1016 2023-05-19 18:44:55.447828 pickled_carrots-0.3.0/pickled_carrots/vinegar/inventory.py
+-rw-r--r--   0        0        0     1069 2023-05-25 14:36:27.387680 pickled_carrots-0.3.0/pickled_carrots/vinegar/tests/test_read_hsf.py
+-rw-r--r--   0        0        0   138987 2023-05-24 17:57:38.942953 pickled_carrots-0.3.0/pickled_carrots/waveforms.py
+-rw-r--r--   0        0        0      678 2023-05-26 12:43:24.597327 pickled_carrots-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2505 1970-01-01 00:00:00.000000 pickled_carrots-0.3.0/setup.py
+-rw-r--r--   0        0        0     2413 1970-01-01 00:00:00.000000 pickled_carrots-0.3.0/PKG-INFO
```

### Comparing `pickled_carrots-0.2.1/README.md` & `pickled_carrots-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/DPData.py` & `pickled_carrots-0.3.0/pickled_carrots/DPData.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/DPPlot.py` & `pickled_carrots-0.3.0/pickled_carrots/DPPlot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/DPUtil.py` & `pickled_carrots-0.3.0/pickled_carrots/DPUtil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/database.py` & `pickled_carrots-0.3.0/pickled_carrots/database.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/dataclass.py` & `pickled_carrots-0.3.0/pickled_carrots/dataclass.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/mathutil.py` & `pickled_carrots-0.3.0/pickled_carrots/mathutil.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/plot.py` & `pickled_carrots-0.3.0/pickled_carrots/plot.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/resources/event_type_lookup.pickle` & `pickled_carrots-0.3.0/pickled_carrots/resources/event_type_lookup.pickle`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/vinegar/core.py` & `pickled_carrots-0.3.0/pickled_carrots/vinegar/core.py`

 * *Files 23% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 import numpy as np
 from pathlib import Path
 from importlib import reload
 import tarfile
 from io import BytesIO
 import tempfile
 from pickled_carrots import waveforms
-import random
-import string
-from ipdb import set_trace
+from uquake.core.data_ensemble import SeismicDataEnsemble
 reload(event)
 
 lookups = HeaderLookups()
 
 
 class HSFHandler(object):
     def __init__(self, st, header, network, experimental=False):
@@ -276,16 +274,16 @@
         return evt
 
     @property
     def catalog(self):
         return Catalog(events=[self.event])
 
     @property
-    def usf_file(self):
-        return USFHandler(self.stream, self.catalog, self.inventory)
+    def sfs_object(self):
+        return SeismicDataEnsemble(self.stream, self.catalog, self.inventory)
 
     @classmethod
     def read(cls, file_path, network, experimental=False):
         if isinstance(file_path, Path):
             file_path = str(file_path)
         with tempfile.NamedTemporaryFile(delete=True) as tmpfile:
             st, head = waveforms.hsf_to_obspy(file_path, print_out=False,
@@ -302,136 +300,14 @@
                 previous_stations.append(tr.stats.station)
             tr.data = (tr.data + volt_range) / 2 * volt_range * 2 ** 32
             tr.data.astype(int)
 
         return cls(st, head, network)
 
 
-class USFHandler(object):
-    def __init__(self, stream, catalog, inventory):
-        self.stream = stream
-        self.catalog = catalog
-        self.inventory = inventory
-
-    def write(self, filepath):
-        filepath = Path(filepath)
-
-        traces = []
-
-        if len(self.inventory[0].code) > 2:
-            self.inventory[0].alternate_code = self.inventory[0].code[:2]
-        else:
-            self.inventory[0].alternate_code = self.inventory[0].code
-
-        alternate_station_codes = generate_unique_names(len(self.inventory[0].stations))
-        for station, asc in zip(self.inventory[0].stations, alternate_station_codes):
-            station.alternate_code = asc
-
-            st = self.stream.copy().select(station=station.code)
-            for tr in st:
-                tr.stats.station = station.alternate_code
-                tr.stats.network = self.inventory[0].alternate_code
-                traces.append(tr)
-
-        st = Stream(traces=traces)
-
-        with tarfile.open(filepath.with_suffix('.sfs'), 'w:gz') as tar:
-
-            catalog_bytes = BytesIO()
-            self.catalog.write(catalog_bytes, format='quakeml')
-            catalog_bytes.seek(0)
-            tarinfo = tarfile.TarInfo('catalog.xml')
-            tarinfo.size = len(catalog_bytes.getvalue())
-            tar.addfile(tarinfo, catalog_bytes)
-
-            stream_bytes = BytesIO()
-            st.write(stream_bytes, format='MSEED', encodings='STEIM2')
-            stream_bytes.seek(0)
-            tarinfo = tarfile.TarInfo('stream.mseed')
-            tarinfo.size = len(stream_bytes.getvalue())
-            tar.addfile(tarinfo, stream_bytes)
-
-            inventory_bytes = BytesIO()
-            self.inventory.write(inventory_bytes, format='stationxml')
-            inventory_bytes.seek(0)
-            tarinfo = tarfile.TarInfo('inventory.xml')
-            tarinfo.size = len(inventory_bytes.getvalue())
-            tar.addfile(tarinfo, inventory_bytes)
-
-        return None
-
-    @classmethod
-    def read(cls, file_path):
-        file_path = Path(file_path).with_suffix('.sfs')
-        catalog = None
-        stream = None
-        inventory = None
-
-        with tarfile.open(file_path, 'r:gz') as tar:
-            for member in tar.getmembers():
-                if member.isfile():
-                    file_bytes = tar.extractfile(member).read()
-                    file_name = member.name
-
-                    if file_name == 'catalog.xml':
-                        catalog = read_events(BytesIO(file_bytes), format='quakeml')
-                    elif file_name == 'stream.mseed':
-                        stream = read(BytesIO(file_bytes), format='MSEED')
-                    elif file_name == 'inventory.xml':
-                        with tempfile.NamedTemporaryFile(delete=True) as tmpfile:
-                            tmpfile.write(file_bytes)
-                            inventory = read_inventory(tmpfile.name, format='stationxml')
-
-        traces = []
-        if inventory and stream:
-            for station in inventory[0].stations:
-                st2 = stream.select(station=station.alternate_code)
-                for tr in st2:
-                    tr.stats.station = station.code
-                    tr.stats.network = inventory[0].code
-                    traces.append(tr)
-
-        out_stream = Stream(traces=traces)
-
-        return cls(out_stream, catalog, inventory)
-
-    def patch_using_catalog(self, catalogue_line, network):
-        event_type = event.uquake_event_from_letter_id(
-            catalogue_line['EvtType'].values[0])
-        self.catalog[0].event_type = event_type
-        if catalogue_line['WF_Modified'].values[0]:
-            evaluation_mode = 'manual'
-            if catalogue_line['Rejected'].values[0]:
-                evaluation_status = 'rejected'
-            else:
-                evaluation_status = 'final'
-        else:
-            if catalogue_line['MultiProc'].values[0]:
-                if catalogue_line['Rejected'].values[0]:
-                    evaluation_status = 'rejected'
-                else:
-                    evaluation_status = 'confirmed'
-            elif catalogue_line['RemoteProc'].values[0]:
-                if catalogue_line['Rejected'].values[0]:
-                    evaluation_status = 'rejected'
-                else:
-                    evaluation_status = 'preliminary'
-
-        for pick in self.catalog[0].picks:
-            pick.evaluation_mode = evaluation_mode
-            pick.evaluation_status = evaluation_status
-
-        self.catalog[0].evaluation_mode = evaluation_mode
-        self.catalog[0].evaluation_status = evaluation_status
-
-        trg_id = catalogue_line['TrgID'].values[0]
-
-        self.catalog[0].resource_id.id = f'esg:/{network}/{trg_id}'
-
-
 def expand_list(to_expand, expand_to):
     """
     Expand a list to match the number of elements in another list while preserving
     correspondence.
 
     :param to_expand: The list to be expanded. It should have the same number of
     elements as the number of unique elements in 'to_expand`.
@@ -455,30 +331,14 @@
     for item in expand_to:
         expanded_list.append(to_expand[count_dict[item] - 1])
         count_dict[item] -= 1
 
     return expanded_list
 
 
-def generate_unique_names(n):
-    """
-    Generate n number of unique 5-character names comprising only lower and upper case letters.
-
-    :param n: The number of unique names to generate.
-    :return: A list of n unique 5-character names.
-    """
-    names = set()  # Set to store unique names
-
-    while len(names) < n:
-        name = ''.join(random.choices(string.ascii_letters, k=5))
-        names.add(name)
-
-    return list(names)
-
-
 def generate_site_code(station_code, location, channel_code):
     return f'{station_code}.{location:02d}.{channel_code}'
 
 
 def station_name_converter(station_name):
     hash = hashlib.md5(station_name.encode('ascii')).hexdigest()
     mseed_station_code = hash[:5]
```

### Comparing `pickled_carrots-0.2.1/pickled_carrots/vinegar/event.py` & `pickled_carrots-0.3.0/pickled_carrots/vinegar/event.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/vinegar/inventory.py` & `pickled_carrots-0.3.0/pickled_carrots/vinegar/inventory.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/vinegar/tests/test_read_hsf.py` & `pickled_carrots-0.3.0/pickled_carrots/vinegar/tests/test_read_hsf.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pickled_carrots/waveforms.py` & `pickled_carrots-0.3.0/pickled_carrots/waveforms.py`

 * *Files identical despite different names*

### Comparing `pickled_carrots-0.2.1/pyproject.toml` & `pickled_carrots-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pickled_carrots"
-version = "0.2.1"
+version = "0.3.0"
 description = ""
 authors = ["pickled cattots team"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 plotly = "^5.14.1"
```

### Comparing `pickled_carrots-0.2.1/setup.py` & `pickled_carrots-0.3.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -25,15 +25,15 @@
  'pytz>=2023.3,<2024.0',
  'shapely>=2.0.1,<3.0.0',
  'statsmodels>=0.14.0,<0.15.0',
  'uquake>=1.2.4,<2.0.0']
 
 setup_kwargs = {
     'name': 'pickled-carrots',
-    'version': '0.2.1',
+    'version': '0.3.0',
     'description': '',
     'long_description': "# ESG_Research\n\nThis repository contains Python and C# code which is used for various different functions. In this document we will go through what each folder contains.\n\n__Analytics_Notebooks__\n\nThis folder contains Jupyter notebooks which have various different functionalities. More notebooks can be found on the DataShare, under Frac4/Notebooks.\n\n&nbsp;\n\n\n__ESG-dash__\n\nA dash-based dashboard for evaluating sensor quality for mining sites.\n\n&nbsp;\n\n\n__ESG__\n\nThe main module folder for our Python codes. The files within this folder are used in most of our jupyter notebooks. More details on what each file contains can be found in the folder.\n\n&nbsp;\n\n__ITG-FMC__\n\nContains the tiltmeter processing dashboard written in Python, a Fiber processing C# app, a DPA and DPA-RTA C# app, and a copy of the Stress Inversion python package (which has since been merged into the main ESG repo.\n\n&nbsp;\n\n__Scripts__\n\nContains various Python scripts which are used to automated processes such as HypoDD or noise analysis.\n\n&nbsp;\n\n__build/lib, dist, esg_das, esg_dts__\n\nPython code for processing Fiber data. \n\n&nbsp;\n\n__Miscellaneous__\n\nThere are some additional files in this folder which are related to replicated anaconda environments. The requirements.txt file can be used to create ESG's default environment.\n",
     'author': 'pickled cattots team',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pickled_carrots-0.2.1/PKG-INFO` & `pickled_carrots-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pickled-carrots
-Version: 0.2.1
+Version: 0.3.0
 Summary: 
 Author: pickled cattots team
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

