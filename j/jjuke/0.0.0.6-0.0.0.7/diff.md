# Comparing `tmp/jjuke-0.0.0.6.tar.gz` & `tmp/jjuke-0.0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jjuke-0.0.0.6.tar", last modified: Fri May 26 07:40:59 2023, max compression
+gzip compressed data, was "dist/jjuke-0.0.0.7.tar", last modified: Fri May 26 18:21:51 2023, max compression
```

## Comparing `jjuke-0.0.0.6.tar` & `jjuke-0.0.0.7.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      162 2023-05-11 12:21:10.000000 jjuke-0.0.0.6/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke/
--rw-r--r--   0 root         (0) root         (0)      121 2023-05-26 07:39:51.000000 jjuke-0.0.0.6/jjuke/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2931 2023-05-25 18:39:27.000000 jjuke-0.0.0.6/jjuke/logger.py
--rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 07:55:24.000000 jjuke-0.0.0.6/jjuke/main.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke/metrics/
--rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 18:10:12.000000 jjuke-0.0.0.6/jjuke/metrics/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11621 2023-05-25 18:09:59.000000 jjuke-0.0.0.6/jjuke/metrics/evaluation_metrics.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-05-24 13:00:20.000000 jjuke-0.0.0.6/jjuke/metrics/pointcloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke/module/
--rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/module/__init__.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/module/func.py
--rw-r--r--   0 root         (0) root         (0)      736 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/module/init.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke/module/loss/
--rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/module/loss/__init__.py
--rw-r--r--   0 root         (0) root         (0)      875 2023-05-24 07:55:26.000000 jjuke-0.0.0.6/jjuke/module/loss/focal.py
--rw-r--r--   0 root         (0) root         (0)      362 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/module/loss/utils.py
--rw-r--r--   0 root         (0) root         (0)     4318 2023-05-24 07:55:25.000000 jjuke-0.0.0.6/jjuke/options.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke/pointcloud/
--rw-r--r--   0 root         (0) root         (0)       23 2023-05-26 07:37:06.000000 jjuke-0.0.0.6/jjuke/pointcloud/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9538 2023-05-26 07:37:15.000000 jjuke-0.0.0.6/jjuke/pointcloud/transform.py
--rw-r--r--   0 root         (0) root         (0)    15015 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/sched.py
--rw-r--r--   0 root         (0) root         (0)    25202 2023-05-24 07:55:25.000000 jjuke-0.0.0.6/jjuke/trainer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke/utils/
--rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2493 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/data.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/dist.py
--rw-r--r--   0 root         (0) root         (0)      457 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/ema.py
--rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/indexing.py
--rw-r--r--   0 root         (0) root         (0)     9553 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/interp1d.py
--rw-r--r--   0 root         (0) root         (0)      259 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/io.py
--rw-r--r--   0 root         (0) root         (0)     7370 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/optim.py
--rw-r--r--   0 root         (0) root         (0)     5673 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/utils.py
--rw-r--r--   0 root         (0) root         (0)     9062 2023-05-11 12:09:23.000000 jjuke-0.0.0.6/jjuke/utils/vis3d.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke.egg-info/
--rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      831 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       42 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 09:08:15.000000 jjuke-0.0.0.6/jjuke.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       81 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/jjuke.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 07:40:59.000000 jjuke-0.0.0.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      622 2023-05-26 07:39:55.000000 jjuke-0.0.0.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      162 2023-05-11 12:21:10.000000 jjuke-0.0.0.7/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/
+-rw-r--r--   0 root         (0) root         (0)      121 2023-05-26 18:21:15.000000 jjuke-0.0.0.7/jjuke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2958 2023-05-26 18:15:56.000000 jjuke-0.0.0.7/jjuke/logger.py
+-rw-r--r--   0 root         (0) root         (0)     1666 2023-05-24 07:55:24.000000 jjuke-0.0.0.7/jjuke/main.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/metrics/
+-rw-r--r--   0 root         (0) root         (0)       67 2023-05-25 18:10:12.000000 jjuke-0.0.0.7/jjuke/metrics/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11621 2023-05-25 18:09:59.000000 jjuke-0.0.0.7/jjuke/metrics/evaluation_metrics.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-05-24 13:00:20.000000 jjuke-0.0.0.7/jjuke/metrics/pointcloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/module/
+-rw-r--r--   0 root         (0) root         (0)       31 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/func.py
+-rw-r--r--   0 root         (0) root         (0)      736 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/init.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/module/loss/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/loss/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      875 2023-05-24 07:55:26.000000 jjuke-0.0.0.7/jjuke/module/loss/focal.py
+-rw-r--r--   0 root         (0) root         (0)      362 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/module/loss/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4318 2023-05-24 07:55:25.000000 jjuke-0.0.0.7/jjuke/options.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/pointcloud/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-05-26 07:37:06.000000 jjuke-0.0.0.7/jjuke/pointcloud/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9538 2023-05-26 07:37:15.000000 jjuke-0.0.0.7/jjuke/pointcloud/transform.py
+-rw-r--r--   0 root         (0) root         (0)    15015 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/sched.py
+-rw-r--r--   0 root         (0) root         (0)    25202 2023-05-24 07:55:25.000000 jjuke-0.0.0.7/jjuke/trainer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke/utils/
+-rw-r--r--   0 root         (0) root         (0)       89 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2493 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/data.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/dist.py
+-rw-r--r--   0 root         (0) root         (0)      457 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/ema.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/indexing.py
+-rw-r--r--   0 root         (0) root         (0)     9553 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/interp1d.py
+-rw-r--r--   0 root         (0) root         (0)      259 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)     7370 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/optim.py
+-rw-r--r--   0 root         (0) root         (0)     5673 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/utils.py
+-rw-r--r--   0 root         (0) root         (0)     9062 2023-05-11 12:09:23.000000 jjuke-0.0.0.7/jjuke/utils/vis3d.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      221 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      831 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       81 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/jjuke.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 18:21:51.000000 jjuke-0.0.0.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      622 2023-05-26 18:21:11.000000 jjuke-0.0.0.7/setup.py
```

### Comparing `jjuke-0.0.0.6/jjuke/logger.py` & `jjuke-0.0.0.7/jjuke/logger.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,31 +3,33 @@
 from functools import reduce
 from pathlib import Path
 
 __all__ = ["CustomLogger", "timenow", "basicConfig", "getLogger"]
 
 
 class CustomLogger:
-    def __init__(self, exp_dir="./exp", exp_name="test", filemode="a", use_color=True, lock=False):
+    def __init__(self, log_dir, filemode="a", isTrain=True, use_color=True, lock=False):
+        self.log_dir = log_dir
         self.lock = lock
-
-        log_dir = os.path.join(exp_dir, exp_name)
+        
         os.makedirs(log_dir, exist_ok = True)
-        filename = os.path.join(log_dir, "train_log.log")
+        
+        if isTrain:
+            filename = os.path.join(log_dir, "train_log.log")
+        else:
+            filename = os.path.join(log_dir, "test_log.log")
 
         if not lock:
             filename = Path(filename)
             if filename.is_dir():
                 timestr = self._get_timestr().replace(" ", "_").replace(":", "-")
                 filename = filename / f"log_{timestr}.log"
             self.file = open(filename, filemode)
-
             self.use_color = use_color
 
-        self.info("Output directory: {}".format(exp_dir))
         self.info("Log path: {}".format(filename))
 
     def _get_timestr(self):
         n = datetime.now()
         return f"{n.year - 2000:02d}:{n.month:02d}:{n.day:02d} {n.hour:02d}:{n.minute:02d}:{n.second:02d}"
 
     def _write(self, msg, level):
```

### Comparing `jjuke-0.0.0.6/jjuke/main.py` & `jjuke-0.0.0.7/jjuke/main.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/metrics/evaluation_metrics.py` & `jjuke-0.0.0.7/jjuke/metrics/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/metrics/pointcloud.py` & `jjuke-0.0.0.7/jjuke/metrics/pointcloud.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/module/func.py` & `jjuke-0.0.0.7/jjuke/module/func.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/module/init.py` & `jjuke-0.0.0.7/jjuke/module/init.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/module/loss/focal.py` & `jjuke-0.0.0.7/jjuke/module/loss/focal.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/options.py` & `jjuke-0.0.0.7/jjuke/options.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/pointcloud/transform.py` & `jjuke-0.0.0.7/jjuke/pointcloud/transform.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/sched.py` & `jjuke-0.0.0.7/jjuke/sched.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/trainer.py` & `jjuke-0.0.0.7/jjuke/trainer.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/utils/data.py` & `jjuke-0.0.0.7/jjuke/utils/data.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/utils/dist.py` & `jjuke-0.0.0.7/jjuke/utils/dist.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/utils/indexing.py` & `jjuke-0.0.0.7/jjuke/utils/indexing.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/utils/interp1d.py` & `jjuke-0.0.0.7/jjuke/utils/interp1d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/utils/optim.py` & `jjuke-0.0.0.7/jjuke/utils/optim.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/utils/utils.py` & `jjuke-0.0.0.7/jjuke/utils/utils.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke/utils/vis3d.py` & `jjuke-0.0.0.7/jjuke/utils/vis3d.py`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/jjuke.egg-info/SOURCES.txt` & `jjuke-0.0.0.7/jjuke.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jjuke-0.0.0.6/setup.py` & `jjuke-0.0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name="jjuke",
-    version="0.0.0.6",
+    version="0.0.0.7",
     description="utilities for AI models with Pytorch by JJukE",
     author="JJukE",
     author_email="psj9156@gmail.com",
     url="https://github.com/JJukE/JJuk_E.git",
     packages=find_packages(),
     zip_safe=False,
     install_requires=[
```

