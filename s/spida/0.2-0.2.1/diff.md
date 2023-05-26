# Comparing `tmp/spida-0.2.tar.gz` & `tmp/spida-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spida-0.2.tar", last modified: Sat May 20 19:51:20 2023, max compression
+gzip compressed data, was "spida-0.2.1.tar", last modified: Fri May 26 18:51:27 2023, max compression
```

## Comparing `spida-0.2.tar` & `spida-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.802600 spida-0.2/
--rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2/LICENSE
--rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     6619 2023-05-20 19:51:20.801581 spida-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6163 2023-05-20 06:34:04.000000 spida-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-20 19:51:20.803606 spida-0.2/setup.cfg
--rw-rw-rw-   0        0        0      777 2023-05-20 19:51:03.000000 spida-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.762864 spida-0.2/spida/
--rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2/spida/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.781863 spida-0.2/spida/data/
--rw-rw-rw-   0        0        0        2 2023-05-20 19:45:58.000000 spida-0.2/spida/data/config.json
--rw-rw-rw-   0        0        0    16070 2023-05-20 19:42:14.000000 spida-0.2/spida/stable_diffusion.py
-drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.799271 spida-0.2/spida/utils/
--rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2/spida/utils/__init__.py
--rw-rw-rw-   0        0        0     5943 2023-05-19 20:05:30.000000 spida-0.2/spida/utils/img.py
--rw-rw-rw-   0        0        0     1042 2023-05-19 13:56:29.000000 spida-0.2/spida/utils/misc.py
--rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.2/spida/utils/net.py
-drwxrwxrwx   0        0        0        0 2023-05-20 19:51:20.781863 spida-0.2/spida.egg-info/
--rw-rw-rw-   0        0        0     6619 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      268 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-20 19:51:20.000000 spida-0.2/spida.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.786683 spida-0.2.1/
+-rw-rw-rw-   0        0        0     1081 2023-05-20 00:50:35.000000 spida-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0       30 2023-05-20 17:17:43.000000 spida-0.2.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     6621 2023-05-26 18:51:27.785675 spida-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6163 2023-05-20 06:34:04.000000 spida-0.2.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-26 18:51:27.786683 spida-0.2.1/setup.cfg
+-rw-rw-rw-   0        0        0      779 2023-05-26 18:50:27.000000 spida-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.744030 spida-0.2.1/spida/
+-rw-rw-rw-   0        0        0       59 2023-05-19 17:08:20.000000 spida-0.2.1/spida/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.776465 spida-0.2.1/spida/data/
+-rw-rw-rw-   0        0        0        2 2023-05-26 18:43:50.000000 spida-0.2.1/spida/data/config.json
+-rw-rw-rw-   0        0        0    16250 2023-05-26 18:34:56.000000 spida-0.2.1/spida/stable_diffusion.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.783149 spida-0.2.1/spida/utils/
+-rw-rw-rw-   0        0        0       30 2023-05-19 15:45:28.000000 spida-0.2.1/spida/utils/__init__.py
+-rw-rw-rw-   0        0        0     5943 2023-05-19 20:05:30.000000 spida-0.2.1/spida/utils/img.py
+-rw-rw-rw-   0        0        0     1042 2023-05-19 13:56:29.000000 spida-0.2.1/spida/utils/misc.py
+-rw-rw-rw-   0        0        0      861 2023-05-17 04:00:18.000000 spida-0.2.1/spida/utils/net.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:51:27.774335 spida-0.2.1/spida.egg-info/
+-rw-rw-rw-   0        0        0     6621 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      268 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 18:51:27.000000 spida-0.2.1/spida.egg-info/top_level.txt
```

### Comparing `spida-0.2/LICENSE` & `spida-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spida-0.2/PKG-INFO` & `spida-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.2
+Version: 0.2.1
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

### Comparing `spida-0.2/README.md` & `spida-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spida-0.2/setup.py` & `spida-0.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("requirements.txt") as f:
     required_packages = f.read().splitlines()
 
 setup(
     name="spida",
-    version="0.2",
+    version="0.2.1",
     packages=find_packages(),
     include_package_data=True,
     license="MIT",
     description="A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     author="h2see",
```

### Comparing `spida-0.2/spida/stable_diffusion.py` & `spida-0.2.1/spida/stable_diffusion.py`

 * *Files 6% similar despite different names*

```diff
@@ -207,17 +207,18 @@
         json=payload,
         fail_action=start,
         fail_message=config["fail_message"],
     )
     r = response.json()
     if verbose:
         pprint.pprint(r["parameters"])
-    size = (len(r["images"]), shape[0], shape[1], 3)
+    dsts_b64strs = r["images"]
+    size = (len(dsts_b64strs), shape[0], shape[1], 3)
     dsts = np.empty(shape=size, dtype=np.uint8)
-    for i, v in enumerate(r["images"]):
+    for i, v in enumerate(dsts_b64strs):
         dsts[i] = utils.img.b64str2img(v)
     return dsts
 
 
 def annotate(
     imgs: np.ndarray,
     annotator: str = "depth",
@@ -263,16 +264,20 @@
     response = utils.net.post(
         url=f'{config["url"]}/controlnet/detect',
         json=payload,
         fail_action=start,
         fail_message=config["fail_message"],
     )
     r = response.json()
-    dsts = np.empty(shape=imgs.shape[:-1], dtype=imgs.dtype)
-    for i, v in enumerate(r["images"]):
+    dsts_b64strs = r["images"]
+    dst = utils.img.b64str2img(dsts_b64strs[0])
+    size = (len(dsts_b64strs), *dst.shape)
+    dsts = np.empty(shape=size, dtype=dst.dtype)
+    dsts[0] = dst
+    for i, v in enumerate(dsts_b64strs[1:], start=1):
         dsts[i] = utils.img.b64str2img(v)
     return dsts
 
 
 def cnet_settings(
     annotated_img: np.ndarray,
     annotator: str = "depth",
```

### Comparing `spida-0.2/spida/utils/img.py` & `spida-0.2.1/spida/utils/img.py`

 * *Files identical despite different names*

### Comparing `spida-0.2/spida/utils/misc.py` & `spida-0.2.1/spida/utils/misc.py`

 * *Files identical despite different names*

### Comparing `spida-0.2/spida/utils/net.py` & `spida-0.2.1/spida/utils/net.py`

 * *Files identical despite different names*

### Comparing `spida-0.2/spida.egg-info/PKG-INFO` & `spida-0.2.1/spida.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spida
-Version: 0.2
+Version: 0.2.1
 Summary: A Stable Diffusion API Wrapper for AUTOMATIC1111/stable-diffusion-webui
 Home-page: https://github.com/h2see/spida
 Author: h2see
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
```

