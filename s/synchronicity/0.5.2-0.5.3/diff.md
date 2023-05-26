# Comparing `tmp/synchronicity-0.5.2-py3-none-any.whl.zip` & `tmp/synchronicity-0.5.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,16 @@
-Zip file size: 22841 bytes, number of entries: 13
--rw-rw-r--  2.0 unx      100 b- defN 23-May-10 19:02 synchronicity/__init__.py
--rw-rw-r--  2.0 unx     1188 b- defN 23-May-12 07:52 synchronicity/annotations.py
--rw-rw-r--  2.0 unx     2581 b- defN 23-May-11 08:00 synchronicity/async_wrap.py
--rw-rw-r--  2.0 unx     1485 b- defN 23-Mar-23 14:53 synchronicity/callback.py
--rw-rw-r--  2.0 unx     1303 b- defN 23-Mar-20 08:05 synchronicity/exceptions.py
--rw-rw-r--  2.0 unx      331 b- defN 23-May-10 19:02 synchronicity/interface.py
--rw-rw-r--  2.0 unx     1792 b- defN 23-May-10 19:02 synchronicity/overload_tracking.py
--rw-rw-r--  2.0 unx    30159 b- defN 23-May-12 08:26 synchronicity/synchronizer.py
--rw-rw-r--  2.0 unx    26494 b- defN 23-May-12 11:52 synchronicity/type_stubs.py
--rw-rw-r--  2.0 unx     7736 b- defN 23-May-12 11:53 synchronicity-0.5.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-12 11:53 synchronicity-0.5.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       14 b- defN 23-May-12 11:53 synchronicity-0.5.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1083 b- defN 23-May-12 11:53 synchronicity-0.5.2.dist-info/RECORD
-13 files, 74358 bytes uncompressed, 21031 bytes compressed:  71.7%
+Zip file size: 23584 bytes, number of entries: 14
+-rw-rw-r--  2.0 unx      100 b- defN 23-May-24 15:12 synchronicity/__init__.py
+-rw-rw-r--  2.0 unx     1188 b- defN 23-May-24 15:12 synchronicity/annotations.py
+-rw-rw-r--  2.0 unx     2581 b- defN 23-May-24 15:12 synchronicity/async_wrap.py
+-rw-rw-r--  2.0 unx     1485 b- defN 23-May-24 15:12 synchronicity/callback.py
+-rw-rw-r--  2.0 unx     2504 b- defN 23-May-26 12:19 synchronicity/combined_types.py
+-rw-rw-r--  2.0 unx     1303 b- defN 23-May-24 15:12 synchronicity/exceptions.py
+-rw-rw-r--  2.0 unx      331 b- defN 23-May-24 15:12 synchronicity/interface.py
+-rw-rw-r--  2.0 unx     1792 b- defN 23-May-24 15:12 synchronicity/overload_tracking.py
+-rw-rw-r--  2.0 unx    28350 b- defN 23-May-26 12:19 synchronicity/synchronizer.py
+-rw-rw-r--  2.0 unx    26772 b- defN 23-May-26 12:19 synchronicity/type_stubs.py
+-rw-rw-r--  2.0 unx     7736 b- defN 23-May-26 12:26 synchronicity-0.5.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 12:26 synchronicity-0.5.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       14 b- defN 23-May-26 12:26 synchronicity-0.5.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1171 b- defN 23-May-26 12:26 synchronicity-0.5.3.dist-info/RECORD
+14 files, 75419 bytes uncompressed, 21636 bytes compressed:  71.3%
```

## zipnote {}

```diff
@@ -6,14 +6,17 @@
 
 Filename: synchronicity/async_wrap.py
 Comment: 
 
 Filename: synchronicity/callback.py
 Comment: 
 
+Filename: synchronicity/combined_types.py
+Comment: 
+
 Filename: synchronicity/exceptions.py
 Comment: 
 
 Filename: synchronicity/interface.py
 Comment: 
 
 Filename: synchronicity/overload_tracking.py
@@ -21,20 +24,20 @@
 
 Filename: synchronicity/synchronizer.py
 Comment: 
 
 Filename: synchronicity/type_stubs.py
 Comment: 
 
-Filename: synchronicity-0.5.2.dist-info/METADATA
+Filename: synchronicity-0.5.3.dist-info/METADATA
 Comment: 
 
-Filename: synchronicity-0.5.2.dist-info/WHEEL
+Filename: synchronicity-0.5.3.dist-info/WHEEL
 Comment: 
 
-Filename: synchronicity-0.5.2.dist-info/top_level.txt
+Filename: synchronicity-0.5.3.dist-info/top_level.txt
 Comment: 
 
-Filename: synchronicity-0.5.2.dist-info/RECORD
+Filename: synchronicity-0.5.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synchronicity/synchronizer.py

```diff
@@ -7,14 +7,15 @@
 import platform
 import threading
 import typing
 import warnings
 from typing import ForwardRef, Optional
 
 from synchronicity.annotations import evaluated_annotation
+from synchronicity.combined_types import MethodWithAio, FunctionWithAio
 
 from .async_wrap import wraps_by_interface
 from .callback import Callback
 from .exceptions import UserCodeException, unwrap_coro_exception, wrap_coro_exception
 from .interface import Interface
 
 _BUILTIN_ASYNC_METHODS = {
@@ -90,57 +91,14 @@
     annos = getattr(func, "__annotations__", {})
     for anno in annos.values():
         if _type_requires_aio_usage(anno, func.__module__):
             return True
     return False
 
 
-class FunctionWithAio:
-    def __init__(self, func, aio_func, synchronizer):
-        self._func = func
-        self._aio_func = self.aio = aio_func
-        self._synchronizer = synchronizer
-
-    def __call__(self, *args, **kwargs):
-        # .__call__ is special - it's being looked up on the class instead of the instance when calling something,
-        # so setting the magic method from the constructor is not possible
-        # https://stackoverflow.com/questions/22390532/object-is-not-callable-after-adding-call-method-to-instance
-        # so we need to use an explicit wrapper function here
-        try:
-            return self._func(*args, **kwargs)
-        except UserCodeException as uc_exc:
-            raise uc_exc.exc from None
-
-
-class MethodWithAio:
-    """Creates a bound method that can have callable child-properties on the method itself.
-
-    Child-properties are also bound to the parent instance.
-    """
-
-    def __init__(self, func, aio_func, synchronizer: "Synchronizer", is_classmethod=False):
-        self._func = func
-        self._aio_func = aio_func
-        self._synchronizer = synchronizer
-        self._is_classmethod = is_classmethod
-
-    def __get__(self, instance, owner=None):
-        bind_var = instance if instance and not self._is_classmethod else owner
-
-        bound_func = functools.wraps(self._func)(functools.partial(self._func, bind_var))  # bound blocking function
-        self._synchronizer._update_wrapper(bound_func, self._func, interface=Interface.BLOCKING)
-
-        bound_aio_func = wraps_by_interface(Interface._ASYNC_WITH_BLOCKING_TYPES, self._aio_func)(
-            functools.partial(self._aio_func, bind_var)
-        )  # bound async function
-        self._synchronizer._update_wrapper(bound_func, self._func, interface=Interface._ASYNC_WITH_BLOCKING_TYPES)
-        bound_func.aio = bound_aio_func
-        return bound_func
-
-
 class Synchronizer:
     """Helps you offer a blocking (synchronous) interface to asynchronous code."""
 
     def __init__(
         self,
         multiwrap_warning=False,
         async_leakage_warning=True,
```

## synchronicity/type_stubs.py

```diff
@@ -18,14 +18,15 @@
 from unittest import mock
 
 import sigtools.specifiers  # type: ignore
 from sigtools._signatures import EmptyAnnotation, UpgradedAnnotation, UpgradedParameter  # type: ignore
 
 import synchronicity
 from synchronicity import Interface, overload_tracking
+from synchronicity import combined_types
 from synchronicity.annotations import evaluated_annotation
 from synchronicity.synchronizer import (
     TARGET_INTERFACE_ATTR,
     SYNCHRONIZER_ATTR,
     MethodWithAio,
     FunctionWithAio,
 )
@@ -379,15 +380,15 @@
         mapped_args = tuple(self._translate_annotation(arg, synchronizer, interface, home_module) for arg in args)
         if interface == Interface.BLOCKING:
             # blocking interface special generic translations:
             if origin == collections.abc.AsyncGenerator:
                 return typing.Generator[mapped_args + (None,)]  # type: ignore
 
             if origin == contextlib.AbstractAsyncContextManager:
-                return typing.ContextManager[mapped_args]  # type: ignore
+                return combined_types.AsyncAndBlockingContextManager[mapped_args]  # type: ignore
 
             if origin == collections.abc.AsyncIterable:
                 return typing.Iterable[mapped_args]  # type: ignore
 
             if origin == collections.abc.AsyncIterator:
                 return typing.Iterator[mapped_args]  # type: ignore
 
@@ -505,16 +506,20 @@
                     # ellipsis (...) needs to be passed as is, or it will be reformatted
                     tuple(ReprObj(self._formatannotation(arg)) if arg != Ellipsis else Ellipsis for arg in args)
                 )
             )
         except Exception:
             raise Exception(f"Could not reformat generic {annotation.__origin__} with arguments {args}")
 
+        formatted_annotation = formatted_annotation.replace(
+            "typing.Abstract", "typing."
+        )  # fix for Python 3.7 formatting typing.AsyncContextManager as 'typing.AbstractContextManager' etc.
         # this is a bit ugly, but gets rid of incorrect module qualification of Generic subclasses:
         # TODO: find a better way...
+
         if formatted_annotation.startswith(self.target_module + "."):
             return formatted_annotation.split(self.target_module + ".", 1)[1]
         return formatted_annotation
 
     def _indent(self, level):
         return level * self._indentation
```

## Comparing `synchronicity-0.5.2.dist-info/METADATA` & `synchronicity-0.5.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synchronicity
-Version: 0.5.2
+Version: 0.5.3
 Summary: Export blocking and async library versions from a single async implementation
 Requires-Python: >=3.7.9
 Description-Content-Type: text/markdown
 Requires-Dist: sigtools (==4.0.1)
 
 ![CI/CD badge](https://github.com/erikbern/synchronicity/actions/workflows/ci.yml/badge.svg)
 [![pypi badge](https://img.shields.io/pypi/v/synchronicity.svg?style=flat)](https://pypi.python.org/pypi/synchronicity)
```

## Comparing `synchronicity-0.5.2.dist-info/RECORD` & `synchronicity-0.5.3.dist-info/RECORD`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 synchronicity/__init__.py,sha256=iLUYrr2mW166J8mGeL1pwiSRVUUdozDXPN2Y_P9hnBA,100
 synchronicity/annotations.py,sha256=aJVxrhaA4DbWxAz6udBoDlhcYoeUAAeUC2ZS_VMgYYQ,1188
 synchronicity/async_wrap.py,sha256=4Q_gBFxOOdCjcRpYGCkmv-NHeAYCes763nZqK-8laPc,2581
 synchronicity/callback.py,sha256=ZPCfzrZkaepalwEmvxdfYewHEc059hDKFz_7oXIdIoY,1485
+synchronicity/combined_types.py,sha256=-wpbAmILWSxARTS_w977fmgyUm2-Egtt1u612t52prk,2504
 synchronicity/exceptions.py,sha256=pJw_RhOvRSr-sMhSRLmCzNb1M5W36W4EFfeE0FD27OA,1303
 synchronicity/interface.py,sha256=OVodgsiXbzr9h_3q0bYc4T7qnbTaWQqorbkhYXdxwo0,331
 synchronicity/overload_tracking.py,sha256=ynM0MhkggMkUe5Dc3Nl2ZpWlbHi_srzT9IKNw21NJdU,1792
-synchronicity/synchronizer.py,sha256=kDIc9Ccr8a3mrVUoWwHNu2atgrFsHxobA4eL6yD3HVo,30159
-synchronicity/type_stubs.py,sha256=uKZ3x3-hdDQKF6cfvDxUn5ovljcZFvZ7G9NGqFUVnHM,26494
-synchronicity-0.5.2.dist-info/METADATA,sha256=HSZQRpanRkLk3KcNhJh9lbKeguknyjYaVoaDKD6O55U,7736
-synchronicity-0.5.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-synchronicity-0.5.2.dist-info/top_level.txt,sha256=pqAkRTgp1bdeADR7z1vhyQijkZNYCCsezJKpOwFizoE,14
-synchronicity-0.5.2.dist-info/RECORD,,
+synchronicity/synchronizer.py,sha256=MgZ_LSDATNalNiFEuz8h6ASLcsvkA42zhcJg6J3xArU,28350
+synchronicity/type_stubs.py,sha256=iJhGs-RjQl5YYxE0ncDOLNPtjGKwZE5Ho12UolRAZUk,26772
+synchronicity-0.5.3.dist-info/METADATA,sha256=bc9BZLd5Iy5KXtlvLaZZjsNUoYlkh6Hlg6oqgngtnPI,7736
+synchronicity-0.5.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+synchronicity-0.5.3.dist-info/top_level.txt,sha256=pqAkRTgp1bdeADR7z1vhyQijkZNYCCsezJKpOwFizoE,14
+synchronicity-0.5.3.dist-info/RECORD,,
```

