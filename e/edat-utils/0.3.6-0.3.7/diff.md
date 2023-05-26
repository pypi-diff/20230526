# Comparing `tmp/edat_utils-0.3.6.tar.gz` & `tmp/edat_utils-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\edat_utils-0.3.6.tar", last modified: Thu May 25 23:55:05 2023, max compression
+gzip compressed data, was "dist\edat_utils-0.3.7.tar", last modified: Fri May 26 00:04:22 2023, max compression
```

## Comparing `edat_utils-0.3.6.tar` & `edat_utils-0.3.7.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 23:55:05.027782 edat_utils-0.3.6/
--rw-rw-rw-   0        0        0      555 2023-05-25 23:55:05.027782 edat_utils-0.3.6/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-25 23:37:25.000000 edat_utils-0.3.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 23:55:05.018256 edat_utils-0.3.6/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.3.6/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-05-25 23:37:25.000000 edat_utils-0.3.6/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.3.6/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1190 2023-05-25 23:54:23.000000 edat_utils-0.3.6/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.3.6/edat_utils/schema.py
--rw-rw-rw-   0        0        0      785 2023-05-25 23:37:25.000000 edat_utils-0.3.6/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-25 23:55:05.026222 edat_utils-0.3.6/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      555 2023-05-25 23:55:04.000000 edat_utils-0.3.6/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-25 23:55:04.000000 edat_utils-0.3.6/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 23:55:04.000000 edat_utils-0.3.6/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-25 23:55:04.000000 edat_utils-0.3.6/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-25 23:55:04.000000 edat_utils-0.3.6/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 23:55:05.029402 edat_utils-0.3.6/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-05-25 23:54:50.000000 edat_utils-0.3.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 00:04:22.792899 edat_utils-0.3.7/
+-rw-rw-rw-   0        0        0      555 2023-05-26 00:04:22.792899 edat_utils-0.3.7/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-25 23:37:25.000000 edat_utils-0.3.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 00:04:22.771864 edat_utils-0.3.7/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.3.7/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1043 2023-05-25 23:37:25.000000 edat_utils-0.3.7/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.3.7/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.3.7/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.3.7/edat_utils/schema.py
+-rw-rw-rw-   0        0        0      785 2023-05-25 23:37:25.000000 edat_utils-0.3.7/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 00:04:22.788833 edat_utils-0.3.7/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 00:04:22.795407 edat_utils-0.3.7/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-05-26 00:04:02.000000 edat_utils-0.3.7/setup.py
```

### Comparing `edat_utils-0.3.6/PKG-INFO` & `edat_utils-0.3.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat_utils
-Version: 0.3.6
+Version: 0.3.7
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT
         Classes utilitarias utilizadas pelo EDAT.
```

### Comparing `edat_utils-0.3.6/edat_utils/generic_controller.py` & `edat_utils-0.3.7/edat_utils/generic_controller.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.6/edat_utils/query_builder.py` & `edat_utils-0.3.7/edat_utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.6/edat_utils/query_runner.py` & `edat_utils-0.3.7/edat_utils/query_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,14 +19,13 @@
     def __get_connection(user: str):
         engine = create_engine(
             f"trino://{config('TRINO_URL')}/{config('TRINO_CATALOG')}/{config('TRINO_SCHEMA')}",
             echo=False,
             connect_args={
                 "http_scheme": "https",
                 "auth": BasicAuthentication(config("TRINO_USERNAME"), config("TRINO_PASSWD")),
-                "extra_credential": [('a.username', user if user else config("TRINO_USERNAME"))],
-                "session_props": {"query_max_run_time": "1234m"},
+                "extra_credential": [('a.username', user if user else config("TRINO_USERNAME"))]
             },
         )
 
         connection = engine.connect()
         return connection
```

### Comparing `edat_utils-0.3.6/edat_utils/schema.py` & `edat_utils-0.3.7/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.6/edat_utils/utils.py` & `edat_utils-0.3.7/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.6/edat_utils.egg-info/PKG-INFO` & `edat_utils-0.3.7/edat_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat-utils
-Version: 0.3.6
+Version: 0.3.7
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT
         Classes utilitarias utilizadas pelo EDAT.
```

### Comparing `edat_utils-0.3.6/setup.py` & `edat_utils-0.3.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.3.6",
+    version="0.3.7",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

