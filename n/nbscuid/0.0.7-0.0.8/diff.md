# Comparing `tmp/nbscuid-0.0.7.tar.gz` & `tmp/nbscuid-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbscuid-0.0.7.tar", last modified: Wed May 17 21:58:29 2023, max compression
+gzip compressed data, was "nbscuid-0.0.8.tar", last modified: Thu May 25 22:57:55 2023, max compression
```

## Comparing `nbscuid-0.0.7.tar` & `nbscuid-0.0.8.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.306395 nbscuid-0.0.7/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      332 2023-05-03 23:21:30.000000 nbscuid-0.0.7/.gitignore
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      715 2023-05-04 22:27:17.000000 nbscuid-0.0.7/.readthedocs.yml
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1073 2023-02-24 23:26:03.000000 nbscuid-0.0.7/LICENSE
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     3115 2023-05-17 21:58:29.305905 nbscuid-0.0.7/PKG-INFO
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1405 2023-05-17 21:52:45.000000 nbscuid-0.0.7/README.md
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.240841 nbscuid-0.0.7/docs/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      638 2023-05-03 20:38:18.000000 nbscuid-0.0.7/docs/Makefile
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      804 2023-05-03 20:38:18.000000 nbscuid-0.0.7/docs/make.bat
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       32 2023-05-04 22:11:40.000000 nbscuid-0.0.7/docs/requirements.txt
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.267614 nbscuid-0.0.7/docs/source/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1915 2023-05-04 15:24:38.000000 nbscuid-0.0.7/docs/source/conf.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       35 2023-05-17 16:40:58.000000 nbscuid-0.0.7/docs/source/gettingstarted.md
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      497 2023-05-17 15:13:04.000000 nbscuid-0.0.7/docs/source/index.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       58 2023-05-03 20:44:35.000000 nbscuid-0.0.7/docs/source/modules.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      795 2023-05-03 20:44:35.000000 nbscuid-0.0.7/docs/source/nbscuid.rst
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     2023 2023-05-17 21:54:08.000000 nbscuid-0.0.7/docs/source/tutorialsetup.md
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.289735 nbscuid-0.0.7/nbscuid/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-02-24 23:33:45.000000 nbscuid-0.0.7/nbscuid/__init__.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1671 2023-05-16 17:45:54.000000 nbscuid-0.0.7/nbscuid/_jupyter-book-config-defaults.yml
--rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     1053 2023-04-24 23:15:21.000000 nbscuid-0.0.7/nbscuid/build.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     7640 2023-02-24 23:27:28.000000 nbscuid-0.0.7/nbscuid/cache.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-05-04 07:46:51.000000 nbscuid-0.0.7/nbscuid/quickstart.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1048 2023-03-08 00:11:40.000000 nbscuid-0.0.7/nbscuid/read.py
--rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     7289 2023-05-15 17:02:44.000000 nbscuid-0.0.7/nbscuid/run.py
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     9661 2023-05-03 23:11:22.000000 nbscuid-0.0.7/nbscuid/util.py
-drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-17 21:58:29.302905 nbscuid-0.0.7/nbscuid.egg-info/
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     3115 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/PKG-INFO
--rw-r--r--   0 eromashkova (38594) ncar      (1000)      612 2023-05-17 21:58:29.295826 nbscuid-0.0.7/nbscuid.egg-info/SOURCES.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        1 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/dependency_links.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       84 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/entry_points.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       94 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/requires.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)        8 2023-05-17 21:58:28.000000 nbscuid-0.0.7/nbscuid.egg-info/top_level.txt
--rw-r--r--   0 eromashkova (38594) ncar      (1000)     1020 2023-05-17 21:58:04.000000 nbscuid-0.0.7/pyproject.toml
--rw-r--r--   0 eromashkova (38594) ncar      (1000)       38 2023-05-17 21:58:29.306626 nbscuid-0.0.7/setup.cfg
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.711661 nbscuid-0.0.8/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      332 2023-05-03 23:21:30.000000 nbscuid-0.0.8/.gitignore
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      715 2023-05-04 22:27:17.000000 nbscuid-0.0.8/.readthedocs.yml
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1073 2023-02-24 23:26:03.000000 nbscuid-0.0.8/LICENSE
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     3205 2023-05-25 22:57:55.710971 nbscuid-0.0.8/PKG-INFO
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1495 2023-05-18 15:54:26.000000 nbscuid-0.0.8/README.md
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.585642 nbscuid-0.0.8/docs/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      638 2023-05-03 20:38:18.000000 nbscuid-0.0.8/docs/Makefile
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      804 2023-05-03 20:38:18.000000 nbscuid-0.0.8/docs/make.bat
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       32 2023-05-04 22:11:40.000000 nbscuid-0.0.8/docs/requirements.txt
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.590756 nbscuid-0.0.8/docs/source/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1915 2023-05-04 15:24:38.000000 nbscuid-0.0.8/docs/source/conf.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       35 2023-05-17 16:40:58.000000 nbscuid-0.0.8/docs/source/gettingstarted.md
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      497 2023-05-17 15:13:04.000000 nbscuid-0.0.8/docs/source/index.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       58 2023-05-03 20:44:35.000000 nbscuid-0.0.8/docs/source/modules.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      795 2023-05-03 20:44:35.000000 nbscuid-0.0.8/docs/source/nbscuid.rst
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1320 2023-05-25 22:52:39.000000 nbscuid-0.0.8/docs/source/tutorialsetup.md
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.598086 nbscuid-0.0.8/nbscuid/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-02-24 23:33:45.000000 nbscuid-0.0.8/nbscuid/__init__.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1671 2023-05-16 17:45:54.000000 nbscuid-0.0.8/nbscuid/_jupyter-book-config-defaults.yml
+-rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     1053 2023-04-24 23:15:21.000000 nbscuid-0.0.8/nbscuid/build.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     7640 2023-02-24 23:27:28.000000 nbscuid-0.0.8/nbscuid/cache.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        0 2023-05-04 07:46:51.000000 nbscuid-0.0.8/nbscuid/quickstart.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     1048 2023-03-08 00:11:40.000000 nbscuid-0.0.8/nbscuid/read.py
+-rwxr-xr-x   0 eromashkova (38594) ncar      (1000)     8247 2023-05-25 20:08:44.000000 nbscuid-0.0.8/nbscuid/run.py
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     9642 2023-05-25 22:23:26.000000 nbscuid-0.0.8/nbscuid/util.py
+drwxr-xr-x   0 eromashkova (38594) ncar      (1000)        0 2023-05-25 22:57:55.603561 nbscuid-0.0.8/nbscuid.egg-info/
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)     3205 2023-05-25 22:57:55.599283 nbscuid-0.0.8/nbscuid.egg-info/PKG-INFO
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      612 2023-05-25 22:57:55.600060 nbscuid-0.0.8/nbscuid.egg-info/SOURCES.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        1 2023-05-25 22:57:55.601259 nbscuid-0.0.8/nbscuid.egg-info/dependency_links.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       84 2023-05-25 22:57:55.602151 nbscuid-0.0.8/nbscuid.egg-info/entry_points.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       94 2023-05-25 22:57:55.602830 nbscuid-0.0.8/nbscuid.egg-info/requires.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)        8 2023-05-25 22:57:55.603658 nbscuid-0.0.8/nbscuid.egg-info/top_level.txt
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)      939 2023-05-25 22:56:29.000000 nbscuid-0.0.8/pyproject.toml
+-rw-r--r--   0 eromashkova (38594) ncar      (1000)       38 2023-05-25 22:57:55.711800 nbscuid-0.0.8/setup.cfg
```

### Comparing `nbscuid-0.0.7/.readthedocs.yml` & `nbscuid-0.0.8/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/LICENSE` & `nbscuid-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/PKG-INFO` & `nbscuid-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbscuid
-Version: 0.0.7
+Version: 0.0.8
 Summary: Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 Author-email: Elena Romashkova <eromashkova@ucar.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -32,15 +32,15 @@
 
 # nbscuid 🦑
 
 ### Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 
 This is a package to enable running notebook-based diagnostic workflows. Based on my-cesm-experiment by matt-long: https://github.com/matt-long/my-cesm-experiment. 
 
-See some examples of workflows at https://github.com/rmshkv/nbscuid-examples.
+See some examples of workflows at https://github.com/rmshkv/nbscuid-examples. For a basic tutorial, follow https://nbscuid.readthedocs.io/en/latest/tutorialsetup.html.
 
 ## Capabilities
 
 - Integration with data catalogs
 - Inject custom parameters into code and Markdown cells
 - Run many notebooks at once on a parameter set, or different parameters per notebook
 - Run different notebooks in different environments
```

### Comparing `nbscuid-0.0.7/README.md` & `nbscuid-0.0.8/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # nbscuid 🦑
 
 ### Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 
 This is a package to enable running notebook-based diagnostic workflows. Based on my-cesm-experiment by matt-long: https://github.com/matt-long/my-cesm-experiment. 
 
-See some examples of workflows at https://github.com/rmshkv/nbscuid-examples.
+See some examples of workflows at https://github.com/rmshkv/nbscuid-examples. For a basic tutorial, follow https://nbscuid.readthedocs.io/en/latest/tutorialsetup.html.
 
 ## Capabilities
 
 - Integration with data catalogs
 - Inject custom parameters into code and Markdown cells
 - Run many notebooks at once on a parameter set, or different parameters per notebook
 - Run different notebooks in different environments
```

### Comparing `nbscuid-0.0.7/docs/Makefile` & `nbscuid-0.0.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/docs/make.bat` & `nbscuid-0.0.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/docs/source/conf.py` & `nbscuid-0.0.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/docs/source/nbscuid.rst` & `nbscuid-0.0.8/docs/source/nbscuid.rst`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/nbscuid/_jupyter-book-config-defaults.yml` & `nbscuid-0.0.8/nbscuid/_jupyter-book-config-defaults.yml`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/nbscuid/build.py` & `nbscuid-0.0.8/nbscuid/build.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/nbscuid/cache.py` & `nbscuid-0.0.8/nbscuid/cache.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/nbscuid/read.py` & `nbscuid-0.0.8/nbscuid/read.py`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/nbscuid/run.py` & `nbscuid-0.0.8/nbscuid/run.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,39 +4,42 @@
 from glob import glob
 import papermill as pm
 import intake
 import nbscuid.util
 import nbscuid.cache
 import sys
 from dask.distributed import Client
+import dask
 import time
 
 def run():
-
+    
     # Get control structure
     config_path = str(sys.argv[1])
-    control = nbscuid.util.get_control_dict(config_path)
+    control = nbscuid.util.get_control_dict(config_path)    
     nbscuid.util.setup_book(config_path)
         
-    # Cluster management 
-    # Notebooks are configured to connect to this cluster    
-    cluster = nbscuid.util.get_Cluster(account=control['account'])
-    cluster.scale(4) # Should this be user modifiable?
+    if control['use_cluster']:    
+        # Cluster management 
+        # Notebooks are configured to connect to this cluster    
+        cluster = nbscuid.util.get_Cluster(account=control['account'])
+        cluster.scale(4) # Should this be user modifiable?
+    else:
+        cluster = None
     
     # Grab paths
     
     ### This code seems repetitive, is there a better way to do this?
-    run_dir = control['data_sources']['run_dir']
+    run_dir = os.path.expanduser(control['data_sources']['run_dir'])
     output_dir = run_dir + "/computed_notebooks/" + control['data_sources']['casename']
     cache_metadata_path = run_dir + "/cache_metadata_path"
     cache_data_path = run_dir + "/cache_data_path"
-    temp_data_path = run_dir + "/temp_data"
-    
-    nb_path_root = control['data_sources']['nb_path_root']
-    
+    temp_data_path = run_dir + "/temp_data" 
+    nb_path_root = os.path.expanduser(control['data_sources']['nb_path_root'])
+
     # Access catalog if it exists
 
     cat_path = None
     
     if 'path_to_cat_json' in control['data_sources']:
         use_catalog = True
         full_cat_path = control['data_sources']['path_to_cat_json']
@@ -49,14 +52,22 @@
             cat_subset = full_cat.search(**first_subset_kwargs)
             # This pulls out the name of the catalog from the path
             cat_subset_name = full_cat_path.split("/")[-1].split('.')[0] + "_subset"
             cat_subset.serialize(directory=temp_data_path, name=cat_subset_name, catalog_type="file")
             cat_path = temp_data_path + "/" + cat_subset_name + ".json"
         else:
             cat_path = full_cat_path
+            
+    
+    # Grabbing global params if they're included
+    
+    global_params = dict()
+    
+    if 'global_params' in control:
+        global_params = control['global_params']
         
     
     #####################################################################
     # Organizing notebooks into three lists
     
     precompute_nbs = dict()
     regular_nbs = dict()
@@ -80,44 +91,49 @@
     for key, item in precompute_nbs.items():
         if key in regular_nbs:
             regular_nbs.pop(key)
             
             
     #####################################################################
     # Pausing to wait for workers to avoid timeout error
-    
-    client = Client(cluster.scheduler_address)
-    
-    nworkers = 1
-    
-    waiting_count = 0
-    
-    while ((client.status == "running") and (len(client.scheduler_info()["workers"]) < nworkers)):
-        time.sleep(1.0)
-        if waiting_count == 0:
-            print("Waiting for Dask workers", end = '')
-        else:
-            print(".", end = '')
-        waiting_count += 1
         
-    print("\n")
+    if control['use_cluster']:
         
-    
-    client.close()
+        dask.config.set({'distributed.comm.timeouts.connect': '90s'})
+
+        client = Client(cluster.scheduler_address)
+
+        nworkers = 1
+
+        waiting_count = 0
+
+        while ((client.status == "running") and (len(client.scheduler_info()["workers"]) < nworkers)):
+            time.sleep(1.0)
+            if waiting_count == 0:
+                print("Waiting for Dask workers", end = '')
+            else:
+                print(".", end = '')
+            waiting_count += 1
+
+        print("\n")
+
+
+        client.close()
     
     
     #####################################################################
     # Calculating precompute notebooks
 
     ### To do: figure out how to organize the caching code better, keeping the whole block for now
     
     for nb, info in precompute_nbs.items():
     
         parameter_groups = info['parameter_groups']
-        use_cluster = info['use_cluster']
+        
+        use_cluster = control['use_cluster'] and info['use_cluster']
 
         ### passing in subset kwargs if they're provided
         if 'subset' in info:
             subset_kwargs = info['subset']
         else:
             subset_kwargs = {}
 
@@ -145,29 +161,28 @@
                 #if multiple matches exist, grabs an arbitrary one (FIX LATER)
                 asset_path = result_df.loc[0,'assets']
                 precompute_nbs[nb]["asset_path"] = asset_path
                 print("Fetching result from cache")
 
             else:
 
-                nb_api = pm.inspect_notebook(input_path)
-
                 asset_path = nbscuid.cache.make_filename(cache_data_path, input_path, full_cat_path) + ".nc"
 
-                if nb_api:
-                    parms_in = dict(**default_params)
-                    parms_in.update(dict(**parms))
-                    parms_in['path_to_cat'] = cat_path
+                parms_in = dict(**default_params)
+                parms_in.update(**global_params)
+                parms_in.update(dict(**parms))
+                parms_in['path_to_cat'] = cat_path
                     
-                    if use_cluster:
-                        parms_in['cluster_scheduler_address'] = cluster.scheduler_address
-                    parms_in['subset_kwargs'] = subset_kwargs
-                    parms_in['asset_path'] = asset_path
+                if use_cluster:
+                    parms_in['cluster_scheduler_address'] = cluster.scheduler_address
                 else:
-                    parms_in = {}
+                    parms_in['cluster_scheduler_address'] = None
+                        
+                parms_in['subset_kwargs'] = subset_kwargs
+                parms_in['asset_path'] = asset_path
 
                 print(f'executing {input_path}')
                 o = pm.execute_notebook(
                     input_path=input_path,
                     output_path=output_path,
                     kernel_name=info['kernel_name'],
                     parameters=parms_in,
@@ -178,32 +193,39 @@
 
                 nbscuid.cache.make_sidecar_entry(cache_metadata_path, 
                                                input_path, 
                                                full_cat_path, 
                                                asset_path=asset_path, 
                                                first_subset=first_subset_kwargs, 
                                                second_subset= subset_kwargs,
+                                               
+                                               ### this might need to be changed to parms_in, not parms, to include global parms  
                                                params=parms)
 
                 # this can only properly handle one save per notebook (FIX LATER)
                 precompute_nbs[nb]["asset_path"] = asset_path
     
     # Calculating regular notebooks
     
     for nb, info in regular_nbs.items():
-    
-        nbscuid.util.run_notebook(nb, info, cluster, cat_path, nb_path_root, output_dir)
+        
+        use_cluster = control['use_cluster'] and info['use_cluster']
+        
+        nbscuid.util.run_notebook(nb, info, use_cluster, cat_path, nb_path_root, output_dir, global_params, cluster=cluster)
     
     # Calculating notebooks with dependencies
     
     for nb, info in dependent_nbs.items():
+        
+        use_cluster = control['use_cluster'] and info['use_cluster']
     
         ### getting necessary asset:
         dependent_asset_path = precompute_nbs[info['dependency']]["asset_path"]
         
-        nbscuid.util.run_notebook(nb, info, cluster, cat_path, nb_path_root, output_dir, dependent_asset_path)
-
-    # Closing cluster
-    cluster.close()
+        nbscuid.util.run_notebook(nb, info, use_cluster, cat_path, nb_path_root, output_dir, global_params, dependent_asset_path=dependent_asset_path, cluster=cluster)
+    
+    if control['use_cluster']:
+        # Closing cluster
+        cluster.close()
     
     return None
```

### Comparing `nbscuid-0.0.7/nbscuid/util.py` & `nbscuid-0.0.8/nbscuid/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -80,14 +80,15 @@
     def ensure_installed(self):
         """install a conda kernel in a location findable by `nbconvert` etc."""
 
         if self.isinstalled():
             return
 
         path = self.getcwd()
+        print(path)
         if path is None:
             raise ValueError(f'conda kernel "{self.kernel_name}" not found')
         path = path / pathlib.Path("share/jupyter/kernels")
 
         kernels_in_conda_env = jupyter_client.kernelspec._list_kernels_in(path)
         py_kernel_key = [k for k in kernels_in_conda_env.keys() if "python" in k][0]
         kernel_path = kernels_in_conda_env[py_kernel_key]
@@ -137,15 +138,15 @@
 
 def setup_book(config_path):
     """Setup run directory and output jupyter book"""
 
     control = get_control_dict(config_path)
 
     # ensure directory
-    run_dir = control['data_sources']["run_dir"]
+    run_dir = os.path.expanduser(control['data_sources']["run_dir"])
     output_root = run_dir + "/computed_notebooks"
     
     os.makedirs(output_root, exist_ok=True)
     
     output_dir = f'{output_root}/{control["data_sources"]["casename"]}'
     
     os.makedirs(output_dir, exist_ok=True)
@@ -177,15 +178,15 @@
 
     # write config file
     with open(f"{output_dir}/_config.yml", "w") as fid:
         yaml.dump(config, fid, sort_keys=False)
 
     # get list of computational notebooks
     
-    nb_path_root = control['data_sources']['nb_path_root']
+    nb_path_root = os.path.expanduser(control['data_sources']['nb_path_root'])
     
     compute_notebooks = [f"{nb_path_root}/{f}.ipynb" for f in control["compute_notebooks"].keys()]
 
     # get toc files; ignore glob expressions
     toc_files = get_toc_files(nb_path_root, toc, include_glob=False)
     copy_files = list(set(toc_files) - set(compute_notebooks))
     
@@ -224,26 +225,25 @@
                     file_list_ext = _toc_files(sub, file_list_ext)
                 file_list.extend(file_list_ext)
 
         return file_list
 
     return _toc_files(toc_dict)
 
-def run_notebook(nb, info, cluster, cat_path, nb_path_root, output_dir, dependent_asset_path=None):
+def run_notebook(nb, info, use_cluster, cat_path, nb_path_root, output_dir, global_params, dependent_asset_path=None, cluster=None):
     """
     nb: key from dict of notebooks
     info: various specifications for the notebook, originally from config.yml
     use_catalog: bool specified earlier, specifying if whole collection uses a catalog or not
     nb_path_root: from config.yml, path to folder containing template notebooks
     output_dir: set directory where computed notebooks get put
     
     """
 
     parameter_groups = info['parameter_groups']
-    use_cluster = info['use_cluster']
 
     ### passing in subset kwargs if they're provided
     if 'subset' in info:
         subset_kwargs = info['subset']
     else:
         subset_kwargs = {}
 
@@ -255,35 +255,33 @@
 
         input_path = f'{nb_path_root}/{nb}.ipynb'
         output_path = (
             f'{output_dir}/{nb}-{key}.ipynb'
             if key != 'none' else f'{output_dir}/{nb}.ipynb'
         )
 
-        # check notebook expectations
-        nb_api = pm.inspect_notebook(input_path)
 
-        if nb_api:
+        ### all of these things should be optional
+        parms_in = dict(**default_params)
+        parms_in.update(**global_params)
+        parms_in.update(dict(**parms))
             
-            ### all of these things should be optional
-            parms_in = dict(**default_params)
-            parms_in.update(dict(**parms))
-            
-            if use_cluster:
-                parms_in['cluster_scheduler_address'] = cluster.scheduler_address
-            parms_in['subset_kwargs'] = subset_kwargs            
+        if use_cluster:
+            parms_in['cluster_scheduler_address'] = cluster.scheduler_address
+        else:
+            parms_in['cluster_scheduler_address'] = None
+                
+        parms_in['subset_kwargs'] = subset_kwargs            
             
-            if cat_path != None:
-                parms_in['path_to_cat'] = cat_path
-            if dependent_asset_path != None:
-                print(dependent_asset_path)
-                parms_in['asset_path'] = dependent_asset_path
+        if cat_path != None:
+            parms_in['path_to_cat'] = cat_path
+        if dependent_asset_path != None:
+            print(dependent_asset_path)
+            parms_in['asset_path'] = dependent_asset_path
                 
-        else:
-            parms_in = {}
 
         print(f'Executing {input_path}')
         o = pm.execute_notebook(
             input_path=input_path,
             output_path=output_path,
             kernel_name=info['kernel_name'],
             parameters=parms_in,
```

### Comparing `nbscuid-0.0.7/nbscuid.egg-info/PKG-INFO` & `nbscuid-0.0.8/nbscuid.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbscuid
-Version: 0.0.7
+Version: 0.0.8
 Summary: Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 Author-email: Elena Romashkova <eromashkova@ucar.edu>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -32,15 +32,15 @@
 
 # nbscuid 🦑
 
 ### Notebook-Based, Super CUstomizable Infrastructure for Diagnostics
 
 This is a package to enable running notebook-based diagnostic workflows. Based on my-cesm-experiment by matt-long: https://github.com/matt-long/my-cesm-experiment. 
 
-See some examples of workflows at https://github.com/rmshkv/nbscuid-examples.
+See some examples of workflows at https://github.com/rmshkv/nbscuid-examples. For a basic tutorial, follow https://nbscuid.readthedocs.io/en/latest/tutorialsetup.html.
 
 ## Capabilities
 
 - Integration with data catalogs
 - Inject custom parameters into code and Markdown cells
 - Run many notebooks at once on a parameter set, or different parameters per notebook
 - Run different notebooks in different environments
```

### Comparing `nbscuid-0.0.7/nbscuid.egg-info/SOURCES.txt` & `nbscuid-0.0.8/nbscuid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nbscuid-0.0.7/pyproject.toml` & `nbscuid-0.0.8/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 [build-system]
 requires = ["setuptools>=61.0", "setuptools_scm[toml]>=6.2"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
-#include-package-data = true
 packages = ["nbscuid"]
 
-#[tool.setuptools.package-data]
-#mypkg = ["*.yml"]
-
 
 [project]
 name = "nbscuid"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Elena Romashkova", email="eromashkova@ucar.edu" },
 ]
 description = "Notebook-Based, Super CUstomizable Infrastructure for Diagnostics"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.9"
```

