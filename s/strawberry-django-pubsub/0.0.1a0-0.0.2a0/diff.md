# Comparing `tmp/strawberry_django_pubsub-0.0.1a0.tar.gz` & `tmp/strawberry_django_pubsub-0.0.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_django_pubsub-0.0.1a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "strawberry_django_pubsub-0.0.2a0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `strawberry_django_pubsub-0.0.1a0.tar` & `strawberry_django_pubsub-0.0.2a0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090251 strawberry_django_pubsub-0.0.1a0/.flake8
--rw-r--r--   0        0        0     3187 2023-05-22 12:10:46.979031 strawberry_django_pubsub-0.0.1a0/.gitignore
--rw-r--r--   0        0        0      264 2023-05-25 12:49:21.090454 strawberry_django_pubsub-0.0.1a0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1058 2023-05-26 06:42:27.160926 strawberry_django_pubsub-0.0.1a0/LICENSE
--rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090542 strawberry_django_pubsub-0.0.1a0/Makefile
--rw-r--r--   0        0        0       29 2023-04-26 10:05:26.787023 strawberry_django_pubsub-0.0.1a0/README.md
--rw-r--r--   0        0        0     1690 2023-05-25 12:50:39.844857 strawberry_django_pubsub-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0     1959 2023-05-25 12:49:21.090815 strawberry_django_pubsub-0.0.1a0/requirements/compile.py
--rw-r--r--   0        0        0     3938 2023-05-25 12:49:21.090957 strawberry_django_pubsub-0.0.1a0/requirements/py310-django41.txt
--rw-r--r--   0        0        0     3936 2023-05-25 12:49:21.091083 strawberry_django_pubsub-0.0.1a0/requirements/py310-django42.txt
--rw-r--r--   0        0        0     3529 2023-05-25 12:49:21.091198 strawberry_django_pubsub-0.0.1a0/requirements/py311-django41.txt
--rw-r--r--   0        0        0     3527 2023-05-25 12:49:21.091307 strawberry_django_pubsub-0.0.1a0/requirements/py311-django42.txt
--rw-r--r--   0        0        0     3937 2023-05-25 12:49:21.091429 strawberry_django_pubsub-0.0.1a0/requirements/py39-django41.txt
--rw-r--r--   0        0        0     3935 2023-05-25 12:49:21.091548 strawberry_django_pubsub-0.0.1a0/requirements/py39-django42.txt
--rw-r--r--   0        0        0       68 2023-05-25 12:49:21.091644 strawberry_django_pubsub-0.0.1a0/requirements/requirements.in
--rw-r--r--   0        0        0       61 2023-05-25 12:50:21.821834 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/__init__.py
--rw-r--r--   0        0        0     5772 2023-05-26 06:41:20.398004 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/asgi.py
--rw-r--r--   0        0        0      521 2023-05-25 12:49:21.091987 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/context.py
--rw-r--r--   0        0        0     1435 2023-05-25 12:49:21.092317 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/debug.py
--rw-r--r--   0        0        0      484 2023-05-25 12:49:21.092418 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/event.py
--rw-r--r--   0        0        0      700 2023-05-25 12:49:21.092518 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/exceptions.py
--rw-r--r--   0        0        0     1992 2023-05-25 12:49:21.092654 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py
--rw-r--r--   0        0        0     4157 2023-05-25 12:49:21.092782 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/queue.py
--rw-r--r--   0        0        0      264 2023-05-25 12:49:21.092910 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/types.py
--rw-r--r--   0        0        0      507 2023-05-25 12:49:21.093182 strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/utils.py
--rw-r--r--   0        0        0      324 2023-05-25 12:49:21.093287 strawberry_django_pubsub-0.0.1a0/tox.ini
--rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 strawberry_django_pubsub-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090251 strawberry_django_pubsub-0.0.2a0/.flake8
+-rw-r--r--   0        0        0     3187 2023-05-22 12:10:46.979031 strawberry_django_pubsub-0.0.2a0/.gitignore
+-rw-r--r--   0        0        0      264 2023-05-25 12:49:21.090454 strawberry_django_pubsub-0.0.2a0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1058 2023-05-26 06:42:27.160926 strawberry_django_pubsub-0.0.2a0/LICENSE
+-rw-r--r--   0        0        0       56 2023-05-25 12:49:21.090542 strawberry_django_pubsub-0.0.2a0/Makefile
+-rw-r--r--   0        0        0       29 2023-04-26 10:05:26.787023 strawberry_django_pubsub-0.0.2a0/README.md
+-rw-r--r--   0        0        0     1690 2023-05-25 12:50:39.844857 strawberry_django_pubsub-0.0.2a0/pyproject.toml
+-rw-r--r--   0        0        0     1959 2023-05-25 12:49:21.090815 strawberry_django_pubsub-0.0.2a0/requirements/compile.py
+-rw-r--r--   0        0        0     3938 2023-05-25 12:49:21.090957 strawberry_django_pubsub-0.0.2a0/requirements/py310-django41.txt
+-rw-r--r--   0        0        0     3936 2023-05-25 12:49:21.091083 strawberry_django_pubsub-0.0.2a0/requirements/py310-django42.txt
+-rw-r--r--   0        0        0     3529 2023-05-25 12:49:21.091198 strawberry_django_pubsub-0.0.2a0/requirements/py311-django41.txt
+-rw-r--r--   0        0        0     3527 2023-05-25 12:49:21.091307 strawberry_django_pubsub-0.0.2a0/requirements/py311-django42.txt
+-rw-r--r--   0        0        0     3937 2023-05-25 12:49:21.091429 strawberry_django_pubsub-0.0.2a0/requirements/py39-django41.txt
+-rw-r--r--   0        0        0     3935 2023-05-25 12:49:21.091548 strawberry_django_pubsub-0.0.2a0/requirements/py39-django42.txt
+-rw-r--r--   0        0        0       68 2023-05-25 12:49:21.091644 strawberry_django_pubsub-0.0.2a0/requirements/requirements.in
+-rw-r--r--   0        0        0       61 2023-05-26 09:07:05.164020 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/__init__.py
+-rw-r--r--   0        0        0     5812 2023-05-26 09:06:21.618698 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/asgi.py
+-rw-r--r--   0        0        0      521 2023-05-25 12:49:21.091987 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/context.py
+-rw-r--r--   0        0        0     1435 2023-05-25 12:49:21.092317 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/debug.py
+-rw-r--r--   0        0        0      484 2023-05-25 12:49:21.092418 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/event.py
+-rw-r--r--   0        0        0      700 2023-05-25 12:49:21.092518 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/exceptions.py
+-rw-r--r--   0        0        0     1992 2023-05-25 12:49:21.092654 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py
+-rw-r--r--   0        0        0     4157 2023-05-25 12:49:21.092782 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/queue.py
+-rw-r--r--   0        0        0      264 2023-05-25 12:49:21.092910 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/types.py
+-rw-r--r--   0        0        0      507 2023-05-25 12:49:21.093182 strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/utils.py
+-rw-r--r--   0        0        0      324 2023-05-25 12:49:21.093287 strawberry_django_pubsub-0.0.2a0/tox.ini
+-rw-r--r--   0        0        0     1354 1970-01-01 00:00:00.000000 strawberry_django_pubsub-0.0.2a0/PKG-INFO
```

### Comparing `strawberry_django_pubsub-0.0.1a0/.gitignore` & `strawberry_django_pubsub-0.0.2a0/.gitignore`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/LICENSE` & `strawberry_django_pubsub-0.0.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/pyproject.toml` & `strawberry_django_pubsub-0.0.2a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/requirements/compile.py` & `strawberry_django_pubsub-0.0.2a0/requirements/compile.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/requirements/py310-django41.txt` & `strawberry_django_pubsub-0.0.2a0/requirements/py310-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/requirements/py310-django42.txt` & `strawberry_django_pubsub-0.0.2a0/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/requirements/py311-django41.txt` & `strawberry_django_pubsub-0.0.2a0/requirements/py311-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/requirements/py311-django42.txt` & `strawberry_django_pubsub-0.0.2a0/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/requirements/py39-django41.txt` & `strawberry_django_pubsub-0.0.2a0/requirements/py39-django41.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/requirements/py39-django42.txt` & `strawberry_django_pubsub-0.0.2a0/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/asgi.py` & `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/asgi.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,16 @@
         """
         Handles ASGI Websocket protocol for Django, without channels dependency.
         """
 
         self.scope = scope
         self._send = send
 
+        self.user = self.scope['user']
+
         self.client_state = WebSocketState.CONNECTING
         self.application_state = WebSocketState.CONNECTING
 
         # ensure where mounted on a websocket
         if not self.scope["type"] == WEBSOCKET_TYPE:
             pretty_print_event(
                 "Connection denied", context=self.scope, debug=self.debug
```

### Comparing `strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/context.py` & `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/context.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/debug.py` & `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/debug.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/exceptions.py` & `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/exceptions.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py` & `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/handlers/graphql_transport_ws_handler.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/strawberry_django_pubsub/queue.py` & `strawberry_django_pubsub-0.0.2a0/strawberry_django_pubsub/queue.py`

 * *Files identical despite different names*

### Comparing `strawberry_django_pubsub-0.0.1a0/PKG-INFO` & `strawberry_django_pubsub-0.0.2a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-django-pubsub
-Version: 0.0.1a0
+Version: 0.0.2a0
 Summary: Strawberry Django PubSub 
 Author-email: DK <dk@terminalkitten.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 4.1
```

