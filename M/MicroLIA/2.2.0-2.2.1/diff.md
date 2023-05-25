# Comparing `tmp/MicroLIA-2.2.0.tar.gz` & `tmp/MicroLIA-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MicroLIA-2.2.0.tar", last modified: Mon May 22 22:02:21 2023, max compression
+gzip compressed data, was "MicroLIA-2.2.1.tar", last modified: Thu May 25 23:51:45 2023, max compression
```

## Comparing `MicroLIA-2.2.0.tar` & `MicroLIA-2.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 22:02:21.854395 MicroLIA-2.2.0/
--rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2022-10-18 03:09:36.000000 MicroLIA-2.2.0/LICENSE.txt
--rw-r--r--   0 daniel     (501) staff       (20)       24 2023-05-22 20:39:52.000000 MicroLIA-2.2.0/MANIFEST.in
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 22:02:21.838681 MicroLIA-2.2.0/MicroLIA/
--rwxr-xr-x   0 daniel     (501) staff       (20)      365 2022-08-12 15:04:07.000000 MicroLIA-2.2.0/MicroLIA/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)   172657 2023-04-16 16:18:23.000000 MicroLIA-2.2.0/MicroLIA/cnn_model.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 22:02:21.852569 MicroLIA-2.2.0/MicroLIA/data/
--rw-r--r--   0 daniel     (501) staff       (20)     6148 2023-05-22 20:44:02.000000 MicroLIA-2.2.0/MicroLIA/data/.DS_Store
--rwxr-xr-x   0 daniel     (501) staff       (20)  1384833 2022-07-17 06:13:15.000000 MicroLIA-2.2.0/MicroLIA/data/Miras_vo.xml
--rwxr-xr-x   0 daniel     (501) staff       (20)       26 2022-07-17 06:13:15.000000 MicroLIA-2.2.0/MicroLIA/data/__init__.py
--rw-r--r--   0 daniel     (501) staff       (20)    36126 2023-04-14 06:02:09.000000 MicroLIA-2.2.0/MicroLIA/data_augmentation.py
--rw-r--r--   0 daniel     (501) staff       (20)    12888 2023-04-14 06:05:32.000000 MicroLIA-2.2.0/MicroLIA/data_processing.py
--rw-r--r--   0 daniel     (501) staff       (20)    54677 2023-04-14 06:20:00.000000 MicroLIA-2.2.0/MicroLIA/ensemble_model.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     5250 2023-03-30 05:00:56.000000 MicroLIA-2.2.0/MicroLIA/extract_features.py
--rwxr-xr-x   0 daniel     (501) staff       (20)   117151 2023-03-30 03:46:20.000000 MicroLIA-2.2.0/MicroLIA/features.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     2719 2023-03-19 23:16:44.000000 MicroLIA-2.2.0/MicroLIA/noise_models.py
--rw-r--r--   0 daniel     (501) staff       (20)   130007 2023-04-14 05:58:12.000000 MicroLIA-2.2.0/MicroLIA/optimization.py
--rwxr-xr-x   0 daniel     (501) staff       (20)     4419 2023-02-26 05:00:18.000000 MicroLIA-2.2.0/MicroLIA/quality_check.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    20101 2023-05-22 20:37:04.000000 MicroLIA-2.2.0/MicroLIA/simulate.py
--rwxr-xr-x   0 daniel     (501) staff       (20)    25956 2023-05-22 21:13:10.000000 MicroLIA-2.2.0/MicroLIA/training_set.py
-drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-22 22:02:21.843628 MicroLIA-2.2.0/MicroLIA.egg-info/
--rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/PKG-INFO
--rw-r--r--   0 daniel     (501) staff       (20)      593 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/SOURCES.txt
--rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/dependency_links.txt
--rw-r--r--   0 daniel     (501) staff       (20)      193 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/requires.txt
--rw-r--r--   0 daniel     (501) staff       (20)        9 2023-05-22 22:02:21.000000 MicroLIA-2.2.0/MicroLIA.egg-info/top_level.txt
--rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-22 22:02:21.853793 MicroLIA-2.2.0/PKG-INFO
--rwxr-xr-x   0 daniel     (501) staff       (20)     2641 2022-10-18 03:09:36.000000 MicroLIA-2.2.0/README.md
--rw-r--r--   0 daniel     (501) staff       (20)      456 2023-05-22 20:31:54.000000 MicroLIA-2.2.0/pyproject.toml
--rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-22 22:02:21.854576 MicroLIA-2.2.0/setup.cfg
--rwxr-xr-x   0 daniel     (501) staff       (20)     1162 2023-05-22 22:00:17.000000 MicroLIA-2.2.0/setup.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-25 23:51:45.613452 MicroLIA-2.2.1/
+-rwxr-xr-x   0 daniel     (501) staff       (20)    35141 2022-10-18 03:09:36.000000 MicroLIA-2.2.1/LICENSE.txt
+-rw-r--r--   0 daniel     (501) staff       (20)       24 2023-05-22 20:39:52.000000 MicroLIA-2.2.1/MANIFEST.in
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-25 23:51:45.590921 MicroLIA-2.2.1/MicroLIA/
+-rwxr-xr-x   0 daniel     (501) staff       (20)      365 2022-08-12 15:04:07.000000 MicroLIA-2.2.1/MicroLIA/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)   172657 2023-04-16 16:18:23.000000 MicroLIA-2.2.1/MicroLIA/cnn_model.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-25 23:51:45.611038 MicroLIA-2.2.1/MicroLIA/data/
+-rw-r--r--   0 daniel     (501) staff       (20)     6148 2023-05-25 23:23:05.000000 MicroLIA-2.2.1/MicroLIA/data/.DS_Store
+-rwxr-xr-x   0 daniel     (501) staff       (20)  1384833 2022-07-17 06:13:15.000000 MicroLIA-2.2.1/MicroLIA/data/Miras_vo.xml
+-rwxr-xr-x   0 daniel     (501) staff       (20)       26 2022-07-17 06:13:15.000000 MicroLIA-2.2.1/MicroLIA/data/__init__.py
+-rw-r--r--   0 daniel     (501) staff       (20)    36126 2023-04-14 06:02:09.000000 MicroLIA-2.2.1/MicroLIA/data_augmentation.py
+-rw-r--r--   0 daniel     (501) staff       (20)    12888 2023-04-14 06:05:32.000000 MicroLIA-2.2.1/MicroLIA/data_processing.py
+-rw-r--r--   0 daniel     (501) staff       (20)    54677 2023-04-14 06:20:00.000000 MicroLIA-2.2.1/MicroLIA/ensemble_model.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     5250 2023-03-30 05:00:56.000000 MicroLIA-2.2.1/MicroLIA/extract_features.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)   117151 2023-03-30 03:46:20.000000 MicroLIA-2.2.1/MicroLIA/features.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     2719 2023-03-19 23:16:44.000000 MicroLIA-2.2.1/MicroLIA/noise_models.py
+-rw-r--r--   0 daniel     (501) staff       (20)   130007 2023-04-14 05:58:12.000000 MicroLIA-2.2.1/MicroLIA/optimization.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)     4419 2023-02-26 05:00:18.000000 MicroLIA-2.2.1/MicroLIA/quality_check.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    19266 2023-05-25 23:47:31.000000 MicroLIA-2.2.1/MicroLIA/simulate.py
+-rwxr-xr-x   0 daniel     (501) staff       (20)    25956 2023-05-22 21:13:10.000000 MicroLIA-2.2.1/MicroLIA/training_set.py
+drwxr-xr-x   0 daniel     (501) staff       (20)        0 2023-05-25 23:51:45.599599 MicroLIA-2.2.1/MicroLIA.egg-info/
+-rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-25 23:51:45.000000 MicroLIA-2.2.1/MicroLIA.egg-info/PKG-INFO
+-rw-r--r--   0 daniel     (501) staff       (20)      593 2023-05-25 23:51:45.000000 MicroLIA-2.2.1/MicroLIA.egg-info/SOURCES.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        1 2023-05-25 23:51:45.000000 MicroLIA-2.2.1/MicroLIA.egg-info/dependency_links.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      193 2023-05-25 23:51:45.000000 MicroLIA-2.2.1/MicroLIA.egg-info/requires.txt
+-rw-r--r--   0 daniel     (501) staff       (20)        9 2023-05-25 23:51:45.000000 MicroLIA-2.2.1/MicroLIA.egg-info/top_level.txt
+-rw-r--r--   0 daniel     (501) staff       (20)      572 2023-05-25 23:51:45.612748 MicroLIA-2.2.1/PKG-INFO
+-rwxr-xr-x   0 daniel     (501) staff       (20)     2641 2022-10-18 03:09:36.000000 MicroLIA-2.2.1/README.md
+-rw-r--r--   0 daniel     (501) staff       (20)      456 2023-05-22 20:31:54.000000 MicroLIA-2.2.1/pyproject.toml
+-rw-r--r--   0 daniel     (501) staff       (20)       38 2023-05-25 23:51:45.614144 MicroLIA-2.2.1/setup.cfg
+-rwxr-xr-x   0 daniel     (501) staff       (20)     1201 2023-05-25 23:41:38.000000 MicroLIA-2.2.1/setup.py
```

### Comparing `MicroLIA-2.2.0/LICENSE.txt` & `MicroLIA-2.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/cnn_model.py` & `MicroLIA-2.2.1/MicroLIA/cnn_model.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/data/.DS_Store` & `MicroLIA-2.2.1/MicroLIA/data/.DS_Store`

 * *Files 24% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 00000230: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
 00000240: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
 00000250: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
 00000260: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
 00000270: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
 00000280: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
 00000290: 6f77 5369 6465 6261 7208 0908 095f 1018  owSidebar...._..
-000002a0: 7b7b 3632 342c 2034 3237 7d2c 207b 3932  {{624, 427}, {92
+000002a0: 7b7b 3236 302c 2033 3239 7d2c 207b 3932  {{260, 329}, {92
 000002b0: 302c 2034 3336 7d7d 0908 1523 2f3b 525f  0, 436}}...#/;R_
 000002c0: 6b6c 6d6e 6f8a 0000 0000 0000 0101 0000  klmno...........
 000002d0: 0000 0000 000d 0000 0000 0000 0000 0000  ................
 000002e0: 0000 0000 008b 0000 0009 0053 0065 0073  ...........S.e.s
 000002f0: 0061 0072 0032 0030 0031 0030 7653 726e  .a.r.2.0.1.0vSrn
 00000300: 6c6f 6e67 0000 0001 0000 0000 0000 0000  long............
 00000310: 0000 0000 0000 0000 0000 0000 0000 0000  ................
```

### Comparing `MicroLIA-2.2.0/MicroLIA/data/Miras_vo.xml` & `MicroLIA-2.2.1/MicroLIA/data/Miras_vo.xml`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/data_augmentation.py` & `MicroLIA-2.2.1/MicroLIA/data_augmentation.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/data_processing.py` & `MicroLIA-2.2.1/MicroLIA/data_processing.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/ensemble_model.py` & `MicroLIA-2.2.1/MicroLIA/ensemble_model.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/extract_features.py` & `MicroLIA-2.2.1/MicroLIA/extract_features.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/features.py` & `MicroLIA-2.2.1/MicroLIA/features.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/noise_models.py` & `MicroLIA-2.2.1/MicroLIA/noise_models.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/optimization.py` & `MicroLIA-2.2.1/MicroLIA/optimization.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/quality_check.py` & `MicroLIA-2.2.1/MicroLIA/quality_check.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA/simulate.py` & `MicroLIA-2.2.1/MicroLIA/simulate.py`

 * *Files 7% similar despite different names*

```diff
@@ -220,31 +220,32 @@
         Times at which to simulate the lightcurve.
     baseline : float
         Baseline at which to simulate the lightcurve.
     bailey : int, optional 
         The type of variable to simulate. A bailey
         value of 1 simulaes RR Lyrae type ab, a value
         of 2 simulates RR Lyrae type c, and a value of 
-        3 simulates a Cepheid variable. If not provided
-        it defaults to a random choice between the three. 
+        3 simulates a Cepheid variable period, but note the amplitude
+        is still derived from the RRLyrae template. If not provided
+        it defaults to a random choice between the 1 and 2. 
 
     Returns
     -------
     mag : array
         Simulated magnitudes given the timestamps.
     amplitude : float
         Amplitude of the signal in mag. 
     period : float
         Period of the signal in days.
     """
 
-    if bailey is None:
-        bailey = np.random.randint(1,4)
-    if bailey < 0 or bailey > 3:
-        raise RuntimeError("Bailey out of range, must be between 1 and 3.")
+    if bailey is None: 
+        bailey = np.random.randint(1,3) #Removing Bailey=3 option
+    if bailey < 0 or bailey > 2:
+        raise RuntimeError("Bailey out of range, must be between 1 and 2.")
 
     if bailey == 1:
         period = np.random.normal(0.6, 0.15)
     elif bailey == 2:
         period = np.random.normal(0.33, 0.1)
     elif bailey == 3:
         period = np.random.lognormal(0., 0.2)
@@ -535,40 +536,25 @@
     len_miras = len(primary_period)
     rand_idx = np.random.randint(0,len_miras,1)
     amplitudes = [amplitude_pp[rand_idx], amplitude_sp[rand_idx], amplitude_tp[rand_idx]]
     periods = [primary_period[rand_idx], secondary_period[rand_idx], tertiary_period[rand_idx]]
 
     return amplitudes, periods
 
-def get_rrlyr_data_path(data_home=None):
+def get_rrlyr_data_path():
     """
-    This function retrieves the path to the data directory of the MicroLIA package.
-    If the `data_home` parameter is None, it attempts to locate the MicroLIA package and sets the data_home
-    to the default location inside the package. Otherwise, it uses the provided `data_home` path.
-    
-    The `data_home` path is expanded to the user's home directory if '~' is present.
-    If the directory does not already exist, it is created.
+    Retrieves the path to the RRLyrae template data directory within the MicroLIA package.
 
     Args:
-        data_home (str or None): Path to the data directory. If None, the default location inside the MicroLIA package is used.
+        None
 
     Returns:
-        data_home (str): Path to the data directory.
+        data_path (str): Path to the data directory.
     """
 
-    if data_home is None:
-        try:
-            spec = importlib.util.find_spec("MicroLIA")
-            if spec is None:
-                raise ValueError("MicroLIA package not found. Please run 'pip install MicroLIA'")
-            microlia_location = spec.origin
-            microlia_dir = os.path.dirname(microlia_location)
-            data_home = os.path.join(microlia_dir, "data")
-        except ImportError:
-            raise ValueError("MicroLIA package not found. Please run 'pip install MicroLIA'")
-
-    data_home = os.path.expanduser(data_home)
-    if not os.path.exists(data_home):
-        os.makedirs(data_home)
-
-    return data_home
+    resource_package = __name__
+    resource_path = 'data/Sesar2010'
+    data_path = pkg_resources.resource_filename(resource_package, resource_path)
+    
+    return data_path
 
+
```

### Comparing `MicroLIA-2.2.0/MicroLIA/training_set.py` & `MicroLIA-2.2.1/MicroLIA/training_set.py`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/MicroLIA.egg-info/PKG-INFO` & `MicroLIA-2.2.1/MicroLIA.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicroLIA
-Version: 2.2.0
+Version: 2.2.1
 Summary: Machine learning classifier for microlensing
 Home-page: https://github.com/Professor-G/MicroLIA
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `MicroLIA-2.2.0/MicroLIA.egg-info/SOURCES.txt` & `MicroLIA-2.2.1/MicroLIA.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/PKG-INFO` & `MicroLIA-2.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MicroLIA
-Version: 2.2.0
+Version: 2.2.1
 Summary: Machine learning classifier for microlensing
 Home-page: https://github.com/Professor-G/MicroLIA
 Author: Daniel Godines
 Author-email: danielgodinez123@gmail.com
 License: GPL-3.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `MicroLIA-2.2.0/README.md` & `MicroLIA-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `MicroLIA-2.2.0/setup.py` & `MicroLIA-2.2.1/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 @author: danielgodinez
 """
 from setuptools import setup, find_packages, Extension
 
 
 setup(
     name="MicroLIA",
-    version="2.2.0",
+    version="2.2.1",
     author="Daniel Godines",
     author_email="danielgodinez123@gmail.com",
     description="Machine learning classifier for microlensing",
     license='GPL-3.0',
     url = "https://github.com/Professor-G/MicroLIA",
     classifiers=[
 		'Development Status :: 5 - Production/Stable',
@@ -26,11 +26,11 @@
     install_requires = ['numpy','scikit-learn', 'scikit-optimize', 'astropy','scipy','peakutils',
         'progress', 'matplotlib', 'optuna', 'boruta', 'BorutaShap', 'xgboost', 'scikit-plot',
         'tensorflow', 'pandas', 'dill', 'opencv-python', 'imbalanced-learn', 'gatspy', 'astroML'],
     python_requires='>=3.7,<4',
     include_package_data=True,
     test_suite="nose.collector",
     package_data={
-    '': ['Miras_vo.xml'],
-},
-
+        '': ['Miras_vo.xml'],
+        'data': ['Sesar2010/*']
+    },
 )
```

