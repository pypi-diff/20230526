# Comparing `tmp/maboss-0.8.4.tar.gz` & `tmp/maboss-0.8.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maboss-0.8.4.tar", last modified: Sat Dec 31 06:50:36 2022, max compression
+gzip compressed data, was "maboss-0.8.5.tar", last modified: Fri May 26 15:39:57 2023, max compression
```

## Comparing `maboss-0.8.4.tar` & `maboss-0.8.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.548639 maboss-0.8.4/
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-12-31 06:50:31.000000 maboss-0.8.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      246 2022-12-31 06:50:36.548639 maboss-0.8.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      816 2022-12-31 06:50:31.000000 maboss-0.8.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.544639 maboss-0.8.4/maboss/
--rw-r--r--   0 runner    (1001) docker     (122)      657 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2127 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/bnetsimulation.py
--rw-r--r--   0 runner    (1001) docker     (122)     3788 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/cmabossresult.py
--rw-r--r--   0 runner    (1001) docker     (122)     3273 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/cmabossresult2.py
--rw-r--r--   0 runner    (1001) docker     (122)     1388 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/cmabosssimulation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.544639 maboss-0.8.4/maboss/ensemble/
--rw-r--r--   0 runner    (1001) docker     (122)       65 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    16773 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/ensemble/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (122)    28638 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/ensemble/result.py
--rw-r--r--   0 runner    (1001) docker     (122)     4205 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/figures.py
--rw-r--r--   0 runner    (1001) docker     (122)     9899 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/gsparser.py
--rw-r--r--   0 runner    (1001) docker     (122)      376 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/logic.py
--rw-r--r--   0 runner    (1001) docker     (122)    10604 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/network.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.544639 maboss-0.8.4/maboss/pipelines/
--rw-r--r--   0 runner    (1001) docker     (122)     4478 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4005 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/result.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.544639 maboss-0.8.4/maboss/results/
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/results/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6479 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/results/baseresult.py
--rw-r--r--   0 runner    (1001) docker     (122)     2309 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/results/finalresult.py
--rw-r--r--   0 runner    (1001) docker     (122)    14183 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/results/probtrajresult.py
--rw-r--r--   0 runner    (1001) docker     (122)     8776 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/results/statdistresult.py
--rw-r--r--   0 runner    (1001) docker     (122)      902 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/results/storedresult.py
--rw-r--r--   0 runner    (1001) docker     (122)     3298 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/sbmlcmabossresult.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/sbmlsimulation.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.548639 maboss-0.8.4/maboss/server/
--rw-r--r--   0 runner    (1001) docker     (122)       32 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1452 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/server/atexit.py
--rw-r--r--   0 runner    (1001) docker     (122)     4731 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/server/client.py
--rw-r--r--   0 runner    (1001) docker     (122)     7274 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/server/comm.py
--rw-r--r--   0 runner    (1001) docker     (122)     3377 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/server/result.py
--rw-r--r--   0 runner    (1001) docker     (122)    15058 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/simulation.py
--rw-r--r--   0 runner    (1001) docker     (122)      901 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.548639 maboss-0.8.4/maboss/upp/
--rw-r--r--   0 runner    (1001) docker     (122)       78 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/upp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    24138 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/upp/cmaboss_results.py
--rw-r--r--   0 runner    (1001) docker     (122)    25318 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/upp/results.py
--rw-r--r--   0 runner    (1001) docker     (122)     7971 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/upp/upp.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.548639 maboss-0.8.4/maboss/widgets/
--rw-r--r--   0 runner    (1001) docker     (122)       66 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/widgets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1827 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/widgets/ipywidgets.py
--rw-r--r--   0 runner    (1001) docker     (122)     1588 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss/widgets/menu.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.544639 maboss-0.8.4/maboss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      246 2022-12-31 06:50:36.000000 maboss-0.8.4/maboss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1126 2022-12-31 06:50:36.000000 maboss-0.8.4/maboss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-12-31 06:50:36.000000 maboss-0.8.4/maboss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       95 2022-12-31 06:50:36.000000 maboss-0.8.4/maboss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       20 2022-12-31 06:50:36.000000 maboss-0.8.4/maboss.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)      245 2022-12-31 06:50:31.000000 maboss-0.8.4/maboss_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-12-31 06:50:36.548639 maboss-0.8.4/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (122)     1147 2022-12-31 06:50:31.000000 maboss-0.8.4/scripts/MBSS_FormatTable.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      825 2022-12-31 06:50:31.000000 maboss-0.8.4/scripts/UpPMaBoSS.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-12-31 06:50:36.548639 maboss-0.8.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)      733 2022-12-31 06:50:31.000000 maboss-0.8.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.891361 maboss-0.8.5/
+-rw-r--r--   0 runner    (1001) docker     (122)       67 2023-05-26 15:39:51.000000 maboss-0.8.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-26 15:39:57.891361 maboss-0.8.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      816 2023-05-26 15:39:51.000000 maboss-0.8.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.887361 maboss-0.8.5/maboss/
+-rw-r--r--   0 runner    (1001) docker     (122)      657 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2127 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/bnetsimulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3788 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/cmabossresult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3273 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/cmabossresult2.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1388 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/cmabosssimulation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.887361 maboss-0.8.5/maboss/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (122)       65 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16773 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/ensemble/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (122)    28638 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/ensemble/result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4205 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/figures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9899 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/gsparser.py
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/logic.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10604 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/network.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.887361 maboss-0.8.5/maboss/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (122)     4478 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4005 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/result.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.887361 maboss-0.8.5/maboss/results/
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/results/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/results/baseresult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2309 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/results/finalresult.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14183 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/results/probtrajresult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8776 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/results/statdistresult.py
+-rw-r--r--   0 runner    (1001) docker     (122)      902 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/results/storedresult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3298 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/sbmlcmabossresult.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/sbmlsimulation.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.887361 maboss-0.8.5/maboss/server/
+-rw-r--r--   0 runner    (1001) docker     (122)       32 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1452 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/server/atexit.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4731 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/server/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7274 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/server/comm.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3377 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/server/result.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15119 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      901 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.887361 maboss-0.8.5/maboss/upp/
+-rw-r--r--   0 runner    (1001) docker     (122)       78 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/upp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24138 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/upp/cmaboss_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25323 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/upp/results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7971 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/upp/upp.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.887361 maboss-0.8.5/maboss/widgets/
+-rw-r--r--   0 runner    (1001) docker     (122)       66 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1827 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/widgets/ipywidgets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1588 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss/widgets/menu.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.887361 maboss-0.8.5/maboss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      246 2023-05-26 15:39:57.000000 maboss-0.8.5/maboss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1126 2023-05-26 15:39:57.000000 maboss-0.8.5/maboss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 15:39:57.000000 maboss-0.8.5/maboss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       95 2023-05-26 15:39:57.000000 maboss-0.8.5/maboss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       20 2023-05-26 15:39:57.000000 maboss-0.8.5/maboss.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      245 2023-05-26 15:39:51.000000 maboss-0.8.5/maboss_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 15:39:57.891361 maboss-0.8.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (122)     1147 2023-05-26 15:39:51.000000 maboss-0.8.5/scripts/MBSS_FormatTable.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)      825 2023-05-26 15:39:51.000000 maboss-0.8.5/scripts/UpPMaBoSS.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 15:39:57.891361 maboss-0.8.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      733 2023-05-26 15:39:51.000000 maboss-0.8.5/setup.py
```

### Comparing `maboss-0.8.4/README.md` & `maboss-0.8.5/README.md`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/__init__.py` & `maboss-0.8.5/maboss/__init__.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/bnetsimulation.py` & `maboss-0.8.5/maboss/bnetsimulation.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/cmabossresult.py` & `maboss-0.8.5/maboss/cmabossresult.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/cmabossresult2.py` & `maboss-0.8.5/maboss/cmabossresult2.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/cmabosssimulation.py` & `maboss-0.8.5/maboss/cmabosssimulation.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/ensemble/ensemble.py` & `maboss-0.8.5/maboss/ensemble/ensemble.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/ensemble/result.py` & `maboss-0.8.5/maboss/ensemble/result.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/figures.py` & `maboss-0.8.5/maboss/figures.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/gsparser.py` & `maboss-0.8.5/maboss/gsparser.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/network.py` & `maboss-0.8.5/maboss/network.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/pipelines/__init__.py` & `maboss-0.8.5/maboss/pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/result.py` & `maboss-0.8.5/maboss/result.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/results/baseresult.py` & `maboss-0.8.5/maboss/results/baseresult.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/results/finalresult.py` & `maboss-0.8.5/maboss/results/finalresult.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/results/probtrajresult.py` & `maboss-0.8.5/maboss/results/probtrajresult.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/results/statdistresult.py` & `maboss-0.8.5/maboss/results/statdistresult.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/results/storedresult.py` & `maboss-0.8.5/maboss/results/storedresult.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/sbmlcmabossresult.py` & `maboss-0.8.5/maboss/sbmlcmabossresult.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/sbmlsimulation.py` & `maboss-0.8.5/maboss/sbmlsimulation.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/server/atexit.py` & `maboss-0.8.5/maboss/server/atexit.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/server/client.py` & `maboss-0.8.5/maboss/server/client.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/server/comm.py` & `maboss-0.8.5/maboss/server/comm.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/server/result.py` & `maboss-0.8.5/maboss/server/result.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/simulation.py` & `maboss-0.8.5/maboss/simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
                 print("Warning: unused parameter %s" % p, file=stderr)
 
     def copy(self):
         new_network = self.network.copy()
         result = Simulation(new_network, self.param, palette=self.palette)
         if self.mutations:
             result.mutations = self.mutations.copy()
+            result.mutationTypes = self.mutationTypes.copy()
         return result
 
     def check(self, command=None):
 
         try:
             path = tempfile.mkdtemp()
             cfg_fd, cfg_path = tempfile.mkstemp(dir=path, suffix='.cfg')
```

### Comparing `maboss-0.8.4/maboss/ui.py` & `maboss-0.8.5/maboss/ui.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/upp/cmaboss_results.py` & `maboss-0.8.5/maboss/upp/cmaboss_results.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/upp/results.py` & `maboss-0.8.5/maboss/upp/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,16 +40,16 @@
 
             for folder in sorted(glob.glob("%s/Step_*/" % self.workdir)):
                 step = os.path.basename(folder[0:-1]).split("_")[-1]
                 self.results[int(step)] = StoredResult(folder)
 
             self.pop_ratios = pd.read_csv(
                 os.path.join(self.workdir, "PopRatios.csv"),
-                index_col=0, squeeze=True
-            ) / self.uppModel.base_ratio
+                index_col=0
+            ).squeeze("columns") / self.uppModel.base_ratio
 
             if previous_run:
                 # Load the previous run final state
                 _get_next_condition_from_trajectory(previous_run, self.uppModel.model, step=previous_run_step)
 
         else:
             if workdir is not None:
```

### Comparing `maboss-0.8.4/maboss/upp/upp.py` & `maboss-0.8.5/maboss/upp/upp.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/widgets/ipywidgets.py` & `maboss-0.8.5/maboss/widgets/ipywidgets.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss/widgets/menu.py` & `maboss-0.8.5/maboss/widgets/menu.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/maboss.egg-info/SOURCES.txt` & `maboss-0.8.5/maboss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/scripts/MBSS_FormatTable.py` & `maboss-0.8.5/scripts/MBSS_FormatTable.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/scripts/UpPMaBoSS.py` & `maboss-0.8.5/scripts/UpPMaBoSS.py`

 * *Files identical despite different names*

### Comparing `maboss-0.8.4/setup.py` & `maboss-0.8.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 optional_contextlib = []
 if version_info[0] < 3:
     optional_contextlib.append("contextlib2")
 
 setup(name='maboss',
-    version="0.8.4",
+    version="0.8.5",
     packages=find_packages(exclude=["test"]),
     py_modules = ["maboss_setup"],
     author="Nicolas Levy",
     author_email="nicolaspierrelevy@gmail.com",
     description="A python and jupyter API for the MaBoSS software",
     install_requires = [
         "colomoto_jupyter >=0.4.10",
```

