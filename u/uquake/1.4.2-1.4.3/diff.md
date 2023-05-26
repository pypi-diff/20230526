# Comparing `tmp/uquake-1.4.2.tar.gz` & `tmp/uquake-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uquake-1.4.2.tar", max compression
+gzip compressed data, was "uquake-1.4.3.tar", max compression
```

## Comparing `uquake-1.4.2.tar` & `uquake-1.4.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0     2399 2023-05-26 13:03:17.308675 uquake-1.4.2/pyproject.toml
--rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.4.2/uquake/__init__.py
--rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/__init__.py
--rw-r--r--   0        0        0     3978 2023-05-26 12:59:35.034368 uquake-1.4.2/uquake/core/data_ensemble.py
--rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/decorators.py
--rw-r--r--   0        0        0    35168 2023-05-26 12:44:33.128508 uquake-1.4.2/uquake/core/event.py
--rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/focal_mechanism.py
--rw-r--r--   0        0        0    38730 2023-05-26 12:30:49.530264 uquake-1.4.2/uquake/core/inventory.py
--rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/logging.py
--rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.4.2/uquake/core/stream.py
--rw-r--r--   0        0        0     5308 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/trace.py
--rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/util/__init__.py
--rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/util/base.py
--rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/util/decorator.py
--rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.4.2/uquake/core/util/requests.py
--rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/core/util/tools.py
--rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/grid/__init__.py
--rw-r--r--   0        0        0    22173 2023-04-27 00:23:45.744173 uquake-1.4.2/uquake/grid/base.py
--rw-r--r--   0        0        0     4660 2023-05-06 10:03:22.429231 uquake-1.4.2/uquake/grid/hdf5.py
--rw-r--r--   0        0        0    47247 2023-04-27 00:26:03.338550 uquake-1.4.2/uquake/grid/nlloc.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/imaging/__init__.py
--rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.4.2/uquake/imaging/plot.py
--rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.4.2/uquake/imaging/stereonet.py
--rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/imaging/waveform.py
--rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/__init__.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/event/__init__.py
--rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/event/core.py
--rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/grid/__init__.py
--rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/grid/core.py
--rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/inventory/__init__.py
--rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/inventory/core.py
--rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/waveform/__init__.py
--rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/io/waveform/core.py
--rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/nlloc/__init__.py
--rw-r--r--   0        0        0    48293 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/nlloc/nlloc.py
--rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/waveform/__init__.py
--rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/waveform/amp_measures.py
--rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/waveform/mag.py
--rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/waveform/mag_utils.py
--rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/waveform/parseval_utils.py
--rw-r--r--   0        0        0    21331 2023-05-16 01:15:39.357070 uquake-1.4.2/uquake/waveform/pick.py
--rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.4.2/uquake/waveform/simple_mag.py
--rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/waveform/smom_measure.py
--rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/waveform/smom_measure_legacy.py
--rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.4.2/uquake/waveform/transforms.py
--rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 uquake-1.4.2/setup.py
--rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 uquake-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0     2399 2023-05-26 13:46:39.889408 uquake-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-01-25 01:11:29.666160 uquake-1.4.3/uquake/__init__.py
+-rw-r--r--   0        0        0      191 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/__init__.py
+-rw-r--r--   0        0        0     4003 2023-05-26 13:46:22.732612 uquake-1.4.3/uquake/core/data_ensemble.py
+-rw-r--r--   0        0        0      658 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/decorators.py
+-rw-r--r--   0        0        0    35168 2023-05-26 12:44:33.128508 uquake-1.4.3/uquake/core/event.py
+-rw-r--r--   0        0        0     6233 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/focal_mechanism.py
+-rw-r--r--   0        0        0    38730 2023-05-26 12:30:49.530264 uquake-1.4.3/uquake/core/inventory.py
+-rw-r--r--   0        0        0      239 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/logging.py
+-rw-r--r--   0        0        0    13782 2023-01-25 01:08:23.561456 uquake-1.4.3/uquake/core/stream.py
+-rw-r--r--   0        0        0     5308 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/trace.py
+-rw-r--r--   0        0        0       67 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/util/__init__.py
+-rw-r--r--   0        0        0     4206 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/util/base.py
+-rw-r--r--   0        0        0     5713 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/util/decorator.py
+-rw-r--r--   0        0        0      620 2023-04-16 18:19:34.782672 uquake-1.4.3/uquake/core/util/requests.py
+-rw-r--r--   0        0        0    13768 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/core/util/tools.py
+-rw-r--r--   0        0        0       28 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/grid/__init__.py
+-rw-r--r--   0        0        0    22173 2023-04-27 00:23:45.744173 uquake-1.4.3/uquake/grid/base.py
+-rw-r--r--   0        0        0     4660 2023-05-06 10:03:22.429231 uquake-1.4.3/uquake/grid/hdf5.py
+-rw-r--r--   0        0        0    47247 2023-04-27 00:26:03.338550 uquake-1.4.3/uquake/grid/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/imaging/__init__.py
+-rw-r--r--   0        0        0    10043 2023-03-08 09:37:25.089762 uquake-1.4.3/uquake/imaging/plot.py
+-rw-r--r--   0        0        0     2474 2023-01-15 00:23:22.715786 uquake-1.4.3/uquake/imaging/stereonet.py
+-rw-r--r--   0        0        0    59743 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/imaging/waveform.py
+-rw-r--r--   0        0        0      423 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/event/__init__.py
+-rw-r--r--   0        0        0     3417 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/event/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/grid/__init__.py
+-rw-r--r--   0        0        0     8496 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/grid/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/inventory/__init__.py
+-rw-r--r--   0        0        0     6531 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/inventory/core.py
+-rw-r--r--   0        0        0       20 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/waveform/__init__.py
+-rw-r--r--   0        0        0     9262 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/io/waveform/core.py
+-rw-r--r--   0        0        0       21 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/nlloc/__init__.py
+-rw-r--r--   0        0        0    48293 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/nlloc/nlloc.py
+-rw-r--r--   0        0        0        0 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/waveform/__init__.py
+-rw-r--r--   0        0        0    34528 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/waveform/amp_measures.py
+-rw-r--r--   0        0        0    15799 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/waveform/mag.py
+-rw-r--r--   0        0        0     5354 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/waveform/mag_utils.py
+-rw-r--r--   0        0        0     2827 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/waveform/parseval_utils.py
+-rw-r--r--   0        0        0    21331 2023-05-16 01:15:39.357070 uquake-1.4.3/uquake/waveform/pick.py
+-rw-r--r--   0        0        0    45461 2023-04-04 17:02:48.691928 uquake-1.4.3/uquake/waveform/simple_mag.py
+-rw-r--r--   0        0        0    32225 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/waveform/smom_measure.py
+-rw-r--r--   0        0        0    33065 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/waveform/smom_measure_legacy.py
+-rw-r--r--   0        0        0     4456 2023-01-15 00:23:22.719786 uquake-1.4.3/uquake/waveform/transforms.py
+-rw-r--r--   0        0        0     2919 1970-01-01 00:00:00.000000 uquake-1.4.3/setup.py
+-rw-r--r--   0        0        0     1152 1970-01-01 00:00:00.000000 uquake-1.4.3/PKG-INFO
```

### Comparing `uquake-1.4.2/pyproject.toml` & `uquake-1.4.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "uquake"
-version = "1.4.2"
+version = "1.4.3"
 description = "extension of the ObsPy library for local seismicity"
 authors = ["uQuake development team <dev@uQuake.org>"]
 license = "MIT"
 
 # poetry config virtualenvs.create false; poetry env info
 
 [tool.poetry.dependencies]
```

### Comparing `uquake-1.4.2/uquake/core/data_ensemble.py` & `uquake-1.4.3/uquake/core/data_ensemble.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from uquake.core.stream import Stream
 from uquake.core.event import Catalog
 from uquake.core.inventory import Inventory
+from pathlib import Path
 
 
 class SeismicDataEnsemble(object):
     def __init__(self, stream: Stream, catalog: Catalog, inventory: Inventory):
         self.stream = stream
         self.catalog = catalog
         self.inventory = inventory
```

### Comparing `uquake-1.4.2/uquake/core/decorators.py` & `uquake-1.4.3/uquake/core/decorators.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/event.py` & `uquake-1.4.3/uquake/core/event.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/focal_mechanism.py` & `uquake-1.4.3/uquake/core/focal_mechanism.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/inventory.py` & `uquake-1.4.3/uquake/core/inventory.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/stream.py` & `uquake-1.4.3/uquake/core/stream.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/trace.py` & `uquake-1.4.3/uquake/core/trace.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/util/base.py` & `uquake-1.4.3/uquake/core/util/base.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/util/decorator.py` & `uquake-1.4.3/uquake/core/util/decorator.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/util/requests.py` & `uquake-1.4.3/uquake/core/util/requests.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/core/util/tools.py` & `uquake-1.4.3/uquake/core/util/tools.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/grid/base.py` & `uquake-1.4.3/uquake/grid/base.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/grid/hdf5.py` & `uquake-1.4.3/uquake/grid/hdf5.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/grid/nlloc.py` & `uquake-1.4.3/uquake/grid/nlloc.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/imaging/plot.py` & `uquake-1.4.3/uquake/imaging/plot.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/imaging/stereonet.py` & `uquake-1.4.3/uquake/imaging/stereonet.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/imaging/waveform.py` & `uquake-1.4.3/uquake/imaging/waveform.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/io/event/core.py` & `uquake-1.4.3/uquake/io/event/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/io/grid/core.py` & `uquake-1.4.3/uquake/io/grid/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/io/inventory/core.py` & `uquake-1.4.3/uquake/io/inventory/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/io/waveform/core.py` & `uquake-1.4.3/uquake/io/waveform/core.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/nlloc/nlloc.py` & `uquake-1.4.3/uquake/nlloc/nlloc.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/amp_measures.py` & `uquake-1.4.3/uquake/waveform/amp_measures.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/mag.py` & `uquake-1.4.3/uquake/waveform/mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/mag_utils.py` & `uquake-1.4.3/uquake/waveform/mag_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/parseval_utils.py` & `uquake-1.4.3/uquake/waveform/parseval_utils.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/pick.py` & `uquake-1.4.3/uquake/waveform/pick.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/simple_mag.py` & `uquake-1.4.3/uquake/waveform/simple_mag.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/smom_measure.py` & `uquake-1.4.3/uquake/waveform/smom_measure.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/smom_measure_legacy.py` & `uquake-1.4.3/uquake/waveform/smom_measure_legacy.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/uquake/waveform/transforms.py` & `uquake-1.4.3/uquake/waveform/transforms.py`

 * *Files identical despite different names*

### Comparing `uquake-1.4.2/setup.py` & `uquake-1.4.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
  'uquake.io.waveform.IMS_ASCII': ['readFormat = '
                                   'uquake.io.waveform:read_IMS_ASCII'],
  'uquake.io.waveform.TEXCEL_CSV': ['readFormat = '
                                    'uquake.io.waveform:read_TEXCEL_CSV']}
 
 setup_kwargs = {
     'name': 'uquake',
-    'version': '1.4.2',
+    'version': '1.4.3',
     'description': 'extension of the ObsPy library for local seismicity',
     'long_description': 'None',
     'author': 'uQuake development team',
     'author_email': 'dev@uQuake.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `uquake-1.4.2/PKG-INFO` & `uquake-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uquake
-Version: 1.4.2
+Version: 1.4.3
 Summary: extension of the ObsPy library for local seismicity
 License: MIT
 Author: uQuake development team
 Author-email: dev@uQuake.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

