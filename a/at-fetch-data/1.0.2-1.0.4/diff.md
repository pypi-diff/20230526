# Comparing `tmp/at-fetch-data-1.0.2.tar.gz` & `tmp/at-fetch-data-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "at-fetch-data-1.0.2.tar", last modified: Tue May 23 12:57:57 2023, max compression
+gzip compressed data, was "at-fetch-data-1.0.4.tar", last modified: Fri May 26 03:52:13 2023, max compression
```

## Comparing `at-fetch-data-1.0.2.tar` & `at-fetch-data-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:57:57.514576 at-fetch-data-1.0.2/
--rw-r--r--   0 ctw        (501) staff       (20)      904 2023-05-23 12:57:57.514439 at-fetch-data-1.0.2/PKG-INFO
--rw-r--r--   0 ctw        (501) staff       (20)      742 2023-05-23 12:38:22.000000 at-fetch-data-1.0.2/README.md
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:57:57.513500 at-fetch-data-1.0.2/at_fetch_data.egg-info/
--rw-r--r--   0 ctw        (501) staff       (20)      904 2023-05-23 12:57:57.000000 at-fetch-data-1.0.2/at_fetch_data.egg-info/PKG-INFO
--rw-r--r--   0 ctw        (501) staff       (20)      250 2023-05-23 12:57:57.000000 at-fetch-data-1.0.2/at_fetch_data.egg-info/SOURCES.txt
--rw-r--r--   0 ctw        (501) staff       (20)        1 2023-05-23 12:57:57.000000 at-fetch-data-1.0.2/at_fetch_data.egg-info/dependency_links.txt
--rw-r--r--   0 ctw        (501) staff       (20)       28 2023-05-23 12:57:57.000000 at-fetch-data-1.0.2/at_fetch_data.egg-info/requires.txt
--rw-r--r--   0 ctw        (501) staff       (20)        6 2023-05-23 12:57:57.000000 at-fetch-data-1.0.2/at_fetch_data.egg-info/top_level.txt
-drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-23 12:57:57.514107 at-fetch-data-1.0.2/fetch/
--rw-r--r--   0 ctw        (501) staff       (20)        0 2023-05-23 12:37:49.000000 at-fetch-data-1.0.2/fetch/__init__.py
--rw-r--r--   0 ctw        (501) staff       (20)      367 2023-05-23 12:37:49.000000 at-fetch-data-1.0.2/fetch/const.py
--rw-r--r--   0 ctw        (501) staff       (20)     2911 2023-05-23 12:42:48.000000 at-fetch-data-1.0.2/fetch/fetch.py
--rw-r--r--   0 ctw        (501) staff       (20)       38 2023-05-23 12:57:57.514631 at-fetch-data-1.0.2/setup.cfg
--rw-r--r--   0 ctw        (501) staff       (20)      454 2023-05-23 12:57:52.000000 at-fetch-data-1.0.2/setup.py
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 03:52:13.167279 at-fetch-data-1.0.4/
+-rw-r--r--   0 ctw        (501) staff       (20)      904 2023-05-26 03:52:13.167139 at-fetch-data-1.0.4/PKG-INFO
+-rw-r--r--   0 ctw        (501) staff       (20)      742 2023-05-23 12:38:22.000000 at-fetch-data-1.0.4/README.md
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 03:52:13.166209 at-fetch-data-1.0.4/at_fetch_data.egg-info/
+-rw-r--r--   0 ctw        (501) staff       (20)      904 2023-05-26 03:52:12.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/PKG-INFO
+-rw-r--r--   0 ctw        (501) staff       (20)      250 2023-05-26 03:52:13.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/SOURCES.txt
+-rw-r--r--   0 ctw        (501) staff       (20)        1 2023-05-26 03:52:12.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/dependency_links.txt
+-rw-r--r--   0 ctw        (501) staff       (20)       28 2023-05-26 03:52:13.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/requires.txt
+-rw-r--r--   0 ctw        (501) staff       (20)        6 2023-05-26 03:52:13.000000 at-fetch-data-1.0.4/at_fetch_data.egg-info/top_level.txt
+drwxr-xr-x   0 ctw        (501) staff       (20)        0 2023-05-26 03:52:13.166765 at-fetch-data-1.0.4/fetch/
+-rw-r--r--   0 ctw        (501) staff       (20)        0 2023-05-23 12:37:49.000000 at-fetch-data-1.0.4/fetch/__init__.py
+-rw-r--r--   0 ctw        (501) staff       (20)      367 2023-05-23 12:37:49.000000 at-fetch-data-1.0.4/fetch/const.py
+-rw-r--r--   0 ctw        (501) staff       (20)     3278 2023-05-26 03:50:28.000000 at-fetch-data-1.0.4/fetch/fetch.py
+-rw-r--r--   0 ctw        (501) staff       (20)       38 2023-05-26 03:52:13.167328 at-fetch-data-1.0.4/setup.cfg
+-rw-r--r--   0 ctw        (501) staff       (20)      454 2023-05-26 03:50:56.000000 at-fetch-data-1.0.4/setup.py
```

### Comparing `at-fetch-data-1.0.2/PKG-INFO` & `at-fetch-data-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: at-fetch-data
-Version: 1.0.2
+Version: 1.0.4
 Summary: UNKNOWN
 Author: ctwel
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## at_fetch_data
```

### Comparing `at-fetch-data-1.0.2/README.md` & `at-fetch-data-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `at-fetch-data-1.0.2/at_fetch_data.egg-info/PKG-INFO` & `at-fetch-data-1.0.4/at_fetch_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: at-fetch-data
-Version: 1.0.2
+Version: 1.0.4
 Summary: UNKNOWN
 Author: ctwel
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 ## at_fetch_data
```

### Comparing `at-fetch-data-1.0.2/fetch/fetch.py` & `at-fetch-data-1.0.4/fetch/fetch.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,7 +69,20 @@
         df = []
         for item in res:
             obj = item.json()
             data = pd.DataFrame(obj["data"])
             df.append(data)
         df_res = pd.concat(df)
         return df_res.drop_duplicates()
+
+    
+    async def get_kline_count(
+        self, url: str, symbol: str, interval: str, start_time: int, end_time: int
+    ):
+        params = {
+            "symbol": symbol,
+            "interval": interval,
+            "start_time": start_time,
+            "end_time": end_time,
+        }
+        res = await self.get(url, params)
+        return res.json()["data"]
```

