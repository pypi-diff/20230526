# Comparing `tmp/xrmap-0.0.7.tar.gz` & `tmp/xrmap-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xrmap-0.0.7.tar", last modified: Fri May 26 11:59:02 2023, max compression
+gzip compressed data, was "xrmap-0.0.8.tar", last modified: Fri May 26 12:03:03 2023, max compression
```

## Comparing `xrmap-0.0.7.tar` & `xrmap-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-26 11:59:02.809445 xrmap-0.0.7/
--rw-r--r--   0 javier     (501) staff       (20)      939 2023-05-26 11:59:02.809609 xrmap-0.0.7/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)     1066 2023-05-26 11:59:02.811394 xrmap-0.0.7/setup.cfg
--rw-r--r--   0 javier     (501) staff       (20)      102 2023-04-26 13:39:17.000000 xrmap-0.0.7/setup.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-26 11:59:02.803275 xrmap-0.0.7/xarray_map/
--rw-r--r--   0 javier     (501) staff       (20)      112 2023-04-26 13:19:23.000000 xrmap-0.0.7/xarray_map/__init__.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-26 11:59:02.803889 xrmap-0.0.7/xarray_map/kmz/
--rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-26 11:34:33.000000 xrmap-0.0.7/xarray_map/kmz/__init__.py
--rw-r--r--   0 javier     (501) staff       (20)     1438 2023-05-26 11:58:44.000000 xrmap-0.0.7/xarray_map/plot_folium.py
-drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-26 11:59:02.809219 xrmap-0.0.7/xrmap.egg-info/
--rw-r--r--   0 javier     (501) staff       (20)      939 2023-05-26 11:59:02.000000 xrmap-0.0.7/xrmap.egg-info/PKG-INFO
--rw-r--r--   0 javier     (501) staff       (20)      266 2023-05-26 11:59:02.000000 xrmap-0.0.7/xrmap.egg-info/SOURCES.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-05-26 11:59:02.000000 xrmap-0.0.7/xrmap.egg-info/dependency_links.txt
--rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-28 08:20:56.000000 xrmap-0.0.7/xrmap.egg-info/not-zip-safe
--rw-r--r--   0 javier     (501) staff       (20)       31 2023-05-26 11:59:02.000000 xrmap-0.0.7/xrmap.egg-info/requires.txt
--rw-r--r--   0 javier     (501) staff       (20)       11 2023-05-26 11:59:02.000000 xrmap-0.0.7/xrmap.egg-info/top_level.txt
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-26 12:03:03.867934 xrmap-0.0.8/
+-rw-r--r--   0 javier     (501) staff       (20)      939 2023-05-26 12:03:03.868019 xrmap-0.0.8/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)     1066 2023-05-26 12:03:03.868994 xrmap-0.0.8/setup.cfg
+-rw-r--r--   0 javier     (501) staff       (20)      102 2023-04-26 13:39:17.000000 xrmap-0.0.8/setup.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-26 12:03:03.848789 xrmap-0.0.8/xarray_map/
+-rw-r--r--   0 javier     (501) staff       (20)      112 2023-04-26 13:19:23.000000 xrmap-0.0.8/xarray_map/__init__.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-26 12:03:03.849109 xrmap-0.0.8/xarray_map/kmz/
+-rw-r--r--   0 javier     (501) staff       (20)        0 2023-04-26 11:34:33.000000 xrmap-0.0.8/xarray_map/kmz/__init__.py
+-rw-r--r--   0 javier     (501) staff       (20)     1403 2023-05-26 12:02:14.000000 xrmap-0.0.8/xarray_map/plot_folium.py
+drwxr-xr-x   0 javier     (501) staff       (20)        0 2023-05-26 12:03:03.867797 xrmap-0.0.8/xrmap.egg-info/
+-rw-r--r--   0 javier     (501) staff       (20)      939 2023-05-26 12:03:03.000000 xrmap-0.0.8/xrmap.egg-info/PKG-INFO
+-rw-r--r--   0 javier     (501) staff       (20)      266 2023-05-26 12:03:03.000000 xrmap-0.0.8/xrmap.egg-info/SOURCES.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-05-26 12:03:03.000000 xrmap-0.0.8/xrmap.egg-info/dependency_links.txt
+-rw-r--r--   0 javier     (501) staff       (20)        1 2023-04-28 08:20:56.000000 xrmap-0.0.8/xrmap.egg-info/not-zip-safe
+-rw-r--r--   0 javier     (501) staff       (20)       31 2023-05-26 12:03:03.000000 xrmap-0.0.8/xrmap.egg-info/requires.txt
+-rw-r--r--   0 javier     (501) staff       (20)       11 2023-05-26 12:03:03.000000 xrmap-0.0.8/xrmap.egg-info/top_level.txt
```

### Comparing `xrmap-0.0.7/PKG-INFO` & `xrmap-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrmap
-Version: 0.0.7
+Version: 0.0.8
 Summary: Plot xarrays lat-lon datasets using folium
 Home-page: https://github.com/javiergvaldecasas/xarray-map
 Author: Javier García-Valdecasas
 Author-email: garciavaldecasas@oritiayboreas.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `xrmap-0.0.7/setup.cfg` & `xrmap-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = xrmap
-version = 0.0.7
+version = 0.0.8
 author = Javier García-Valdecasas
 author_email = garciavaldecasas@oritiayboreas.com
 license = Apache-2.0
 description = Plot xarrays lat-lon datasets using folium
 long_description_content_type = text/x-rst
 long_description = Plot xarrays lat-lon datasets using folium
 url = https://github.com/javiergvaldecasas/xarray-map
```

### Comparing `xrmap-0.0.7/xarray_map/plot_folium.py` & `xrmap-0.0.8/xarray_map/plot_folium.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,16 +31,14 @@
         longitude = self.longitude
     elif 'lat' in self.dims:
         latitude = self.lat
         longitude = self.lon
     else:
         raise ValueError('dimensions: latitude or lat ')
 
-    values[values<=vmin] = np.nan
-
     img = folium.raster_layers.ImageOverlay(
             name="",
             image= values,
             bounds=[[float(latitude.min().values), float(longitude.min().values)],
                     [float(latitude.max().values), float(longitude.max().values)]],
             opacity=opacity,
             interactive=True,
```

### Comparing `xrmap-0.0.7/xrmap.egg-info/PKG-INFO` & `xrmap-0.0.8/xrmap.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xrmap
-Version: 0.0.7
+Version: 0.0.8
 Summary: Plot xarrays lat-lon datasets using folium
 Home-page: https://github.com/javiergvaldecasas/xarray-map
 Author: Javier García-Valdecasas
 Author-email: garciavaldecasas@oritiayboreas.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

