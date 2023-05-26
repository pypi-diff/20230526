# Comparing `tmp/edat_utils-0.4.0.tar.gz` & `tmp/edat_utils-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edat_utils-0.4.0.tar", last modified: Fri May 26 12:33:22 2023, max compression
+gzip compressed data, was "edat_utils-0.4.1.tar", last modified: Fri May 26 12:41:22 2023, max compression
```

## Comparing `edat_utils-0.4.0.tar` & `edat_utils-0.4.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:33:22.738179 edat_utils-0.4.0/
--rw-rw-rw-   0        0        0      491 2023-05-26 12:33:22.737178 edat_utils-0.4.0/PKG-INFO
--rw-rw-rw-   0        0        0      217 2023-05-26 12:02:26.000000 edat_utils-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 12:33:22.725176 edat_utils-0.4.0/edat_utils/
--rw-rw-rw-   0        0        0        0 2023-04-12 14:43:25.000000 edat_utils-0.4.0/edat_utils/__init__.py
--rw-rw-rw-   0        0        0     1228 2023-05-26 12:31:56.000000 edat_utils-0.4.0/edat_utils/generic_controller.py
--rw-rw-rw-   0        0        0     3924 2023-04-13 18:06:40.000000 edat_utils-0.4.0/edat_utils/query_builder.py
--rw-rw-rw-   0        0        0     1122 2023-05-26 11:50:02.000000 edat_utils-0.4.0/edat_utils/query_runner.py
--rw-rw-rw-   0        0        0      987 2023-05-26 12:30:34.000000 edat_utils-0.4.0/edat_utils/schema.py
--rw-rw-rw-   0        0        0      785 2023-04-13 20:03:38.000000 edat_utils-0.4.0/edat_utils/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:33:22.736232 edat_utils-0.4.0/edat_utils.egg-info/
--rw-rw-rw-   0        0        0      491 2023-05-26 12:33:22.000000 edat_utils-0.4.0/edat_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-05-26 12:33:22.000000 edat_utils-0.4.0/edat_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:33:22.000000 edat_utils-0.4.0/edat_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-26 12:33:22.000000 edat_utils-0.4.0/edat_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-26 12:33:22.000000 edat_utils-0.4.0/edat_utils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 12:33:22.738179 edat_utils-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0      855 2023-05-26 12:32:08.000000 edat_utils-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:41:22.143034 edat_utils-0.4.1/
+-rw-rw-rw-   0        0        0      491 2023-05-26 12:41:22.143034 edat_utils-0.4.1/PKG-INFO
+-rw-rw-rw-   0        0        0      217 2023-05-26 12:02:26.000000 edat_utils-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 12:41:22.128045 edat_utils-0.4.1/edat_utils/
+-rw-rw-rw-   0        0        0        0 2023-04-12 14:43:25.000000 edat_utils-0.4.1/edat_utils/__init__.py
+-rw-rw-rw-   0        0        0     1240 2023-05-26 12:40:01.000000 edat_utils-0.4.1/edat_utils/generic_controller.py
+-rw-rw-rw-   0        0        0     3924 2023-04-13 18:06:40.000000 edat_utils-0.4.1/edat_utils/query_builder.py
+-rw-rw-rw-   0        0        0     1122 2023-05-26 11:50:02.000000 edat_utils-0.4.1/edat_utils/query_runner.py
+-rw-rw-rw-   0        0        0      970 2023-05-26 12:40:17.000000 edat_utils-0.4.1/edat_utils/schema.py
+-rw-rw-rw-   0        0        0      785 2023-04-13 20:03:38.000000 edat_utils-0.4.1/edat_utils/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:41:22.141034 edat_utils-0.4.1/edat_utils.egg-info/
+-rw-rw-rw-   0        0        0      491 2023-05-26 12:41:22.000000 edat_utils-0.4.1/edat_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-05-26 12:41:22.000000 edat_utils-0.4.1/edat_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:41:22.000000 edat_utils-0.4.1/edat_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-26 12:41:22.000000 edat_utils-0.4.1/edat_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-26 12:41:22.000000 edat_utils-0.4.1/edat_utils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 12:41:22.143034 edat_utils-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0      855 2023-05-26 12:40:40.000000 edat_utils-0.4.1/setup.py
```

### Comparing `edat_utils-0.4.0/edat_utils/generic_controller.py` & `edat_utils-0.4.1/edat_utils/generic_controller.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Any, Generic, TypeVar, Type
 from strawberry.types import Info
 from edat_utils.utils import EdatUtils
 from edat_utils.query_builder import EdatQueryBuilder
 from edat_utils.query_runner import EdatQueriyRunner
-from edat_utils.schema import EdatGenericType, EdatPagination, EdatOrder, EdatPaginationWindow, EdatGrouped
+from edat_utils.schema import EdatFilter, EdatGenericType, EdatPagination, EdatOrder, EdatPaginationWindow, EdatGrouped
 from typing import List
 
 T = TypeVar("T")
 
 
 class GenericController(Generic[T]):
```

### Comparing `edat_utils-0.4.0/edat_utils/query_builder.py` & `edat_utils-0.4.1/edat_utils/query_builder.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.0/edat_utils/query_runner.py` & `edat_utils-0.4.1/edat_utils/query_runner.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.0/edat_utils/schema.py` & `edat_utils-0.4.1/edat_utils/schema.py`

 * *Files 27% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     serialize=lambda v: v,
     parse_value=lambda v: v,
 )
 
 EdatGenericType = TypeVar("EdatGenericType")
 
 @strawberry.interface
-class EdatGrouped(EdatGenericType):
+class EdatGrouped:
     contador: int
 
 @strawberry.type
 class EdatPaginationWindow(List[EdatGenericType]):
     items: List[EdatGenericType] = strawberry.field(
         description="The list of items in this pagination window."
     )
```

### Comparing `edat_utils-0.4.0/edat_utils/utils.py` & `edat_utils-0.4.1/edat_utils/utils.py`

 * *Files identical despite different names*

### Comparing `edat_utils-0.4.0/setup.py` & `edat_utils-0.4.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
 
 # This call to setup() does all the work
 setup(
     name="edat_utils",
-    version="0.4.0",
+    version="0.4.1",
     description="Biblioteca de Apoio ao desenvolvimento no EDAT",
     long_description="# Utilitarios EDAT <br /> Classes utilitarias utilizadas pelo EDAT.",
     long_description_content_type="text/markdown",
     author="Escritório de Dados",
     author_email="dados@unicamp.br",
     license="MIT",
     classifiers=[
```

