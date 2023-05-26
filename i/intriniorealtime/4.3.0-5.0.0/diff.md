# Comparing `tmp/intriniorealtime-4.3.0.tar.gz` & `tmp/intriniorealtime-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/intriniorealtime-4.3.0.tar", last modified: Wed Apr 19 20:03:10 2023, max compression
+gzip compressed data, was "dist/intriniorealtime-5.0.0.tar", last modified: Fri May 26 16:35:06 2023, max compression
```

## Comparing `intriniorealtime-4.3.0.tar` & `intriniorealtime-5.0.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/
--rw-r--r--   0 shawn      (503) staff       (20)     9401 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/PKG-INFO
--rw-r--r--   0 shawn      (503) staff       (20)    35141 2022-01-04 22:35:51.000000 intriniorealtime-4.3.0/LICENSE
--rw-r--r--   0 shawn      (503) staff       (20)       65 2022-01-04 22:35:51.000000 intriniorealtime-4.3.0/MANIFEST.in
--rw-r--r--   0 shawn      (503) staff       (20)     7113 2023-04-19 19:47:24.000000 intriniorealtime-4.3.0/README.md
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime/
--rw-r--r--   0 shawn      (503) staff       (20)    15258 2023-04-19 19:54:13.000000 intriniorealtime-4.3.0/intriniorealtime/client.py
--rw-r--r--   0 shawn      (503) staff       (20)        0 2022-01-04 22:35:51.000000 intriniorealtime-4.3.0/intriniorealtime/__init__.py
-drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/
--rw-r--r--   0 shawn      (503) staff       (20)     9401 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/PKG-INFO
--rw-r--r--   0 shawn      (503) staff       (20)      303 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/SOURCES.txt
--rw-r--r--   0 shawn      (503) staff       (20)       56 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/requires.txt
--rw-r--r--   0 shawn      (503) staff       (20)       17 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/top_level.txt
--rw-r--r--   0 shawn      (503) staff       (20)        1 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/intriniorealtime.egg-info/dependency_links.txt
--rw-r--r--   0 shawn      (503) staff       (20)      963 2023-04-19 19:41:25.000000 intriniorealtime-4.3.0/setup.py
--rw-r--r--   0 shawn      (503) staff       (20)       79 2023-04-19 20:03:10.000000 intriniorealtime-4.3.0/setup.cfg
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/
+-rw-r--r--   0 shawn      (503) staff       (20)     9403 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/PKG-INFO
+-rw-r--r--   0 shawn      (503) staff       (20)    35141 2022-01-04 22:35:51.000000 intriniorealtime-5.0.0/LICENSE
+-rw-r--r--   0 shawn      (503) staff       (20)       65 2022-01-04 22:35:51.000000 intriniorealtime-5.0.0/MANIFEST.in
+-rw-r--r--   0 shawn      (503) staff       (20)     7114 2023-05-26 16:34:00.000000 intriniorealtime-5.0.0/README.md
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/intriniorealtime/
+-rw-r--r--   0 shawn      (503) staff       (20)    17712 2023-05-26 16:34:00.000000 intriniorealtime-5.0.0/intriniorealtime/client.py
+-rw-r--r--   0 shawn      (503) staff       (20)        0 2022-01-04 22:35:51.000000 intriniorealtime-5.0.0/intriniorealtime/__init__.py
+drwxr-xr-x   0 shawn      (503) staff       (20)        0 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/intriniorealtime.egg-info/
+-rw-r--r--   0 shawn      (503) staff       (20)     9403 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/intriniorealtime.egg-info/PKG-INFO
+-rw-r--r--   0 shawn      (503) staff       (20)      303 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/intriniorealtime.egg-info/SOURCES.txt
+-rw-r--r--   0 shawn      (503) staff       (20)       56 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/intriniorealtime.egg-info/requires.txt
+-rw-r--r--   0 shawn      (503) staff       (20)       17 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/intriniorealtime.egg-info/top_level.txt
+-rw-r--r--   0 shawn      (503) staff       (20)        1 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/intriniorealtime.egg-info/dependency_links.txt
+-rw-r--r--   0 shawn      (503) staff       (20)      964 2023-05-26 16:34:00.000000 intriniorealtime-5.0.0/setup.py
+-rw-r--r--   0 shawn      (503) staff       (20)       79 2023-05-26 16:35:06.000000 intriniorealtime-5.0.0/setup.cfg
```

### Comparing `intriniorealtime-4.3.0/PKG-INFO` & `intriniorealtime-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: intriniorealtime
-Version: 4.3.0
+Version: 5.0.0
 Summary: Intrinio Python SDK for Real-Time Stock Prices
 Home-page: https://intrinio.com
 Author: Intrinio Python SDK for Real-Time Stock Prices
 Author-email: success@intrinio.com
 License: UNKNOWN
-Download-URL: https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.3.0.tar.gz
+Download-URL: https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v5.0.0.tar.gz
 Description: # intrinio realtime python sdk
         SDK for working with Intrinio's realtime Multi-Exchange prices feed.  Intrinio’s Multi-Exchange feed bridges the gap by merging real-time equity pricing from the IEX and MEMX exchanges. Get a comprehensive view with increased market volume and enjoy no exchange fees, no per-user requirements, no permissions or authorizations, and little to no paperwork.
         
         [Intrinio](https://intrinio.com/) provides real-time stock prices via a two-way WebSocket connection. To get started, [subscribe to a real-time data feed](https://intrinio.com/real-time-multi-exchange) and follow the instructions below.
         
         [Documentation for our legacy realtime client](https://github.com/intrinio/intrinio-realtime-python-sdk/tree/2.2.0)
         
         ## Requirements
         
-        - Python 3.6
+        - Python 3.10
         - You need https://pypi.org/project/websocket-client/, not https://pypi.org/project/websocket/.
         
         ## Docker
         Add your API key to the example_app.py file, then
         ```
         docker compose build
         docker compose run client
@@ -213,9 +213,9 @@
         
         `client.leave_all()` - Leaves all channels.
         
 Keywords: realtime,stock prices,intrinio,stock market,stock data,financial
 Platform: UNKNOWN
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: ~=3.6
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
```

### Comparing `intriniorealtime-4.3.0/LICENSE` & `intriniorealtime-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `intriniorealtime-4.3.0/README.md` & `intriniorealtime-5.0.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 [Intrinio](https://intrinio.com/) provides real-time stock prices via a two-way WebSocket connection. To get started, [subscribe to a real-time data feed](https://intrinio.com/real-time-multi-exchange) and follow the instructions below.
 
 [Documentation for our legacy realtime client](https://github.com/intrinio/intrinio-realtime-python-sdk/tree/2.2.0)
 
 ## Requirements
 
-- Python 3.6
+- Python 3.10
 - You need https://pypi.org/project/websocket-client/, not https://pypi.org/project/websocket/.
 
 ## Docker
 Add your API key to the example_app.py file, then
 ```
 docker compose build
 docker compose run client
```

### Comparing `intriniorealtime-4.3.0/intriniorealtime.egg-info/PKG-INFO` & `intriniorealtime-5.0.0/intriniorealtime.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: intriniorealtime
-Version: 4.3.0
+Version: 5.0.0
 Summary: Intrinio Python SDK for Real-Time Stock Prices
 Home-page: https://intrinio.com
 Author: Intrinio Python SDK for Real-Time Stock Prices
 Author-email: success@intrinio.com
 License: UNKNOWN
-Download-URL: https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.3.0.tar.gz
+Download-URL: https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v5.0.0.tar.gz
 Description: # intrinio realtime python sdk
         SDK for working with Intrinio's realtime Multi-Exchange prices feed.  Intrinio’s Multi-Exchange feed bridges the gap by merging real-time equity pricing from the IEX and MEMX exchanges. Get a comprehensive view with increased market volume and enjoy no exchange fees, no per-user requirements, no permissions or authorizations, and little to no paperwork.
         
         [Intrinio](https://intrinio.com/) provides real-time stock prices via a two-way WebSocket connection. To get started, [subscribe to a real-time data feed](https://intrinio.com/real-time-multi-exchange) and follow the instructions below.
         
         [Documentation for our legacy realtime client](https://github.com/intrinio/intrinio-realtime-python-sdk/tree/2.2.0)
         
         ## Requirements
         
-        - Python 3.6
+        - Python 3.10
         - You need https://pypi.org/project/websocket-client/, not https://pypi.org/project/websocket/.
         
         ## Docker
         Add your API key to the example_app.py file, then
         ```
         docker compose build
         docker compose run client
@@ -213,9 +213,9 @@
         
         `client.leave_all()` - Leaves all channels.
         
 Keywords: realtime,stock prices,intrinio,stock market,stock data,financial
 Platform: UNKNOWN
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: Topic :: Office/Business :: Financial :: Investment
-Requires-Python: ~=3.6
+Requires-Python: ~=3.10
 Description-Content-Type: text/markdown
```

### Comparing `intriniorealtime-4.3.0/setup.py` & `intriniorealtime-5.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 def readme():
     with open('README.md') as f:
         return f.read()
 
 setup(
     name = 'intriniorealtime',
     packages = ['intriniorealtime'],
-    version = '4.3.0',
+    version = '5.0.0',
     author = 'Intrinio Python SDK for Real-Time Stock Prices',
     author_email = 'success@intrinio.com',
     url = 'https://intrinio.com',
     description = 'Intrinio Python SDK for Real-Time Stock Prices',
     long_description = readme(),
     long_description_content_type = 'text/markdown',
     install_requires = ['requests>=2.26.0','websocket-client>=1.2.1','wsaccel>=0.6.3'],
-    python_requires = '~=3.6',
-    download_url = 'https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v4.3.0.tar.gz',
+    python_requires = '~=3.10',
+    download_url = 'https://github.com/intrinio/intrinio-realtime-python-sdk/archive/v5.0.0.tar.gz',
     keywords = ['realtime','stock prices','intrinio','stock market','stock data','financial'],
     classifiers = [
         'Intended Audience :: Financial and Insurance Industry',
         'Topic :: Office/Business :: Financial :: Investment'
     ]
 )
```

