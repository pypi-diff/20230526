# Comparing `tmp/vortex_api-1.0.6.dev3.tar.gz` & `tmp/vortex_api-1.0.6.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-6u4zrxvm/vortex_api-1.0.6.dev3.tar", last modified: Fri May 26 09:42:39 2023, max compression
+gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-1nme3hvo/vortex_api-1.0.6.dev4.tar", last modified: Fri May 26 09:54:38 2023, max compression
```

## Comparing `vortex_api-1.0.6.dev3.tar` & `vortex_api-1.0.6.dev4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:42:39.690368 vortex_api-1.0.6.dev3/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev3/LICENSE
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     2882 2023-05-26 09:42:39.690487 vortex_api-1.0.6.dev3/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     2021 2023-05-26 09:38:35.000000 vortex_api-1.0.6.dev3/README.md
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 09:42:39.690776 vortex_api-1.0.6.dev3/setup.cfg
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1533 2023-05-26 07:20:10.000000 vortex_api-1.0.6.dev3/setup.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:42:39.688597 vortex_api-1.0.6.dev3/vortex_api/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev3/vortex_api/__init__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 09:42:06.000000 vortex_api-1.0.6.dev3/vortex_api/__version__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev3/vortex_api/api.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    22011 2023-05-26 09:41:32.000000 vortex_api-1.0.6.dev3/vortex_api/vortex_feed.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:42:39.690216 vortex_api-1.0.6.dev3/vortex_api.egg-info/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     2882 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/SOURCES.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/dependency_links.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      111 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/requires.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/top_level.txt
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:54:38.574833 vortex_api-1.0.6.dev4/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev4/LICENSE
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     3206 2023-05-26 09:54:38.574921 vortex_api-1.0.6.dev4/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     2345 2023-05-26 09:51:08.000000 vortex_api-1.0.6.dev4/README.md
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 09:54:38.575193 vortex_api-1.0.6.dev4/setup.cfg
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1569 2023-05-26 09:54:09.000000 vortex_api-1.0.6.dev4/setup.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:54:38.573412 vortex_api-1.0.6.dev4/vortex_api/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev4/vortex_api/__init__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 09:54:17.000000 vortex_api-1.0.6.dev4/vortex_api/__version__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev4/vortex_api/api.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    22011 2023-05-26 09:41:32.000000 vortex_api-1.0.6.dev4/vortex_api/vortex_feed.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:54:38.574696 vortex_api-1.0.6.dev4/vortex_api.egg-info/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     3206 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      136 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/requires.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 09:54:38.000000 vortex_api-1.0.6.dev4/vortex_api.egg-info/top_level.txt
```

### Comparing `vortex_api-1.0.6.dev3/LICENSE` & `vortex_api-1.0.6.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev3/PKG-INFO` & `vortex_api-1.0.6.dev4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex_api
-Version: 1.0.6.dev3
+Version: 1.0.6.dev4
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -57,14 +57,17 @@
 client.orders(limit=20,offset=1)
 
 
 ```
 
 # Connecting to websocket
 
+Using the feed, you can listen to both price quote changes and order/trade updates. You need to define your own callbacks for `on_price_update`
+and `on_order_update`. The packet structure for `on_order_update` is the same as that received in postbacks and is available [here](https://vortex.asthatrade.com/docs/postbacks/)
+
 ```
 from vortex_api import VortexFeed
 from vortex_api import Constants as Vc
 import time
 
 def main():
     # Get access token from any of the login methods
```

### Comparing `vortex_api-1.0.6.dev3/README.md` & `vortex_api-1.0.6.dev4/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -36,14 +36,17 @@
 client.orders(limit=20,offset=1)
 
 
 ```
 
 # Connecting to websocket
 
+Using the feed, you can listen to both price quote changes and order/trade updates. You need to define your own callbacks for `on_price_update`
+and `on_order_update`. The packet structure for `on_order_update` is the same as that received in postbacks and is available [here](https://vortex.asthatrade.com/docs/postbacks/)
+
 ```
 from vortex_api import VortexFeed
 from vortex_api import Constants as Vc
 import time
 
 def main():
     # Get access token from any of the login methods
```

### Comparing `vortex_api-1.0.6.dev3/setup.py` & `vortex_api-1.0.6.dev4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,16 @@
     packages=["vortex_api"],
     install_requires=[
         "requests>=2.25.1",
         "wrapt>=1.15.0",
         "six>=1.11.0",
         "pyOpenSSL>=17.5.0",
         "python-dateutil>=2.6.1",
-        "autobahn[twisted]==19.11.2"
+        "autobahn[twisted]==19.11.2",
+        "service_identity>=18.1.0"
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `vortex_api-1.0.6.dev3/vortex_api/__init__.py` & `vortex_api-1.0.6.dev4/vortex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev3/vortex_api/api.py` & `vortex_api-1.0.6.dev4/vortex_api/api.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev3/vortex_api/vortex_feed.py` & `vortex_api-1.0.6.dev4/vortex_api/vortex_feed.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev3/vortex_api.egg-info/PKG-INFO` & `vortex_api-1.0.6.dev4/vortex_api.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex-api
-Version: 1.0.6.dev3
+Version: 1.0.6.dev4
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -57,14 +57,17 @@
 client.orders(limit=20,offset=1)
 
 
 ```
 
 # Connecting to websocket
 
+Using the feed, you can listen to both price quote changes and order/trade updates. You need to define your own callbacks for `on_price_update`
+and `on_order_update`. The packet structure for `on_order_update` is the same as that received in postbacks and is available [here](https://vortex.asthatrade.com/docs/postbacks/)
+
 ```
 from vortex_api import VortexFeed
 from vortex_api import Constants as Vc
 import time
 
 def main():
     # Get access token from any of the login methods
```

