# Comparing `tmp/samscore-1.3.tar.gz` & `tmp/samscore-1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samscore-1.3.tar", last modified: Fri May 26 17:16:45 2023, max compression
+gzip compressed data, was "samscore-1.31.tar", last modified: Fri May 26 17:32:30 2023, max compression
```

## Comparing `samscore-1.3.tar` & `samscore-1.31.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 17:16:45.932255 samscore-1.3/
--rw-rw-rw-   0        0        0     1357 2021-10-01 16:16:03.000000 samscore-1.3/LICENSE
--rw-rw-rw-   0        0        0     2118 2023-05-26 17:16:45.932255 samscore-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2023-05-26 15:56:37.000000 samscore-1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 17:16:45.900865 samscore-1.3/data/
--rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.3/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:16:45.900865 samscore-1.3/data/dataset/
--rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.3/data/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:16:45.900865 samscore-1.3/samscore/
--rw-rw-rw-   0        0        0     3725 2023-05-24 20:49:46.000000 samscore-1.3/samscore/__init__.py
--rw-rw-rw-   0        0        0     8060 2023-05-26 17:16:36.000000 samscore-1.3/samscore/samscore.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:16:45.916490 samscore-1.3/samscore.egg-info/
--rw-rw-rw-   0        0        0     2118 2023-05-26 17:16:45.000000 samscore-1.3/samscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-26 17:16:45.000000 samscore-1.3/samscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 17:16:45.000000 samscore-1.3/samscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2023-05-26 17:16:45.000000 samscore-1.3/samscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-26 17:16:45.000000 samscore-1.3/samscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 17:16:45.932255 samscore-1.3/setup.cfg
--rw-rw-rw-   0        0        0      804 2023-05-26 17:13:20.000000 samscore-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 17:16:45.932255 samscore-1.3/util/
--rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.3/util/__init__.py
--rw-rw-rw-   0        0        0     2023 2021-10-01 16:16:03.000000 samscore-1.3/util/html.py
--rw-rw-rw-   0        0        0     1433 2021-10-01 16:16:03.000000 samscore-1.3/util/util.py
--rw-rw-rw-   0        0        0     8568 2021-10-01 16:16:03.000000 samscore-1.3/util/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:32:30.289377 samscore-1.31/
+-rw-rw-rw-   0        0        0     1357 2021-10-01 16:16:03.000000 samscore-1.31/LICENSE
+-rw-rw-rw-   0        0        0     2119 2023-05-26 17:32:30.288379 samscore-1.31/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2023-05-26 15:56:37.000000 samscore-1.31/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 17:32:30.238050 samscore-1.31/data/
+-rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.31/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:32:30.239051 samscore-1.31/data/dataset/
+-rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.31/data/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:32:30.243051 samscore-1.31/samscore/
+-rw-rw-rw-   0        0        0     3725 2023-05-24 20:49:46.000000 samscore-1.31/samscore/__init__.py
+-rw-rw-rw-   0        0        0     8069 2023-05-26 17:30:54.000000 samscore-1.31/samscore/samscore.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:32:30.279323 samscore-1.31/samscore.egg-info/
+-rw-rw-rw-   0        0        0     2119 2023-05-26 17:32:29.000000 samscore-1.31/samscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-26 17:32:30.000000 samscore-1.31/samscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 17:32:29.000000 samscore-1.31/samscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2023-05-26 17:32:29.000000 samscore-1.31/samscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-26 17:32:29.000000 samscore-1.31/samscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 17:32:30.290376 samscore-1.31/setup.cfg
+-rw-rw-rw-   0        0        0      805 2023-05-26 17:31:00.000000 samscore-1.31/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 17:32:30.287377 samscore-1.31/util/
+-rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.31/util/__init__.py
+-rw-rw-rw-   0        0        0     2023 2021-10-01 16:16:03.000000 samscore-1.31/util/html.py
+-rw-rw-rw-   0        0        0     1433 2021-10-01 16:16:03.000000 samscore-1.31/util/util.py
+-rw-rw-rw-   0        0        0     8568 2021-10-01 16:16:03.000000 samscore-1.31/util/visualizer.py
```

### Comparing `samscore-1.3/LICENSE` & `samscore-1.31/LICENSE`

 * *Files identical despite different names*

### Comparing `samscore-1.3/PKG-INFO` & `samscore-1.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samscore
-Version: 1.3
+Version: 1.31
 Summary: SAMScore Similarity Metric
 Home-page: https://github.com/Kent0n-Li/SAMScore
 Author: Yunxiang Li
 Author-email: yunxiang.li@utsouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `samscore-1.3/README.md` & `samscore-1.31/README.md`

 * *Files identical despite different names*

### Comparing `samscore-1.3/samscore/__init__.py` & `samscore-1.31/samscore/__init__.py`

 * *Files identical despite different names*

### Comparing `samscore-1.3/samscore/samscore.py` & `samscore-1.31/samscore/samscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,16 +128,15 @@
 
     response = requests.get(url+model_name, stream=True)
 
     if response.status_code == 200:
         with open(destination, "wb") as file:
             for chunk in response.iter_content(chunk_size=chunk_size):
                 file.write(chunk)
-        print("File downloaded successfully.")
-        return destination
+        print("Weights downloaded successfully.")
     else:
         print("Failed to download file. Status code:", response.status_code)
 
 
 class SAMScore(nn.Module):
     def __init__(self, model_type = "vit_l", model_weight_path = None ,version='1.0'):
         """ Initializes a perceptual loss torch.nn.Module
@@ -176,15 +175,16 @@
             
         # to download the model weights from online link
         if model_weight_path is None:
             save_path = "weights"
             destination_path = os.path.join(save_path,online_model_weight_name)
             if not os.path.exists(destination_path):
                 os.makedirs(save_path,exist_ok=True)
-                model_weight_path = download_model(url = download_url,model_name = online_model_weight_name, destination= destination_path)
+                download_model(url = download_url,model_name = online_model_weight_name, destination= destination_path)
+                model_weight_path = destination_path
 
                                                
 
         self.version = version
         self.model_type = model_type
         self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         self.sam = sam_model_registry[self.model_type](checkpoint=model_weight_path)
```

### Comparing `samscore-1.3/samscore.egg-info/PKG-INFO` & `samscore-1.31/samscore.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: samscore
-Version: 1.3
+Version: 1.31
 Summary: SAMScore Similarity Metric
 Home-page: https://github.com/Kent0n-Li/SAMScore
 Author: Yunxiang Li
 Author-email: yunxiang.li@utsouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `samscore-1.3/util/html.py` & `samscore-1.31/util/html.py`

 * *Files identical despite different names*

### Comparing `samscore-1.3/util/util.py` & `samscore-1.31/util/util.py`

 * *Files identical despite different names*

### Comparing `samscore-1.3/util/visualizer.py` & `samscore-1.31/util/visualizer.py`

 * *Files identical despite different names*

