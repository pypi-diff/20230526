# Comparing `tmp/vbarongdatools001-0.0.1.tar.gz` & `tmp/vbarongdatools001-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbarongdatools001-0.0.1.tar", last modified: Fri May 26 09:22:15 2023, max compression
+gzip compressed data, was "vbarongdatools001-0.0.2.tar", last modified: Fri May 26 10:09:53 2023, max compression
```

## Comparing `vbarongdatools001-0.0.1.tar` & `vbarongdatools001-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 09:22:15.692748 vbarongdatools001-0.0.1/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 vbarongdatools001-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 vbarongdatools001-0.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0      397 2023-05-26 09:22:15.692748 vbarongdatools001-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 vbarongdatools001-0.0.1/README.md
--rw-rw-rw-   0        0        0      136 2023-05-26 09:22:15.693719 vbarongdatools001-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      969 2023-05-26 09:21:53.000000 vbarongdatools001-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:22:15.671718 vbarongdatools001-0.0.1/vbarongdatools001/
-drwxrwxrwx   0        0        0        0 2023-05-26 09:22:15.684745 vbarongdatools001-0.0.1/vbarongdatools001/Function/
--rw-rw-rw-   0        0        0   470528 2023-04-28 06:08:00.000000 vbarongdatools001-0.0.1/vbarongdatools001/Function/MkdirFunction.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 vbarongdatools001-0.0.1/vbarongdatools001/Function/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:22:15.690751 vbarongdatools001-0.0.1/vbarongdatools001/Ui/
--rw-rw-rw-   0        0        0    40448 2023-04-28 06:06:04.000000 vbarongdatools001-0.0.1/vbarongdatools001/Ui/MaskWin.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 vbarongdatools001-0.0.1/vbarongdatools001/Ui/__init__.py
--rw-rw-rw-   0        0        0    71680 2023-04-28 06:08:08.000000 vbarongdatools001-0.0.1/vbarongdatools001/Ui/mkdirUi.pyd
--rw-rw-rw-   0        0        0        0 2023-03-01 06:05:54.000000 vbarongdatools001-0.0.1/vbarongdatools001/__init__.py
--rw-rw-rw-   0        0        0   146944 2023-05-25 02:07:26.000000 vbarongdatools001-0.0.1/vbarongdatools001/makeDirs.pyd
-drwxrwxrwx   0        0        0        0 2023-05-26 09:22:15.678718 vbarongdatools001-0.0.1/vbarongdatools001.egg-info/
--rw-rw-rw-   0        0        0      397 2023-05-26 09:22:15.000000 vbarongdatools001-0.0.1/vbarongdatools001.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      460 2023-05-26 09:22:15.000000 vbarongdatools001-0.0.1/vbarongdatools001.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 09:22:15.000000 vbarongdatools001-0.0.1/vbarongdatools001.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-05-26 09:22:15.000000 vbarongdatools001-0.0.1/vbarongdatools001.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 10:09:53.069659 vbarongdatools001-0.0.2/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 vbarongdatools001-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 vbarongdatools001-0.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      397 2023-05-26 10:09:53.069659 vbarongdatools001-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 vbarongdatools001-0.0.2/README.md
+-rw-rw-rw-   0        0        0      136 2023-05-26 10:09:53.070549 vbarongdatools001-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      969 2023-05-26 10:09:45.000000 vbarongdatools001-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 10:09:53.066547 vbarongdatools001-0.0.2/vbarongdatools001.egg-info/
+-rw-rw-rw-   0        0        0      397 2023-05-26 10:09:53.000000 vbarongdatools001-0.0.2/vbarongdatools001.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-26 10:09:53.000000 vbarongdatools001-0.0.2/vbarongdatools001.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 10:09:53.000000 vbarongdatools001-0.0.2/vbarongdatools001.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 10:09:53.000000 vbarongdatools001-0.0.2/vbarongdatools001.egg-info/top_level.txt
```

### Comparing `vbarongdatools001-0.0.1/LICENSE.txt` & `vbarongdatools001-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `vbarongdatools001-0.0.1/setup.py` & `vbarongdatools001-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
-PATCH = 1
+PATCH = 2
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "vbarongdatools001",
```

