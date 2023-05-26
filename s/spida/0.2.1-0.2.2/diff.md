# Comparing `tmp/spida-0.2.1.tar.gz` & `tmp/spida-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.2.1.tar", last modified: Fri May 26 18:51:27 2023, max compression
+gzip compressed data, was "spida-0.2.2.tar", last modified: Fri May 26 20:20:04 2023, max compression
```

## Comparing `spida-0.2.1.tar` & `spida-0.2.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.786683 spida-0.2.1/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2.1/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2.1/MANIFEST.in
--rw-rw-rw-   0        0        0     6621 2023-05-26 18:51:27.785675 spida-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0     6163 2023-05-20 06:34:04.000000 spida-0.2.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-26 18:51:27.786683 spida-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0      779 2023-05-26 18:50:27.000000 spida-0.2.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.744030 spida-0.2.1/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2.1/spida/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.776465 spida-0.2.1/spida/data/
--rw-rw-rw-   0        0        0        2 2023-05-26 18:43:50.000000 spida-0.2.1/spida/data/config.json
--rw-rw-rw-   0        0        0    16250 2023-05-26 18:34:56.000000 spida-0.2.1/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.783149 spida-0.2.1/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2.1/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5943 2023-05-19 20:05:30.000000 spida-0.2.1/spida/utils/img.py
--rw-rw-rw-   0        0        0     1042 2023-05-19 13:56:29.000000 spida-0.2.1/spida/utils/misc.py
--rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.2.1/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.774335 spida-0.2.1/spida.egg-info/
--rw-rw-rw-   0        0        0     6621 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 20:20:04.287084 spida-0.2.2/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     6621 2023-05-26 20:20:04.286072 spida-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6163 2023-05-20 06:34:04.000000 spida-0.2.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 20:20:04.287084 spida-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-05-26 20:00:03.000000 spida-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:20:04.238954 spida-0.2.2/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2.2/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:20:04.277863 spida-0.2.2/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-26 19:59:37.000000 spida-0.2.2/spida/data/config.json
+-rw-rw-rw-   0        0        0    16254 2023-05-26 19:17:58.000000 spida-0.2.2/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:20:04.284985 spida-0.2.2/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2.2/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     5913 2023-05-26 19:58:34.000000 spida-0.2.2/spida/utils/img.py
+-rw-rw-rw-   0        0        0      935 2023-05-26 19:59:04.000000 spida-0.2.2/spida/utils/misc.py
+-rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.2.2/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:20:04.275850 spida-0.2.2/spida.egg-info/
+-rw-rw-rw-   0        0        0     6621 2023-05-26 20:20:04.000000 spida-0.2.2/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-26 20:20:04.000000 spida-0.2.2/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 20:20:04.000000 spida-0.2.2/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-26 20:20:04.000000 spida-0.2.2/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 20:20:04.000000 spida-0.2.2/spida.egg-info/top_level.txt
```

### Comparing `spida-0.2.1/LICENSE` & `spida-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.2.1/PKG-INFO` & `spida-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `spida-0.2.1/README.md` & `spida-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `spida-0.2.1/setup.py` & `spida-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.2.1",
+    version="0.2.2",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
```

### Comparing `spida-0.2.1/spida/stable_diffusion.py` & `spida-0.2.2/spida/stable_diffusion.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
         A dictionary containing the settings for a ControlNet unit.
     """
     if search:
         annotator_res = search_annotators(annotator)[0]
     else:
         annotator_res = annotator
     if model is None:
-        model = search_cnet_models(annotator)[0]
+        model = search_cnet_models(annotator_res)[0]
     if resolution is None:
         resolution = min(annotated_img.shape[:2])
     if mask is None:
         mask_b64str = None
     else:
         mask_b64str = utils.img.img2b64str(mask)
     input_b64str = utils.img.img2b64str(annotated_img)
```

### Comparing `spida-0.2.1/spida/utils/img.py` & `spida-0.2.2/spida/utils/img.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import io
+import glob
 import base64
 from PIL import Image
 from matplotlib import pyplot as plt
 import math
 import numpy as np
 from tkinter import Tk, filedialog
 
-from . import misc
-
 Tk().withdraw()
 
 
 def show(
     img: np.ndarray, use_matplot: bool = False, cmap: str = None, vmin=None, vmax=None
 ):
     """
@@ -47,18 +46,19 @@
     img : numpy.ndarray
         The image array to be saved.
 
     file_name : str, optional
         The filename of the output file. If None, a file name will be automatically generated. Default is None.
     """
     if file_name is None:
-        png_files = [i for i in misc.get_cwd_files() if i.endswith(".png")]
+        png_files = glob.glob("img_*.png")
         if png_files:
-            img_num = int(png_files[-1].split(".")[0].split("_")[-1])
-            file_name = f"img_{img_num+1}.png"
+            nums = [int(i[4:-4]) for i in png_files]
+            fnum = max(nums) + 1
+            file_name = f"img_{fnum}.png"
         else:
             file_name = "img_0.png"
     Image.fromarray(img).save(file_name)
 
 
 def open(path: str = None):
     """
```

### Comparing `spida-0.2.1/spida/utils/misc.py` & `spida-0.2.2/spida/utils/misc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from difflib import SequenceMatcher
-import os
 
 
 def search(query: str, lst: list, match_case=True):
     """
     Searches a list of strings and returns them sorted by similarity to a query string.
 
     Parameters
@@ -25,11 +24,7 @@
     """
     if match_case:
         query_lower = query.lower()
         sims = [SequenceMatcher(None, query_lower, i.lower()).ratio() for i in lst]
     else:
         sims = [SequenceMatcher(None, query, i).ratio() for i in lst]
     return [i for _, i in sorted(zip(sims, lst), reverse=True)]
-
-
-def get_cwd_files():
-    return [f for f in os.listdir(os.getcwd()) if os.path.isfile(f)]
```

### Comparing `spida-0.2.1/spida/utils/net.py` & `spida-0.2.2/spida/utils/net.py`

 * *Files identical despite different names*

### Comparing `spida-0.2.1/spida.egg-info/PKG-INFO` & `spida-0.2.2/spida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

