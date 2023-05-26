# Comparing `tmp/my_provider-0.1.3.tar.gz` & `tmp/my_provider-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/my_provider-0.1.3.tar", last modified: Fri May 26 07:43:15 2023, max compression
+gzip compressed data, was "my_provider-0.1.4.tar", last modified: Fri May 26 08:13:46 2023, max compression
```

## Comparing `my_provider-0.1.3.tar` & `my_provider-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,19 @@
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:43:15.000000 my_provider-0.1.3/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 07:43:15.000000 my_provider-0.1.3/PKG-INFO
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider/
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider/operators/
--rw-r--r--   0 huangzheng   (501) staff       (20)      524 2023-05-26 06:59:16.000000 my_provider-0.1.3/my_provider/operators/my_operator.py
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my_provider-0.1.3/my_provider/operators/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     2681 2023-05-26 07:32:07.000000 my_provider-0.1.3/my_provider/operators/dlc_operator.py
--rw-r--r--   0 huangzheng   (501) staff       (20)      283 2023-05-26 06:59:16.000000 my_provider-0.1.3/my_provider/__init__.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider/hooks/
--rw-r--r--   0 huangzheng   (501) staff       (20)      299 2023-05-11 12:30:07.000000 my_provider-0.1.3/my_provider/hooks/my_hook.py
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my_provider-0.1.3/my_provider/hooks/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     7738 2023-05-26 07:27:32.000000 my_provider-0.1.3/my_provider/hooks/dlc_hook.py
--rw-r--r--   0 huangzheng   (501) staff       (20)      355 2023-05-26 07:43:13.000000 my_provider-0.1.3/setup.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider.egg-info/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider.egg-info/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)      442 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider.egg-info/SOURCES.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       53 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider.egg-info/entry_points.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       64 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider.egg-info/requires.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider.egg-info/top_level.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-26 07:43:15.000000 my_provider-0.1.3/my_provider.egg-info/dependency_links.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-26 07:43:15.000000 my_provider-0.1.3/setup.cfg
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 08:13:46.125814 my_provider-0.1.4/
+-rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-26 08:13:46.125543 my_provider-0.1.4/PKG-INFO
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 08:13:46.120869 my_provider-0.1.4/my_provider/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      186 2023-05-26 08:13:15.000000 my_provider-0.1.4/my_provider/__init__.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 08:13:46.123896 my_provider-0.1.4/my_provider/hooks/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my_provider-0.1.4/my_provider/hooks/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     7738 2023-05-26 07:27:32.000000 my_provider-0.1.4/my_provider/hooks/dlc_hook.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 08:13:46.124868 my_provider-0.1.4/my_provider/operators/
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my_provider-0.1.4/my_provider/operators/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     2665 2023-05-26 08:13:15.000000 my_provider-0.1.4/my_provider/operators/dlc_operator.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 08:13:46.123265 my_provider-0.1.4/my_provider.egg-info/
+-rw-r--r--   0 huangzheng   (501) staff       (20)       55 2023-05-26 08:13:46.000000 my_provider-0.1.4/my_provider.egg-info/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)      376 2023-05-26 08:13:46.000000 my_provider-0.1.4/my_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-26 08:13:46.000000 my_provider-0.1.4/my_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       52 2023-05-26 08:13:46.000000 my_provider-0.1.4/my_provider.egg-info/entry_points.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       64 2023-05-26 08:13:46.000000 my_provider-0.1.4/my_provider.egg-info/requires.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       12 2023-05-26 08:13:46.000000 my_provider-0.1.4/my_provider.egg-info/top_level.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-26 08:13:46.125898 my_provider-0.1.4/setup.cfg
+-rw-r--r--   0 huangzheng   (501) staff       (20)      355 2023-05-26 08:13:34.000000 my_provider-0.1.4/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `my_provider-0.1.3/my_provider/operators/dlc_operator.py` & `my_provider-0.1.4/my_provider/operators/dlc_operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any
 
 from airflow.models.baseoperator import BaseOperator
 from airflow.utils.context import Context
-from my_provider_top.my_provider.hooks.dlc_hook import DLCHook
+from my_provider.hooks.dlc_hook import DLCHook
 import logging
 LOG = logging.getLogger(__name__)
 
 
 class DLCOperator(BaseOperator):
     def __init__(
             self,
```

### Comparing `my_provider-0.1.3/my_provider/hooks/dlc_hook.py` & `my_provider-0.1.4/my_provider/hooks/dlc_hook.py`

 * *Files identical despite different names*

