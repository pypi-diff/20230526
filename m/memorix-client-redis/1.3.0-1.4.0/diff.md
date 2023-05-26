# Comparing `tmp/memorix_client_redis-1.3.0.tar.gz` & `tmp/memorix_client_redis-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memorix_client_redis-1.3.0.tar", max compression
+gzip compressed data, was "memorix_client_redis-1.4.0.tar", max compression
```

## Comparing `memorix_client_redis-1.3.0.tar` & `memorix_client_redis-1.4.0.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     1200 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/__init__.py
--rw-r--r--   0        0        0      365 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/example-schema.memorix
--rw-r--r--   0        0        0     2731 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/example_schema_generated.py
--rw-r--r--   0        0        0        0 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/__init__.py
--rw-r--r--   0        0        0     3073 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/api.py
--rw-r--r--   0        0        0        0 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/cache/__init__.py
--rw-r--r--   0        0        0      114 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/cache/cache_api.py
--rw-r--r--   0        0        0     5882 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/cache/cache_item.py
--rw-r--r--   0        0        0     1120 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/cache/cache_options.py
--rw-r--r--   0        0        0      255 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/hash_key.py
--rw-r--r--   0        0        0     1488 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/json.py
--rw-r--r--   0        0        0        0 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/pubsub/__init__.py
--rw-r--r--   0        0        0      115 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/pubsub/pubsub_api.py
--rw-r--r--   0        0        0     3752 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/pubsub/pubsub_item.py
--rw-r--r--   0        0        0        0 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/task/__init__.py
--rw-r--r--   0        0        0      113 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/task/task_api.py
--rw-r--r--   0        0        0     9975 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/task/task_item.py
--rw-r--r--   0        0        0      454 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/features/api/task/task_options.py
--rw-r--r--   0        0        0        0 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/py.typed
--rw-r--r--   0        0        0     1463 2023-03-29 14:52:04.446641 memorix_client_redis-1.3.0/memorix_client_redis/start.py
--rw-r--r--   0        0        0      580 2023-03-29 14:52:51.647108 memorix_client_redis-1.3.0/pyproject.toml
--rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 memorix_client_redis-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0      706 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/cache/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/cache/cache_base.py
+-rw-r--r--   0        0        0     6028 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/cache/cache_item.py
+-rw-r--r--   0        0        0     1120 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/cache/cache_options.py
+-rw-r--r--   0        0        0      456 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/default_options.py
+-rw-r--r--   0        0        0      496 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/example-schema.memorix
+-rw-r--r--   0        0        0     2021 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/example_schema_generated.py
+-rw-r--r--   0        0        0      369 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/hash_key.py
+-rw-r--r--   0        0        0     1488 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/json.py
+-rw-r--r--   0        0        0     1037 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/memorix_base.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/pubsub/__init__.py
+-rw-r--r--   0        0        0      141 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/pubsub/pubsub_base.py
+-rw-r--r--   0        0        0     3892 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/pubsub/pubsub_item.py
+-rw-r--r--   0        0        0      217 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/redis_connection.py
+-rw-r--r--   0        0        0     1415 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/start.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/task/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/task/task_base.py
+-rw-r--r--   0        0        0    10093 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/task/task_item.py
+-rw-r--r--   0        0        0      454 2023-05-26 11:29:17.230481 memorix_client_redis-1.4.0/memorix_client_redis/task/task_options.py
+-rw-r--r--   0        0        0      580 2023-05-26 11:30:17.603054 memorix_client_redis-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0      484 1970-01-01 00:00:00.000000 memorix_client_redis-1.4.0/PKG-INFO
```

### Comparing `memorix_client_redis-1.3.0/memorix_client_redis/features/api/cache/cache_item.py` & `memorix_client_redis-1.4.0/memorix_client_redis/cache/cache_item.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 import asyncio
 import functools
-from memorix_client_redis.features.api.hash_key import hash_key
-from memorix_client_redis.features.api.json import from_json, to_json, bytes_to_str
+from memorix_client_redis.hash_key import hash_key
+from memorix_client_redis.json import from_json, to_json, bytes_to_str
 from typing import Generic, Optional, Type, TypeVar, cast
-from ..api import Api, ApiDefaults
+from memorix_client_redis.memorix_base import MemorixBase
 from .cache_options import CacheOptions
 
 KT = TypeVar("KT")
 PT = TypeVar("PT")
 
 
 class CacheItem(Generic[KT, PT]):
+    Options = CacheOptions
+
     def __init__(
         self,
-        api: Api,
+        api: MemorixBase,
         id: str,
         payload_class: Type[PT],
         options: Optional[CacheOptions] = None,
     ) -> None:
         self._api = api
         self._id = id
         self._payload_class = payload_class
@@ -25,27 +27,27 @@
 
     def get(
         self,
         key: KT,
         options: Optional[CacheOptions] = None,
     ) -> Optional[PT]:
         merged_options = self._options
-        try:
+        if self._api._default_options is not None:
             merged_options = CacheOptions.merge(
-                cast(ApiDefaults, self._api._defaults).cache_set_options,
+                self._api._default_options.cache,
                 self._options,
             )
-        except AttributeError:
-            pass
         merged_options = CacheOptions.merge(
             merged_options,
             options,
         )
 
-        data_bytes = self._api._redis.get(hash_key(self._id, key=key))
+        data_bytes = self._api._connection.redis.get(
+            hash_key(api=self._api, id=self._id, key=key),
+        )
         if data_bytes is None:
             return None
         if (
             merged_options is not None
             and merged_options.expire is not None
             and merged_options.expire.extend_on_get
         ):
@@ -70,29 +72,27 @@
     def set(
         self,
         key: KT,
         payload: PT,
         options: Optional[CacheOptions] = None,
     ) -> Optional[bool]:
         merged_options = self._options
-        try:
+        if self._api._default_options is not None:
             merged_options = CacheOptions.merge(
-                cast(ApiDefaults, self._api._defaults).cache_set_options,
+                self._api._default_options.cache,
                 self._options,
             )
-        except AttributeError:
-            pass
         merged_options = CacheOptions.merge(
             merged_options,
             options,
         )
 
         payload_json = to_json(payload)
-        return self._api._redis.set(
-            hash_key(self._id, key=key),
+        return self._api._connection.redis.set(
+            hash_key(api=self._api, id=self._id, key=key),
             payload_json,
             ex=merged_options.expire.value
             if merged_options is not None
             and merged_options.expire is not None
             and not merged_options.expire.is_in_ms
             else None,
             px=merged_options.expire.value
@@ -122,30 +122,34 @@
         return res
 
     def extend(
         self,
         key: KT,
     ) -> None:
         merged_options = self._options
-        try:
+        if self._api._default_options is not None:
             merged_options = CacheOptions.merge(
-                cast(ApiDefaults, self._api._defaults).cache_set_options,
+                self._api._default_options.cache,
                 self._options,
             )
-        except AttributeError:
-            pass
         if merged_options is None or merged_options.expire is None:
             return
 
-        hashed_key = hash_key(self._id, key=key)
+        hashed_key = hash_key(api=self._api, id=self._id, key=key)
 
         if merged_options.expire.is_in_ms:
-            self._api._redis.pexpire(hashed_key, merged_options.expire.value)
+            self._api._connection.redis.pexpire(
+                hashed_key,
+                merged_options.expire.value,
+            )
         else:
-            self._api._redis.expire(hashed_key, merged_options.expire.value)
+            self._api._connection.redis.expire(
+                hashed_key,
+                merged_options.expire.value,
+            )
 
     async def async_extend(
         self,
         key: KT,
     ) -> None:
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
```

### Comparing `memorix_client_redis-1.3.0/memorix_client_redis/features/api/cache/cache_options.py` & `memorix_client_redis-1.4.0/memorix_client_redis/cache/cache_options.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.3.0/memorix_client_redis/features/api/json.py` & `memorix_client_redis-1.4.0/memorix_client_redis/json.py`

 * *Files identical despite different names*

### Comparing `memorix_client_redis-1.3.0/memorix_client_redis/features/api/pubsub/pubsub_item.py` & `memorix_client_redis-1.4.0/memorix_client_redis/pubsub/pubsub_item.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import asyncio
 import functools
-from memorix_client_redis.features.api.hash_key import hash_key
-from memorix_client_redis.features.api.json import from_json, to_json, bytes_to_str
-from ..api import Api
+from memorix_client_redis.hash_key import hash_key
+from memorix_client_redis.json import from_json, to_json, bytes_to_str
+from memorix_client_redis.memorix_base import MemorixBase
 from typing import AsyncGenerator, Dict, Generator, Generic, Type, TypeVar, Union, cast
 
 KT = TypeVar("KT")
 PT = TypeVar("PT")
 
 
 class PubSubItemPublish(object):
@@ -24,26 +24,26 @@
     ) -> None:
         self.payload = payload
 
 
 class PubSubItem(Generic[KT, PT]):
     def __init__(
         self,
-        api: Api,
+        api: MemorixBase,
         id: str,
         payload_class: Type[PT],
     ) -> None:
         self._api = api
         self._id = id
         self._payload_class = payload_class
 
     def publish(self, key: KT, payload: PT) -> PubSubItemPublish:
         payload_json = to_json(payload)
-        subscribers_size = self._api._redis.publish(
-            hash_key(self._id, key=key),
+        subscribers_size = self._api._connection.redis.publish(
+            hash_key(api=self._api, id=self._id, key=key),
             payload_json,
         )
         return PubSubItemPublish(subscribers_size=subscribers_size)
 
     async def async_publish(self, key: KT, payload: PT) -> PubSubItemPublish:
         loop = asyncio.get_running_loop()
         res = await loop.run_in_executor(
@@ -54,29 +54,32 @@
                 key=key,
                 payload=payload,
             ),
         )
         return res
 
     def subscribe(self, key: KT) -> Generator[PubSubItemSubscribe[PT], None, None]:
-        sub = self._api._redis.pubsub()
-        sub.subscribe(hash_key(self._id, key=key))
-        for message in cast(Generator[Dict[str, Union[int, bytes]], None, None], sub.listen()):  # type: ignore
+        sub = self._api._connection.redis.pubsub()
+        sub.subscribe(hash_key(api=self._api, id=self._id, key=key))
+        for message in cast(
+            Generator[Dict[str, Union[int, bytes]], None, None],
+            sub.listen(),  # type: ignore
+        ):
             data_bytes = message["data"]
             if isinstance(data_bytes, bytes):
                 data_str = bytes_to_str(data_bytes)
                 data = from_json(value=data_str, data_class=self._payload_class)
                 yield PubSubItemSubscribe(payload=data)
 
     async def async_subscribe(
         self,
         key: KT,
     ) -> AsyncGenerator[PubSubItemSubscribe[PT], None]:
-        sub = self._api._redis.pubsub()
-        sub.subscribe(hash_key(self._id, key=key))
+        sub = self._api._connection.redis.pubsub()
+        sub.subscribe(hash_key(api=self._api, id=self._id, key=key))
         loop = asyncio.get_running_loop()
         while True:
             message = await loop.run_in_executor(
                 None,
                 functools.partial(
                     sub.get_message,
                     ignore_subscribe_messages=True,
```

### Comparing `memorix_client_redis-1.3.0/memorix_client_redis/features/api/task/task_item.py` & `memorix_client_redis-1.4.0/memorix_client_redis/task/task_item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 import functools
-from memorix_client_redis.features.api.hash_key import hash_key
+from memorix_client_redis.hash_key import hash_key
 from uuid import uuid4
-from memorix_client_redis.features.api.json import from_json, to_json, bytes_to_str
+from memorix_client_redis.json import from_json, to_json, bytes_to_str
 import typing
-from ..api import Api, ApiDefaults
+from memorix_client_redis.memorix_base import MemorixBase
 from .task_options import TaskDequequeOptions
 
 KT = typing.TypeVar("KT")
 PT = typing.TypeVar("PT")
 RT = typing.TypeVar("RT")
 
 
@@ -72,17 +72,19 @@
         return typing.cast(
             TaskItemQueue,
             self._returns_task.async_queue(key=self._returns_id, payload=returns),
         )
 
 
 class TaskItem(typing.Generic[KT, PT, RT]):
+    Options = TaskDequequeOptions
+
     def __init__(
         self,
-        api: Api,
+        api: MemorixBase,
         id: str,
         payload_class: typing.Type[PT],
         returns_class: typing.Optional[typing.Type[RT]] = None,
         options: typing.Optional[TaskDequequeOptions] = None,
     ) -> None:
         self._api = api
         self._id = id
@@ -103,16 +105,16 @@
                 [returns_id, payload],
             )
         else:
             wrapped_payload_json = to_json(
                 [payload],
             )
 
-        queue_size = self._api._redis.rpush(
-            hash_key(self._id, key=key),
+        queue_size = self._api._connection.redis.rpush(
+            hash_key(api=self._api, id=self._id, key=key),
             wrapped_payload_json,
         )
         if returns_id is None:
             return typing.cast(
                 TaskItemQueueWithReturns[RT],
                 TaskItemQueue(queue_size=queue_size),
             )
@@ -128,34 +130,32 @@
 
     def dequeue(
         self,
         key: KT,
         options: typing.Optional[TaskDequequeOptions] = None,
     ) -> typing.Generator[TaskItemDequeueWithReturns[PT], None, None]:
         merged_options = self._options
-        try:
+        if self._api._default_options is not None:
             merged_options = TaskDequequeOptions.merge(
-                typing.cast(ApiDefaults, self._api._defaults).task_dequeque_options,
+                self._api._default_options.task,
                 self._options,
             )
-        except AttributeError:
-            pass
         merged_options = TaskDequequeOptions.merge(
             merged_options,
             options,
         )
 
         while True:
             if merged_options is not None and merged_options.take_newest:
-                [channel_bytes, data_bytes] = self._api._redis.brpop(
-                    hash_key(self._id, key=key),
+                [channel_bytes, data_bytes] = self._api._connection.redis.brpop(
+                    hash_key(api=self._api, id=self._id, key=key),
                 )
             else:
-                [channel_bytes, data_bytes] = self._api._redis.blpop(
-                    hash_key(self._id, key=key),
+                [channel_bytes, data_bytes] = self._api._connection.redis.blpop(
+                    hash_key(api=self._api, id=self._id, key=key),
                 )
 
             data_str = bytes_to_str(data_bytes)
 
             if hasattr(self, "_returns_task"):
                 seperator_index = data_str.index(",")
                 returns_id = data_str[2 : seperator_index - 1]
@@ -182,16 +182,16 @@
         self,
         key: KT,
     ) -> typing.AsyncGenerator[TaskItemDequeueWithReturns[PT], None]:
         print("dequeue async")
         yield typing.cast(TaskItemDequeueWithReturns[PT], None)
 
     def clear(self, key: KT) -> None:
-        self._api._redis.delete(
-            hash_key(self._id, key=key),
+        self._api._connection.redis.delete(
+            hash_key(api=self._api, id=self._id, key=key),
         )
 
     async def async_clear(self, key: KT) -> None:
         loop = asyncio.get_running_loop()
         await loop.run_in_executor(
             None,
             functools.partial(
@@ -227,15 +227,15 @@
     async def async_clear(self) -> None:  # type: ignore
         await TaskItem.async_clear(self, key=None)
 
 
 class TaskItemNoReturns(TaskItem[KT, PT, None]):
     def __init__(
         self,
-        api: Api,
+        api: MemorixBase,
         id: str,
         payload_class: typing.Type[PT],
     ) -> None:
         super().__init__(
             api=api,
             id=id,
             payload_class=payload_class,
```

### Comparing `memorix_client_redis-1.3.0/memorix_client_redis/start.py` & `memorix_client_redis-1.4.0/memorix_client_redis/start.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,54 @@
 import os
-from .example_schema_generated import Animal, MemorixApi, User
+from .example_schema_generated import Animal, Memorix, User
 import multiprocessing
 from time import sleep
 
 redis_url = os.environ["REDIS_URL"]
 
 
 def listen_to_message() -> None:
-    memorix_api = MemorixApi(redis_url=redis_url)
-    for res in memorix_api.pubsub.message.subscribe():
+    memorix = Memorix(redis_url=redis_url)
+    for res in memorix.pubsub.message.subscribe():
         print("message:", res.payload)
 
 
 def listen_to_algo() -> None:
-    memorix_api = MemorixApi(redis_url=redis_url)
-    for res in memorix_api.task.runAlgo.dequeue():
+    memorix = Memorix(redis_url=redis_url)
+    for res in memorix.task.runAlgo.dequeue():
         print("task:", res.payload)
         res.send_returns(returns=Animal.dog)
 
 
 def start() -> None:
-    memorix_api = MemorixApi(redis_url=redis_url)
+    memorix = Memorix(redis_url=redis_url)
 
-    memorix_api.cache.user.set("uv", User(name="uv", age=29))
+    memorix.cache.user.set("uv", User(name="uv", age=29))
 
-    user = memorix_api.cache.user.get("uv")
+    user = memorix.cache.user.get("uv")
     if user is None:
         raise Exception("Didn't get user from redis")
     print(user.age)
 
     process = multiprocessing.Process(target=listen_to_message)
     process.start()
 
     for _num in (1, 2, 3, 4):
         sleep(0.1)
-        res = memorix_api.pubsub.message.publish(payload="Heyy buddy")
+        res = memorix.pubsub.message.publish(payload="Heyy buddy")
         print("listeners:", res.subscribers_size)
 
     sleep(0.2)
     process.kill()
 
     task = multiprocessing.Process(target=listen_to_algo)
     task.start()
 
     for _num2 in (1, 2, 3, 4):
         sleep(0.1)
-        queue = memorix_api.task.runAlgo.queue(payload="Im a task!")
+        queue = memorix.task.runAlgo.queue(payload="Im a task!")
         print("queue_size:", queue.queue_size)
         res2 = queue.get_returns()
         print("animal:", res2.value)
 
     sleep(0.2)
     task.kill()
```

### Comparing `memorix_client_redis-1.3.0/pyproject.toml` & `memorix_client_redis-1.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "memorix_client_redis"
-version = "1.3.0"
+version = "1.4.0"
 description = ""
 authors = ["Yuval Saraf <unimonkiez@gmail.com>"]
 
 [tool.poetry.scripts]
 start = "memorix_client_redis.start:start"
 
 [tool.poetry.dependencies]
```

