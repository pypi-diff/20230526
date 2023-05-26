# Comparing `tmp/jjuke-0.0.0.7.tar.gz` & `tmp/jjuke-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jjuke-0.0.0.7.tar", last modified: Fri May 26 18:21:51 2023, max compression
+gzip compressed data, was "dist/jjuke-0.0.0.8.tar", last modified: Fri May 26 18:57:30 2023, max compression
```

## Comparing `jjuke-0.0.0.7.tar` & `jjuke-0.0.0.8.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-11 12:21:10.000000 jjuke-0.0.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-26 18:21:15.000000 jjuke-0.0.0.7/jjuke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2958 2023-05-26 18:15:56.000000 jjuke-0.0.0.7/jjuke/logger.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 07:55:24.000000 jjuke-0.0.0.7/jjuke/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/metrics/
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 18:10:12.000000 jjuke-0.0.0.7/jjuke/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11621 2023-05-25 18:09:59.000000 jjuke-0.0.0.7/jjuke/metrics/evaluation_metrics.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-05-24 13:00:20.000000 jjuke-0.0.0.7/jjuke/metrics/pointcloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/module/
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/func.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/module/loss/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-05-24 07:55:26.000000 jjuke-0.0.0.7/jjuke/module/loss/focal.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/loss/utils.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-05-24 07:55:25.000000 jjuke-0.0.0.7/jjuke/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/pointcloud/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-26 07:37:06.000000 jjuke-0.0.0.7/jjuke/pointcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9538 2023-05-26 07:37:15.000000 jjuke-0.0.0.7/jjuke/pointcloud/transform.py
--rw-r--r--   0 root         (0) root         (0)    15015 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/sched.py
--rw-r--r--   0 root         (0) root         (0)    25202 2023-05-24 07:55:25.000000 jjuke-0.0.0.7/jjuke/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/utils/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/data.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/dist.py
--rw-r--r--   0 root         (0) root         (0)      457 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/ema.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/indexing.py
--rw-r--r--   0 root         (0) root         (0)     9553 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/interp1d.py
--rw-r--r--   0 root         (0) root         (0)      259 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     7370 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/optim.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)     9062 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/vis3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-26 18:21:11.000000 jjuke-0.0.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-11 12:21:10.000000 jjuke-0.0.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-26 18:56:46.000000 jjuke-0.0.0.8/jjuke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-05-26 18:56:26.000000 jjuke-0.0.0.8/jjuke/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 07:55:24.000000 jjuke-0.0.0.8/jjuke/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/metrics/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 18:10:12.000000 jjuke-0.0.0.8/jjuke/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11621 2023-05-25 18:09:59.000000 jjuke-0.0.0.8/jjuke/metrics/evaluation_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-05-24 13:00:20.000000 jjuke-0.0.0.8/jjuke/metrics/pointcloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/module/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/func.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/module/loss/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-05-24 07:55:26.000000 jjuke-0.0.0.8/jjuke/module/loss/focal.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/module/loss/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-05-24 07:55:25.000000 jjuke-0.0.0.8/jjuke/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/pointcloud/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-26 07:37:06.000000 jjuke-0.0.0.8/jjuke/pointcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9538 2023-05-26 07:37:15.000000 jjuke-0.0.0.8/jjuke/pointcloud/transform.py
+-rw-r--r--   0 root         (0) root         (0)    15015 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/sched.py
+-rw-r--r--   0 root         (0) root         (0)    25202 2023-05-24 07:55:25.000000 jjuke-0.0.0.8/jjuke/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke/utils/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/data.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/dist.py
+-rw-r--r--   0 root         (0) root         (0)      457 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/ema.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/indexing.py
+-rw-r--r--   0 root         (0) root         (0)     9553 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/interp1d.py
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     7370 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/optim.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9062 2023-05-11 12:09:23.000000 jjuke-0.0.0.8/jjuke/utils/vis3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/jjuke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 18:57:30.000000 jjuke-0.0.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-26 18:56:40.000000 jjuke-0.0.0.8/setup.py
```

### Comparing `jjuke-0.0.0.7/jjuke/logger.py` & `jjuke-0.0.0.8/jjuke/logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import reduce
 from pathlib import Path
 
 __all__ = ["CustomLogger", "timenow", "basicConfig", "getLogger"]
 
 
 class CustomLogger:
-    def __init__(self, log_dir, filemode="a", isTrain=True, use_color=True, lock=False):
+    def __init__(self, log_dir="./exps", filemode="a", isTrain=True, use_color=True, lock=False):
         self.log_dir = log_dir
         self.lock = lock
         
         os.makedirs(log_dir, exist_ok = True)
         
         if isTrain:
             filename = os.path.join(log_dir, "train_log.log")
```

### Comparing `jjuke-0.0.0.7/jjuke/main.py` & `jjuke-0.0.0.8/jjuke/main.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/metrics/evaluation_metrics.py` & `jjuke-0.0.0.8/jjuke/metrics/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/metrics/pointcloud.py` & `jjuke-0.0.0.8/jjuke/metrics/pointcloud.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/module/func.py` & `jjuke-0.0.0.8/jjuke/module/func.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/module/init.py` & `jjuke-0.0.0.8/jjuke/module/init.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/module/loss/focal.py` & `jjuke-0.0.0.8/jjuke/module/loss/focal.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/options.py` & `jjuke-0.0.0.8/jjuke/options.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/pointcloud/transform.py` & `jjuke-0.0.0.8/jjuke/pointcloud/transform.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/sched.py` & `jjuke-0.0.0.8/jjuke/sched.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/trainer.py` & `jjuke-0.0.0.8/jjuke/trainer.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/utils/data.py` & `jjuke-0.0.0.8/jjuke/utils/data.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/utils/dist.py` & `jjuke-0.0.0.8/jjuke/utils/dist.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/utils/indexing.py` & `jjuke-0.0.0.8/jjuke/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/utils/interp1d.py` & `jjuke-0.0.0.8/jjuke/utils/interp1d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/utils/optim.py` & `jjuke-0.0.0.8/jjuke/utils/optim.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/utils/utils.py` & `jjuke-0.0.0.8/jjuke/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke/utils/vis3d.py` & `jjuke-0.0.0.8/jjuke/utils/vis3d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/jjuke.egg-info/SOURCES.txt` & `jjuke-0.0.0.8/jjuke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.7/setup.py` & `jjuke-0.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="jjuke",
-    version="0.0.0.7",
+    version="0.0.0.8",
     description="utilities for AI models with Pytorch by JJukE",
     author="JJukE",
     author_email="psj9156@gmail.com",
     url="https://github.com/JJukE/JJuk_E.git",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
```

