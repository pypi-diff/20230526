# Comparing `tmp/communica-0.2.1b3.tar.gz` & `tmp/communica-0.2.1b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "communica-0.2.1b3.tar", last modified: Sun May 21 12:33:33 2023, max compression
+gzip compressed data, was "communica-0.2.1b4.tar", last modified: Fri May 26 08:36:15 2023, max compression
```

## Comparing `communica-0.2.1b3.tar` & `communica-0.2.1b4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 12:33:33.842145 communica-0.2.1b3/
--rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b3/LICENSE.txt
--rw-rw-rw-   0        0        0     2233 2023-05-21 12:33:33.842145 communica-0.2.1b3/PKG-INFO
--rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 12:33:33.814145 communica-0.2.1b3/communica/
--rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b3/communica/__init__.py
--rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b3/communica/clients.py
-drwxrwxrwx   0        0        0        0 2023-05-21 12:33:33.826645 communica-0.2.1b3/communica/connectors/
--rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b3/communica/connectors/__init__.py
--rw-rw-rw-   0        0        0     2835 2023-05-21 11:38:53.000000 communica-0.2.1b3/communica/connectors/_stream_local.py
--rw-rw-rw-   0        0        0     5455 2023-05-01 12:51:49.000000 communica-0.2.1b3/communica/connectors/base.py
--rw-rw-rw-   0        0        0    28038 2023-05-08 07:38:53.000000 communica-0.2.1b3/communica/connectors/rabbitmq.py
--rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.1b3/communica/connectors/stream.py
--rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b3/communica/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-21 12:33:33.831145 communica-0.2.1b3/communica/pairs/
--rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b3/communica/pairs/__init__.py
--rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b3/communica/pairs/base.py
--rw-rw-rw-   0        0        0     9865 2023-05-21 12:18:42.000000 communica-0.2.1b3/communica/pairs/route.py
--rw-rw-rw-   0        0        0    16118 2023-05-21 12:16:21.000000 communica-0.2.1b3/communica/pairs/simple.py
-drwxrwxrwx   0        0        0        0 2023-05-21 12:33:33.836147 communica-0.2.1b3/communica/serializers/
--rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b3/communica/serializers/__init__.py
--rw-rw-rw-   0        0        0     1274 2023-05-09 20:44:57.000000 communica-0.2.1b3/communica/serializers/adaptix.py
--rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b3/communica/serializers/base.py
--rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b3/communica/serializers/json.py
--rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b3/communica/servers.py
--rw-rw-rw-   0        0        0     4246 2023-05-21 11:53:38.000000 communica-0.2.1b3/communica/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-21 12:33:33.820646 communica-0.2.1b3/communica.egg-info/
--rw-rw-rw-   0        0        0     2233 2023-05-21 12:33:33.000000 communica-0.2.1b3/communica.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      811 2023-05-21 12:33:33.000000 communica-0.2.1b3/communica.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 12:33:33.000000 communica-0.2.1b3/communica.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      164 2023-05-21 12:33:33.000000 communica-0.2.1b3/communica.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-21 12:33:33.000000 communica-0.2.1b3/communica.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1130 2023-05-21 12:24:50.000000 communica-0.2.1b3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-21 12:33:33.842646 communica-0.2.1b3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-21 12:33:33.841146 communica-0.2.1b3/tests/
--rw-rw-rw-   0        0        0     2146 2023-05-04 12:13:21.000000 communica-0.2.1b3/tests/test_connectors.py
--rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b3/tests/test_entities.py
--rw-rw-rw-   0        0        0     2481 2023-04-23 14:30:49.000000 communica-0.2.1b3/tests/test_rmq_conn_check_policy.py
--rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b3/tests/test_serializers.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.798051 communica-0.2.1b4/
+-rw-rw-rw-   0        0        0      568 2023-03-25 20:48:52.000000 communica-0.2.1b4/LICENSE.txt
+-rw-rw-rw-   0        0        0     2233 2023-05-26 08:36:15.797552 communica-0.2.1b4/PKG-INFO
+-rw-rw-rw-   0        0        0     1456 2023-04-04 20:46:58.000000 communica-0.2.1b4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.777051 communica-0.2.1b4/communica/
+-rw-rw-rw-   0        0        0      101 2023-02-15 13:48:00.000000 communica-0.2.1b4/communica/__init__.py
+-rw-rw-rw-   0        0        0      130 2023-03-19 21:29:46.000000 communica-0.2.1b4/communica/clients.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.786050 communica-0.2.1b4/communica/connectors/
+-rw-rw-rw-   0        0        0      170 2023-03-31 19:34:58.000000 communica-0.2.1b4/communica/connectors/__init__.py
+-rw-rw-rw-   0        0        0     2835 2023-05-21 11:38:53.000000 communica-0.2.1b4/communica/connectors/_stream_local.py
+-rw-rw-rw-   0        0        0     5455 2023-05-01 12:51:49.000000 communica-0.2.1b4/communica/connectors/base.py
+-rw-rw-rw-   0        0        0    28038 2023-05-08 07:38:53.000000 communica-0.2.1b4/communica/connectors/rabbitmq.py
+-rw-rw-rw-   0        0        0    10130 2023-05-21 11:36:08.000000 communica-0.2.1b4/communica/connectors/stream.py
+-rw-rw-rw-   0        0        0     1945 2023-05-08 09:05:11.000000 communica-0.2.1b4/communica/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.789551 communica-0.2.1b4/communica/pairs/
+-rw-rw-rw-   0        0        0      223 2023-03-19 15:01:07.000000 communica-0.2.1b4/communica/pairs/__init__.py
+-rw-rw-rw-   0        0        0     2975 2023-05-04 13:02:31.000000 communica-0.2.1b4/communica/pairs/base.py
+-rw-rw-rw-   0        0        0     9863 2023-05-21 12:35:07.000000 communica-0.2.1b4/communica/pairs/route.py
+-rw-rw-rw-   0        0        0    16180 2023-05-23 13:25:30.000000 communica-0.2.1b4/communica/pairs/simple.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.793551 communica-0.2.1b4/communica/serializers/
+-rw-rw-rw-   0        0        0      242 2023-05-08 07:15:52.000000 communica-0.2.1b4/communica/serializers/__init__.py
+-rw-rw-rw-   0        0        0     1672 2023-05-23 11:23:18.000000 communica-0.2.1b4/communica/serializers/adaptix.py
+-rw-rw-rw-   0        0        0      657 2023-03-18 18:41:17.000000 communica-0.2.1b4/communica/serializers/base.py
+-rw-rw-rw-   0        0        0      315 2023-03-18 19:40:10.000000 communica-0.2.1b4/communica/serializers/json.py
+-rw-rw-rw-   0        0        0      128 2023-03-19 21:29:36.000000 communica-0.2.1b4/communica/servers.py
+-rw-rw-rw-   0        0        0     4246 2023-05-21 11:53:38.000000 communica-0.2.1b4/communica/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.781051 communica-0.2.1b4/communica.egg-info/
+-rw-rw-rw-   0        0        0     2233 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      811 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      164 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-26 08:36:15.000000 communica-0.2.1b4/communica.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1130 2023-05-26 08:35:41.000000 communica-0.2.1b4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 08:36:15.798051 communica-0.2.1b4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 08:36:15.797051 communica-0.2.1b4/tests/
+-rw-rw-rw-   0        0        0     2146 2023-05-04 12:13:21.000000 communica-0.2.1b4/tests/test_connectors.py
+-rw-rw-rw-   0        0        0     6508 2023-05-08 10:49:51.000000 communica-0.2.1b4/tests/test_entities.py
+-rw-rw-rw-   0        0        0     2481 2023-04-23 14:30:49.000000 communica-0.2.1b4/tests/test_rmq_conn_check_policy.py
+-rw-rw-rw-   0        0        0     1081 2023-05-08 10:22:35.000000 communica-0.2.1b4/tests/test_serializers.py
```

### Comparing `communica-0.2.1b3/LICENSE.txt` & `communica-0.2.1b4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/PKG-INFO` & `communica-0.2.1b4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b3
+Version: 0.2.1b4
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b3/README.md` & `communica-0.2.1b4/README.md`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica/connectors/_stream_local.py` & `communica-0.2.1b4/communica/connectors/_stream_local.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica/connectors/base.py` & `communica-0.2.1b4/communica/connectors/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica/connectors/rabbitmq.py` & `communica-0.2.1b4/communica/connectors/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica/connectors/stream.py` & `communica-0.2.1b4/communica/connectors/stream.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica/exceptions.py` & `communica-0.2.1b4/communica/exceptions.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica/pairs/base.py` & `communica-0.2.1b4/communica/pairs/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica/pairs/route.py` & `communica-0.2.1b4/communica/pairs/route.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         return decorator
 
     async def request(
             self,
             route: str,
             data: Any,
             serializer: 'BaseSerializer | None' = None
-    ) -> bytes:
+    ) -> Any:
         """
         Send request, wait response.
 
         Args:
             route: Handler identifier
             client_id: If omitted or None, random client will be chosen
         """
```

### Comparing `communica-0.2.1b3/communica/pairs/simple.py` & `communica-0.2.1b4/communica/pairs/simple.py`

 * *Files 0% similar despite different names*

```diff
@@ -347,15 +347,15 @@
 
         self._client_id = client_id or uuid4().hex
         self._run_task = None
 
     def _not_defined_handler(self, data: Any):
         raise RespError('Client side not defined handler for server requests')
 
-    async def request(self, data: Any) -> bytes:
+    async def request(self, data: Any) -> Any:
         """Send request, wait response."""
         return await self._flow.request(data)
 
     async def throw(self, data: Any) -> None:
         """Send request without waiting response."""
         return await self._flow.throw(data)
 
@@ -370,14 +370,17 @@
     async def init(self):
         if not hasattr(self, '_server') or not self._server.is_serving():
             self._server = await self.connector.server_start(
                 self._handshaker, self._on_client_connect)
         return self
 
     async def close(self) -> None:
+        if not hasattr(self, '_server'):
+            return
+
         self._server.close()
         await self._server.wait_closed()
 
         for client_id, flow in self._known_clients.items():
             if isinstance(flow, ReqRepMessageFlow):
                 self._cancel_handler_tasks(flow)
                 await flow._connection.close()
```

### Comparing `communica-0.2.1b3/communica/serializers/adaptix.py` & `communica-0.2.1b4/communica/serializers/adaptix.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 TReq = TypeVar('TReq')
 TResp = TypeVar('TResp')
 
 
 class AdaptixSerializer(BaseSerializer, Generic[TReq, TResp]):
     __slots__ = ('_retort', '_req_model', '_resp_model')
 
+    # XXX: один из вариантов
+    # FROM_HANDLER = специальное значение
+    # если регистратор ручки видит это значение вместо сериалайзера,
+    # он берет ручку и через какой-нибудь метод собирает сериалайзер
+    # по сигнатуре ручки
+
     def __init__(
             self,
             request_model: Type[TReq],
             response_model: 'Type[TResp] | None' = None,
             retort: 'adaptix.Retort | None' = None
     ) -> None:
         if not _HAVE_ADAPTIX:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `communica-0.2.1b3/communica/serializers/base.py` & `communica-0.2.1b4/communica/serializers/base.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica/utils.py` & `communica-0.2.1b4/communica/utils.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/communica.egg-info/PKG-INFO` & `communica-0.2.1b4/communica.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: communica
-Version: 0.2.1b3
+Version: 0.2.1b4
 Summary: Easy to use IPC library
 Author-email: Elchin Sarkarov <elchin751@gmail.com>
 Project-URL: Homepage, https://github.com/elchinchel/communica-py
 Project-URL: Bug Tracker, https://github.com/elchinchel/communica-py/issues
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `communica-0.2.1b3/communica.egg-info/SOURCES.txt` & `communica-0.2.1b4/communica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/pyproject.toml` & `communica-0.2.1b4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "communica"
-version = "0.2.1b3"
+version = "0.2.1b4"
 authors = [
   { name="Elchin Sarkarov", email="elchin751@gmail.com" },
 ]
 description = "Easy to use IPC library"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `communica-0.2.1b3/tests/test_connectors.py` & `communica-0.2.1b4/tests/test_connectors.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/tests/test_entities.py` & `communica-0.2.1b4/tests/test_entities.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/tests/test_rmq_conn_check_policy.py` & `communica-0.2.1b4/tests/test_rmq_conn_check_policy.py`

 * *Files identical despite different names*

### Comparing `communica-0.2.1b3/tests/test_serializers.py` & `communica-0.2.1b4/tests/test_serializers.py`

 * *Files identical despite different names*

