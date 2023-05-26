# Comparing `tmp/cnwigee-1.0.0.tar.gz` & `tmp/cnwigee-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cnwigee-1.0.0.tar", last modified: Thu May 25 18:45:34 2023, max compression
+gzip compressed data, was "cnwigee-1.0.1.tar", last modified: Fri May 26 12:54:58 2023, max compression
```

## Comparing `cnwigee-1.0.0.tar` & `cnwigee-1.0.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 18:45:34.507997 cnwigee-1.0.0/
--rw-rw-rw-   0        0        0     1091 2023-05-04 17:08:09.000000 cnwigee-1.0.0/LICENSE
--rw-rw-rw-   0        0        0     2518 2023-05-25 18:45:34.507997 cnwigee-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     2191 2023-05-04 17:08:09.000000 cnwigee-1.0.0/README.md
--rw-rw-rw-   0        0        0       82 2023-05-16 18:35:50.000000 cnwigee-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0      492 2023-05-25 18:45:34.507997 cnwigee-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0       71 2023-05-16 18:35:50.000000 cnwigee-1.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 18:45:34.476141 cnwigee-1.0.0/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 18:45:34.493903 cnwigee-1.0.0/src/cnwi/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/__init__.py
--rw-rw-rw-   0        0        0     5574 2023-05-24 16:06:22.000000 cnwigee-1.0.0/src/cnwi/acas.py
--rw-rw-rw-   0        0        0     1837 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/cmap.py
-drwxrwxrwx   0        0        0        0 2023-05-25 18:45:34.493903 cnwigee-1.0.0/src/cnwi/data/
--rw-rw-rw-   0        0        0        0 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/data/__init__.py
--rw-rw-rw-   0        0        0     4422 2023-05-24 12:55:30.000000 cnwigee-1.0.0/src/cnwi/datacube.py
--rw-rw-rw-   0        0        0     3464 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/datasets.py
--rw-rw-rw-   0        0        0     7105 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/derivatives.py
--rw-rw-rw-   0        0        0     1842 2023-05-24 12:55:30.000000 cnwigee-1.0.0/src/cnwi/elev.py
--rw-rw-rw-   0        0        0     6910 2023-05-24 12:55:30.000000 cnwigee-1.0.0/src/cnwi/fourier.py
--rw-rw-rw-   0        0        0     3052 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/moa.py
--rw-rw-rw-   0        0        0     4694 2023-05-24 12:55:30.000000 cnwigee-1.0.0/src/cnwi/opt.py
--rw-rw-rw-   0        0        0     2904 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/prebuilt.py
--rw-rw-rw-   0        0        0     1490 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/rf.py
--rw-rw-rw-   0        0        0     1891 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/sar.py
--rw-rw-rw-   0        0        0     3810 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/sfilters.py
--rw-rw-rw-   0        0        0      429 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/stack.py
-drwxrwxrwx   0        0        0        0 2023-05-25 18:45:34.493903 cnwigee-1.0.0/src/cnwi/tools/
--rw-rw-rw-   0        0        0        0 2023-05-24 16:06:22.000000 cnwigee-1.0.0/src/cnwi/tools/__init__.py
--rw-rw-rw-   0        0        0     1983 2023-05-24 16:06:22.000000 cnwigee-1.0.0/src/cnwi/tools/prep_training_data.py
-drwxrwxrwx   0        0        0        0 2023-05-25 18:45:34.507997 cnwigee-1.0.0/src/cnwi/tools/to_cloud/
--rw-rw-rw-   0        0        0        0 2023-05-25 17:17:40.000000 cnwigee-1.0.0/src/cnwi/tools/to_cloud/__init__.py
--rw-rw-rw-   0        0        0     5099 2023-05-25 17:17:40.000000 cnwigee-1.0.0/src/cnwi/tools/to_cloud/variables.py
--rw-rw-rw-   0        0        0     3397 2023-05-23 19:47:33.000000 cnwigee-1.0.0/src/cnwi/trainingd.py
-drwxrwxrwx   0        0        0        0 2023-05-25 18:45:34.507997 cnwigee-1.0.0/src/cnwigee.egg-info/
--rw-rw-rw-   0        0        0     2518 2023-05-25 18:45:34.000000 cnwigee-1.0.0/src/cnwigee.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      686 2023-05-25 18:45:34.000000 cnwigee-1.0.0/src/cnwigee.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 18:45:34.000000 cnwigee-1.0.0/src/cnwigee.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-05-25 18:45:34.000000 cnwigee-1.0.0/src/cnwigee.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 18:45:34.507997 cnwigee-1.0.0/tests/
--rw-rw-rw-   0        0        0     2018 2023-05-16 18:35:50.000000 cnwigee-1.0.0/tests/test_eecnwi_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.843606 cnwigee-1.0.1/
+-rw-rw-rw-   0        0        0     1091 2023-05-04 17:08:09.000000 cnwigee-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0     2518 2023-05-26 12:54:58.843606 cnwigee-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2191 2023-05-04 17:08:09.000000 cnwigee-1.0.1/README.md
+-rw-rw-rw-   0        0        0       82 2023-05-16 18:35:50.000000 cnwigee-1.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0      492 2023-05-26 12:54:58.859584 cnwigee-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0       71 2023-05-16 18:35:50.000000 cnwigee-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.595882 cnwigee-1.0.1/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.783744 cnwigee-1.0.1/src/cnwi/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/__init__.py
+-rw-rw-rw-   0        0        0     5574 2023-05-24 16:06:22.000000 cnwigee-1.0.1/src/cnwi/acas.py
+-rw-rw-rw-   0        0        0     1837 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/cmap.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.786759 cnwigee-1.0.1/src/cnwi/data/
+-rw-rw-rw-   0        0        0        0 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/data/__init__.py
+-rw-rw-rw-   0        0        0     4422 2023-05-24 12:55:30.000000 cnwigee-1.0.1/src/cnwi/datacube.py
+-rw-rw-rw-   0        0        0     3464 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/datasets.py
+-rw-rw-rw-   0        0        0     7105 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/derivatives.py
+-rw-rw-rw-   0        0        0     1843 2023-05-26 12:34:54.000000 cnwigee-1.0.1/src/cnwi/elev.py
+-rw-rw-rw-   0        0        0     6246 2023-05-26 11:57:44.000000 cnwigee-1.0.1/src/cnwi/fourier.py
+-rw-rw-rw-   0        0        0     3052 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/moa.py
+-rw-rw-rw-   0        0        0     4694 2023-05-24 12:55:30.000000 cnwigee-1.0.1/src/cnwi/opt.py
+-rw-rw-rw-   0        0        0     2904 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/prebuilt.py
+-rw-rw-rw-   0        0        0     1490 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/rf.py
+-rw-rw-rw-   0        0        0     1891 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/sar.py
+-rw-rw-rw-   0        0        0     3810 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/sfilters.py
+-rw-rw-rw-   0        0        0      429 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/stack.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.795915 cnwigee-1.0.1/src/cnwi/tools/
+-rw-rw-rw-   0        0        0        0 2023-05-24 16:06:22.000000 cnwigee-1.0.1/src/cnwi/tools/__init__.py
+-rw-rw-rw-   0        0        0     1983 2023-05-24 16:06:22.000000 cnwigee-1.0.1/src/cnwi/tools/prep_training_data.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.806931 cnwigee-1.0.1/src/cnwi/tools/to_cloud/
+-rw-rw-rw-   0        0        0        0 2023-05-25 17:17:40.000000 cnwigee-1.0.1/src/cnwi/tools/to_cloud/__init__.py
+-rw-rw-rw-   0        0        0     5104 2023-05-26 12:53:25.000000 cnwigee-1.0.1/src/cnwi/tools/to_cloud/variables.py
+-rw-rw-rw-   0        0        0     3397 2023-05-23 19:47:33.000000 cnwigee-1.0.1/src/cnwi/trainingd.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.843606 cnwigee-1.0.1/src/cnwigee.egg-info/
+-rw-rw-rw-   0        0        0     2518 2023-05-26 12:54:58.000000 cnwigee-1.0.1/src/cnwigee.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      686 2023-05-26 12:54:58.000000 cnwigee-1.0.1/src/cnwigee.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:54:58.000000 cnwigee-1.0.1/src/cnwigee.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-05-26 12:54:58.000000 cnwigee-1.0.1/src/cnwigee.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 12:54:58.843606 cnwigee-1.0.1/tests/
+-rw-rw-rw-   0        0        0     2018 2023-05-16 18:35:50.000000 cnwigee-1.0.1/tests/test_eecnwi_helpers.py
```

### Comparing `cnwigee-1.0.0/LICENSE` & `cnwigee-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/PKG-INFO` & `cnwigee-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnwigee
-Version: 1.0.0
+Version: 1.0.1
 Summary: Your description of the project
 Author: Ryan Hamilton
 Author-email: ryangilberthamilton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnwigee-1.0.0/README.md` & `cnwigee-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/acas.py` & `cnwigee-1.0.1/src/cnwi/acas.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/cmap.py` & `cnwigee-1.0.1/src/cnwi/cmap.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/datacube.py` & `cnwigee-1.0.1/src/cnwi/datacube.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/datasets.py` & `cnwigee-1.0.1/src/cnwi/datasets.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/derivatives.py` & `cnwigee-1.0.1/src/cnwi/derivatives.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/elev.py` & `cnwigee-1.0.1/src/cnwi/elev.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,14 +46,14 @@
         warnings.warn("Terrain Analysis as been Set to True... Please Note this is very memroy intenseve")
         # do terrain analysis raise warning to the end user
         gaus_filt = s.gaussian_filter(3)
         pm = s.perona_malik()
         
         rectnalge = build_rectangle(aoi)
 
-        dem_guas = dem_guas(dem)
+        dem_guas = gaus_filt(dem)
         ta_gauss = tagee.terrainAnalysis(dem_guas, rectnalge).select(GUASSIAN_BANDS)
         
         dem_pm = pm(dem)
         ta_pm = tagee.terrainAnalysis(dem_pm, rectnalge).select(PERONA_MALIK_BANDS)
         
         return ee.Image.cat(ta_gauss, ta_pm)
```

### Comparing `cnwigee-1.0.0/src/cnwi/fourier.py` & `cnwigee-1.0.1/src/cnwi/fourier.py`

 * *Files 9% similar despite different names*

```diff
@@ -127,52 +127,35 @@
 def fit(model: model) -> ee.ImageCollection:
     def fit_wrapper(image: ee.Image):
         return image.addBands(image.select(model.independent).multiply(model.coefficients)\
             .reduce('sum').rename('fitted'))
     return model.harmonics.map(fit_wrapper)
 
 #~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~#
-def fourier(target_aoi: ee.Geometry, modes: int = 3, cloud_pix_percent: int = 20,
-            variable: d._RasterCalculator = None, date_range: Tuple[str] = None) -> FourierImage:
+# TODO update function def to use raster calc object, 
+def fourier(ee_object: ee.ImageCollection, modes: int = 5, omega: float = 1.5, nir: str = None, 
+            red: str = None) -> FourierImage:
     """Applys fourier transform to defined image collection. Image Collection needs to be filtered 
     by start and end date, as well have a cloud mask applied. It also needs to have NDVI band in the 
     stack
 
     Args:
         ee_object (ee.ImageCollection): Optical Image Collection to have fourier transform fitted to
         modes (int, optional): number of modes to include. Defaults to 5.
         omega (float, optional): _description_. Defaults to 1.5.
     """
+    # construct the input collection
+    nir = "B8" if nir is None else nir
+    red = "B4" if red is None else red
     
-    def cloud_mask(element: ee.Image):
-        qa = element.select('QA60')
-        cloudBitMask = 1 << 10
-        cirrusBitMask = 1 << 11
-        mask = qa.bitwiseAnd(cloudBitMask).eq(0)\
-            .And(qa.bitwiseAnd(cirrusBitMask).eq(0))
-        return element.updateMask(mask)
-    
-    def min_max(*dates):
-        """ Calculates the time dif in days """
-        t1, t2 = dates
-        dif = ee.Date(t1).difference(ee.Date(t2), 'day').abs()
-        return dif.gt(365)   
-    
-    DATES = ('2017', '2022') if date_range is None else date_range
-    VARIABLE = d.NDVI() if variable is None else variable
-    OMEGA = 1 if min_max(*DATES) else 1.5
+    # TODO add date minMax checker, if greater than 365 days use omega of 1
     
-    t1, t2 = DATES
-    # construct the input collection
-    time_series = Sentinel2SR().filterBounds(target_aoi).filterDate(str(t1), str(t2))\
-        .filter(f'CLOUDY_PIXEL_PERCENTAGE > {cloud_pix_percent}')\
-        .map(cloud_mask)\
-        .map(VARIABLE)\
+    time_series = ee_object.map(add_ndvi(nir=nir, red=red))\
         .map(add_constant)\
-        .map(add_time(omega=OMEGA))
-    
+        .map(add_time(omega=omega))\
+
     fourier_model = model(
         ee_object=time_series,
         modes=modes,
-        dependent_var=VARIABLE.NAME
+        dependent_var="NDVI"
     )
     return FourierImage(model=fourier_model, ee_image_collection=time_series)
```

### Comparing `cnwigee-1.0.0/src/cnwi/moa.py` & `cnwigee-1.0.1/src/cnwi/moa.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/opt.py` & `cnwigee-1.0.1/src/cnwi/opt.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/prebuilt.py` & `cnwigee-1.0.1/src/cnwi/prebuilt.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/rf.py` & `cnwigee-1.0.1/src/cnwi/rf.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/sar.py` & `cnwigee-1.0.1/src/cnwi/sar.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/sfilters.py` & `cnwigee-1.0.1/src/cnwi/sfilters.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/tools/prep_training_data.py` & `cnwigee-1.0.1/src/cnwi/tools/prep_training_data.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwi/tools/to_cloud/variables.py` & `cnwigee-1.0.1/src/cnwi/tools/to_cloud/variables.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,25 +80,25 @@
             skipEmptyTiles=True,
             formatOptions={
                 'cloudOptimized': True
             }
         )
         task.start()
     print("Exports: Running on Cloud")
-    if not os.path.exits("./logging"):
-        os.path.makedirs("./logging")
+    if not os.path.exists("../logging"):
+        os.makedirs("../logging")
     # step into the task monitoring routine
     tasks = ee.batch.Task.list()[:len(grid_ids)]
     ids = [task.id for task in tasks]
     ids.reverse()
     gdf2['FOURIER_TASK_IDS'] = ids
-    gdf.to_file('./logging/fourier-grid.geojson', driver='GeoJSON')
+    gdf2.to_file('../logging/fourier-grid.geojson', driver='GeoJSON')
     while any([task.state in ['READY', 'RUNNING'] for task in tasks]):
         time.sleep(10)
-        tasks = [task for task in ee.batch.Task.list() if task.id in gdf2['FOURIER_IDS'].tolist()]
+        tasks = [task for task in ee.batch.Task.list() if task.id in gdf2['FOURIER_TASK_IDS'].tolist()]
 
     print("Export: Complete")
 
 
 def terrain_analysis_2_cloud(grid: gpd.GeoDataFrame, bucket: str, file_prefix: str, filename: str = None):
    
     gdf = grid
@@ -133,19 +133,19 @@
             }
         )
         task.start()
     
     # gets the inital state of the tasks
     print("Exports: Running on Cloud")
     # step into the task monitoring routine
-    if not os.path.exits("./logging"):
-        os.path.makedirs("./logging")
+    if not os.path.exists("../logging"):
+        os.makedirs("../logging")
     tasks = ee.batch.Task.list()[:len(grid_ids)]
     ids = [task.id for task in tasks]
     ids.reverse()
     gdf2['TERRAIN_TASK_IDS'] = ids
-    gdf.to_file('./logging/terrain-grid.geojson', driver='GeoJSON')
+    gdf2.to_file('../logging/terrain-grid.geojson', driver='GeoJSON')
     while any([task.state in ['READY', 'RUNNING'] for task in tasks]):
         time.sleep(10)
         tasks = [task for task in ee.batch.Task.list() if task.id in gdf2['TERRAIN_TASK_IDS']\
             .tolist()]
     print("Export: Complete")
```

### Comparing `cnwigee-1.0.0/src/cnwi/trainingd.py` & `cnwigee-1.0.1/src/cnwi/trainingd.py`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/src/cnwigee.egg-info/PKG-INFO` & `cnwigee-1.0.1/src/cnwigee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cnwigee
-Version: 1.0.0
+Version: 1.0.1
 Summary: Your description of the project
 Author: Ryan Hamilton
 Author-email: ryangilberthamilton@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `cnwigee-1.0.0/src/cnwigee.egg-info/SOURCES.txt` & `cnwigee-1.0.1/src/cnwigee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cnwigee-1.0.0/tests/test_eecnwi_helpers.py` & `cnwigee-1.0.1/tests/test_eecnwi_helpers.py`

 * *Files identical despite different names*

