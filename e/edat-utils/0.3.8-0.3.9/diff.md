# Comparing `tmp/edat_utils-0.3.8.tar.gz` & `tmp/edat_utils-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\edat_utils-0.3.8.tar", last modified: Fri May 26 00:37:11 2023, max compression
+gzip compressed data, was "edat_utils-0.3.9.tar", last modified: Fri May 26 12:03:12 2023, max compression
```

## Comparing `edat_utils-0.3.8.tar` & `edat_utils-0.3.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 00:37:11.742956 edat_utils-0.3.8/
--rw-rw-rw-   0        0        0      555 2023-05-26 00:37:11.742956 edat_utils-0.3.8/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-25 23:37:25.000000 edat_utils-0.3.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 00:37:11.727328 edat_utils-0.3.8/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.3.8/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1064 2023-05-26 00:36:21.000000 edat_utils-0.3.8/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.3.8/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.3.8/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.3.8/edat_utils/schema.py
--rw-rw-rw-   0        0        0      785 2023-05-25 23:37:25.000000 edat_utils-0.3.8/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 00:37:11.727328 edat_utils-0.3.8/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      555 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 00:37:11.742956 edat_utils-0.3.8/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-05-26 00:36:31.000000 edat_utils-0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:03:12.857412 edat_utils-0.3.9/
+-rw-rw-rw-   0        0        0      491 2023-05-26 12:03:12.857412 edat_utils-0.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-26 12:02:26.000000 edat_utils-0.3.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 12:03:12.847056 edat_utils-0.3.9/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 14:43:25.000000 edat_utils-0.3.9/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1142 2023-05-26 11:59:09.000000 edat_utils-0.3.9/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3924 2023-04-13 18:06:40.000000 edat_utils-0.3.9/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 11:50:02.000000 edat_utils-0.3.9/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-26 11:50:02.000000 edat_utils-0.3.9/edat_utils/schema.py
+-rw-rw-rw-   0        0        0      785 2023-04-13 20:03:38.000000 edat_utils-0.3.9/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:03:12.855265 edat_utils-0.3.9/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-05-26 12:03:12.000000 edat_utils-0.3.9/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 12:03:12.000000 edat_utils-0.3.9/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:03:12.000000 edat_utils-0.3.9/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 12:03:12.000000 edat_utils-0.3.9/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 12:03:12.000000 edat_utils-0.3.9/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 12:03:12.857412 edat_utils-0.3.9/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-26 11:59:21.000000 edat_utils-0.3.9/setup.py
```

### Comparing `edat_utils-0.3.8/edat_utils/generic_controller.py` & `edat_utils-0.3.9/edat_utils/generic_controller.py`

 * *Files 20% similar despite different names*

```diff
@@ -15,12 +15,14 @@
         table = EdatUtils.get_table_name(info)
         grouped = True if isinstance(T, EdatGrouped) else False
         fields = EdatUtils.get_fields(info)
         user = EdatUtils.get_user(info)
         query = EdatQueryBuilder.build_query(table, filter, fields, pagination, orders, grouped)
         print(query)
         rows = EdatQueriyRunner.list(query, user)
-        print(rows)
+        print(rows[1]._asdict())
+        print(rows[1]._fields)
+        print(rows[1]._mapping)
         return EdatPaginationWindow(items=rows, total_items_count=len(rows))
```

### Comparing `edat_utils-0.3.8/edat_utils/query_builder.py` & `edat_utils-0.3.9/edat_utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.8/edat_utils/query_runner.py` & `edat_utils-0.3.9/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.8/edat_utils/schema.py` & `edat_utils-0.3.9/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.8/edat_utils/utils.py` & `edat_utils-0.3.9/edat_utils/utils.py`

 * *Files identical despite different names*

