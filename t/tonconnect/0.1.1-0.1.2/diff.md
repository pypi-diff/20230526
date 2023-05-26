# Comparing `tmp/tonconnect-0.1.1.tar.gz` & `tmp/tonconnect-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonconnect-0.1.1.tar", last modified: Mon May 15 14:06:44 2023, max compression
+gzip compressed data, was "tonconnect-0.1.2.tar", last modified: Fri May 26 12:46:35 2023, max compression
```

## Comparing `tonconnect-0.1.1.tar` & `tonconnect-0.1.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.1.1/.gitignore
--rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.1.1/LICENSE.md
--rw-r--r--   0        0        0     2479 2023-05-15 14:06:16.868138 tonconnect-0.1.1/README.md
--rw-r--r--   0        0        0      288 2023-05-15 13:57:22.007525 tonconnect-0.1.1/examples/address.py
--rw-r--r--   0        0        0      324 2023-05-15 13:59:35.231854 tonconnect-0.1.1/examples/all_versions_support.py
--rw-r--r--   0        0        0      464 2023-05-15 13:57:18.790724 tonconnect-0.1.1/examples/async_address.py
--rw-r--r--   0        0        0      782 2023-04-21 11:32:11.563469 tonconnect-0.1.1/examples/transactions.py
--rw-r--r--   0        0        0      556 2023-05-15 13:59:54.795490 tonconnect-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.1.1/tonconnect/__init__.py
--rw-r--r--   0        0        0      261 2023-04-25 17:59:41.572138 tonconnect-0.1.1/tonconnect/apps.py
--rw-r--r--   0        0        0     3759 2023-04-25 18:07:17.059721 tonconnect-0.1.1/tonconnect/bridge.py
--rw-r--r--   0        0        0     3973 2023-05-15 13:58:03.508537 tonconnect-0.1.1/tonconnect/connector.py
--rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.1.1/tonconnect/crypto.py
--rw-r--r--   0        0        0     3442 2023-04-12 07:39:01.886103 tonconnect-0.1.1/tonconnect/events.py
--rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.1.1/tonconnect/exceptions.py
--rw-r--r--   0        0        0     2930 2023-04-25 18:02:37.265076 tonconnect-0.1.1/tonconnect/httpbridge.py
--rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.1.1/tonconnect/options.py
--rw-r--r--   0        0        0     1733 2023-04-24 10:38:25.387486 tonconnect-0.1.1/tonconnect/requests.py
--rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.1.1/tonconnect/static.py
--rw-r--r--   0        0        0      330 2023-05-12 16:46:40.731106 tonconnect-0.1.1/tonconnect/url.py
--rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.1.1/tonconnect/utils.py
--rw-r--r--   0        0        0      416 2023-04-25 17:06:44.302885 tonconnect-0.1.1/tonconnect/wallet.py
--rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 tonconnect-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       34 2023-04-14 20:07:11.801816 tonconnect-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11350 2023-04-14 20:08:17.432870 tonconnect-0.1.2/LICENSE.md
+-rw-r--r--   0        0        0     2501 2023-05-26 12:46:02.932893 tonconnect-0.1.2/README.md
+-rw-r--r--   0        0        0      288 2023-05-26 09:22:35.528472 tonconnect-0.1.2/examples/address.py
+-rw-r--r--   0        0        0      324 2023-05-15 14:11:06.445617 tonconnect-0.1.2/examples/all_versions_support.py
+-rw-r--r--   0        0        0      464 2023-05-26 12:33:52.390794 tonconnect-0.1.2/examples/async_address.py
+-rw-r--r--   0        0        0      782 2023-04-21 11:32:11.563469 tonconnect-0.1.2/examples/transactions.py
+-rw-r--r--   0        0        0      556 2023-05-26 12:46:07.691963 tonconnect-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-12 07:29:33.705331 tonconnect-0.1.2/tonconnect/__init__.py
+-rw-r--r--   0        0        0      261 2023-05-26 12:32:45.875304 tonconnect-0.1.2/tonconnect/apps.py
+-rw-r--r--   0        0        0     3759 2023-04-25 18:07:17.059721 tonconnect-0.1.2/tonconnect/bridge.py
+-rw-r--r--   0        0        0     4081 2023-05-26 12:44:26.568017 tonconnect-0.1.2/tonconnect/connector.py
+-rw-r--r--   0        0        0     1202 2023-04-12 07:19:51.920373 tonconnect-0.1.2/tonconnect/crypto.py
+-rw-r--r--   0        0        0     3442 2023-05-26 12:30:59.031168 tonconnect-0.1.2/tonconnect/events.py
+-rw-r--r--   0        0        0      162 2023-04-12 09:29:00.652526 tonconnect-0.1.2/tonconnect/exceptions.py
+-rw-r--r--   0        0        0     2930 2023-04-25 18:02:37.265076 tonconnect-0.1.2/tonconnect/httpbridge.py
+-rw-r--r--   0        0        0      472 2023-04-12 09:30:53.246514 tonconnect-0.1.2/tonconnect/options.py
+-rw-r--r--   0        0        0     1733 2023-04-24 10:38:25.387486 tonconnect-0.1.2/tonconnect/requests.py
+-rw-r--r--   0        0        0      320 2023-04-12 07:22:22.791632 tonconnect-0.1.2/tonconnect/static.py
+-rw-r--r--   0        0        0      330 2023-05-12 16:46:40.731106 tonconnect-0.1.2/tonconnect/url.py
+-rw-r--r--   0        0        0      225 2023-04-12 07:24:37.312579 tonconnect-0.1.2/tonconnect/utils.py
+-rw-r--r--   0        0        0      416 2023-04-25 17:06:44.302885 tonconnect-0.1.2/tonconnect/wallet.py
+-rw-r--r--   0        0        0     2997 1970-01-01 00:00:00.000000 tonconnect-0.1.2/PKG-INFO
```

### Comparing `tonconnect-0.1.1/LICENSE.md` & `tonconnect-0.1.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.1/README.md` & `tonconnect-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,16 @@
 
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.1.2
+    * Bug fix
 * 0.1.1
     * Added tonapi.io support
 * 0.1.0
     * Async wrapper
 * 0.0.2 & 0.0.3
     * pyproject.toml fix
 * 0.0.1
```

### Comparing `tonconnect-0.1.1/examples/transactions.py` & `tonconnect-0.1.2/examples/transactions.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.1/pyproject.toml` & `tonconnect-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "tonconnect"
 description = "TON Connect - Python library for using TON Connect 2."
 readme = "README.md"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
     {name = "Vlad100"}
 ]
 dependencies = [
     "pynacl",
     "requests",
     "tonsdk",
```

### Comparing `tonconnect-0.1.1/tonconnect/bridge.py` & `tonconnect-0.1.2/tonconnect/bridge.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.1/tonconnect/connector.py` & `tonconnect-0.1.2/tonconnect/connector.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,35 +17,38 @@
         self.metadata_url = metadata
         self.metadata: Metadata = None
         self.wallet: Wallet = None
         self.bridge: Bridge = None
         self.use_tonapi: bool = use_tonapi
         self.tonapi_token: str = tonapi_token
     
-    def connect(self, wallet: str, payload: str):
+    def connect(self, wallet: Wallet, payload: str):
         metadata = Metadata(self.metadata_url, [AddressRequestOption(), ProofRequestOption(payload)])
         
-        if wallet not in APPS:
-            raise ConnectorException(f'Unknown wallet {wallet}.')
-        
-        self.wallet = APPS[wallet]()
+        if isinstance(wallet, str):
+            if wallet not in APPS:
+                raise ConnectorException(f'Unknown wallet {wallet}.')
+            
+            wallet = APPS[wallet]()
+            
+        self.wallet = wallet
         self.bridge = self.wallet.bridge
         
         self.bridge.connect(self.session)
         return self.wallet.get_url(metadata)
     
     def get_address(self):
         event = self.bridge.get_event()
         
         return self.check_address_proof_event(event)
     
     def get_verify_key(self, address: str) -> str:
         result = requests.get(f'https://tonapi.io/v2/blockchain/accounts/{address}/methods/get_public_key', headers={'Authorization': self.tonapi_token})
         json = result.json()
-        verify_key = VerifyKey(key=int(json['decoded']['public_key']).to_bytes(32, byteorder='big'))
+        verify_key = VerifyKey(key=int(json['stack'][-1]['num'][2:], base=16).to_bytes(32, byteorder='big'))
         
         return verify_key
     
     def check_address_proof_event(self, event: ConnectEvent):
         if event.address is None or event.proof is None:
             raise ConnectorException('Getting address without ton proof and ton address.')
         
@@ -77,15 +80,15 @@
         
         return await self.check_address_proof_event(event)
     
     async def get_verify_key(self, address: str):
         async with aiohttp.ClientSession() as client:
             result = await client.get(f'https://tonapi.io/v2/blockchain/accounts/{address}/methods/get_public_key', headers={'Authorization': self.tonapi_token})
             json = await result.json()
-            verify_key = VerifyKey(key=int(json['decoded']['public_key']).to_bytes(32, byteorder='big'))
+            verify_key = VerifyKey(key=int(json['stack'][-1]['num'][2:], base=16).to_bytes(32, byteorder='big'))
         
         return verify_key
 
     async def check_address_proof_event(self, event: ConnectEvent):
         if event.address is None or event.proof is None:
             raise ConnectorException('Getting address without ton proof and ton address.')
```

### Comparing `tonconnect-0.1.1/tonconnect/crypto.py` & `tonconnect-0.1.2/tonconnect/crypto.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.1/tonconnect/events.py` & `tonconnect-0.1.2/tonconnect/events.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.1/tonconnect/httpbridge.py` & `tonconnect-0.1.2/tonconnect/httpbridge.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.1/tonconnect/requests.py` & `tonconnect-0.1.2/tonconnect/requests.py`

 * *Files identical despite different names*

### Comparing `tonconnect-0.1.1/PKG-INFO` & `tonconnect-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tonconnect
-Version: 0.1.1
+Version: 0.1.2
 Summary: TON Connect - Python library for using TON Connect 2.
 Author: Vlad100
 Description-Content-Type: text/markdown
 Requires-Dist: pynacl
 Requires-Dist: requests
 Requires-Dist: tonsdk
 Requires-Dist: aiohttp
@@ -94,14 +94,16 @@
 
 ## Authors
 
 [@Vlad10081](https://t.me/dalvgames)
 
 ## Version History
 
+* 0.1.2
+    * Bug fix
 * 0.1.1
     * Added tonapi.io support
 * 0.1.0
     * Async wrapper
 * 0.0.2 & 0.0.3
     * pyproject.toml fix
 * 0.0.1
```

