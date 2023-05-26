# Comparing `tmp/aiodiskqueue-0.1.0a5.tar.gz` & `tmp/aiodiskqueue-0.1.0a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiodiskqueue-0.1.0a5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "aiodiskqueue-0.1.0a6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `aiodiskqueue-0.1.0a5.tar` & `aiodiskqueue-0.1.0a6.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a5/.coveragerc
--rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a5/.github/workflows/main.yml
--rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a5/.gitignore
--rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a5/.readthedocs.yaml
--rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a5/LICENSE
--rw-r--r--   0        0        0     2012 2023-05-25 19:52:58.687290 aiodiskqueue-0.1.0a5/README.rst
--rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a5/docs/Makefile
--rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a5/docs/_static/custom.css
--rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a5/docs/api.rst
--rw-r--r--   0        0        0     1873 2023-05-25 13:02:52.209564 aiodiskqueue-0.1.0a5/docs/conf.py
--rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a5/docs/index.rst
--rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a5/docs/make.bat
--rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a5/examples/__init__.py
--rw-r--r--   0        0        0      210 2023-05-25 19:53:16.675360 aiodiskqueue-0.1.0a5/examples/basic_usage.py
--rw-r--r--   0        0        0      933 2023-05-25 19:47:09.774293 aiodiskqueue-0.1.0a5/examples/multiple_consumers.py
--rw-r--r--   0        0        0      879 2023-05-25 19:45:20.370257 aiodiskqueue-0.1.0a5/examples/single_consumer.py
--rw-r--r--   0        0        0      943 2023-05-24 22:01:37.989063 aiodiskqueue-0.1.0a5/pyproject.toml
--rw-r--r--   0        0        0      188 2023-05-25 14:35:48.129507 aiodiskqueue-0.1.0a5/src/aiodiskqueue/__init__.py
--rw-r--r--   0        0        0     4206 2023-05-25 20:16:18.165114 aiodiskqueue-0.1.0a5/src/aiodiskqueue/core.py
--rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a5/src/aiodiskqueue/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a5/tests/__init__.py
--rw-r--r--   0        0        0     2695 2023-05-25 20:12:15.141090 aiodiskqueue-0.1.0a5/tests/test_core.py
--rw-r--r--   0        0        0      394 2023-05-24 14:12:01.108384 aiodiskqueue-0.1.0a5/tox.ini
--rw-r--r--   0        0        0     2818 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a5/PKG-INFO
+-rw-r--r--   0        0        0      227 2023-05-24 13:44:43.729148 aiodiskqueue-0.1.0a6/.coveragerc
+-rw-r--r--   0        0        0      964 2023-05-24 14:34:49.657277 aiodiskqueue-0.1.0a6/.github/workflows/main.yml
+-rw-r--r--   0        0        0      107 2023-05-24 14:44:42.314154 aiodiskqueue-0.1.0a6/.gitignore
+-rw-r--r--   0        0        0      477 2023-05-17 22:01:56.296859 aiodiskqueue-0.1.0a6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      142 2023-05-24 16:15:47.425496 aiodiskqueue-0.1.0a6/.readthedocs.yaml
+-rw-r--r--   0        0        0     1080 2023-05-23 20:46:51.856056 aiodiskqueue-0.1.0a6/LICENSE
+-rw-r--r--   0        0        0     1967 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/README.rst
+-rw-r--r--   0        0        0      634 2023-05-24 14:44:01.590463 aiodiskqueue-0.1.0a6/docs/Makefile
+-rw-r--r--   0        0        0       37 2023-05-24 17:17:07.835418 aiodiskqueue-0.1.0a6/docs/_static/custom.css
+-rw-r--r--   0        0        0      228 2023-05-24 15:12:23.388951 aiodiskqueue-0.1.0a6/docs/api.rst
+-rw-r--r--   0        0        0     1837 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/docs/conf.py
+-rw-r--r--   0        0        0      347 2023-05-24 15:23:38.770047 aiodiskqueue-0.1.0a6/docs/index.rst
+-rw-r--r--   0        0        0      800 2023-05-24 14:44:01.594463 aiodiskqueue-0.1.0a6/docs/make.bat
+-rw-r--r--   0        0        0        0 2023-05-24 11:55:33.417325 aiodiskqueue-0.1.0a6/examples/__init__.py
+-rw-r--r--   0        0        0      197 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/examples/basic_usage.py
+-rw-r--r--   0        0        0      920 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/examples/multiple_consumers.py
+-rw-r--r--   0        0        0      866 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/examples/single_consumer.py
+-rw-r--r--   0        0        0      942 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/pyproject.toml
+-rw-r--r--   0        0        0      187 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/src/aiodiskqueue/__init__.py
+-rw-r--r--   0        0        0     3793 2023-05-26 21:04:16.766942 aiodiskqueue-0.1.0a6/src/aiodiskqueue/core.py
+-rw-r--r--   0        0        0      212 2023-05-24 13:48:27.949169 aiodiskqueue-0.1.0a6/src/aiodiskqueue/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-24 11:07:45.426708 aiodiskqueue-0.1.0a6/tests/__init__.py
+-rw-r--r--   0        0        0      514 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a6/tests/factories.py
+-rw-r--r--   0        0        0     3031 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a6/tests/loadtest.py
+-rw-r--r--   0        0        0     3033 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a6/tests/test_core.py
+-rw-r--r--   0        0        0      415 2023-05-26 21:04:16.770942 aiodiskqueue-0.1.0a6/tox.ini
+-rw-r--r--   0        0        0     2771 1970-01-01 00:00:00.000000 aiodiskqueue-0.1.0a6/PKG-INFO
```

### Comparing `aiodiskqueue-0.1.0a5/.github/workflows/main.yml` & `aiodiskqueue-0.1.0a6/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a5/LICENSE` & `aiodiskqueue-0.1.0a6/LICENSE`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a5/README.rst` & `aiodiskqueue-0.1.0a6/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,51 +1,50 @@
 aiodiskqueue
 ============
 
-Persistent queues for Python AsyncIO.
+Persistent queue for Python AsyncIO.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
 This library provides a persistent queue for Python AsyncIO.
 
-It's main advantage is that it's content will survive a normal process restart and potentially even a process crash.
-
-Each queue is stored in it's own SQLite database on disk to provide maximum isolation between queues.
+It has an API similar to the standard `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_,
+but items in the queue will persists between process restarts.
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
 
-   import asyncio
-   from aiodiskqueue import Queue
+    import asyncio
+    from aiodiskqueue import Queue
 
-   async def main():
-       q = await Queue.create("example_queue.sqlite")
-       await q.put("some item")
-       item = await q.get()
-       print(item)
+    async def main():
+        q = Queue("example_queue.sqlite")
+        await q.put("some item")
+        item = await q.get()
+        print(item)
 
-   asyncio.run(main())
+    asyncio.run(main())
 
 Please see the examples folder for more usage examples.
 
 Installation
 ------------
 
 You can install directly from PyPI with the following command:
 
 .. code:: shell
 
-   pip install aiodiskqueue
+    pip install aiodiskqueue
 
 
 
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
```

### Comparing `aiodiskqueue-0.1.0a5/docs/Makefile` & `aiodiskqueue-0.1.0a6/docs/Makefile`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a5/docs/conf.py` & `aiodiskqueue-0.1.0a6/docs/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,25 +19,24 @@
 exclude_patterns = ["_build", "Thumbs.db", ".DS_Store"]
 
 # -- Options for autodoc -----------------------------------------------------
 # autoclass_content = "both"
 autodoc_default_options = {
     "members": True,
     "member-order": "alphabetical",
-    "special-members": "__init__",
     "undoc-members": False,
     "exclude-members": "__weakref__",
 }
 
 # -- Options for HTML output -------------------------------------------------
 # https://www.sphinx-doc.org/en/master/usage/configuration.html#options-for-html-output
 
 html_theme = "alabaster"
 html_theme_options = {
-    "description": "Persistent queues for Python AsyncIO",
+    "description": "Persistent queue for Python AsyncIO",
     "fixed_sidebar": True,
     "badge_branch": "master",
     "github_button": True,
     "github_user": "ErikKalkoken",
     "github_repo": "aiodiskqueue",
     "show_powered_by": False,
     "sidebar_collapse": False,
```

### Comparing `aiodiskqueue-0.1.0a5/docs/make.bat` & `aiodiskqueue-0.1.0a6/docs/make.bat`

 * *Files identical despite different names*

### Comparing `aiodiskqueue-0.1.0a5/examples/multiple_consumers.py` & `aiodiskqueue-0.1.0a6/examples/multiple_consumers.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     while True:
         message = await queue.get()
         print(message)
 
 
 async def main():
     path = Path.cwd() / "example_queue.sqlite"
-    queue = await Queue.create(path)
+    queue = Queue(path)
     coroutines = [
         consumer(queue),
         consumer(queue),
         producer(queue, 1),
         producer(queue, 2),
         producer(queue, 3),
         producer(queue, 4),
```

### Comparing `aiodiskqueue-0.1.0a5/examples/single_consumer.py` & `aiodiskqueue-0.1.0a6/examples/single_consumer.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     while True:
         message = await queue.get()
         print(message)
 
 
 async def main():
     path = Path.cwd() / "example_queue.sqlite"
-    queue = await Queue.create(path)
+    queue = Queue(path)
     coroutines = [
         consumer(queue),
         producer(queue, 1),
         producer(queue, 2),
         producer(queue, 3),
     ]
     await asyncio.gather(*coroutines)
```

### Comparing `aiodiskqueue-0.1.0a5/pyproject.toml` & `aiodiskqueue-0.1.0a6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dynamic = ["version", "description"]
 requires-python = ">=3.8"
 dependencies = [
-    "aiosqlite>=0.19.0"
+    "aiofiles>=23.1.0"
 ]
 
 [project.urls]
 Documentation = "https://aiodiskqueue.readthedocs.io/en/latest/"
 Source = "https://github.com/ErikKalkoken/aiodiskqueue"
 Tracker = "https://github.com/ErikKalkoken/aiodiskqueue/issues"
```

### Comparing `aiodiskqueue-0.1.0a5/tests/test_core.py` & `aiodiskqueue-0.1.0a6/tests/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,92 +1,108 @@
 import asyncio
-import datetime as dt
 import shutil
 import tempfile
 from pathlib import Path
 from unittest import IsolatedAsyncioTestCase
 
+import aiofiles
+
 from aiodiskqueue import Queue, QueueEmpty
 
+from .factories import ItemFactory
+
 
 class TestQueue(IsolatedAsyncioTestCase):
     def setUp(self) -> None:
         self.temp_dir = Path(tempfile.mkdtemp())
-        self.db_path = self.temp_dir / "test_queue.sqlite"
+        self.db_path = self.temp_dir / "queue.dat"
 
     def tearDown(self) -> None:
         shutil.rmtree(self.temp_dir, ignore_errors=True)
 
     async def test_should_create_queue_and_measure_size(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         # when
         result = await q.qsize()
         # then
         self.assertEqual(result, 0)
 
     async def test_should_put_items_and_measure_size(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         # when
-        await q.put("dummy")
+        await q.put(ItemFactory())
+        await q.put(ItemFactory())
         # then
         result = await q.qsize()
-        self.assertEqual(result, 1)
+        self.assertEqual(result, 2)
 
-    async def test_should_get_items(self):
+    async def test_should_get_item(self):
         # given
-        q = await Queue.create(self.db_path)
-        await q.put("dummy")
-        # when
-        result = await q.get_nowait()
-        # then
-        self.assertEqual(result, "dummy")
-
-    async def test_should_handle_complex_items(self):
-        # given
-        q = await Queue.create(self.db_path)
-        item = {
-            "alpha": ["one", "two", "three"],
-            "now": dt.datetime.now(tz=dt.timezone.utc),
-        }
+        q = Queue(self.db_path)
+        item = ItemFactory()
         await q.put(item)
+        await q.put(ItemFactory())
         # when
         result = await q.get_nowait()
         # then
         self.assertEqual(result, item)
 
     async def test_should_raise_exception_when_get_on_empty_queue(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         # when/then
         with self.assertRaises(QueueEmpty):
             await q.get_nowait()
 
     async def test_should_report_as_empty(self):
         # given
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         # when/then
         self.assertTrue(await q.empty())
 
     async def test_should_not_report_as_empty(self):
         # given
-        q = await Queue.create(self.db_path)
-        await q.put("dummy")
+        q = Queue(self.db_path)
+        await q.put(ItemFactory())
         # when/then
         self.assertFalse(await q.empty())
 
     async def test_get_should_wait_until_item_is_available(self):
         async def consumer():
             item = await q.get()
             await queue_2.put(item)
 
         # given
         queue_2 = asyncio.Queue()
-        q = await Queue.create(self.db_path)
+        q = Queue(self.db_path)
         asyncio.create_task(consumer())
         # when
         await asyncio.sleep(1)  # consumer sees an empty queue when task starts
-        await q.put("special-item")
+        item = ItemFactory()
+        await q.put(item)
+        # then
+        item_new = await queue_2.get()
+        self.assertEqual(item_new, item)
+
+    async def test_should_create_new_file_when_current_file_is_corrupt(self):
+        # given
+        async with aiofiles.open(self.db_path, "wb") as fp:
+            await fp.write(b"invalid-data")
+        q = Queue(self.db_path)
+        # when
+        result = await q.qsize()
+        # then
+        self.assertEqual(result, 0)
+
+    async def test_should_preserve_queue_content(self):
+        # given
+        queue_1 = Queue(self.db_path)
+        item = ItemFactory()
+        await queue_1.put(item)
+        # when
+        del queue_1
+        queue_2 = Queue(self.db_path)
+        item_new = await queue_2.get()
         # then
-        item = await queue_2.get_nowait()
-        self.assertEqual(item, "special-item")
+        self.assertEqual(item_new, item)
```

### Comparing `aiodiskqueue-0.1.0a5/PKG-INFO` & `aiodiskqueue-0.1.0a6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,70 +1,69 @@
 Metadata-Version: 2.1
 Name: aiodiskqueue
-Version: 0.1.0a5
-Summary: Persistent queues for Python AsyncIO.
+Version: 0.1.0a6
+Summary: Persistent queue for Python AsyncIO.
 Author-email: Erik Kalkoken <kalkoken87@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiosqlite>=0.19.0
+Requires-Dist: aiofiles>=23.1.0
 Project-URL: Documentation, https://aiodiskqueue.readthedocs.io/en/latest/
 Project-URL: Source, https://github.com/ErikKalkoken/aiodiskqueue
 Project-URL: Tracker, https://github.com/ErikKalkoken/aiodiskqueue/issues
 
 aiodiskqueue
 ============
 
-Persistent queues for Python AsyncIO.
+Persistent queue for Python AsyncIO.
 
 |release| |python| |tests| |codecov| |docs| |pre-commit| |Code style: black|
 
 Description
 -----------
 
 This library provides a persistent queue for Python AsyncIO.
 
-It's main advantage is that it's content will survive a normal process restart and potentially even a process crash.
-
-Each queue is stored in it's own SQLite database on disk to provide maximum isolation between queues.
+It has an API similar to the standard `asyncio.Queue <https://docs.python.org/3/library/asyncio-queue.html#queue>`_,
+but items in the queue will persists between process restarts.
 
 Usage
 -----
 
 Here is a basic example on how to use the queue:
 
 .. code:: python
 
-   import asyncio
-   from aiodiskqueue import Queue
+    import asyncio
+    from aiodiskqueue import Queue
 
-   async def main():
-       q = await Queue.create("example_queue.sqlite")
-       await q.put("some item")
-       item = await q.get()
-       print(item)
+    async def main():
+        q = Queue("example_queue.sqlite")
+        await q.put("some item")
+        item = await q.get()
+        print(item)
 
-   asyncio.run(main())
+    asyncio.run(main())
 
 Please see the examples folder for more usage examples.
 
 Installation
 ------------
 
 You can install directly from PyPI with the following command:
 
 .. code:: shell
 
-   pip install aiodiskqueue
+    pip install aiodiskqueue
 
 
 
 .. |release| image:: https://img.shields.io/pypi/v/aiodiskqueue?label=release
    :target: https://pypi.org/project/aiodiskqueue/
 .. |python| image:: https://img.shields.io/pypi/pyversions/aiodiskqueue
    :target: https://pypi.org/project/aiodiskqueue/
```

