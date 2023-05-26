# Comparing `tmp/edat_utils-0.4.2.tar.gz` & `tmp/edat_utils-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edat_utils-0.4.2.tar", last modified: Fri May 26 12:59:05 2023, max compression
+gzip compressed data, was "dist\edat_utils-0.4.3.tar", last modified: Fri May 26 18:02:15 2023, max compression
```

## Comparing `edat_utils-0.4.2.tar` & `edat_utils-0.4.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:59:05.077001 edat_utils-0.4.2/
--rw-rw-rw-   0        0        0      491 2023-05-26 12:59:05.076002 edat_utils-0.4.2/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-26 12:02:26.000000 edat_utils-0.4.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 12:59:05.064365 edat_utils-0.4.2/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 14:43:25.000000 edat_utils-0.4.2/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-05-26 12:54:51.000000 edat_utils-0.4.2/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-04-13 18:06:40.000000 edat_utils-0.4.2/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-05-26 11:50:02.000000 edat_utils-0.4.2/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-05-26 12:40:17.000000 edat_utils-0.4.2/edat_utils/schema.py
--rw-rw-rw-   0        0        0      785 2023-04-13 20:03:38.000000 edat_utils-0.4.2/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:59:05.075000 edat_utils-0.4.2/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      491 2023-05-26 12:59:04.000000 edat_utils-0.4.2/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-26 12:59:04.000000 edat_utils-0.4.2/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:59:04.000000 edat_utils-0.4.2/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 12:59:04.000000 edat_utils-0.4.2/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 12:59:04.000000 edat_utils-0.4.2/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 12:59:05.077001 edat_utils-0.4.2/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-26 12:55:12.000000 edat_utils-0.4.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:02:15.222459 edat_utils-0.4.3/
+-rw-rw-rw-   0        0        0      541 2023-05-26 18:02:15.222459 edat_utils-0.4.3/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.4.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 18:02:15.210487 edat_utils-0.4.3/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.4.3/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1119 2023-05-26 18:01:06.000000 edat_utils-0.4.3/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.4.3/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.4.3/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.4.3/edat_utils/schema.py
+-rw-rw-rw-   0        0        0     1372 2023-05-26 18:00:05.000000 edat_utils-0.4.3/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 18:02:15.220408 edat_utils-0.4.3/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 18:02:15.000000 edat_utils-0.4.3/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 18:02:15.224576 edat_utils-0.4.3/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-26 18:01:34.000000 edat_utils-0.4.3/setup.py
```

### Comparing `edat_utils-0.4.2/edat_utils/generic_controller.py` & `edat_utils-0.4.3/edat_utils/generic_controller.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,17 +15,12 @@
         table = EdatUtils.get_table_name(info)
         grouped = True if isinstance(T, EdatGrouped) else False
         fields = EdatUtils.get_fields(info)
         user = EdatUtils.get_user(info)
         query = EdatQueryBuilder.build_query(table, filter, fields, pagination, orders, grouped)
         print(query)
         rows = EdatQueriyRunner.list(query, user)
-        print(rows[1]._asdict())
-        print(rows[1]._fields)
-        print(rows[1]._mapping)
-        t = self.__orig_class__.__args__[0]()
-        t.__dict__.update(rows[1]._asdict())
-        print(t)
-        return EdatPaginationWindow(items=rows, total_items_count=len(rows))
+        obj_list = EdatUtils.get_list(info, rows)
+        return EdatPaginationWindow(items=obj_list, total_items_count=len(obj_list))
```

### Comparing `edat_utils-0.4.2/edat_utils/query_builder.py` & `edat_utils-0.4.3/edat_utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.2/edat_utils/query_runner.py` & `edat_utils-0.4.3/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.2/edat_utils/schema.py` & `edat_utils-0.4.3/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.2/setup.py` & `edat_utils-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.4.2",
+    version="0.4.3",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description="# Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.",
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

