# Comparing `tmp/my_provider-0.1.0.tar.gz` & `tmp/my_provider-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/my_provider-0.1.0.tar", last modified: Fri May 26 03:16:14 2023, max compression
+gzip compressed data, was "dist/my_provider-0.1.1.tar", last modified: Fri May 26 03:32:02 2023, max compression
```

## Comparing `my_provider-0.1.0.tar` & `my_provider-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:16:14.000000 my_provider-0.1.0/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 03:16:14.000000 my_provider-0.1.0/PKG-INFO
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:16:14.000000 my_provider-0.1.0/operators/
--rw-r--r--   0 huangzheng   (501) staff       (20)      508 2023-05-11 12:35:18.000000 my_provider-0.1.0/operators/my_operator.py
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my_provider-0.1.0/operators/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     2615 2023-05-25 10:56:20.000000 my_provider-0.1.0/operators/dlc_operator.py
--rw-r--r--   0 huangzheng   (501) staff       (20)      301 2023-05-26 03:15:39.000000 my_provider-0.1.0/setup.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:16:14.000000 my_provider-0.1.0/hooks/
--rw-r--r--   0 huangzheng   (501) staff       (20)      299 2023-05-11 12:30:07.000000 my_provider-0.1.0/hooks/my_hook.py
--rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my_provider-0.1.0/hooks/__init__.py
--rw-r--r--   0 huangzheng   (501) staff       (20)     7290 2023-05-25 10:01:16.000000 my_provider-0.1.0/hooks/dlc_hook.py
-drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:16:14.000000 my_provider-0.1.0/my_provider.egg-info/
--rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 03:16:14.000000 my_provider-0.1.0/my_provider.egg-info/PKG-INFO
--rw-r--r--   0 huangzheng   (501) staff       (20)      346 2023-05-26 03:16:14.000000 my_provider-0.1.0/my_provider.egg-info/SOURCES.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       53 2023-05-26 03:16:14.000000 my_provider-0.1.0/my_provider.egg-info/entry_points.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       22 2023-05-26 03:16:14.000000 my_provider-0.1.0/my_provider.egg-info/requires.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       16 2023-05-26 03:16:14.000000 my_provider-0.1.0/my_provider.egg-info/top_level.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-26 03:16:14.000000 my_provider-0.1.0/my_provider.egg-info/dependency_links.txt
--rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-26 03:16:14.000000 my_provider-0.1.0/setup.cfg
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:32:02.000000 my_provider-0.1.1/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 03:32:02.000000 my_provider-0.1.1/PKG-INFO
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:32:02.000000 my_provider-0.1.1/operators/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      508 2023-05-11 12:35:18.000000 my_provider-0.1.1/operators/my_operator.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:27.000000 my_provider-0.1.1/operators/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     2615 2023-05-25 10:56:20.000000 my_provider-0.1.1/operators/dlc_operator.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)      355 2023-05-26 03:31:34.000000 my_provider-0.1.1/setup.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:32:02.000000 my_provider-0.1.1/hooks/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      299 2023-05-11 12:30:07.000000 my_provider-0.1.1/hooks/my_hook.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)        0 2023-05-10 03:24:15.000000 my_provider-0.1.1/hooks/__init__.py
+-rw-r--r--   0 huangzheng   (501) staff       (20)     7290 2023-05-25 10:01:16.000000 my_provider-0.1.1/hooks/dlc_hook.py
+drwxr-xr-x   0 huangzheng   (501) staff       (20)        0 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/
+-rw-r--r--   0 huangzheng   (501) staff       (20)      185 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/PKG-INFO
+-rw-r--r--   0 huangzheng   (501) staff       (20)      346 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       53 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/entry_points.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       64 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/requires.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       16 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/top_level.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)        1 2023-05-26 03:32:02.000000 my_provider-0.1.1/my_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 huangzheng   (501) staff       (20)       38 2023-05-26 03:32:02.000000 my_provider-0.1.1/setup.cfg
```

### Comparing `my_provider-0.1.0/operators/dlc_operator.py` & `my_provider-0.1.1/operators/dlc_operator.py`

 * *Files identical despite different names*

### Comparing `my_provider-0.1.0/hooks/dlc_hook.py` & `my_provider-0.1.1/hooks/dlc_hook.py`

 * *Files identical despite different names*

