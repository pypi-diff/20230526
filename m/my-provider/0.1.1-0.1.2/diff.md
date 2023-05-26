# Comparing `tmp/my_provider-0.1.1.tar.gz` & `tmp/my_provider-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/my_provider-0.1.1.tar", last modified: Fri May 26 03:32:02 2023, max compression
+gzip compressed data, was "dist/my_provider-0.1.2.tar", last modified: Fri May 26 07:01:24 2023, max compression
```

## Comparing `my_provider-0.1.1.tar` & `my_provider-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:32:02.000000 my_provider-0.1.1/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 03:32:02.000000 my_provider-0.1.1/PKG-INFO
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:32:02.000000 my_provider-0.1.1/operators/
--rw-r--r--   0 huangzheng   (501) staff       (20)      508 2023-05-11 12:35:18.000000 my_provider-0.1.1/operators/my_operator.py
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my_provider-0.1.1/operators/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     2615 2023-05-25 10:56:20.000000 my_provider-0.1.1/operators/dlc_operator.py
--rw-r--r--   0 huangzheng   (501) staff       (20)      355 2023-05-26 03:31:34.000000 my_provider-0.1.1/setup.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:32:02.000000 my_provider-0.1.1/hooks/
--rw-r--r--   0 huangzheng   (501) staff       (20)      299 2023-05-11 12:30:07.000000 my_provider-0.1.1/hooks/my_hook.py
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my_provider-0.1.1/hooks/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     7290 2023-05-25 10:01:16.000000 my_provider-0.1.1/hooks/dlc_hook.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)      346 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/SOURCES.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       53 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/entry_points.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       64 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/requires.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       16 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/top_level.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/dependency_links.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-26 03:32:02.000000 my_provider-0.1.1/setup.cfg
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:01:24.000000 my_provider-0.1.2/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 07:01:24.000000 my_provider-0.1.2/PKG-INFO
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider/
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider/operators/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      524 2023-05-26 06:59:16.000000 my_provider-0.1.2/my_provider/operators/my_operator.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my_provider-0.1.2/my_provider/operators/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     2591 2023-05-26 06:59:16.000000 my_provider-0.1.2/my_provider/operators/dlc_operator.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      283 2023-05-26 06:59:16.000000 my_provider-0.1.2/my_provider/__init__.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider/hooks/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      299 2023-05-11 12:30:07.000000 my_provider-0.1.2/my_provider/hooks/my_hook.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my_provider-0.1.2/my_provider/hooks/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     7290 2023-05-25 10:01:16.000000 my_provider-0.1.2/my_provider/hooks/dlc_hook.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      355 2023-05-26 06:59:53.000000 my_provider-0.1.2/setup.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider.egg-info/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider.egg-info/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)      442 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       53 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider.egg-info/entry_points.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       64 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider.egg-info/requires.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider.egg-info/top_level.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-26 07:01:24.000000 my_provider-0.1.2/my_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-26 07:01:24.000000 my_provider-0.1.2/setup.cfg
```

### Comparing `my_provider-0.1.1/operators/dlc_operator.py` & `my_provider-0.1.2/my_provider/operators/dlc_operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Any
 
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.context import Context
-from my_provider.hooks.dlc_hook import DLCHook
-from airflow.models import TaskInstance
+from my_provider_top.my_provider.hooks.dlc_hook import DLCHook
 import logging
 LOG = logging.getLogger(__name__)
 
 
 class DLCOperator(BaseOperator):
     def __init__(
             self,
```

### Comparing `my_provider-0.1.1/hooks/dlc_hook.py` & `my_provider-0.1.2/my_provider/hooks/dlc_hook.py`

 * *Files identical despite different names*

