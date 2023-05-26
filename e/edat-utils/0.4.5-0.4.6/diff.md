# Comparing `tmp/edat_utils-0.4.5.tar.gz` & `tmp/edat_utils-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\edat_utils-0.4.5.tar", last modified: Fri May 26 18:21:32 2023, max compression
+gzip compressed data, was "dist\edat_utils-0.4.6.tar", last modified: Fri May 26 18:47:52 2023, max compression
```

## Comparing `edat_utils-0.4.5.tar` & `edat_utils-0.4.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 18:21:32.609080 edat_utils-0.4.5/
--rw-rw-rw-   0        0        0      541 2023-05-26 18:21:32.609080 edat_utils-0.4.5/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.4.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 18:21:32.567786 edat_utils-0.4.5/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.4.5/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-05-26 18:20:57.000000 edat_utils-0.4.5/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.4.5/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.4.5/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.4.5/edat_utils/schema.py
--rw-rw-rw-   0        0        0     1597 2023-05-26 18:20:17.000000 edat_utils-0.4.5/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 18:21:32.605490 edat_utils-0.4.5/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      541 2023-05-26 18:21:32.000000 edat_utils-0.4.5/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-26 18:21:32.000000 edat_utils-0.4.5/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 18:21:32.000000 edat_utils-0.4.5/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 18:21:32.000000 edat_utils-0.4.5/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 18:21:32.000000 edat_utils-0.4.5/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 18:21:32.610092 edat_utils-0.4.5/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-26 18:20:38.000000 edat_utils-0.4.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:47:52.258560 edat_utils-0.4.6/
+-rw-rw-rw-   0        0        0      541 2023-05-26 18:47:52.258560 edat_utils-0.4.6/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.4.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 18:47:52.245057 edat_utils-0.4.6/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.4.6/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-05-26 18:20:57.000000 edat_utils-0.4.6/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3955 2023-05-26 18:43:34.000000 edat_utils-0.4.6/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.4.6/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.4.6/edat_utils/schema.py
+-rw-rw-rw-   0        0        0     1597 2023-05-26 18:20:17.000000 edat_utils-0.4.6/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:47:52.257293 edat_utils-0.4.6/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-05-26 18:47:52.000000 edat_utils-0.4.6/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 18:47:52.000000 edat_utils-0.4.6/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 18:47:52.000000 edat_utils-0.4.6/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 18:47:52.000000 edat_utils-0.4.6/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 18:47:52.000000 edat_utils-0.4.6/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 18:47:52.261904 edat_utils-0.4.6/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-26 18:44:00.000000 edat_utils-0.4.6/setup.py
```

### Comparing `edat_utils-0.4.5/PKG-INFO` & `edat_utils-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat_utils
-Version: 0.4.5
+Version: 0.4.6
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.4.5/edat_utils/generic_controller.py` & `edat_utils-0.4.6/edat_utils/generic_controller.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.5/edat_utils/query_builder.py` & `edat_utils-0.4.6/edat_utils/query_builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
     @staticmethod
     def build_query(table: str, filter: EdatFilter, fields: List[str], pagination: EdatPagination, orders: List[EdatOrder], grouped: bool):
         
         select = []
         where = []
         group = []
-        pagination = ''
+        pagination_text = ''
         orderBy = []
 
         for key in filter:
             value = filter[key]
             if isinstance(value, dict):
                 key_dict = list(value.keys())[0]
                 value_dict = EdatQueryBuilder.__get_value(value[key_dict])
@@ -62,17 +62,17 @@
             for field in fields:
                 underline_field = re.sub(
                     r'(?<!^)(?=[A-Z])', '_', field).lower()
                 select.append(underline_field)
 
         if pagination:
             if pagination.limit and pagination.limit != 0:
-                pagination = pagination + ' LIMIT ' + str(pagination.limit)
-            if pagination.limit and pagination.offset != 0:
-                pagination = pagination + ' OFFSET ' + str(pagination.offset)
+                pagination_text = pagination_text + ' LIMIT ' + str(pagination.limit)
+            if pagination.offset and pagination.offset != 0:
+                pagination_text = pagination_text + ' OFFSET ' + str(pagination.offset)
 
         if orders:
             for order in orders:
                 orderBy.append(order.field + ' ' + order.type.value)
 
 
         query = 'SELECT '
@@ -80,15 +80,15 @@
         query = query + ' FROM ' + table
         if where:
             query = query + ' WHERE '+ AND.join(where)
         if group:
             query = query + ' GROUP BY '+ COMMA_SEPARARATOR.join(group)
         if orderBy:
             query = query + ' ORDER BY ' + COMMA_SEPARARATOR.join(orderBy)
-        query = query + pagination
+        query = query + pagination_text
        
         return query
 
     @staticmethod
     def __get_value(value):
         if isinstance(value, numbers.Number):
             return str(value)
```

### Comparing `edat_utils-0.4.5/edat_utils/query_runner.py` & `edat_utils-0.4.6/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.5/edat_utils/schema.py` & `edat_utils-0.4.6/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.5/edat_utils/utils.py` & `edat_utils-0.4.6/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.5/edat_utils.egg-info/PKG-INFO` & `edat_utils-0.4.6/edat_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat-utils
-Version: 0.4.5
+Version: 0.4.6
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.4.5/setup.py` & `edat_utils-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.4.5",
+    version="0.4.6",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description="# Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.",
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

