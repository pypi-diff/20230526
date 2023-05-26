# Comparing `tmp/edat_utils-0.3.7.tar.gz` & `tmp/edat_utils-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\edat_utils-0.3.7.tar", last modified: Fri May 26 00:04:22 2023, max compression
+gzip compressed data, was "dist\edat_utils-0.3.8.tar", last modified: Fri May 26 00:37:11 2023, max compression
```

## Comparing `edat_utils-0.3.7.tar` & `edat_utils-0.3.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 00:04:22.792899 edat_utils-0.3.7/
--rw-rw-rw-   0        0        0      555 2023-05-26 00:04:22.792899 edat_utils-0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0       63 2023-05-25 23:37:25.000000 edat_utils-0.3.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 00:04:22.771864 edat_utils-0.3.7/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.3.7/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1043 2023-05-25 23:37:25.000000 edat_utils-0.3.7/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.3.7/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.3.7/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.3.7/edat_utils/schema.py
--rw-rw-rw-   0        0        0      785 2023-05-25 23:37:25.000000 edat_utils-0.3.7/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 00:04:22.788833 edat_utils-0.3.7/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      555 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 00:04:22.000000 edat_utils-0.3.7/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 00:04:22.795407 edat_utils-0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     1114 2023-05-26 00:04:02.000000 edat_utils-0.3.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 00:37:11.742956 edat_utils-0.3.8/
+-rw-rw-rw-   0        0        0      555 2023-05-26 00:37:11.742956 edat_utils-0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0       63 2023-05-25 23:37:25.000000 edat_utils-0.3.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 00:37:11.727328 edat_utils-0.3.8/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.3.8/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1064 2023-05-26 00:36:21.000000 edat_utils-0.3.8/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3924 2023-05-25 23:37:25.000000 edat_utils-0.3.8/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.3.8/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.3.8/edat_utils/schema.py
+-rw-rw-rw-   0        0        0      785 2023-05-25 23:37:25.000000 edat_utils-0.3.8/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 00:37:11.727328 edat_utils-0.3.8/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      555 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 00:37:11.000000 edat_utils-0.3.8/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 00:37:11.742956 edat_utils-0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     1114 2023-05-26 00:36:31.000000 edat_utils-0.3.8/setup.py
```

### Comparing `edat_utils-0.3.7/PKG-INFO` & `edat_utils-0.3.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat_utils
-Version: 0.3.7
+Version: 0.3.8
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT
         Classes utilitarias utilizadas pelo EDAT.
```

### Comparing `edat_utils-0.3.7/edat_utils/generic_controller.py` & `edat_utils-0.3.8/edat_utils/generic_controller.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,11 +15,12 @@
         table = EdatUtils.get_table_name(info)
         grouped = True if isinstance(T, EdatGrouped) else False
         fields = EdatUtils.get_fields(info)
         user = EdatUtils.get_user(info)
         query = EdatQueryBuilder.build_query(table, filter, fields, pagination, orders, grouped)
         print(query)
         rows = EdatQueriyRunner.list(query, user)
+        print(rows)
         return EdatPaginationWindow(items=rows, total_items_count=len(rows))
```

### Comparing `edat_utils-0.3.7/edat_utils/query_builder.py` & `edat_utils-0.3.8/edat_utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.7/edat_utils/query_runner.py` & `edat_utils-0.3.8/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.7/edat_utils/schema.py` & `edat_utils-0.3.8/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.7/edat_utils/utils.py` & `edat_utils-0.3.8/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.3.7/edat_utils.egg-info/PKG-INFO` & `edat_utils-0.3.8/edat_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat-utils
-Version: 0.3.7
+Version: 0.3.8
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT
         Classes utilitarias utilizadas pelo EDAT.
```

### Comparing `edat_utils-0.3.7/setup.py` & `edat_utils-0.3.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.3.7",
+    version="0.3.8",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

