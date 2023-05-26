# Comparing `tmp/at-fetch-data-1.0.4.tar.gz` & `tmp/at-fetch-data-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "at-fetch-data-1.0.4.tar", last modified: Fri May 26 03:52:13 2023, max compression
+gzip compressed data, was "at-fetch-data-1.0.5.tar", last modified: Fri May 26 04:02:39 2023, max compression
```

## Comparing `at-fetch-data-1.0.4.tar` & `at-fetch-data-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 03:52:13.167279 at-fetch-data-1.0.4/
--rw-r--r--   0 ctw        (501) staff       (20)      904 2023-05-26 03:52:13.167139 at-fetch-data-1.0.4/PKG-INFO
--rw-r--r--   0 ctw        (501) staff       (20)      742 2023-05-23 12:38:22.000000 at-fetch-data-1.0.4/README.md
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 03:52:13.166209 at-fetch-data-1.0.4/at_fetch_data.egg-info/
--rw-r--r--   0 ctw        (501) staff       (20)      904 2023-05-26 03:52:12.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/PKG-INFO
--rw-r--r--   0 ctw        (501) staff       (20)      250 2023-05-26 03:52:13.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/SOURCES.txt
--rw-r--r--   0 ctw        (501) staff       (20)        1 2023-05-26 03:52:12.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/dependency_links.txt
--rw-r--r--   0 ctw        (501) staff       (20)       28 2023-05-26 03:52:13.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/requires.txt
--rw-r--r--   0 ctw        (501) staff       (20)        6 2023-05-26 03:52:13.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/top_level.txt
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 03:52:13.166765 at-fetch-data-1.0.4/fetch/
--rw-r--r--   0 ctw        (501) staff       (20)        0 2023-05-23 12:37:49.000000 at-fetch-data-1.0.4/fetch/__init__.py
--rw-r--r--   0 ctw        (501) staff       (20)      367 2023-05-23 12:37:49.000000 at-fetch-data-1.0.4/fetch/const.py
--rw-r--r--   0 ctw        (501) staff       (20)     3278 2023-05-26 03:50:28.000000 at-fetch-data-1.0.4/fetch/fetch.py
--rw-r--r--   0 ctw        (501) staff       (20)       38 2023-05-26 03:52:13.167328 at-fetch-data-1.0.4/setup.cfg
--rw-r--r--   0 ctw        (501) staff       (20)      454 2023-05-26 03:50:56.000000 at-fetch-data-1.0.4/setup.py
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 04:02:39.318212 at-fetch-data-1.0.5/
+-rw-r--r--   0 ctw        (501) staff       (20)     1159 2023-05-26 04:02:39.318057 at-fetch-data-1.0.5/PKG-INFO
+-rw-r--r--   0 ctw        (501) staff       (20)      997 2023-05-26 04:02:34.000000 at-fetch-data-1.0.5/README.md
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 04:02:39.317116 at-fetch-data-1.0.5/at_fetch_data.egg-info/
+-rw-r--r--   0 ctw        (501) staff       (20)     1159 2023-05-26 04:02:38.000000 at-fetch-data-1.0.5/at_fetch_data.egg-info/PKG-INFO
+-rw-r--r--   0 ctw        (501) staff       (20)      250 2023-05-26 04:02:39.000000 at-fetch-data-1.0.5/at_fetch_data.egg-info/SOURCES.txt
+-rw-r--r--   0 ctw        (501) staff       (20)        1 2023-05-26 04:02:39.000000 at-fetch-data-1.0.5/at_fetch_data.egg-info/dependency_links.txt
+-rw-r--r--   0 ctw        (501) staff       (20)       28 2023-05-26 04:02:39.000000 at-fetch-data-1.0.5/at_fetch_data.egg-info/requires.txt
+-rw-r--r--   0 ctw        (501) staff       (20)        6 2023-05-26 04:02:39.000000 at-fetch-data-1.0.5/at_fetch_data.egg-info/top_level.txt
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 04:02:39.317694 at-fetch-data-1.0.5/fetch/
+-rw-r--r--   0 ctw        (501) staff       (20)        0 2023-05-23 12:37:49.000000 at-fetch-data-1.0.5/fetch/__init__.py
+-rw-r--r--   0 ctw        (501) staff       (20)      367 2023-05-23 12:37:49.000000 at-fetch-data-1.0.5/fetch/const.py
+-rw-r--r--   0 ctw        (501) staff       (20)     3278 2023-05-26 03:50:28.000000 at-fetch-data-1.0.5/fetch/fetch.py
+-rw-r--r--   0 ctw        (501) staff       (20)       38 2023-05-26 04:02:39.318265 at-fetch-data-1.0.5/setup.cfg
+-rw-r--r--   0 ctw        (501) staff       (20)      454 2023-05-26 04:02:28.000000 at-fetch-data-1.0.5/setup.py
```

### Comparing `at-fetch-data-1.0.4/README.md` & `at-fetch-data-1.0.5/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,31 @@
 ## at_fetch_data
 
 ```
 pip install at_fetch_data
-poetry add at_fetch_data
 ```
 
-### example
+### api
+
+
+- get_all_klines_data: 
+    - url:str 
+        - http://47.243.179.153:8000/api/kline/spot
+    - symbol: str 
+    - interval: str
+    - start_time: int
+    - end_time: int
+- get_kline_count: 
+    - url: str
+        - http://47.243.179.153:8000/api/kline/spot_count
+    - symbol: str
+    - interval: str
+    - start_time: int
+    - end_time: int
 
-```
-poetry install
-poetry run python -m example.start_time
-```
 
 ### usage
 
 ```
 from fetch.fetch import Fetch
 import asyncio
 import time
```

### Comparing `at-fetch-data-1.0.4/fetch/fetch.py` & `at-fetch-data-1.0.5/fetch/fetch.py`

 * *Files identical despite different names*

