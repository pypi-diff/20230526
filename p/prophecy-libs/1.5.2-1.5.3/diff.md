# Comparing `tmp/prophecy-libs-1.5.2.tar.gz` & `tmp/prophecy-libs-1.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prophecy-libs-1.5.2.tar", last modified: Thu May 25 10:51:48 2023, max compression
+gzip compressed data, was "prophecy-libs-1.5.3.tar", last modified: Fri May 26 15:20:33 2023, max compression
```

## Comparing `prophecy-libs-1.5.2.tar` & `prophecy-libs-1.5.3.tar`

### file list

```diff
@@ -1,38 +1,45 @@
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.252760 prophecy-libs-1.5.2/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-25 10:51:48.252760 prophecy-libs-1.5.2/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/README.md
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.248759 prophecy-libs-1.5.2/prophecy/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/__init__.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.248759 prophecy-libs-1.5.2/prophecy/config/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/config/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/config/config_base.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     4346 2023-05-25 10:51:46.000000 prophecy-libs-1.5.2/prophecy/config/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.248759 prophecy-libs-1.5.2/prophecy/libs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/libs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      619 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/libs/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.248759 prophecy-libs-1.5.2/prophecy/lookups/
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/lookups/LookupsBase.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/lookups/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/random_data_creator.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.252760 prophecy-libs-1.5.2/prophecy/streaming/
--rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/streaming/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/streaming/delta_lake_utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.252760 prophecy-libs-1.5.2/prophecy/test/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/test/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.2/prophecy/test/base_test_case.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.2/prophecy/test/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.252760 prophecy-libs-1.5.2/prophecy/udfs/
--rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/udfs/__init__.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/udfs/rest_api_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/udfs/sample_udf.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)      985 2023-03-12 14:51:36.000000 prophecy-libs-1.5.2/prophecy/udfs/scala_udf_wrapper.py
--rw-r--r--   0 jenkins    (109) jenkins    (114)     8981 2023-04-12 12:00:52.000000 prophecy-libs-1.5.2/prophecy/utils.py
-drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-25 10:51:48.252760 prophecy-libs-1.5.2/prophecy_libs.egg-info/
--rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-25 10:51:48.000000 prophecy-libs-1.5.2/prophecy_libs.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (109) jenkins    (114)      773 2023-05-25 10:51:48.000000 prophecy-libs-1.5.2/prophecy_libs.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-05-25 10:51:48.000000 prophecy-libs-1.5.2/prophecy_libs.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.2/prophecy_libs.egg-info/not-zip-safe
--rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-05-25 10:51:48.000000 prophecy-libs-1.5.2/prophecy_libs.egg-info/requires.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-05-25 10:51:48.000000 prophecy-libs-1.5.2/prophecy_libs.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-05-25 10:51:48.252760 prophecy-libs-1.5.2/setup.cfg
--rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-05-25 10:51:46.000000 prophecy-libs-1.5.2/setup.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.710185 prophecy-libs-1.5.3/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       22 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/README.md
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/__init__.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/config/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/config/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2221 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/config/config_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     4346 2023-05-25 10:51:46.000000 prophecy-libs-1.5.3/prophecy/config/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/libs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       20 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/libs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1500 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/libs/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/lookups/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3191 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/lookups/LookupsBase.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       27 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/lookups/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     3118 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/random_data_creator.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.702184 prophecy-libs-1.5.3/prophecy/streaming/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        0 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/streaming/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     5283 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/streaming/delta_lake_utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/prophecy/test/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       30 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/test/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1165 2023-05-15 15:31:20.000000 prophecy-libs-1.5.3/prophecy/test/base_test_case.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     9189 2023-04-19 07:54:52.000000 prophecy-libs-1.5.3/prophecy/test/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/prophecy/transpiler/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      147 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      764 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/abi_base.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    22812 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/abi_core_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     1571 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/abi_fcn_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6432 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/dataframe_fcns.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     6368 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/transpiler/fixed_file_schema.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/prophecy/udfs/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       87 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/udfs/__init__.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)     2154 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/udfs/rest_api_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      172 2023-03-12 14:51:36.000000 prophecy-libs-1.5.3/prophecy/udfs/sample_udf.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      988 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/udfs/scala_udf_wrapper.py
+-rw-r--r--   0 jenkins    (109) jenkins    (114)    16532 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/prophecy/utils.py
+drwxr-xr-x   0 jenkins    (109) jenkins    (114)        0 2023-05-26 15:20:33.706184 prophecy-libs-1.5.3/prophecy_libs.egg-info/
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      313 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      992 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        1 2023-03-12 14:51:37.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       33 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)        9 2023-05-26 15:20:33.000000 prophecy-libs-1.5.3/prophecy_libs.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (109) jenkins    (114)       38 2023-05-26 15:20:33.710185 prophecy-libs-1.5.3/setup.cfg
+-rw-r--r--   0 jenkins    (109) jenkins    (114)      474 2023-05-26 15:20:32.000000 prophecy-libs-1.5.3/setup.py
```

### Comparing `prophecy-libs-1.5.2/prophecy/config/config_base.py` & `prophecy-libs-1.5.3/prophecy/config/config_base.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.2/prophecy/config/utils.py` & `prophecy-libs-1.5.3/prophecy/config/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.2/prophecy/lookups/LookupsBase.py` & `prophecy-libs-1.5.3/prophecy/lookups/LookupsBase.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.2/prophecy/random_data_creator.py` & `prophecy-libs-1.5.3/prophecy/random_data_creator.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.2/prophecy/streaming/delta_lake_utils.py` & `prophecy-libs-1.5.3/prophecy/streaming/delta_lake_utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.2/prophecy/test/base_test_case.py` & `prophecy-libs-1.5.3/prophecy/test/base_test_case.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.2/prophecy/test/utils.py` & `prophecy-libs-1.5.3/prophecy/test/utils.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.2/prophecy/udfs/rest_api_udf.py` & `prophecy-libs-1.5.3/prophecy/udfs/rest_api_udf.py`

 * *Files identical despite different names*

### Comparing `prophecy-libs-1.5.2/prophecy/udfs/scala_udf_wrapper.py` & `prophecy-libs-1.5.3/prophecy/udfs/scala_udf_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 from pyspark.sql.functions import udf
 from pyspark.sql.types import IntegerType
 from pyspark.sql.column import Column, _to_java_column, _to_seq
 
+
 class UDFBase:
     sparkSession = None
     UDFUtils = None
 
     def __init__(self, spark):
         self.UDFUtils = spark.sparkContext._jvm.io.prophecy.libs.python.UDFUtils
         self.sparkSession = spark
@@ -26,11 +27,12 @@
 def rest_api(*cols):
     _cols = udfConfig.sparkSession.sparkContext._jvm.PythonUtils.toList(
         [item._jc for item in list(cols)]
     )
     rest_api_response = udfConfig.UDFUtils.rest_api(_cols)
     return 1
 
+
 def call_udf(udfName: str, *cols):
     _cols = _to_seq(udfConfig.sparkSession.sparkContext, cols, _to_java_column)
     call_udf_result = udfConfig.UDFUtils.call_udf(udfName, _cols)
-    return Column(call_udf_result)
+    return Column(call_udf_result)
```

### Comparing `prophecy-libs-1.5.2/prophecy_libs.egg-info/SOURCES.txt` & `prophecy-libs-1.5.3/prophecy_libs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,14 +11,20 @@
 prophecy/lookups/LookupsBase.py
 prophecy/lookups/__init__.py
 prophecy/streaming/__init__.py
 prophecy/streaming/delta_lake_utils.py
 prophecy/test/__init__.py
 prophecy/test/base_test_case.py
 prophecy/test/utils.py
+prophecy/transpiler/__init__.py
+prophecy/transpiler/abi_base.py
+prophecy/transpiler/abi_core_fcns.py
+prophecy/transpiler/abi_fcn_wrapper.py
+prophecy/transpiler/dataframe_fcns.py
+prophecy/transpiler/fixed_file_schema.py
 prophecy/udfs/__init__.py
 prophecy/udfs/rest_api_udf.py
 prophecy/udfs/sample_udf.py
 prophecy/udfs/scala_udf_wrapper.py
 prophecy_libs.egg-info/PKG-INFO
 prophecy_libs.egg-info/SOURCES.txt
 prophecy_libs.egg-info/dependency_links.txt
```

