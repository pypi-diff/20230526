# Comparing `tmp/PyLTSpice-4.0.2.tar.gz` & `tmp/PyLTSpice-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\sandbox\PySpice\dist\.tmp-6neuci_y\PyLTSpice-4.0.2.tar", last modified: Sat May 13 07:47:28 2023, max compression
+gzip compressed data, was "C:\sandbox\PySpice\dist\.tmp-mre5943o\PyLTSpice-4.0.3.tar", last modified: Fri May 26 20:02:26 2023, max compression
```

## Comparing `PyLTSpice-4.0.2.tar` & `PyLTSpice-4.0.3.tar`

### file list

```diff
@@ -1,62 +1,61 @@
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.651518 PyLTSpice-4.0.2/
--rw-rw-rw-   0        0        0    35823 2022-12-04 12:18:59.000000 PyLTSpice-4.0.2/LICENSE
--rw-rw-rw-   0        0        0    56683 2023-05-13 07:47:28.650520 PyLTSpice-4.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.544803 PyLTSpice-4.0.2/PyLTSpice/
--rw-rw-rw-   0        0        0     9679 2023-05-12 18:44:35.000000 PyLTSpice-4.0.2/PyLTSpice/Histogram.py
--rw-rw-rw-   0        0        0      362 2023-02-12 22:14:27.000000 PyLTSpice-4.0.2/PyLTSpice/LTSpiceBatch.py
--rw-rw-rw-   0        0        0      333 2023-02-12 22:14:27.000000 PyLTSpice-4.0.2/PyLTSpice/LTSpice_RawRead.py
--rw-rw-rw-   0        0        0      332 2023-02-12 22:14:27.000000 PyLTSpice-4.0.2/PyLTSpice/LTSpice_RawWrite.py
--rw-rw-rw-   0        0        0     6615 2023-05-12 19:45:12.000000 PyLTSpice-4.0.2/PyLTSpice/LTSteps.py
--rw-rw-rw-   0        0        0      337 2023-04-30 19:07:01.000000 PyLTSpice-4.0.2/PyLTSpice/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.570733 PyLTSpice-4.0.2/PyLTSpice/client_server/
--rw-rw-rw-   0        0        0        0 2023-04-08 17:08:22.000000 PyLTSpice-4.0.2/PyLTSpice/client_server/__init__.py
--rw-rw-rw-   0        0        0     8400 2023-04-19 21:29:58.000000 PyLTSpice-4.0.2/PyLTSpice/client_server/sim_client.py
--rw-rw-rw-   0        0        0     5427 2023-04-23 11:45:04.000000 PyLTSpice-4.0.2/PyLTSpice/client_server/sim_server.py
--rw-rw-rw-   0        0        0     4737 2023-04-23 11:45:04.000000 PyLTSpice-4.0.2/PyLTSpice/client_server/srv_sim_runner.py
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.578712 PyLTSpice-4.0.2/PyLTSpice/log/
--rw-rw-rw-   0        0        0        0 2023-04-08 22:49:34.000000 PyLTSpice-4.0.2/PyLTSpice/log/__init__.py
--rw-rw-rw-   0        0        0    29860 2023-02-23 16:46:29.000000 PyLTSpice-4.0.2/PyLTSpice/log/ltsteps.py
--rw-rw-rw-   0        0        0     6047 2023-04-30 22:25:50.000000 PyLTSpice-4.0.2/PyLTSpice/log/semi_dev_op_reader.py
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.591678 PyLTSpice-4.0.2/PyLTSpice/raw/
--rw-rw-rw-   0        0        0        0 2023-04-08 22:49:18.000000 PyLTSpice-4.0.2/PyLTSpice/raw/__init__.py
--rw-rw-rw-   0        0        0    14667 2023-04-30 20:34:58.000000 PyLTSpice-4.0.2/PyLTSpice/raw/raw_classes.py
--rw-rw-rw-   0        0        0     5609 2023-04-30 17:57:03.000000 PyLTSpice-4.0.2/PyLTSpice/raw/raw_convert.py
--rw-rw-rw-   0        0        0    36025 2023-05-13 07:43:03.000000 PyLTSpice-4.0.2/PyLTSpice/raw/raw_read.py
--rw-rw-rw-   0        0        0    16752 2023-04-30 22:29:26.000000 PyLTSpice-4.0.2/PyLTSpice/raw/raw_write.py
--rw-rw-rw-   0        0        0     4236 2023-05-12 20:33:51.000000 PyLTSpice-4.0.2/PyLTSpice/rawplot.py
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.626584 PyLTSpice-4.0.2/PyLTSpice/sim/
--rw-rw-rw-   0        0        0        0 2023-02-12 22:11:29.000000 PyLTSpice-4.0.2/PyLTSpice/sim/__init__.py
--rw-rw-rw-   0        0        0     8568 2023-04-30 18:47:14.000000 PyLTSpice-4.0.2/PyLTSpice/sim/ltspice_simulator.py
--rw-rw-rw-   0        0        0     4636 2023-04-26 20:04:46.000000 PyLTSpice-4.0.2/PyLTSpice/sim/ngspice_simulator.py
--rw-rw-rw-   0        0        0     1505 2023-04-23 16:20:26.000000 PyLTSpice-4.0.2/PyLTSpice/sim/process_callback.py
--rw-rw-rw-   0        0        0     6059 2023-04-23 21:06:11.000000 PyLTSpice-4.0.2/PyLTSpice/sim/run_task.py
--rw-rw-rw-   0        0        0     4809 2023-04-26 21:05:36.000000 PyLTSpice-4.0.2/PyLTSpice/sim/sim_analysis.py
--rw-rw-rw-   0        0        0    10749 2023-04-23 14:18:49.000000 PyLTSpice-4.0.2/PyLTSpice/sim/sim_batch.py
--rw-rw-rw-   0        0        0    23686 2023-04-30 18:47:14.000000 PyLTSpice-4.0.2/PyLTSpice/sim/sim_runner.py
--rw-rw-rw-   0        0        0     9221 2023-04-26 21:05:36.000000 PyLTSpice-4.0.2/PyLTSpice/sim/sim_stepping.py
--rw-rw-rw-   0        0        0     4652 2023-04-08 19:00:33.000000 PyLTSpice-4.0.2/PyLTSpice/sim/simulator.py
--rw-rw-rw-   0        0        0    46608 2023-04-30 22:25:50.000000 PyLTSpice-4.0.2/PyLTSpice/sim/spice_editor.py
--rw-rw-rw-   0        0        0     7384 2023-04-07 13:28:50.000000 PyLTSpice-4.0.2/PyLTSpice/sim/xyce_simulator.py
--rw-rw-rw-   0        0        0    21705 2023-05-13 07:43:03.000000 PyLTSpice-4.0.2/PyLTSpice/sim_batch.py
--rw-rw-rw-   0        0        0    10037 2023-05-13 07:43:03.000000 PyLTSpice-4.0.2/PyLTSpice/simulator.py
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.634563 PyLTSpice-4.0.2/PyLTSpice/utils/
--rw-rw-rw-   0        0        0     2935 2023-05-12 19:51:10.000000 PyLTSpice-4.0.2/PyLTSpice/utils/detect_encoding.py
--rw-rw-rw-   0        0        0    11563 2023-01-15 18:28:54.000000 PyLTSpice-4.0.2/PyLTSpice/utils/sweep_iterators.py
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.559763 PyLTSpice-4.0.2/PyLTSpice.egg-info/
--rw-rw-rw-   0        0        0    56683 2023-05-13 07:47:28.000000 PyLTSpice-4.0.2/PyLTSpice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1384 2023-05-13 07:47:28.000000 PyLTSpice-4.0.2/PyLTSpice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-13 07:47:28.000000 PyLTSpice-4.0.2/PyLTSpice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      165 2023-05-13 07:47:28.000000 PyLTSpice-4.0.2/PyLTSpice.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-05-13 07:47:28.000000 PyLTSpice-4.0.2/PyLTSpice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       41 2023-05-13 07:47:28.000000 PyLTSpice-4.0.2/PyLTSpice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14902 2023-05-13 07:38:52.000000 PyLTSpice-4.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.637555 PyLTSpice-4.0.2/doc/
--rw-rw-rw-   0        0        0     2448 2023-01-15 08:45:40.000000 PyLTSpice-4.0.2/doc/conf.py
--rw-rw-rw-   0        0        0     1193 2023-05-13 07:38:52.000000 PyLTSpice-4.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-13 07:47:28.651518 PyLTSpice-4.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.640547 PyLTSpice-4.0.2/tests/
--rw-rw-rw-   0        0        0      801 2023-04-23 17:09:47.000000 PyLTSpice-4.0.2/tests/test_ltsteps.py
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.644536 PyLTSpice-4.0.2/tests/unittest/
-drwxrwxrwx   0        0        0        0 2023-05-13 07:47:28.646532 PyLTSpice-4.0.2/tests/unittest/sweep_iterators/
--rw-rw-rw-   0        0        0     6014 2023-02-23 17:53:15.000000 PyLTSpice-4.0.2/tests/unittest/sweep_iterators/sweep_iterators_unittest.py
--rw-rw-rw-   0        0        0    19227 2023-05-13 07:43:03.000000 PyLTSpice-4.0.2/tests/unittest/test_pyltspice.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.906688 PyLTSpice-4.0.3/
+-rw-rw-rw-   0        0        0    35823 2022-12-04 12:18:59.000000 PyLTSpice-4.0.3/LICENSE
+-rw-rw-rw-   0        0        0    56816 2023-05-26 20:02:26.904687 PyLTSpice-4.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.750594 PyLTSpice-4.0.3/PyLTSpice/
+-rw-rw-rw-   0        0        0     9679 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/Histogram.py
+-rw-rw-rw-   0        0        0      362 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/LTSpiceBatch.py
+-rw-rw-rw-   0        0        0      333 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/LTSpice_RawRead.py
+-rw-rw-rw-   0        0        0      332 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/LTSpice_RawWrite.py
+-rw-rw-rw-   0        0        0     6609 2023-05-26 19:49:19.000000 PyLTSpice-4.0.3/PyLTSpice/LTSteps.py
+-rw-rw-rw-   0        0        0      293 2023-05-14 19:17:53.000000 PyLTSpice-4.0.3/PyLTSpice/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.790504 PyLTSpice-4.0.3/PyLTSpice/client_server/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/client_server/__init__.py
+-rw-rw-rw-   0        0        0     8400 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/client_server/sim_client.py
+-rw-rw-rw-   0        0        0     5427 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/client_server/sim_server.py
+-rw-rw-rw-   0        0        0     4737 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/client_server/srv_sim_runner.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.801686 PyLTSpice-4.0.3/PyLTSpice/log/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/log/__init__.py
+-rw-rw-rw-   0        0        0    29860 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/log/ltsteps.py
+-rw-rw-rw-   0        0        0     6047 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/log/semi_dev_op_reader.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.826656 PyLTSpice-4.0.3/PyLTSpice/raw/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/raw/__init__.py
+-rw-rw-rw-   0        0        0    14667 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/raw/raw_classes.py
+-rw-rw-rw-   0        0        0     5609 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/raw/raw_convert.py
+-rw-rw-rw-   0        0        0    36030 2023-05-26 19:50:13.000000 PyLTSpice-4.0.3/PyLTSpice/raw/raw_read.py
+-rw-rw-rw-   0        0        0    16752 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/raw/raw_write.py
+-rw-rw-rw-   0        0        0     4014 2023-05-14 19:17:53.000000 PyLTSpice-4.0.3/PyLTSpice/rawplot.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.873530 PyLTSpice-4.0.3/PyLTSpice/sim/
+-rw-rw-rw-   0        0        0        0 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/__init__.py
+-rw-rw-rw-   0        0        0     8568 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/ltspice_simulator.py
+-rw-rw-rw-   0        0        0     4636 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/ngspice_simulator.py
+-rw-rw-rw-   0        0        0     1505 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/process_callback.py
+-rw-rw-rw-   0        0        0     6059 2023-05-26 19:50:13.000000 PyLTSpice-4.0.3/PyLTSpice/sim/run_task.py
+-rw-rw-rw-   0        0        0     4809 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/sim_analysis.py
+-rw-rw-rw-   0        0        0    10749 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/sim_batch.py
+-rw-rw-rw-   0        0        0    23686 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/sim_runner.py
+-rw-rw-rw-   0        0        0     9221 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/sim_stepping.py
+-rw-rw-rw-   0        0        0     4652 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/simulator.py
+-rw-rw-rw-   0        0        0    46631 2023-05-26 14:01:10.000000 PyLTSpice-4.0.3/PyLTSpice/sim/spice_editor.py
+-rw-rw-rw-   0        0        0     7384 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim/xyce_simulator.py
+-rw-rw-rw-   0        0        0    21705 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/sim_batch.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.881748 PyLTSpice-4.0.3/PyLTSpice/utils/
+-rw-rw-rw-   0        0        0     2935 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/utils/detect_encoding.py
+-rw-rw-rw-   0        0        0    11563 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/PyLTSpice/utils/sweep_iterators.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.774837 PyLTSpice-4.0.3/PyLTSpice.egg-info/
+-rw-rw-rw-   0        0        0    56816 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1361 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      165 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       25 2023-05-26 20:02:26.000000 PyLTSpice-4.0.3/PyLTSpice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    15035 2023-05-26 20:01:44.000000 PyLTSpice-4.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.886779 PyLTSpice-4.0.3/doc/
+-rw-rw-rw-   0        0        0     2448 2023-05-14 19:17:07.000000 PyLTSpice-4.0.3/doc/conf.py
+-rw-rw-rw-   0        0        0     1193 2023-05-26 19:59:48.000000 PyLTSpice-4.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 20:02:26.906688 PyLTSpice-4.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.890724 PyLTSpice-4.0.3/tests/
+-rw-rw-rw-   0        0        0      801 2023-05-14 19:17:08.000000 PyLTSpice-4.0.3/tests/test_ltsteps.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.893716 PyLTSpice-4.0.3/tests/unittest/
+drwxrwxrwx   0        0        0        0 2023-05-26 20:02:26.899701 PyLTSpice-4.0.3/tests/unittest/sweep_iterators/
+-rw-rw-rw-   0        0        0     6014 2023-05-14 19:17:08.000000 PyLTSpice-4.0.3/tests/unittest/sweep_iterators/sweep_iterators_unittest.py
+-rw-rw-rw-   0        0        0    19227 2023-05-14 19:17:08.000000 PyLTSpice-4.0.3/tests/unittest/test_pyltspice.py
```

### Comparing `PyLTSpice-4.0.2/LICENSE` & `PyLTSpice-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PKG-INFO` & `PyLTSpice-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 4.0.2
+Version: 4.0.3
 Summary: A set of tools to Automate LTSpice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -954,14 +954,18 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.3\
+  Fixing issue in elapsed time calculation.
+  Fixing issue with the import of LTSpiceLogReader from LTSteps.py
+
 * Version 4.0.2\
   Changing list of Library dependencies.
 
 * Version 4.0.1\
   Bug fix on CLI for the Histogram.py and LTSteps.py
 
 * Version 4.0.0\
```

### Comparing `PyLTSpice-4.0.2/PyLTSpice/Histogram.py` & `PyLTSpice-4.0.3/PyLTSpice/Histogram.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/LTSteps.py` & `PyLTSpice-4.0.3/PyLTSpice/LTSteps.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,10 +149,10 @@
             else:
                 # just reformats
                 data = LTSpiceLogReader(filename)
             data.split_complex_values_on_datasets()
             data.export_data(fname_out)
             data.export_data(fname_out)
 
-    # input("Press Enter to Continue")
 
-main()
+if __name__ == "__main__":
+    main()
```

### Comparing `PyLTSpice-4.0.2/PyLTSpice/client_server/sim_client.py` & `PyLTSpice-4.0.3/PyLTSpice/client_server/sim_client.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/client_server/sim_server.py` & `PyLTSpice-4.0.3/PyLTSpice/client_server/sim_server.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/client_server/srv_sim_runner.py` & `PyLTSpice-4.0.3/PyLTSpice/client_server/srv_sim_runner.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/log/ltsteps.py` & `PyLTSpice-4.0.3/PyLTSpice/log/ltsteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/log/semi_dev_op_reader.py` & `PyLTSpice-4.0.3/PyLTSpice/log/semi_dev_op_reader.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/raw/raw_classes.py` & `PyLTSpice-4.0.3/PyLTSpice/raw/raw_classes.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/raw/raw_convert.py` & `PyLTSpice-4.0.3/PyLTSpice/raw/raw_convert.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/raw/raw_read.py` & `PyLTSpice-4.0.3/PyLTSpice/raw/raw_read.py`

 * *Files 0% similar despite different names*

```diff
@@ -354,15 +354,15 @@
         'Operating Point',
         'Transient Analysis',
         'Transfer Function',
         'Noise Spectral Density',
         'Frequency Response Analysis',
     )
 
-    def __init__(self, raw_filename: str, traces_to_read: Union[str, List[str], Tuple[str], None] = '*', **kwargs):
+    def __init__(self, raw_filename: str, traces_to_read: Union[str, List[str], Tuple[str, ...], None] = '*', **kwargs):
         self.verbose = kwargs.get('verbose', True)
         raw_filename = Path(raw_filename)
         if traces_to_read is not None:
             assert isinstance(traces_to_read, (str, list, tuple)), "traces_to_read must be a string, a list or None"
 
         raw_file_size = os.stat(raw_filename).st_size  # Get the file size in order to know the data size
         raw_file = open(raw_filename, "rb")
```

### Comparing `PyLTSpice-4.0.2/PyLTSpice/raw/raw_write.py` & `PyLTSpice-4.0.3/PyLTSpice/raw/raw_write.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/rawplot.py` & `PyLTSpice-4.0.3/PyLTSpice/rawplot.py`

 * *Files 20% similar despite different names*

```diff
@@ -22,32 +22,37 @@
 
 from PyLTSpice import RawRead
 
 
 def main():
     """Uses matplotlib to plot the data in the raw file"""
     import sys
+    import matplotlib
     import matplotlib.pyplot as plt
     import os
     from os.path import split as path_split
     from os.path import join as path_join
-    from numpy import abs as mag
+    from numpy import abs as mag, angle as phase_np
 
     def what_to_units(whattype):
         """Determines the unit to display on the plot Y axis"""
         if 'voltage' in whattype:
             return 'V'
         if 'current' in whattype:
             return 'A'
 
     directory = os.getcwd()
+    matplotlib.use('wxagg')
 
     if len(sys.argv) > 2:
         raw_filename = sys.argv[1]
         trace_names = sys.argv[2:]
+    elif len(sys.argv) > 1:
+        raw_filename = sys.argv[1]
+        trace_names = '*'  # All traces
     else:
         print("Usage: rawplot.py RAW_FILE TRACE_NAME")
         print("TRACE_NAME is the traces to plot")
         sys.exit(-1)
 
     LTR = RawRead(raw_filename, trace_names, verbose=True)
     for param, value in LTR.raw_params.items():
@@ -60,65 +65,54 @@
     traces = [LTR.get_trace(trace) for trace in trace_names]
     if LTR.axis is not None:
         steps_data = LTR.get_steps()
     else:
         steps_data = [0]
     print("Steps read are :", list(steps_data))
 
-    if 'complex' in LTR.flags:
-        n_axis = len(traces) * 2
-    else:
-        n_axis = len(traces)
+    n_axis = len(traces)
 
     fig, axis_set = plt.subplots(nrows=n_axis, ncols=1, sharex='all')
-    write_labels = True
+
+    if n_axis == 1:
+        axis_set = [axis_set]  # Needs to have a list of axis
 
     for i, trace in enumerate(traces):
-        if 'complex' in LTR.flags:
-            axis_set = axis_set[2 * i: 2 * i + 2]  # Returns two axis
-        else:
-            if n_axis == 1:
-                axis_set = [axis_set]  # Needs to return a list
-            else:
-                axis_set = axis_set[i:i + 1]  # Returns just one axis but enclosed in a list
-        magnitude = True
-        for ax in axis_set:
-            ax.grid(True)
-            if 'log' in LTR.flags:
-                ax.set_xscale('log')
-            for step_i in steps_data:
-                if LTR.axis:
-                    x = LTR.get_axis(step_i)
-                else:
-                    x = arange(LTR.nPoints)
-                y = traces[i].get_wave(step_i)
-                if 'complex' in LTR.flags:
-                    x = mag(x)
-                    if magnitude:
-                        ax.set_yscale('log')
-                        y = mag(y)
-                    else:
-                        y = angle(y, deg=True)
-                if write_labels:
-                    ax.plot(x, y, label=str(steps_data[step_i]))
-                else:
-                    ax.plot(x, y)
-            write_labels = False
+        ax = axis_set[i]
 
+        ax.grid(True)
+        if 'log' in LTR.flags:
+            ax.set_xscale('log')
+        for step_i in steps_data:
+            if LTR.axis:
+                x = LTR.get_axis(step_i)
+            else:
+                x = arange(LTR.nPoints)
+            y = traces[i].get_wave(step_i)
+            label = f"{trace.name}:{steps_data[step_i]})"
             if 'complex' in LTR.flags:
-                if magnitude:
-                    title = f"{trace.name} Mag [db{what_to_units(trace.whattype)}]"
-                    magnitude = False
-                else:
-                    title = f"{trace.name} Phase [deg]"
+                x = mag(x)
+                ax.set_yscale('log')
+                y = mag(y)
+                ax.yaxis.label.set_color('blue')
+                ax.set(ylabel=label+'(dB)')
+                ax.plot(x, y)
+                ax_phase = ax.twinx()
+                y = phase_np(y, deg=True)
+                ax_phase.plot(x, y, color='red', linestyle='-.')
+                ax_phase.yaxis.label.set_color('red')
+                ax_phase.set(ylabel=label+'Phase (o)')
+                # title = f"{trace.name} Phase [deg]"
+                # ax.set_title(title)
             else:
-                title = f"{trace.name} [{what_to_units(trace.whattype)}]"
-            ax.set_title(title)
-
-    plt.figlegend()
+                ax.plot(x, y)
+                ax.set(ylabel=label)
+                # title = f"{trace.name} [{what_to_units(trace.whattype)}]"
+                # ax.set_title(title)
+    fig.tight_layout()
     plt.show()
 '''
 '''
 # out = open("RAW_TEST_out_test1.txt", 'w')
 #
 # for step in LTR.get_steps():
 #     for x in range(len(LTR[0].data)):
```

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/ltspice_simulator.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/ltspice_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/ngspice_simulator.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/ngspice_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/process_callback.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/process_callback.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/run_task.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/run_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 from .simulator import Simulator
 
 END_LINE_TERM = '\n'
 
 logging.basicConfig(filename='SpiceBatch.log', level=logging.INFO)
 
 if sys.version_info.major >= 3 and sys.version_info.minor >= 6:
-    clock_function = time.process_time
+    clock_function = time.perf_counter
 else:
     clock_function = time.clock
 
 
 class RunTask(threading.Thread):
     """This is an internal Class and should not be used directly by the User."""
```

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/sim_analysis.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/sim_analysis.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/sim_batch.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/sim_batch.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/sim_runner.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/sim_runner.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/sim_stepping.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/sim_stepping.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/simulator.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/spice_editor.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/spice_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -976,17 +976,17 @@
         self.modified_subcircuits.clear()
         if self.netlist_file.exists():
             with self.netlist_file.open('r', encoding=self.encoding, errors='replace') as f:
                 lines = iter(f)  # Creates an iterator object to consume the file
                 finished = self._add_lines(lines)
                 if not finished:
                     raise SyntaxError("Netlist with missing .END or .ENDS statements")
-                else:
-                    for remainig_lines in lines:
-                        print("Ignoring %s" % remainig_lines)
+                # else:
+                #     for _ in lines:  # Consuming the rest of the file.
+                #         pass  # print("Ignoring %s" % _)
         else:
             self.logger.error("Netlist file not found")
 
     @staticmethod
     def find_subckt_in_lib(library, subckt_name) -> Union['SpiceCircuit', None]:
         """
         Finds returns a Subckt from a library file.
```

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim/xyce_simulator.py` & `PyLTSpice-4.0.3/PyLTSpice/sim/xyce_simulator.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/sim_batch.py` & `PyLTSpice-4.0.3/PyLTSpice/sim_batch.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/utils/detect_encoding.py` & `PyLTSpice-4.0.3/PyLTSpice/utils/detect_encoding.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice/utils/sweep_iterators.py` & `PyLTSpice-4.0.3/PyLTSpice/utils/sweep_iterators.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/PyLTSpice.egg-info/PKG-INFO` & `PyLTSpice-4.0.3/PyLTSpice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyLTSpice
-Version: 4.0.2
+Version: 4.0.3
 Summary: A set of tools to Automate LTSpice simulations
 Author-email: Nuno Brum <me@nunobrum.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -954,14 +954,18 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.3\
+  Fixing issue in elapsed time calculation.
+  Fixing issue with the import of LTSpiceLogReader from LTSteps.py
+
 * Version 4.0.2\
   Changing list of Library dependencies.
 
 * Version 4.0.1\
   Bug fix on CLI for the Histogram.py and LTSteps.py
 
 * Version 4.0.0\
```

### Comparing `PyLTSpice-4.0.2/PyLTSpice.egg-info/SOURCES.txt` & `PyLTSpice-4.0.3/PyLTSpice.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 PyLTSpice/LTSpiceBatch.py
 PyLTSpice/LTSpice_RawRead.py
 PyLTSpice/LTSpice_RawWrite.py
 PyLTSpice/LTSteps.py
 PyLTSpice/__init__.py
 PyLTSpice/rawplot.py
 PyLTSpice/sim_batch.py
-PyLTSpice/simulator.py
 PyLTSpice.egg-info/PKG-INFO
 PyLTSpice.egg-info/SOURCES.txt
 PyLTSpice.egg-info/dependency_links.txt
 PyLTSpice.egg-info/entry_points.txt
 PyLTSpice.egg-info/requires.txt
 PyLTSpice.egg-info/top_level.txt
 PyLTSpice/client_server/__init__.py
```

### Comparing `PyLTSpice-4.0.2/README.md` & `PyLTSpice-4.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -265,14 +265,18 @@
 ## To whom do I talk to? ##
 
 * Tools website : [https://www.nunobrum.com/pyltspice.html](https://www.nunobrum.com/pyltspice.html)
 * Repo owner : [me@nunobrum.com](me@nunobrum.com)
 * Alternative contact : nuno.brum@gmail.com
 
 ## History ##
+* Version 4.0.3\
+  Fixing issue in elapsed time calculation.
+  Fixing issue with the import of LTSpiceLogReader from LTSteps.py
+
 * Version 4.0.2\
   Changing list of Library dependencies.
 
 * Version 4.0.1\
   Bug fix on CLI for the Histogram.py and LTSteps.py
 
 * Version 4.0.0\
```

### Comparing `PyLTSpice-4.0.2/doc/conf.py` & `PyLTSpice-4.0.3/doc/conf.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/pyproject.toml` & `PyLTSpice-4.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 [project]
 name = "PyLTSpice"
-version = "4.0.2"
+version = "4.0.3"
 authors = [
   { name="Nuno Brum", email="me@nunobrum.com" },
 ]
 description = "A set of tools to Automate LTSpice simulations"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `PyLTSpice-4.0.2/tests/test_ltsteps.py` & `PyLTSpice-4.0.3/tests/test_ltsteps.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/tests/unittest/sweep_iterators/sweep_iterators_unittest.py` & `PyLTSpice-4.0.3/tests/unittest/sweep_iterators/sweep_iterators_unittest.py`

 * *Files identical despite different names*

### Comparing `PyLTSpice-4.0.2/tests/unittest/test_pyltspice.py` & `PyLTSpice-4.0.3/tests/unittest/test_pyltspice.py`

 * *Files identical despite different names*

