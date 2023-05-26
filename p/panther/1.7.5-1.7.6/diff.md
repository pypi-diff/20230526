# Comparing `tmp/panther-1.7.5.tar.gz` & `tmp/panther-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panther-1.7.5.tar", last modified: Tue May 16 14:09:33 2023, max compression
+gzip compressed data, was "panther-1.7.6.tar", last modified: Fri May 26 10:27:58 2023, max compression
```

## Comparing `panther-1.7.5.tar` & `panther-1.7.6.tar`

### file list

```diff
@@ -1,55 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:09:33.897847 panther-1.7.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-16 14:09:18.000000 panther-1.7.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-16 14:09:33.897847 panther-1.7.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-16 14:09:18.000000 panther-1.7.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:09:33.893846 panther-1.7.5/panther/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-16 14:09:18.000000 panther-1.7.5/panther/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-16 14:09:18.000000 panther-1.7.5/panther/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-16 14:09:18.000000 panther-1.7.5/panther/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-16 14:09:18.000000 panther-1.7.5/panther/authentications.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-16 14:09:18.000000 panther-1.7.5/panther/caching.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:09:33.893846 panther-1.7.5/panther/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 14:09:18.000000 panther-1.7.5/panther/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-16 14:09:18.000000 panther-1.7.5/panther/cli/create_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-16 14:09:18.000000 panther-1.7.5/panther/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-16 14:09:18.000000 panther-1.7.5/panther/cli/monitor_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-16 14:09:18.000000 panther-1.7.5/panther/cli/run_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-16 14:09:18.000000 panther-1.7.5/panther/cli/template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-16 14:09:18.000000 panther-1.7.5/panther/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-05-16 14:09:18.000000 panther-1.7.5/panther/configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:09:33.893846 panther-1.7.5/panther/db/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-16 14:09:18.000000 panther-1.7.5/panther/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-16 14:09:18.000000 panther-1.7.5/panther/db/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1024 2023-05-16 14:09:18.000000 panther-1.7.5/panther/db/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:09:33.893846 panther-1.7.5/panther/db/queries/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 14:09:18.000000 panther-1.7.5/panther/db/queries/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-16 14:09:18.000000 panther-1.7.5/panther/db/queries/mongodb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-16 14:09:18.000000 panther-1.7.5/panther/db/queries/pantherdb_queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-16 14:09:18.000000 panther-1.7.5/panther/db/queries/queries.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-16 14:09:18.000000 panther-1.7.5/panther/db/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 14:09:18.000000 panther-1.7.5/panther/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-16 14:09:18.000000 panther-1.7.5/panther/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7824 2023-05-16 14:09:18.000000 panther-1.7.5/panther/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:09:33.897847 panther-1.7.5/panther/middlewares/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-16 14:09:18.000000 panther-1.7.5/panther/middlewares/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-16 14:09:18.000000 panther-1.7.5/panther/middlewares/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-16 14:09:18.000000 panther-1.7.5/panther/middlewares/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-16 14:09:18.000000 panther-1.7.5/panther/middlewares/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-16 14:09:18.000000 panther-1.7.5/panther/middlewares/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-16 14:09:18.000000 panther-1.7.5/panther/permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-16 14:09:18.000000 panther-1.7.5/panther/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-16 14:09:18.000000 panther-1.7.5/panther/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-16 14:09:18.000000 panther-1.7.5/panther/routings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-16 14:09:18.000000 panther-1.7.5/panther/status.py
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-16 14:09:18.000000 panther-1.7.5/panther/throttling.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-16 14:09:18.000000 panther-1.7.5/panther/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:09:33.893846 panther-1.7.5/panther.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-16 14:09:33.000000 panther-1.7.5/panther.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-16 14:09:33.000000 panther-1.7.5/panther.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:09:33.000000 panther-1.7.5/panther.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-16 14:09:33.000000 panther-1.7.5/panther.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-16 14:09:33.000000 panther-1.7.5/panther.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 14:09:33.000000 panther-1.7.5/panther.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-16 14:09:18.000000 panther-1.7.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 14:09:33.897847 panther-1.7.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-16 14:09:18.000000 panther-1.7.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-26 10:27:43.000000 panther-1.7.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-26 10:27:58.124644 panther-1.7.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-26 10:27:43.000000 panther-1.7.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-26 10:27:43.000000 panther-1.7.6/panther/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 10:27:43.000000 panther-1.7.6/panther/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-26 10:27:43.000000 panther-1.7.6/panther/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-26 10:27:43.000000 panther-1.7.6/panther/authentications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-26 10:27:43.000000 panther-1.7.6/panther/caching.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/create_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/monitor_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/run_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3093 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-05-26 10:27:43.000000 panther-1.7.6/panther/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-05-26 10:27:43.000000 panther-1.7.6/panther/configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/db/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/db/queries/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/queries/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/queries/mongodb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/queries/pantherdb_queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/queries/queries.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-05-26 10:27:43.000000 panther-1.7.6/panther/db/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-26 10:27:43.000000 panther-1.7.6/panther/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-05-26 10:27:43.000000 panther-1.7.6/panther/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9849 2023-05-26 10:27:43.000000 panther-1.7.6/panther/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/middlewares/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-05-26 10:27:43.000000 panther-1.7.6/panther/middlewares/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther/panel/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-26 10:27:43.000000 panther-1.7.6/panther/panel/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 10:27:43.000000 panther-1.7.6/panther/panel/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      383 2023-05-26 10:27:43.000000 panther-1.7.6/panther/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4382 2023-05-26 10:27:43.000000 panther-1.7.6/panther/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-26 10:27:43.000000 panther-1.7.6/panther/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-26 10:27:43.000000 panther-1.7.6/panther/routings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2674 2023-05-26 10:27:43.000000 panther-1.7.6/panther/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 10:27:43.000000 panther-1.7.6/panther/throttling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 10:27:43.000000 panther-1.7.6/panther/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 10:27:58.124644 panther-1.7.6/panther.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5090 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 10:27:58.000000 panther-1.7.6/panther.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-26 10:27:43.000000 panther-1.7.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 10:27:58.124644 panther-1.7.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-26 10:27:43.000000 panther-1.7.6/setup.py
```

### Comparing `panther-1.7.5/LICENSE` & `panther-1.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/PKG-INFO` & `panther-1.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.5
+Version: 1.7.6
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panther-1.7.5/README.md` & `panther-1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/_utils.py` & `panther-1.7.6/panther/_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,23 +52,23 @@
     if monitoring is not None:
         await monitoring.after(status_code=status_code)
 
     await _http_response_start(send, status_code=status_code)
     await _http_response_body(send, body=body)
 
 
-def import_class(_klass: str, /):
+def import_class(dotted_path: str, /):
     """
     Example:
         Input: panther.db.models.User
         Output: User (The Class)
     """
-    seperator = _klass.rfind('.')
-    module = importlib.import_module(_klass[:seperator])
-    return getattr(module, _klass[seperator + 1:])
+    path, name = dotted_path.rsplit('.', 1)
+    module = importlib.import_module(path)
+    return getattr(module, name)
 
 
 def read_multipart_form_data(content_type: str, body: str) -> dict:
     """
     content_type = 'application/json'
     content_type = 'multipart/form-data; boundary=--------------------------984465134948354357674418'
     """
```

### Comparing `panther-1.7.5/panther/app.py` & `panther-1.7.6/panther/app.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/authentications.py` & `panther-1.7.6/panther/authentications.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/caching.py` & `panther-1.7.6/panther/caching.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/cli/create_command.py` & `panther-1.7.6/panther/cli/create_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/cli/main.py` & `panther-1.7.6/panther/cli/main.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/cli/monitor_command.py` & `panther-1.7.6/panther/cli/monitor_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/cli/run_command.py` & `panther-1.7.6/panther/cli/run_command.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/cli/template.py` & `panther-1.7.6/panther/cli/template.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/cli/utils.py` & `panther-1.7.6/panther/cli/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/configs.py` & `panther-1.7.6/panther/configs.py`

 * *Files 13% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     db_engine: str
     default_cache_exp: timedelta | None
     secret_key: bytes | None
     authentication: ModelMetaclass | None
     jwt_config: JWTConfig | None
     user_model: ModelMetaclass | None
     throttling: Throttling | None
+    models: list[dict]
 
 
 config: Config = {
     'base_dir': Path(),
     'monitoring': False,
     'log_queries': False,
     'secret_key': None,
@@ -40,8 +41,9 @@
     'reversed_middlewares': [],
     'db_engine': '',
     'default_cache_exp': None,
     'jwt_config': None,
     'authentication': None,
     'user_model': None,
     'throttling': None,
+    'models': [],
 }
```

### Comparing `panther-1.7.5/panther/db/connection.py` & `panther-1.7.6/panther/db/connection.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/db/models.py` & `panther-1.7.6/panther/db/models.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import bson
-from pydantic import Field
-from pydantic.main import BaseModel as PydanticBaseModel
+from pydantic import Field, BaseModel as PydanticBaseModel
 
 from panther.configs import config
 from panther.db.queries import Query
 
 
 class BsonObjectId(bson.ObjectId):
     @classmethod
```

### Comparing `panther-1.7.5/panther/db/queries/mongodb_queries.py` & `panther-1.7.6/panther/db/queries/mongodb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/db/queries/pantherdb_queries.py` & `panther-1.7.6/panther/db/queries/pantherdb_queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/db/queries/queries.py` & `panther-1.7.6/panther/db/queries/queries.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/db/utils.py` & `panther-1.7.6/panther/db/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/exceptions.py` & `panther-1.7.6/panther/exceptions.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/logger.py` & `panther-1.7.6/panther/logger.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/main.py` & `panther-1.7.6/panther/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+import ast
 import asyncio
 from pathlib import Path
 from runpy import run_path
 from pydantic.main import ModelMetaclass
 
 from panther import status
 from panther.request import Request
@@ -15,19 +17,18 @@
 
 """ We can't import logger on the top cause it needs config['base_dir'] ans its fill in __init__ """
 
 
 class Panther:
 
     def __init__(self, name):
-        import os
         os.system('clear')
         config['base_dir'] = Path(name).resolve().parent
+        self.panther_dir = Path(__file__).parent
         self.load_configs()
-        del os
 
     def load_configs(self) -> None:
         from panther.logger import logger
         logger.debug(f'Base directory: {config["base_dir"]}')
 
         # Check & Read The Configs File
         self._check_configs()
@@ -42,19 +43,26 @@
         config['middlewares'] = self._get_middlewares()
         config['reversed_middlewares'] = config['middlewares'][::-1]
         config['user_model'] = self._get_user_model()
 
         config['authentication'] = self._get_authentication_class()
         config['jwt_config'] = self._get_jwt_config()
 
+        # Find Database Models
+        self.collect_models_for_panel()
+
         # Check & Collect URLs
         #   check_urls should be the last call in load_configs,
         #   because it will read all files and load them.
         config['urls'] = self._load_urls()
 
+        # This import shouldn't be on top
+        from panther.panel.urls import urls as panel_urls
+        config['urls']['_panel'] = panel_urls
+
         logger.debug('Configs loaded.')
         if config['monitoring']:
             logger.info('Run "panther monitor" in another session for Monitoring.')
 
     def _load_urls(self) -> dict:
         urls = check_urls(self.settings.get('URLs')) or {}
         collect_urls('', urls, collected_urls := dict())
@@ -99,14 +107,46 @@
 
     def _get_jwt_config(self) -> JWTConfig:
         """Only Collect JWT Config If Authentication Is JWTAuthentication"""
         if getattr(config['authentication'], '__name__', None) == 'JWTAuthentication':
             user_config = self.settings.get('JWTConfig')
             return JWTConfig(**user_config) if user_config else JWTConfig(key=config['secret_key'].decode())
 
+    def collect_models_for_panel(self):
+        from panther.db.models import Model
+
+        for root, _, files in os.walk(config['base_dir']):
+            # Traverse through each directory
+            for f in files:
+                # Traverse through each file of directory
+                if f == 'models.py':
+                    # If the file was "models.py" read it
+                    file_path = f'{root}/models.py'
+                    with open(file_path, 'r') as file:
+                        # Parse the file with ast
+                        node = ast.parse(file.read())
+                        for n in node.body:
+                            # Find classes in each element of files' body
+                            if type(n) is ast.ClassDef and n.bases:
+                                class_path = file_path\
+                                    .removesuffix('/models.py')\
+                                    .removeprefix(f'{config["base_dir"]}/')\
+                                    .replace('/', '.')
+                                # Import the class to check his father and brother
+                                klass = import_class(f'{class_path}.models.{n.name}')
+                                for parent in klass.__mro__:
+                                    if parent is Model:
+                                        # The class was one our database models so collect it
+                                        config['models'].append({
+                                            'name': n.name,
+                                            'path':  file_path,
+                                            'class': klass,
+                                            'app': class_path.split('.'),
+                                        })
+
     async def __call__(self, scope, receive, send) -> None:
         """
         We Used Python3.11 For asyncio.TaskGroup()
         1.
             async with asyncio.TaskGroup() as tg:
                 tg.create_task(self.run(scope, receive, send))
         2.
```

### Comparing `panther-1.7.5/panther/middlewares/monitoring.py` & `panther-1.7.6/panther/middlewares/monitoring.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/middlewares/redis.py` & `panther-1.7.6/panther/middlewares/redis.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/request.py` & `panther-1.7.6/panther/request.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/response.py` & `panther-1.7.6/panther/response.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/routings.py` & `panther-1.7.6/panther/routings.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/status.py` & `panther-1.7.6/panther/status.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther/utils.py` & `panther-1.7.6/panther/utils.py`

 * *Files identical despite different names*

### Comparing `panther-1.7.5/panther.egg-info/PKG-INFO` & `panther-1.7.6/panther.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panther
-Version: 1.7.5
+Version: 1.7.6
 Summary: Fast &  Friendly, Web Framework For Building Async APIs
 Home-page: https://github.com/alirn76/panther
 Author: Ali RajabNezhad
 Author-email: alirn76@yahoo.com
 License: MIT
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `panther-1.7.5/panther.egg-info/SOURCES.txt` & `panther-1.7.6/panther.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -39,8 +39,10 @@
 panther/db/queries/mongodb_queries.py
 panther/db/queries/pantherdb_queries.py
 panther/db/queries/queries.py
 panther/middlewares/__init__.py
 panther/middlewares/base.py
 panther/middlewares/db.py
 panther/middlewares/monitoring.py
-panther/middlewares/redis.py
+panther/middlewares/redis.py
+panther/panel/apis.py
+panther/panel/urls.py
```

### Comparing `panther-1.7.5/setup.py` & `panther-1.7.6/setup.py`

 * *Files identical despite different names*

