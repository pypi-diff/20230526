# Comparing `tmp/mapel-core-2.0.3.dev7.tar.gz` & `tmp/mapel-core-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-core-2.0.3.dev7.tar", last modified: Wed May 24 17:34:47 2023, max compression
+gzip compressed data, was "mapel-core-2.0.4.tar", last modified: Fri May 26 10:40:01 2023, max compression
```

## Comparing `mapel-core-2.0.3.dev7.tar` & `mapel-core-2.0.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.060550 mapel-core-2.0.3.dev7/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-24 17:34:47.060550 mapel-core-2.0.3.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 17:34:47.060550 mapel-core-2.0.3.dev7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.052550 mapel-core-2.0.3.dev7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.052550 mapel-core-2.0.3.dev7/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.056550 mapel-core-2.0.3.dev7/src/mapel/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.056550 mapel-core-2.0.3.dev7/src/mapel/core/embedding/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/initial_positions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.056550 mapel-core-2.0.3.dev7/src/mapel/core/embedding/kamada_kawai/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/kamada_kawai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/kamada_kawai/energy_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.056550 mapel-core-2.0.3.dev7/src/mapel/core/embedding/simulated_annealing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/simulated_annealing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.056550 mapel-core-2.0.3.dev7/src/mapel/core/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/features/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/features/distortion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/features/monotonicity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/features/stability.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/features_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/glossary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/inner_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/matchings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.056550 mapel-core-2.0.3.dev7/src/mapel/core/objects/
--rw-r--r--   0 runner    (1001) docker     (123)    24209 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/objects/Experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/objects/Family.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/objects/Instance.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.056550 mapel-core-2.0.3.dev7/src/mapel/core/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/persistence/experiment_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/persistence/experiment_imports.py
--rw-r--r--   0 runner    (1001) docker     (123)    62604 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/printing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-24 17:34:28.000000 mapel-core-2.0.3.dev7/src/mapel/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 17:34:47.056550 mapel-core-2.0.3.dev7/src/mapel_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-24 17:34:47.000000 mapel-core-2.0.3.dev7/src/mapel_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-24 17:34:47.000000 mapel-core-2.0.3.dev7/src/mapel_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 17:34:47.000000 mapel-core-2.0.3.dev7/src/mapel_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-24 17:34:47.000000 mapel-core-2.0.3.dev7/src/mapel_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-24 17:34:47.000000 mapel-core-2.0.3.dev7/src/mapel_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 10:39:44.000000 mapel-core-2.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-26 10:40:01.649973 mapel-core-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-26 10:39:44.000000 mapel-core-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-26 10:39:44.000000 mapel-core-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 10:39:44.000000 mapel-core-2.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:40:01.649973 mapel-core-2.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.645973 mapel-core-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.645973 mapel-core-2.0.4/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/src/mapel/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/src/mapel/core/embedding/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/initial_positions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/src/mapel/core/embedding/kamada_kawai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/kamada_kawai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/kamada_kawai/energy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/src/mapel/core/embedding/simulated_annealing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/simulated_annealing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5195 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/src/mapel/core/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/features/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/features/distortion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/features/monotonicity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/features/stability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/features_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6788 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/glossary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3496 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/inner_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/matchings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/src/mapel/core/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)    24483 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/objects/Experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/objects/Family.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/objects/Instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/src/mapel/core/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/persistence/experiment_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/persistence/experiment_imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62604 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/printing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-05-26 10:39:44.000000 mapel-core-2.0.4/src/mapel/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:40:01.649973 mapel-core-2.0.4/src/mapel_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-26 10:40:01.000000 mapel-core-2.0.4/src/mapel_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-26 10:40:01.000000 mapel-core-2.0.4/src/mapel_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:40:01.000000 mapel-core-2.0.4/src/mapel_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 10:40:01.000000 mapel-core-2.0.4/src/mapel_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 10:40:01.000000 mapel-core-2.0.4/src/mapel_core.egg-info/top_level.txt
```

### Comparing `mapel-core-2.0.3.dev7/LICENSE.txt` & `mapel-core-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/PKG-INFO` & `mapel-core-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.0.3.dev7
+Version: 2.0.4
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-core-2.0.3.dev7/README.md` & `mapel-core-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/pyproject.toml` & `mapel-core-2.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-core"
-version = "2.0.3.dev7"
+version = "2.0.4"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Kasper Sapala", email = "kasper.sapala@gmail.com"},
  {name = "Tomasz Was", email = "tomasz.t.was@gmail.com"},
 ]
```

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/embedding/initial_positions.py` & `mapel-core-2.0.4/src/mapel/core/embedding/initial_positions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/embedding/kamada_kawai/energy_functions.py` & `mapel-core-2.0.4/src/mapel/core/embedding/kamada_kawai/energy_functions.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py` & `mapel-core-2.0.4/src/mapel/core/embedding/kamada_kawai/kamada_kawai.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py` & `mapel-core-2.0.4/src/mapel/core/embedding/kamada_kawai/optimization_algorithms.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                 if 1 - percentage < min_improvement_percentage:
                     return x.copy()
 
             min_energy = current_energy
             min_energy_snap = x.copy()
             min_energy_iter = i
         elif i - min_energy_iter > max_iter_without_improvement:
-            print(f'More than {max_iter_without_improvement} iterations without improvement')
+            # print(f'More than {max_iter_without_improvement} iterations without improvement')
             return min_energy_snap
 
         # print(f'Energy: {current_energy}: {min_energy}, grad norm: {np.linalg.norm(prev_grad)} {i}')
         if stop_energy_val is not None and current_energy < stop_energy_val:
             return min_energy_snap
         s = x - prev_x
         g = grad_func(x, *args)
```

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py` & `mapel-core-2.0.4/src/mapel/core/embedding/simulated_annealing/simulated_annealing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py` & `mapel-core-2.0.4/src/mapel/core/embedding/simulated_annealing/simulated_annealing_energy.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/features/common.py` & `mapel-core-2.0.4/src/mapel/core/features/common.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/features/distortion.py` & `mapel-core-2.0.4/src/mapel/core/features/distortion.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/features/monotonicity.py` & `mapel-core-2.0.4/src/mapel/core/features/monotonicity.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/features/stability.py` & `mapel-core-2.0.4/src/mapel/core/features/stability.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/features_main.py` & `mapel-core-2.0.4/src/mapel/core/features_main.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/glossary.py` & `mapel-core-2.0.4/src/mapel/core/glossary.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/inner_distances.py` & `mapel-core-2.0.4/src/mapel/core/inner_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/matchings.py` & `mapel-core-2.0.4/src/mapel/core/matchings.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/objects/Experiment.py` & `mapel-core-2.0.4/src/mapel/core/objects/Experiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 
 from mapel.core.embedding.kamada_kawai.kamada_kawai import KamadaKawai
 from mapel.core.embedding.simulated_annealing.simulated_annealing import SimulatedAnnealing
 
 import mapel.core.persistence.experiment_imports as imports
 import mapel.core.persistence.experiment_exports as exports
 
-
 COLORS = []
 
 try:
     from sklearn.manifold import MDS
     from sklearn.manifold import TSNE
     from sklearn.manifold import SpectralEmbedding
     from sklearn.manifold import LocallyLinearEmbedding
@@ -106,17 +105,24 @@
         if isinstance(instances, dict):
             self.instances = instances
             print('=== Omitting import! ===')
         elif is_imported and self.experiment_id != 'virtual':
             try:
                 self.instances = self.add_instances_to_experiment()
                 self.num_instances = len(self.instances)
-                print('=== Elections imported successfully! ===')
+
+                for instance in self.instances.values():
+                    if instance.votes is None:
+                        print('=== Instances not found! ===')
+                        break
+                else:
+                    print('=== Instances imported successfully! ===')
+
             except FileNotFoundError:
-                print('=== Elections not found! ===')
+                print('=== Instances not found! ===')
                 self.instances = {}
         else:
             self.instances = {}
 
         if isinstance(distances, dict):
             self.distances = distances
             print('=== Omitting import! ===')
@@ -325,18 +331,18 @@
     def print_map_1d(self, **kwargs) -> None:
         pr.print_map_1d(self, **kwargs)
 
     def print_map_2d(self, **kwargs) -> None:
         pr.print_map_2d(self, **kwargs)
 
     def print_map_2d_colored_by_feature(self, **kwargs) -> None:
-        pr.print_map_2d(self, **kwargs)
+        pr.print_map_2d_colored_by_feature(self, **kwargs)
 
     def print_map_2d_colored_by_features(self, **kwargs) -> None:
-        pr.print_map_2d(self, **kwargs)
+        pr.print_map_2d_colored_by_features(self, **kwargs)
 
     def print_map_3d(self, **kwargs) -> None:
         pr.print_map_3d(self, **kwargs)
 
     def print_map(self, dim: int = 2, **kwargs) -> None:
         if dim == 1:
             pr.print_map_1d(self, **kwargs)
@@ -403,15 +409,15 @@
                 coordinates_by_families[family_id] = [[] for _ in range(3)]
 
                 if dim == 2:
                     for instance_id in self.families[family_id].instance_ids:
                         coordinates_by_families[family_id][0].append(
                             self.coordinates[instance_id][0])
                         coordinates_by_families[family_id][1].append(
-                                self.coordinates[instance_id][1])
+                            self.coordinates[instance_id][1])
 
         self.coordinates_by_families = coordinates_by_families
 
     def get_distance(self, i, j):
         """ Compute Euclidean distance in two-dimensional space"""
 
         distance = 0.
@@ -482,16 +488,16 @@
 
     def import_feature(self, feature_id, column_id='value', rule=None):
         if rule is None:
             feature_long_id = feature_id
         else:
             feature_long_id = f'{feature_id}_{rule}'
         return imports.get_values_from_csv_file(self, feature_id=feature_id,
-                                           column_id=column_id,
-                                           feature_long_id=feature_long_id)
+                                                column_id=column_id,
+                                                feature_long_id=feature_long_id)
 
     def normalize_feature_by_feature(self, nom=None, denom=None, saveas=None, column_id='value'):
 
         f1 = self.get_feature(nom, column_id=column_id)
         f2 = self.get_feature(denom, column_id=column_id)
         f3 = {}
 
@@ -623,15 +629,15 @@
                 new_image.paste(images[i + j * ncol], (image1_size[0] * i, image1_size[1] * j))
 
         new_image.save(f'images/microscope/{name}.png', "PNG", quality=85)
         if show:
             new_image.show()
 
     def merge_election_images_in_parts(self, size=250, name=None, show=False, ncol=1, nrow=1,
-                              distance_id='hamming'):
+                                       distance_id='hamming'):
         pass
 
     def merge_election_images_double(self, size=250, name=None,
                                      distance_ids=None,
                                      show=False, ncol=1, nrow=1):
         images = []
         for i, election in enumerate(self.instances.values()):
@@ -645,10 +651,7 @@
         for i in range(ncol):
             for j in range(nrow):
                 new_image.paste(images[i + j * ncol], (image1_size[0] * i, image1_size[1] * j))
 
         new_image.save(f'images/microscope/{name}.png', "PNG", quality=85)
         if show:
             new_image.show()
-
-
-
```

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/objects/Family.py` & `mapel-core-2.0.4/src/mapel/core/objects/Family.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/persistence/experiment_exports.py` & `mapel-core-2.0.4/src/mapel/core/persistence/experiment_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/persistence/experiment_imports.py` & `mapel-core-2.0.4/src/mapel/core/persistence/experiment_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/printing.py` & `mapel-core-2.0.4/src/mapel/core/printing.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel/core/utils.py` & `mapel-core-2.0.4/src/mapel/core/utils.py`

 * *Files identical despite different names*

### Comparing `mapel-core-2.0.3.dev7/src/mapel_core.egg-info/PKG-INFO` & `mapel-core-2.0.4/src/mapel_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-core
-Version: 2.0.3.dev7
+Version: 2.0.4
 Summary: Map of Elections---essential parts
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanisław Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-core-2.0.3.dev7/src/mapel_core.egg-info/SOURCES.txt` & `mapel-core-2.0.4/src/mapel_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

