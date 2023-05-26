# Comparing `tmp/rio-stac-0.7.1.tar.gz` & `tmp/rio_stac-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rio-stac-0.7.1.tar", last modified: Wed May  3 19:06:41 2023, max compression
+gzip compressed data, was "rio_stac-0.8.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `rio-stac-0.7.1.tar` & `rio_stac-0.8.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      212 2023-05-03 19:06:28.322383 rio-stac-0.7.1/.bumpversion.cfg
--rw-r--r--   0        0        0     1172 2023-05-03 19:06:28.322383 rio-stac-0.7.1/.gitignore
--rw-r--r--   0        0        0      822 2023-05-03 19:06:28.322383 rio-stac-0.7.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-05-03 19:06:28.322383 rio-stac-0.7.1/LICENSE
--rw-r--r--   0        0        0     5232 2023-05-03 19:06:28.322383 rio-stac-0.7.1/README.md
--rw-r--r--   0        0        0     2127 2023-05-03 19:06:28.322383 rio-stac-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      127 2023-05-03 19:06:28.326383 rio-stac-0.7.1/rio_stac/__init__.py
--rw-r--r--   0        0        0       28 2023-05-03 19:06:28.326383 rio-stac-0.7.1/rio_stac/scripts/__init__.py
--rw-r--r--   0        0        0     4801 2023-05-03 19:06:28.326383 rio-stac-0.7.1/rio_stac/scripts/cli.py
--rw-r--r--   0        0        0    13889 2023-05-03 19:06:28.326383 rio-stac-0.7.1/rio_stac/stac.py
--rw-r--r--   0        0        0     6503 1970-01-01 00:00:00.000000 rio-stac-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0      212 2023-05-26 09:26:22.462557 rio_stac-0.8.0/.bumpversion.cfg
+-rw-r--r--   0        0        0     1172 2023-05-26 09:26:22.462557 rio_stac-0.8.0/.gitignore
+-rw-r--r--   0        0        0      822 2023-05-26 09:26:22.462557 rio_stac-0.8.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-05-26 09:26:22.462557 rio_stac-0.8.0/LICENSE
+-rw-r--r--   0        0        0     5232 2023-05-26 09:26:22.462557 rio_stac-0.8.0/README.md
+-rw-r--r--   0        0        0     2149 2023-05-26 09:26:22.470557 rio_stac-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      127 2023-05-26 09:26:22.470557 rio_stac-0.8.0/rio_stac/__init__.py
+-rw-r--r--   0        0        0       28 2023-05-26 09:26:22.470557 rio_stac-0.8.0/rio_stac/scripts/__init__.py
+-rw-r--r--   0        0        0     4801 2023-05-26 09:26:22.470557 rio_stac-0.8.0/rio_stac/scripts/cli.py
+-rw-r--r--   0        0        0    13889 2023-05-26 09:26:22.470557 rio_stac-0.8.0/rio_stac/stac.py
+-rw-r--r--   0        0        0     6550 1970-01-01 00:00:00.000000 rio_stac-0.8.0/PKG-INFO
```

### Comparing `rio-stac-0.7.1/.gitignore` & `rio_stac-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.1/.pre-commit-config.yaml` & `rio_stac-0.8.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.1/LICENSE` & `rio_stac-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.1/README.md` & `rio_stac-0.8.0/README.md`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.1/pyproject.toml` & `rio_stac-0.8.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 ]
 dev = [
     "pre-commit",
 ]
 doc = [
     "mkdocs",
     "mkdocs-material",
+    "mkdocs-jupyter",
     "pygments",
     "pdocs",
 ]
 
 [project.urls]
 Source = "https://github.com/developmentseed/rio-stac"
 Documentation = "https://developmentseed.org/rio-stac/"
```

### Comparing `rio-stac-0.7.1/rio_stac/scripts/cli.py` & `rio_stac-0.8.0/rio_stac/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `rio-stac-0.7.1/rio_stac/stac.py` & `rio_stac-0.8.0/rio_stac/stac.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 import rasterio
 from pystac.utils import str_to_datetime
 from rasterio import transform, warp
 from rasterio.features import bounds as feature_bounds
 from rasterio.io import DatasetReader, DatasetWriter, MemoryFile
 from rasterio.vrt import WarpedVRT
 
-PROJECTION_EXT_VERSION = "v1.0.0"
+PROJECTION_EXT_VERSION = "v1.1.0"
 RASTER_EXT_VERSION = "v1.1.0"
-EO_EXT_VERSION = "v1.0.0"
+EO_EXT_VERSION = "v1.1.0"
 
 EPSG_4326 = rasterio.crs.CRS.from_epsg(4326)
 
 
 def bbox_to_geom(bbox: Tuple[float, float, float, float]) -> Dict:
     """Return a geojson geometry from a bbox."""
     return {
```

### Comparing `rio-stac-0.7.1/PKG-INFO` & `rio_stac-0.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rio-stac
-Version: 0.7.1
+Version: 0.8.0
 Summary: Create STAC Items from raster datasets.
 Author-email: Vincent Sarago <vincent@developmentseed.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -14,14 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: rasterio
 Requires-Dist: pystac>=1.0.0,<2.0.0
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs ; extra == "doc"
 Requires-Dist: mkdocs-material ; extra == "doc"
+Requires-Dist: mkdocs-jupyter ; extra == "doc"
 Requires-Dist: pygments ; extra == "doc"
 Requires-Dist: pdocs ; extra == "doc"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: requests ; extra == "test"
 Requires-Dist: jsonschema>=3.0 ; extra == "test"
 Project-URL: Documentation, https://developmentseed.org/rio-stac/
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: rio-stac Version: 0.7.1 Summary: Create STAC Items
+Metadata-Version: 2.1 Name: rio-stac Version: 0.8.0 Summary: Create STAC Items
 from raster datasets. Author-email: Vincent Sarago
 developmentseed.com> Requires-Python: >=3.8 Description-Content-Type: text/
 markdown Classifier: Intended Audience :: Information Technology Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Topic :: Scientific/Engineering :: GIS Requires-Dist: rasterio Requires-Dist:
 pystac>=1.0.0,<2.0.0 Requires-Dist: pre-commit ; extra == "dev" Requires-Dist:
 mkdocs ; extra == "doc" Requires-Dist: mkdocs-material ; extra == "doc"
-Requires-Dist: pygments ; extra == "doc" Requires-Dist: pdocs ; extra == "doc"
-Requires-Dist: pytest ; extra == "test" Requires-Dist: pytest-cov ; extra ==
-"test" Requires-Dist: requests ; extra == "test" Requires-Dist: jsonschema>=3.0
-; extra == "test" Project-URL: Documentation, https://developmentseed.org/rio-
-stac/ Project-URL: Source, https://github.com/developmentseed/rio-stac
-Provides-Extra: dev Provides-Extra: doc Provides-Extra: test # rio-stac
+Requires-Dist: mkdocs-jupyter ; extra == "doc" Requires-Dist: pygments ; extra
+== "doc" Requires-Dist: pdocs ; extra == "doc" Requires-Dist: pytest ; extra ==
+"test" Requires-Dist: pytest-cov ; extra == "test" Requires-Dist: requests ;
+extra == "test" Requires-Dist: jsonschema>=3.0 ; extra == "test" Project-URL:
+Documentation, https://developmentseed.org/rio-stac/ Project-URL: Source,
+https://github.com/developmentseed/rio-stac Provides-Extra: dev Provides-Extra:
+doc Provides-Extra: test # rio-stac
                                   [rio-stac]
                     Create STAC Items from raster datasets.
           [Test] [Coverage] [Package_version] [Downloads] [Downloads]
 --- **Documentation**: https://developmentseed.github.io/rio-stac/ **Source
 Code**: https://github.com/developmentseed/rio-stac --- `rio-stac` is a simple
 [rasterio](https://github.com/mapbox/rasterio) plugin for creating valid STAC
 items from a raster dataset. The library is built on top of [pystac](https://
```

