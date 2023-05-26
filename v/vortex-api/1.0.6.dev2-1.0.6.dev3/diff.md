# Comparing `tmp/vortex_api-1.0.6.dev2.tar.gz` & `tmp/vortex_api-1.0.6.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-38ufni9h/vortex_api-1.0.6.dev2.tar", last modified: Fri May 26 07:59:29 2023, max compression
+gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-6u4zrxvm/vortex_api-1.0.6.dev3.tar", last modified: Fri May 26 09:42:39 2023, max compression
```

## Comparing `vortex_api-1.0.6.dev2.tar` & `vortex_api-1.0.6.dev3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:59:29.199145 vortex_api-1.0.6.dev2/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev2/LICENSE
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     2420 2023-05-26 07:59:29.199583 vortex_api-1.0.6.dev2/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1559 2023-05-26 07:58:48.000000 vortex_api-1.0.6.dev2/README.md
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 07:59:29.200019 vortex_api-1.0.6.dev2/setup.cfg
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1533 2023-05-26 07:20:10.000000 vortex_api-1.0.6.dev2/setup.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:59:29.191244 vortex_api-1.0.6.dev2/vortex_api/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev2/vortex_api/__init__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 07:59:05.000000 vortex_api-1.0.6.dev2/vortex_api/__version__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev2/vortex_api/api.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    22309 2023-05-26 07:18:33.000000 vortex_api-1.0.6.dev2/vortex_api/vortex_feed.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:59:29.198984 vortex_api-1.0.6.dev2/vortex_api.egg-info/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     2420 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/SOURCES.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/dependency_links.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      111 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/requires.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 07:59:29.000000 vortex_api-1.0.6.dev2/vortex_api.egg-info/top_level.txt
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:42:39.690368 vortex_api-1.0.6.dev3/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev3/LICENSE
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     2882 2023-05-26 09:42:39.690487 vortex_api-1.0.6.dev3/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     2021 2023-05-26 09:38:35.000000 vortex_api-1.0.6.dev3/README.md
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 09:42:39.690776 vortex_api-1.0.6.dev3/setup.cfg
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1533 2023-05-26 07:20:10.000000 vortex_api-1.0.6.dev3/setup.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:42:39.688597 vortex_api-1.0.6.dev3/vortex_api/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev3/vortex_api/__init__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 09:42:06.000000 vortex_api-1.0.6.dev3/vortex_api/__version__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev3/vortex_api/api.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    22011 2023-05-26 09:41:32.000000 vortex_api-1.0.6.dev3/vortex_api/vortex_feed.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 09:42:39.690216 vortex_api-1.0.6.dev3/vortex_api.egg-info/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     2882 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      111 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/requires.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 09:42:39.000000 vortex_api-1.0.6.dev3/vortex_api.egg-info/top_level.txt
```

### Comparing `vortex_api-1.0.6.dev2/LICENSE` & `vortex_api-1.0.6.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev2/PKG-INFO` & `vortex_api-1.0.6.dev3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex_api
-Version: 1.0.6.dev2
+Version: 1.0.6.dev3
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -60,29 +60,43 @@
 ```
 
 # Connecting to websocket
 
 ```
 from vortex_api import VortexFeed
 from vortex_api import Constants as Vc
+import time
 
 def main():
-       # Get access token from any of the login methods
-       wire = VortexFeed(access_token) 
+    # Get access token from any of the login methods
+    wire = VortexFeed(access_token) 
+
+    wire.on_price_update = on_price_update
+    wire.on_order_update = on_order_update
+    wire.on_connect = on_connect
+    wire.connect(threaded=True) 
+    # If you make threaded = False, anything after this line will not execute
+
+    time.sleep(10)
+    
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000)
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 26009)
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 2885)
 
-       wire.on_price_update = on_price_update
-       wire.on_order_update = on_order_update
-       wire.on_connect = on_connect
 
 def on_price_update(ws,data): 
-       print(data)
+    print(data)
 
 def on_order_update(ws,data): 
-       print(data)
+    print(data)
 
 def on_connect(ws, response):
-       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to NIFTY 50 
-       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to BANKNIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000, Vc.QuoteModes.LTP) #Subscribe to NIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26009,Vc.QuoteModes.OHLCV) # Subscribe to BANKNIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 2885,Vc.QuoteModes.FULL) # Subscribe to RELIANCE 
+
+if __name__ == "__main__":
+    main()
 
 ```
 Refer to the [python document](https://vortex.asthatrade.com/docs/pyvortex/vortex_api.html) for all methods and features
```

### Comparing `vortex_api-1.0.6.dev2/README.md` & `vortex_api-1.0.6.dev3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -39,29 +39,43 @@
 ```
 
 # Connecting to websocket
 
 ```
 from vortex_api import VortexFeed
 from vortex_api import Constants as Vc
+import time
 
 def main():
-       # Get access token from any of the login methods
-       wire = VortexFeed(access_token) 
+    # Get access token from any of the login methods
+    wire = VortexFeed(access_token) 
+
+    wire.on_price_update = on_price_update
+    wire.on_order_update = on_order_update
+    wire.on_connect = on_connect
+    wire.connect(threaded=True) 
+    # If you make threaded = False, anything after this line will not execute
+
+    time.sleep(10)
+    
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000)
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 26009)
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 2885)
 
-       wire.on_price_update = on_price_update
-       wire.on_order_update = on_order_update
-       wire.on_connect = on_connect
 
 def on_price_update(ws,data): 
-       print(data)
+    print(data)
 
 def on_order_update(ws,data): 
-       print(data)
+    print(data)
 
 def on_connect(ws, response):
-       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to NIFTY 50 
-       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to BANKNIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000, Vc.QuoteModes.LTP) #Subscribe to NIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26009,Vc.QuoteModes.OHLCV) # Subscribe to BANKNIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 2885,Vc.QuoteModes.FULL) # Subscribe to RELIANCE 
+
+if __name__ == "__main__":
+    main()
 
 ```
 Refer to the [python document](https://vortex.asthatrade.com/docs/pyvortex/vortex_api.html) for all methods and features
```

### Comparing `vortex_api-1.0.6.dev2/setup.py` & `vortex_api-1.0.6.dev3/setup.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev2/vortex_api/__init__.py` & `vortex_api-1.0.6.dev3/vortex_api/__init__.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev2/vortex_api/api.py` & `vortex_api-1.0.6.dev3/vortex_api/api.py`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.6.dev2/vortex_api/vortex_feed.py` & `vortex_api-1.0.6.dev3/vortex_api/vortex_feed.py`

 * *Files 2% similar despite different names*

```diff
@@ -165,15 +165,14 @@
     maxDelay = 5
     maxRetries = 10
 
     _last_connection_time = None
 
     def __init__(self, *args, **kwargs):
         """Initialize with default callback method values."""
-        self.debug = True
         self.ws = None
         self.on_open = None
         self.on_error = None
         self.on_close = None
         self.on_message = None
         self.on_connect = None
         self.on_reconnect = None
@@ -233,15 +232,15 @@
     # Default reconnect attempts
     RECONNECT_MAX_TRIES = 50
     _is_first_connect = True
     _message_subscribe = "subscribe"
     _message_unsubscribe = "unsubscribe"
 
     def __init__(self, access_token: str, websocket_endpoint="wss://wire.asthatrade.com/ws",reconnect=True, reconnect_max_tries=RECONNECT_MAX_TRIES, reconnect_max_delay=RECONNECT_MAX_DELAY,
-                 connect_timeout=CONNECT_TIMEOUT) -> None:
+                 connect_timeout=CONNECT_TIMEOUT, debug = False) -> None:
         self._maximum_reconnect_max_tries = self.RECONNECT_MAX_TRIES
         self._minimum_reconnect_max_delay = 0 
         if reconnect == False: 
             self.reconnect_max_tries = 0 
         elif reconnect_max_tries > self._maximum_reconnect_max_tries:
             log.warning("`reconnect_max_tries` can not be more than {val}. Setting to highest possible value - {val}.".format(
                 val=self._maximum_reconnect_max_tries))
@@ -257,15 +256,15 @@
             self.reconnect_max_delay = reconnect_max_delay
         
         self.connect_timeout = connect_timeout
         self.socket_url = websocket_endpoint+"?auth_token="+access_token
         self.access_token = access_token
         self.socket_token = self.__getSocketToken__(self.access_token)
 
-        self.debug = True
+        self.debug = debug
         # self.on_price_update = None
         self.on_price_update = None
         self.on_open = None
         self.on_close = None
         self.on_error = None
         self.on_connect = None
         self.on_message = None
@@ -275,15 +274,15 @@
         self.subscribed_tokens = {}
         pass
 
     def __getSocketToken__(self,access_token: str)->str:
         return 
     
     def _create_connection(self, url, **kwargs):
-        self.factory = ClientFactory(url, **kwargs)
+        self.factory = ClientFactory(url,self.debug, **kwargs)
         self.ws = self.factory.ws
         self.factory.debug = self.debug
 
         self.factory.on_open = self._on_open
         self.factory.on_error = self._on_error
         self.factory.on_close = self._on_close
         self.factory.on_message = self._on_message
@@ -356,40 +355,40 @@
         reactor.stop()
 
     def stop_retry(self):
         """Stop auto retry when it is in progress."""
         if self.factory:
             self.factory.stopTrying()
 
-    def subscribe(self, exchange,token,mode):
+    def subscribe(self, exchange: str,token: int,mode: str)->bool:
         """
         Subscribe to a list of instrument_tokens.
         - `instrument_tokens` is list of instrument instrument_tokens to subscribe
         """
         try:
-            self.ws.sendMessage(six.b(json.dumps({"message_type": self._message_subscribe, "segment_id": exchange,"token": token,"mode": mode})))     
+            self.ws.sendMessage(six.b(json.dumps({"message_type": self._message_subscribe, "exchange": exchange,"token": token,"mode": mode})))     
 
             try: 
                 self.subscribed_tokens[exchange][token] = mode
             except KeyError: 
                 self.subscribed_tokens[exchange] = {}
                 self.subscribed_tokens[exchange][token] = mode
 
             return True
         except Exception as e:
             self._close(reason="Error while subscribe: {}".format(str(e)))
             raise
 
-    def unsubscribe(self, exchange,token):
+    def unsubscribe(self, exchange: str,token: int)->bool:
         """
         Unsubscribe the given list of instrument_tokens.
         - `instrument_tokens` is list of instrument_tokens to unsubscribe.
         """
         try:
-            self.ws.sendMessage(six.b(json.dumps({"message_type": self._message_unsubscribe, "segment_id": exchange,"token": token})))            
+            self.ws.sendMessage(six.b(json.dumps({"message_type": self._message_unsubscribe, "exchange": exchange,"token": token})))            
 
             try: 
                 del(self.subscribed_tokens[exchange][token])
             except KeyError: 
                 pass 
 
             return True
@@ -399,29 +398,15 @@
 
     def resubscribe(self):
         """Resubscribe to all current subscribed tokens."""
         modes = {}
 
         for exchange in self.subscribed_tokens: 
             for token in self.subscribed_tokens[exchange]: 
-                self.subscribe(exchange=exchange, token=token)
-
-        for token in self.subscribed_tokens:
-            m = self.subscribed_tokens[token]
-
-            if not modes.get(m):
-                modes[m] = []
-
-            modes[m].append(token)
-
-        for mode in modes:
-            if self.debug:
-                log.debug("Resubscribe and set mode: {} - {}".format(mode, modes[mode]))
-
-            self.subscribe(modes[mode])
+                self.subscribe(exchange=exchange, token=token,mode=self.subscribed_tokens[exchange][token])
 
     def _on_connect(self, ws, response):
         self.ws = ws
         if self.on_connect:
             self.on_connect(self, response)
 
     def _on_close(self, ws, code, reason):
```

### Comparing `vortex_api-1.0.6.dev2/vortex_api.egg-info/PKG-INFO` & `vortex_api-1.0.6.dev3/vortex_api.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex-api
-Version: 1.0.6.dev2
+Version: 1.0.6.dev3
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
@@ -60,29 +60,43 @@
 ```
 
 # Connecting to websocket
 
 ```
 from vortex_api import VortexFeed
 from vortex_api import Constants as Vc
+import time
 
 def main():
-       # Get access token from any of the login methods
-       wire = VortexFeed(access_token) 
+    # Get access token from any of the login methods
+    wire = VortexFeed(access_token) 
+
+    wire.on_price_update = on_price_update
+    wire.on_order_update = on_order_update
+    wire.on_connect = on_connect
+    wire.connect(threaded=True) 
+    # If you make threaded = False, anything after this line will not execute
+
+    time.sleep(10)
+    
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000)
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 26009)
+    wire.unsubscribe(Vc.ExchangeTypes.NSE_EQUITY, 2885)
 
-       wire.on_price_update = on_price_update
-       wire.on_order_update = on_order_update
-       wire.on_connect = on_connect
 
 def on_price_update(ws,data): 
-       print(data)
+    print(data)
 
 def on_order_update(ws,data): 
-       print(data)
+    print(data)
 
 def on_connect(ws, response):
-       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to NIFTY 50 
-       ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000) # Subscribe to BANKNIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26000, Vc.QuoteModes.LTP) #Subscribe to NIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 26009,Vc.QuoteModes.OHLCV) # Subscribe to BANKNIFTY 
+    ws.subscribe(Vc.ExchangeTypes.NSE_EQUITY, 2885,Vc.QuoteModes.FULL) # Subscribe to RELIANCE 
+
+if __name__ == "__main__":
+    main()
 
 ```
 Refer to the [python document](https://vortex.asthatrade.com/docs/pyvortex/vortex_api.html) for all methods and features
```

