# Comparing `tmp/MicroLIA-2.2.3.tar.gz` & `tmp/MicroLIA-2.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MicroLIA-2.2.3.tar", last modified: Fri May 26 00:13:40 2023, max compression
+gzip compressed data, was "MicroLIA-2.2.5.tar", last modified: Fri May 26 00:33:37 2023, max compression
```

## Comparing `MicroLIA-2.2.3.tar` & `MicroLIA-2.2.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:13:40.944091 MicroLIA-2.2.3/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2022-10-18 03:09:36.000000 MicroLIA-2.2.3/LICENSE.txt
--rw-r--r--   0 daniel     (501) staff       (20)       24 2023-05-22 20:39:52.000000 MicroLIA-2.2.3/MANIFEST.in
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:13:40.899679 MicroLIA-2.2.3/MicroLIA/
--rwxr-xr-x   0 daniel     (501) staff       (20)      365 2022-08-12 15:04:07.000000 MicroLIA-2.2.3/MicroLIA/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)   172657 2023-04-16 16:18:23.000000 MicroLIA-2.2.3/MicroLIA/cnn_model.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:13:40.933572 MicroLIA-2.2.3/MicroLIA/data/
--rwxr-xr-x   0 daniel     (501) staff       (20)  1384833 2022-07-17 06:13:15.000000 MicroLIA-2.2.3/MicroLIA/data/Miras_vo.xml
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:13:40.942226 MicroLIA-2.2.3/MicroLIA/data/Sesar2010/
--rw-r--r--   0 daniel     (501) staff       (20)   172713 2023-05-22 18:52:51.000000 MicroLIA-2.2.3/MicroLIA/data/Sesar2010/RRLyr_ugriz_templates.tar.gz
--rwxr-xr-x   0 daniel     (501) staff       (20)      365 2023-05-26 00:06:44.000000 MicroLIA-2.2.3/MicroLIA/data/Sesar2010/__init__.py
--rwxr-xr-x   0 daniel     (501) staff       (20)      365 2023-05-26 00:06:30.000000 MicroLIA-2.2.3/MicroLIA/data/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    36126 2023-04-14 06:02:09.000000 MicroLIA-2.2.3/MicroLIA/data_augmentation.py
--rw-r--r--   0 daniel     (501) staff       (20)    12888 2023-04-14 06:05:32.000000 MicroLIA-2.2.3/MicroLIA/data_processing.py
--rw-r--r--   0 daniel     (501) staff       (20)    54677 2023-04-14 06:20:00.000000 MicroLIA-2.2.3/MicroLIA/ensemble_model.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     5250 2023-03-30 05:00:56.000000 MicroLIA-2.2.3/MicroLIA/extract_features.py
--rwxr-xr-x   0 daniel     (501) staff       (20)   117151 2023-03-30 03:46:20.000000 MicroLIA-2.2.3/MicroLIA/features.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     2719 2023-03-19 23:16:44.000000 MicroLIA-2.2.3/MicroLIA/noise_models.py
--rw-r--r--   0 daniel     (501) staff       (20)   130007 2023-04-14 05:58:12.000000 MicroLIA-2.2.3/MicroLIA/optimization.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     4419 2023-02-26 05:00:18.000000 MicroLIA-2.2.3/MicroLIA/quality_check.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    19266 2023-05-25 23:47:31.000000 MicroLIA-2.2.3/MicroLIA/simulate.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    25956 2023-05-22 21:13:10.000000 MicroLIA-2.2.3/MicroLIA/training_set.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:13:40.912284 MicroLIA-2.2.3/MicroLIA.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-26 00:13:40.000000 MicroLIA-2.2.3/MicroLIA.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      658 2023-05-26 00:13:40.000000 MicroLIA-2.2.3/MicroLIA.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-26 00:13:40.000000 MicroLIA-2.2.3/MicroLIA.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)      193 2023-05-26 00:13:40.000000 MicroLIA-2.2.3/MicroLIA.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        9 2023-05-26 00:13:40.000000 MicroLIA-2.2.3/MicroLIA.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-26 00:13:40.943505 MicroLIA-2.2.3/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)     2641 2022-10-18 03:09:36.000000 MicroLIA-2.2.3/README.md
--rw-r--r--   0 daniel     (501) staff       (20)      456 2023-05-22 20:31:54.000000 MicroLIA-2.2.3/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-26 00:13:40.944293 MicroLIA-2.2.3/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)     1201 2023-05-26 00:11:29.000000 MicroLIA-2.2.3/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:33:37.678797 MicroLIA-2.2.5/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2022-10-18 03:09:36.000000 MicroLIA-2.2.5/LICENSE.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       24 2023-05-22 20:39:52.000000 MicroLIA-2.2.5/MANIFEST.in
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:33:37.655200 MicroLIA-2.2.5/MicroLIA/
+-rwxr-xr-x   0 daniel     (501) staff       (20)      365 2022-08-12 15:04:07.000000 MicroLIA-2.2.5/MicroLIA/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)   172657 2023-04-16 16:18:23.000000 MicroLIA-2.2.5/MicroLIA/cnn_model.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:33:37.671787 MicroLIA-2.2.5/MicroLIA/data/
+-rwxr-xr-x   0 daniel     (501) staff       (20)  1384833 2022-07-17 06:13:15.000000 MicroLIA-2.2.5/MicroLIA/data/Miras_vo.xml
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:33:37.676650 MicroLIA-2.2.5/MicroLIA/data/Sesar2010/
+-rw-r--r--   0 daniel     (501) staff       (20)   172713 2023-05-22 18:52:51.000000 MicroLIA-2.2.5/MicroLIA/data/Sesar2010/RRLyr_ugriz_templates.tar.gz
+-rwxr-xr-x   0 daniel     (501) staff       (20)      365 2023-05-26 00:06:44.000000 MicroLIA-2.2.5/MicroLIA/data/Sesar2010/__init__.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)      365 2023-05-26 00:06:30.000000 MicroLIA-2.2.5/MicroLIA/data/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    36126 2023-04-14 06:02:09.000000 MicroLIA-2.2.5/MicroLIA/data_augmentation.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12888 2023-04-14 06:05:32.000000 MicroLIA-2.2.5/MicroLIA/data_processing.py
+-rw-r--r--   0 daniel     (501) staff       (20)    54677 2023-04-14 06:20:00.000000 MicroLIA-2.2.5/MicroLIA/ensemble_model.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     5250 2023-03-30 05:00:56.000000 MicroLIA-2.2.5/MicroLIA/extract_features.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)   117151 2023-03-30 03:46:20.000000 MicroLIA-2.2.5/MicroLIA/features.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     2719 2023-03-19 23:16:44.000000 MicroLIA-2.2.5/MicroLIA/noise_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)   130007 2023-04-14 05:58:12.000000 MicroLIA-2.2.5/MicroLIA/optimization.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     4419 2023-02-26 05:00:18.000000 MicroLIA-2.2.5/MicroLIA/quality_check.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    19252 2023-05-26 00:29:59.000000 MicroLIA-2.2.5/MicroLIA/simulate.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    25956 2023-05-22 21:13:10.000000 MicroLIA-2.2.5/MicroLIA/training_set.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-26 00:33:37.661983 MicroLIA-2.2.5/MicroLIA.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-26 00:33:37.000000 MicroLIA-2.2.5/MicroLIA.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      658 2023-05-26 00:33:37.000000 MicroLIA-2.2.5/MicroLIA.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-26 00:33:37.000000 MicroLIA-2.2.5/MicroLIA.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      193 2023-05-26 00:33:37.000000 MicroLIA-2.2.5/MicroLIA.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        9 2023-05-26 00:33:37.000000 MicroLIA-2.2.5/MicroLIA.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-26 00:33:37.678102 MicroLIA-2.2.5/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)     2641 2022-10-18 03:09:36.000000 MicroLIA-2.2.5/README.md
+-rw-r--r--   0 daniel     (501) staff       (20)      456 2023-05-22 20:31:54.000000 MicroLIA-2.2.5/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-26 00:33:37.678988 MicroLIA-2.2.5/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1201 2023-05-26 00:30:26.000000 MicroLIA-2.2.5/setup.py
```

### Comparing `MicroLIA-2.2.3/LICENSE.txt` & `MicroLIA-2.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/cnn_model.py` & `MicroLIA-2.2.5/MicroLIA/cnn_model.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/data/Miras_vo.xml` & `MicroLIA-2.2.5/MicroLIA/data/Miras_vo.xml`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/data/Sesar2010/RRLyr_ugriz_templates.tar.gz` & `MicroLIA-2.2.5/MicroLIA/data/Sesar2010/RRLyr_ugriz_templates.tar.gz`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/data_augmentation.py` & `MicroLIA-2.2.5/MicroLIA/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/data_processing.py` & `MicroLIA-2.2.5/MicroLIA/data_processing.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/ensemble_model.py` & `MicroLIA-2.2.5/MicroLIA/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/extract_features.py` & `MicroLIA-2.2.5/MicroLIA/extract_features.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/features.py` & `MicroLIA-2.2.5/MicroLIA/features.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/noise_models.py` & `MicroLIA-2.2.5/MicroLIA/noise_models.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/optimization.py` & `MicroLIA-2.2.5/MicroLIA/optimization.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/quality_check.py` & `MicroLIA-2.2.5/MicroLIA/quality_check.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA/simulate.py` & `MicroLIA-2.2.5/MicroLIA/simulate.py`

 * *Files 1% similar despite different names*

```diff
@@ -222,30 +222,30 @@
         Baseline at which to simulate the lightcurve.
     bailey : int, optional 
         The type of variable to simulate. A bailey
         value of 1 simulaes RR Lyrae type ab, a value
         of 2 simulates RR Lyrae type c, and a value of 
         3 simulates a Cepheid variable period, but note the amplitude
         is still derived from the RRLyrae template. If not provided
-        it defaults to a random choice between the 1 and 2. 
+        it defaults to a random choice between 1 and 2. 
 
     Returns
     -------
     mag : array
         Simulated magnitudes given the timestamps.
     amplitude : float
         Amplitude of the signal in mag. 
     period : float
         Period of the signal in days.
     """
 
     if bailey is None: 
         bailey = np.random.randint(1,3) #Removing Bailey=3 option
-    if bailey < 0 or bailey > 2:
-        raise RuntimeError("Bailey out of range, must be between 1 and 2.")
+    if bailey < 0 or bailey > 3:
+        raise RuntimeError("Bailey out of range, must be between 1 and 3.")
 
     if bailey == 1:
         period = np.random.normal(0.6, 0.15)
     elif bailey == 2:
         period = np.random.normal(0.33, 0.1)
     elif bailey == 3:
         period = np.random.lognormal(0., 0.2)
@@ -548,13 +548,13 @@
         None
 
     Returns:
         data_path (str): Path to the data directory.
     """
 
     resource_package = __name__
-    resource_path = 'data/Sesar2010'
+    resource_path = 'data'
     data_path = pkg_resources.resource_filename(resource_package, resource_path)
     
     return data_path
```

### Comparing `MicroLIA-2.2.3/MicroLIA/training_set.py` & `MicroLIA-2.2.5/MicroLIA/training_set.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/MicroLIA.egg-info/PKG-INFO` & `MicroLIA-2.2.5/MicroLIA.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicroLIA
-Version: 2.2.3
+Version: 2.2.5
 Summary: Machine learning classifier for microlensing
 Home-page: https://github.com/Professor-G/MicroLIA
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `MicroLIA-2.2.3/MicroLIA.egg-info/SOURCES.txt` & `MicroLIA-2.2.5/MicroLIA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/PKG-INFO` & `MicroLIA-2.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicroLIA
-Version: 2.2.3
+Version: 2.2.5
 Summary: Machine learning classifier for microlensing
 Home-page: https://github.com/Professor-G/MicroLIA
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `MicroLIA-2.2.3/README.md` & `MicroLIA-2.2.5/README.md`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.3/setup.py` & `MicroLIA-2.2.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 
 setup(
     name="MicroLIA",
-    version="2.2.3",
+    version="2.2.5",
     author="Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="Machine learning classifier for microlensing",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/MicroLIA",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
```

