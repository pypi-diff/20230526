# Comparing `tmp/edat_utils-0.4.3.tar.gz` & `tmp/edat_utils-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\edat_utils-0.4.3.tar", last modified: Fri May 26 18:02:15 2023, max compression
+gzip compressed data, was "dist\edat_utils-0.4.4.tar", last modified: Fri May 26 18:14:07 2023, max compression
```

## Comparing `edat_utils-0.4.3.tar` & `edat_utils-0.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 18:02:15.222459 edat_utils-0.4.3/
--rw-rw-rw-   0        0        0      541 2023-05-26 18:02:15.222459 edat_utils-0.4.3/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.4.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 18:02:15.210487 edat_utils-0.4.3/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.4.3/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1119 2023-05-26 18:01:06.000000 edat_utils-0.4.3/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.4.3/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.4.3/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.4.3/edat_utils/schema.py
--rw-rw-rw-   0        0        0     1372 2023-05-26 18:00:05.000000 edat_utils-0.4.3/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:02:15.220408 edat_utils-0.4.3/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      541 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 18:02:15.224576 edat_utils-0.4.3/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-26 18:01:34.000000 edat_utils-0.4.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:14:07.858133 edat_utils-0.4.4/
+-rw-rw-rw-   0        0        0      541 2023-05-26 18:14:07.858133 edat_utils-0.4.4/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.4.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 18:14:07.848148 edat_utils-0.4.4/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.4.4/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-05-26 18:13:21.000000 edat_utils-0.4.4/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.4.4/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.4.4/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.4.4/edat_utils/schema.py
+-rw-rw-rw-   0        0        0     1372 2023-05-26 18:00:05.000000 edat_utils-0.4.4/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:14:07.858133 edat_utils-0.4.4/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-05-26 18:14:07.000000 edat_utils-0.4.4/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 18:14:07.000000 edat_utils-0.4.4/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 18:14:07.000000 edat_utils-0.4.4/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 18:14:07.000000 edat_utils-0.4.4/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 18:14:07.000000 edat_utils-0.4.4/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 18:14:07.858133 edat_utils-0.4.4/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-26 18:13:31.000000 edat_utils-0.4.4/setup.py
```

### Comparing `edat_utils-0.4.3/PKG-INFO` & `edat_utils-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat_utils
-Version: 0.4.3
+Version: 0.4.4
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.4.3/edat_utils/generic_controller.py` & `edat_utils-0.4.4/edat_utils/generic_controller.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 T = TypeVar("T")
 
 
 class GenericController(Generic[T]):
 
     def get(self, info:Info, filter: EdatFilter, pagination: EdatPagination = None, orders: List[EdatOrder] = None) -> EdatPaginationWindow[T]:             
         table = EdatUtils.get_table_name(info)
-        grouped = True if isinstance(T, EdatGrouped) else False
+        grouped = True if issubclass(T, EdatGrouped) else False
         fields = EdatUtils.get_fields(info)
         user = EdatUtils.get_user(info)
         query = EdatQueryBuilder.build_query(table, filter, fields, pagination, orders, grouped)
         print(query)
         rows = EdatQueriyRunner.list(query, user)
         obj_list = EdatUtils.get_list(info, rows)
         return EdatPaginationWindow(items=obj_list, total_items_count=len(obj_list))
```

### Comparing `edat_utils-0.4.3/edat_utils/query_builder.py` & `edat_utils-0.4.4/edat_utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.3/edat_utils/query_runner.py` & `edat_utils-0.4.4/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.3/edat_utils/schema.py` & `edat_utils-0.4.4/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.3/edat_utils/utils.py` & `edat_utils-0.4.4/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.3/edat_utils.egg-info/PKG-INFO` & `edat_utils-0.4.4/edat_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat-utils
-Version: 0.4.3
+Version: 0.4.4
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.4.3/setup.py` & `edat_utils-0.4.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.4.3",
+    version="0.4.4",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description="# Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.",
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

