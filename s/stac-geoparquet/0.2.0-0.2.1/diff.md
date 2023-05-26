# Comparing `tmp/stac_geoparquet-0.2.0.tar.gz` & `tmp/stac_geoparquet-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_geoparquet-0.2.0.tar", last modified: Mon Apr 24 17:00:06 2023, max compression
+gzip compressed data, was "stac_geoparquet-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `stac_geoparquet-0.2.0.tar` & `stac_geoparquet-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1081 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/LICENSE
--rw-r--r--   0        0        0     1810 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/README.md
--rw-r--r--   0        0        0     1275 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      199 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/__init__.py
--rw-r--r--   0        0        0      143 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/_compat.py
--rw-r--r--   0        0        0     3823 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/cli.py
--rw-r--r--   0        0        0     4455 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/pc_runner.py
--rw-r--r--   0        0        0    12037 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/pgstac_reader.py
--rw-r--r--   0        0        0     3799 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/stac_geoparquet.py
--rw-r--r--   0        0        0     2480 2023-04-24 16:59:42.002009 stac_geoparquet-0.2.0/stac_geoparquet/utils.py
--rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 stac_geoparquet-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1810 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/README.md
+-rw-r--r--   0        0        0     1275 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/__init__.py
+-rw-r--r--   0        0        0      143 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/_compat.py
+-rw-r--r--   0        0        0     3823 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/cli.py
+-rw-r--r--   0        0        0     4455 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/pc_runner.py
+-rw-r--r--   0        0        0    12037 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/pgstac_reader.py
+-rw-r--r--   0        0        0     3817 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/stac_geoparquet.py
+-rw-r--r--   0        0        0     2480 2023-05-26 14:30:16.179537 stac_geoparquet-0.2.1/stac_geoparquet/utils.py
+-rw-r--r--   0        0        0     2911 1970-01-01 00:00:00.000000 stac_geoparquet-0.2.1/PKG-INFO
```

### Comparing `stac_geoparquet-0.2.0/LICENSE` & `stac_geoparquet-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.0/README.md` & `stac_geoparquet-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.0/pyproject.toml` & `stac_geoparquet-0.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.0/stac_geoparquet/cli.py` & `stac_geoparquet-0.2.1/stac_geoparquet/cli.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.0/stac_geoparquet/pc_runner.py` & `stac_geoparquet-0.2.1/stac_geoparquet/pc_runner.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.0/stac_geoparquet/pgstac_reader.py` & `stac_geoparquet-0.2.1/stac_geoparquet/pgstac_reader.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.0/stac_geoparquet/stac_geoparquet.py` & `stac_geoparquet-0.2.1/stac_geoparquet/stac_geoparquet.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
             item_geometry = fix_empty_multipolygon(item_geometry)  # type: ignore
         geometry.append(item_geometry)
 
     gdf = geopandas.GeoDataFrame(items2, geometry=geometry, crs="WGS84")
 
     for column in ["datetime", "start_datetime", "end_datetime"]:
         if column in gdf.columns:
-            gdf[column] = pd.to_datetime(gdf[column])
+            gdf[column] = pd.to_datetime(gdf[column], format="ISO8601")
 
     columns = [
         "type",
         "stac_version",
         "stac_extensions",
         "id",
         "geometry",
```

### Comparing `stac_geoparquet-0.2.0/stac_geoparquet/utils.py` & `stac_geoparquet-0.2.1/stac_geoparquet/utils.py`

 * *Files identical despite different names*

### Comparing `stac_geoparquet-0.2.0/PKG-INFO` & `stac_geoparquet-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac_geoparquet
-Version: 0.2.0
+Version: 0.2.1
 Summary: stac-geoparquet
 Author-email: Tom Augspurger <taugspurger@microsoft.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: pystac
 Requires-Dist: geopandas
```

