# Comparing `tmp/async_dramatiq-0.1.1.tar.gz` & `tmp/async_dramatiq-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_dramatiq-0.1.1.tar", max compression
+gzip compressed data, was "async_dramatiq-0.1.2.tar", max compression
```

## Comparing `async_dramatiq-0.1.1.tar` & `async_dramatiq-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.1/LICENSE
--rw-r--r--   0        0        0       45 2023-05-25 20:37:01.348380 async_dramatiq-0.1.1/README.md
--rw-r--r--   0        0        0     3447 2023-05-26 09:13:24.665600 async_dramatiq-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      120 2023-05-26 07:37:33.566267 async_dramatiq-0.1.1/src/async_dramatiq/__init__.py
--rw-r--r--   0        0        0     3003 2023-05-26 09:10:55.772556 async_dramatiq-0.1.1/src/async_dramatiq/actors.py
--rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.1/src/async_dramatiq/backends/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-26 07:37:33.566695 async_dramatiq-0.1.1/src/async_dramatiq/backends/async_redis.py
--rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.1/src/async_dramatiq/backends/async_stub.py
--rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.1/src/async_dramatiq/middleware/__init__.py
--rw-r--r--   0        0        0      694 2023-05-26 07:37:33.567156 async_dramatiq-0.1.1/src/async_dramatiq/middleware/async_base.py
--rw-r--r--   0        0        0      728 2023-05-26 07:37:33.567263 async_dramatiq-0.1.1/src/async_dramatiq/middleware/async_stub.py
--rw-r--r--   0        0        0      961 2023-05-26 07:37:33.567386 async_dramatiq-0.1.1/src/async_dramatiq/scheduler.py
--rw-r--r--   0        0        0      342 2023-05-26 07:37:33.567506 async_dramatiq-0.1.1/src/async_dramatiq/types.py
--rw-r--r--   0        0        0     1112 2023-05-26 07:37:33.567624 async_dramatiq-0.1.1/src/async_dramatiq/worker.py
--rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     3812 2023-05-26 09:10:55.772756 async_dramatiq-0.1.1/tests/test_actors.py
--rw-r--r--   0        0        0     2563 2023-05-26 08:26:10.168282 async_dramatiq-0.1.1/tests/test_backends.py
--rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.1/tests/test_scheduler.py
--rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.1/tests/test_workers.py
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 async_dramatiq-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.2/LICENSE
+-rw-r--r--   0        0        0       45 2023-05-25 20:37:01.348380 async_dramatiq-0.1.2/README.md
+-rw-r--r--   0        0        0     3447 2023-05-26 09:35:05.996374 async_dramatiq-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      176 2023-05-26 09:32:22.203972 async_dramatiq-0.1.2/src/async_dramatiq/__init__.py
+-rw-r--r--   0        0        0     3003 2023-05-26 09:20:33.742002 async_dramatiq-0.1.2/src/async_dramatiq/actors.py
+-rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.2/src/async_dramatiq/backends/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-26 07:37:33.566695 async_dramatiq-0.1.2/src/async_dramatiq/backends/async_redis.py
+-rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.2/src/async_dramatiq/backends/async_stub.py
+-rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.2/src/async_dramatiq/middleware/__init__.py
+-rw-r--r--   0        0        0      694 2023-05-26 07:37:33.567156 async_dramatiq-0.1.2/src/async_dramatiq/middleware/async_base.py
+-rw-r--r--   0        0        0      728 2023-05-26 07:37:33.567263 async_dramatiq-0.1.2/src/async_dramatiq/middleware/async_stub.py
+-rw-r--r--   0        0        0      961 2023-05-26 07:37:33.567386 async_dramatiq-0.1.2/src/async_dramatiq/scheduler.py
+-rw-r--r--   0        0        0      342 2023-05-26 07:37:33.567506 async_dramatiq-0.1.2/src/async_dramatiq/types.py
+-rw-r--r--   0        0        0     1112 2023-05-26 07:37:33.567624 async_dramatiq-0.1.2/src/async_dramatiq/worker.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     3812 2023-05-26 09:10:55.772756 async_dramatiq-0.1.2/tests/test_actors.py
+-rw-r--r--   0        0        0     2563 2023-05-26 08:26:10.168282 async_dramatiq-0.1.2/tests/test_backends.py
+-rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.2/tests/test_scheduler.py
+-rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.2/tests/test_workers.py
+-rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 async_dramatiq-0.1.2/PKG-INFO
```

### Comparing `async_dramatiq-0.1.1/LICENSE` & `async_dramatiq-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/pyproject.toml` & `async_dramatiq-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "async_dramatiq"
-version = "0.1.1"
+version = "0.1.2"
 description = "Dramatiq with Asyncio support and some other goodies"
 authors = ["Ryan Houlihan <ryan@rhoulihan.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{ include = "async_dramatiq", from = "src" }]
 include = [{ path = "tests", format = "sdist" }]
 homepage = "https://github.com/motherofcoconuts/async-dramatiq"
```

### Comparing `async_dramatiq-0.1.1/src/async_dramatiq/actors.py` & `async_dramatiq-0.1.2/src/async_dramatiq/actors.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import asyncio
 import inspect
 from datetime import timedelta
 from typing import Any, Callable
 
 import dramatiq as dq
 
+
 from .scheduler import register_cron, register_interval
 from .types import DramatiqWorkerPriority
 
 
 class AsyncActor(dq.Actor):
     def __init__(self, *args: Any, **kwargs: dict[str, Any]) -> None:
         super().__init__(*args, **kwargs)
@@ -45,15 +46,14 @@
         else:
             result = self.fn(*args, **kwargs)
         return result
 
     def set_event_loop(self, loop: asyncio.BaseEventLoop | None) -> None:
         self.event_loop = loop
 
-
 def async_dramatiq_actor(
     *,
     interval: timedelta | None = None,
     crontab: str | None = None,
     priority: DramatiqWorkerPriority = DramatiqWorkerPriority.MEDIUM,
     actor_class: type[AsyncActor] = AsyncActor,
     queue_name: str = "default",
```

### Comparing `async_dramatiq-0.1.1/src/async_dramatiq/backends/async_redis.py` & `async_dramatiq-0.1.2/src/async_dramatiq/backends/async_redis.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/src/async_dramatiq/backends/async_stub.py` & `async_dramatiq-0.1.2/src/async_dramatiq/backends/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/src/async_dramatiq/middleware/async_base.py` & `async_dramatiq-0.1.2/src/async_dramatiq/middleware/async_base.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/src/async_dramatiq/middleware/async_stub.py` & `async_dramatiq-0.1.2/src/async_dramatiq/middleware/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/src/async_dramatiq/scheduler.py` & `async_dramatiq-0.1.2/src/async_dramatiq/scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/src/async_dramatiq/worker.py` & `async_dramatiq-0.1.2/src/async_dramatiq/worker.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/tests/conftest.py` & `async_dramatiq-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/tests/test_actors.py` & `async_dramatiq-0.1.2/tests/test_actors.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/tests/test_backends.py` & `async_dramatiq-0.1.2/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/tests/test_scheduler.py` & `async_dramatiq-0.1.2/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/tests/test_workers.py` & `async_dramatiq-0.1.2/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.1/PKG-INFO` & `async_dramatiq-0.1.2/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-dramatiq
-Version: 0.1.1
+Version: 0.1.2
 Summary: Dramatiq with Asyncio support and some other goodies
 Home-page: https://github.com/motherofcoconuts/async-dramatiq
 License: MIT
 Author: Ryan Houlihan
 Author-email: ryan@rhoulihan.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

