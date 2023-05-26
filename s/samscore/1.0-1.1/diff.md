# Comparing `tmp/samscore-1.0.tar.gz` & `tmp/samscore-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "samscore-1.0.tar", last modified: Fri May 26 15:57:46 2023, max compression
+gzip compressed data, was "samscore-1.1.tar", last modified: Fri May 26 16:35:37 2023, max compression
```

## Comparing `samscore-1.0.tar` & `samscore-1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:46.584750 samscore-1.0/
--rw-rw-rw-   0        0        0     1357 2021-10-01 16:16:03.000000 samscore-1.0/LICENSE
--rw-rw-rw-   0        0        0     2160 2023-05-26 15:57:46.584750 samscore-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1608 2023-05-26 15:56:37.000000 samscore-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:46.500051 samscore-1.0/data/
--rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.0/data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:46.500051 samscore-1.0/data/dataset/
--rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.0/data/dataset/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:46.500051 samscore-1.0/samscore/
--rw-rw-rw-   0        0        0     3725 2023-05-24 20:49:46.000000 samscore-1.0/samscore/__init__.py
--rw-rw-rw-   0        0        0     7879 2023-05-26 15:00:21.000000 samscore-1.0/samscore/samscore.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:46.515668 samscore-1.0/samscore.egg-info/
--rw-rw-rw-   0        0        0     2160 2023-05-26 15:57:45.000000 samscore-1.0/samscore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      331 2023-05-26 15:57:46.000000 samscore-1.0/samscore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 15:57:45.000000 samscore-1.0/samscore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       92 2023-05-26 15:57:45.000000 samscore-1.0/samscore.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-26 15:57:45.000000 samscore-1.0/samscore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 15:57:46.584750 samscore-1.0/setup.cfg
--rw-rw-rw-   0        0        0      831 2023-05-23 19:59:05.000000 samscore-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 15:57:46.584750 samscore-1.0/util/
--rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.0/util/__init__.py
--rw-rw-rw-   0        0        0     2023 2021-10-01 16:16:03.000000 samscore-1.0/util/html.py
--rw-rw-rw-   0        0        0     1433 2021-10-01 16:16:03.000000 samscore-1.0/util/util.py
--rw-rw-rw-   0        0        0     8568 2021-10-01 16:16:03.000000 samscore-1.0/util/visualizer.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:35:37.436278 samscore-1.1/
+-rw-rw-rw-   0        0        0     1357 2021-10-01 16:16:03.000000 samscore-1.1/LICENSE
+-rw-rw-rw-   0        0        0     2118 2023-05-26 16:35:37.436278 samscore-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1608 2023-05-26 15:56:37.000000 samscore-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 16:35:37.405043 samscore-1.1/data/
+-rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.1/data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:35:37.405043 samscore-1.1/data/dataset/
+-rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.1/data/dataset/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:35:37.420653 samscore-1.1/samscore/
+-rw-rw-rw-   0        0        0     3725 2023-05-24 20:49:46.000000 samscore-1.1/samscore/__init__.py
+-rw-rw-rw-   0        0        0     7937 2023-05-26 16:33:37.000000 samscore-1.1/samscore/samscore.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:35:37.420653 samscore-1.1/samscore.egg-info/
+-rw-rw-rw-   0        0        0     2118 2023-05-26 16:35:36.000000 samscore-1.1/samscore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      331 2023-05-26 16:35:37.000000 samscore-1.1/samscore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 16:35:36.000000 samscore-1.1/samscore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-05-26 16:35:36.000000 samscore-1.1/samscore.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-26 16:35:37.000000 samscore-1.1/samscore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 16:35:37.436278 samscore-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-26 16:34:25.000000 samscore-1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 16:35:37.436278 samscore-1.1/util/
+-rw-rw-rw-   0        0        0        0 2021-10-01 16:16:03.000000 samscore-1.1/util/__init__.py
+-rw-rw-rw-   0        0        0     2023 2021-10-01 16:16:03.000000 samscore-1.1/util/html.py
+-rw-rw-rw-   0        0        0     1433 2021-10-01 16:16:03.000000 samscore-1.1/util/util.py
+-rw-rw-rw-   0        0        0     8568 2021-10-01 16:16:03.000000 samscore-1.1/util/visualizer.py
```

### Comparing `samscore-1.0/LICENSE` & `samscore-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `samscore-1.0/PKG-INFO` & `samscore-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: samscore
-Version: 1.0
+Version: 1.1
 Summary: SAMScore Similarity Metric
 Home-page: https://github.com/Kent0n-Li/SAMScore
 Author: Yunxiang Li
 Author-email: yunxiang.li@utsouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: dev
 License-File: LICENSE
 
 
 ## SAMScore: A Semantic Structural Similarity Metric for Image Translation Evaluation
 
 [Yunxiang Li](https://www.yunxiangli.top/), Meixu Chen, Wenxuan Yang, Kai Wang, [Jun Ma](https://scholar.google.com/citations?hl=zh-CN&user=bW1UV4IAAAAJ), [Alan C. Bovik](https://www.ece.utexas.edu/people/faculty/alan-bovik), [You Zhang](https://profiles.utsouthwestern.edu/profile/161901/you-zhang.html).
```

### Comparing `samscore-1.0/README.md` & `samscore-1.1/README.md`

 * *Files identical despite different names*

### Comparing `samscore-1.0/samscore/__init__.py` & `samscore-1.1/samscore/__init__.py`

 * *Files identical despite different names*

### Comparing `samscore-1.0/samscore/samscore.py` & `samscore-1.1/samscore/samscore.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,17 @@
             elif model_type == "vit_h":
                 online_model_weight_name = online_vit_h_model_name
             else:
                 raise ValueError("model_type must be one of 'vit_l','vit_b','vit_h'")
             
         # to download the model weights from online link
         if model_weight_path is None:
-            model_weight_path = download_model(url = download_url,model_name = online_model_weight_name, destination= os.path.join("samscore","weights",online_model_weight_name))
+            save_path = "weights"
+            os.makedirs(save_path)
+            model_weight_path = download_model(url = download_url,model_name = online_model_weight_name, destination= os.path.join(save_path,online_model_weight_name))
 
                                                
 
         self.version = version
         self.model_type = model_type
         self.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         self.sam = sam_model_registry[self.model_type](checkpoint=model_weight_path)
```

### Comparing `samscore-1.0/samscore.egg-info/PKG-INFO` & `samscore-1.1/samscore.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 Metadata-Version: 2.1
 Name: samscore
-Version: 1.0
+Version: 1.1
 Summary: SAMScore Similarity Metric
 Home-page: https://github.com/Kent0n-Li/SAMScore
 Author: Yunxiang Li
 Author-email: yunxiang.li@utsouthwestern.edu
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
-Provides-Extra: all
-Provides-Extra: dev
 License-File: LICENSE
 
 
 ## SAMScore: A Semantic Structural Similarity Metric for Image Translation Evaluation
 
 [Yunxiang Li](https://www.yunxiangli.top/), Meixu Chen, Wenxuan Yang, Kai Wang, [Jun Ma](https://scholar.google.com/citations?hl=zh-CN&user=bW1UV4IAAAAJ), [Alan C. Bovik](https://www.ece.utexas.edu/people/faculty/alan-bovik), [You Zhang](https://profiles.utsouthwestern.edu/profile/161901/you-zhang.html).
```

### Comparing `samscore-1.0/setup.py` & `samscore-1.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 import setuptools
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setuptools.setup(
      name='samscore',
-     version='1.0',
+     version='1.1',
      author="Yunxiang Li",
      author_email="yunxiang.li@utsouthwestern.edu",
      description="SAMScore Similarity Metric",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/Kent0n-Li/SAMScore",
      packages=find_packages(),
-    extras_require={
-        "all": ["matplotlib", "pycocotools", "opencv-python", "onnx", "onnxruntime"],
-        "dev": ["flake8", "isort", "black", "mypy"],
-    },
+    install_requires=[
+        "segment_anything"
+        "torch>=1.0.0",
+        "numpy",
+        "requests",
+        "tqdm>=4.31.1",
+        "matplotlib",
+        "packaging>=20.9",
+    ],
     classifiers=[
          "Programming Language :: Python :: 3",
          "License :: OSI Approved :: BSD License",
          "Operating System :: OS Independent",
      ],
 )
```

### Comparing `samscore-1.0/util/html.py` & `samscore-1.1/util/html.py`

 * *Files identical despite different names*

### Comparing `samscore-1.0/util/util.py` & `samscore-1.1/util/util.py`

 * *Files identical despite different names*

### Comparing `samscore-1.0/util/visualizer.py` & `samscore-1.1/util/visualizer.py`

 * *Files identical despite different names*

