# Comparing `tmp/datazets-0.1.4.tar.gz` & `tmp/datazets-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datazets-0.1.4.tar", last modified: Sun May 14 16:58:27 2023, max compression
+gzip compressed data, was "datazets-0.1.5.tar", last modified: Fri May 26 15:32:28 2023, max compression
```

## Comparing `datazets-0.1.4.tar` & `datazets-0.1.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-14 16:58:27.069577 datazets-0.1.4/
--rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.4/LICENSE
--rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.4/MANIFEST.in
--rw-rw-rw-   0        0        0     4613 2023-05-14 16:58:27.068583 datazets-0.1.4/PKG-INFO
--rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-14 16:58:27.026581 datazets-0.1.4/datazets/
--rw-rw-rw-   0        0        0      755 2023-05-14 16:57:49.000000 datazets-0.1.4/datazets/__init__.py
--rw-rw-rw-   0        0        0    15624 2023-05-14 16:52:31.000000 datazets-0.1.4/datazets/datazets.py
--rw-rw-rw-   0        0        0      987 2023-05-14 16:33:27.000000 datazets-0.1.4/datazets/examples.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:58:27.066587 datazets-0.1.4/datazets/utils/
--rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.4/datazets/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-14 16:58:27.063593 datazets-0.1.4/datazets.egg-info/
--rw-rw-rw-   0        0        0     4613 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      287 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-14 16:58:26.000000 datazets-0.1.4/datazets.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-14 16:58:27.069577 datazets-0.1.4/setup.cfg
--rw-rw-rw-   0        0        0     1382 2023-05-13 18:52:09.000000 datazets-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:32:28.301885 datazets-0.1.5/
+-rw-rw-rw-   0        0        0     1121 2022-03-22 18:16:18.000000 datazets-0.1.5/LICENSE
+-rw-rw-rw-   0        0        0       56 2023-05-12 07:39:26.000000 datazets-0.1.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     4613 2023-05-26 15:32:28.300885 datazets-0.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4060 2023-05-13 19:04:51.000000 datazets-0.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 15:32:28.283570 datazets-0.1.5/datazets/
+-rw-rw-rw-   0        0        0      765 2023-05-26 15:13:41.000000 datazets-0.1.5/datazets/__init__.py
+-rw-rw-rw-   0        0        0    18570 2023-05-26 15:22:45.000000 datazets-0.1.5/datazets/datazets.py
+-rw-rw-rw-   0        0        0      987 2023-05-14 16:33:27.000000 datazets-0.1.5/datazets/examples.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:32:28.299899 datazets-0.1.5/datazets/utils/
+-rw-rw-rw-   0        0        0        0 2020-01-01 22:53:45.000000 datazets-0.1.5/datazets/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:32:28.297971 datazets-0.1.5/datazets.egg-info/
+-rw-rw-rw-   0        0        0     4613 2023-05-26 15:32:27.000000 datazets-0.1.5/datazets.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      287 2023-05-26 15:32:28.000000 datazets-0.1.5/datazets.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:32:27.000000 datazets-0.1.5/datazets.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2023-05-26 15:32:27.000000 datazets-0.1.5/datazets.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 15:32:27.000000 datazets-0.1.5/datazets.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:32:28.301885 datazets-0.1.5/setup.cfg
+-rw-rw-rw-   0        0        0     1382 2023-05-13 18:52:09.000000 datazets-0.1.5/setup.py
```

### Comparing `datazets-0.1.4/LICENSE` & `datazets-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `datazets-0.1.4/PKG-INFO` & `datazets-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.4
+Version: 0.1.5
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.4.tar.gz
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.5.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `datazets-0.1.4/README.md` & `datazets-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `datazets-0.1.4/datazets/datazets.py` & `datazets-0.1.5/datazets/datazets.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,18 +7,19 @@
 # Licence     : See licences
 # --------------------------------------------------
 
 import os
 import pandas as pd
 import numpy as np
 import requests
-# from urllib.parse import urlparse
 import logging
 import zipfile
 import fnmatch
+from io import BytesIO
+from urllib.parse import urlparse
 
 logger = logging.getLogger('')
 for handler in logger.handlers[:]:
     logger.removeHandler(handler)
 console = logging.StreamHandler()
 formatter = logging.Formatter('[datazets] >%(levelname)s> %(message)s')
 console.setFormatter(formatter)
@@ -464,8 +465,89 @@
 # %%
 def _makedir(filename, url):
     curpath = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data')
     # filename = os.path.basename(urlparse(url).path)
     PATH_TO_DATA = os.path.join(curpath, filename)
     if not os.path.isdir(curpath):
         os.makedirs(curpath, exist_ok=True)
-    return PATH_TO_DATA
+    return PATH_TO_DATA
+
+
+# %% URL to disk
+def url2disk(urls, save_dir):
+    """Write url locations to disk.
+
+    Import images from url locations and store to disk.
+
+    Parameters
+    ----------
+    urls : list
+        list of url locations with image path.
+    save_dir : str
+        location to disk.
+
+    Returns
+    -------
+    urls : list of str.
+        list to url locations that are now stored on disk.
+
+    Examples
+    --------
+    >>> # Init with default settings
+    >>> import clustimage as cl
+    >>>
+    >>> # Importing the files files from disk, cleaning and pre-processing
+    >>> url_to_images = ['https://erdogant.github.io/datasets/images/flower_images/flower_orange.png',
+    >>>                  'https://erdogant.github.io/datasets/images/flower_images/flower_white_1.png',
+    >>>                  'https://erdogant.github.io/datasets/images/flower_images/flower_white_2.png',
+    >>>                  'https://erdogant.github.io/datasets/images/flower_images/flower_yellow_1.png',
+    >>>                  'https://erdogant.github.io/datasets/images/flower_images/flower_yellow_2.png']
+    >>>
+    >>> # Import into model
+    >>> results = cl.url2disk(url_to_images, r'c:/temp/out/')
+    >>>
+
+    """
+    try:
+        from PIL import Image
+    except:
+        logger.error('Could not import <pillow> library. Try to pip install first <pip install pillow>')
+
+    if not isinstance(urls, list): urls = [urls]
+    # Set filepath to the output of urls in case no url are used. Then the normal filepath is returned.
+    filepath = urls.copy()
+    idx_url = np.where(list(map(lambda x: x[0:4]=='http', filepath)))[0]
+    if len(idx_url)>0:
+        logger.info('[%.0d] urls are detected and stored on disk: [%s]' %(len(idx_url), save_dir))
+    else:
+        urls = None
+
+    if not os.path.isdir(save_dir):
+        logger.info('Create dir: [%s]' %(save_dir))
+        os.mkdir(save_dir)
+
+    for idx in idx_url:
+        try:
+            # Make connection to file
+            response = requests.get(urls[idx])
+            img = Image.open(BytesIO(response.content))
+            # Get url
+            url = urlparse(urls[idx])
+            # Extract filename from url
+            url_filename = os.path.basename(url.path)
+            path_to_file = os.path.join(save_dir, url_filename)
+            if os.path.isfile(path_to_file):
+                logger.info('File already exists and is overwritten: [%s]' %(url.path))
+            else:
+                logger.info('Downloading [%s]' %(urls[idx]))
+            # save a image using extension
+            img.save(path_to_file)
+            # Store new location
+            filepath[idx] = path_to_file
+        except:
+            logger.warning('error downloading file from [%s]' %(urls[idx]))
+
+    # Make dictionary output
+    out = {'url': urls, 'pathnames': filepath}
+
+    # Return
+    return out
```

### Comparing `datazets-0.1.4/datazets/examples.py` & `datazets-0.1.5/datazets/examples.py`

 * *Files identical despite different names*

### Comparing `datazets-0.1.4/datazets.egg-info/PKG-INFO` & `datazets-0.1.5/datazets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: datazets
-Version: 0.1.4
+Version: 0.1.5
 Summary: Datazets is a python package to import well known example data sets.
 Home-page: https://github.com/erdogant/datazets
-Download-URL: https://github.com/erdogant/datazets/archive/0.1.4.tar.gz
+Download-URL: https://github.com/erdogant/datazets/archive/0.1.5.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
```

### Comparing `datazets-0.1.4/setup.py` & `datazets-0.1.5/setup.py`

 * *Files identical despite different names*

