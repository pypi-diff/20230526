# Comparing `tmp/edat_utils-0.3.4.tar.gz` & `tmp/edat_utils-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edat_utils-0.3.4.tar", last modified: Wed Apr 26 18:27:14 2023, max compression
+gzip compressed data, was "dist\edat_utils-0.3.5.tar", last modified: Thu May 25 23:41:41 2023, max compression
```

## Comparing `edat_utils-0.3.4.tar` & `edat_utils-0.3.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 18:27:14.572835 edat_utils-0.3.4/
--rw-rw-rw-   0        0        0      487 2023-04-26 18:27:14.571835 edat_utils-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-04-26 18:24:30.000000 edat_utils-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 18:27:14.562842 edat_utils-0.3.4/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 14:43:25.000000 edat_utils-0.3.4/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-04-13 20:04:16.000000 edat_utils-0.3.4/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-04-13 18:06:40.000000 edat_utils-0.3.4/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1221 2023-04-13 17:37:40.000000 edat_utils-0.3.4/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      967 2023-04-12 14:54:05.000000 edat_utils-0.3.4/edat_utils/schema.py
--rw-rw-rw-   0        0        0      785 2023-04-13 20:03:38.000000 edat_utils-0.3.4/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-04-26 18:27:14.570836 edat_utils-0.3.4/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      487 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-26 18:27:14.000000 edat_utils-0.3.4/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-26 18:27:14.572835 edat_utils-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-04-13 20:04:23.000000 edat_utils-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:41:41.576445 edat_utils-0.3.5/
+-rw-rw-rw-   0        0        0      555 2023-05-25 23:41:41.576445 edat_utils-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-25 23:37:25.000000 edat_utils-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-25 23:41:41.560920 edat_utils-0.3.5/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.3.5/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-05-25 23:37:25.000000 edat_utils-0.3.5/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.3.5/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1174 2023-05-25 23:37:25.000000 edat_utils-0.3.5/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.3.5/edat_utils/schema.py
+-rw-rw-rw-   0        0        0      785 2023-05-25 23:37:25.000000 edat_utils-0.3.5/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-25 23:41:41.570483 edat_utils-0.3.5/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-25 23:41:41.000000 edat_utils-0.3.5/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-25 23:41:41.000000 edat_utils-0.3.5/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-25 23:41:41.000000 edat_utils-0.3.5/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-25 23:41:41.000000 edat_utils-0.3.5/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-25 23:41:41.000000 edat_utils-0.3.5/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-25 23:41:41.579761 edat_utils-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-05-25 23:38:04.000000 edat_utils-0.3.5/setup.py
```

### Comparing `edat_utils-0.3.4/edat_utils/generic_controller.py` & `edat_utils-0.3.5/edat_utils/generic_controller.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.4/edat_utils/query_builder.py` & `edat_utils-0.3.5/edat_utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.4/edat_utils/query_runner.py` & `edat_utils-0.3.5/edat_utils/query_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from sqlalchemy import create_engine
-from requests.auth import HTTPBasicAuth
+from trino.auth import BasicAuthentication
 from decouple import config
 from sqlalchemy.sql.expression import text
 
 class EdatQueriyRunner:
 
     @staticmethod
     def unique_result(query:str, user: str):
@@ -17,18 +17,16 @@
     
     @staticmethod
     def __get_connection(user: str):
         engine = create_engine(
             f"trino://{config('TRINO_URL')}/{config('TRINO_CATALOG')}/{config('TRINO_SCHEMA')}",
             echo=False,
             connect_args={
-                "protocol": "https",
-                "requests_kwargs": {
-                    "auth": HTTPBasicAuth(config("TRINO_USERNAME"), config("TRINO_PASSWD"))
-                },
+                "http_scheme": "https",
+                "auth": BasicAuthentication(config("TRINO_USERNAME"), config("TRINO_PASSWD")),
                 "principal_username": user if user else config("TRINO_USERNAME"),
                 "session_props": {"query_max_run_time": "1234m"},
             },
         )
 
         connection = engine.connect()
-        return connection
+        return connection
```

### Comparing `edat_utils-0.3.4/edat_utils/schema.py` & `edat_utils-0.3.5/edat_utils/schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     parse_value=lambda v: v,
 )
 
 EdatGenericType = TypeVar("EdatGenericType")
 
 @strawberry.interface
 class EdatGrouped:
-    count: int
+    contador: int
 
 @strawberry.type
 class EdatPaginationWindow(List[EdatGenericType]):
     items: List[EdatGenericType] = strawberry.field(
         description="The list of items in this pagination window."
     )
```

### Comparing `edat_utils-0.3.4/edat_utils/utils.py` & `edat_utils-0.3.5/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.4/setup.py` & `edat_utils-0.3.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.3.4",
+    version="0.3.5",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

