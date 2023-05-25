# Comparing `tmp/rivian_python_client-0.2.2.tar.gz` & `tmp/rivian_python_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rivian_python_client-0.2.2.tar", max compression
+gzip compressed data, was "rivian_python_client-0.2.3.tar", max compression
```

## Comparing `rivian_python_client-0.2.2.tar` & `rivian_python_client-0.2.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      325 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/README.md
--rw-r--r--   0        0        0      555 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      102 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/__init__.py
--rw-r--r--   0        0        0     2888 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/const.py
--rw-r--r--   0        0        0      779 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/exceptions.py
--rw-r--r--   0        0        0    23660 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/rivian.py
--rw-r--r--   0        0        0     7280 2023-05-24 00:28:52.005462 rivian_python_client-0.2.2/src/rivian/ws_monitor.py
--rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 rivian_python_client-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      325 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/README.md
+-rw-r--r--   0        0        0      555 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0      102 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/__init__.py
+-rw-r--r--   0        0        0     2888 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/const.py
+-rw-r--r--   0        0        0      779 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/exceptions.py
+-rw-r--r--   0        0        0    23660 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/rivian.py
+-rw-r--r--   0        0        0     7356 2023-05-25 23:07:28.617647 rivian_python_client-0.2.3/src/rivian/ws_monitor.py
+-rw-r--r--   0        0        0      883 1970-01-01 00:00:00.000000 rivian_python_client-0.2.3/PKG-INFO
```

### Comparing `rivian_python_client-0.2.2/pyproject.toml` & `rivian_python_client-0.2.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rivian-python-client"
-version = "0.2.2"
+version = "0.2.3"
 description = "Rivian API Client (Unofficial)"
 readme = "README.md"
 authors = ["Brian Retterer <bretterer@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "rivian", from = "src" },
 ]
```

### Comparing `rivian_python_client-0.2.2/src/rivian/const.py` & `rivian_python_client-0.2.3/src/rivian/const.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-0.2.2/src/rivian/exceptions.py` & `rivian_python_client-0.2.3/src/rivian/exceptions.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-0.2.2/src/rivian/rivian.py` & `rivian_python_client-0.2.3/src/rivian/rivian.py`

 * *Files identical despite different names*

### Comparing `rivian_python_client-0.2.2/src/rivian/ws_monitor.py` & `rivian_python_client-0.2.3/src/rivian/ws_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,14 +128,16 @@
         if not (websocket := self._ws):
             return
         while not websocket.closed:
             try:
                 msg = await websocket.receive(timeout=60)
                 if msg.type in (WSMsgType.CLOSE, WSMsgType.CLOSING, WSMsgType.CLOSED):
                     self._log_message(msg)
+                    if msg.extra == "Unauthenticated":
+                        self._disconnect = True
                     break
                 self._last_received = datetime.now(timezone.utc)
                 if msg.type == WSMsgType.TEXT:
                     data = loads(msg.data)
                     if (data_type := data.get("type")) == "connection_ack":
                         self._connection_ack.set()
                     elif data_type == "next":
@@ -152,15 +154,15 @@
         self._connection_ack.clear()
         self._log_message("web socket stopped")
 
     async def _monitor(self) -> None:
         """Monitor a web socket connection."""
         attempt = 0
         while not self._disconnect:
-            while self.connected or not self._subscriptions:
+            while self.connected:
                 if self._receiver_task.done():  # Need to restart the receiver
                     self._receiver_task = asyncio.ensure_future(self._receiver())
                 await asyncio.sleep(1)
             if not self._disconnect:
                 try:
                     await self.new_connection()
                 except Exception as ex:  # pylint: disable=broad-except
```

### Comparing `rivian_python_client-0.2.2/PKG-INFO` & `rivian_python_client-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rivian-python-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Rivian API Client (Unofficial)
 License: MIT
 Author: Brian Retterer
 Author-email: bretterer@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

