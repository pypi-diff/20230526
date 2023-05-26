# Comparing `tmp/timor_locations-0.0.1.tar.gz` & `tmp/timor_locations-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "timor_locations-0.0.1.tar", max compression
+gzip compressed data, was "timor_locations-0.0.2.tar", max compression
```

## Comparing `timor_locations-0.0.1.tar` & `timor_locations-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
--rw-r--r--   0        0        0     1029 2023-05-24 16:20:08.175041 timor_locations-0.0.1/README.md
--rw-r--r--   0        0        0     1654 2023-05-24 16:17:07.227269 timor_locations-0.0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/__init__.py
--rw-r--r--   0        0        0      194 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/admin.py
--rw-r--r--   0        0        0      126 2023-05-24 16:14:01.023615 timor_locations-0.0.1/timor_locations/api.py
--rw-r--r--   0        0        0     1011 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/gis_functions.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/management/commands/__init__.py
--rw-r--r--   0        0        0     2292 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/management/commands/import_timor_geo_data.py
--rw-r--r--   0        0        0     3014 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/migrations/0001_initial.py
--rw-r--r--   0        0        0     1131 2023-05-24 16:14:01.023615 timor_locations-0.0.1/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py
--rw-r--r--   0        0        0     1401 2023-05-24 16:14:01.023615 timor_locations-0.0.1/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py
--rw-r--r--   0        0        0      887 2023-05-24 16:14:01.023615 timor_locations-0.0.1/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/migrations/__init__.py
--rw-r--r--   0        0        0     2572 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/models.py
--rw-r--r--   0        0        0     1345 2023-05-24 16:14:01.023615 timor_locations-0.0.1/timor_locations/router.py
--rw-r--r--   0        0        0      271 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/schemas.py
--rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/settings.py
--rw-r--r--   0        0        0      216 2023-05-24 16:14:01.023615 timor_locations-0.0.1/timor_locations/urls.py
--rw-r--r--   0        0        0      414 2023-05-24 16:14:01.019615 timor_locations-0.0.1/timor_locations/wsgi.py
--rw-r--r--   0        0        0     1779 1970-01-01 00:00:00.000000 timor_locations-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1029 2023-05-24 16:20:08.175041 timor_locations-0.0.2/README.md
+-rw-r--r--   0        0        0     1734 2023-05-26 10:04:34.088710 timor_locations-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/__init__.py
+-rw-r--r--   0        0        0      279 2023-05-26 06:37:53.703110 timor_locations-0.0.2/timor_locations/admin.py
+-rw-r--r--   0        0        0      125 2023-05-26 06:37:53.699110 timor_locations-0.0.2/timor_locations/api.py
+-rw-r--r--   0        0        0     1011 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/gis_functions.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/management/commands/__init__.py
+-rw-r--r--   0        0        0     1273 2023-05-26 09:50:10.256772 timor_locations-0.0.2/timor_locations/management/commands/create_topology.py
+-rw-r--r--   0        0        0     2726 2023-05-26 09:51:35.426460 timor_locations-0.0.2/timor_locations/management/commands/import_timor_geo_data.py
+-rw-r--r--   0        0        0     3014 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1131 2023-05-24 16:14:01.023615 timor_locations-0.0.2/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py
+-rw-r--r--   0        0        0     1401 2023-05-24 16:14:01.023615 timor_locations-0.0.2/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py
+-rw-r--r--   0        0        0      887 2023-05-24 16:14:01.023615 timor_locations-0.0.2/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py
+-rw-r--r--   0        0        0      783 2023-05-26 09:15:33.722459 timor_locations-0.0.2/timor_locations/migrations/0005_topojson.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/migrations/__init__.py
+-rw-r--r--   0        0        0     4719 2023-05-26 09:55:46.818367 timor_locations-0.0.2/timor_locations/models.py
+-rw-r--r--   0        0        0     1610 2023-05-26 09:50:10.276774 timor_locations-0.0.2/timor_locations/router.py
+-rw-r--r--   0        0        0      983 2023-05-26 09:50:10.248771 timor_locations-0.0.2/timor_locations/schemas.py
+-rw-r--r--   0        0        0        0 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/settings.py
+-rw-r--r--   0        0        0      213 2023-05-26 06:37:53.707110 timor_locations-0.0.2/timor_locations/urls.py
+-rw-r--r--   0        0        0      414 2023-05-24 16:14:01.019615 timor_locations-0.0.2/timor_locations/wsgi.py
+-rw-r--r--   0        0        0     1739 1970-01-01 00:00:00.000000 timor_locations-0.0.2/PKG-INFO
```

### Comparing `timor_locations-0.0.1/README.md` & `timor_locations-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.1/pyproject.toml` & `timor_locations-0.0.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 [tool.ruff]
 line-length = 119
 exclude = ['migrations']
 
 [tool.poetry]
 name = "timor-locations"
-version = "0.0.1"
+version = "0.0.2"
 description = "Timor-Leste geographic datasets"
 authors = [
   "Joshua Brooks <josh@catalpa.io>",
   "Anders Hofstee <anders@catalpa.io>",
 ]
 exclude = ["tests", "sl_tests", "timor_locations/data", "docs"]
 license = "GPLv3"
@@ -37,15 +37,14 @@
 repository = "https://github.com/catalpainternational/timor_locations"
 homepage = "https://github.com/catalpainternational/timor_locations"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 pydantic = ">1.10.6,<2"
 django-ninja = ">=0.21.0"
-django-geojson = ">=4.0.0"
 geojson-pydantic = "^0.6.2"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "*"
@@ -57,14 +56,20 @@
 psycopg2-binary = "*"
 pytest-django = "*"
 pytest-cov = "*"
 factory-boy = "*"
 ruff = "^0.0.269"
 django-extensions = "^3.2.1"
 
+[tool.poetry.group.topology]
+optional = true
+
+[tool.poetry.group.topology.dependencies]
+topojson = "^1.5"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 plugins = ["mypy_django_plugin.main"]
```

### Comparing `timor_locations-0.0.1/timor_locations/gis_functions.py` & `timor_locations-0.0.2/timor_locations/gis_functions.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.1/timor_locations/management/commands/import_timor_geo_data.py` & `timor_locations-0.0.2/timor_locations/management/commands/import_timor_geo_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,33 +1,47 @@
-from django.core.management.base import BaseCommand
-from pathlib import Path
+import csv
+import os
+from importlib import resources
+
 from django.contrib.gis.gdal import DataSource
 from django.contrib.gis.utils import LayerMapping
+from django.core.management.base import BaseCommand
 from django.db import connection
-from timor_locations.models import Suco, AdministrativePost, Municipality
-import csv
 
+from timor_locations.models import AdministrativePost, Municipality, Suco
 
 suco_mapping = {"geom": "MULTIPOLYGON", "name": "SUCONAME", "pcode": "SUCOCODE"}
 
+# Data for this is help in Git LFS
+
+
+SOURCE_GEO = resources.files("timor_locations.data").joinpath("sukus.gpkg")
+SOURCE_CSV = resources.files("timor_locations.data").joinpath("sukus.csv")
+
 
 class Command(BaseCommand):
     help = "Import Timor data from source shapefiles."
 
     def handle(self, *args, **options):
         self.stdout.write(self.style.SUCCESS("Priming the Districts table"))
-        ds = DataSource(Path() / "timor_locations" / "data" / "sucos.gpkg")
+
+        if not os.path.exists(SOURCE_GEO):
+            raise FileNotFoundError(f"The geographic data is not present: expected a file at {SOURCE_GEO}")
+        if not os.path.exists(SOURCE_CSV):
+            raise FileNotFoundError(f"The CSV file for data is not present: expected a file at {SOURCE_CSV}")
+
+        ds = DataSource(SOURCE_GEO)
 
         lm = LayerMapping(Suco, ds, suco_mapping)
         self.stdout.write(self.style.SUCCESS("Saving sucos from the gpkg file"))
         lm.save()
 
         self.stdout.write(self.style.SUCCESS("Adding admin posts and municipalities"))
 
-        with open(Path() / "timor_locations" / "data" / "suco.csv") as csvfile:
+        with open(SOURCE_CSV) as csvfile:
             csvreader = csv.reader(csvfile)
             posts: list[str, str] = list(csvreader)[1:]
             for SUCONAME, SUBDSTCODE, DISTCODE, DISTNAME, SUBDISTRCT, SUCOCODE, REGION in posts:
                 municipality, _ = Municipality.objects.update_or_create(pcode=DISTCODE, defaults=dict(name=DISTNAME))
                 adminpost, _ = AdministrativePost.objects.update_or_create(
                     pcode=SUBDSTCODE, defaults=dict(name=SUBDISTRCT, municipality=municipality)
                 )
@@ -37,13 +51,13 @@
 
         self.stdout.write(
             self.style.SUCCESS("Populate the admin post / municipality geometries based on the Suco geometries")
         )
         with connection.cursor() as c:
             c.execute(
                 """
-                UPDATE timor_locations_administrativepost ap 
+                UPDATE timor_locations_administrativepost ap
                     SET geom = (SELECT st_multi(st_union(geom)) FROM timor_locations_suco s WHERE s.adminpost_id = ap.pcode);
                 UPDATE timor_locations_municipality m
                     SET geom = (SELECT st_multi(st_union(geom)) FROM timor_locations_administrativepost ap WHERE ap.municipality_id = m.pcode);
                 """
             )
```

### Comparing `timor_locations-0.0.1/timor_locations/migrations/0001_initial.py` & `timor_locations-0.0.2/timor_locations/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.1/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py` & `timor_locations-0.0.2/timor_locations/migrations/0002_remove_administrativepost_id_remove_municipality_id_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.1/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py` & `timor_locations-0.0.2/timor_locations/migrations/0003_alter_administrativepost_municipality_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.1/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py` & `timor_locations-0.0.2/timor_locations/migrations/0004_alter_administrativepost_date_modified_and_more.py`

 * *Files identical despite different names*

### Comparing `timor_locations-0.0.1/timor_locations/router.py` & `timor_locations-0.0.2/timor_locations/router.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,12 +1,11 @@
-from ninja import Router
-
 from geojson_pydantic import FeatureCollection
+from ninja import Router
 
-from timor_locations import schemas, models
+from timor_locations import models, schemas
 
 router = Router(tags=["Timor GIS"])
 
 
 @router.get("/area/list.json", response=list[schemas.AreaOut])
 def area_list(request):
     """
@@ -37,7 +36,16 @@
 def admin_posts(request):
     return models.AdministrativePost.objects.as_feature_collection()
 
 
 @router.get("/municipalities.json", response=FeatureCollection)
 def municipalities(request):
     return models.Municipality.objects.as_feature_collection()
+
+
+# The following endpoints require appropriate data in the database
+# See the `create_topology` command
+
+
+@router.get("/{slug}.topojson", response=schemas.Topology)
+def original_topojson(request, slug: str):
+    return models.TopoJson.objects.get(pk=slug).topology
```

### Comparing `timor_locations-0.0.1/PKG-INFO` & `timor_locations-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 Metadata-Version: 2.1
 Name: timor-locations
-Version: 0.0.1
+Version: 0.0.2
 Summary: Timor-Leste geographic datasets
 Home-page: https://github.com/catalpainternational/timor_locations
 License: GPLv3
 Author: Joshua Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: django-geojson (>=4.0.0)
 Requires-Dist: django-ninja (>=0.21.0)
 Requires-Dist: geojson-pydantic (>=0.6.2,<0.7.0)
 Requires-Dist: pydantic (>1.10.6,<2)
 Project-URL: Repository, https://github.com/catalpainternational/timor_locations
 Description-Content-Type: text/markdown
 
 # Timor GIS
```

