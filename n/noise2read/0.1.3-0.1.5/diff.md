# Comparing `tmp/noise2read-0.1.3.tar.gz` & `tmp/noise2read-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "noise2read-0.1.3.tar", last modified: Thu May 25 04:40:12 2023, max compression
+gzip compressed data, was "noise2read-0.1.5.tar", last modified: Fri May 26 06:19:22 2023, max compression
```

## Comparing `noise2read-0.1.3.tar` & `noise2read-0.1.5.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-25 04:40:12.759254 noise2read-0.1.3/
--rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.1.3/LICENSE
--rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-25 04:40:12.760634 noise2read-0.1.3/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.1.3/README.rst
--rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.1.3/pyproject.toml
--rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-25 04:40:12.763844 noise2read-0.1.3/setup.cfg
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-25 04:40:12.609970 noise2read-0.1.3/src/
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-25 04:40:12.701946 noise2read-0.1.3/src/noise2read/
--rw-r--r--   0 pping    (55472) Research  (5010)      181 2023-05-25 03:20:22.000000 noise2read-0.1.3/src/noise2read/__init__.py
--rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.1.3/src/noise2read/classifier.py
--rw-r--r--   0 pping    (55472) Research  (5010)    17772 2023-05-25 04:28:54.000000 noise2read-0.1.3/src/noise2read/config.py
--rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.1.3/src/noise2read/coverage.py
--rw-r--r--   0 pping    (55472) Research  (5010)    70175 2023-04-20 03:30:20.000000 noise2read-0.1.3/src/noise2read/data_analysis.py
--rw-r--r--   0 pping    (55472) Research  (5010)    56303 2023-05-24 04:48:03.000000 noise2read-0.1.3/src/noise2read/data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)    11566 2023-05-21 07:12:51.000000 noise2read-0.1.3/src/noise2read/data_preprocessing.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.1.3/src/noise2read/encoding.py
--rw-r--r--   0 pping    (55472) Research  (5010)    30905 2023-05-25 03:14:47.000000 noise2read-0.1.3/src/noise2read/error_orrection.py
--rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.1.3/src/noise2read/isolates_correction.py
--rw-r--r--   0 pping    (55472) Research  (5010)    26142 2023-05-25 04:15:46.000000 noise2read-0.1.3/src/noise2read/noise2read.py
--rw-r--r--   0 pping    (55472) Research  (5010)    39224 2023-05-23 08:52:23.000000 noise2read-0.1.3/src/noise2read/reads2vectors.py
--rw-r--r--   0 pping    (55472) Research  (5010)    25173 2023-05-25 00:59:34.000000 noise2read-0.1.3/src/noise2read/simulation.py
--rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.1.3/src/noise2read/umitest.py
--rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.1.3/src/noise2read/utils.py
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-25 04:40:12.739883 noise2read-0.1.3/src/noise2read.egg-info/
--rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-25 04:40:12.000000 noise2read-0.1.3/src/noise2read.egg-info/PKG-INFO
--rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-25 04:40:12.000000 noise2read-0.1.3/src/noise2read.egg-info/SOURCES.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-25 04:40:12.000000 noise2read-0.1.3/src/noise2read.egg-info/dependency_links.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-25 04:40:12.000000 noise2read-0.1.3/src/noise2read.egg-info/entry_points.txt
--rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.1.3/src/noise2read.egg-info/not-zip-safe
--rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-25 04:40:12.000000 noise2read-0.1.3/src/noise2read.egg-info/requires.txt
--rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-25 04:40:12.000000 noise2read-0.1.3/src/noise2read.egg-info/top_level.txt
-drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-25 04:40:12.754802 noise2read-0.1.3/tests/
--rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.1.3/tests/test_data_generation.py
--rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.1.3/tests/test_reads2vector.py
--rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.1.3/tests/test_utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-26 06:19:22.392622 noise2read-0.1.5/
+-rw-r--r--   0 pping    (55472) Research  (5010)     1068 2023-04-20 03:30:20.000000 noise2read-0.1.5/LICENSE
+-rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-26 06:19:22.393900 noise2read-0.1.5/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)     5531 2023-05-13 12:21:26.000000 noise2read-0.1.5/README.rst
+-rw-r--r--   0 pping    (55472) Research  (5010)       90 2023-04-20 03:30:20.000000 noise2read-0.1.5/pyproject.toml
+-rw-r--r--   0 pping    (55472) Research  (5010)      999 2023-05-26 06:19:22.397674 noise2read-0.1.5/setup.cfg
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-26 06:19:22.109135 noise2read-0.1.5/src/
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-26 06:19:22.258286 noise2read-0.1.5/src/noise2read/
+-rw-r--r--   0 pping    (55472) Research  (5010)      181 2023-05-26 03:48:17.000000 noise2read-0.1.5/src/noise2read/__init__.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    13443 2023-05-16 08:27:41.000000 noise2read-0.1.5/src/noise2read/classifier.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    17548 2023-05-26 03:51:43.000000 noise2read-0.1.5/src/noise2read/config.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     2701 2023-04-20 03:30:20.000000 noise2read-0.1.5/src/noise2read/coverage.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    71846 2023-05-26 04:00:17.000000 noise2read-0.1.5/src/noise2read/data_analysis.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    57420 2023-05-26 04:01:57.000000 noise2read-0.1.5/src/noise2read/data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    11566 2023-05-21 07:12:51.000000 noise2read-0.1.5/src/noise2read/data_preprocessing.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    30052 2023-05-14 01:00:24.000000 noise2read-0.1.5/src/noise2read/encoding.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    31512 2023-05-25 13:51:45.000000 noise2read-0.1.5/src/noise2read/error_orrection.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    16773 2023-04-20 03:30:20.000000 noise2read-0.1.5/src/noise2read/isolates_correction.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    26445 2023-05-25 12:08:29.000000 noise2read-0.1.5/src/noise2read/noise2read.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    40000 2023-05-26 04:03:27.000000 noise2read-0.1.5/src/noise2read/reads2vectors.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    28571 2023-05-26 04:07:33.000000 noise2read-0.1.5/src/noise2read/simulation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     3475 2023-04-20 03:30:20.000000 noise2read-0.1.5/src/noise2read/umitest.py
+-rw-r--r--   0 pping    (55472) Research  (5010)    15905 2023-04-20 03:30:20.000000 noise2read-0.1.5/src/noise2read/utils.py
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-26 06:19:22.321854 noise2read-0.1.5/src/noise2read.egg-info/
+-rw-r--r--   0 pping    (55472) Research  (5010)     5950 2023-05-26 06:19:21.000000 noise2read-0.1.5/src/noise2read.egg-info/PKG-INFO
+-rw-r--r--   0 pping    (55472) Research  (5010)      837 2023-05-26 06:19:22.000000 noise2read-0.1.5/src/noise2read.egg-info/SOURCES.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-05-26 06:19:21.000000 noise2read-0.1.5/src/noise2read.egg-info/dependency_links.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       58 2023-05-26 06:19:22.000000 noise2read-0.1.5/src/noise2read.egg-info/entry_points.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)        1 2023-04-20 03:31:42.000000 noise2read-0.1.5/src/noise2read.egg-info/not-zip-safe
+-rw-r--r--   0 pping    (55472) Research  (5010)      217 2023-05-26 06:19:22.000000 noise2read-0.1.5/src/noise2read.egg-info/requires.txt
+-rw-r--r--   0 pping    (55472) Research  (5010)       11 2023-05-26 06:19:22.000000 noise2read-0.1.5/src/noise2read.egg-info/top_level.txt
+drwxr-xr-x   0 pping    (55472) Research  (5010)        0 2023-05-26 06:19:22.369791 noise2read-0.1.5/tests/
+-rw-r--r--   0 pping    (55472) Research  (5010)     3641 2023-04-20 03:30:20.000000 noise2read-0.1.5/tests/test_data_generation.py
+-rw-r--r--   0 pping    (55472) Research  (5010)      985 2023-04-20 03:30:20.000000 noise2read-0.1.5/tests/test_reads2vector.py
+-rw-r--r--   0 pping    (55472) Research  (5010)     4216 2023-04-20 03:30:20.000000 noise2read-0.1.5/tests/test_utils.py
```

### Comparing `noise2read-0.1.3/LICENSE` & `noise2read-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/PKG-INFO` & `noise2read-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.1.3
+Version: 0.1.5
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.1.3/README.rst` & `noise2read-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/setup.cfg` & `noise2read-0.1.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/src/noise2read/classifier.py` & `noise2read-0.1.5/src/noise2read/classifier.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/src/noise2read/config.py` & `noise2read-0.1.5/src/noise2read/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-19 10:56:38
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-25 14:28:54
+# @Last Modified time: 2023-05-26 13:51:43
 
 import configparser
 import os
 
 class Config(object):
     def __init__(self, config_file, logger):
         conf = configparser.ConfigParser()
@@ -261,44 +261,40 @@
             # else:
             #     self.amplicon_error_node_degree = 4 # default   
 
             # Simulation
             if conf.has_option("Simulation", "min_freq"):
                 self.min_freq = conf.getint("Simulation", "min_freq")
             else:
-                self.min_freq = 7 # default
-            # if conf.has_option("Simulation", "min_read_count"):
-            #     self.min_read_count = conf.getint("Simulation", "min_read_count")
-            # else:
-            #     self.min_read_count = 30 # default
-                
-            if conf.has_option("Simulation", "substations"):
-                self.substations = conf.getboolean("Simulation", "substations")
-            else:
-                self.substations = True
-            if conf.has_option("Simulation", "indels"):
-                self.indels = conf.getboolean("Simulation", "indels")
+                self.min_freq = 4 # default
+            if conf.has_option("Simulation", "min_read_count"):
+                self.min_read_count = conf.getint("Simulation", "min_read_count")
             else:
-                self.indels = False
+                self.min_read_count = 30 # default
+                
+            # if conf.has_option("Simulation", "substations"):
+            #     self.substations = conf.getboolean("Simulation", "substations")
+            # else:
+            #     self.substations = True
+            # if conf.has_option("Simulation", "indels"):
+            #     self.indels = conf.getboolean("Simulation", "indels")
+            # else:
+            #     self.indels = False
 
             if conf.has_option("Simulation", "error_rate1"):
                 self.error_rate1 = conf.getfloat("Simulation", "error_rate1")
             else:
-                self.error_rate1 = 0.1 # default
+                self.error_rate1 = 0.09 # default
 
             if conf.has_option("Simulation", "error_rate2"):
                 self.error_rate2 = conf.getfloat("Simulation", "error_rate2")
             else:
-                self.error_rate2 = 0.05 # default
+                self.error_rate2 = 0.02 # default
+
 
-            if conf.has_option("Simulation", "sim_seed"):
-                self.sim_seed = conf.getint("Simulation", "sim_seed")
-            else:
-                self.sim_seed = 42 # default
-                
             # # Evaluation
             # if conf.has_option("Evaluation", "delta"):
             #     self.delta = conf.getint("Evaluation", "delta")
             # else:
             #     self.delta = 10 # default
 
         if config_file == None:
@@ -372,22 +368,21 @@
             #amplicon
             self.amplicon_low_freq = 50
             self.amplicon_high_freq = 5000
             self.amplicon_threshold_proba = 0.85
             # self.amplicon_error_node_degree = 4
 
             # simulation
-            self.min_freq = 7
-            # self.min_read_count = 30
-            self.substations = True
-            self.indels = False
-            self.error_rate1 = 0.1
-            self.error_rate2 = 0.05
-            self.sim_seed = 42
-
+            self.min_freq = 4
+            self.min_read_count = 30
+            # self.substations = True
+            # self.indels = False
+            self.error_rate1 = 0.09
+            self.error_rate2 = 0.02
+  
             # # Evaluation
             # self.delta = 1
 
             # # coverage
             # self.library_layout = 'PE'
             # self.Alignment = '--local' # '--end-to-end'
```

### Comparing `noise2read-0.1.3/src/noise2read/coverage.py` & `noise2read-0.1.5/src/noise2read/coverage.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/src/noise2read/data_analysis.py` & `noise2read-0.1.5/src/noise2read/data_analysis.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-30 09:35:18
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-04-11 17:09:30
+# @Last Modified time: 2023-05-26 14:00:17
 
 from collections import Counter
 import collections
 import math
 from Bio import SeqIO
 import os
 import editdistance
@@ -639,56 +639,101 @@
         non_frequent_raw_reads = raw_unique_reads - frequent_reads
         raw_entropy_items = []
         for read in non_frequent_raw_reads:
             raw_entropy_items.append(raw_read2count[read])
 
         raw_nonFre_reads_total_num = sum(raw_entropy_items)
         # raw entropy
-        with WorkerPool(self.config.num_workers, shared_objects=raw_nonFre_reads_total_num, start_method='fork') as pool:
-            raw_entropy_lst = pool.map(self.entropy_item, raw_entropy_items)
-        raw_entropy = sum(raw_entropy_lst) 
+        try:
+            with WorkerPool(self.config.num_workers, shared_objects=raw_nonFre_reads_total_num, start_method='fork') as pool:
+                raw_entropy_lst = pool.map(self.entropy_item, raw_entropy_items)
+            raw_entropy = sum(raw_entropy_lst) 
+        except KeyboardInterrupt:
+            # Handle termination signal (Ctrl+C)
+            pool.terminate()  # Terminate the WorkerPool before exiting
+
+        except Exception:
+            # Handle other exceptions
+            pool.terminate()  # Terminate the WorkerPool before exiting
+            raise
 
         # correct dateset
         non_frequent_correct_reads = correct_unique_reads - frequent_reads
         correct_entropy_items = []
         for read in non_frequent_correct_reads:
             correct_entropy_items.append(correct_read2count[read])
 
         # correct entropy
         correct_nonFre_reads_total_num = sum(correct_entropy_items)
-
-        with WorkerPool(self.config.num_workers, shared_objects=correct_nonFre_reads_total_num, start_method='fork') as pool:
-            correct_entropy_lst = pool.map(self.entropy_item, correct_entropy_items) 
-        correct_entropy = sum(correct_entropy_lst)
+        try:
+            with WorkerPool(self.config.num_workers, shared_objects=correct_nonFre_reads_total_num, start_method='fork') as pool:
+                correct_entropy_lst = pool.map(self.entropy_item, correct_entropy_items) 
+            correct_entropy = sum(correct_entropy_lst)
+        except KeyboardInterrupt:
+            # Handle termination signal (Ctrl+C)
+            pool.terminate()  # Terminate the WorkerPool before exiting
+
+        except Exception:
+            # Handle other exceptions
+            pool.terminate()  # Terminate the WorkerPool before exiting
+            raise
         ##################################################################################
         #information gain (\delta I) heatmap
         new_reads = correct_unique_reads - raw_unique_reads
         new_reads_num = len(new_reads)
         self.logger.info("Wrongly introduced {} new reads".format(new_reads_num))
 
         raw_kept_counts = []
         correct_kept_counts = []
         kept_reads = correct_unique_reads & raw_unique_reads
         for read in kept_reads:
             correct_kept_counts.append(correct_read2count[read])
             raw_kept_counts.append(raw_read2count[read])
 
-        with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
-            raw_kept_entropy_lst = pool.map(self.entropy_item, raw_kept_counts)
-
-        with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
-            correct_kept_entropy_lst = pool.map(self.entropy_item, correct_kept_counts) 
+        try:
+            with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
+                raw_kept_entropy_lst = pool.map(self.entropy_item, raw_kept_counts)
+        except KeyboardInterrupt:
+            # Handle termination signal (Ctrl+C)
+            pool.terminate()  # Terminate the WorkerPool before exiting
+
+        except Exception:
+            # Handle other exceptions
+            pool.terminate()  # Terminate the WorkerPool before exiting
+            raise
+
+        try:
+            with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
+                correct_kept_entropy_lst = pool.map(self.entropy_item, correct_kept_counts) 
+        except KeyboardInterrupt:
+            # Handle termination signal (Ctrl+C)
+            pool.terminate()  # Terminate the WorkerPool before exiting
+
+        except Exception:
+            # Handle other exceptions
+            pool.terminate()  # Terminate the WorkerPool before exiting
+            raise
 
         raw_removed_reads = raw_unique_reads - correct_unique_reads
         raw_removed_items = []
         for read in raw_removed_reads:
             raw_removed_items.append(raw_read2count[read])
 
-        with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
-            raw_removed_entropy_items_lst = pool.map(self.entropy_item, raw_removed_items)
+        try:
+            with WorkerPool(self.config.num_workers, shared_objects=total_num, start_method='fork') as pool:
+                raw_removed_entropy_items_lst = pool.map(self.entropy_item, raw_removed_items)
+        except KeyboardInterrupt:
+            # Handle termination signal (Ctrl+C)
+            pool.terminate()  # Terminate the WorkerPool before exiting
+
+        except Exception:
+            # Handle other exceptions
+            pool.terminate()  # Terminate the WorkerPool before exiting
+            raise
+        
         for i in raw_removed_entropy_items_lst:
             if i <=0:
                 print('Warning')
         entropy_item_lst = []
         for i, j in zip(raw_kept_entropy_lst, correct_kept_entropy_lst):
             entropy_item_lst.append(i - j)
         entropy_item_lst.extend(raw_removed_entropy_items_lst)
```

### Comparing `noise2read-0.1.3/src/noise2read/data_generation.py` & `noise2read-0.1.5/src/noise2read/data_generation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-01-16 15:52:44
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-24 14:48:03
+# @Last Modified time: 2023-05-26 14:01:57
 
 import editdistance
 import networkx as nx
 import os
 import csv
 from tqdm import tqdm
 from noise2read.utils import *
@@ -238,16 +238,26 @@
 
         genuine_lst = []
         for gexf_file in gexf_files:
             cur_graph = nx.read_gexf(gexf_file)
             sub_graphs = [cur_graph.subgraph(c).copy() for c in nx.connected_components(cur_graph)]
             
             subgraph_num = len(sub_graphs)
-            with WorkerPool(self.config.num_workers, shared_objects=sub_graphs, start_method='fork') as pool:
-                cur_genuine_lsts = pool.imap(self.extract_umi_genuine_errs_subgraph, range(subgraph_num))
+            try:
+                with WorkerPool(self.config.num_workers, shared_objects=sub_graphs, start_method='fork') as pool:
+                    cur_genuine_lsts = pool.imap(self.extract_umi_genuine_errs_subgraph, range(subgraph_num))
+            except KeyboardInterrupt:
+                # Handle termination signal (Ctrl+C)
+                pool.terminate()  # Terminate the WorkerPool before exiting
+
+            except Exception:
+                # Handle other exceptions
+                pool.terminate()  # Terminate the WorkerPool before exiting
+                raise
+            
             for item in cur_genuine_lsts:
                 genuine_lst.extend(item)
 
             os.remove(gexf_file)
             del cur_graph, sub_graphs
 
         genuine_df = pd.DataFrame(genuine_lst, columns=["StartRead","StartReadCount", "StartDegree", "ErrorTye","ErrorPosition", "StartErrKmer", "EndErrKmer", "EndRead", "EndReadCount", "EndDegree"])
@@ -346,23 +356,31 @@
 
         high_idx = 0
         genuine_lst = []
         ambiguous_lst = []
         for gexf_file in gexf_files:
             cur_graph = nx.read_gexf(gexf_file)
             sub_graphs = [cur_graph.subgraph(c).copy() for c in nx.connected_components(cur_graph)]
+            try:
+                subgraph_num = len(sub_graphs)
+                shared_obs = sub_graphs, edit_dis
+                with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
+                    for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num)): # progress_bar=self.config.verbose
+                        if genu_ambi_lst[0]:
+                            genuine_lst.extend(genu_ambi_lst[0])
+                            ambiguous_lst.extend(genu_ambi_lst[1])
+            except KeyboardInterrupt:
+                # Handle termination signal (Ctrl+C)
+                pool.terminate()  # Terminate the WorkerPool before exiting
+
+            except Exception:
+                # Handle other exceptions
+                pool.terminate()  # Terminate the WorkerPool before exiting
+                raise
             
-            subgraph_num = len(sub_graphs)
-            shared_obs = sub_graphs, edit_dis
-            with WorkerPool(self.config.num_workers, shared_objects=shared_obs, start_method='fork') as pool:
-                for genu_ambi_lst in pool.imap(self.extract_genuine_ambi_errs_subgraph, range(subgraph_num)): # progress_bar=self.config.verbose
-                    if genu_ambi_lst[0]:
-                        genuine_lst.extend(genu_ambi_lst[0])
-                        ambiguous_lst.extend(genu_ambi_lst[1])
-
             if self.config.high_ambiguous:
                 cur_lst, cur_idx = self.extract_high_ambiguous_errs(sub_graphs, high_idx)
                 high_ambi_lst.extend(cur_lst)
                 high_idx = cur_idx + 1
             os.remove(gexf_file)
             del cur_graph, sub_graphs
         
@@ -684,22 +702,31 @@
         edges_lst = []
         if edit_dis == 1:
             shared_unique_seqs = unique_seqs
         elif edit_dis == 2:
             shared_unique_seqs = low_freq
         
         self.logger.debug("Searching edges for constructing " + str(edit_dis) + "nt-edit-distance read graph...")
-        with WorkerPool(self.config.num_workers, shared_objects=shared_unique_seqs, start_method='fork') as pool:
-            if edit_dis == 1:
-                for edge_lst in pool.imap(self.real_ed1_seqs, high_freq, progress_bar=self.config.verbose):
-                    edges_lst.extend(edge_lst)
-            elif edit_dis == 2:
-                for edge_lst in pool.imap(self.real_ed2_seqs, high_freq, progress_bar=self.config.verbose):
-                    edges_lst.extend(edge_lst)
-
+        try:
+            with WorkerPool(self.config.num_workers, shared_objects=shared_unique_seqs, start_method='fork') as pool:
+                if edit_dis == 1:
+                    for edge_lst in pool.imap(self.real_ed1_seqs, high_freq, progress_bar=self.config.verbose):
+                        edges_lst.extend(edge_lst)
+                elif edit_dis == 2:
+                    for edge_lst in pool.imap(self.real_ed2_seqs, high_freq, progress_bar=self.config.verbose):
+                        edges_lst.extend(edge_lst)
+        except KeyboardInterrupt:
+            # Handle termination signal (Ctrl+C)
+            pool.terminate()  # Terminate the WorkerPool before exiting
+
+        except Exception:
+            # Handle other exceptions
+            pool.terminate()  # Terminate the WorkerPool before exiting
+            raise
+        
         if len(edges_lst) > 0:
             self.logger.debug(len(edges_lst))
             self.logger.debug(edges_lst[0])
             graph.add_edges_from(edges_lst)
         # self.logger.info(str(edit_dis) + "nt-edit-distance read graph construction done.")
         self.logger.info("Done!")
         ########################################################
```

### Comparing `noise2read-0.1.3/src/noise2read/data_preprocessing.py` & `noise2read-0.1.5/src/noise2read/data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/src/noise2read/encoding.py` & `noise2read-0.1.5/src/noise2read/encoding.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/src/noise2read/error_orrection.py` & `noise2read-0.1.5/src/noise2read/error_orrection.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-25 13:14:46
+# @Last Modified time: 2023-05-25 23:51:45
 
 import os
 from Bio import SeqIO
 import pandas as pd
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from noise2read.isolates_correction import IsolatesErrorCorrection
@@ -56,51 +56,59 @@
                 corrected_file (str): The corrected data filename including path.
                 tmp_correct: The filename including path of corrected data without prediction high ambiguous errors
                 new_negative_df: pandas dataframe containing negative samples from the prediction result of ambiguous errors
         """
         corrected_file = self.config.result_dir + self.base[0] + '_corrected.' + self.out_file_tye  
         if isinstance(high_ambiguous_df, pd.DataFrame) and high_ambiguous_df.empty:
             self.logger.info("No ambiguous between high-frequency reads identified!")
-        if isinstance(high_ambiguous_df, pd.DataFrame) and not high_ambiguous_df.empty:
-            genuine_ambi_errs_df, new_negative_df, high_ambi_df = self.all_in_one_ambiguous_err_prediction(unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df, edit_dis=1)
-            # correct errors
-            genuine_corrected_file = self.correct_errors(non_isolates_file, genuine_ambi_errs_df)
-            self.logger.info("Genuine and ambiguous errors corrected.")
-            
-            del genuine_ambi_errs_df, genuine_df, negative_df, ambiguous_df, unique_seqs
-            ###############################################################################################
-            # IEC = IsolatesErrorCorrection(self.logger, self.config.num_workers, isolates_file, genuine_corrected_file, self.config.result_dir, self.config.iso_change_detail, self.config.min_iters)
-            # tmp_corrected_isolates = IEC.bcool_correct_isolates() 
-            # tmp_correct = self.config.result_dir + self.base[0] + '_correct_no_high.' + self.out_file_tye  
-            # if tmp_corrected_isolates and genuine_corrected_file:
-            #     os.system("cat %s %s > %s" % (tmp_corrected_isolates, genuine_corrected_file, tmp_correct))
-            # # if os.path.exists(tmp_corrected_isolates):     
-            # #     os.system("rm %s" % tmp_corrected_isolates)
-            # del IEC
-            #####################################################################
-            non_isolates_correct = self.all_in_one_high_ambiguous_err_correction(genuine_corrected_file, high_ambi_df)
-            del high_ambiguous_df
-            self.logger.info("High ambiguous errors corrected.")
-            self.logger.info('1nt-edit-distance based Errors Correction finished.')
-            self.logger.info("#############################################")
+        if not genuine_df.empty and not ambiguous_df.empty and not negative_df.empty:
+            if isinstance(high_ambiguous_df, pd.DataFrame) and not high_ambiguous_df.empty:
+                genuine_ambi_errs_df, new_negative_df, high_ambi_df = self.all_in_one_ambiguous_err_prediction(unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df, edit_dis=1)
+                # correct errors
+                genuine_corrected_file = self.correct_errors(non_isolates_file, genuine_ambi_errs_df)
+                self.logger.info("Genuine and ambiguous errors corrected.")
+                
+                del genuine_ambi_errs_df, genuine_df, negative_df, ambiguous_df, unique_seqs
+                ###############################################################################################
+                # IEC = IsolatesErrorCorrection(self.logger, self.config.num_workers, isolates_file, genuine_corrected_file, self.config.result_dir, self.config.iso_change_detail, self.config.min_iters)
+                # tmp_corrected_isolates = IEC.bcool_correct_isolates() 
+                # tmp_correct = self.config.result_dir + self.base[0] + '_correct_no_high.' + self.out_file_tye  
+                # if tmp_corrected_isolates and genuine_corrected_file:
+                #     os.system("cat %s %s > %s" % (tmp_corrected_isolates, genuine_corrected_file, tmp_correct))
+                # # if os.path.exists(tmp_corrected_isolates):     
+                # #     os.system("rm %s" % tmp_corrected_isolates)
+                # del IEC
+                #####################################################################
+                non_isolates_correct = self.all_in_one_high_ambiguous_err_correction(genuine_corrected_file, high_ambi_df)
+                del high_ambiguous_df
+                self.logger.info("High ambiguous errors corrected.")
+                self.logger.info('1nt-edit-distance based Errors Correction finished.')
+                self.logger.info("#############################################")
+            else:
+                genuine_ambi_errs_df, new_negative_df = self.all_in_one_ambiguous_err_prediction(unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df=None, edit_dis=1)
+                # correct errors
+                self.logger.info("Correcting 1nt-edit-distance based Errors")
+
+                non_isolates_correct = self.correct_errors(non_isolates_file, genuine_ambi_errs_df)
+                self.logger.info('1nt-edit-distance based Errors Correction Finished')
+                del genuine_ambi_errs_df, negative_df, ambiguous_df, unique_seqs
+        elif not genuine_df.empty:
+            non_isolates_correct = self.correct_errors(non_isolates_file, genuine_df)
+            new_negative_df = pd.DataFrame()
         else:
-            genuine_ambi_errs_df, new_negative_df = self.all_in_one_ambiguous_err_prediction(unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df=None, edit_dis=1)
-            # correct errors
-            self.logger.info("Correcting 1nt-edit-distance based Errors")
-
-            non_isolates_correct = self.correct_errors(non_isolates_file, genuine_ambi_errs_df)
-            self.logger.info('1nt-edit-distance based Errors Correction Finished')
-            del genuine_ambi_errs_df, negative_df, ambiguous_df, unique_seqs
+            self.logger.error("No genuine and ambiguous errors identified, failed to do error correction!")
+            non_isolates_correct = non_isolates_file
+            sys.exit(1)
         # # bcool correction
         IEC = IsolatesErrorCorrection(self.logger, self.config.num_workers, isolates_file, non_isolates_correct, self.config.result_dir, self.config.iso_change_detail, self.config.min_iters)
         corrected_isolates = IEC.bcool_correct_isolates() 
         if corrected_isolates and non_isolates_correct:
             os.system("cat %s %s > %s" % (corrected_isolates, non_isolates_correct, corrected_file))
         else:
-            self.logger.error("No corrected_isolates and/or non_isolates_correct")
+            self.logger.error("No corrected_isolates and/or non_isolates_correct, failed to do error correction")
         del IEC
         if os.path.exists(isolates_file):
             os.system("rm %s" % isolates_file)
         if os.path.exists(non_isolates_file):
             os.system("rm %s" % non_isolates_file)
         if os.path.exists(corrected_isolates):   
             os.system("rm %s" % corrected_isolates)
@@ -125,14 +133,15 @@
             ambiguous_df (DataFrame): pandas dataframe containing ambiguous samples for prediction
             high_ambiguous_df (DataFrame): pandas dataframe containing high ambiguous samples for prediction
             edit_dis (int): edit distance 1 or 2
 
         Returns:
             MultiVariables: genuine_df, new_negative_df, high_ambiguous_df
         """
+        
         RV = Reads2Vectors(self.logger, self.config, edit_dis)
         # RV = Reads2Vectors(self.logger, self.config.num_workers, self.config.result_dir, self.config.read_max_len, self.config.entropy_kmer, self.config.entropy_q, self.config.kmer_freq, self.config.read_type, edit_dis)
         if edit_dis == 1:
             study_name = 'ambiguous_1nt'
         elif edit_dis == 2:
             study_name = 'ambiguous_2nt'
```

### Comparing `noise2read-0.1.3/src/noise2read/isolates_correction.py` & `noise2read-0.1.5/src/noise2read/isolates_correction.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/src/noise2read/noise2read.py` & `noise2read-0.1.5/src/noise2read/noise2read.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2022-12-29 23:04:12
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-25 14:15:46
+# @Last Modified time: 2023-05-25 22:08:29
 
 from noise2read.config import Config
 import sys, getopt
 from noise2read.data_generation import DataGneration
 from noise2read.error_orrection import ErrorCorrection
 from noise2read.data_analysis import DataAnalysis
 import os
@@ -235,16 +235,20 @@
                         corrected_file, new_negative_df = EC.all_in_one_correction(isolates_file, non_isolates_file, unique_seqs, genuine_df, negative_df, ambiguous_df, high_ambiguous_df =None) 
                     if read_min_len > config.min_read_len:
                         genuine_df2, negative_df2, ambiguous_df2, unique_seqs2 = DG.extract_ed2_errors(corrected_file)
                         mid_result = EC.all_in_one_ed2_correction(corrected_file, unique_seqs2, genuine_df2, negative_df2, ambiguous_df2)
                     else:
                         mid_result = corrected_file
                     # mid_result = config.input_file
-                    amplicon_df = DG.extract_amplicon_err_samples(mid_result)
-                    config.correct_data = EC.correct_amplicon_err(mid_result, genuine_df, negative_df, new_negative_df, amplicon_df, config.amplicon_threshold_proba)
+                    if (not new_negative_df.empty or not negative_df.empty) and not genuine_df.empty:
+                        amplicon_df = DG.extract_amplicon_err_samples(mid_result)
+                        config.correct_data = EC.correct_amplicon_err(mid_result, genuine_df, negative_df, new_negative_df, amplicon_df, config.amplicon_threshold_proba)
+                    else:
+                        self.logger.warning("No genuine or negative samples for amplicon errors prediction!")
+                        config.correct_data = mid_result
                 
                     DataAnalysis(logger, config).evaluation()
                     # delete bcool result
                     bcool_dir = os.path.join(config.result_dir, 'bcool/')
                     if os.path.exists(bcool_dir):
                         os.system("rm -rf %s" % bcool_dir)
 ############################################################################################################################
```

### Comparing `noise2read-0.1.3/src/noise2read/reads2vectors.py` & `noise2read-0.1.5/src/noise2read/reads2vectors.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:01:06
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-23 18:52:23
+# @Last Modified time: 2023-05-26 14:03:18
 
 from typing import Counter
 import numpy as np
 # import os
 from sklearn.preprocessing import StandardScaler
 from noise2read.encoding import EncodeScheme
 from mpire import WorkerPool
@@ -455,17 +455,27 @@
             for i in range(len(chunks)):
                 chunk = chunks[i]
                 # print(i)
                 # print(len(chunk), type(chunk))
                 # print(chunk)
                 shared_objects = ES, chunk
                 vectors = []
-                with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-                    for item in pool.imap(self.read2features, range(len(chunk))):
-                        vectors.append(item)
+                try:
+                    with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+                        for item in pool.imap(self.read2features, range(len(chunk))):
+                            vectors.append(item)
+                except KeyboardInterrupt:
+                    # Handle termination signal (Ctrl+C)
+                    pool.terminate()  # Terminate the WorkerPool before exiting
+
+                except Exception:
+                    # Handle other exceptions
+                    pool.terminate()  # Terminate the WorkerPool before exiting
+                    raise
+
                 # Generate the pickle file name
                 file_name = self.config.result_dir + f"chunk_{i}.pickle"
                 # Write the vectors to the pickle file
                 with open(file_name, "wb") as file:
                     pickle.dump(vectors, file)
                 chunk_names.append(file_name)
                 del vectors
@@ -476,19 +486,29 @@
                 with open(file_name, "rb") as file:
                     vectors = pickle.load(file)
                     combined_data.extend(vectors)
                     del vectors
                 os.remove(file_name)
             return combined_data
         else:
-            vectors = []
-            shared_objects = ES, original_features_lst
-            with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-                for item in pool.imap(self.read2features, range(len(original_features_lst))):
-                    vectors.append(item)
+            try:
+                vectors = []
+                shared_objects = ES, original_features_lst
+                with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+                    for item in pool.imap(self.read2features, range(len(original_features_lst))):
+                        vectors.append(item)
+            except KeyboardInterrupt:
+                # Handle termination signal (Ctrl+C)
+                pool.terminate()  # Terminate the WorkerPool before exiting
+
+            except Exception:
+                # Handle other exceptions
+                pool.terminate()  # Terminate the WorkerPool before exiting
+                raise
+
             return vectors
 
     
     def high_all_in_one_embedding(self, genuine_df, negative_df, new_negative_df, ambiguous_df):
         self.logger.info("Embedding genuine and high ambiguous data.")
         base_lst = ['A', 'C', 'G', 'T', 'N']
         if self.config.read_type == "DNA":
```

### Comparing `noise2read-0.1.3/src/noise2read/simulation.py` & `noise2read-0.1.5/src/noise2read/simulation.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 # @Author: Pengyao Ping
 # @Date:   2023-02-16 11:04:45
 # @Last Modified by:   Pengyao Ping
-# @Last Modified time: 2023-05-25 10:59:34
+# @Last Modified time: 2023-05-26 14:07:33
 
 import collections
 from Bio import SeqIO
 # import gzip
 from Bio.SeqRecord import SeqRecord
 from Bio.Seq import Seq
 from tqdm import tqdm
@@ -160,210 +160,124 @@
         raw_data, true_data = self.error_injection(corrected_data)
         # raw_data, true_data = self.error_injection(self.config.input_file)
         DP = DataProcessing( 
             self.logger,
             self.config)
         umi_raw_dataset, umi_true_dataset = DP.write_mimic_umis(raw_data, true_data)
         return umi_raw_dataset, umi_true_dataset
-
+    
     def error_injection(self, data_set):
         records_dict, file_type = parse_data_dict(data_set)
         id_lst = list(records_dict.keys())
 
         total_seqs_lst = []
         seq2id_dict = {}
         for item in id_lst:
             seq = str(records_dict[item].seq)
             seq2id_dict.setdefault(seq, []).append(item)
             total_seqs_lst.append(seq)
-            # total_bases += len(seq)
-            # total_reads += 1
-            
+  
         read2counts = collections.Counter(total_seqs_lst)
         select_id_lst = []
-        # total_bases = 0
-        total_reads = 0
-        new_read2counts = {}
+        mutated_id_pool = []
         for read, count in read2counts.items():
-            # if count >= 5:
             if count > self.config.min_freq:
                 select_id_lst.extend(seq2id_dict[read])
-            # if count > self.config.min_read_count:
-            #     new_read2counts[read] = count
-            #     total_reads += count
-            #     # total_bases += len(read) * count
+            if count > self.config.min_read_count:
+                mutated_id_pool.extend(seq2id_dict[read])
 
-        if self.config.error_rate1 > 0:
-            total_id_num = len(select_id_lst)
-            err_1base_read_num = round(total_id_num * self.config.error_rate1)
-            rng = np.random.default_rng(seed=self.config.sim_seed)
-            indices = rng.permutation(total_id_num)[:err_1base_read_num]
+        if self.config.error_rate1 > 0 and self.config.error_rate1 < 1:
+            flag1 = True
             err_1_id_lst = []
-            err_1_id_lst.extend(select_id_lst[i] for i in indices)
-            self.logger.info(f"Total reads: {total_id_num}, 1-base-error per read error rate: {self.config.error_rate1}, 1-base-error reads number: {len(err_1_id_lst)}")
+            total_id_num = len(mutated_id_pool)
+            err_1base_read_num = round(total_id_num * self.config.error_rate1)
+
+            random.shuffle(mutated_id_pool)
+            err_1_id_lst.extend(random.sample(mutated_id_pool, err_1base_read_num))
+      
+            self.logger.info(f"Total candidature reads: {total_id_num}, 1-base-error per read error rate: {self.config.error_rate1}, 1-base-error reads number: {err_1base_read_num}")
         else:
             self.logger.error("Input invalid 1-base-error per read error rate!")
             sys.exit(1)
 
-        # two base errors
-        if self.config.error_rate2 > 0:
-            remain_id_lst = list(set(select_id_lst) - set(err_1_id_lst))
+        # # two base errors
+        if self.config.error_rate2 > 0 and self.config.error_rate2 < 1:
+            flag2 = True
+            remain_id_lst = list(set(mutated_id_pool) - set(err_1_id_lst))
             remain_id_num = len(remain_id_lst)
             err_2bases_read_num = round(remain_id_num * self.config.error_rate2)
 
             err_2_id_lst = []
-            rng = np.random.default_rng(seed=self.config.sim_seed)
-            indices_2 = rng.permutation(remain_id_num)[:err_2bases_read_num]
-            err_2_id_lst.extend(remain_id_lst[i] for i in indices_2)
-            self.logger.info(f"Total reads: {total_id_num}, 2-base-errors per read error rate: {self.config.error_rate2}, 2-base-errors reads number: {len(err_2_id_lst)}")
+            random.shuffle(remain_id_lst)
+            err_2_id_lst.extend(random.sample(remain_id_lst, err_2bases_read_num))
+
+            self.logger.info(f"Remaining candidature reads: {remain_id_num}, 2-base-errors per read error rate: {self.config.error_rate2}, 2-base-errors reads number: {err_2bases_read_num}")
         else:
             self.logger.error("Input invalid 2-base-errors per read error rate!")
             sys.exit(1)
 
-        err_1base_records = []
-        shared_objects = records_dict, file_type
-        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-            for tmp_rec in pool.imap(self.mutate_seq, err_1_id_lst, progress_bar=self.config.verbose):
-                err_1base_records.append(tmp_rec)
-
-        err_2base_records = []
+        err_records = []
         shared_objects = records_dict, file_type
-        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-            for tmp_rec in pool.imap(self.mutate_2base_seq, err_2_id_lst, progress_bar=self.config.verbose):
-                err_2base_records.append(tmp_rec)
+        if flag1:
+            try:
+                with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+                    for tmp_rec in pool.imap(self.mutate_seq, err_1_id_lst, progress_bar=self.config.verbose):
+                        err_records.append(tmp_rec)
+            except KeyboardInterrupt:
+                # Handle termination signal (Ctrl+C)
+                pool.terminate()  # Terminate the WorkerPool before exiting
+
+            except Exception:
+                # Handle other exceptions
+                pool.terminate()  # Terminate the WorkerPool before exiting
+                raise
+        if flag2:
+            try:
+                with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+                    for tmp_rec in pool.imap(self.mutate_2base_seq, err_2_id_lst, progress_bar=self.config.verbose):
+                        err_records.append(tmp_rec)
+            except KeyboardInterrupt:
+                # Handle termination signal (Ctrl+C)
+                pool.terminate()  # Terminate the WorkerPool before exiting
+
+            except Exception:
+                # Handle other exceptions
+                pool.terminate()  # Terminate the WorkerPool before exiting
+                raise
 
-        err_records = err_1base_records + err_2base_records
         err_subdataset = self.config.result_dir + "err_subdataset" + file_type
         with open(err_subdataset, "w") as handle:
             SeqIO.write(err_records, handle, file_type)
 
         ########################################################################################
         err_free_subdataset = self.config.result_dir + "err_free_subdataset" + file_type
 
-        err_id_lst = err_1_id_lst + err_2_id_lst
-        err_free_id_lst = list(set(select_id_lst) - set(err_id_lst))
-        extract_records(self.config.result_dir, err_free_id_lst, data_set, err_free_subdataset)
-
-        base = self.config.input_file.split("/")[-1]
-        file_name = base.split(file_type)[0]
-        raw_data = self.config.result_dir + "simulated_raw_" + file_name + file_type
-        os.system("cat %s %s > %s" % (err_subdataset, err_free_subdataset, raw_data))
-        ##################################################################################
-        err_free_subdataset_2 = self.config.result_dir + "err_free_subdataset2" + file_type
-        extract_records(self.config.result_dir, err_id_lst, data_set, err_free_subdataset_2)
-        true_data = self.config.result_dir + "simulated_true_" + file_name + file_type  
-        os.system("cat %s %s > %s" % (err_free_subdataset_2, err_free_subdataset, true_data))     
-        return raw_data, true_data
-        
-    ''' 
-    def error_injection(self, data_set):
-        records_dict, file_type = parse_data_dict(data_set)
-        id_lst = list(records_dict.keys())
-        total_seqs_lst = []
-        seq2id_dict = {}
-        for item in id_lst:
-            seq = str(records_dict[item].seq)
-            seq2id_dict.setdefault(seq, []).append(item)
-            total_seqs_lst.append(seq)
-            # total_bases += len(seq)
-            # total_reads += 1
-            
-        read2counts = collections.Counter(total_seqs_lst)
-        select_id_lst = []
-        # total_bases = 0
-        total_reads = 0
-        new_read2counts = {}
-        for read, count in read2counts.items():
-            # if count >= 5:
-            if count > self.config.min_freq:
-                select_id_lst.extend(seq2id_dict[read])
-            if count > self.config.min_read_count:
-                new_read2counts[read] = count
-                total_reads += count
-                # total_bases += len(read) * count
-                
-        # one base error
-        err_1_base_num = round(total_reads * self.config.error_rate1)
-        if total_reads > err_1_base_num:
-            per_num =  err_1_base_num / total_reads
-            err_1_id_lst = []
-            for read, count in new_read2counts.items():
-                random_num = round(count * per_num)
-                name_lst = seq2id_dict[read]
-
-                rng = np.random.default_rng(seed=self.config.sim_seed)
-                indices = rng.permutation(len(name_lst))[:random_num]
-                # print(indices)
-                err_1_id_lst.extend(name_lst[i] for i in indices)
-                # print(err_1_id_lst)
+        if flag1 and flag2:
+            err_id_lst = err_1_id_lst + err_2_id_lst
+        elif flag1 and not flag2:
+            err_id_lst = err_1_id_lst
+        elif not flag1 and flag2:
+            err_id_lst = err_2_id_lst
         else:
-            self.logger.error("1 base error reads number is larger than the total reads number!")
-            sys.exit(1)
-
-        # two base errors
-        if self.config.error_rate2 > 0:
-            err_2_id_lst = []
-            cur_total_reads = total_reads - len(err_1_id_lst)
-            err_2_base_num = round(cur_total_reads * self.config.error_rate2)
-
-            if cur_total_reads > err_2_base_num:
-                per_num_2base =  err_2_base_num / (cur_total_reads * 2)
-                for read, count in new_read2counts.items():
-                    random_num_2base = round(count * per_num_2base)
-                    cur_name_lst = list(set(seq2id_dict[read]) - set(err_1_id_lst))
-
-                    rng = np.random.default_rng(seed=self.config.sim_seed)
-                    indices = rng.permutation(len(cur_name_lst))[:random_num_2base]
-                    err_2_id_lst.extend(cur_name_lst[i] for i in indices)
-                    
-                self.logger.info(f"Total reads: {total_reads}, 1 base error per read error rate: {self.config.error_rate1}, 1 base error reads number: {len(err_1_id_lst)}, 2 bases per read error rate: {self.config.error_rate2}, 2 bases error reads number: {len(err_2_id_lst)}")
-            else:
-                self.logger.error("2 bases error reads number is larger than the total reads number!")
-                sys.exit(1)
-        else:
-            # err_reads_num = round(total_bases * self.config.error_rate / total_reads)
-            self.logger.info(f"Total reads: {total_reads}, 1 base error per read error rate: {self.config.error_rate1}, 1 base error reads number: {len(err_1_id_lst)}")
-        
-        err_1base_records = []
-        shared_objects = records_dict, file_type
-        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-            for tmp_rec in pool.imap(self.mutate_seq, err_1_id_lst, progress_bar=self.config.verbose):
-                err_1base_records.append(tmp_rec)
-
-        err_2base_records = []
-        shared_objects = records_dict, file_type
-        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
-            for tmp_rec in pool.imap(self.mutate_2base_seq, err_2_id_lst, progress_bar=self.config.verbose):
-                err_2base_records.append(tmp_rec)
-
-        err_records = err_1base_records + err_2base_records
-        err_subdataset = self.config.result_dir + "err_subdataset" + file_type
-        with open(err_subdataset, "w") as handle:
-            SeqIO.write(err_records, handle, file_type)
-
-        ########################################################################################
-        err_free_subdataset = self.config.result_dir + "err_free_subdataset" + file_type
-
-        err_id_lst = err_1_id_lst + err_2_id_lst
+            self.logger.error("No error id selected, simulation failed!")
+            sys.exit(1)            
         err_free_id_lst = list(set(select_id_lst) - set(err_id_lst))
         extract_records(self.config.result_dir, err_free_id_lst, data_set, err_free_subdataset)
 
         base = self.config.input_file.split("/")[-1]
         file_name = base.split(file_type)[0]
         raw_data = self.config.result_dir + "simulated_raw_" + file_name + file_type
         os.system("cat %s %s > %s" % (err_subdataset, err_free_subdataset, raw_data))
         ##################################################################################
         err_free_subdataset_2 = self.config.result_dir + "err_free_subdataset2" + file_type
         extract_records(self.config.result_dir, err_id_lst, data_set, err_free_subdataset_2)
         true_data = self.config.result_dir + "simulated_true_" + file_name + file_type  
         os.system("cat %s %s > %s" % (err_free_subdataset_2, err_free_subdataset, true_data))     
         return raw_data, true_data
-    '''
-
-
+    
     def find_first_diff_char(self, string1, string2):
         min_len = min(len(string1), len(string2))
 
         for i in range(min_len):
             if string1[i] != string2[i]:
                 return i
 
@@ -374,64 +288,64 @@
 
         # If both strings are identical
         return -1
 
     def mutate_seq(self, shared_objects, idx):
         records_dict, file_type = shared_objects
         ori_seq = str(records_dict[idx].seq)
-        mutation_seq = self.read2err_read(ori_seq)
+
+        possible_seqs = []
+        possible_seqs.extend(self.seq2substitution(ori_seq))
+
+        num = len(possible_seqs)
+        # random.seed(idx)
+        # Do not set seed here because it can produce the same position errors which is not random, or you can set different seed for different sequence
+        random.shuffle(possible_seqs)
+        ii = random.randint(0, num-1)
+        mutation_seq = possible_seqs[ii]
+
         if file_type == "fastq":
-            # dis = editdistance.eval(ori_seq, mutation_seq)
-            # if dis == 0:
-            #     pass
-            # elif dis == 1:
-            #     indel_idx = self.find_first_diff_char(ori_seq, mutation_seq)
-            #     # Get the quality scores list from letter_annotations
-            #     quality_scores = records_dict[idx].letter_annotations["phred_quality"]
-            #     if len(ori_seq) < len(mutation_seq):
-            #         # Calculate the average score
-            #         min_score = min(quality_scores)
-            #         # Insert the average score at the specified index
-            #         quality_scores.insert(indel_idx, min_score)
-            #         records_dict[idx].letter_annotations["phred_quality"] = quality_scores
-            #     elif len(ori_seq) > len(mutation_seq):
-            #         quality_scores.pop(indel_idx)
-            #         records_dict[idx].letter_annotations["phred_quality"] = quality_scores
-            # else:
-            #     self.logger.error("Generate non 1-base error read.")
-            #     sys.exit(1)
             return SeqRecord(Seq(mutation_seq), id=records_dict[idx].id, description=records_dict[idx].description, letter_annotations=records_dict[idx].letter_annotations)
         elif file_type == "fasta":
             return SeqRecord(Seq(mutation_seq).seq, id=records_dict[idx].id, description=records_dict[idx].description)     
 
     def mutate_2base_seq(self, shared_objects, idx):
         records_dict, file_type = shared_objects
         ori_seq = str(records_dict[idx].seq)
-        mutation_seq = self.read2_2baseerr_read(ori_seq)
+
+        possible_seqs = self.enumerate_ed2_seqs(ori_seq)
+        num = len(possible_seqs)
+        # random.seed(idx)
+        # Do not set seed here because it can produce the same position errors which is not random, or you can set different seed for different sequence
+        random.shuffle(possible_seqs)
+        ii = random.randint(0, num-1)
+        mutation_seq = possible_seqs[ii]
+
         if file_type == "fastq":
             return SeqRecord(Seq(mutation_seq), id=records_dict[idx].id, description=records_dict[idx].description, letter_annotations=records_dict[idx].letter_annotations)
         elif file_type == "fasta":
             return SeqRecord(Seq(mutation_seq).seq, id=records_dict[idx].id, description=records_dict[idx].description)  
 
-    def read2_2baseerr_read(self, read):
-        possible_seqs = self.enumerate_ed2_seqs(read)
-        num = len(possible_seqs)
-        random.seed(self.config.sim_seed)
-        random.shuffle(possible_seqs)
-        idx = random.randint(0, num-1)
-        return possible_seqs[idx]
 
     def enumerate_ed2_seqs(self, read):
         possible_ed1 = seq2substitution(read)
         possible_ed2 = []
         for seq in possible_ed1:
             possible_ed2.extend(list(set(seq2substitution(seq)) - possible_ed1))
         return list(set(possible_ed2))
 
     '''
+    def read2_2baseerr_read(self, read):
+        possible_seqs = self.enumerate_ed2_seqs(read)
+        num = len(possible_seqs)
+        random.seed(self.config.sim_seed)
+        random.shuffle(possible_seqs)
+        idx = random.randint(0, num-1)
+        return possible_seqs[idx]
+        
     def extract_seq(self, shared_objects, name):
         records_dict, file_type = shared_objects
         if file_type == "fastq":
             return SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description, letter_annotations=records_dict[name].letter_annotations)
         elif file_type == "fasta":
             return SeqRecord(records_dict[name].seq, id=records_dict[name].id, description=records_dict[name].description)
 
@@ -445,15 +359,16 @@
                     # print(tmp_rec)
                     sub_records.append(tmp_rec)
                     pbar.update() 
         # print(type(sub_records[0]), sub_records[0])
         with open(sub_dataset, "w") as handle:
             SeqIO.write(sub_records, handle, file_type)
         return 
-
+    '''
+    '''
     def error_injection(self, data_set):
         records_dict, file_type = parse_data_dict(data_set)
         id_lst = list(records_dict.keys())
 
         total_seqs_lst = []
         seq2id_dict = {}
         for item in id_lst:
@@ -473,27 +388,27 @@
                 select_id_lst.extend(seq2id_dict[read])
             if count >= self.config.min_read_count:
                 new_read2counts[read] = count
                 
                 total_reads += count
                 total_bases += len(read) * count
 
-        err_reads_num = round(total_bases * self.config.error_rate)
+        err_reads_num = round(total_bases * self.config.error_rate1)
     
         if total_reads > err_reads_num:
             per_num =  err_reads_num / total_reads
         err_id_lst = []
         for read, count in new_read2counts.items():
             random_num = round(count * per_num)
             name_lst = seq2id_dict[read]
             random.shuffle(name_lst)
             err_id_lst.extend(random.sample(name_lst, random_num))
 
-        # err_reads_num = round(total_bases * self.config.error_rate / total_reads)
-        self.logger.info(f"total bases: {total_bases}, total reads: {total_reads}, error rate: {self.config.error_rate}, calculated error reads number: {err_reads_num}, actual error reads number: {len(err_id_lst)}")
+        # err_reads_num = round(total_bases * self.config.error_rate1 / total_reads)
+        self.logger.info(f"total bases: {total_bases}, total reads: {total_reads}, error rate: {self.config.error_rate1}, calculated error reads number: {err_reads_num}, actual error reads number: {len(err_id_lst)}")
 
         err_subdataset = self.config.result_dir + "err_subdataset" + file_type
         err_records = []
         shared_objects = records_dict, file_type
         with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
             for tmp_rec in pool.imap(self.mutate_seq, err_id_lst, progress_bar=self.config.verbose):
                 err_records.append(tmp_rec)
@@ -519,17 +434,191 @@
         os.system("cat %s %s > %s" % (err_subdataset, err_free_subdataset, raw_data))
         ##################################################################################
         err_free_subdataset_2 = self.config.result_dir + "err_free_subdataset2" + file_type
         extract_records(self.config.result_dir, err_id_lst, data_set, err_free_subdataset_2)
         true_data = self.config.result_dir + "simulated_true_" + file_name + file_type  
         os.system("cat %s %s > %s" % (err_free_subdataset_2, err_free_subdataset, true_data))     
         return raw_data, true_data
+    '''
 
     '''
-    
+    def mutate_seq(self, shared_objects, idx):
+        records_dict, file_type = shared_objects
+        ori_seq = str(records_dict[idx].seq)
+        mutation_seq = self.read2err_read(ori_seq)
+        if file_type == "fastq":
+            # dis = editdistance.eval(ori_seq, mutation_seq)
+            # if dis == 0:
+            #     pass
+            # elif dis == 1:
+            #     indel_idx = self.find_first_diff_char(ori_seq, mutation_seq)
+            #     # Get the quality scores list from letter_annotations
+            #     quality_scores = records_dict[idx].letter_annotations["phred_quality"]
+            #     if len(ori_seq) < len(mutation_seq):
+            #         # Calculate the average score
+            #         min_score = min(quality_scores)
+            #         # Insert the average score at the specified index
+            #         quality_scores.insert(indel_idx, min_score)
+            #         records_dict[idx].letter_annotations["phred_quality"] = quality_scores
+            #     elif len(ori_seq) > len(mutation_seq):
+            #         quality_scores.pop(indel_idx)
+            #         records_dict[idx].letter_annotations["phred_quality"] = quality_scores
+            # else:
+            #     self.logger.error("Generate non 1-base error read.")
+            #     sys.exit(1)
+            return SeqRecord(Seq(mutation_seq), id=records_dict[idx].id, description=records_dict[idx].description, letter_annotations=records_dict[idx].letter_annotations)
+        elif file_type == "fasta":
+            return SeqRecord(Seq(mutation_seq).seq, id=records_dict[idx].id, description=records_dict[idx].description) 
+    '''
+
+    ''' 
+    def error_injection(self, data_set):
+        records_dict, file_type = parse_data_dict(data_set)
+        id_lst = list(records_dict.keys())
+        total_seqs_lst = []
+        seq2id_dict = {}
+        for item in id_lst:
+            seq = str(records_dict[item].seq)
+            seq2id_dict.setdefault(seq, []).append(item)
+            total_seqs_lst.append(seq)
+            # total_bases += len(seq)
+            # total_reads += 1
+            
+        read2counts = collections.Counter(total_seqs_lst)
+        select_id_lst = []
+        # total_bases = 0
+        total_reads = 0
+        new_read2counts = {}
+        for read, count in read2counts.items():
+            # if count >= 5:
+            if count > self.config.min_freq:
+                select_id_lst.extend(seq2id_dict[read])
+            if count > self.config.min_read_count:
+                new_read2counts[read] = count
+                total_reads += count
+                # total_bases += len(read) * count
+                
+        # one base error
+        err_1_base_num = round(total_reads * self.config.error_rate1)
+        if total_reads > err_1_base_num:
+            per_num =  err_1_base_num / total_reads
+            err_1_id_lst = []
+            for read, count in new_read2counts.items():
+                random_num = round(count * per_num)
+                name_lst = seq2id_dict[read]
+
+                rng = np.random.default_rng(seed=self.config.sim_seed)
+                indices = rng.permutation(len(name_lst))[:random_num]
+                # print(indices)
+                err_1_id_lst.extend(name_lst[i] for i in indices)
+                # print(err_1_id_lst)
+        else:
+            self.logger.error("1 base error reads number is larger than the total reads number!")
+            sys.exit(1)
+
+        # two base errors
+        if self.config.error_rate2 > 0:
+            err_2_id_lst = []
+            cur_total_reads = total_reads - len(err_1_id_lst)
+            err_2_base_num = round(cur_total_reads * self.config.error_rate2)
+
+            if cur_total_reads > err_2_base_num:
+                per_num_2base =  err_2_base_num / (cur_total_reads * 2)
+                for read, count in new_read2counts.items():
+                    random_num_2base = round(count * per_num_2base)
+                    cur_name_lst = list(set(seq2id_dict[read]) - set(err_1_id_lst))
+
+                    rng = np.random.default_rng(seed=self.config.sim_seed)
+                    indices = rng.permutation(len(cur_name_lst))[:random_num_2base]
+                    err_2_id_lst.extend(cur_name_lst[i] for i in indices)
+                    
+                self.logger.info(f"Total reads: {total_reads}, 1 base error per read error rate: {self.config.error_rate1}, 1 base error reads number: {len(err_1_id_lst)}, 2 bases per read error rate: {self.config.error_rate2}, 2 bases error reads number: {len(err_2_id_lst)}")
+            else:
+                self.logger.error("2 bases error reads number is larger than the total reads number!")
+                sys.exit(1)
+        else:
+            # err_reads_num = round(total_bases * self.config.error_rate / total_reads)
+            self.logger.info(f"Total reads: {total_reads}, 1 base error per read error rate: {self.config.error_rate1}, 1 base error reads number: {len(err_1_id_lst)}")
+        
+        err_1base_records = []
+        shared_objects = records_dict, file_type
+        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+            for tmp_rec in pool.imap(self.mutate_seq, err_1_id_lst, progress_bar=self.config.verbose):
+                err_1base_records.append(tmp_rec)
+
+        err_2base_records = []
+        shared_objects = records_dict, file_type
+        with WorkerPool(self.config.num_workers, shared_objects=shared_objects, start_method='fork') as pool:
+            for tmp_rec in pool.imap(self.mutate_2base_seq, err_2_id_lst, progress_bar=self.config.verbose):
+                err_2base_records.append(tmp_rec)
+
+        err_records = err_1base_records + err_2base_records
+        err_subdataset = self.config.result_dir + "err_subdataset" + file_type
+        with open(err_subdataset, "w") as handle:
+            SeqIO.write(err_records, handle, file_type)
+
+        ########################################################################################
+        err_free_subdataset = self.config.result_dir + "err_free_subdataset" + file_type
+
+        err_id_lst = err_1_id_lst + err_2_id_lst
+        err_free_id_lst = list(set(select_id_lst) - set(err_id_lst))
+        extract_records(self.config.result_dir, err_free_id_lst, data_set, err_free_subdataset)
+
+        base = self.config.input_file.split("/")[-1]
+        file_name = base.split(file_type)[0]
+        raw_data = self.config.result_dir + "simulated_raw_" + file_name + file_type
+        os.system("cat %s %s > %s" % (err_subdataset, err_free_subdataset, raw_data))
+        ##################################################################################
+        err_free_subdataset_2 = self.config.result_dir + "err_free_subdataset2" + file_type
+        extract_records(self.config.result_dir, err_id_lst, data_set, err_free_subdataset_2)
+        true_data = self.config.result_dir + "simulated_true_" + file_name + file_type  
+        os.system("cat %s %s > %s" % (err_free_subdataset_2, err_free_subdataset, true_data))     
+        return raw_data, true_data
+    '''
+
+    '''
+    total_seqs_lst = []
+    seq2id_dict = {}
+    for item in id_lst:
+        seq = str(records_dict[item].seq)
+        seq2id_dict.setdefault(seq, []).append(item)
+        total_seqs_lst.append(seq)
+        # total_bases += len(seq)
+        # total_reads += 1
+
+    read2counts = collections.Counter(total_seqs_lst)
+    select_id_lst = []
+    total_bases = 0
+    total_reads = 0
+    new_read2counts = {}
+    for read, count in read2counts.items():
+        if count >= 5:
+            select_id_lst.extend(seq2id_dict[read])
+        if count >= self.config.min_read_count:
+            new_read2counts[read] = count
+            
+            total_reads += count
+            total_bases += len(read) * count
+
+    err_reads_num = round(total_bases * self.config.error_rate1)
+
+    if total_reads > err_reads_num:
+        per_num =  err_reads_num / total_reads
+    err_1_id_lst = []
+    for read, count in new_read2counts.items():
+        random_num = round(count * per_num)
+        name_lst = seq2id_dict[read]
+        random.shuffle(name_lst)
+        err_1_id_lst.extend(random.sample(name_lst, random_num))
+
+    # err_reads_num = round(total_bases * self.config.error_rate1 / total_reads)
+    self.logger.info(f"total bases: {total_bases}, total reads: {total_reads}, error rate: {self.config.error_rate1}, calculated error reads number: {err_reads_num}, actual error reads number: {len(err_1_id_lst)}")
+    '''
+
+
 # if __name__ == '__main__':
 #     logger = custom_logger("simulation", debug_mode=True)
 #     input_file = "/home/pping/Data/Repo/data/noise2read_data/group3/SAS-Cov-2/noise2read_result/new_no_ml/output/umi_simulated_raw_original_sars_r1_corrected_correct.fastq"
 #     sim = Simulation(logger, 30, )
 
 #     raw_data, true_data = sim.error_injection(input_file)
 #     output_dir = "/home/pping/Data/Repo/data/noise2read_data/group3/SAS-Cov-2/"
```

### Comparing `noise2read-0.1.3/src/noise2read/umitest.py` & `noise2read-0.1.5/src/noise2read/umitest.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/src/noise2read/utils.py` & `noise2read-0.1.5/src/noise2read/utils.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/src/noise2read.egg-info/PKG-INFO` & `noise2read-0.1.5/src/noise2read.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: noise2read
-Version: 0.1.3
+Version: 0.1.5
 Summary: Turn noise to read
 Home-page: https://github.com/Jappy0/noise2read
 Author: Penagyao Ping
 Author-email: ping.pengyao@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `noise2read-0.1.3/src/noise2read.egg-info/SOURCES.txt` & `noise2read-0.1.5/src/noise2read.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/tests/test_data_generation.py` & `noise2read-0.1.5/tests/test_data_generation.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/tests/test_reads2vector.py` & `noise2read-0.1.5/tests/test_reads2vector.py`

 * *Files identical despite different names*

### Comparing `noise2read-0.1.3/tests/test_utils.py` & `noise2read-0.1.5/tests/test_utils.py`

 * *Files identical despite different names*

