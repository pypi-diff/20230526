# Comparing `tmp/troncos-4.0.0b5.tar.gz` & `tmp/troncos-4.0.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "troncos-4.0.0b5.tar", max compression
+gzip compressed data, was "troncos-4.0.0b6.tar", max compression
```

## Comparing `troncos-4.0.0b5.tar` & `troncos-4.0.0b6.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1077 2023-05-26 08:40:43.276001 troncos-4.0.0b5/LICENSE
--rw-r--r--   0        0        0     7753 2023-05-26 08:40:43.276001 troncos-4.0.0b5/README.md
--rw-r--r--   0        0        0     2389 2023-05-26 08:40:43.276001 troncos-4.0.0b5/pyproject.toml
--rw-r--r--   0        0        0      291 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/logging/__init__.py
--rw-r--r--   0        0        0     5058 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/profiling/__init__.py
--rw-r--r--   0        0        0      576 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/asgi/profiling/app.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/celery/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.276001 troncos-4.0.0b5/troncos/contrib/celery/logging/__init__.py
--rw-r--r--   0        0        0      949 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/celery/logging/signals.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/logging/__init__.py
--rw-r--r--   0        0        0     2334 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/logging/middleware.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/profiling/__init__.py
--rw-r--r--   0        0        0      265 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/django/profiling/views.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/starlette/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/starlette/profiling/__init__.py
--rw-r--r--   0        0        0      291 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/starlette/profiling/views.py
--rw-r--r--   0        0        0     4053 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/structlog/__init__.py
--rw-r--r--   0        0        0      705 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/contrib/structlog/processors.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/__init__.py
--rw-r--r--   0        0        0      192 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/auto.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/bootstrap/__init__.py
--rw-r--r--   0        0        0      439 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/bootstrap/profile.py
--rw-r--r--   0        0        0      343 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/bootstrap/start.py
--rw-r--r--   0        0        0     1814 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/profiling/profiler.py
--rw-r--r--   0        0        0        0 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/py.typed
--rw-r--r--   0        0        0      690 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/__init__.py
--rw-r--r--   0        0        0       82 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/_enums.py
--rw-r--r--   0        0        0     2053 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/_otel.py
--rw-r--r--   0        0        0     4114 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/_span.py
--rw-r--r--   0        0        0     1886 2023-05-26 08:40:43.280001 troncos-4.0.0b5/troncos/tracing/_writer.py
--rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-26 09:46:04.242572 troncos-4.0.0b6/LICENSE
+-rw-r--r--   0        0        0     7753 2023-05-26 09:46:04.242572 troncos-4.0.0b6/README.md
+-rw-r--r--   0        0        0     2389 2023-05-26 09:46:04.242572 troncos-4.0.0b6/pyproject.toml
+-rw-r--r--   0        0        0      291 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/logging/__init__.py
+-rw-r--r--   0        0        0     5058 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/profiling/__init__.py
+-rw-r--r--   0        0        0      576 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/asgi/profiling/app.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/celery/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/celery/logging/__init__.py
+-rw-r--r--   0        0        0      949 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/celery/logging/signals.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/logging/__init__.py
+-rw-r--r--   0        0        0     2334 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/logging/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/profiling/__init__.py
+-rw-r--r--   0        0        0      265 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/django/profiling/views.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/starlette/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/starlette/profiling/__init__.py
+-rw-r--r--   0        0        0      291 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/starlette/profiling/views.py
+-rw-r--r--   0        0        0     4053 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/structlog/__init__.py
+-rw-r--r--   0        0        0      705 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/contrib/structlog/processors.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/__init__.py
+-rw-r--r--   0        0        0      192 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/auto.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/bootstrap/__init__.py
+-rw-r--r--   0        0        0      439 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/bootstrap/profile.py
+-rw-r--r--   0        0        0      343 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/bootstrap/start.py
+-rw-r--r--   0        0        0     1814 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/profiling/profiler.py
+-rw-r--r--   0        0        0        0 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/py.typed
+-rw-r--r--   0        0        0      690 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/tracing/__init__.py
+-rw-r--r--   0        0        0       82 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/tracing/_enums.py
+-rw-r--r--   0        0        0     2053 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/tracing/_otel.py
+-rw-r--r--   0        0        0     4054 2023-05-26 09:46:04.242572 troncos-4.0.0b6/troncos/tracing/_span.py
+-rw-r--r--   0        0        0     1886 2023-05-26 09:46:04.246573 troncos-4.0.0b6/troncos/tracing/_writer.py
+-rw-r--r--   0        0        0     8744 1970-01-01 00:00:00.000000 troncos-4.0.0b6/PKG-INFO
```

### Comparing `troncos-4.0.0b5/LICENSE` & `troncos-4.0.0b6/LICENSE`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/README.md` & `troncos-4.0.0b6/README.md`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/pyproject.toml` & `troncos-4.0.0b6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "troncos"
-version = "4.0.0b5"
+version = "4.0.0b6"
 description = "Collection of Python logging, tracing and profiling tools"
 authors = [
     "Guðmundur Björn Birkisson <gudmundur.birkisson@oda.com>",
     "Karl Fredrik Haugland <karlfredrik.haugland@oda.com>",
     "Eirik Martiniussen Sylliaas <eirik.sylliaas@oda.com>",
 ]
 license = "MIT"
@@ -13,17 +13,17 @@
 repository = "https://github.com/kolonialno/troncos"
 documentation = "https://github.com/kolonialno/troncos"
 keywords = ["logs", "traces", "opentelemetry"]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<4.0"
 ddtrace = "1.13.3"
-opentelemetry-sdk = "1.17.0"
-opentelemetry-exporter-otlp-proto-http = "1.17.0"
-opentelemetry-exporter-otlp-proto-grpc = {version = "1.17.0", optional = true}
+opentelemetry-sdk = "1.18.0"
+opentelemetry-exporter-otlp-proto-http = "1.18.0"
+opentelemetry-exporter-otlp-proto-grpc = {version = "1.18.0", optional = true}
 python-ipware = "^0.9.0"
 
 [tool.poetry.extras]
 grpc = ["opentelemetry-exporter-otlp-proto-grpc"]
 
 [tool.poetry.group.dev.dependencies]
 isort = "^5.12.0"
```

### Comparing `troncos-4.0.0b5/troncos/contrib/asgi/logging/middleware.py` & `troncos-4.0.0b6/troncos/contrib/asgi/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/contrib/asgi/profiling/app.py` & `troncos-4.0.0b6/troncos/contrib/asgi/profiling/app.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/contrib/celery/logging/signals.py` & `troncos-4.0.0b6/troncos/contrib/celery/logging/signals.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/contrib/django/logging/middleware.py` & `troncos-4.0.0b6/troncos/contrib/django/logging/middleware.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/contrib/structlog/__init__.py` & `troncos-4.0.0b6/troncos/contrib/structlog/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/contrib/structlog/processors.py` & `troncos-4.0.0b6/troncos/contrib/structlog/processors.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/profiling/profiler.py` & `troncos-4.0.0b6/troncos/profiling/profiler.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/tracing/__init__.py` & `troncos-4.0.0b6/troncos/tracing/__init__.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/tracing/_otel.py` & `troncos-4.0.0b6/troncos/tracing/_otel.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/troncos/tracing/_span.py` & `troncos-4.0.0b6/troncos/tracing/_span.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 from typing import Any
 
 from ddtrace import constants, ext
 from ddtrace.span import Span as DDSpan
-from opentelemetry.attributes import BoundedAttributes  # type: ignore
 from opentelemetry.sdk.resources import Resource
-from opentelemetry.sdk.trace import Event, ReadableSpan
+from opentelemetry.sdk.trace import Event, ReadableSpan, Span
 from opentelemetry.trace import SpanContext, SpanKind, Status, StatusCode
 from opentelemetry.trace.span import TraceFlags
-from opentelemetry.util import types
 
 _dd_span_ignore_attr = [
     "runtime-id",
     "_sampling_priority_v1",
     "env",
     "version",
     "span.kind",
 ]
 
 
+class _Span(Span):
+    """Class needed to allow us to make a Span outside of a tracer."""
+
+    pass
+
+
 def _span_context(span: DDSpan) -> SpanContext:
     return SpanContext(
         trace_id=span.trace_id,
         span_id=span.span_id,
         is_remote=False,
         trace_flags=TraceFlags(1),
     )
@@ -49,15 +53,15 @@
 def _span_kind(dd_span: DDSpan) -> SpanKind:
     dd_kind = dd_span._meta.get(constants.SPAN_KIND, "none")
     return _span_kind_map.get(dd_kind, SpanKind.INTERNAL)
 
 
 def _span_status_and_attributes(
     dd_span: DDSpan, ignore_attrs: list[str]
-) -> tuple[Status, list[Event], types.Attributes]:
+) -> tuple[Status, list[Event], dict[str, Any]]:
     dd_span_err_attr_mapping = {
         "error.msg": "exception.message",
         "error.type": "exception.type",
         "error.stack": "exception.stacktrace",
     }
 
     # Collect all "attributes" from the dd span
@@ -78,17 +82,15 @@
             continue
         elif otel_err_attr:
             otel_error_attrs[otel_err_attr] = v
         elif k not in ignore_attrs:
             otel_attrs[k] = v
 
     if otel_error_attrs:
-        events.append(
-            Event("exception", BoundedAttributes(attributes=otel_error_attrs))
-        )
+        events.append(Event("exception", attributes=otel_error_attrs))
 
         status_exp_type = otel_error_attrs.get("exception.type", None)
         status_exp_msg = otel_error_attrs.get("exception.message", None)
 
         status = Status(
             status_code=StatusCode.ERROR,
             description=f"{status_exp_type}: {status_exp_msg}",
@@ -117,21 +119,22 @@
     assert dd_span.duration_ns, "Span not finished."
 
     status, events, attributes = _span_status_and_attributes(
         dd_span,
         ignore_attrs=_dd_span_ignore_attr + list(default_resource.attributes.keys()),
     )
 
-    otel_span = ReadableSpan(
+    otel_span = _Span(
         name=dd_span.name,
         context=_span_context(dd_span),
         parent=_parent_span_context(dd_span),
         resource=_span_resource(dd_span, default_resource),
-        attributes=BoundedAttributes(attributes=attributes),
+        attributes=attributes,
         events=events,
         kind=_span_kind(dd_span),
-        status=status,
-        start_time=dd_span.start_ns,
-        end_time=dd_span.start_ns + dd_span.duration_ns,
     )
 
+    otel_span.set_status(status=status)
+    otel_span.start(dd_span.start_ns)
+    otel_span.end(dd_span.start_ns + dd_span.duration_ns)
+
     return otel_span
```

### Comparing `troncos-4.0.0b5/troncos/tracing/_writer.py` & `troncos-4.0.0b6/troncos/tracing/_writer.py`

 * *Files identical despite different names*

### Comparing `troncos-4.0.0b5/PKG-INFO` & `troncos-4.0.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: troncos
-Version: 4.0.0b5
+Version: 4.0.0b6
 Summary: Collection of Python logging, tracing and profiling tools
 Home-page: https://github.com/kolonialno/troncos
 License: MIT
 Keywords: logs,traces,opentelemetry
 Author: Guðmundur Björn Birkisson
 Author-email: gudmundur.birkisson@oda.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc
 Requires-Dist: ddtrace (==1.13.3)
-Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.17.0) ; extra == "grpc"
-Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.17.0)
-Requires-Dist: opentelemetry-sdk (==1.17.0)
+Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra == "grpc"
+Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0)
+Requires-Dist: opentelemetry-sdk (==1.18.0)
 Requires-Dist: python-ipware (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://github.com/kolonialno/troncos
 Project-URL: Repository, https://github.com/kolonialno/troncos
 Description-Content-Type: text/markdown
 
 <h1 align="center" style="border-bottom: 0">
   🪵<br>
```

#### html2text {}

```diff
@@ -1,18 +1,18 @@
-Metadata-Version: 2.1 Name: troncos Version: 4.0.0b5 Summary: Collection of
+Metadata-Version: 2.1 Name: troncos Version: 4.0.0b6 Summary: Collection of
 Python logging, tracing and profiling tools Home-page: https://github.com/
 kolonialno/troncos License: MIT Keywords: logs,traces,opentelemetry Author:
 GuÃ°mundur BjÃ¶rn Birkisson Author-email: gudmundur.birkisson@oda.com Requires-
 Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: grpc Requires-Dist: ddtrace (==1.13.3) Requires-Dist:
-opentelemetry-exporter-otlp-proto-grpc (==1.17.0) ; extra == "grpc" Requires-
-Dist: opentelemetry-exporter-otlp-proto-http (==1.17.0) Requires-Dist:
-opentelemetry-sdk (==1.17.0) Requires-Dist: python-ipware (>=0.9.0,<0.10.0)
+opentelemetry-exporter-otlp-proto-grpc (==1.18.0) ; extra == "grpc" Requires-
+Dist: opentelemetry-exporter-otlp-proto-http (==1.18.0) Requires-Dist:
+opentelemetry-sdk (==1.18.0) Requires-Dist: python-ipware (>=0.9.0,<0.10.0)
 Project-URL: Documentation, https://github.com/kolonialno/troncos Project-URL:
 Repository, https://github.com/kolonialno/troncos Description-Content-Type:
 text/markdown
                                   ****** ðªµ
                                    Troncos
                                      ******
           Collection of Python logging, tracing and profiling tools
```

