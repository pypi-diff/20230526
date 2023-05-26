# Comparing `tmp/Light-Pipe-0.2.2.tar.gz` & `tmp/light-pipe-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/richardcorrero/Projects/light-pipe/dist/.tmp-15m60exz/Light-Pipe-0.2.2.tar", last modified: Mon Feb  6 19:31:30 2023, max compression
+gzip compressed data, was "light-pipe-0.3.0.tar", last modified: Fri May 26 21:15:57 2023, max compression
```

## Comparing `Light-Pipe-0.2.2.tar` & `light-pipe-0.3.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
-drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1465 2022-12-24 21:34:11.000000 Light-Pipe-0.2.2/LICENSE
-drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/Light_Pipe.egg-info/
--rw-r--r--   0 richardcorrero   (501) staff       (20)      660 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/Light_Pipe.egg-info/PKG-INFO
--rw-r--r--   0 richardcorrero   (501) staff       (20)      257 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/Light_Pipe.egg-info/SOURCES.txt
--rw-r--r--   0 richardcorrero   (501) staff       (20)        1 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/Light_Pipe.egg-info/dependency_links.txt
--rw-r--r--   0 richardcorrero   (501) staff       (20)       11 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/Light_Pipe.egg-info/top_level.txt
--rw-r--r--   0 richardcorrero   (501) staff       (20)      660 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/PKG-INFO
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1014 2023-01-03 00:59:54.000000 Light-Pipe-0.2.2/README.md
-drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/light_pipe/
--rw-r--r--   0 richardcorrero   (501) staff       (20)     1171 2023-02-06 18:59:25.000000 Light-Pipe-0.2.2/light_pipe/__init__.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)     3470 2023-02-06 18:59:25.000000 Light-Pipe-0.2.2/light_pipe/data.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)     9895 2023-02-06 18:59:25.000000 Light-Pipe-0.2.2/light_pipe/parallelizer.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)     3844 2023-02-06 18:59:25.000000 Light-Pipe-0.2.2/light_pipe/transformer.py
--rw-r--r--   0 richardcorrero   (501) staff       (20)       38 2023-02-06 19:31:30.000000 Light-Pipe-0.2.2/setup.cfg
--rw-r--r--   0 richardcorrero   (501) staff       (20)      740 2023-02-06 19:10:39.000000 Light-Pipe-0.2.2/setup.py
+drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-26 21:15:57.307282 light-pipe-0.3.0/
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1465 2022-12-24 21:34:11.000000 light-pipe-0.3.0/LICENSE
+drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-26 21:15:57.294447 light-pipe-0.3.0/Light_Pipe.egg-info/
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1100 2023-05-26 21:15:57.000000 light-pipe-0.3.0/Light_Pipe.egg-info/PKG-INFO
+-rw-r--r--   0 richardcorrero   (501) staff       (20)      446 2023-05-26 21:15:57.000000 light-pipe-0.3.0/Light_Pipe.egg-info/SOURCES.txt
+-rw-r--r--   0 richardcorrero   (501) staff       (20)        1 2023-05-26 21:15:57.000000 light-pipe-0.3.0/Light_Pipe.egg-info/dependency_links.txt
+-rw-r--r--   0 richardcorrero   (501) staff       (20)       11 2023-05-26 21:15:57.000000 light-pipe-0.3.0/Light_Pipe.egg-info/top_level.txt
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1100 2023-05-26 21:15:57.306588 light-pipe-0.3.0/PKG-INFO
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1915 2023-05-26 21:13:35.000000 light-pipe-0.3.0/README.md
+drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-26 21:15:57.302267 light-pipe-0.3.0/light_pipe/
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1171 2023-02-06 18:59:25.000000 light-pipe-0.3.0/light_pipe/__init__.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     3680 2023-05-26 19:43:35.000000 light-pipe-0.3.0/light_pipe/data.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)    11386 2023-05-26 20:48:32.000000 light-pipe-0.3.0/light_pipe/parallelizer.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     4083 2023-05-26 20:51:46.000000 light-pipe-0.3.0/light_pipe/transformer.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)       38 2023-05-26 21:15:57.307397 light-pipe-0.3.0/setup.cfg
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1180 2023-05-26 21:15:10.000000 light-pipe-0.3.0/setup.py
+drwxr-xr-x   0 richardcorrero   (501) staff       (20)        0 2023-05-26 21:15:57.304593 light-pipe-0.3.0/tests/
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     2103 2023-05-26 19:58:45.000000 light-pipe-0.3.0/tests/test_parallelizer.py
+-rw-r--r--   0 richardcorrero   (501) staff       (20)     1313 2023-05-26 19:58:49.000000 light-pipe-0.3.0/tests/test_transformer.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Light-Pipe-0.2.2/LICENSE` & `light-pipe-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Light-Pipe-0.2.2/README.md` & `light-pipe-0.3.0/light_pipe/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,15 @@
+__author__ = "Richard Correro (richard@richardcorrero.com)"
+
+
+from .data import *
+from .parallelizer import *
+from .transformer import *
+
+__doc__ = """
 # [Light-Pipe](https://github.com/rcorrero/light-pipe)
 
 ---
 
 ## Overview
 
 [Light-Pipe](https://www.light-pipe.io/) is an extensible, light-weight Python framework for data pipelines that scale. It provides a set of intuitive abstractions designed to decouple pipeline implementation from the operations they perform. It is designed to scale effortlessly, being built from the ground-up to support concurrency in all its forms, and it has zero non-standard dependencies. It's also super fast and efficient, used to perform critical geospatial data processing tasks [at least an order of magnitude faster than existing systems](https://github.com/rcorrero/light-pipe/blob/depth_first/data/plots/test_geo_tiling.png).
@@ -12,8 +20,9 @@
 
 - [GitHub](https://github.com/rcorrero/light-pipe)
 
 - [Documentation](https://www.light-pipe.io/)
 
 ---
 
-Copyright 2020-2023 [Richard Correro](https://www.richardcorrero.com/).
+Copyright 2020-2023 [Richard Correro](https://www.richardcorrero.com/).
+"""
```

### Comparing `Light-Pipe-0.2.2/light_pipe/data.py` & `light-pipe-0.3.0/light_pipe/data.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,8 +106,15 @@
             store_results = self.store_results
         _results_stored = self._results_stored
         args = (*args, *self.args)
         kwargs = {**kwargs, **self.kwargs}
         return self._copy(
            *args, generator=generator, store_results=store_results, 
            _results_stored=_results_stored, **kwargs
-        )        
+        )
+
+def make_data(
+    generator: Optional[Union[Callable, Iterable]] = None
+) -> Callable:
+    def data_wrapper(*args, **kwargs) -> Data:
+        return Data(generator=generator, *args, **kwargs)
+    return data_wrapper
```

### Comparing `Light-Pipe-0.2.2/light_pipe/parallelizer.py` & `light-pipe-0.3.0/light_pipe/parallelizer.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 __author__ = "Richard Correro (richard@richardcorrero.com)"
 
 
 import asyncio
 import concurrent.futures
 import functools
-import time
-import unittest
-from typing import (Any, AsyncGenerator, Callable, Coroutine, Generator,
+from concurrent.futures import Future
+from typing import (Any, AsyncGenerator, Callable, Coroutine, Dict, Generator,
                     Iterable, List, Optional, Tuple, Union)
 
 
 class Parallelizer:
     def __call__(
-        self, iterable: Iterable    
+        self, iterable: Iterable, tuple_to_args: Optional[bool] = True,
+        dict_to_kwargs: Optional[bool] = True
     ):
         for f, item, args, kwargs in iterable:
-            yield f(item, *args, **kwargs)
+            if tuple_to_args and isinstance(item, Tuple):
+                yield f(*item, *args, **kwargs)
+            elif dict_to_kwargs and isinstance(item, Dict):
+                yield f(*args, **item, **kwargs)
+            else:
+                yield f(item, *args, **kwargs)
 
 
 class Pooler(Parallelizer):
     def __init__(
         self, max_workers: Optional[int] = None,
         DefaultExecutor: Optional[type] = None,
         executor: Optional[Union[
@@ -36,36 +41,65 @@
 
 
     def __call__(
         self, iterable: Iterable, max_workers: Optional[int] = None,
         executor: Optional[Union[
             concurrent.futures.ThreadPoolExecutor, 
             concurrent.futures.ProcessPoolExecutor
-        ]] = None
+        ]] = None, 
+        tuple_to_args: Optional[bool] = True,
+        dict_to_kwargs: Optional[bool] = True
     ) -> Generator:
         if executor is None:
             executor = self.executor
         if max_workers is None:
             max_workers = self.max_workers
 
         if executor is not None:
-            futures = [
-                executor.submit(f, item, *args, **kwargs) for 
-                f, item, args, kwargs in iterable
-            ]
-            for future in concurrent.futures.as_completed(futures):
-                yield future.result()
+            # futures = [
+            #     executor.submit(f, item, *args, **kwargs) for 
+            #     f, item, args, kwargs in iterable
+            # ]
+            yield from self._submit_tasks(
+                iterable=iterable, executor=executor, tuple_to_args=tuple_to_args, 
+                dict_to_kwargs=dict_to_kwargs
+            )
         else:
             with self.DefaultExecutor(max_workers=max_workers) as executor:
-                futures = [
-                    executor.submit(f, item, *args, **kwargs) for 
-                    f, item, args, kwargs in iterable
-                ]
-                for future in concurrent.futures.as_completed(futures):
-                    yield future.result()   
+                # futures = [
+                #     executor.submit(f, item, *args, **kwargs) for 
+                #     f, item, args, kwargs in iterable
+                # ]
+                # for future in concurrent.futures.as_completed(futures):
+                #     yield future.result()
+                yield from self._submit_tasks(
+                    iterable=iterable, executor=executor, 
+                    tuple_to_args=tuple_to_args, dict_to_kwargs=dict_to_kwargs
+                )
+
+
+    def _submit_tasks(
+        self, iterable: Iterable, 
+        executor: Union[
+            concurrent.futures.ThreadPoolExecutor, 
+            concurrent.futures.ProcessPoolExecutor
+        ],
+        tuple_to_args: Optional[bool] = True, 
+        dict_to_kwargs: Optional[bool] = True
+    ) -> Generator:
+        futures: list = list()
+        for f, item, args, kwargs in iterable:
+            if tuple_to_args and isinstance(item, Tuple):
+                futures.append(executor.submit(f, *item, *args, **kwargs))
+            elif dict_to_kwargs and isinstance(item, Dict):
+                futures.append(executor.submit(f, *args, **item, **kwargs))
+            else:
+                futures.append(executor.submit(f, item, *args, **kwargs))
+        for future in concurrent.futures.as_completed(futures):
+            yield future.result()
 
 
 class ThreadPooler(Pooler):
     def __init__(
         self, *args, 
         DefaultExecutor: Optional[type] = concurrent.futures.ThreadPoolExecutor,
         **kwargs
@@ -96,32 +130,58 @@
                 "Both `max_workers` and `queue_size` must be set if `executor` is not passed."
         self.max_workers = max_workers
         self.DefaultBlockingExecutor = DefaultBlockingExecutor
         self.queue_size = queue_size
         self.executor = executor
 
 
+    def _submit_task(
+        self, f: Callable, item: Any,
+        executor: Union[
+            concurrent.futures.ThreadPoolExecutor, 
+            concurrent.futures.ProcessPoolExecutor
+        ],
+        tuple_to_args: Optional[bool] = True, 
+        dict_to_kwargs: Optional[bool] = True,
+        *args, **kwargs
+    ) -> Future:
+        if tuple_to_args and isinstance(item, Tuple):
+            return executor.submit(f, *item, *args, **kwargs)
+        elif dict_to_kwargs and isinstance(item, Dict):
+            return executor.submit(f, *args, **item, **kwargs)
+        else:
+            return executor.submit(f, item, *args, **kwargs)
+
+
     def _blocking_submitter(
         self,  iterable: Iterable, queue_size: int,
         executor: Optional[Union[
             concurrent.futures.ThreadPoolExecutor, 
             concurrent.futures.ProcessPoolExecutor
         ]] = None,
+        tuple_to_args: Optional[bool] = True, 
+        dict_to_kwargs: Optional[bool] = True,
     ) -> Generator:
         futures = dict()
         exhausted = False
         num_submitted = 0
         while True:
             while not exhausted and num_submitted < queue_size:
                 try:
                     f, item, args, kwargs = next(iterable)
                 except StopIteration:
                     exhausted = True
                     break
-                futures[executor.submit(f, item, *args, **kwargs)] = "Done"
+                # futures[executor.submit(f, item, *args, **kwargs)] = "Done"
+                futures[
+                    self._submit_task(
+                        f=f, item=item, executor=executor, tuple_to_args=tuple_to_args, 
+                        dict_to_kwargs=dict_to_kwargs, *args, **kwargs
+                    )
+                ] = "Done"
                 num_submitted += 1
             if futures: # There's at least one task left to await
                 done, _ = concurrent.futures.wait(
                     futures, return_when=concurrent.futures.FIRST_COMPLETED
                 ) # Will block until at least one future finishes or cancels
                 future = done.pop()
                 yield future.result()
@@ -135,33 +195,37 @@
 
     def __call__(
         self, iterable: Iterable, max_workers: Optional[int] = None,
         queue_size: Optional[int] = None,
         executor: Optional[Union[
             concurrent.futures.ThreadPoolExecutor, 
             concurrent.futures.ProcessPoolExecutor
-        ]] = None
+        ]] = None,
+        tuple_to_args: Optional[bool] = True, 
+        dict_to_kwargs: Optional[bool] = True,
     ) -> Generator:
         if max_workers is None:
             max_workers = self.max_workers
         if queue_size is None:
             queue_size = self.queue_size
         if executor is None:
             executor = self.executor     
 
         if executor is not None:
             yield from self._blocking_submitter(
-                iterable=iterable, queue_size=queue_size, executor=executor
+                iterable=iterable, queue_size=queue_size, executor=executor,
+                tuple_to_args=tuple_to_args, dict_to_kwargs=dict_to_kwargs
             )
         else:
             with self.DefaultBlockingExecutor(
                 max_workers=max_workers,
             ) as executor:
                 yield from self._blocking_submitter(
-                    iterable=iterable, queue_size=queue_size, executor=executor
+                    iterable=iterable, queue_size=queue_size, executor=executor,
+                    tuple_to_args=tuple_to_args, dict_to_kwargs=dict_to_kwargs
                 )
 
 
 class BlockingThreadPooler(BlockingPooler):
     def __init__(
         self, *args, 
         DefaultBlockingExecutor: Optional[type] = concurrent.futures.ThreadPoolExecutor,
@@ -191,20 +255,26 @@
             if isinstance(result, Coroutine):
                 return await result
             return result
         return async_wrapper
 
 
     def _get_tasks(
-        self, iterable: Iterable, **kwargs
+        self, iterable: Iterable, tuple_to_args: Optional[bool] = True, 
+        dict_to_kwargs: Optional[bool] = True, **kwargs
     ) -> List[asyncio.Task]:
         tasks = list()
         for f, item, args, wkwargs in iterable:
             f = self._make_async_decorator(f)
-            tasks.append(f(item, *args, **kwargs, **wkwargs))
+            if tuple_to_args and isinstance(item, Tuple):
+                tasks.append(f(*item, *args, **kwargs, **wkwargs))
+            elif dict_to_kwargs and isinstance(item, Dict):
+                tasks.append(f(*args, **item, **kwargs, **wkwargs))
+            else:
+                tasks.append(f(item, *args, **kwargs, **wkwargs))
         return tasks
             
 
     async def _async_gen(
         self, iterable: Iterable, **kwargs
     ) -> AsyncGenerator:
         tasks = self._get_tasks(iterable, **kwargs)
@@ -230,83 +300,17 @@
             if done:
                 break
             yield obj        
 
 
     def __call__(
         self, iterable: Iterable,
-        loop: Optional[asyncio.AbstractEventLoop] = None, 
+        loop: Optional[asyncio.AbstractEventLoop] = None,
+        tuple_to_args: Optional[bool] = True, 
+        dict_to_kwargs: Optional[bool] = True,
     ) -> Generator:
         if loop is None:
             loop = asyncio.get_event_loop()
-        async_generator = self._async_gen(iterable)
+        async_generator = self._async_gen(
+            iterable, tuple_to_args=tuple_to_args, dict_to_kwargs=dict_to_kwargs
+        )
         yield from self._iter(loop, async_generator)
-
-
-class TestParallelizers(unittest.TestCase):
-    @staticmethod
-    def task(num_tasks_submitted: int):
-        num_tasks_submitted[0] += 1       
-
-
-    def test_blocking_thread_pooler(self):
-        num_tasks_submitted = [0]
-
-
-        def gen(num_tasks):
-            iterable = [
-                (self.task, num_tasks_submitted, list(), dict()) for _ in range(num_tasks)
-            ]
-            yield from iterable
-
-
-        num_tasks = 1000
-        iterable = gen(num_tasks=num_tasks)
-
-        max_workers = 8
-        queue_size = 3
-        p = BlockingThreadPooler(max_workers=max_workers, queue_size=queue_size)        
-        for _ in p(iterable=iterable):
-            assert num_tasks_submitted[0] <= queue_size
-            num_tasks_submitted[0] -= 1
-
-
-    def test_blocking_process_pooler(self):
-        num_tasks_submitted = [0]
-
-
-        def gen(num_tasks):
-            iterable = [
-                (self.task, num_tasks_submitted, list(), dict()) for _ in range(num_tasks)
-            ]
-            yield from iterable
-
-
-        num_tasks = 1000
-        iterable = gen(num_tasks=num_tasks)
-
-        max_workers = 8
-        queue_size = 3
-        p = BlockingProcessPooler(max_workers=max_workers, queue_size=queue_size)        
-        for _ in p(iterable=iterable):
-            assert num_tasks_submitted[0] <= queue_size
-            num_tasks_submitted[0] -= 1            
-        
-
-    def test_async_gatherer(self):
-        async def sleep(seconds: int, *args, **kwargs):
-            await asyncio.sleep(seconds)
-
-
-        num_tasks = 1000
-        seconds = 1
-        iterable = [
-            (sleep, seconds, list(), dict()) for _ in range(num_tasks)
-        ]
-        start = time.time()
-        list(AsyncGatherer()(iterable=iterable))
-        end = time.time()
-        self.assertLessEqual(end - start, 1.5 * seconds)
-
-
-if __name__ == "__main__":
-    unittest.main()
```

### Comparing `Light-Pipe-0.2.2/light_pipe/transformer.py` & `light-pipe-0.3.0/light_pipe/transformer.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 __author__ = "Richard Correro (richard@richardcorrero.com)"
 
 
 import functools
 from typing import Callable, Generator, Iterable, Iterator, Optional
 
-from light_pipe import data, parallelizer
+from .data import Data
+from .parallelizer import Parallelizer
 
 
 class Transformer:
     __name__: str = "Transformer"
 
 
     def __init__(
         self, transform_item: Optional[Callable] = None,
         join_fn: Optional[Callable] = None,
-        parallelizer: Optional[parallelizer.Parallelizer] = parallelizer.Parallelizer(),
+        parallelizer: Optional[Parallelizer] = Parallelizer(),
         *args, **kwargs
     ):
         if transform_item is not None:
             self.transform_item = transform_item
         self.join_fn = join_fn
         self.parallelizer = parallelizer
         self.args = args
@@ -28,39 +29,41 @@
     @classmethod
     def fork(
         cls, f: Callable, iterable: Iterable, *args,
         recurse: Optional[bool] = True, **kwargs
     ) -> Generator:
         if recurse:
             for item in iterable:
-                if isinstance(item, data.Data) or isinstance(item, Iterator):
+                if isinstance(item, Data) or isinstance(item, Iterator):
                     yield from cls.fork(f, item, *args, recurse=recurse, **kwargs)
                 else:
                     yield f, item, args, kwargs
         else:
             for item in iterable:
                 yield f, item, args, kwargs           
 
 
     @classmethod
     def join(cls, iterable: Iterable, recurse: Optional[bool] = True) -> Generator:
         for item in iterable:
             if recurse and (
-                isinstance(item, data.Data) or isinstance(item, Iterator)
+                isinstance(item, Data) or isinstance(item, Iterator)
             ):
                 yield from cls.join(item, recurse=recurse)
             else:
                 yield item
 
 
     @staticmethod
     def transform_item(*args, **kwargs):
         raise NotImplementedError(
-            f"Either pass a `Callable` instance to __init__() or overwrite this \
-                method in a subclass of {Transformer.__name__}."
+            (
+                f"Either pass a `Callable` instance to __init__() or overwrite this "
+                f"method in a subclass of {Transformer.__name__}."
+            )
         )
 
 
     def _make_decorator(self, *args, recurse: Optional[bool] = True, **kwargs):
         def decorator(fn: Callable):
             @functools.wraps(fn)
             def wrapper(*wargs, **wkwargs):
@@ -78,36 +81,36 @@
                     recurse=recurse
                 )
             return wrapper
         return decorator
 
 
     def transform(
-        self, data: data.Data, *args, return_copy: Optional[bool] = True,
+        self, data: Data, *args, return_copy: Optional[bool] = True,
         block: Optional[bool] = False, **kwargs
-    ) -> data.Data:
+    ) -> Data:
         decorator = self._make_decorator(*args, *self.args, **kwargs, **self.kwargs)
         if return_copy:
             data = data.copy(*args, **kwargs)
         data.wrap_generator(decorator, *args, **kwargs)
         if block:
             data.store_results = True # Overwrite setting when blocking on transformer
             data(block=block, no_return=True)
         return data
 
 
-    def __call__(self, data: data.Data, *args, **kwargs):
+    def __call__(self, data: Data, *args, **kwargs):
         return self.transform(data, *args, **kwargs)
 
 
-    def __ror__(self, data: data.Data):
+    def __ror__(self, data: Data):
         return self(data, return_copy=True)
 
 
-    def __rlshift__(self, data: data.Data):
+    def __rlshift__(self, data: Data):
         """
         The left-shift operator is overloaded for symmetry with the right-shift
         operator overloading. Currently 
         ```
             Data(...) | Transformer(...)
         ```
         and 
@@ -115,10 +118,17 @@
             Data(...) << Transformer(...)
         ```
         do the same thing.
         """
         return self(data, return_copy=True)        
 
 
-    def __rrshift__(self, data: data.Data):
-        return self(data, return_copy=False) 
-    
+    def __rrshift__(self, data: Data):
+        return self(data, return_copy=False)
+    
+
+def make_transformer(
+    transform_item: Optional[Callable] = None
+) -> Callable:
+    def transformer_wrapper(*args, **kwargs) -> Transformer:
+        return Transformer(transform_item=transform_item, *args, **kwargs)
+    return transformer_wrapper
```

