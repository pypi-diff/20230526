# Comparing `tmp/troncos-4.0.0b4.tar.gz` & `tmp/troncos-4.0.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.0b4.tar", max compression
+gzip compressed data, was "troncos-4.0.0b5.tar", max compression
```

## Comparing `troncos-4.0.0b4.tar` & `troncos-4.0.0b5.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1077 2023-05-25 10:04:06.571970 troncos-4.0.0b4/LICENSE
--rw-r--r--   0        0        0     7753 2023-05-25 10:04:06.571970 troncos-4.0.0b4/README.md
--rw-r--r--   0        0        0     2389 2023-05-25 10:04:06.571970 troncos-4.0.0b4/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5058 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      949 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      265 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.571970 troncos-4.0.0b4/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     4053 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      705 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/profiling/profiler.py
--rw-r--r--   0        0        0        0 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4062 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/tracing/_span.py
--rw-r--r--   0        0        0     1886 2023-05-25 10:04:06.575971 troncos-4.0.0b4/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-26 08:40:43.276001 troncos-4.0.0b5/LICENSE
+-rw-r--r--   0        0        0     7753 2023-05-26 08:40:43.276001 troncos-4.0.0b5/README.md
+-rw-r--r--   0        0        0     2389 2023-05-26 08:40:43.276001 troncos-4.0.0b5/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5058 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      949 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     4053 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4114 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     1886 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b5/PKG-INFO
```

### Comparing `troncos-4.0.0b4/LICENSE` & `troncos-4.0.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/README.md` & `troncos-4.0.0b5/README.md`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/pyproject.toml` & `troncos-4.0.0b5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.0b4"
+version = "4.0.0b5"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
```

### Comparing `troncos-4.0.0b4/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.0b5/troncos/contrib/asgi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.0b5/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/contrib/celery/logging/signals.py` & `troncos-4.0.0b5/troncos/contrib/celery/logging/signals.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.0b5/troncos/contrib/django/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/contrib/structlog/__init__.py` & `troncos-4.0.0b5/troncos/contrib/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/contrib/structlog/processors.py` & `troncos-4.0.0b5/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/profiling/profiler.py` & `troncos-4.0.0b5/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/tracing/__init__.py` & `troncos-4.0.0b5/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/tracing/_otel.py` & `troncos-4.0.0b5/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/troncos/tracing/_span.py` & `troncos-4.0.0b5/troncos/tracing/_span.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,17 @@
             continue
         elif otel_err_attr:
             otel_error_attrs[otel_err_attr] = v
         elif k not in ignore_attrs:
             otel_attrs[k] = v
 
     if otel_error_attrs:
-        events.append(Event("exception", otel_error_attrs))
+        events.append(
+            Event("exception", BoundedAttributes(attributes=otel_error_attrs))
+        )
 
         status_exp_type = otel_error_attrs.get("exception.type", None)
         status_exp_msg = otel_error_attrs.get("exception.message", None)
 
         status = Status(
             status_code=StatusCode.ERROR,
             description=f"{status_exp_type}: {status_exp_msg}",
```

### Comparing `troncos-4.0.0b4/troncos/tracing/_writer.py` & `troncos-4.0.0b5/troncos/tracing/_writer.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b4/PKG-INFO` & `troncos-4.0.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.0b4
+Version: 4.0.0b5
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.0b4 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.0b5 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc Requires-Dist: ddtrace (==1.13.3) Requires-Dist:
```

