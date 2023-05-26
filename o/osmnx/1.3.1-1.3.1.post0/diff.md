# Comparing `tmp/osmnx-1.3.1.tar.gz` & `tmp/osmnx-1.3.1.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osmnx-1.3.1.tar", last modified: Wed May 24 21:55:50 2023, max compression
+gzip compressed data, was "osmnx-1.3.1.post0.tar", last modified: Fri May 26 21:13:03 2023, max compression
```

## Comparing `osmnx-1.3.1.tar` & `osmnx-1.3.1.post0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxrwxr-x   0 geoff     (1000) geoff     (1000)        0 2023-05-24 21:55:50.437286 osmnx-1.3.1/
--rw-r--r--   0 geoff     (1000) geoff     (1000)    19206 2023-05-24 21:42:36.000000 osmnx-1.3.1/CHANGELOG.md
--rw-r--r--   0 geoff     (1000) geoff     (1000)     1111 2022-12-22 03:13:01.000000 osmnx-1.3.1/LICENSE.txt
--rw-rw-r--   0 geoff     (1000) geoff     (1000)       45 2022-12-14 16:25:06.000000 osmnx-1.3.1/MANIFEST.in
--rw-rw-r--   0 geoff     (1000) geoff     (1000)     2268 2023-05-24 21:55:50.437286 osmnx-1.3.1/PKG-INFO
--rw-r--r--   0 geoff     (1000) geoff     (1000)     4357 2022-12-28 21:55:23.000000 osmnx-1.3.1/README.md
-drwxrwxr-x   0 geoff     (1000) geoff     (1000)        0 2023-05-24 21:55:50.437286 osmnx-1.3.1/osmnx/
--rw-r--r--   0 geoff     (1000) geoff     (1000)       73 2022-09-03 08:24:38.000000 osmnx-1.3.1/osmnx/__init__.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)     1993 2023-05-22 22:51:40.000000 osmnx-1.3.1/osmnx/_api.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)      505 2022-12-17 00:29:35.000000 osmnx-1.3.1/osmnx/_errors.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)     1758 2022-12-17 00:29:35.000000 osmnx-1.3.1/osmnx/_polygon_features.py
--rw-r--r--   0 geoff     (1000) geoff     (1000)       52 2023-05-24 21:42:36.000000 osmnx-1.3.1/osmnx/_version.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    12165 2023-05-22 22:51:40.000000 osmnx-1.3.1/osmnx/bearing.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    17675 2023-05-11 18:19:00.000000 osmnx-1.3.1/osmnx/distance.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    29369 2023-05-16 15:42:19.000000 osmnx-1.3.1/osmnx/downloader.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)     9178 2022-12-17 00:29:35.000000 osmnx-1.3.1/osmnx/elevation.py
--rw-r--r--   0 geoff     (1000) geoff     (1000)     5725 2023-05-24 16:21:01.000000 osmnx-1.3.1/osmnx/folium.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)     8406 2023-01-14 20:32:17.000000 osmnx-1.3.1/osmnx/geocoder.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    39964 2023-05-24 17:58:29.000000 osmnx-1.3.1/osmnx/geometries.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    29082 2023-05-24 17:58:29.000000 osmnx-1.3.1/osmnx/graph.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    14242 2023-03-20 17:40:38.000000 osmnx-1.3.1/osmnx/io.py
--rw-r--r--   0 geoff     (1000) geoff     (1000)    15244 2023-05-24 21:22:23.000000 osmnx-1.3.1/osmnx/osm_xml.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    27017 2023-05-22 22:51:40.000000 osmnx-1.3.1/osmnx/plot.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)     6343 2022-12-17 00:29:36.000000 osmnx-1.3.1/osmnx/projection.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)     7996 2023-05-22 22:51:40.000000 osmnx-1.3.1/osmnx/settings.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    25685 2023-03-20 17:40:38.000000 osmnx-1.3.1/osmnx/simplification.py
--rw-r--r--   0 geoff     (1000) geoff     (1000)     9144 2023-05-22 03:49:01.000000 osmnx-1.3.1/osmnx/speed.py
--rw-r--r--   0 geoff     (1000) geoff     (1000)    12691 2022-12-22 03:13:01.000000 osmnx-1.3.1/osmnx/stats.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)     6740 2022-12-17 00:29:36.000000 osmnx-1.3.1/osmnx/truncate.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    10547 2023-03-20 17:40:38.000000 osmnx-1.3.1/osmnx/utils.py
--rw-rw-r--   0 geoff     (1000) geoff     (1000)    16245 2023-02-22 17:24:42.000000 osmnx-1.3.1/osmnx/utils_geo.py
--rw-r--r--   0 geoff     (1000) geoff     (1000)    17793 2023-05-24 16:21:01.000000 osmnx-1.3.1/osmnx/utils_graph.py
-drwxrwxr-x   0 geoff     (1000) geoff     (1000)        0 2023-05-24 21:55:50.437286 osmnx-1.3.1/osmnx.egg-info/
--rw-r--r--   0 geoff     (1000) geoff     (1000)     2268 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/PKG-INFO
--rw-r--r--   0 geoff     (1000) geoff     (1000)      691 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/SOURCES.txt
--rw-r--r--   0 geoff     (1000) geoff     (1000)        1 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/dependency_links.txt
--rw-r--r--   0 geoff     (1000) geoff     (1000)      208 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/requires.txt
--rw-r--r--   0 geoff     (1000) geoff     (1000)        6 2023-05-24 21:55:50.000000 osmnx-1.3.1/osmnx.egg-info/top_level.txt
--rw-r--r--   0 geoff     (1000) geoff     (1000)      110 2023-05-24 16:21:28.000000 osmnx-1.3.1/requirements.txt
--rw-rw-r--   0 geoff     (1000) geoff     (1000)      405 2023-05-24 21:55:50.437286 osmnx-1.3.1/setup.cfg
--rw-r--r--   0 geoff     (1000) geoff     (1000)     2961 2023-05-24 21:42:36.000000 osmnx-1.3.1/setup.py
-drwxrwxr-x   0 geoff     (1000) geoff     (1000)        0 2023-05-24 21:55:50.437286 osmnx-1.3.1/tests/
--rwxr--r--   0 geoff     (1000) geoff     (1000)    20089 2023-05-24 17:58:29.000000 osmnx-1.3.1/tests/test_osmnx.py
+drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-05-26 21:13:03.236554 osmnx-1.3.1.post0/
+-rw-r--r--   0 geoff      (501) staff       (20)    19296 2023-05-26 20:50:26.000000 osmnx-1.3.1.post0/CHANGELOG.md
+-rw-r--r--   0 geoff      (501) staff       (20)     1111 2022-12-22 03:13:01.000000 osmnx-1.3.1.post0/LICENSE.txt
+-rw-r--r--   0 geoff      (501) staff       (20)       45 2022-12-14 16:25:06.000000 osmnx-1.3.1.post0/MANIFEST.in
+-rw-r--r--   0 geoff      (501) staff       (20)     2324 2023-05-26 21:13:03.236627 osmnx-1.3.1.post0/PKG-INFO
+-rw-r--r--   0 geoff      (501) staff       (20)     4357 2022-12-28 21:55:23.000000 osmnx-1.3.1.post0/README.md
+drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-05-26 21:13:03.235529 osmnx-1.3.1.post0/osmnx/
+-rw-r--r--   0 geoff      (501) staff       (20)       73 2022-09-03 08:24:38.000000 osmnx-1.3.1.post0/osmnx/__init__.py
+-rw-r--r--   0 geoff      (501) staff       (20)     1993 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/_api.py
+-rw-r--r--   0 geoff      (501) staff       (20)      505 2022-12-17 00:29:35.000000 osmnx-1.3.1.post0/osmnx/_errors.py
+-rw-r--r--   0 geoff      (501) staff       (20)     1758 2022-12-17 00:29:35.000000 osmnx-1.3.1.post0/osmnx/_polygon_features.py
+-rw-r--r--   0 geoff      (501) staff       (20)       58 2023-05-26 20:46:22.000000 osmnx-1.3.1.post0/osmnx/_version.py
+-rw-r--r--   0 geoff      (501) staff       (20)    12165 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/bearing.py
+-rw-r--r--   0 geoff      (501) staff       (20)    17675 2023-05-11 18:07:46.000000 osmnx-1.3.1.post0/osmnx/distance.py
+-rw-r--r--   0 geoff      (501) staff       (20)    29369 2023-05-22 03:49:01.000000 osmnx-1.3.1.post0/osmnx/downloader.py
+-rw-r--r--   0 geoff      (501) staff       (20)     9178 2022-12-17 00:29:35.000000 osmnx-1.3.1.post0/osmnx/elevation.py
+-rw-r--r--   0 geoff      (501) staff       (20)     5725 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/folium.py
+-rw-r--r--   0 geoff      (501) staff       (20)     8406 2023-01-14 20:32:17.000000 osmnx-1.3.1.post0/osmnx/geocoder.py
+-rw-r--r--   0 geoff      (501) staff       (20)    39964 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/geometries.py
+-rw-r--r--   0 geoff      (501) staff       (20)    29082 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/graph.py
+-rw-r--r--   0 geoff      (501) staff       (20)    14242 2023-03-20 17:40:38.000000 osmnx-1.3.1.post0/osmnx/io.py
+-rw-r--r--   0 geoff      (501) staff       (20)    15244 2023-05-24 23:37:40.000000 osmnx-1.3.1.post0/osmnx/osm_xml.py
+-rw-r--r--   0 geoff      (501) staff       (20)    27017 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/plot.py
+-rw-r--r--   0 geoff      (501) staff       (20)     6343 2022-12-17 00:29:36.000000 osmnx-1.3.1.post0/osmnx/projection.py
+-rw-r--r--   0 geoff      (501) staff       (20)     7996 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/settings.py
+-rw-r--r--   0 geoff      (501) staff       (20)    25685 2023-03-20 17:40:38.000000 osmnx-1.3.1.post0/osmnx/simplification.py
+-rw-r--r--   0 geoff      (501) staff       (20)     9144 2023-05-22 03:49:01.000000 osmnx-1.3.1.post0/osmnx/speed.py
+-rw-r--r--   0 geoff      (501) staff       (20)    12691 2022-12-22 03:13:01.000000 osmnx-1.3.1.post0/osmnx/stats.py
+-rw-r--r--   0 geoff      (501) staff       (20)     6740 2022-12-17 00:29:36.000000 osmnx-1.3.1.post0/osmnx/truncate.py
+-rw-r--r--   0 geoff      (501) staff       (20)    10547 2023-03-20 17:40:38.000000 osmnx-1.3.1.post0/osmnx/utils.py
+-rw-r--r--   0 geoff      (501) staff       (20)    16245 2023-02-22 17:24:42.000000 osmnx-1.3.1.post0/osmnx/utils_geo.py
+-rw-r--r--   0 geoff      (501) staff       (20)    17793 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/osmnx/utils_graph.py
+drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-05-26 21:13:03.236242 osmnx-1.3.1.post0/osmnx.egg-info/
+-rw-r--r--   0 geoff      (501) staff       (20)     2324 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/PKG-INFO
+-rw-r--r--   0 geoff      (501) staff       (20)      691 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/SOURCES.txt
+-rw-r--r--   0 geoff      (501) staff       (20)        1 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/dependency_links.txt
+-rw-r--r--   0 geoff      (501) staff       (20)      208 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/requires.txt
+-rw-r--r--   0 geoff      (501) staff       (20)        6 2023-05-26 21:13:03.000000 osmnx-1.3.1.post0/osmnx.egg-info/top_level.txt
+-rw-r--r--   0 geoff      (501) staff       (20)      110 2023-05-24 23:37:40.000000 osmnx-1.3.1.post0/requirements.txt
+-rw-r--r--   0 geoff      (501) staff       (20)      405 2023-05-26 21:13:03.236984 osmnx-1.3.1.post0/setup.cfg
+-rw-r--r--   0 geoff      (501) staff       (20)     3012 2023-05-26 20:46:40.000000 osmnx-1.3.1.post0/setup.py
+drwxr-xr-x   0 geoff      (501) staff       (20)        0 2023-05-26 21:13:03.236392 osmnx-1.3.1.post0/tests/
+-rwxr-xr-x   0 geoff      (501) staff       (20)    20089 2023-05-26 20:41:18.000000 osmnx-1.3.1.post0/tests/test_osmnx.py
```

### Comparing `osmnx-1.3.1/CHANGELOG.md` & `osmnx-1.3.1.post0/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Change log
 
+## 1.3.1.post0 (2023-05-26)
+
+  - add Python 3.8 compatibility back for one final release
+
 ## 1.3.1 (2023-05-24)
 
   - improve DNS resolution when using proxies or on networks blocking DNS-over-HTTPS
   - improve processing of per-lane values when adding edge speeds
   - improve file writing in save_graph_xml function
   - ensure node coordinates are non-null and covertible to float in the add_edge_lengths function
   - ignore ways tagged highway=no or highway=razed in built-in filters
```

### Comparing `osmnx-1.3.1/LICENSE.txt` & `osmnx-1.3.1.post0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/PKG-INFO` & `osmnx-1.3.1.post0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.3.1
+Version: 1.3.1.post0
 Summary: Retrieve, model, analyze, and visualize OpenStreetMap street networks and other spatial data
 Home-page: https://github.com/gboeing/osmnx
 Author: Geoff Boeing
 Author-email: boeing@usc.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,18 +14,19 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: entropy
 Provides-Extra: nearest_neighbor
 Provides-Extra: raster
 Provides-Extra: web_map
 License-File: LICENSE.txt
```

### Comparing `osmnx-1.3.1/README.md` & `osmnx-1.3.1.post0/README.md`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/_api.py` & `osmnx-1.3.1.post0/osmnx/_api.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/_polygon_features.py` & `osmnx-1.3.1.post0/osmnx/_polygon_features.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/bearing.py` & `osmnx-1.3.1.post0/osmnx/bearing.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/distance.py` & `osmnx-1.3.1.post0/osmnx/distance.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/downloader.py` & `osmnx-1.3.1.post0/osmnx/downloader.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/elevation.py` & `osmnx-1.3.1.post0/osmnx/elevation.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/folium.py` & `osmnx-1.3.1.post0/osmnx/folium.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/geocoder.py` & `osmnx-1.3.1.post0/osmnx/geocoder.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/geometries.py` & `osmnx-1.3.1.post0/osmnx/geometries.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/graph.py` & `osmnx-1.3.1.post0/osmnx/graph.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/io.py` & `osmnx-1.3.1.post0/osmnx/io.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/osm_xml.py` & `osmnx-1.3.1.post0/osmnx/osm_xml.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/plot.py` & `osmnx-1.3.1.post0/osmnx/plot.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/projection.py` & `osmnx-1.3.1.post0/osmnx/projection.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/settings.py` & `osmnx-1.3.1.post0/osmnx/settings.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/simplification.py` & `osmnx-1.3.1.post0/osmnx/simplification.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/speed.py` & `osmnx-1.3.1.post0/osmnx/speed.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/stats.py` & `osmnx-1.3.1.post0/osmnx/stats.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/truncate.py` & `osmnx-1.3.1.post0/osmnx/truncate.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/utils.py` & `osmnx-1.3.1.post0/osmnx/utils.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/utils_geo.py` & `osmnx-1.3.1.post0/osmnx/utils_geo.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx/utils_graph.py` & `osmnx-1.3.1.post0/osmnx/utils_graph.py`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/osmnx.egg-info/PKG-INFO` & `osmnx-1.3.1.post0/osmnx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osmnx
-Version: 1.3.1
+Version: 1.3.1.post0
 Summary: Retrieve, model, analyze, and visualize OpenStreetMap street networks and other spatial data
 Home-page: https://github.com/gboeing/osmnx
 Author: Geoff Boeing
 Author-email: boeing@usc.edu
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,18 +14,19 @@
 Classifier: Topic :: Scientific/Engineering :: GIS
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: entropy
 Provides-Extra: nearest_neighbor
 Provides-Extra: raster
 Provides-Extra: web_map
 License-File: LICENSE.txt
```

### Comparing `osmnx-1.3.1/osmnx.egg-info/SOURCES.txt` & `osmnx-1.3.1.post0/osmnx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osmnx-1.3.1/setup.py` & `osmnx-1.3.1.post0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,14 +39,15 @@
     "Topic :: Scientific/Engineering :: GIS",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Scientific/Engineering :: Physics",
     "Topic :: Scientific/Engineering :: Mathematics",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 DESC = (
     "Retrieve, model, analyze, and visualize OpenStreetMap street networks and other spatial data"
@@ -58,26 +59,26 @@
 else:
     with open("requirements.txt") as f:
         INSTALL_REQUIRES = [line.strip() for line in f.readlines()]
 
 # now call setup
 setup(
     name="osmnx",
-    version="1.3.1",
+    version="1.3.1.post0",
     description=DESC,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/x-rst",
     classifiers=CLASSIFIERS,
     url="https://github.com/gboeing/osmnx",
     author="Geoff Boeing",
     author_email="boeing@usc.edu",
     license="MIT",
     platforms="any",
     packages=["osmnx"],
-    python_requires=">=3.9",
+    python_requires=">=3.8",
     install_requires=INSTALL_REQUIRES,
     extras_require={
         "entropy": ["scipy"],
         "nearest_neighbor": ["scikit-learn", "scipy"],
         "raster": ["gdal", "rasterio"],
         "web_map": ["folium"],
     },
```

### Comparing `osmnx-1.3.1/tests/test_osmnx.py` & `osmnx-1.3.1.post0/tests/test_osmnx.py`

 * *Files identical despite different names*

