# Comparing `tmp/edat_utils-0.5.1.tar.gz` & `tmp/edat_utils-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\edat_utils-0.5.1.tar", last modified: Fri May 26 20:46:35 2023, max compression
+gzip compressed data, was "dist\edat_utils-0.5.2.tar", last modified: Fri May 26 20:54:54 2023, max compression
```

## Comparing `edat_utils-0.5.1.tar` & `edat_utils-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 20:46:35.584660 edat_utils-0.5.1/
--rw-rw-rw-   0        0        0      541 2023-05-26 20:46:35.584660 edat_utils-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 20:46:35.571215 edat_utils-0.5.1/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.5.1/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-05-26 18:20:57.000000 edat_utils-0.5.1/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     4332 2023-05-26 20:45:29.000000 edat_utils-0.5.1/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.5.1/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.5.1/edat_utils/schema.py
--rw-rw-rw-   0        0        0     1597 2023-05-26 18:20:17.000000 edat_utils-0.5.1/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 20:46:35.582175 edat_utils-0.5.1/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      541 2023-05-26 20:46:35.000000 edat_utils-0.5.1/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-26 20:46:35.000000 edat_utils-0.5.1/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 20:46:35.000000 edat_utils-0.5.1/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 20:46:35.000000 edat_utils-0.5.1/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 20:46:35.000000 edat_utils-0.5.1/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 20:46:35.586717 edat_utils-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-26 20:46:17.000000 edat_utils-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:54:54.594224 edat_utils-0.5.2/
+-rw-rw-rw-   0        0        0      541 2023-05-26 20:54:54.593711 edat_utils-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 20:54:54.582490 edat_utils-0.5.2/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.5.2/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-05-26 18:20:57.000000 edat_utils-0.5.2/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     4422 2023-05-26 20:54:16.000000 edat_utils-0.5.2/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.5.2/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.5.2/edat_utils/schema.py
+-rw-rw-rw-   0        0        0     1597 2023-05-26 18:20:17.000000 edat_utils-0.5.2/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:54:54.587574 edat_utils-0.5.2/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-05-26 20:54:54.000000 edat_utils-0.5.2/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 20:54:54.000000 edat_utils-0.5.2/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 20:54:54.000000 edat_utils-0.5.2/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 20:54:54.000000 edat_utils-0.5.2/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 20:54:54.000000 edat_utils-0.5.2/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 20:54:54.594224 edat_utils-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-26 20:54:24.000000 edat_utils-0.5.2/setup.py
```

### Comparing `edat_utils-0.5.1/PKG-INFO` & `edat_utils-0.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat_utils
-Version: 0.5.1
+Version: 0.5.2
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.5.1/edat_utils/generic_controller.py` & `edat_utils-0.5.2/edat_utils/generic_controller.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.5.1/edat_utils/query_builder.py` & `edat_utils-0.5.2/edat_utils/query_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,20 +93,22 @@
             query = query + ' ORDER BY ' + COMMA_SEPARARATOR.join(orderBy)
         query = query + pagination_text
        
         return query
 
     @staticmethod
     def __get_value(value):
+        date_pattern_str = r'^\d{4}-\d{2}-\d{2}$'
         if isinstance(value, numbers.Number):
             return str(value)
-        elif isinstance(value, date):
-            return "date '" + value + "'"
         elif isinstance(value, str):
-            return "'" + value + "'"
+            if re.match(date_pattern_str, value):
+                return "date '" + value + "'"
+            else:
+                return "'" + value + "'"
         elif isinstance(value, list) or isinstance(value, dict):
             if isinstance(value[0], str):
                 return "('" + "', '".join(value) + "')"
             else:
                 return "(" + ", ".join(map(str, value)) + ")"
         else: 
             return value
```

### Comparing `edat_utils-0.5.1/edat_utils/query_runner.py` & `edat_utils-0.5.2/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.5.1/edat_utils/schema.py` & `edat_utils-0.5.2/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.5.1/edat_utils/utils.py` & `edat_utils-0.5.2/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.5.1/edat_utils.egg-info/PKG-INFO` & `edat_utils-0.5.2/edat_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat-utils
-Version: 0.5.1
+Version: 0.5.2
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.5.1/setup.py` & `edat_utils-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.5.1",
+    version="0.5.2",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description="# Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.",
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

