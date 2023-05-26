# Comparing `tmp/PyShoreVolume-1.0.2.tar.gz` & `tmp/PyShoreVolume-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyShoreVolume-1.0.2.tar", last modified: Sat May 20 11:39:49 2023, max compression
+gzip compressed data, was "PyShoreVolume-1.0.3.tar", last modified: Fri May 26 16:27:29 2023, max compression
```

## Comparing `PyShoreVolume-1.0.2.tar` & `PyShoreVolume-1.0.3.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-20 11:39:49.743554 PyShoreVolume-1.0.2/
--rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-20 11:39:49.743645 PyShoreVolume-1.0.2/PKG-INFO
--rw-r--r--   0 owenjames   (501) staff       (20)    15186 2023-04-27 16:59:49.000000 PyShoreVolume-1.0.2/README.txt
--rw-r--r--   0 owenjames   (501) staff       (20)      117 2023-05-20 11:39:49.744169 PyShoreVolume-1.0.2/setup.cfg
--rw-r--r--   0 owenjames   (501) staff       (20)     2579 2023-05-20 11:39:13.000000 PyShoreVolume-1.0.2/setup.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-20 11:39:49.721693 PyShoreVolume-1.0.2/src/
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-20 11:39:49.726483 PyShoreVolume-1.0.2/src/PyShoreVolume/
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-20 11:39:49.728109 PyShoreVolume-1.0.2/src/PyShoreVolume/CleanandTransectLocator/
--rw-r--r--   0 owenjames   (501) staff       (20)     6705 2023-04-26 16:01:36.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5970 2023-04-26 14:58:53.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py
--rw-r--r--   0 owenjames   (501) staff       (20)      258 2023-04-26 10:05:08.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/CleanandTransectLocator/__init__.py
--rw-r--r--   0 owenjames   (501) staff       (20)     3355 2023-05-02 13:07:00.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/DOD1.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5508 2023-05-02 13:08:54.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/DataImportandTransectDefinition1.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-20 11:39:49.737635 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/
--rw-r--r--   0 owenjames   (501) staff       (20)    28792 2023-05-10 13:13:01.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/End Point Rate.jpg
--rw-r--r--   0 owenjames   (501) staff       (20)     1197 2023-05-17 14:53:48.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/File_Organisation_Script.py
--rw-r--r--   0 owenjames   (501) staff       (20)        5 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Intersections2.cpg
--rw-r--r--   0 owenjames   (501) staff       (20)   853906 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Intersections2.dbf
--rw-r--r--   0 owenjames   (501) staff       (20)      417 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Intersections2.prj
--rw-r--r--   0 owenjames   (501) staff       (20)    36528 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Intersections2.shp
--rw-r--r--   0 owenjames   (501) staff       (20)    10508 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Intersections2.shx
--rw-r--r--   0 owenjames   (501) staff       (20)   236652 2023-05-09 10:01:48.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/NetShorelineMovementErosionandAccretion.jpg
--rw-r--r--   0 owenjames   (501) staff       (20)     1587 2023-05-17 14:54:14.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/QGISMergedShoreline.py
--rw-r--r--   0 owenjames   (501) staff       (20)        5 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Transect1.cpg
--rw-r--r--   0 owenjames   (501) staff       (20)     6261 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Transect1.dbf
--rw-r--r--   0 owenjames   (501) staff       (20)      417 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Transect1.prj
--rw-r--r--   0 owenjames   (501) staff       (20)     7756 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Transect1.shp
--rw-r--r--   0 owenjames   (501) staff       (20)      796 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Transect1.shx
--rw-r--r--   0 owenjames   (501) staff       (20)        0 2023-05-01 13:34:09.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/__init__.py
--rw-r--r--   0 owenjames   (501) staff       (20)    32234 2023-05-10 13:13:01.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/eprresults.pkl
--rw-r--r--   0 owenjames   (501) staff       (20)     9487 2023-05-08 13:42:46.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/lrrdictionary.pkl
--rw-r--r--   0 owenjames   (501) staff       (20)   224924 2023-05-09 10:09:18.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/netshorelinemovement.jpg
--rw-r--r--   0 owenjames   (501) staff       (20)    21751 2023-05-08 13:43:15.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/nsm.pkl
--rw-r--r--   0 owenjames   (501) staff       (20)    21748 2023-05-08 13:42:54.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/scedic.pkl
--rw-r--r--   0 owenjames   (501) staff       (20)   235175 2023-05-09 10:02:52.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/shorleinechangeenvelope.jpg
--rwxr--r--   0 owenjames   (501) staff       (20)     1806 2023-05-02 13:05:10.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/SCA1.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-20 11:39:49.740076 PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/
--rw-r--r--   0 owenjames   (501) staff       (20)    11033 2023-05-03 09:55:00.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/EPR.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5629 2023-04-26 16:11:01.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/LRR.py
--rw-r--r--   0 owenjames   (501) staff       (20)     7972 2023-05-19 17:58:28.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/NSM.py
--rw-r--r--   0 owenjames   (501) staff       (20)     9638 2023-05-03 10:00:49.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/NSMEandA.py
--rw-r--r--   0 owenjames   (501) staff       (20)     7935 2023-05-03 07:48:32.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/SCE.py
--rw-r--r--   0 owenjames   (501) staff       (20)      181 2023-03-22 20:35:05.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/__init__.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-20 11:39:49.743259 PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/
--rw-r--r--   0 owenjames   (501) staff       (20)    15278 2023-05-03 10:08:13.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/DEMofDifference.py
--rw-r--r--   0 owenjames   (501) staff       (20)     6106 2023-05-03 09:06:39.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/DODSubPlot.py
--rw-r--r--   0 owenjames   (501) staff       (20)     1772 2023-05-03 09:26:29.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/MaskingDEM.py
--rw-r--r--   0 owenjames   (501) staff       (20)     3219 2023-04-28 12:05:59.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py
--rw-r--r--   0 owenjames   (501) staff       (20)    11070 2023-05-03 09:27:46.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py
--rw-r--r--   0 owenjames   (501) staff       (20)    73653 2023-05-03 09:50:15.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py
--rw-r--r--   0 owenjames   (501) staff       (20)      458 2023-04-28 10:20:21.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/__init__.py
--rw-r--r--   0 owenjames   (501) staff       (20)      236 2023-05-02 14:03:43.000000 PyShoreVolume-1.0.2/src/PyShoreVolume/__init__.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-20 11:39:49.727241 PyShoreVolume-1.0.2/src/PyShoreVolume.egg-info/
--rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-20 11:39:49.000000 PyShoreVolume-1.0.2/src/PyShoreVolume.egg-info/PKG-INFO
--rw-r--r--   0 owenjames   (501) staff       (20)     2036 2023-05-20 11:39:49.000000 PyShoreVolume-1.0.2/src/PyShoreVolume.egg-info/SOURCES.txt
--rw-r--r--   0 owenjames   (501) staff       (20)        1 2023-05-20 11:39:49.000000 PyShoreVolume-1.0.2/src/PyShoreVolume.egg-info/dependency_links.txt
--rw-r--r--   0 owenjames   (501) staff       (20)      256 2023-05-20 11:39:49.000000 PyShoreVolume-1.0.2/src/PyShoreVolume.egg-info/requires.txt
--rw-r--r--   0 owenjames   (501) staff       (20)       59 2023-05-20 11:39:49.000000 PyShoreVolume-1.0.2/src/PyShoreVolume.egg-info/top_level.txt
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.533633 PyShoreVolume-1.0.3/
+-rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-26 16:27:29.533757 PyShoreVolume-1.0.3/PKG-INFO
+-rw-r--r--   0 owenjames   (501) staff       (20)    15186 2023-04-27 16:59:49.000000 PyShoreVolume-1.0.3/README.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)      117 2023-05-26 16:27:29.534273 PyShoreVolume-1.0.3/setup.cfg
+-rw-r--r--   0 owenjames   (501) staff       (20)     2579 2023-05-26 16:23:37.000000 PyShoreVolume-1.0.3/setup.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.513538 PyShoreVolume-1.0.3/src/
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.515344 PyShoreVolume-1.0.3/src/PyShoreVolume/
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.516743 PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/
+-rw-r--r--   0 owenjames   (501) staff       (20)     6705 2023-04-26 16:01:36.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5970 2023-04-26 14:58:53.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      258 2023-04-26 10:05:08.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/__init__.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     3355 2023-05-02 13:07:00.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/DOD1.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5508 2023-05-02 13:08:54.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/DataImportandTransectDefinition1.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.528368 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/
+-rw-r--r--   0 owenjames   (501) staff       (20)    28792 2023-05-10 13:13:01.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/End Point Rate.jpg
+-rw-r--r--   0 owenjames   (501) staff       (20)     1197 2023-05-17 14:53:48.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/File_Organisation_Script.py
+-rw-r--r--   0 owenjames   (501) staff       (20)        5 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.cpg
+-rw-r--r--   0 owenjames   (501) staff       (20)   853906 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.dbf
+-rw-r--r--   0 owenjames   (501) staff       (20)      417 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.prj
+-rw-r--r--   0 owenjames   (501) staff       (20)    36528 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.shp
+-rw-r--r--   0 owenjames   (501) staff       (20)    10508 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.shx
+-rw-r--r--   0 owenjames   (501) staff       (20)   236652 2023-05-09 10:01:48.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/NetShorelineMovementErosionandAccretion.jpg
+-rw-r--r--   0 owenjames   (501) staff       (20)     1587 2023-05-17 14:54:14.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/QGISMergedShoreline.py
+-rw-r--r--   0 owenjames   (501) staff       (20)        5 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.cpg
+-rw-r--r--   0 owenjames   (501) staff       (20)     6261 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.dbf
+-rw-r--r--   0 owenjames   (501) staff       (20)      417 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.prj
+-rw-r--r--   0 owenjames   (501) staff       (20)     7756 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.shp
+-rw-r--r--   0 owenjames   (501) staff       (20)      796 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.shx
+-rw-r--r--   0 owenjames   (501) staff       (20)        0 2023-05-01 13:34:09.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/__init__.py
+-rw-r--r--   0 owenjames   (501) staff       (20)    32234 2023-05-10 13:13:01.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/eprresults.pkl
+-rw-r--r--   0 owenjames   (501) staff       (20)     9487 2023-05-08 13:42:46.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/lrrdictionary.pkl
+-rw-r--r--   0 owenjames   (501) staff       (20)   224924 2023-05-09 10:09:18.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/netshorelinemovement.jpg
+-rw-r--r--   0 owenjames   (501) staff       (20)    21751 2023-05-08 13:43:15.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/nsm.pkl
+-rw-r--r--   0 owenjames   (501) staff       (20)    21748 2023-05-08 13:42:54.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/scedic.pkl
+-rw-r--r--   0 owenjames   (501) staff       (20)   235175 2023-05-09 10:02:52.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/shorleinechangeenvelope.jpg
+-rwxr--r--   0 owenjames   (501) staff       (20)     1806 2023-05-02 13:05:10.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/SCA1.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.531320 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/
+-rw-r--r--   0 owenjames   (501) staff       (20)    11033 2023-05-03 09:55:00.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/EPR.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5629 2023-04-26 16:11:01.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/LRR.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     7895 2023-05-26 14:52:49.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/NSM.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     9638 2023-05-03 10:00:49.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/NSMEandA.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     7935 2023-05-03 07:48:32.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/SCE.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      181 2023-03-22 20:35:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/__init__.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.533328 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/
+-rw-r--r--   0 owenjames   (501) staff       (20)    15278 2023-05-03 10:08:13.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/DEMofDifference.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     6106 2023-05-03 09:06:39.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/DODSubPlot.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     1772 2023-05-03 09:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/MaskingDEM.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     3219 2023-04-28 12:05:59.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py
+-rw-r--r--   0 owenjames   (501) staff       (20)    11070 2023-05-03 09:27:46.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py
+-rw-r--r--   0 owenjames   (501) staff       (20)    73653 2023-05-03 09:50:15.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      458 2023-04-28 10:20:21.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/__init__.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      236 2023-05-02 14:03:43.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/__init__.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.516101 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/
+-rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/PKG-INFO
+-rw-r--r--   0 owenjames   (501) staff       (20)     2036 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/SOURCES.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)        1 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/dependency_links.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)      256 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/requires.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)       59 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/top_level.txt
```

### Comparing `PyShoreVolume-1.0.2/PKG-INFO` & `PyShoreVolume-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShoreVolume
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Based Shoreline Change and Beach Volume Analysis Tool
 Home-page: https://github.com/owencaseyjames/PyShoreVolume
 Author: Owen Casey James
 Author-email: owen.james@kcl.ac.uk
 License: MIT
 Keywords: Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyShoreVolume-1.0.2/README.txt` & `PyShoreVolume-1.0.3/README.txt`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/setup.py` & `PyShoreVolume-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='PyShoreVolume',
-      version ='1.0.2',
+      version ='1.0.3',
       description ='Python Based Shoreline Change and Beach Volume Analysis Tool',
       author ='Owen Casey James',
       author_email = 'owen.james@kcl.ac.uk',
       licence ='MIT',
       keywords = 'Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR',
       long_description=long_description,
       long_description_content_type='text/markdown',
```

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/DOD1.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/DOD1.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/DataImportandTransectDefinition1.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/DataImportandTransectDefinition1.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/End Point Rate.jpg` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/End Point Rate.jpg`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/File_Organisation_Script.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/File_Organisation_Script.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Intersections2.dbf` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.dbf`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Intersections2.shp` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.shp`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Intersections2.shx` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.shx`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/NetShorelineMovementErosionandAccretion.jpg` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/NetShorelineMovementErosionandAccretion.jpg`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/QGISMergedShoreline.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/QGISMergedShoreline.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Transect1.dbf` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.dbf`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Transect1.shp` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.shp`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/Transect1.shx` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.shx`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/eprresults.pkl` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/eprresults.pkl`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/lrrdictionary.pkl` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/lrrdictionary.pkl`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/netshorelinemovement.jpg` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/netshorelinemovement.jpg`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/nsm.pkl` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/nsm.pkl`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/scedic.pkl` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/scedic.pkl`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/Extra/shorleinechangeenvelope.jpg` & `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/shorleinechangeenvelope.jpg`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/SCA1.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/SCA1.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/EPR.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/EPR.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/LRR.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/LRR.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/NSM.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/NSM.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,16 +35,14 @@
 
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib import cm
 from matplotlib.colors import LinearSegmentedColormap
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from matplotlib.lines import Line2D
-import matplotlib_scalebar
-from matplotlib_scalebar.scalebar import ScaleBar
 
 import contextily as ctx
 
 import pyproj
 
 import time
```

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/NSMEandA.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/NSMEandA.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/ShorelineChange/SCE.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/SCE.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/DEMofDifference.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/DEMofDifference.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/DODSubPlot.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/DODSubPlot.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/MaskingDEM.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/MaskingDEM.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py` & `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume.egg-info/PKG-INFO` & `PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShoreVolume
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python Based Shoreline Change and Beach Volume Analysis Tool
 Home-page: https://github.com/owencaseyjames/PyShoreVolume
 Author: Owen Casey James
 Author-email: owen.james@kcl.ac.uk
 License: MIT
 Keywords: Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyShoreVolume-1.0.2/src/PyShoreVolume.egg-info/SOURCES.txt` & `PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/SOURCES.txt`

 * *Files identical despite different names*

