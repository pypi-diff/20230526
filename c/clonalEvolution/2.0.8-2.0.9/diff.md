# Comparing `tmp/clonalEvolution-2.0.8.tar.gz` & `tmp/clonalEvolution-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clonalEvolution-2.0.8.tar", last modified: Thu May 25 22:45:00 2023, max compression
+gzip compressed data, was "clonalEvolution-2.0.9.tar", last modified: Thu May 25 23:16:32 2023, max compression
```

## Comparing `clonalEvolution-2.0.8.tar` & `clonalEvolution-2.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 22:45:00.841974 clonalEvolution-2.0.8/
--rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.8/LICENSE
--rw-rw-rw-   0        0        0     5378 2023-05-25 22:45:00.842973 clonalEvolution-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.8/README.md
--rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       81 2023-05-25 22:45:00.843970 clonalEvolution-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     3866 2023-05-25 22:44:48.000000 clonalEvolution-2.0.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:45:00.793921 clonalEvolution-2.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-05-25 22:45:00.822981 clonalEvolution-2.0.8/src/clonalEvolution/
--rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.8/src/clonalEvolution/__init__.py
--rw-rw-rw-   0        0        0    21317 2023-05-22 16:22:59.000000 clonalEvolution-2.0.8/src/clonalEvolution/__main__.py
--rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.8/src/clonalEvolution/clonal_evolution_binned_loop.py
--rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.8/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
--rw-rw-rw-   0        0        0    25157 2023-05-25 22:36:13.000000 clonalEvolution-2.0.8/src/clonalEvolution/clonal_evolution_init.py
--rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.8/src/clonalEvolution/clonal_evolution_loop.py
--rw-rw-rw-   0        0        0    32641 2023-05-25 22:44:36.000000 clonalEvolution-2.0.8/src/clonalEvolution/external_plots.py
--rw-rw-rw-   0        0        0    45629 2023-05-25 22:36:13.000000 clonalEvolution-2.0.8/src/clonalEvolution/mainView.py
--rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.8/src/clonalEvolution/wmean.py
-drwxrwxrwx   0        0        0        0 2023-05-25 22:45:00.837941 clonalEvolution-2.0.8/src/clonalEvolution.egg-info/
--rw-rw-rw-   0        0        0     5378 2023-05-25 22:45:00.000000 clonalEvolution-2.0.8/src/clonalEvolution.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      695 2023-05-25 22:45:00.000000 clonalEvolution-2.0.8/src/clonalEvolution.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 22:45:00.000000 clonalEvolution-2.0.8/src/clonalEvolution.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-25 22:45:00.000000 clonalEvolution-2.0.8/src/clonalEvolution.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       36 2023-05-25 22:45:00.000000 clonalEvolution-2.0.8/src/clonalEvolution.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-25 22:45:00.000000 clonalEvolution-2.0.8/src/clonalEvolution.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 22:45:00.839936 clonalEvolution-2.0.8/tests/
--rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.8/tests/test_simple.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:16:32.667678 clonalEvolution-2.0.9/
+-rw-rw-rw-   0        0        0    33092 2022-08-22 08:14:00.000000 clonalEvolution-2.0.9/LICENSE
+-rw-rw-rw-   0        0        0     5378 2023-05-25 23:16:32.667678 clonalEvolution-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     4385 2022-11-14 12:37:06.000000 clonalEvolution-2.0.9/README.md
+-rw-rw-rw-   0        0        0      101 2022-08-26 06:02:56.000000 clonalEvolution-2.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2023-05-25 23:16:32.669673 clonalEvolution-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     3866 2023-05-25 23:16:18.000000 clonalEvolution-2.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:16:32.621684 clonalEvolution-2.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-05-25 23:16:32.647639 clonalEvolution-2.0.9/src/clonalEvolution/
+-rw-rw-rw-   0        0        0        0 2022-08-19 13:09:48.000000 clonalEvolution-2.0.9/src/clonalEvolution/__init__.py
+-rw-rw-rw-   0        0        0    21317 2023-05-22 16:22:59.000000 clonalEvolution-2.0.9/src/clonalEvolution/__main__.py
+-rw-rw-rw-   0        0        0    11534 2022-10-20 07:43:40.000000 clonalEvolution-2.0.9/src/clonalEvolution/clonal_evolution_binned_loop.py
+-rw-rw-rw-   0        0        0     8264 2022-12-14 17:16:26.000000 clonalEvolution-2.0.9/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py
+-rw-rw-rw-   0        0        0    25158 2023-05-25 23:16:11.000000 clonalEvolution-2.0.9/src/clonalEvolution/clonal_evolution_init.py
+-rw-rw-rw-   0        0        0     5977 2022-11-06 16:00:04.000000 clonalEvolution-2.0.9/src/clonalEvolution/clonal_evolution_loop.py
+-rw-rw-rw-   0        0        0    32641 2023-05-25 22:44:36.000000 clonalEvolution-2.0.9/src/clonalEvolution/external_plots.py
+-rw-rw-rw-   0        0        0    45629 2023-05-25 22:36:13.000000 clonalEvolution-2.0.9/src/clonalEvolution/mainView.py
+-rw-rw-rw-   0        0        0      185 2022-08-22 08:11:04.000000 clonalEvolution-2.0.9/src/clonalEvolution/wmean.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:16:32.662692 clonalEvolution-2.0.9/src/clonalEvolution.egg-info/
+-rw-rw-rw-   0        0        0     5378 2023-05-25 23:16:32.000000 clonalEvolution-2.0.9/src/clonalEvolution.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      695 2023-05-25 23:16:32.000000 clonalEvolution-2.0.9/src/clonalEvolution.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 23:16:32.000000 clonalEvolution-2.0.9/src/clonalEvolution.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-25 23:16:32.000000 clonalEvolution-2.0.9/src/clonalEvolution.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       36 2023-05-25 23:16:32.000000 clonalEvolution-2.0.9/src/clonalEvolution.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-25 23:16:32.000000 clonalEvolution-2.0.9/src/clonalEvolution.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-25 23:16:32.664686 clonalEvolution-2.0.9/tests/
+-rw-rw-rw-   0        0        0      417 2022-03-24 22:23:18.000000 clonalEvolution-2.0.9/tests/test_simple.py
```

### Comparing `clonalEvolution-2.0.8/LICENSE` & `clonalEvolution-2.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.8/PKG-INFO` & `clonalEvolution-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.8
+Version: 2.0.9
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.8/README.md` & `clonalEvolution-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.8/setup.py` & `clonalEvolution-2.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # There are some restrictions on what makes a valid project name
     # specification here:
     # https://packaging.python.org/specifications/core-metadata/#name
     name="clonalEvolution", 
-    version="2.0.8",
+    version="2.0.9",
     description="Software for simulating clonal evolution in binned and tau leap version.",
     url="https://github.com/JGil-polsl/clonalEvolution",
     author="Jaroslaw Gil",  
     author_email="jaroslaw.gil@polsl.pl",
     long_description=long_description,
     long_description_content_type='text/markdown',
     # Classifiers help users find your project by categorizing it.
```

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution/__main__.py` & `clonalEvolution-2.0.9/src/clonalEvolution/__main__.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution/clonal_evolution_binned_loop.py` & `clonalEvolution-2.0.9/src/clonalEvolution/clonal_evolution_binned_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py` & `clonalEvolution-2.0.9/src/clonalEvolution/clonal_evolution_clone_matrix_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution/clonal_evolution_init.py` & `clonalEvolution-2.0.9/src/clonalEvolution/clonal_evolution_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -520,15 +520,15 @@
         if select == 0: 
             if(len(iPop)) >= 10*pop:
                 break
         elif select == 1:
             if(sum([row[1] for row in iPop])) >= 10*pop:
                 break
         elif select == 2:
-            if(sum([row[1] for row in iPop])) >= 10*pop:
+            if(sum([row[1] for row in iPop])) >= 100*pop:
                 break
         
         if select == 0:            
             iPop = CEL.clonalEvolutionLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads)
         elif select == 1:
             iPop = CEBL.clonalEvolutionBinnedLoop(iPop, cap, tau, mut_prob, mut_effect, resume, q, threads, print_time)
         elif select == 2:
```

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution/clonal_evolution_loop.py` & `clonalEvolution-2.0.9/src/clonalEvolution/clonal_evolution_loop.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution/external_plots.py` & `clonalEvolution-2.0.9/src/clonalEvolution/external_plots.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution/mainView.py` & `clonalEvolution-2.0.9/src/clonalEvolution/mainView.py`

 * *Files identical despite different names*

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution.egg-info/PKG-INFO` & `clonalEvolution-2.0.9/src/clonalEvolution.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clonalEvolution
-Version: 2.0.8
+Version: 2.0.9
 Summary: Software for simulating clonal evolution in binned and tau leap version.
 Home-page: https://github.com/JGil-polsl/clonalEvolution
 Author: Jaroslaw Gil
 Author-email: jaroslaw.gil@polsl.pl
 Project-URL: Bug Reports, https://github.com/JGil-polsl/clonalEvolution/issues
 Project-URL: Source, https://github.com/JGil-polsl/clonalEvolution
 Keywords: clonal evolution,microbial,numerical modelling
```

### Comparing `clonalEvolution-2.0.8/src/clonalEvolution.egg-info/SOURCES.txt` & `clonalEvolution-2.0.9/src/clonalEvolution.egg-info/SOURCES.txt`

 * *Files identical despite different names*

