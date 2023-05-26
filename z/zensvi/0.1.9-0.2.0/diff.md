# Comparing `tmp/zensvi-0.1.9.tar.gz` & `tmp/zensvi-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zensvi-0.1.9.tar", max compression
+gzip compressed data, was "zensvi-0.2.0.tar", max compression
```

## Comparing `zensvi-0.1.9.tar` & `zensvi-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.1.9/LICENSE
--rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.1.9/README.md
--rwxr-xr-x   0        0        0      694 2023-05-16 13:00:07.306317 zensvi-0.1.9/pyproject.toml
--rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.1.9/src/zensvi/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.1.9/src/zensvi/cv/__init__.py
--rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.1.9/src/zensvi/cv/segmentation/__init__.py
--rwxr-xr-x   0        0        0    39332 2023-05-16 12:59:53.127925 zensvi-0.1.9/src/zensvi/cv/segmentation/segmentation.py
--rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.1.9/src/zensvi/download/__init__.py
--rwxr-xr-x   0        0        0    21150 2023-05-16 12:53:24.204133 zensvi-0.1.9/src/zensvi/download/streetview_downloader.py
--rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.1.9/src/zensvi/download/utils/UserAgent.csv
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.1.9/src/zensvi/download/utils/__init__.py
--rwxr-xr-x   0        0        0     8291 2023-05-14 13:25:54.052907 zensvi-0.1.9/src/zensvi/download/utils/geoprocess.py
--rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.1.9/src/zensvi/download/utils/get_pids.py
--rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.1.9/src/zensvi/download/utils/helpers.py
--rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.1.9/src/zensvi/download/utils/imtool.py
--rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.1.9/src/zensvi/download/utils/proxies.csv
--rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.1.9/src/zensvi/transform/__init__.py
--rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.1.9/src/zensvi/transform/transform_image.py
--rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.1.9/src/zensvi/zensvi.py
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.1.9/PKG-INFO
+-rwxr-xr-x   0        0        0     1072 2023-05-10 07:40:35.070000 zensvi-0.2.0/LICENSE
+-rwxr-xr-x   0        0        0      669 2023-05-14 01:59:06.762105 zensvi-0.2.0/README.md
+-rwxr-xr-x   0        0        0      694 2023-05-26 08:59:44.901237 zensvi-0.2.0/pyproject.toml
+-rwxr-xr-x   0        0        0      131 2023-05-14 01:59:06.769291 zensvi-0.2.0/src/zensvi/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769717 zensvi-0.2.0/src/zensvi/cv/__init__.py
+-rwxr-xr-x   0        0        0       27 2023-05-14 01:59:06.769911 zensvi-0.2.0/src/zensvi/cv/segmentation/__init__.py
+-rwxr-xr-x   0        0        0    39841 2023-05-25 00:58:05.893778 zensvi-0.2.0/src/zensvi/cv/segmentation/segmentation.py
+-rwxr-xr-x   0        0        0       55 2023-05-14 01:59:06.771355 zensvi-0.2.0/src/zensvi/download/__init__.py
+-rwxr-xr-x   0        0        0    22836 2023-05-26 08:59:23.004525 zensvi-0.2.0/src/zensvi/download/streetview_downloader.py
+-rwxr-xr-x   0        0        0   316244 2023-05-14 01:59:06.772840 zensvi-0.2.0/src/zensvi/download/utils/UserAgent.csv
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.772946 zensvi-0.2.0/src/zensvi/download/utils/__init__.py
+-rwxr-xr-x   0        0        0     8291 2023-05-26 08:32:40.233104 zensvi-0.2.0/src/zensvi/download/utils/geoprocess.py
+-rwxr-xr-x   0        0        0     2000 2023-05-14 12:56:31.947491 zensvi-0.2.0/src/zensvi/download/utils/get_pids.py
+-rwxr-xr-x   0        0        0      956 2023-05-14 09:11:59.596085 zensvi-0.2.0/src/zensvi/download/utils/helpers.py
+-rwxr-xr-x   0        0        0     8165 2023-05-15 13:48:37.487829 zensvi-0.2.0/src/zensvi/download/utils/imtool.py
+-rw-r--r--   0        0        0    82321 2023-05-11 09:02:38.204470 zensvi-0.2.0/src/zensvi/download/utils/proxies.csv
+-rwxr-xr-x   0        0        0       30 2023-05-14 01:59:06.778122 zensvi-0.2.0/src/zensvi/transform/__init__.py
+-rwxr-xr-x   0        0        0     6500 2023-05-14 01:59:06.778828 zensvi-0.2.0/src/zensvi/transform/transform_image.py
+-rwxr-xr-x   0        0        0        0 2023-05-14 01:59:06.778944 zensvi-0.2.0/src/zensvi/zensvi.py
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 zensvi-0.2.0/PKG-INFO
```

### Comparing `zensvi-0.1.9/LICENSE` & `zensvi-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.9/README.md` & `zensvi-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.9/pyproject.toml` & `zensvi-0.2.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zensvi"
-version = "0.1.9"
+version = "0.2.0"
 description = "This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner."
 authors = ["koito19960406"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `zensvi-0.1.9/src/zensvi/cv/segmentation/segmentation.py` & `zensvi-0.2.0/src/zensvi/cv/segmentation/segmentation.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,15 +519,22 @@
             for image_file, img, output, pixel_ratio in zip(image_files, images, outputs, pixel_ratios):
                 if (len(self.save_image_options) > 0) & (dir_output is not None):
                     self._save_segmentation_image(task, image_file, img, dir_output, output)
                 image_file_key = Path(image_file).stem
                 pixel_ratio_dict[image_file_key] = pixel_ratio
 
     # Modify the segment method inside the Segmenter class
-    def segment(self, dir_input: Union[str, Path], dir_image_output: Union[str, Path, None] = None, dir_pixel_ratio_output: Union[str, Path, None] = None, task="semantic", batch_size=1, save_image_options = ["segmented_image", "blend_image"], pixel_ratio_save_format = ["json", "csv"]):
+    def segment(self, dir_input: Union[str, Path], 
+                dir_image_output: Union[str, Path, None] = None, 
+                dir_pixel_ratio_output: Union[str, Path, None] = None, 
+                task="semantic", 
+                batch_size=1, 
+                save_image_options = ["segmented_image", "blend_image"], 
+                pixel_ratio_save_format = ["json", "csv"],
+                max_workers: Union[int, None] = None):
         # make sure that at least one of dir_image_output and dir_pixel_ratio_output is not None
         if (dir_image_output is None) & (dir_pixel_ratio_output is None):
             raise ValueError("At least one of dir_image_output and dir_pixel_ratio_output must not be None.")
         
         # save_image_options as a property of the class
         self.save_image_options = save_image_options
         
@@ -552,29 +559,33 @@
             if checkpoint_start_index > 0:
                 for checkpoint in checkpoints:
                     with open(checkpoint, 'r') as f:
                         checkpoint_dict = json.load(f)
                         completed_image_files.update(checkpoint_dict.keys())
 
         # Get the list of all image files and filter the ones that are not completed yet
-        image_files = [str(f) for f in Path(dir_input).glob("*.jpg") if str(f) not in completed_image_files]
+        # List of possible image file extensions
+        image_extensions = [".jpg", ".jpeg", ".png", ".tif", ".tiff", ".bmp", ".dib", ".pbm", ".pgm", ".ppm", ".sr", ".ras", ".exr", ".jp2"]
+
+        # Get the list of all image files in the directory that are not completed yet
+        image_file_list = [str(f) for f in Path(dir_input).iterdir() if f.suffix in image_extensions and str(f) not in completed_image_files]
 
         outer_batch_size = 1000  # Number of inner batches in one outer batch
-        num_outer_batches = (len(image_files) + outer_batch_size * batch_size - 1) // (outer_batch_size * batch_size)
+        num_outer_batches = (len(image_file_list) + outer_batch_size * batch_size - 1) // (outer_batch_size * batch_size)
 
-        for i in tqdm(range(num_outer_batches), desc=f"Processing outer batches of size {min(outer_batch_size * batch_size, len(image_files))}"):
+        for i in tqdm(range(num_outer_batches), desc=f"Processing outer batches of size {min(outer_batch_size * batch_size, len(image_file_list))}"):
             # Get the image files for the current outer batch
-            outer_batch_image_files = image_files[i * outer_batch_size * batch_size : (i+1) * outer_batch_size * batch_size]
+            outer_batch_image_file_list = image_file_list[i * outer_batch_size * batch_size : (i+1) * outer_batch_size * batch_size]
 
-            dataset = ImageDataset(outer_batch_image_files)
+            dataset = ImageDataset(outer_batch_image_file_list)
             dataloader = DataLoader(dataset, batch_size=batch_size, collate_fn=dataset.collate_fn)
 
             pixel_ratio_dict = defaultdict(dict)  # reset pixel_ratio_dict for each outer batch
 
-            with ThreadPoolExecutor() as executor:
+            with ThreadPoolExecutor(max_workers=max_workers) as executor:
                 futures = []
 
                 for batch in dataloader:
                     image_files, images, original_img_shape = batch
                     future = executor.submit(self._process_images, task, image_files, images, dir_image_output, pixel_ratio_dict, original_img_shape)
                     futures.append(future)
```

### Comparing `zensvi-0.1.9/src/zensvi/download/streetview_downloader.py` & `zensvi-0.2.0/src/zensvi/download/streetview_downloader.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import warnings
 from shapely.errors import ShapelyDeprecationWarning
 warnings.filterwarnings("ignore", category=ShapelyDeprecationWarning)
 import csv
 import glob
 import shutil
 import numpy as np
+import osmnx as ox
 
 from zensvi.download.utils.imtool import ImageTool
 from zensvi.download.utils.get_pids import panoids
 from zensvi.download.utils.geoprocess import GeoProcessor
 from zensvi.download.utils.helpers import standardize_column_names, create_buffer_gdf
 
 class StreetViewDownloader:
@@ -34,107 +35,119 @@
         self._nthreads = nthreads
         self._distance = distance
         self._user_agent = self._get_ua()
         self._proxies = self._get_proxies()
         self._grid = grid
         self._grid_size = grid_size
 
+
     @property
     def gsv_api_key(self):
         return self._gsv_api_key    
     @gsv_api_key.setter
     def gsv_api_key(self,gsv_api_key):
         self._gsv_api_key = gsv_api_key
 
+
     @property
     def log_path(self):
         return self._log_path    
     @log_path.setter
     def log_path(self,log_path):
         self._log_path = log_path
         
+        
     @property
     def nthreads(self):
         return self._nthreads    
     @nthreads.setter
     def nthreads(self,nthreads):
         self._nthreads = nthreads
     
     @property
     def distance(self):
         return self._distance    
     @distance.setter
     def distance(self,distance):
         self._distance = distance
     
+    
     @property
     def grid(self):
         return self._grid    
     @grid.setter
     def grid(self,grid):
         self._grid = grid
         
+        
     @property
     def grid_size(self):
         return self._grid_size    
     @grid_size.setter
     def grid_size(self,grid_size):
         self._grid_size = grid_size
     
+    
     @property
     def user_agent(self):
         return self._user_agent  
     
+    
     def _get_ua(self):
         user_agent_file = pkg_resources.resource_filename('zensvi.download.utils', 'UserAgent.csv')
         UA = []
         with open(user_agent_file, 'r') as f:
             for line in f:
                 ua = {"user_agent": line.strip()}
                 UA.append(ua)
         return UA
     
+    
     @property
     def proxies(self):
         return self._proxies
     
+    
     def _get_proxies(self):
         proxies_file = pkg_resources.resource_filename('zensvi.download.utils', 'proxies.csv')
         proxies = []
-        with open(proxies_file, 'r') as f:
+        # open with "utf-8" encoding to avoid UnicodeDecodeError
+        with open(proxies_file, 'r', encoding = "utf-8") as f:
             reader = csv.DictReader(f)
             for row in reader:
                 ip = row['ip']
                 port = row['port']
                 protocols = row['protocols']
                 proxy_dict = {protocols: f"{ip}:{port}"}
                 proxies.append(proxy_dict)
         return proxies
     
+    
     def _read_pids(self, path_pid):
         pid_df = pd.read_csv(path_pid)
         # get unique pids as a list
         pids = pid_df.iloc[:,0].unique().tolist()
         return pids
 
+
     def _check_already(self, all_panoids):
-        # Get the list of already downloaded images
-        name_r = set(name.split(".")[0] for name in os.listdir(self.panorama_output))
+        # Get the set of already downloaded images
+        name_r = set(name.split(".")[0] for name in tqdm(os.listdir(self.panorama_output), desc="Checking already downloaded images"))
 
         # Filter the list of all panoids to only include those not already downloaded
-        all_panoids[:] = [pid for pid in all_panoids if pid not in name_r]
-
+        all_panoids = list(set(all_panoids) - name_r)
         return all_panoids
 
 
     def _log_write(self, pids):
         with open(self.log_path, 'a+') as fw:
             for pid in pids:
                 fw.write(pid+'\n')
     
+    
     def _augment_metadata(self, df):
         if self.cache_pids_augmented.exists():
             df = pd.read_csv(self.cache_pids_augmented)
             print("The augmented panorama IDs have been read from the cache")
             return df
         
         # Create a new directory called "augmented_metadata_checkpoints"
@@ -206,14 +219,15 @@
         # delete cache_pids_raw
         self.cache_pids_raw.unlink()
         # delete the cache directory
         if dir_cache_augmented_metadata.exists():
             shutil.rmtree(dir_cache_augmented_metadata)
         return df
 
+
     def _get_pids_from_csv(self, df, id_columns=None, closest=False, disp=False):
         # 1. Create a new directory called "pids" to store each batch pids
         dir_cache_pids = self.dir_cache / 'raw_pids'
         dir_cache_pids.mkdir(parents=True, exist_ok=True)
 
         # 2. Load all the checkpoint csv files
         checkpoints = glob.glob(str(dir_cache_pids / '*.csv'))
@@ -302,16 +316,17 @@
             # Save the results of retried rows as another checkpoint
             if len(results) > 0:
                 pd.DataFrame(results).to_csv(f'{dir_cache_pids}/checkpoint_retry.csv', index=False)
                 # Merge the retry checkpoint into the final dataframe
                 retry_df = pd.read_csv(f'{dir_cache_pids}/checkpoint_retry.csv')
                 results_df = pd.concat([results_df, retry_df], ignore_index=True)
 
-        # now save results_df as a new cache afte dropping lat_lon_id
+        # now save results_df as a new cache after dropping lat_lon_id and drop duplicates in panoid
         results_df = results_df.drop(columns='lat_lon_id')
+        results_df = results_df.drop_duplicates(subset='panoid')
         results_df.to_csv(self.cache_pids_raw, index=False)
 
         # delete the cache directory
         if dir_cache_pids.exists():
             shutil.rmtree(dir_cache_pids)
         return results_df
 
@@ -325,14 +340,15 @@
             gp = GeoProcessor(gdf, distance=self.distance, grid=self.grid, grid_size=self.grid_size, id_columns = id_columns)
             df = gp.get_lat_lon()
             df['lat_lon_id'] = np.arange(1, len(df) + 1)
             # save df to cache
             df.to_csv(self.cache_lat_lon, index=False)
 
         if self.cache_pids_raw.exists():
+            print("The raw panorama IDs have been read from the cache")
             results_df = pd.read_csv(self.cache_pids_raw)
         else:
             # Use _get_pids_from_csv to get pids from df
             results_df = self._get_pids_from_csv(df, id_columns, closest=closest, disp=disp)
 
         # Check if lat and lon are within input polygons
         polygons = gpd.GeoSeries([geom for geom in gdf['geometry'] if geom.type in ['Polygon', 'MultiPolygon']])
@@ -366,81 +382,118 @@
         # Return only those points within polygons
         results_within_polygons_df = results_df[results_df['within_polygon']]
         # Drop the 'within_polygon' column
         results_within_polygons_df = results_within_polygons_df.drop(columns='within_polygon')
         return results_within_polygons_df
 
 
-    def get_pids(self, path_pid, lat = None, lon = None, input_csv_file = "", input_shp_file = "", id_columns=None, buffer = 0, closest=False, disp=False, augment_metadata=False):
+    def _get_raw_pid(self, **kwargs):
+        defaults = {
+            'lat': None, 'lon': None, 'input_csv_file': "", 'input_shp_file': "",
+            'input_place_name': "", 'id_columns': None, 'buffer': 0, 
+            'closest': False, 'disp': False
+        }
+        
+        defaults.update(kwargs)
+
+        if self.cache_pids_raw.exists():
+            pid = pd.read_csv(self.cache_pids_raw)
+            print("The raw panorama IDs have been read from the cache")
+            return pid
+
+        if defaults['lat'] is not None and defaults['lon'] is not None:
+            pid = panoids(defaults['lat'], defaults['lon'], closest=defaults['closest'], disp=defaults['disp'])
+        elif defaults['input_csv_file'] != "":
+            df = pd.read_csv(defaults['input_csv_file'])
+            df = standardize_column_names(df)
+            if defaults['buffer'] > 0:
+                gdf = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.longitude, df.latitude), crs='EPSG:4326')
+                gdf = create_buffer_gdf(gdf, defaults['buffer'])
+                pid = self._get_pids_from_gdf(gdf, defaults['id_columns'], closest=False, disp=False)
+            else:
+                pid = self._get_pids_from_csv(df, defaults['id_columns'], closest=False, disp=False)
+        elif defaults['input_shp_file'] != "":
+            gdf = gpd.read_file(defaults['input_shp_file'])
+            if defaults['buffer'] > 0:
+                gdf = create_buffer_gdf(gdf, defaults['buffer'])
+            pid = self._get_pids_from_gdf(gdf, defaults['id_columns'], closest=False, disp=False)
+        elif defaults['input_place_name'] != "":
+            print("Geocoding the input place name")
+            gdf = ox.geocoder.geocode_to_gdf(defaults['input_place_name'])
+            if defaults['buffer'] > 0:
+                gdf = create_buffer_gdf(gdf, defaults['buffer'])
+            pid = self._get_pids_from_gdf(gdf, defaults['id_columns'], closest=False, disp=False) 
+        else:
+            raise ValueError("Please input the lat and lon, csv file, or shapefile.")
+
+        return pid
+
+
+    def get_pids(self, path_pid, **kwargs):
+        defaults = {
+            'lat': None, 'lon': None, 'input_csv_file': "", 'input_shp_file': "",
+            'input_place_name': "", 'id_columns': None, 'buffer': 0, 
+            'closest': False, 'disp': False, 'augment_metadata': False
+        }
+        
+        defaults.update(kwargs)
+        id_columns = defaults['id_columns']
         if id_columns is not None:
             if isinstance(id_columns, str):
                 id_columns = [id_columns.lower()]
             elif isinstance(id_columns, list):
                 id_columns = [column.lower() for column in id_columns]
         else:
             id_columns = []
-        if lat != None and lon != None:
-            pid = panoids(lat, lon, closest=closest, disp=disp)
-        elif input_csv_file != "":
-            df = pd.read_csv(input_csv_file)
-            df = standardize_column_names(df)
-            if buffer > 0:
-                gdf = gpd.GeoDataFrame(df, geometry=gpd.points_from_xy(df.longitude, df.latitude), crs='EPSG:4326')
-                gdf = create_buffer_gdf(gdf, buffer)
-                pid = self._get_pids_from_gdf(gdf, id_columns, closest=False, disp=False)
-            else:
-                if self.cache_pids_raw.exists():
-                    pid = pd.read_csv(self.cache_pids_raw)
-                    print("The raw panorama IDs have been read from the cache")
-                else:
-                    pid = self._get_pids_from_csv(df, id_columns, closest=False, disp=False)
-        elif input_shp_file != "":
-            gdf = gpd.read_file(input_shp_file)
-            if buffer > 0:
-                gdf = create_buffer_gdf(gdf, buffer)
-            pid = self._get_pids_from_gdf(gdf, id_columns, closest=False, disp=False)
-        else:
-            raise ValueError("Please input the lat and lon, csv file, or shapefile.")
-        # save the pids
+        # update id_columns
+        defaults['id_columns'] = id_columns
+        
+        # get raw pid
+        pid = self._get_raw_pid(**defaults)
+
+        # convert pid to dataframe
         pid_df = pd.DataFrame(pid)
-        pid_df = pid_df.drop_duplicates(subset='panoid')
-        if augment_metadata & (self.gsv_api_key != None):
+        
+        if defaults["augment_metadata"] & (self.gsv_api_key != None):
             pid_df = self._augment_metadata(pid_df)
-        elif augment_metadata & (self.gsv_api_key == None):
+        elif defaults["augment_metadata"] & (self.gsv_api_key == None):
             raise ValueError("Please set the gsv api key by calling the gsv_api_key method.")
         pid_df.to_csv(path_pid, index=False)
         print("The panorama IDs have been saved to {}".format(path_pid)) 
 
+
     def _set_dirs(self, dir_output):
         # set dir_output as attribute and create the directory
         self.dir_output = Path(dir_output)
         self.dir_output.mkdir(parents=True, exist_ok=True)
         # set dir_cache as attribute and create the directory
         self.dir_cache = self.dir_output / "cache_zensvi"
         self.dir_cache.mkdir(parents=True, exist_ok=True)
         # set other cache directories
         self.cache_lat_lon = self.dir_cache / "lat_lon.csv"
         self.cache_pids_raw = self.dir_cache / "pids_raw.csv"
         self.cache_pids_augmented = self.dir_cache / "pids_augemented.csv"
         
+        
     def download_gsv(self, dir_output, path_pid = None, zoom=2, h_tiles=4, v_tiles=2, cropped=False, full=True, 
-                lat=None, lon=None, input_csv_file="", input_shp_file = "", id_columns=None, buffer = 0, closest=False, 
+                lat=None, lon=None, input_csv_file="", input_shp_file = "", input_place_name = "", id_columns=None, buffer = 0, closest=False, 
                 disp=False, augment_metadata=False, update_pids = False):
         # set necessary directories
         self._set_dirs(dir_output)
         
         # call get_pids function first if path_pid is None
         if (path_pid is None) & (self.cache_pids_augmented.exists() == False):
             print("Getting pids...")
             path_pid = self.dir_output / "pids.csv"
             if path_pid.exists() & (update_pids == False):
                 print("update_pids is set to False. So the following csv file will be used: {}".format(path_pid))
             else:
                 self.get_pids(path_pid, lat=lat, lon=lon,
-                            input_csv_file=input_csv_file, input_shp_file = input_shp_file, id_columns=id_columns, buffer = buffer, closest=closest, disp=disp, augment_metadata=augment_metadata)
+                            input_csv_file=input_csv_file, input_shp_file = input_shp_file, input_place_name = input_place_name, 
+                            id_columns=id_columns, buffer = buffer, closest=closest, disp=disp, augment_metadata=augment_metadata)
         elif self.cache_pids_augmented.exists():
             # copy the cache pids_augmented to path_pid
             path_pid = self.dir_output / "pids.csv"
             shutil.copy2(self.cache_pids_augmented, path_pid)
             print("The augmented panorama IDs have been saved to {}".format(path_pid))
         # Horizontal Google Street View tiles
         # zoom 3: (8, 4); zoom 5: (26, 13) zoom 2: (4, 2) zoom 1: (2, 1);4:(8,16)
```

### Comparing `zensvi-0.1.9/src/zensvi/download/utils/UserAgent.csv` & `zensvi-0.2.0/src/zensvi/download/utils/UserAgent.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.9/src/zensvi/download/utils/geoprocess.py` & `zensvi-0.2.0/src/zensvi/download/utils/geoprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
     def process_polygon(self, gdf):
         batch_size = 100  # Modify this to a suitable value
         num_batches = (len(gdf) + batch_size - 1) // batch_size
         failed_geoms = []
         results = []
 
-        for i in tqdm(range(num_batches), desc=f"Processing polgyon by batch size {min(batch_size, len(gdf))}"):
+        for i in tqdm(range(num_batches), desc=f"Processing polygon by batch size {min(batch_size, len(gdf))}"):
             with ProcessPoolExecutor() as executor:
                 batch_futures = {}
                 for geom in gdf.geometry.iloc[i*batch_size : (i+1)*batch_size]:
                     if self.grid == False:
                         future = executor.submit(self.get_street_points, geom)
                     else:
                         future = executor.submit(self.create_point_grid, geom, self.grid_size)
```

### Comparing `zensvi-0.1.9/src/zensvi/download/utils/get_pids.py` & `zensvi-0.2.0/src/zensvi/download/utils/get_pids.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.9/src/zensvi/download/utils/helpers.py` & `zensvi-0.2.0/src/zensvi/download/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.9/src/zensvi/download/utils/imtool.py` & `zensvi-0.2.0/src/zensvi/download/utils/imtool.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.9/src/zensvi/download/utils/proxies.csv` & `zensvi-0.2.0/src/zensvi/download/utils/proxies.csv`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.9/src/zensvi/transform/transform_image.py` & `zensvi-0.2.0/src/zensvi/transform/transform_image.py`

 * *Files identical despite different names*

### Comparing `zensvi-0.1.9/PKG-INFO` & `zensvi-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zensvi
-Version: 0.1.9
+Version: 0.2.0
 Summary: This package handles downloading, cleaning, analyzing street view imagery in one-stop and zen manner.
 License: MIT
 Author: koito19960406
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

