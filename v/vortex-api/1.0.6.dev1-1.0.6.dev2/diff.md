# Comparing `tmp/vortex_api-1.0.6.dev1.tar.gz` & `tmp/vortex_api-1.0.6.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-86slbcnf/vortex_api-1.0.6.dev1.tar", last modified: Fri May 26 07:29:28 2023, max compression
+gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-38ufni9h/vortex_api-1.0.6.dev2.tar", last modified: Fri May 26 07:59:29 2023, max compression
```

## Comparing `vortex_api-1.0.6.dev1.tar` & `vortex_api-1.0.6.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:29:28.019294 vortex_api-1.0.6.dev1/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev1/LICENSE
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1776 2023-05-26 07:29:28.019433 vortex_api-1.0.6.dev1/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      915 2023-05-10 20:08:17.000000 vortex_api-1.0.6.dev1/README.md
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 07:29:28.019820 vortex_api-1.0.6.dev1/setup.cfg
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1533 2023-05-26 07:20:10.000000 vortex_api-1.0.6.dev1/setup.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:29:28.017553 vortex_api-1.0.6.dev1/vortex_api/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev1/vortex_api/__init__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 07:27:02.000000 vortex_api-1.0.6.dev1/vortex_api/__version__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev1/vortex_api/api.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    22309 2023-05-26 07:18:33.000000 vortex_api-1.0.6.dev1/vortex_api/vortex_feed.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:29:28.019138 vortex_api-1.0.6.dev1/vortex_api.egg-info/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1776 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/SOURCES.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/dependency_links.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      111 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/requires.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/top_level.txt
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:59:29.199145 vortex_api-1.0.6.dev2/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev2/LICENSE
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     2420 2023-05-26 07:59:29.199583 vortex_api-1.0.6.dev2/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1559 2023-05-26 07:58:48.000000 vortex_api-1.0.6.dev2/README.md
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 07:59:29.200019 vortex_api-1.0.6.dev2/setup.cfg
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1533 2023-05-26 07:20:10.000000 vortex_api-1.0.6.dev2/setup.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:59:29.191244 vortex_api-1.0.6.dev2/vortex_api/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev2/vortex_api/__init__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 07:59:05.000000 vortex_api-1.0.6.dev2/vortex_api/__version__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev2/vortex_api/api.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    22309 2023-05-26 07:18:33.000000 vortex_api-1.0.6.dev2/vortex_api/vortex_feed.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:59:29.198984 vortex_api-1.0.6.dev2/vortex_api.egg-info/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     2420 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      111 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/requires.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/top_level.txt
```

### Comparing `vortex_api-1.0.6.dev1/LICENSE` & `vortex_api-1.0.6.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev1/PKG-INFO` & `vortex_api-1.0.6.dev2/vortex_api.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vortex_api
-Version: 1.0.6.dev1
+Name: vortex-api
+Version: 1.0.6.dev2
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -54,9 +54,35 @@
        validity = Vc.ValidityTypes.FULL_DAY)
 
 #Get order book 
 client.orders(limit=20,offset=1)
 
 
 ```
+
+# Connecting to websocket
+
+```
+from vortex_api import VortexFeed
+from vortex_api import Constants as Vc
+
+def main():
+       # Get access token from any of the login methods
+       wire = VortexFeed(access_token) 
+
+       wire.on_price_update = on_price_update
+       wire.on_order_update = on_order_update
+       wire.on_connect = on_connect
+
+def on_price_update(ws,data): 
+       print(data)
+
+def on_order_update(ws,data): 
+       print(data)
+
+def on_connect(ws, response):
+       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to NIFTY 50 
+       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to BANKNIFTY 
+
+```
 Refer to the [python document](https://vortex.asthatrade.com/docs/pyvortex/vortex_api.html) for all methods and features
```

### Comparing `vortex_api-1.0.6.dev1/README.md` & `vortex_api-1.0.6.dev2/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -33,9 +33,35 @@
        validity = Vc.ValidityTypes.FULL_DAY)
 
 #Get order book 
 client.orders(limit=20,offset=1)
 
 
 ```
+
+# Connecting to websocket
+
+```
+from vortex_api import VortexFeed
+from vortex_api import Constants as Vc
+
+def main():
+       # Get access token from any of the login methods
+       wire = VortexFeed(access_token) 
+
+       wire.on_price_update = on_price_update
+       wire.on_order_update = on_order_update
+       wire.on_connect = on_connect
+
+def on_price_update(ws,data): 
+       print(data)
+
+def on_order_update(ws,data): 
+       print(data)
+
+def on_connect(ws, response):
+       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to NIFTY 50 
+       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to BANKNIFTY 
+
+```
 Refer to the [python document](https://vortex.asthatrade.com/docs/pyvortex/vortex_api.html) for all methods and features
```

### Comparing `vortex_api-1.0.6.dev1/setup.py` & `vortex_api-1.0.6.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev1/vortex_api/__init__.py` & `vortex_api-1.0.6.dev2/vortex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev1/vortex_api/api.py` & `vortex_api-1.0.6.dev2/vortex_api/api.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev1/vortex_api/vortex_feed.py` & `vortex_api-1.0.6.dev2/vortex_api/vortex_feed.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev1/vortex_api.egg-info/PKG-INFO` & `vortex_api-1.0.6.dev2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: vortex-api
-Version: 1.0.6.dev1
+Name: vortex_api
+Version: 1.0.6.dev2
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -54,9 +54,35 @@
        validity = Vc.ValidityTypes.FULL_DAY)
 
 #Get order book 
 client.orders(limit=20,offset=1)
 
 
 ```
+
+# Connecting to websocket
+
+```
+from vortex_api import VortexFeed
+from vortex_api import Constants as Vc
+
+def main():
+       # Get access token from any of the login methods
+       wire = VortexFeed(access_token) 
+
+       wire.on_price_update = on_price_update
+       wire.on_order_update = on_order_update
+       wire.on_connect = on_connect
+
+def on_price_update(ws,data): 
+       print(data)
+
+def on_order_update(ws,data): 
+       print(data)
+
+def on_connect(ws, response):
+       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to NIFTY 50 
+       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to BANKNIFTY 
+
+```
 Refer to the [python document](https://vortex.asthatrade.com/docs/pyvortex/vortex_api.html) for all methods and features
```

