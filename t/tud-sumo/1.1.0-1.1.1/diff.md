# Comparing `tmp/tud_sumo-1.1.0.tar.gz` & `tmp/tud_sumo-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tud_sumo-1.1.0.tar", last modified: Fri May 26 14:31:09 2023, max compression
+gzip compressed data, was "tud_sumo-1.1.1.tar", last modified: Fri May 26 14:47:57 2023, max compression
```

## Comparing `tud_sumo-1.1.0.tar` & `tud_sumo-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:31:09.690202 tud_sumo-1.1.0/
--rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.1.0/.gitattributes
--rw-r--r--   0 callumevans (50765939) 1653728465       35 2023-04-18 16:21:02.000000 tud_sumo-1.1.0/.gitignore
--rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.1.0/LICENSE
--rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-05-26 14:31:09.690087 tud_sumo-1.1.0/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      760 2023-04-18 15:15:39.000000 tud_sumo-1.1.0/README.md
--rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-05-26 14:28:13.000000 tud_sumo-1.1.0/pyproject.toml
--rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-05-26 14:31:09.690244 tud_sumo-1.1.0/setup.cfg
--rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.1.0/setup.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:31:09.688927 tud_sumo-1.1.0/tud_sumo/
--rw-r--r--   0 callumevans (50765939) 1653728465    24250 2023-05-26 14:26:41.000000 tud_sumo-1.1.0/tud_sumo/tud_sumo.py
-drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:31:09.689926 tud_sumo-1.1.0/tud_sumo.egg-info/
--rw-r--r--   0 callumevans (50765939) 1653728465     2367 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/PKG-INFO
--rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/SOURCES.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/dependency_links.txt
--rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/requires.txt
--rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-05-26 14:31:09.000000 tud_sumo-1.1.0/tud_sumo.egg-info/top_level.txt
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:47:57.433461 tud_sumo-1.1.1/
+-rw-r--r--   0 callumevans (50765939) 1653728465       66 2023-04-18 15:01:44.000000 tud_sumo-1.1.1/.gitattributes
+-rw-r--r--   0 callumevans (50765939) 1653728465       58 2023-05-26 14:42:14.000000 tud_sumo-1.1.1/.gitignore
+-rw-r--r--   0 callumevans (50765939) 1653728465     1069 2023-04-18 15:38:19.000000 tud_sumo-1.1.1/LICENSE
+-rw-r--r--   0 callumevans (50765939) 1653728465     2552 2023-05-26 14:47:57.433336 tud_sumo-1.1.1/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      945 2023-05-26 14:45:46.000000 tud_sumo-1.1.1/README.md
+-rw-r--r--   0 callumevans (50765939) 1653728465      528 2023-05-26 14:39:45.000000 tud_sumo-1.1.1/pyproject.toml
+-rw-r--r--   0 callumevans (50765939) 1653728465       38 2023-05-26 14:47:57.433500 tud_sumo-1.1.1/setup.cfg
+-rw-r--r--   0 callumevans (50765939) 1653728465       37 2023-04-18 15:52:01.000000 tud_sumo-1.1.1/setup.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:47:57.432304 tud_sumo-1.1.1/tud_sumo/
+-rw-r--r--   0 callumevans (50765939) 1653728465    15851 2023-05-26 14:39:21.000000 tud_sumo-1.1.1/tud_sumo/tud_sumo.py
+drwxr-xr-x   0 callumevans (50765939) 1653728465        0 2023-05-26 14:47:57.433166 tud_sumo-1.1.1/tud_sumo.egg-info/
+-rw-r--r--   0 callumevans (50765939) 1653728465     2552 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/PKG-INFO
+-rw-r--r--   0 callumevans (50765939) 1653728465      247 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/SOURCES.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        1 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/dependency_links.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465       22 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/requires.txt
+-rw-r--r--   0 callumevans (50765939) 1653728465        9 2023-05-26 14:47:57.000000 tud_sumo-1.1.1/tud_sumo.egg-info/top_level.txt
```

### Comparing `tud_sumo-1.1.0/LICENSE` & `tud_sumo-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tud_sumo-1.1.0/PKG-INFO` & `tud_sumo-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud_sumo
-Version: 1.1.0
+Version: 1.1.1
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,24 +30,26 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TU Delft SUMO Wrapper
 
-Python SUMO wrapper, using traci.
+Python SUMO wrapper, using traci, written for AIM Lab at TU Delft. Download with [pip](https://pypi.org/project/tud-sumo/) or from [GitHub](https://github.com/calluume/tud_sumo).
 
 ## Requirements 
 
 Required packages are: `tqdm`, `matplotlib` and `traci`.
 
 ## Usage example
 
 ```python    
-sim = Simulation()
+from tud_sumo import tud_sumo
+
+sim = tud_sumo.Simulation()
 
 # The phase dictionary is a dictionary containing the phases and times
 # for a given junction, eg:
 
 # {'junctionID': {'phases': ['gggggggggggggggrrrrrrrrrrrrrrrrr', ... ],   -> Phase light settings
 #                 'times':  [6.224149003633258, 2.775850996366742 ... ]}} -> Phase durations
 sim.set_phases(phase_dictionary)
```

### Comparing `tud_sumo-1.1.0/pyproject.toml` & `tud_sumo-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tud_sumo"
-version = "1.1.0"
+version = "1.1.1"
 description = "TU Delft SUMO wrapper"
 readme = "README.md"
 authors = [{ name = "Callum Evans", email = "c.evans@tudelft.nl" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `tud_sumo-1.1.0/tud_sumo.egg-info/PKG-INFO` & `tud_sumo-1.1.1/tud_sumo.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tud-sumo
-Version: 1.1.0
+Version: 1.1.1
 Summary: TU Delft SUMO wrapper
 Author-email: Callum Evans <c.evans@tudelft.nl>
 License: MIT License
         
         Copyright (c) 2023 Callum Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -30,24 +30,26 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # TU Delft SUMO Wrapper
 
-Python SUMO wrapper, using traci.
+Python SUMO wrapper, using traci, written for AIM Lab at TU Delft. Download with [pip](https://pypi.org/project/tud-sumo/) or from [GitHub](https://github.com/calluume/tud_sumo).
 
 ## Requirements 
 
 Required packages are: `tqdm`, `matplotlib` and `traci`.
 
 ## Usage example
 
 ```python    
-sim = Simulation()
+from tud_sumo import tud_sumo
+
+sim = tud_sumo.Simulation()
 
 # The phase dictionary is a dictionary containing the phases and times
 # for a given junction, eg:
 
 # {'junctionID': {'phases': ['gggggggggggggggrrrrrrrrrrrrrrrrr', ... ],   -> Phase light settings
 #                 'times':  [6.224149003633258, 2.775850996366742 ... ]}} -> Phase durations
 sim.set_phases(phase_dictionary)
```

