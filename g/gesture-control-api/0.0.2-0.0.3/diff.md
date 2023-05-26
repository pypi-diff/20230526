# Comparing `tmp/gesture-control-api-0.0.2.tar.gz` & `tmp/gesture-control-api-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gesture-control-api-0.0.2.tar", last modified: Fri May 26 00:12:22 2023, max compression
+gzip compressed data, was "gesture-control-api-0.0.3.tar", last modified: Fri May 26 00:33:18 2023, max compression
```

## Comparing `gesture-control-api-0.0.2.tar` & `gesture-control-api-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 00:12:22.656007 gesture-control-api-0.0.2/
--rw-rw-rw-   0        0        0      144 2023-05-26 00:12:22.654995 gesture-control-api-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-26 00:12:22.641329 gesture-control-api-0.0.2/gesture_control_api/
--rw-rw-rw-   0        0        0        0 2023-05-25 23:57:50.000000 gesture-control-api-0.0.2/gesture_control_api/__init__.py
--rw-rw-rw-   0        0        0    12758 2023-05-19 07:57:00.000000 gesture-control-api-0.0.2/gesture_control_api/cameracontrol.py
--rw-rw-rw-   0        0        0     3386 2023-05-18 16:25:38.000000 gesture-control-api-0.0.2/gesture_control_api/detector.py
--rw-rw-rw-   0        0        0     3475 2023-05-19 01:35:43.000000 gesture-control-api-0.0.2/gesture_control_api/gesturecontrolapi.py
--rw-rw-rw-   0        0        0     2075 2023-05-19 01:11:38.000000 gesture-control-api-0.0.2/gesture_control_api/gesturemodel.py
--rw-rw-rw-   0        0        0     1315 2023-05-11 19:36:02.000000 gesture-control-api-0.0.2/gesture_control_api/imaging.py
--rw-rw-rw-   0        0        0     6839 2023-05-19 01:26:47.000000 gesture-control-api-0.0.2/gesture_control_api/landmarking.py
-drwxrwxrwx   0        0        0        0 2023-05-26 00:12:22.653486 gesture-control-api-0.0.2/gesture_control_api.egg-info/
--rw-rw-rw-   0        0        0      144 2023-05-26 00:12:22.000000 gesture-control-api-0.0.2/gesture_control_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-05-26 00:12:22.000000 gesture-control-api-0.0.2/gesture_control_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 00:12:22.000000 gesture-control-api-0.0.2/gesture_control_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     1154 2023-05-26 00:12:22.000000 gesture-control-api-0.0.2/gesture_control_api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2023-05-26 00:12:22.000000 gesture-control-api-0.0.2/gesture_control_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 00:12:22.657196 gesture-control-api-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2166 2023-05-26 00:11:38.000000 gesture-control-api-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 00:33:18.364723 gesture-control-api-0.0.3/
+-rw-rw-rw-   0        0        0      144 2023-05-26 00:33:18.362686 gesture-control-api-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 00:33:18.348688 gesture-control-api-0.0.3/gesture_control_api/
+-rw-rw-rw-   0        0        0        0 2023-05-25 23:57:50.000000 gesture-control-api-0.0.3/gesture_control_api/__init__.py
+-rw-rw-rw-   0        0        0    12758 2023-05-19 07:57:00.000000 gesture-control-api-0.0.3/gesture_control_api/cameracontrol.py
+-rw-rw-rw-   0        0        0     3386 2023-05-18 16:25:38.000000 gesture-control-api-0.0.3/gesture_control_api/detector.py
+-rw-rw-rw-   0        0        0     3475 2023-05-19 01:35:43.000000 gesture-control-api-0.0.3/gesture_control_api/gesturecontrolapi.py
+-rw-rw-rw-   0        0        0     2027 2023-05-26 00:31:37.000000 gesture-control-api-0.0.3/gesture_control_api/gesturemodel.py
+-rw-rw-rw-   0        0        0     1315 2023-05-11 19:36:02.000000 gesture-control-api-0.0.3/gesture_control_api/imaging.py
+-rw-rw-rw-   0        0        0     6839 2023-05-19 01:26:47.000000 gesture-control-api-0.0.3/gesture_control_api/landmarking.py
+drwxrwxrwx   0        0        0        0 2023-05-26 00:33:18.359686 gesture-control-api-0.0.3/gesture_control_api.egg-info/
+-rw-rw-rw-   0        0        0      144 2023-05-26 00:33:18.000000 gesture-control-api-0.0.3/gesture_control_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      466 2023-05-26 00:33:18.000000 gesture-control-api-0.0.3/gesture_control_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 00:33:18.000000 gesture-control-api-0.0.3/gesture_control_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     1154 2023-05-26 00:33:18.000000 gesture-control-api-0.0.3/gesture_control_api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-05-26 00:33:18.000000 gesture-control-api-0.0.3/gesture_control_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 00:33:18.364723 gesture-control-api-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2292 2023-05-26 00:30:50.000000 gesture-control-api-0.0.3/setup.py
```

### Comparing `gesture-control-api-0.0.2/gesture_control_api/cameracontrol.py` & `gesture-control-api-0.0.3/gesture_control_api/cameracontrol.py`

 * *Files identical despite different names*

### Comparing `gesture-control-api-0.0.2/gesture_control_api/detector.py` & `gesture-control-api-0.0.3/gesture_control_api/detector.py`

 * *Files identical despite different names*

### Comparing `gesture-control-api-0.0.2/gesture_control_api/gesturecontrolapi.py` & `gesture-control-api-0.0.3/gesture_control_api/gesturecontrolapi.py`

 * *Files identical despite different names*

### Comparing `gesture-control-api-0.0.2/gesture_control_api/gesturemodel.py` & `gesture-control-api-0.0.3/gesture_control_api/gesturemodel.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     class GestureCategory(Enum):
         NEUTRAL = 0
         PINCH = 1
         POINT_WITH_INDEX_AND_MIDDLE = 2
         FIST = 3
         PINCH_CLOSED_HAND = 4
 
-    def __init__(self, path_to_model="machine_learning_models/robust_model_4.tflite"):
+    def __init__(self, path_to_model):
         self.detector = TfLiteDetector(path_to_model)
 
         self.memory = [self.GestureCategory.NEUTRAL.value] * 4
 
     def predict_gesture_from_landmarks(self, landmarks: Landmarks) -> GestureCategory:
         cat_idx = self.detector.detect_from_landmarks(landmarks)
```

### Comparing `gesture-control-api-0.0.2/gesture_control_api/imaging.py` & `gesture-control-api-0.0.3/gesture_control_api/imaging.py`

 * *Files identical despite different names*

### Comparing `gesture-control-api-0.0.2/gesture_control_api/landmarking.py` & `gesture-control-api-0.0.3/gesture_control_api/landmarking.py`

 * *Files identical despite different names*

### Comparing `gesture-control-api-0.0.2/gesture_control_api.egg-info/requires.txt` & `gesture-control-api-0.0.3/gesture_control_api.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `gesture-control-api-0.0.2/setup.py` & `gesture-control-api-0.0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gesture-control-api',
-    version='0.0.2',
+    version='0.0.3',
     author='Marcell Dancsó',
     description='Simple gesture control API for 3D software',
     packages=find_packages(),
+    package_data={
+        'gesture-control-api': ['gesture_control_api/*.tflite'],
+    },
+    include_package_data=True,
     install_requires=[
         'absl-py==1.4.0',
         'astunparse==1.6.3',
         'attrs==23.1.0',
         'cachetools==5.3.0',
         'certifi==2023.5.7',
         'cffi==1.15.1',
```

