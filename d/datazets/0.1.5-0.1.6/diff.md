# Comparing `tmp/datazets-0.1.5.tar.gz` & `tmp/datazets-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazets-0.1.5.tar", last modified: Fri May 26 15:32:28 2023, max compression
+gzip compressed data, was "datazets-0.1.6.tar", last modified: Fri May 26 18:19:42 2023, max compression
```

## Comparing `datazets-0.1.5.tar` & `datazets-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:32:28.301885 datazets-0.1.5/
--rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     4613 2023-05-26 15:32:28.300885 datazets-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 15:32:28.283570 datazets-0.1.5/datazets/
--rw-rw-rw-   0        0        0      765 2023-05-26 15:13:41.000000 datazets-0.1.5/datazets/__init__.py
--rw-rw-rw-   0        0        0    18570 2023-05-26 15:22:45.000000 datazets-0.1.5/datazets/datazets.py
--rw-rw-rw-   0        0        0      987 2023-05-14 16:33:27.000000 datazets-0.1.5/datazets/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:32:28.299899 datazets-0.1.5/datazets/utils/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.5/datazets/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:32:28.297971 datazets-0.1.5/datazets.egg-info/
--rw-rw-rw-   0        0        0     4613 2023-05-26 15:32:27.000000 datazets-0.1.5/datazets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-26 15:32:28.000000 datazets-0.1.5/datazets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:32:27.000000 datazets-0.1.5/datazets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-26 15:32:27.000000 datazets-0.1.5/datazets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 15:32:27.000000 datazets-0.1.5/datazets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 15:32:28.301885 datazets-0.1.5/setup.cfg
--rw-rw-rw-   0        0        0     1382 2023-05-13 18:52:09.000000 datazets-0.1.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:19:42.059783 datazets-0.1.6/
+-rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     4613 2023-05-26 18:19:42.059783 datazets-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 18:19:42.043962 datazets-0.1.6/datazets/
+-rw-rw-rw-   0        0        0      765 2023-05-26 18:14:25.000000 datazets-0.1.6/datazets/__init__.py
+-rw-rw-rw-   0        0        0    19064 2023-05-26 18:19:14.000000 datazets-0.1.6/datazets/datazets.py
+-rw-rw-rw-   0        0        0     1069 2023-05-26 18:19:02.000000 datazets-0.1.6/datazets/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:19:42.058398 datazets-0.1.6/datazets/utils/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.6/datazets/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:19:42.056793 datazets-0.1.6/datazets.egg-info/
+-rw-rw-rw-   0        0        0     4613 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 18:19:41.000000 datazets-0.1.6/datazets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 18:19:42.060797 datazets-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0     1382 2023-05-26 18:14:10.000000 datazets-0.1.6/setup.py
```

### Comparing `datazets-0.1.5/LICENSE` & `datazets-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `datazets-0.1.5/PKG-INFO` & `datazets-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.5
+Version: 0.1.6
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.5.tar.gz
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `datazets-0.1.5/README.md` & `datazets-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `datazets-0.1.5/datazets/datazets.py` & `datazets-0.1.6/datazets/datazets.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,27 +24,27 @@
 formatter = logging.Formatter('[datazets] >%(levelname)s> %(message)s')
 console.setFormatter(formatter)
 logger.addHandler(console)
 logger = logging.getLogger(__name__)
 
 
 # %% Import example dataset.
-def get(data=None, url=None, sep=',', verbose='info', **args):
+def get(data=None, url=None, sep=',', verbose='info', overwrite=False, **args):
     """Import example dataset from github source.
 
     Import one of the few datasets from github source or specify your own download url link.
 
     Parameters
     ----------
     data : str
         Multicollinear data sets:
             * 'titanic'
             * 'student'
             * 'fifa'
-            * 'DS_salaries'
+            * 'ds_salaries'
             * 'waterpump'
             * 'elections'
             * 'tips'
             * 'predictive_maintenance'
         source-target
             * 'energy'
             * 'stormofswords'
@@ -115,23 +115,27 @@
     * Census Income. (1996). UCI Machine Learning Repository. https://doi.org/10.24432/C5S595.
 
     """
     set_logger(verbose=verbose)
     if data is None and url is None:
         logger.error('Input parameter <data> or <url> should be used.')
         return None
-
+    
     # Get and Set data information
     dataproperties = get_dataproperties(data, sep, url)
     logger.info('Import dataset [%s]' %(dataproperties['input']))
 
     if dataproperties['url'] is None:
         logger.info('Nothing to download.')
         return None
 
+    if overwrite and os.path.isfile(os.path.join(dataproperties['curpath'], dataproperties['filename'])):
+        logger.info('Removing [%s] from disk.' %(dataproperties['input']))
+        os.remove(os.path.join(dataproperties['curpath'], dataproperties['filename']))
+
     # Import dataset
     if dataproperties['type']=='files':
         df = _extract_files(dataproperties)
     elif dataproperties['type']=='synthetic':
         df = _generate_data(dataproperties['filename'], **args)
     elif dataproperties['type']=='DAG':
         df = _extract_files(dataproperties, targetdir=os.path.join(dataproperties['curpath'], dataproperties['input']), ext='*')
@@ -472,15 +476,17 @@
     return PATH_TO_DATA
 
 
 # %% URL to disk
 def url2disk(urls, save_dir):
     """Write url locations to disk.
 
-    Import images from url locations and store to disk.
+    Images can also be imported from url locations.
+    Each image is first downloaded and stored on a (specified) temp directory.
+    In this example we will download 5 images from url locations. Note that url images and path locations can be combined.
 
     Parameters
     ----------
     urls : list
         list of url locations with image path.
     save_dir : str
         location to disk.
```

### Comparing `datazets-0.1.5/datazets/examples.py` & `datazets-0.1.6/datazets/examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # %%
 import datazets as dz
+df = dz.get(data='ds_salaries', overwrite=True)
+
+
+# %%
+import datazets as dz
 url='https://archive.ics.uci.edu/ml/machine-learning-databases/adult/adult.data'
 df = dz.get(url=url, sep=',')
 df.shape
 
 # %%
 import datazets as dz
 df = dz.get(data='auto_mpg')
```

### Comparing `datazets-0.1.5/datazets.egg-info/PKG-INFO` & `datazets-0.1.6/datazets.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.5
+Version: 0.1.6
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.5.tar.gz
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.6.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `datazets-0.1.5/setup.py` & `datazets-0.1.6/setup.py`

 * *Files identical despite different names*

