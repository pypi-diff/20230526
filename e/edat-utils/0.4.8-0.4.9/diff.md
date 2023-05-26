# Comparing `tmp/edat_utils-0.4.8.tar.gz` & `tmp/edat_utils-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\edat_utils-0.4.8.tar", last modified: Fri May 26 19:15:01 2023, max compression
+gzip compressed data, was "dist\edat_utils-0.4.9.tar", last modified: Fri May 26 19:26:03 2023, max compression
```

## Comparing `edat_utils-0.4.8.tar` & `edat_utils-0.4.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 19:15:01.577710 edat_utils-0.4.8/
--rw-rw-rw-   0        0        0      541 2023-05-26 19:15:01.577710 edat_utils-0.4.8/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.4.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 19:15:01.562195 edat_utils-0.4.8/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.4.8/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1100 2023-05-26 18:20:57.000000 edat_utils-0.4.8/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     4069 2023-05-26 19:09:12.000000 edat_utils-0.4.8/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.4.8/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.4.8/edat_utils/schema.py
--rw-rw-rw-   0        0        0     1597 2023-05-26 18:20:17.000000 edat_utils-0.4.8/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:15:01.574567 edat_utils-0.4.8/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      541 2023-05-26 19:15:01.000000 edat_utils-0.4.8/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-26 19:15:01.000000 edat_utils-0.4.8/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 19:15:01.000000 edat_utils-0.4.8/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 19:15:01.000000 edat_utils-0.4.8/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 19:15:01.000000 edat_utils-0.4.8/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 19:15:01.579719 edat_utils-0.4.8/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-26 19:09:21.000000 edat_utils-0.4.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:26:03.018925 edat_utils-0.4.9/
+-rw-rw-rw-   0        0        0      541 2023-05-26 19:26:03.017897 edat_utils-0.4.9/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-26 17:57:10.000000 edat_utils-0.4.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 19:26:03.003493 edat_utils-0.4.9/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 17:41:48.000000 edat_utils-0.4.9/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1100 2023-05-26 18:20:57.000000 edat_utils-0.4.9/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     4211 2023-05-26 19:25:17.000000 edat_utils-0.4.9/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 00:03:39.000000 edat_utils-0.4.9/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-25 23:41:19.000000 edat_utils-0.4.9/edat_utils/schema.py
+-rw-rw-rw-   0        0        0     1597 2023-05-26 18:20:17.000000 edat_utils-0.4.9/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 19:26:03.015238 edat_utils-0.4.9/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      541 2023-05-26 19:26:02.000000 edat_utils-0.4.9/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 19:26:02.000000 edat_utils-0.4.9/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 19:26:02.000000 edat_utils-0.4.9/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 19:26:02.000000 edat_utils-0.4.9/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 19:26:02.000000 edat_utils-0.4.9/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 19:26:03.020960 edat_utils-0.4.9/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-26 19:25:40.000000 edat_utils-0.4.9/setup.py
```

### Comparing `edat_utils-0.4.8/PKG-INFO` & `edat_utils-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat_utils
-Version: 0.4.8
+Version: 0.4.9
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.4.8/edat_utils/generic_controller.py` & `edat_utils-0.4.9/edat_utils/generic_controller.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.8/edat_utils/query_builder.py` & `edat_utils-0.4.9/edat_utils/query_builder.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,20 +50,24 @@
                         where.append(key_dict + ' = ' + value_dict)
             else:
                 where.append(key + ' = ' + str(value))
 
         if grouped:
             select.append("SUM(contador)")
             for field in fields:
+                if field == 'contador':
+                    continue
                 underline_field = re.sub(
                     r'(?<!^)(?=[A-Z])', '_', field).lower()
                 select.append(underline_field)
                 group.append(underline_field)
         else:
             for field in fields:
+                if field == 'contador':
+                    continue
                 underline_field = re.sub(
                     r'(?<!^)(?=[A-Z])', '_', field).lower()
                 select.append(underline_field)
 
         if pagination:
             if pagination.limit and pagination.limit != 0:
                 pagination_text = pagination_text + ' LIMIT ' + str(pagination.limit)
```

### Comparing `edat_utils-0.4.8/edat_utils/query_runner.py` & `edat_utils-0.4.9/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.8/edat_utils/schema.py` & `edat_utils-0.4.9/edat_utils/schema.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.8/edat_utils/utils.py` & `edat_utils-0.4.9/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.8/edat_utils.egg-info/PKG-INFO` & `edat_utils-0.4.9/edat_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edat-utils
-Version: 0.4.8
+Version: 0.4.9
 Summary: Biblioteca de Apoio ao desenvolvimento no EDAT
 Home-page: UNKNOWN
 Author: Escritório de Dados
 Author-email: dados@unicamp.br
 License: MIT
 Description: # Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.
 Platform: UNKNOWN
```

### Comparing `edat_utils-0.4.8/setup.py` & `edat_utils-0.4.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.4.8",
+    version="0.4.9",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description="# Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.",
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

