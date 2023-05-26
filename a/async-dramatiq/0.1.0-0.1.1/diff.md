# Comparing `tmp/async_dramatiq-0.1.0.tar.gz` & `tmp/async_dramatiq-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "async_dramatiq-0.1.0.tar", max compression
+gzip compressed data, was "async_dramatiq-0.1.1.tar", max compression
```

## Comparing `async_dramatiq-0.1.0.tar` & `async_dramatiq-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1065 2023-05-26 07:14:48.487934 async_dramatiq-0.1.0/LICENSE
--rw-r--r--   0        0        0       45 2023-05-25 20:37:01.348380 async_dramatiq-0.1.0/README.md
--rw-r--r--   0        0        0      120 2023-05-26 07:37:33.566267 async_dramatiq-0.1.0/async_dramatiq/__init__.py
--rw-r--r--   0        0        0     3429 2023-05-26 07:37:33.566415 async_dramatiq-0.1.0/async_dramatiq/actors.py
--rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.0/async_dramatiq/backends/__init__.py
--rw-r--r--   0        0        0     1577 2023-05-26 07:37:33.566695 async_dramatiq-0.1.0/async_dramatiq/backends/async_redis.py
--rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.0/async_dramatiq/backends/async_stub.py
--rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.0/async_dramatiq/middleware/__init__.py
--rw-r--r--   0        0        0      694 2023-05-26 07:37:33.567156 async_dramatiq-0.1.0/async_dramatiq/middleware/async_base.py
--rw-r--r--   0        0        0      728 2023-05-26 07:37:33.567263 async_dramatiq-0.1.0/async_dramatiq/middleware/async_stub.py
--rw-r--r--   0        0        0      961 2023-05-26 07:37:33.567386 async_dramatiq-0.1.0/async_dramatiq/scheduler.py
--rw-r--r--   0        0        0      342 2023-05-26 07:37:33.567506 async_dramatiq-0.1.0/async_dramatiq/types.py
--rw-r--r--   0        0        0     1112 2023-05-26 07:37:33.567624 async_dramatiq-0.1.0/async_dramatiq/worker.py
--rw-r--r--   0        0        0     3434 2023-05-26 07:44:24.419344 async_dramatiq-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 20:54:24.000439 async_dramatiq-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     1471 2023-05-26 07:12:33.420508 async_dramatiq-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0     3656 2023-05-26 07:24:11.756453 async_dramatiq-0.1.0/tests/test_actors.py
--rw-r--r--   0        0        0     2563 2023-05-26 07:12:33.420850 async_dramatiq-0.1.0/tests/test_backends.py
--rw-r--r--   0        0        0     1024 2023-05-26 07:12:33.421035 async_dramatiq-0.1.0/tests/test_scheduler.py
--rw-r--r--   0        0        0      595 2023-05-26 07:12:33.421190 async_dramatiq-0.1.0/tests/test_workers.py
--rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 async_dramatiq-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-26 08:26:10.164949 async_dramatiq-0.1.1/LICENSE
+-rw-r--r--   0        0        0       45 2023-05-25 20:37:01.348380 async_dramatiq-0.1.1/README.md
+-rw-r--r--   0        0        0     3447 2023-05-26 09:13:24.665600 async_dramatiq-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      120 2023-05-26 07:37:33.566267 async_dramatiq-0.1.1/src/async_dramatiq/__init__.py
+-rw-r--r--   0        0        0     3003 2023-05-26 09:10:55.772556 async_dramatiq-0.1.1/src/async_dramatiq/actors.py
+-rw-r--r--   0        0        0      491 2023-05-26 07:37:33.566566 async_dramatiq-0.1.1/src/async_dramatiq/backends/__init__.py
+-rw-r--r--   0        0        0     1577 2023-05-26 07:37:33.566695 async_dramatiq-0.1.1/src/async_dramatiq/backends/async_redis.py
+-rw-r--r--   0        0        0     1758 2023-05-26 07:37:33.566814 async_dramatiq-0.1.1/src/async_dramatiq/backends/async_stub.py
+-rw-r--r--   0        0        0      112 2023-05-26 07:37:33.566965 async_dramatiq-0.1.1/src/async_dramatiq/middleware/__init__.py
+-rw-r--r--   0        0        0      694 2023-05-26 07:37:33.567156 async_dramatiq-0.1.1/src/async_dramatiq/middleware/async_base.py
+-rw-r--r--   0        0        0      728 2023-05-26 07:37:33.567263 async_dramatiq-0.1.1/src/async_dramatiq/middleware/async_stub.py
+-rw-r--r--   0        0        0      961 2023-05-26 07:37:33.567386 async_dramatiq-0.1.1/src/async_dramatiq/scheduler.py
+-rw-r--r--   0        0        0      342 2023-05-26 07:37:33.567506 async_dramatiq-0.1.1/src/async_dramatiq/types.py
+-rw-r--r--   0        0        0     1112 2023-05-26 07:37:33.567624 async_dramatiq-0.1.1/src/async_dramatiq/worker.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:26:10.167650 async_dramatiq-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     1471 2023-05-26 08:26:10.167926 async_dramatiq-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     3812 2023-05-26 09:10:55.772756 async_dramatiq-0.1.1/tests/test_actors.py
+-rw-r--r--   0        0        0     2563 2023-05-26 08:26:10.168282 async_dramatiq-0.1.1/tests/test_backends.py
+-rw-r--r--   0        0        0     1024 2023-05-26 08:26:10.168435 async_dramatiq-0.1.1/tests/test_scheduler.py
+-rw-r--r--   0        0        0      595 2023-05-26 08:26:10.168609 async_dramatiq-0.1.1/tests/test_workers.py
+-rw-r--r--   0        0        0      777 1970-01-01 00:00:00.000000 async_dramatiq-0.1.1/PKG-INFO
```

### Comparing `async_dramatiq-0.1.0/LICENSE` & `async_dramatiq-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/async_dramatiq/actors.py` & `async_dramatiq-0.1.1/src/async_dramatiq/actors.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,14 @@
 import asyncio
 import inspect
 from datetime import timedelta
 from typing import Any, Callable
 
 import dramatiq as dq
 
-# from baton_tms.helpers.monitoring import monitor
-# from sentry_sdk import start_transaction
-
 from .scheduler import register_cron, register_interval
 from .types import DramatiqWorkerPriority
 
 
 class AsyncActor(dq.Actor):
     def __init__(self, *args: Any, **kwargs: dict[str, Any]) -> None:
         super().__init__(*args, **kwargs)
@@ -29,15 +26,14 @@
         :return: Whatever the underlying function backing this actor returns.
         """
         try:
             running_event_loop = asyncio.get_running_loop()
         except RuntimeError:
             running_event_loop = None
 
-        # with start_transaction(op="actor", name=self.actor_name):
         if inspect.iscoroutinefunction(self.fn):
             if running_event_loop:  # Call function directly
                 result = self.fn(*args, **kwargs)
             elif (  # Call function through worker thread
                 self.event_loop and self.event_loop.is_running()
             ):
                 future = asyncio.run_coroutine_threadsafe(
@@ -50,46 +46,40 @@
             result = self.fn(*args, **kwargs)
         return result
 
     def set_event_loop(self, loop: asyncio.BaseEventLoop | None) -> None:
         self.event_loop = loop
 
 
-def dramatiq_actor(
+def async_dramatiq_actor(
     *,
     interval: timedelta | None = None,
     crontab: str | None = None,
-    monitor_id: str | None = None,
     priority: DramatiqWorkerPriority = DramatiqWorkerPriority.MEDIUM,
+    actor_class: type[AsyncActor] = AsyncActor,
+    queue_name: str = "default",
     **kwargs: Any,
 ) -> Any:
     """Thin wrapper which turns a function into a dramatiq actor.
 
     :param interval: Run this function at a defined interval
     :param crontab: Run this function as a cron job
-    :param monitor_id: The Sentry `monitor_id` for this job
     :param priority: The actor's global priority.  If two tasks have
         been pulled on a worker concurrently and one has a higher
         priority than the other then it will be processed first.
         Lower numbers represent higher priorities.
+    :param actor_class: The actor class to use
+    :param queue_name: The name of the queue to send messages to
     :param kwargs: Input parameters for the dramatiq actor
 
     Dramatiq Actor: https://dramatiq.io/_modules/dramatiq/actor.html
     """
+
     def decorator(func: Callable[..., Any]) -> dq.Actor:
-        if interval or crontab:
-            queue_name = kwargs.get("queue_name") or "default"
-            throws: tuple[Exception, ...] = kwargs.get("throws", ())
-            # func = monitor(
-            #     func,
-            #     name=f"{func.__name__} from {queue_name}",
-            #     monitor_id=monitor_id,
-            #     throws=throws,
-            # )
-        actor = dq.actor(func, actor_class=AsyncActor, priority=priority, **kwargs)
+        actor = dq.actor(func, actor_class=actor_class, priority=priority, **kwargs)
         if crontab:
             register_cron(actor.fn, crontab)
         if interval:
             register_interval(actor.fn, interval)
 
         return actor
```

### Comparing `async_dramatiq-0.1.0/async_dramatiq/backends/async_redis.py` & `async_dramatiq-0.1.1/src/async_dramatiq/backends/async_redis.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/async_dramatiq/backends/async_stub.py` & `async_dramatiq-0.1.1/src/async_dramatiq/backends/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/async_dramatiq/middleware/async_base.py` & `async_dramatiq-0.1.1/src/async_dramatiq/middleware/async_base.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/async_dramatiq/middleware/async_stub.py` & `async_dramatiq-0.1.1/src/async_dramatiq/middleware/async_stub.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/async_dramatiq/scheduler.py` & `async_dramatiq-0.1.1/src/async_dramatiq/scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/async_dramatiq/worker.py` & `async_dramatiq-0.1.1/src/async_dramatiq/worker.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/pyproject.toml` & `async_dramatiq-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [tool.poetry]
-name = "async-dramatiq"
-version = "0.1.0"
+name = "async_dramatiq"
+version = "0.1.1"
 description = "Dramatiq with Asyncio support and some other goodies"
 authors = ["Ryan Houlihan <ryan@rhoulihan.com>"]
 license = "MIT License"
 readme = "README.md"
-packages = [{ include = "async_dramatiq" }]
+packages = [{ include = "async_dramatiq", from = "src" }]
 include = [{ path = "tests", format = "sdist" }]
 homepage = "https://github.com/motherofcoconuts/async-dramatiq"
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/motherofcoconuts/async-dramatiq/issues"
 
 [tool.poetry.dependencies]
@@ -23,28 +23,28 @@
 black = "^23.3.0"
 coverage = "^7.2.5"
 pytest-asyncio = "*"
 pytest = "*"
 pytest-cov = "*"
 
 [build-system]
-requires = ["setuptools", "poetry-core"]
+requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 junit_family = "xunit2"
 asyncio_mode = "auto"
 addopts = "--cov --cov-report term --cov-report xml"
 testpaths = [
   "tests"
 ]
 filterwarnings = ["ignore::DeprecationWarning", "ignore::UserWarning:stytch.*"]
 
 [tool.coverage.run]
-source = ["src/async_dramatiq"]
+source = ["async_dramatiq"]
 omit = ["*migratons*", "*tests*", "*scripts*"]
 
 [tool.coverage.report]
 exclude_lines = [
     "pragma: no cover",
     "def __repr__",
     "def __str__",
@@ -101,15 +101,15 @@
 '''
 
 [tool.vulture]
 exclude = ["scripts/"]
 ignore_decorators = ["@app.route", "@require_*"]
 make_whitelist = true
 min_confidence = 80
-paths = ["src/async_dramatiq"]
+paths = ["async_dramatiq"]
 sort_by_size = true
 verbose = false
 
 [tool.mypy]
 python_version = "3.11"
 ignore_missing_imports = true
 scripts_are_modules = true
```

### Comparing `async_dramatiq-0.1.0/tests/conftest.py` & `async_dramatiq-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/tests/test_actors.py` & `async_dramatiq-0.1.1/tests/test_actors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 # Standard Library Imports
 import asyncio
 from datetime import timedelta
+from typing import Any, Callable, TypeVar
 
 import pytest
 from apscheduler.triggers.cron import CronTrigger
 from apscheduler.triggers.interval import IntervalTrigger
 from dramatiq import Worker
 
 # Local Application Imports
-from async_dramatiq.actors import dramatiq_actor
+from async_dramatiq.actors import async_dramatiq_actor
 from async_dramatiq.backends import AsyncStubBackend, get_backend
 from async_dramatiq.scheduler import scheduled_jobs
 
+F = TypeVar("F", bound=Callable[..., Any])
 
-def test_dramatiq_actor() -> None:
+def test_async_dramatiq_actor() -> None:
     scheduled_jobs_len = len(scheduled_jobs)
 
-    @dramatiq_actor(interval=timedelta(seconds=5))
+    @async_dramatiq_actor(interval=timedelta(seconds=5))
     def test_interval():
         return None
 
-    @dramatiq_actor(crontab="* * * * *")
+    @async_dramatiq_actor(crontab="* * * * *")
     def test_cron():
         return None
 
-    @dramatiq_actor()
+    @async_dramatiq_actor()
     async def test_async():
         return None
 
     assert len(scheduled_jobs) == scheduled_jobs_len + 2
     assert isinstance(scheduled_jobs[-1].trigger, CronTrigger)
     assert scheduled_jobs[-1].module_path, test_cron.__module__
     assert scheduled_jobs[-1].func_name, test_cron.__name__
@@ -37,40 +39,39 @@
     assert scheduled_jobs[-2].module_path, test_interval.__module__
     assert scheduled_jobs[-2].func_name, test_interval.__name__
 
 
 async def test_async_actor_func(event_loop: asyncio.BaseEventLoop) -> None:
     result = "generic result"
 
-    @dramatiq_actor()
+    @async_dramatiq_actor()
     async def test_async():
         return result
 
     # Test generic run
     assert result == await test_async()
 
-
 def test_async_actor_func_no_loop() -> None:
     result = "generic result"
 
-    @dramatiq_actor()
+    @async_dramatiq_actor()
     async def test_async():
         return result
 
     # Test generic run
     with pytest.raises(RuntimeError):
         test_async()
 
 
 async def test_async_actor_func_in_thread(
     worker: Worker, async_stub_backend: AsyncStubBackend
 ) -> None:
     result = "generic result"
 
-    @dramatiq_actor(store_results=True)
+    @async_dramatiq_actor(store_results=True)
     async def test_async():
         return result
 
     # Setup actor event loop
     loop = (w.event_loop for w in worker.workers if hasattr(w, "event_loop"))
     test_async.event_loop = next(loop, None)
 
@@ -81,37 +82,37 @@
     return_result = await get_backend().get_result(msg, block=True)
     assert return_result == result
 
 
 async def test_sync_actor_func() -> None:
     result = "generic result"
 
-    @dramatiq_actor()
+    @async_dramatiq_actor()
     def test_sync():
         return result
 
     assert result == test_sync()
 
 
 def test_sync_actor_func_no_loop() -> None:
     result = "generic result"
 
-    @dramatiq_actor()
+    @async_dramatiq_actor()
     def test_sync():
         return result
 
     assert result == test_sync()
 
 
 async def test_sync_actor_func_in_thread(
     worker: Worker, async_stub_backend: AsyncStubBackend
 ) -> None:
     result = "generic result"
 
-    @dramatiq_actor(store_results=True)
+    @async_dramatiq_actor(store_results=True)
     def test_async():
         return result
 
     # Send actor to worker
     msg = test_async.send()
     worker.join()
 
@@ -119,15 +120,15 @@
 
     assert return_result == result
 
 
 async def test_async_request(
     worker: Worker, async_stub_backend: AsyncStubBackend
 ) -> None:
-    @dramatiq_actor(store_results=True)
+    @async_dramatiq_actor(store_results=True)
     async def test_async():
         await asyncio.sleep(0.25)
         return True
 
     # Setup actor event loop
     loop = (w.event_loop for w in worker.workers if hasattr(w, "event_loop"))
     test_async.event_loop = next(loop, None)
```

### Comparing `async_dramatiq-0.1.0/tests/test_backends.py` & `async_dramatiq-0.1.1/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/tests/test_scheduler.py` & `async_dramatiq-0.1.1/tests/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/tests/test_workers.py` & `async_dramatiq-0.1.1/tests/test_workers.py`

 * *Files identical despite different names*

### Comparing `async_dramatiq-0.1.0/PKG-INFO` & `async_dramatiq-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: async-dramatiq
-Version: 0.1.0
+Version: 0.1.1
 Summary: Dramatiq with Asyncio support and some other goodies
 Home-page: https://github.com/motherofcoconuts/async-dramatiq
 License: MIT
 Author: Ryan Houlihan
 Author-email: ryan@rhoulihan.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
```

