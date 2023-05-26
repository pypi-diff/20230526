# Comparing `tmp/syncanysql-0.1.3.tar.gz` & `tmp/syncanysql-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syncanysql-0.1.3.tar", last modified: Fri May 12 09:49:37 2023, max compression
+gzip compressed data, was "syncanysql-0.1.4.tar", last modified: Fri May 26 10:44:08 2023, max compression
```

## Comparing `syncanysql-0.1.3.tar` & `syncanysql-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,45 @@
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:37.662877 syncanysql-0.1.3/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-12 09:49:37.664874 syncanysql-0.1.3/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.3/README.md
--rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-12 09:49:37.672875 syncanysql-0.1.3/setup.cfg
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2002 2023-05-08 07:06:40.000000 syncanysql-0.1.3/setup.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:36.232618 syncanysql-0.1.3/syncanysql/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.3/syncanysql/__init__.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:36.723836 syncanysql-0.1.3/syncanysql/calculaters/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1130 2023-04-23 06:35:38.000000 syncanysql-0.1.3/syncanysql/calculaters/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6152 2023-03-25 11:43:14.000000 syncanysql-0.1.3/syncanysql/calculaters/aggregate_calculater.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_calculater.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:37.095112 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/
--rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-03-14 09:33:57.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    10197 2023-05-04 10:22:31.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/json_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/number_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/string_funcs.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)   135990 2023-05-04 10:48:36.000000 syncanysql-0.1.3/syncanysql/compiler.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    12804 2023-05-08 04:32:02.000000 syncanysql-0.1.3/syncanysql/config.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.3/syncanysql/errors.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     8446 2023-05-08 04:35:48.000000 syncanysql-0.1.3/syncanysql/executor.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.3/syncanysql/main.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.3/syncanysql/parser.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.3/syncanysql/prompt.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:37.619874 syncanysql-0.1.3/syncanysql/taskers/
--rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.3/syncanysql/taskers/__init__.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.3/syncanysql/taskers/delete.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.3/syncanysql/taskers/execute.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.3/syncanysql/taskers/explain.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.3/syncanysql/taskers/into.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)    21231 2023-05-04 02:54:58.000000 syncanysql-0.1.3/syncanysql/taskers/query.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2890 2023-05-08 04:04:28.000000 syncanysql-0.1.3/syncanysql/taskers/set.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.3/syncanysql/taskers/show.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.3/syncanysql/taskers/use.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      754 2023-05-08 04:04:28.000000 syncanysql-0.1.3/syncanysql/utils.py
--rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-05-04 02:34:02.000000 syncanysql-0.1.3/syncanysql/version.py
-drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-12 09:49:36.542839 syncanysql-0.1.3/syncanysql.egg-info/
--rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-12 09:49:34.000000 syncanysql-0.1.3/syncanysql.egg-info/PKG-INFO
--rwxrwxrwx   0 snower    (1000) snower    (1000)     1111 2023-05-12 09:49:35.000000 syncanysql-0.1.3/syncanysql.egg-info/SOURCES.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-12 09:49:34.000000 syncanysql-0.1.3/syncanysql.egg-info/dependency_links.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-05-12 09:49:35.000000 syncanysql-0.1.3/syncanysql.egg-info/entry_points.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.3/syncanysql.egg-info/not-zip-safe
--rwxrwxrwx   0 snower    (1000) snower    (1000)      390 2023-05-12 09:49:35.000000 syncanysql-0.1.3/syncanysql.egg-info/requires.txt
--rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-05-12 09:49:35.000000 syncanysql-0.1.3/syncanysql.egg-info/top_level.txt
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:08.178205 syncanysql-0.1.4/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-26 10:44:08.179206 syncanysql-0.1.4/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3018 2023-04-25 10:14:55.000000 syncanysql-0.1.4/README.md
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       67 2023-05-26 10:44:08.189200 syncanysql-0.1.4/setup.cfg
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2006 2023-05-26 07:22:02.000000 syncanysql-0.1.4/setup.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:06.626398 syncanysql-0.1.4/syncanysql/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     9167 2023-04-26 01:56:02.000000 syncanysql-0.1.4/syncanysql/__init__.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:07.190394 syncanysql-0.1.4/syncanysql/calculaters/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1256 2023-05-26 03:51:27.000000 syncanysql-0.1.4/syncanysql/calculaters/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6162 2023-05-23 08:35:54.000000 syncanysql-0.1.4/syncanysql/calculaters/aggregate_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      722 2023-05-26 03:56:52.000000 syncanysql-0.1.4/syncanysql/calculaters/env_variable_calculater.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1207 2023-04-23 06:39:00.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_calculater.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:07.564024 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      320 2023-05-17 08:58:39.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    10197 2023-05-04 10:22:31.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/datetime_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6002 2023-04-20 03:57:39.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/json_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6193 2023-04-24 06:11:11.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/number_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6461 2023-04-24 07:12:16.000000 syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/string_funcs.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)   171950 2023-05-26 07:01:52.000000 syncanysql-0.1.4/syncanysql/compiler.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    12804 2023-05-08 04:32:02.000000 syncanysql-0.1.4/syncanysql/config.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      229 2023-02-08 10:09:29.000000 syncanysql-0.1.4/syncanysql/errors.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     8602 2023-05-26 04:09:39.000000 syncanysql-0.1.4/syncanysql/executor.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     3750 2023-04-26 01:56:02.000000 syncanysql-0.1.4/syncanysql/main.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4366 2023-03-01 11:22:09.000000 syncanysql-0.1.4/syncanysql/parser.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     6965 2023-04-27 09:10:45.000000 syncanysql-0.1.4/syncanysql/prompt.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:08.125182 syncanysql-0.1.4/syncanysql/taskers/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       59 2023-02-13 05:49:03.000000 syncanysql-0.1.4/syncanysql/taskers/__init__.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1356 2023-03-29 02:07:07.000000 syncanysql-0.1.4/syncanysql/taskers/delete.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1603 2023-04-24 02:15:57.000000 syncanysql-0.1.4/syncanysql/taskers/execute.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1325 2023-04-28 03:17:36.000000 syncanysql-0.1.4/syncanysql/taskers/explain.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4258 2023-04-26 01:31:23.000000 syncanysql-0.1.4/syncanysql/taskers/into.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)    20959 2023-05-18 08:15:36.000000 syncanysql-0.1.4/syncanysql/taskers/query.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2890 2023-05-08 04:04:28.000000 syncanysql-0.1.4/syncanysql/taskers/set.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     2143 2023-03-29 02:06:08.000000 syncanysql-0.1.4/syncanysql/taskers/show.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1221 2023-04-25 04:04:01.000000 syncanysql-0.1.4/syncanysql/taskers/use.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      754 2023-05-08 04:04:28.000000 syncanysql-0.1.4/syncanysql/utils.py
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      106 2023-05-17 03:49:43.000000 syncanysql-0.1.4/syncanysql/version.py
+drwxrwxrwx   0 snower    (1000) snower    (1000)        0 2023-05-26 10:44:06.924782 syncanysql-0.1.4/syncanysql.egg-info/
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     4345 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/PKG-INFO
+-rwxrwxrwx   0 snower    (1000) snower    (1000)     1161 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/SOURCES.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/dependency_links.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       54 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/entry_points.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)        1 2023-04-25 10:06:25.000000 syncanysql-0.1.4/syncanysql.egg-info/not-zip-safe
+-rwxrwxrwx   0 snower    (1000) snower    (1000)      394 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/requires.txt
+-rwxrwxrwx   0 snower    (1000) snower    (1000)       11 2023-05-26 10:44:05.000000 syncanysql-0.1.4/syncanysql.egg-info/top_level.txt
```

### Comparing `syncanysql-0.1.3/PKG-INFO` & `syncanysql-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.3/README.md` & `syncanysql-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/setup.py` & `syncanysql-0.1.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # 23/02/07
 # create by: snower
 
 import sys
 import os
 from setuptools import find_packages, setup
 
-version = "0.1.3"
+version = "0.1.4"
 
 if os.path.exists("README.md"):
     if sys.version_info[0] >= 3:
         try:
             with open("README.md", encoding="utf-8") as fp:
                 long_description = fp.read()
         except Exception as e:
@@ -33,15 +33,15 @@
     author='snower',
     author_email='sujian199@gmail.com',
     license='MIT',
     packages=find_packages(exclude=['*tests*']),
     zip_safe=False,
     install_requires=[
         "pyyaml>=5.1.2",
-        "sqlglot>=10.6.2",
+        "sqlglot>=11.5.5,<12",
         "syncany>=0.2.9",
         'Pygments>=2.14.0',
         'prompt-toolkit>=3.0.36',
         "rich>=9.11.1",
     ],
     extras_require={
         "pymongo": ['pymongo>=3.6.1'],
```

### Comparing `syncanysql-0.1.3/syncanysql/__init__.py` & `syncanysql-0.1.4/syncanysql/__init__.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/calculaters/__init__.py` & `syncanysql-0.1.4/syncanysql/calculaters/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 # 2023/3/2
 # create by: snower
 
 from syncany.calculaters import CALCULATERS, Calculater, TypeFormatCalculater, TypingCalculater, MathematicalCalculater
 from syncany.calculaters import register_calculater, find_calculater, CalculaterUnknownException
+from .env_variable_calculater import CurrentEnvVariableCalculater
 from .mysql_calculater import MysqlCalculater
 from .aggregate_calculater import *
 
 SQL_CALCULATERS = {
+    "current_env_variable": CurrentEnvVariableCalculater,
     "mysql": MysqlCalculater,
     "aggregate_key": AggregateKeyCalculater,
     "aggregate_count": AggregateCountCalculater,
     "aggregate_sum": AggregateSumCalculater,
     "aggregate_max": AggregateMaxCalculater,
     "aggregate_min": AggregateMinCalculater,
     "aggregate_avg": AggregateAvgCalculater,
```

### Comparing `syncanysql-0.1.3/syncanysql/calculaters/aggregate_calculater.py` & `syncanysql-0.1.4/syncanysql/calculaters/aggregate_calculater.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             return self.reduce(*args)
         return super(StateAggregateCalculater, self).calculate(*args)
 
 
 class AggregateCountCalculater(AggregateCalculater):
     def aggregate(self, state_value, data_value):
         if data_value is None:
-            return state_value
+            return state_value or 0
         try:
             return state_value + 1
         except:
             if state_value is None:
                 return 1
             try:
                 return int(state_value) + 1
@@ -76,15 +76,15 @@
 
 class AggregateSumCalculater(AggregateCalculater):
     def aggregate(self, state_value, data_value):
         try:
             return state_value + data_value
         except:
             if data_value is None:
-                return state_value
+                return state_value or 0
             if state_value is None:
                 return data_value
             try:
                 if isinstance(state_value, (int, float)):
                     return state_value + type(state_value)(data_value)
                 try:
                     return int(state_value) + int(data_value)
```

### Comparing `syncanysql-0.1.3/syncanysql/calculaters/mysql_calculater.py` & `syncanysql-0.1.4/syncanysql/calculaters/mysql_calculater.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/datetime_funcs.py` & `syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/datetime_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/json_funcs.py` & `syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/json_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/number_funcs.py` & `syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/number_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/calculaters/mysql_funcs/string_funcs.py` & `syncanysql-0.1.4/syncanysql/calculaters/mysql_funcs/string_funcs.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/compiler.py` & `syncanysql-0.1.4/syncanysql/compiler.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,41 +22,31 @@
 from .taskers.explain import ExplainTasker
 from .taskers.set import SetCommandTasker
 from .taskers.execute import ExecuteTasker
 from .taskers.use import UseCommandTasker
 from .taskers.show import ShowCommandTasker
 
 
-class EnvVariableGetter(object):
-    def __init__(self, env_variables, key):
-        self.env_variables = env_variables
-        self.key = key
-
-    def get(self, key):
-        return self.env_variables.get_value(key)
-
-    def __deepcopy__(self, memodict=None):
-        return self
-
-    def __copy__(self):
-        return self
-
-
 class CompilerDialect(Dialect):
     class Tokenizer(tokens.Tokenizer):
         QUOTES = ["'", '"']
         COMMENTS = ["--", "#", ("/*", "*/")]
         IDENTIFIERS = ["`"]
         ESCAPES = ["'", "\\"]
         BIT_STRINGS = [("b'", "'"), ("B'", "'"), ("0b", "")]
         HEX_STRINGS = [("x'", "'"), ("X'", "'"), ("0x", "")]
 
 
 class Compiler(object):
     ESCAPE_CHARS = ['\\\\a', '\\\\b', '\\\\f', '\\\\n', '\\\\r', '\\\\t', '\\\\v', '\\\\0']
+    TYPE_FILTERS = {"int": "int", "float": "float", "str": "str", "bytes": "bytes", 'bool': 'bool', 'array': 'array', 'set': 'set',
+                   'map': 'map', "objectid": "objectid", "uuid": "uuid", "datetime": "datetime", "date": "date", "time": "time",
+                   "char": "str", "varchar": "str", "nchar": "str", "text": "str", "mediumtext": "str", "tinytext": "str",
+                   "bigint": "int", "mediumint": "int", "SMALLINT": "int", "tinyint": "int", "decimal": "float", "double": "float",
+                   "boolean": "bool", "binary": "bytes", "varbinary": "bytes", "blob": "bytes", "timestamp": "datetime"}
 
     def __init__(self, config, env_variables):
         self.config = config
         self.env_variables = env_variables
         self.mapping = {}
 
     def compile(self, sql, arguments):
@@ -152,31 +142,47 @@
             "querys": {},
             "schema": "$.*",
             "intercepts": [],
             "orders": [],
             "dependencys": [],
             "pipelines": []
         })
+
+        if expression.args.get("with"):
+            self.compile_with(expression.args.get("with"), config, arguments)
         if isinstance(expression, sqlglot_expressions.Union):
             self.compile_union(expression, config, arguments)
         elif isinstance(expression, sqlglot_expressions.Insert):
             self.compile_insert_into(expression, config, arguments)
         elif isinstance(expression, sqlglot_expressions.Select):
-            self.compile_select(expression, config, arguments)
+            self.compile_select(self.optimize_rewrite(expression, config, arguments), config, arguments)
         else:
             raise SyncanySqlCompileException('unknown sql "%s"' % self.to_sql(expression))
         return config
 
+    def compile_with(self, expression, config, arguments):
+        for sub_expression in expression.args["expressions"]:
+            table_name = sub_expression.args["alias"].name
+            subquery_arguments = {key: arguments[key] for key in CONST_CONFIG_KEYS if key in arguments}
+            subquery_config = self.compile_query(sub_expression.args["this"], subquery_arguments)
+            subquery_config["output"] = "&.--." + table_name + "::" + \
+                                        subquery_config["output"].split("::")[-1].split(" use ")[0] + " use I"
+            subquery_config["name"] = subquery_config["name"] + "#" + table_name + "#select"
+            arguments.update({subquery_config["name"] + "@" + key: value for key, value in subquery_arguments.items()})
+            config["dependencys"].append(subquery_config)
+
     def compile_subquery(self, expression, arguments):
         if not isinstance(expression, sqlglot_expressions.Subquery):
             table_name = "anonymous"
         else:
-            table_name = expression.args["alias"].args["this"].name if "alias" in expression.args \
-                                                                       and expression.args["alias"] else "anonymous"
-        subquery_name = "__subquery_" + str(uuid.uuid1().int) + "_" + table_name
+            table_name = expression.args["alias"].args["this"].name if expression.args.get("alias") else "anonymous"
+        if table_name.startswith("__subquery_"):
+            subquery_name = table_name
+        else:
+            subquery_name = "__subquery_" + str(uuid.uuid1().int) + "_" + table_name
         subquery_arguments = {key: arguments[key] for key in CONST_CONFIG_KEYS if key in arguments}
         subquery_config = self.compile_query(expression if not isinstance(expression, sqlglot_expressions.Subquery)
                                              else expression.args["this"], subquery_arguments)
         subquery_config["output"] = "&.--." + subquery_name + "::" + subquery_config["output"].split("::")[-1]
         subquery_config["name"] = subquery_config["name"] + "#" + subquery_name[2:]
         arguments.update({subquery_config["name"] + "@" + key: value for key, value in subquery_arguments.items()})
         arguments["@primary_order"] = False
@@ -280,15 +286,15 @@
         config["input"] = "&.--." + query_name + "::" + config["dependencys"][0]["output"].split("::")[-1].split(" ")[0]
         config["output"] = config["output"].split("::")[0] + "::" + config["input"].split("::")[-1].split(" ")[0]
         arguments["@primary_order"] = False
         arguments["@limit"] = 0
 
     def compile_select(self, expression, config, arguments):
         primary_table = {"db": None, "name": None, "table_name": None, "table_alias": None, "seted_primary_keys": False,
-                         "loader_primary_keys": [], "outputer_primary_keys": [], "columns": {}, "subquery": None}
+                         "loader_primary_keys": [], "outputer_primary_keys": [], "columns": {}, "subquery": None, "select_columns": {}}
 
         from_expression = expression.args.get("from")
         if not from_expression:
             primary_table["db"] = "--"
             primary_table["name"] = "--"
             primary_table["table_alias"] = "--"
             primary_table["table_name"] = "--"
@@ -310,15 +316,15 @@
                 primary_table["table_alias"] = table_info["table_alias"]
                 primary_table["table_name"] = table_info["table_name"]
             elif isinstance(from_expression, sqlglot_expressions.Subquery):
                 if "alias" not in from_expression.args:
                     raise SyncanySqlCompileException('error subquery, must have an alias name, related sql "%s"'
                                                      % self.to_sql(expression))
                 primary_table["table_alias"] = from_expression.args["alias"].args["this"].name \
-                    if "alias" in from_expression.args and from_expression.args["alias"] else None
+                    if from_expression.args.get("alias") else None
                 primary_table["table_name"] = primary_table["table_alias"]
                 subquery_name, subquery_config = self.compile_subquery(from_expression, arguments)
                 primary_table["db"] = "--"
                 primary_table["name"] = subquery_name
                 primary_table["subquery"] = subquery_config
                 config["dependencys"].append(subquery_config)
                 if self.compile_pipleline_select(expression, config, arguments, primary_table):
@@ -326,15 +332,15 @@
                 if not primary_table["table_alias"]:
                     raise SyncanySqlCompileException('error subquery, must have an alias name, related sql "%s"'
                                                      % self.to_sql(expression))
             else:
                 raise SyncanySqlCompileException('unknown select table, related sql "%s"' % self.to_sql(expression))
 
         join_tables = self.parse_joins(expression, config, arguments, primary_table, expression.args["joins"]) \
-            if "joins" in expression.args and expression.args["joins"] else {}
+            if expression.args.get("joins") else {}
         group_expression = expression.args.get("group")
 
         select_expressions = expression.args.get("expressions")
         if not select_expressions:
             raise SyncanySqlCompileException('unknown select columns, related sql "%s"' % self.to_sql(expression))
         config["schema"] = {}
         for select_expression in select_expressions:
@@ -350,15 +356,15 @@
             if not isinstance(config["schema"], dict):
                 raise SyncanySqlCompileException('unknown select * columns, related sql "%s"' % self.to_sql(expression))
 
             column_expression, aggregate_expression, calculate_expression, column_alias = None, None, None, None
             if self.is_column(select_expression, config, arguments):
                 column_expression = select_expression
             elif isinstance(select_expression, sqlglot_expressions.Alias):
-                column_alias = select_expression.args["alias"].name if "alias" in select_expression.args else None
+                column_alias = select_expression.args["alias"].name if select_expression.args.get("alias") else None
                 if column_alias and column_alias in self.mapping:
                     column_alias = self.mapping[column_alias]
                 if self.is_const(select_expression.args["this"], config, arguments):
                     const_info = self.parse_const(select_expression.args["this"], config, arguments)
                     config["schema"][column_alias] = self.compile_const(select_expression.args["this"], config, arguments, const_info)
                     continue
                 elif self.is_column(select_expression.args["this"], config, arguments):
@@ -547,14 +553,15 @@
             config["schema"][column_alias] = self.compile_join_column(expression, config, arguments, primary_table, 
                                                                       self.compile_column(expression, config, arguments, 
                                                                                           column_info), column_join_tables)
         else:
             config["schema"][column_alias] = self.compile_column(expression, config, arguments, column_info)
         if not column_info["table_name"] or column_info["table_name"] == primary_table["table_name"]:
             primary_table["columns"][column_info["column_name"]] = column_info
+        primary_table["select_columns"][column_alias] = expression
 
         if not column_info["column_name"].isidentifier() or not column_alias.isidentifier():
             return None
         if "pk" in column_info["typing_options"]:
             if not primary_table["seted_primary_keys"]:
                 primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"], primary_table["seted_primary_keys"] = [], [], True
             primary_table["loader_primary_keys"].append(column_info["column_name"])
@@ -580,14 +587,15 @@
                                             [join_tables[calculate_table_name] for calculate_table_name in calculate_table_names],
                                             join_tables, column_join_tables)
             calculate_column = self.compile_calculate(expression, config, arguments, primary_table, column_join_tables)
             config["schema"][column_alias] = self.compile_join_column(expression, config, arguments, primary_table,
                                                                       calculate_column, column_join_tables)
         else:
             config["schema"][column_alias] = self.compile_calculate(expression, config, arguments, primary_table, [])
+        primary_table["select_columns"][column_alias] = expression
         if parse_primary_key and not primary_table["seted_primary_keys"] and not primary_table["outputer_primary_keys"] \
                 and column_alias.isidentifier():
             loader_primary_keys = [calculate_field["column_name"] for calculate_field in calculate_fields
                                    if calculate_field["column_name"].isidentifier() and
                                    (not calculate_field["table_name"] or calculate_field["table_name"] == primary_table["table_name"])]
             if loader_primary_keys:
                 primary_table["loader_primary_keys"], primary_table["outputer_primary_keys"] = loader_primary_keys, [column_alias]
@@ -608,57 +616,94 @@
                                          for join_column in join_table["join_columns"] if join_column["table_name"] and join_column["table_name"] != primary_table["table_name"]}),
                                    key=lambda x: 0xffffff if x == primary_table["table_name"] else join_tables[x]["ref_count"])
         self.compile_join_column_tables(expression, config, arguments, primary_table,
                                         [join_tables[column_join_name] for column_join_name in column_join_names
                                          if column_join_name != primary_table["table_name"]], join_tables, column_join_tables)
 
     def compile_join_column(self, expression, config, arguments, primary_table, column, column_join_tables):
+        jit_define_name = None
+        if isinstance(column, list) and len(column) == 3 and column[0] == "#call" and column[1].startswith("jit_define_") and column[2] == "$.*":
+            jit_define_name, column = column[1], config["defines"][column[1]]
+
+        if isinstance(column, str):
+            column = ":" + column
+        elif isinstance(column, list):
+            if column and isinstance(column[0], str):
+                column[0] = ":" + column[0]
+            else:
+                column = [":"] + column
+        else:
+            column = [":", column]
+
         for i in range(len(column_join_tables)):
             join_table = column_join_tables[i]
-            if isinstance(column, str):
-                column = ":" + column
-            elif isinstance(column, list):
-                if column and isinstance(column[0], str):
-                    column[0] = ":" + column[0]
-                else:
-                    column = [":"] + column
-            else:
-                column = [":", column]
             if len(join_table["calculate_expressions"]) == 1:
-                join_columns = self.compile_calculate(join_table["calculate_expressions"][0], config, arguments, primary_table, column_join_tables, i)
+                join_columns = self.compile_calculate(join_table["calculate_expressions"][0], config, arguments,
+                                                      primary_table, column_join_tables, i)
             else:
-                join_columns = [self.compile_calculate(calculate_expression, config, arguments, primary_table, column_join_tables, i)
-                               for calculate_expression in join_table["calculate_expressions"]]
-            join_db_table = "&." + join_table["db"] + "." + join_table["table"] + "::" + "+".join(join_table["primary_keys"])
+                join_columns = [self.compile_calculate(calculate_expression, config, arguments, primary_table,
+                                                       column_join_tables, i)
+                                for calculate_expression in join_table["calculate_expressions"]]
+
+
+            join_db_table = "&." + join_table["db"] + "." + join_table["table"] + "::" + (
+                "+".join(join_table["primary_keys"]) if join_table["primary_keys"] else "id")
             if join_table["querys"]:
                 join_db_table = [join_db_table, join_table["querys"]]
-            column = [join_columns, join_db_table, column]
+
+            if join_table["having_expressions"]:
+                if len(join_table["having_expressions"]) == 1:
+                    having_columns = self.compile_calculate(join_table["having_expressions"][0], config, arguments,
+                                                            primary_table, column_join_tables, i - 1)
+                else:
+                    def compile_having_column(left_having_expression, right_having_expression):
+                        left_having_column = self.compile_calculate(left_having_expression, config, arguments,
+                                                                    primary_table, column_join_tables, i - 1)
+                        if isinstance(right_having_expression, list):
+                            if len(right_having_expression) > 1:
+                                right_having_column = compile_having_column(right_having_expression[0],
+                                                                            right_having_expression[1:])
+                                return ["#if", left_having_column, right_having_column, ["#const", False]]
+                            right_having_expression = right_having_expression[0]
+                        right_having_column = self.compile_calculate(right_having_expression, config, arguments,
+                                                                     primary_table, column_join_tables, i - 1)
+                        return ["#if", left_having_column, right_having_column, ["#const", False]]
+                    having_columns = compile_having_column(join_table["having_expressions"][0],
+                                                           join_table["having_expressions"][1:])
+                column = [join_columns, join_db_table, having_columns, column] \
+                    if join_columns else [join_db_table, having_columns, column]
+            else:
+                column = [join_columns, join_db_table, column] if join_columns else [join_db_table, column]
+
+        if jit_define_name:
+            config["defines"][jit_define_name] = column
+            return ["#call", jit_define_name, "$.*"]
         return column
 
     def compile_join_column_field(self, expression, config, arguments, primary_table, ci, join_column, column_join_tables):
         if not join_column["table_name"] or join_column["table_name"] == primary_table["table_name"]:
             return self.compile_column(expression, config, arguments, join_column, len(column_join_tables) - ci)
         ji = [j for j in range(len(column_join_tables)) if join_column["table_name"] == column_join_tables[j]["name"]][0]
         return self.compile_column(expression, config, arguments, join_column, ji - ci)
 
     def compile_where_condition(self, expression, config, arguments, primary_table, join_tables, is_query_condition=True):
         if isinstance(expression, sqlglot_expressions.And):
             left_condition = self.compile_where_condition(expression.args.get("this"), config, arguments,
-                                                          primary_table, join_tables, True)
+                                                          primary_table, join_tables, is_query_condition)
             right_condition = self.compile_where_condition(expression.args.get("expression"), config, arguments,
-                                                           primary_table, join_tables, True)
+                                                           primary_table, join_tables, is_query_condition)
             if left_condition and right_condition:
-                return ["@and", left_condition, right_condition]
+                return ["#if", left_condition, right_condition, ["#const", False]]
             return left_condition or right_condition or None
         if isinstance(expression, sqlglot_expressions.Or):
-            return [
-                "@or",
-                self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table, join_tables, False),
-                self.compile_where_condition(expression.args.get("expression"), config, arguments, primary_table, join_tables, False)
-            ]
+            left_condition = self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table,
+                                                          join_tables, False)
+            right_condition = self.compile_where_condition(expression.args.get("expression"), config, arguments,
+                                                           primary_table, join_tables, False)
+            return ["#if", left_condition, ["#const", True], right_condition]
 
         def parse_calucate(calculate_expression):
             if not isinstance(config.get("schema"), dict):
                 return calculate_expression
             if self.is_column(calculate_expression, config, arguments):
                 calculate_name = "__where_condition_value_%d__" % id(calculate_expression)
                 self.compile_select_calculate_column(calculate_expression, config, arguments, primary_table,
@@ -682,19 +727,25 @@
             is_query_column, left_column, left_calculater = False, None, None
             if expression.args.get("expressions"):
                 left_expression, right_expression = expression.args["this"], expression.args["expressions"]
             elif expression.args.get("query"):
                 left_expression, right_expression = expression.args["this"], expression.args["query"]
             else:
                 left_expression, right_expression = expression.args["this"], expression.args["expression"]
+
             if self.is_column(left_expression, config, arguments):
                 left_column = self.parse_column(left_expression, config, arguments)
-                if is_query_condition and (left_column["table_name"] and primary_table["table_alias"] == left_column["table_name"]) \
-                        or not left_column["table_name"]:
+                if is_query_condition and ((left_column["table_name"]
+                                            and primary_table["table_name"] == left_column["table_name"]) or not left_column["table_name"]):
                     is_query_column = True
+            if not is_query_column and self.is_column(right_expression, config, arguments):
+                right_column = self.parse_column(right_expression, config, arguments)
+                if is_query_condition and ((right_column["table_name"]
+                                            and primary_table["table_name"] == right_column["table_name"]) or not right_column["table_name"]):
+                    left_expression, right_expression, is_query_column, left_column = right_expression, left_expression, True, right_column
             if not is_query_column:
                 if not isinstance(config["schema"], dict):
                     raise SyncanySqlCompileException(
                         'error where condition, only "=,!=,>,>=,<,<=,in" operations executed by the database cannot be transparently transmitted,'
                         ' and it is executed with the having statement, column unkown, related sql "%s"'
                         % self.to_sql(expression))
                 left_calculater = self.compile_calculate(parse_calucate(left_expression), config, arguments,
@@ -802,23 +853,18 @@
             is_query_column, condition_column, left_calculater, right_calculater = parse(expression)
             if not isinstance(right_calculater, list) or len(right_calculater) != 2 or right_calculater[0] != "#const":
                 raise SyncanySqlCompileException(
                     'error having condition, like condition value must be const, related sql "%s"'
                     % self.to_sql(expression))
             return ["#if", ["@re::match", right_calculater[1].replace("%", ".*").replace(".*.*", "%"), left_calculater],
                     ["#const", True], ["#const", False]]
-        elif isinstance(expression, (sqlglot_expressions.Not, sqlglot_expressions.Is)):
-            return self.compile_calculate(parse_calucate(expression), config, arguments, primary_table, [])
-        elif isinstance(expression, sqlglot_expressions.Between):
-            return self.compile_calculate(parse_calucate(expression), config, arguments, primary_table, [])
         elif isinstance(expression, sqlglot_expressions.Paren):
             return self.compile_where_condition(expression.args.get("this"), config, arguments, primary_table, join_tables, False)
         else:
-            raise SyncanySqlCompileException('unknown where condition, only "=,!=,>,>=,<,<=,in" operations are supported, related sql "%s"'
-                                             % self.to_sql(expression))
+            return self.compile_calculate(parse_calucate(expression), config, arguments, primary_table, [])
 
     def compile_query_condition(self, expression, config, arguments, primary_table, typing_filters):
         if isinstance(expression, sqlglot_expressions.Select):
             select_expressions = expression.args.get("expressions")
             if not select_expressions or len(select_expressions) != 1 or \
                     (not isinstance(select_expressions[0], sqlglot_expressions.Alias) and
                      not self.is_column(select_expressions[0], config, arguments)):
@@ -998,25 +1044,26 @@
 
         config["schema"][column_alias] = ["#make", {
             "key": copy.deepcopy(group_column),
             "value": copy.deepcopy(value_column),
         }, copy.deepcopy(aggregate_column["aggregate"])]
         config["aggregate"]["key"] = copy.deepcopy(aggregate_column["key"])
         config["aggregate"]["schema"][column_alias] = aggregate_column
+        primary_table["select_columns"][column_alias] = expression
 
     def compile_aggregate_key(self, expression, config, arguments, primary_table, join_tables):
         if not expression:
             return ["@aggregate_key", ["#const", "__k_g__"]]
 
         group_column = ["@aggregate_key"]
         for group_expression in expression.args["expressions"]:
             if self.is_column(group_expression, config, arguments):
                 group_expression_column = self.parse_column(group_expression, config, arguments)
                 if isinstance(config["schema"], dict) and not group_expression_column["table_name"] \
-                        and primary_table["table_alias"] and group_expression_column["column_name"] in config["schema"]:
+                        and group_expression_column["column_name"] in config["schema"]:
                     group_column.append(config["schema"][group_expression_column["column_name"]])
                     continue
                 if not group_expression_column["table_name"] or group_expression_column["table_name"] == primary_table["table_name"]:
                     group_column.append(self.compile_column(group_expression, config, arguments, group_expression_column))
                     continue
 
             calculate_fields = []
@@ -1143,14 +1190,28 @@
                     if self.is_const(arg_expression, config, arguments):
                         column.append(self.compile_const(arg_expression, config, arguments,
                                                          self.parse_const(arg_expression, config, arguments)))
                     else:
                         column.append(self.compile_calculate(arg_expression, config, arguments, primary_table, column_join_tables, join_index))
                 return column
 
+            if calculater_name == "jit":
+                if len(expression.args["expressions"]) != 1:
+                    raise SyncanySqlCompileException(
+                        'unknown calculate expression, jit run must by one expression related sql "%s"' % self.to_sql(expression))
+                define_name = "jit_define_" + str(str(expression).__hash__()).replace("-", "_")
+                if "defines" not in config:
+                    config["defines"] = {}
+                if self.is_const(expression.args["expressions"][0], config, arguments):
+                    config["defines"][define_name] = self.compile_const(expression.args["expressions"][0], config, arguments,
+                                                                        self.parse_const(expression.args["expressions"][0], config, arguments))
+                else:
+                    config["defines"][define_name] = self.compile_calculate(expression.args["expressions"][0], config, arguments, primary_table, column_join_tables, join_index)
+                return ["#call", define_name, "$.*"]
+
             if calculater_name == "yield_data":
                 column = ["#yield"]
                 for arg_expression in expression.args.get("expressions", []):
                     if self.is_const(arg_expression, config, arguments):
                         column.append(self.compile_const(arg_expression, config, arguments,
                                                          self.parse_const(arg_expression, config, arguments)))
                     else:
@@ -1303,22 +1364,24 @@
             return self.compile_const(expression, config, arguments, self.parse_const(expression, config, arguments))
         else:
             raise SyncanySqlCompileException('unknown calculate expression, related sql "%s"' % self.to_sql(expression))
 
     def compile_having_condition(self, expression, config, arguments, primary_table):
         if isinstance(expression, sqlglot_expressions.And):
             return [
-                "@and",
+                "#if",
                 self.compile_having_condition(expression.args.get("this"), config, arguments, primary_table),
-                self.compile_having_condition(expression.args.get("expression"), config, arguments, primary_table)
+                self.compile_having_condition(expression.args.get("expression"), config, arguments, primary_table),
+                ["#const", False]
             ]
         if isinstance(expression, sqlglot_expressions.Or):
             return [
-                "@or",
+                "#if",
                 self.compile_having_condition(expression.args.get("this"), config, arguments, primary_table),
+                ["#const", True],
                 self.compile_having_condition(expression.args.get("expression"), config, arguments, primary_table)
             ]
 
         def parse(expression):
             left_column = None
             if "aggregate" not in config:
                 config["aggregate"] = copy.deepcopy(DEAULT_AGGREGATE)
@@ -1404,29 +1467,40 @@
         elif isinstance(expression, sqlglot_expressions.Like):
             left_calculater, right_calculater = parse(expression)
             if not isinstance(right_calculater, list) or len(right_calculater) != 2 or right_calculater[0] != "#const":
                 raise SyncanySqlCompileException('error having condition, like condition value must be const, related sql "%s"'
                                                  % self.to_sql(expression))
             return ["#if", ["@re::match", right_calculater[1].replace("%", ".*").replace(".*.*", "%"), left_calculater],
                     ["#const", True], ["#const", False]]
-        elif isinstance(expression, (sqlglot_expressions.Not, sqlglot_expressions.Is)):
-            return self.compile_calculate(expression, config, arguments, primary_table, [])
-        elif isinstance(expression, sqlglot_expressions.Between):
-            return self.compile_calculate(expression, config, arguments, primary_table, [])
         elif isinstance(expression, sqlglot_expressions.Paren):
             return self.compile_having_condition(expression.args.get("this"), config, arguments, primary_table)
         else:
-            raise SyncanySqlCompileException('unknown having condition, related sql "%s"' % self.to_sql(expression))
+            return self.compile_calculate(expression, config, arguments, primary_table, [])
 
     def compile_order(self, expression, config, arguments, primary_table):
         primary_sort_keys, sort_keys = [], []
         for order_expression in expression:
+            if not self.is_column(order_expression.args["this"], config, arguments):
+                if isinstance(config["schema"], dict):
+                    if str(order_expression.args["this"]) in config["schema"]:
+                        sort_keys.append((str(order_expression.args["this"]), True if order_expression.args["desc"] else False))
+                        continue
+                    has_column = False
+                    for column_alias, column_expression in primary_table["select_columns"].items():
+                        if str(order_expression.args["this"]).lower() == str(column_expression).lower():
+                            sort_keys.append((column_alias, True if order_expression.args["desc"] else False))
+                            has_column = True
+                            break
+                    if has_column:
+                        continue
+                raise SyncanySqlCompileException('unknown order by column, the order by field must appear in the select field, related sql "%s"'
+                                                 % self.to_sql(expression))
             column = self.parse_column(order_expression.args["this"], config, arguments)
             if not isinstance(config["schema"], dict) or \
-                    (column["table_name"] and primary_table["table_alias"] == column["table_name"]) or \
+                    (column["table_name"] and primary_table["table_name"] == column["table_name"]) or \
                     (not column["table_name"] and column["column_name"] in primary_table["columns"]):
                 primary_sort_keys.append([column["column_name"], True if order_expression.args["desc"] else False])
             sort_keys.append((column["column_name"], True if order_expression.args["desc"] else False))
         if sort_keys and len(primary_sort_keys) < len(sort_keys):
             if isinstance(config["schema"], dict):
                 for sort_key, _ in sort_keys:
                     if sort_key not in config["schema"]:
@@ -1447,195 +1521,254 @@
                     return child_filter_column
                 return [typing_filter_column, compile_column_filter(typing_filters[1:])]
             return [typing_filter_column, compile_column_filter(column["typing_filters"][1:])]
         return ("$" * scope_depth) + "." + column["column_name"]
     
     def compile_const(self, expression, config, arguments, literal):
         if "value_getter" in literal and literal["value_getter"]:
-            if "imports" not in config:
-                config["imports"] = {}
-            config["imports"]["getter_" + str(id(literal["value_getter"]))] = literal["value_getter"]
-            return ["@getter_" + str(id(literal["value_getter"])) + "::get", ["#const", literal["value_getter"].key]]
+            return literal["value_getter"]
         return ["#const", literal["value"]]
 
     def parse_joins(self, expression, config, arguments, primary_table, join_expressions):
         join_tables = {}
         for join_expression in join_expressions:
-            if "alias" not in join_expression.args["this"].args:
-                raise SyncanySqlCompileException('error join, table must be alias name, related sql "%s"' % self.to_sql(join_expression))
-            name = join_expression.args["this"].args["alias"].args["this"].name
+            if (join_expression.kind and join_expression.kind.lower() != "cross") \
+                    or (join_expression.side and join_expression.side.lower() != "left"):
+                raise SyncanySqlCompileException('unknown join expression, unsupported join type, related sql "%s"' % self.to_sql(join_expression))
             if isinstance(join_expression.args["this"], sqlglot_expressions.Table):
                 table_info = self.parse_table(join_expression.args["this"], config, arguments)
                 db, table, subquery_config = table_info["db"], table_info["name"], None
             elif isinstance(join_expression.args["this"], sqlglot_expressions.Subquery):
                 subquery_name, subquery_config = self.compile_subquery(join_expression.args["this"], arguments)
                 db, table = "--", subquery_name
                 config["dependencys"].append(subquery_config)
             else:
                 raise SyncanySqlCompileException('unknown join expression, related sql "%s"' % self.to_sql(join_expression))
-            if "on" not in join_expression.args:
-                raise SyncanySqlCompileException('error join, on condition is unknown, related sql "%s"'
-                                                 % self.to_sql(join_expression))
+            if not join_expression.args["this"].args.get("alias"):
+                name = db + "." + table
+            else:
+                name = join_expression.args["this"].args["alias"].args["this"].name
             join_table = {
-                "db": db, "table": table, "name": name, "primary_keys": [],
+                "db": db, "table": table, "name": name, "primary_keys": [], "columns": set([]),
                 "join_columns": [], "calculate_expressions": [], "querys": {}, "ref_count": 0,
-                "subquery": subquery_config
+                "having_expressions": [], "subquery": subquery_config
             }
-            self.parse_on_condition(join_expression.args["on"], config, arguments, primary_table, join_table)
-            self.parse_condition_typing_filter(expression, join_table, arguments)
-            if not join_table["primary_keys"] or not join_table["join_columns"]:
-                raise SyncanySqlCompileException('error join, columns unknown, related sql "%s"' % self.to_sql(join_expression))
+            if join_expression.args.get("on"):
+                self.parse_on_condition(join_expression.args["on"], config, arguments, primary_table, join_table)
+                self.parse_condition_typing_filter(expression, join_table, arguments)
+            if not join_table["primary_keys"]:
+                if join_table["columns"]:
+                    join_table["primary_keys"].append(list(join_table["columns"])[0])
+                else:
+                    def find_primary_key(item_expression):
+                        if not isinstance(item_expression, sqlglot_expressions.Expression):
+                            return None
+                        if isinstance(item_expression, sqlglot_expressions.Column):
+                            item_column = self.parse_column(item_expression, config, arguments)
+                            if item_column["table_name"] and item_column["table_name"] == join_table["name"]:
+                                return item_column["column_name"]
+                            return None
+                        for child_item_expressions in item_expression.args.values():
+                            if not isinstance(child_item_expressions, list):
+                                child_item_expressions = [child_item_expressions]
+                            for child_item_expression in child_item_expressions:
+                                column_name = find_primary_key(child_item_expression)
+                                if column_name is not None:
+                                    return column_name
+                        return None
+                    primary_key = find_primary_key(expression)
+                    if not primary_key:
+                        raise SyncanySqlCompileException('unknown join expression, related sql "%s"' % self.to_sql(join_expression))
+                    join_table["primary_keys"].append(primary_key)
             join_tables[join_table["name"]] = join_table
 
         for name, join_table in join_tables.items():
+            if not join_table["join_columns"]:
+                continue
             for join_column in join_table["join_columns"]:
                 if not join_column["table_name"] or join_column["table_name"] == primary_table["table_name"]:
                     continue
                 if join_column["table_name"] not in join_tables:
                     raise SyncanySqlCompileException("unknown join table: " + join_column["table_name"])
                 join_tables[join_column["table_name"]]["ref_count"] += 1
         return join_tables
 
     def parse_on_condition(self, expression, config, arguments, primary_table, join_table):
-        if not expression:
-            return
         if isinstance(expression, sqlglot_expressions.And):
             self.parse_on_condition(expression.args.get("this"), config, arguments, primary_table, join_table)
             self.parse_on_condition(expression.args.get("expression"), config, arguments, primary_table, join_table)
             return
+        if isinstance(expression, sqlglot_expressions.Or):
+            calculate_fields = []
+            self.parse_calculate(expression.args.get("this"), config, arguments, primary_table, calculate_fields)
+            self.parse_calculate(expression.args.get("expression"), config, arguments, primary_table, calculate_fields)
+            for calculate_field in calculate_fields:
+                if calculate_field["table_name"] != join_table["name"]:
+                    join_table["join_columns"].append(calculate_field)
+                else:
+                    join_table["columns"].add(calculate_field["column_name"])
+            join_table["having_expressions"].append(expression)
+            return
 
         def parse(expression):
-            table_expression, value_expression = None, None
-            if isinstance(expression, sqlglot_expressions.EQ) and expression.args.get("expression"):
-                for arg_expression in (expression.args["this"], expression.args["expression"]):
-                    if not isinstance(arg_expression, sqlglot_expressions.Column):
-                        if not self.is_column(arg_expression, config, arguments):
-                            continue
-                        arg_column = self.parse_column(arg_expression, config, arguments)
-                        condition_table = arg_column["table_name"]
-                    else:
-                        condition_table = arg_expression.args["table"].name if "table" in arg_expression.args else None
-                    if condition_table and condition_table == join_table["name"]:
-                        table_expression = arg_expression
-                        break
-                if table_expression is None:
-                    raise SyncanySqlCompileException('unkonw join on condition, related sql "%s"' % self.to_sql(expression))
-                value_expression = expression.args["expression"] if table_expression == expression.args["this"] else expression.args["this"]
-            elif expression.args.get("expressions"):
-                table_expression, value_expression = expression.args["this"], expression.args["expressions"]
+            if expression.args.get("expressions"):
+                left_expression, right_expression = expression.args["this"], expression.args["expressions"]
             elif expression.args.get("query"):
-                table_expression, value_expression = expression.args["this"], expression.args["query"]
-            elif isinstance(expression.args["expression"], sqlglot_expressions.Subquery):
-                table_expression, value_expression = expression.args["this"], expression.args["expression"].args["this"]
-            else:
-                table_expression, value_expression = expression.args["this"], expression.args["expression"]
-
-            condition_column = self.parse_column(table_expression, config, arguments)
-            if not isinstance(expression, sqlglot_expressions.EQ) or self.is_const(value_expression, config, arguments) \
-                    or isinstance(value_expression, list) or isinstance(value_expression, sqlglot_expressions.Select):
-                if not self.is_column(table_expression, config, arguments) or not condition_column["table_name"]:
-                    raise SyncanySqlCompileException('unkonw join on condition, related sql "%s"' % self.to_sql(expression))
-                if isinstance(value_expression, (sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union)):
-                    value_column = self.compile_query_condition(value_expression, config, arguments, primary_table,
-                                                                condition_column["typing_filters"])
-                    if isinstance(expression, sqlglot_expressions.In):
-                        value_column = ["@convert_array", value_column]
-                    else:
-                        value_column = ["@convert_array", value_column, ":$.:0"]
-                    return False, condition_column, value_column
-                if isinstance(value_expression, list):
-                    value_items = []
-                    for value_expression_item in value_expression:
-                        if not self.is_const(value_expression_item, config, arguments):
-                            raise SyncanySqlCompileException('error join on condition, array must be const value, related sql "%s"'
-                                                             % self.to_sql(expression))
-                        value_items.append(self.parse_const(value_expression_item, config, arguments)["value"])
-                    return False, condition_column, value_items
-                calculate_fields = []
-                self.parse_calculate(value_expression, config, arguments, primary_table, calculate_fields)
-                if calculate_fields:
-                    raise SyncanySqlCompileException('error join on condition, conditions except = conditions must be constants, related sql "%s"'
-                                                     % self.to_sql(expression))
-                return False, condition_column, self.compile_calculate(value_expression, config, arguments, primary_table, [])
+                left_expression, right_expression = expression.args["this"], expression.args["query"]
+            else:
+                left_expression, right_expression = expression.args["this"], expression.args["expression"]
+
+            left_column, right_column = None, None
+            if self.is_column(left_expression, config, arguments):
+                left_column = self.parse_column(left_expression, config, arguments)
+            if self.is_column(right_expression, config, arguments):
+                right_column = self.parse_column(right_expression, config, arguments)
+
+            condition_column, join_on_expression, value_expression = left_column, None, right_expression
+            if isinstance(expression, sqlglot_expressions.EQ):
+                if left_column and left_column["table_name"] == join_table["name"]:
+                    condition_column, value_expression = left_column, right_expression
+                    if not self.is_const(right_expression, config, arguments) and not isinstance(right_expression, list) \
+                            and not isinstance(right_expression, sqlglot_expressions.Select):
+                        join_on_expression = right_expression
+                else:
+                    if right_column and right_column["table_name"] == join_table["name"]:
+                        condition_column, value_expression = right_column, left_expression
+                        if not self.is_const(left_expression, config, arguments) and not isinstance(left_expression, list) \
+                                and not isinstance(left_expression, sqlglot_expressions.Select):
+                            join_on_expression = left_expression
+            if condition_column and not condition_column["table_name"]:
+                raise SyncanySqlCompileException('unkonw join on condition, related sql "%s"' % self.to_sql(expression))
+
+            if condition_column and join_on_expression:
+                if self.is_column(join_on_expression, config, arguments):
+                    if condition_column["column_name"] in join_table["primary_keys"]:
+                        raise SyncanySqlCompileException(
+                            'error join on condition, primary_key duplicate, related sql "%s"' % self.to_sql(expression))
+                    join_table["join_columns"].append(self.parse_column(join_on_expression, config, arguments))
+                    join_table["primary_keys"].append(condition_column["column_name"])
+                    join_table["columns"].add(condition_column["column_name"])
+                    join_table["calculate_expressions"].append(join_on_expression)
+                    return True, condition_column, None
 
-            if self.is_column(value_expression, config, arguments):
+                calculate_fields = []
+                self.parse_calculate(join_on_expression, config, arguments, primary_table, calculate_fields)
+                if not calculate_fields and condition_column["table_name"] == join_table["name"]:
+                    return False, condition_column, self.compile_calculate(join_on_expression, config, arguments,
+                                                                           primary_table, [])
                 if condition_column["column_name"] in join_table["primary_keys"]:
-                    raise SyncanySqlCompileException('error join on condition, primary_key duplicate, related sql "%s"' % self.to_sql(expression))
-                join_table["join_columns"].append(self.parse_column(value_expression, config, arguments))
+                    raise SyncanySqlCompileException(
+                        'error join on condition, primary_key duplicate, related sql "%s"' % self.to_sql(expression))
+                join_table["join_columns"].extend(calculate_fields)
                 join_table["primary_keys"].append(condition_column["column_name"])
-                join_table["calculate_expressions"].append(value_expression)
+                join_table["columns"].add(condition_column["column_name"])
+                join_table["calculate_expressions"].append(join_on_expression)
                 return True, condition_column, None
+
             calculate_fields = []
-            self.parse_calculate(value_expression, config, arguments, primary_table, calculate_fields)
-            if not calculate_fields and condition_column["table_name"] == join_table["name"]:
-                return False, condition_column, self.compile_calculate(value_expression, config, arguments, primary_table, [])
-            if condition_column["column_name"] in join_table["primary_keys"]:
-                raise SyncanySqlCompileException('error join on condition, primary_key duplicate, related sql "%s"' % self.to_sql(expression))
-            join_table["join_columns"].extend(calculate_fields)
-            join_table["primary_keys"].append(condition_column["column_name"])
-            join_table["calculate_expressions"].append(value_expression)
-            return True, condition_column, None
+            if condition_column and not isinstance(value_expression, (sqlglot_expressions.Select,
+                                                                      sqlglot_expressions.Subquery, sqlglot_expressions.Union, list)):
+                self.parse_calculate(value_expression, config, arguments, primary_table, calculate_fields)
+            if not condition_column or calculate_fields:
+                self.parse_calculate(right_expression if value_expression is left_expression else left_expression,
+                                     config, arguments, primary_table, calculate_fields)
+                for calculate_field in calculate_fields:
+                    if calculate_field["table_name"] != join_table["name"]:
+                        join_table["join_columns"].append(calculate_field)
+                    else:
+                        join_table["columns"].add(calculate_field["column_name"])
+                join_table["having_expressions"].append(expression)
+                return False, None, None
+
+            if isinstance(value_expression, (sqlglot_expressions.Select, sqlglot_expressions.Subquery, sqlglot_expressions.Union)):
+                value_column = self.compile_query_condition(value_expression, config, arguments, primary_table, condition_column["typing_filters"])
+                if isinstance(expression, sqlglot_expressions.In):
+                    value_column = ["@convert_array", value_column]
+                else:
+                    value_column = ["@convert_array", value_column, ":$.:0"]
+                return False, condition_column, value_column
+            if isinstance(value_expression, list):
+                value_items = []
+                for value_expression_item in value_expression:
+                    if not self.is_const(value_expression_item, config, arguments):
+                        raise SyncanySqlCompileException('error join on condition, array must be const value, related sql "%s"'
+                                                         % self.to_sql(expression))
+                    value_items.append(self.parse_const(value_expression_item, config, arguments)["value"])
+                return False, condition_column, value_items
+            return False, condition_column, self.compile_calculate(value_expression, config, arguments, primary_table, [])
 
         if isinstance(expression, sqlglot_expressions.EQ):
             is_column, condition_column, value_column = parse(expression)
-            if not is_column:
+            if not is_column and condition_column:
                 if condition_column["typing_name"] not in join_table["querys"]:
                     join_table["querys"][condition_column["typing_name"]] = {}
                 join_table["querys"][condition_column["typing_name"]]["=="] = value_column
         elif isinstance(expression, sqlglot_expressions.NEQ):
             is_column, condition_column, value_column = parse(expression)
             if is_column:
-                raise SyncanySqlCompileException('error join on condition, conditions except = conditions must be constants, related sql "%s"'
+                raise SyncanySqlCompileException('error join on condition, conditions except != conditions must be constants, related sql "%s"'
                                                  % self.to_sql(expression))
-            if condition_column["typing_name"] not in join_table["querys"]:
-                join_table["querys"][condition_column["typing_name"]] = {}
-            join_table["querys"][condition_column["typing_name"]]["!="] = value_column
+            if condition_column:
+                if condition_column["typing_name"] not in join_table["querys"]:
+                    join_table["querys"][condition_column["typing_name"]] = {}
+                join_table["querys"][condition_column["typing_name"]]["!="] = value_column
         elif isinstance(expression, sqlglot_expressions.GT):
             is_column, condition_column, value_column = parse(expression)
             if is_column:
-                raise SyncanySqlCompileException('error join on condition, conditions except = conditions must be constants, related sql "%s"'
+                raise SyncanySqlCompileException('error join on condition, conditions except > conditions must be constants, related sql "%s"'
                                                  % self.to_sql(expression))
-            if condition_column["typing_name"] not in join_table["querys"]:
-                join_table["querys"][condition_column["typing_name"]] = {}
-            join_table["querys"][condition_column["typing_name"]][">"] = value_column
+            if condition_column:
+                if condition_column["typing_name"] not in join_table["querys"]:
+                    join_table["querys"][condition_column["typing_name"]] = {}
+                join_table["querys"][condition_column["typing_name"]][">"] = value_column
         elif isinstance(expression, sqlglot_expressions.GTE):
             is_column, condition_column, value_column = parse(expression)
             if is_column:
-                raise SyncanySqlCompileException('error join on condition, conditions except = conditions must be constants, related sql "%s"'
+                raise SyncanySqlCompileException('error join on condition, conditions except >= conditions must be constants, related sql "%s"'
                                                  % self.to_sql(expression))
-            if condition_column["typing_name"] not in join_table["querys"]:
-                join_table["querys"][condition_column["typing_name"]] = {}
-            join_table["querys"][condition_column["typing_name"]][">="] = value_column
+            if condition_column:
+                if condition_column["typing_name"] not in join_table["querys"]:
+                    join_table["querys"][condition_column["typing_name"]] = {}
+                join_table["querys"][condition_column["typing_name"]][">="] = value_column
         elif isinstance(expression, sqlglot_expressions.LT):
             is_column, condition_column, value_column = parse(expression)
             if is_column:
-                raise SyncanySqlCompileException('error join on condition, conditions except = conditions must be constants, related sql "%s"'
+                raise SyncanySqlCompileException('error join on condition, conditions except < conditions must be constants, related sql "%s"'
                                                  % self.to_sql(expression))
-            if condition_column["typing_name"] not in join_table["querys"]:
-                join_table["querys"][condition_column["typing_name"]] = {}
-            join_table["querys"][condition_column["typing_name"]]["<"] = value_column
+            if condition_column:
+                if condition_column["typing_name"] not in join_table["querys"]:
+                    join_table["querys"][condition_column["typing_name"]] = {}
+                join_table["querys"][condition_column["typing_name"]]["<"] = value_column
         elif isinstance(expression, sqlglot_expressions.LTE):
             is_column, condition_column, value_column = parse(expression)
             if is_column:
-                raise SyncanySqlCompileException('error join on condition, conditions except = conditions must be constants, related sql "%s"'
+                raise SyncanySqlCompileException('error join on condition, conditions except <= conditions must be constants, related sql "%s"'
                                                  % self.to_sql(expression))
-            if condition_column["typing_name"] not in join_table["querys"]:
-                join_table["querys"][condition_column["typing_name"]] = {}
-            join_table["querys"][condition_column["typing_name"]]["<="] = value_column
+            if condition_column:
+                if condition_column["typing_name"] not in join_table["querys"]:
+                    join_table["querys"][condition_column["typing_name"]] = {}
+                join_table["querys"][condition_column["typing_name"]]["<="] = value_column
         elif isinstance(expression, sqlglot_expressions.In):
             is_column, condition_column, value_column = parse(expression)
             if is_column:
-                raise SyncanySqlCompileException('error join on condition, conditions except = conditions must be constants, related sql "%s"'
+                raise SyncanySqlCompileException('error join on condition, conditions except in conditions must be constants, related sql "%s"'
                                                  % self.to_sql(expression))
-            if condition_column["typing_name"] not in join_table["querys"]:
-                join_table["querys"][condition_column["typing_name"]] = {}
-            join_table["querys"][condition_column["typing_name"]]["in"] = value_column
+            if condition_column:
+                if condition_column["typing_name"] not in join_table["querys"]:
+                    join_table["querys"][condition_column["typing_name"]] = {}
+                join_table["querys"][condition_column["typing_name"]]["in"] = value_column
         else:
-            raise SyncanySqlCompileException('error join on condition, only "=,!=,>,>=,<,<=,in" operations are supported, related sql "%s"'
-                                             % self.to_sql(expression))
+            calculate_fields = []
+            self.parse_calculate(expression, config, arguments, primary_table, calculate_fields)
+            for calculate_field in calculate_fields:
+                if calculate_field["table_name"] != join_table["name"]:
+                    join_table["join_columns"].append(calculate_field)
+                else:
+                    join_table["columns"].add(calculate_field["column_name"])
+            join_table["having_expressions"].append(expression)
 
     def parse_calculate(self, expression, config, arguments, primary_table, calculate_fields):
         if hasattr(expression, "syncany_valuer"):
             return
         if isinstance(expression, sqlglot_expressions.Anonymous):
             for arg_expression in expression.args.get("expressions", []):
                 self.parse_calculate(arg_expression, config, arguments, primary_table, calculate_fields)
@@ -1648,15 +1781,15 @@
             if expression.args.get("false"):
                 self.parse_calculate(expression.args["false"], config, arguments, primary_table, calculate_fields)
         elif isinstance(expression, sqlglot_expressions.Case):
             if expression.args.get("this"):
                 self.parse_calculate(expression.args["this"], config, arguments, primary_table, calculate_fields)
             if expression.args.get("default"):
                 self.parse_calculate(expression.args["default"], config, arguments, primary_table, calculate_fields)
-            if "ifs" in expression.args:
+            if expression.args.get("ifs"):
                 for case_expression in expression.args["ifs"]:
                     self.parse_calculate(case_expression, config, arguments, primary_table, calculate_fields)
         elif isinstance(expression, sqlglot_expressions.Paren):
             self.parse_calculate(expression.args["this"], config, arguments, primary_table, calculate_fields)
         elif self.is_column(expression, config, arguments):
             column = self.parse_column(expression, config, arguments)
             if not column["table_name"] or primary_table["table_name"] == column["table_name"]:
@@ -1664,20 +1797,22 @@
             calculate_fields.append(column)
         elif isinstance(expression, (sqlglot_expressions.Select, sqlglot_expressions.Star, sqlglot_expressions.Interval,
                                      sqlglot_expressions.DataType)):
             pass
         elif self.is_const(expression, config, arguments):
             pass
         else:
-            if "this" in expression.args and expression.args["this"]:
+            if not isinstance(expression, sqlglot_expressions.Expression):
+                return
+            if expression.args.get("this"):
                 self.parse_calculate(expression.args["this"], config, arguments, primary_table, calculate_fields)
-            if "expression" in expression.args and expression.args["expression"]:
+            if expression.args.get("expression"):
                 self.parse_calculate(expression.args["expression"], config, arguments, primary_table, calculate_fields)
-            if "expressions" in expression.args and expression.args["expressions"] and isinstance(expression.args["expressions"], list):
-                for arg_expression in expression.args.get("expressions", []):
+            if expression.args.get("expressions") and isinstance(expression.args["expressions"], list):
+                for arg_expression in expression.args["expressions"]:
                     self.parse_calculate(arg_expression, config, arguments, primary_table, calculate_fields)
             for arg_type in expression.arg_types:
                 if arg_type in ("this", "expression", "expressions"):
                     continue
                 if arg_type not in expression.args or not expression.args[arg_type]:
                     continue
                 if isinstance(expression.args[arg_type], list):
@@ -1695,15 +1830,15 @@
             if isinstance(child_expression, list):
                 for child_expression_item in child_expression:
                     self.parse_aggregate(child_expression_item, config, arguments, aggregate_expressions)
             else:
                 self.parse_aggregate(child_expression, config, arguments, aggregate_expressions)
 
     def parse_table(self, expression, config, arguments):
-        db_name = expression.args["db"].name if "db" in expression.args and expression.args["db"] else None
+        db_name = expression.args["db"].name if expression.args.get("db") else None
         if isinstance(expression.args["this"], sqlglot_expressions.Dot):
             def parse(expression):
                 return (parse(expression.args["this"]) if isinstance(expression.args["this"],
                                                                      sqlglot_expressions.Dot) else expression.args["this"].name) \
                        + "." + (parse(expression.args["expression"]) if isinstance(expression.args["expression"],
                                                                                    sqlglot_expressions.Dot) else expression.args["expression"].name)
             table_name = parse(expression.args["this"])
@@ -1722,17 +1857,17 @@
         try:
             start_index, end_index = origin_name.index("<"), origin_name.rindex(">")
             table_name = origin_name[:start_index]
             typing_options = origin_name[start_index + 1: end_index].split(",")
         except ValueError:
             table_name = origin_name
             typing_options = []
-        if "catalog" in expression.args and expression.args["catalog"]:
+        if expression.args.get("catalog"):
             db_name, table_name = expression.args["catalog"].name, ((db_name + ".") if db_name else "") + table_name
-        table_alias = expression.args["alias"].args["this"].name if "alias" in expression.args else None
+        table_alias = expression.args["alias"].args["this"].name if expression.args.get("alias") else None
 
         if table_name in ("_", "."):
             db_name, table_name = "-", "&1"
         elif table_name in (".txt", ".csv", ".json"):
             format_type = table_name[1:]
             database = None
             if "databases" not in config:
@@ -1791,15 +1926,15 @@
                 db_name = database["name"]
             else:
                 db_name = "--"
 
         return {
             "db": db_name,
             "name": table_name,
-            "table_name": table_alias if table_alias else table_name,
+            "table_name": table_alias if table_alias else ((db_name + "." + table_name if db_name else table_name)),
             "table_alias": table_alias,
             "origin_name": origin_name,
             "typing_options": typing_options,
         }
         
     def parse_column(self, expression, config, arguments):
         dot_keys = []
@@ -1811,33 +1946,39 @@
                     return dot_expression.args["this"]
                 column_expression = parse_dot(dot_expression.args["this"])
                 if dot_expression.args.get("expression"):
                     dot_keys.append(dot_expression.args["expression"].name)
                 return column_expression
             expression = parse_dot(expression)
 
-        table_name = expression.args["table"].name if "table" in expression.args else None
+        db_name = expression.args["db"].name if expression.args.get("db") else None
+        table_name = expression.args["table"].name if expression.args.get("table") else None
         column_name = expression.args["this"].name
         origin_name = self.mapping[column_name] if column_name in self.mapping else column_name
         try:
             start_index, end_index = origin_name.index("["), origin_name.rindex("]")
-            typing_filters = origin_name[start_index+1: end_index].split(";")
+            typing_filters = []
+            for typing_filter in origin_name[start_index+1: end_index].split(";"):
+                typing_filter = typing_filter.split(" ")
+                if not typing_filter or typing_filter[0].lower() not in self.TYPE_FILTERS:
+                    continue
+                typing_filters.append(" ".join([self.TYPE_FILTERS[typing_filter[0].lower()]] + typing_filter[1:]))
             column_name = origin_name[:start_index]
             typing_name = (column_name + "|" + typing_filters[0]) if typing_filters else column_name
         except ValueError:
             typing_filters = []
             column_name = origin_name
             typing_name = column_name
         try:
             start_index, end_index = origin_name.index("<"), origin_name.rindex(">")
             typing_options = origin_name[start_index+1: end_index].split(",")
         except ValueError:
             typing_options = []
         return {
-            "table_name": table_name,
+            "table_name": (db_name + "." + table_name) if db_name else table_name,
             "column_name": (column_name + "." + ".".join(dot_keys)) if dot_keys else column_name,
             "origin_name": origin_name,
             "typing_name": typing_name,
             "dot_keys": dot_keys,
             "typing_filters": typing_filters,
             "typing_options": typing_options,
             "expression": expression
@@ -1879,15 +2020,15 @@
             name = expression.args["this"].args["this"]
             if name in self.mapping:
                 name = self.mapping[name]
             try:
                 value = self.env_variables.get_value("@" + name)
                 if isinstance(value, (int, float, bool)):
                     typing_filter = str(type(value).__name__)
-                value_getter = EnvVariableGetter(self.env_variables, "@" + name)
+                value_getter = ["@current_env_variable::get_value", ["#const", "@" + name]]
             except KeyError:
                 raise SyncanySqlCompileException('unkonw parameter variable, related sql "%s"' % self.to_sql(expression))
         else:
             value = None
         return {
             "value": value,
             "value_getter": value_getter,
@@ -1998,14 +2139,406 @@
             try:
                 find_aggregate_calculater(calculater_name)
             except CalculaterUnknownException:
                 return False
             return True
         return False
 
+    def optimize_rewrite(self, expression, config, arguments):
+        from_expression = expression.args.get("from")
+        if not from_expression or not from_expression.expressions:
+            return expression
+        if len(from_expression.expressions) > 1:
+            expression = self.optimize_rewrite_multi_select(expression, config, arguments, from_expression)
+
+        if not expression.args.get("joins") or not expression.args.get("expressions"):
+            return expression
+        for join_expression in expression.args["joins"]:
+            if join_expression.side and join_expression.side.lower() == "right":
+                expression = self.optimize_rewrite_right_join(expression, config, arguments)
+                break
+        for join_expression in expression.args["joins"]:
+            if join_expression.kind and join_expression.kind.lower() == "inner":
+                expression = self.optimize_rewrite_inner_join(expression, config, arguments)
+                break
+
+        if len(expression.args["expressions"]) == 1:
+            if isinstance(expression.args["expressions"][0], sqlglot_expressions.Star):
+                return expression
+        aggregate_expressions = []
+        for select_expression in expression.args["expressions"]:
+            if isinstance(select_expression, sqlglot_expressions.Alias):
+                self.parse_aggregate(select_expression.args["this"], config, arguments, aggregate_expressions)
+            else:
+                self.parse_aggregate(select_expression, config, arguments, aggregate_expressions)
+        if aggregate_expressions or expression.args.get("group"):
+            expression = self.optimize_rewrite_aggregate(expression, config, arguments, aggregate_expressions)
+        return expression
+
+    def optimize_rewrite_multi_select(self, expression, config, arguments, from_expression):
+        primary_table = self.optimize_rewrite_parse_table(expression, config, arguments,
+                                                          expression.args["from"].expressions[0])
+        if not primary_table["table_name"]:
+            return expression
+
+        join_tables = []
+        for from_table_expression in from_expression.expressions[1:]:
+            join_table = {"table_name": self.optimize_rewrite_parse_table(expression, config, arguments,
+                                                                          from_table_expression)["table_name"],
+                          "related_tables": set([]), "on_expressions": [], "const_expressions": [],
+                          "calcuate_expressions": [], "join_expression": from_table_expression, "join_type": "left",
+                          "table_expression": from_table_expression}
+            if expression.args.get("where"):
+                self.optimize_rewrite_parse_condition(expression, config, arguments, primary_table, expression.args["where"].args["this"],
+                                                      join_table["table_name"], join_table["related_tables"],
+                                                      join_table["on_expressions"], join_table["const_expressions"],
+                                                      join_table["calcuate_expressions"])
+            join_tables.append(join_table)
+
+        sql = ["SELECT"]
+        if expression.args.get("distinct"):
+            sql.append(str(expression.args["distinct"]))
+        sql.append(", ".join([str(select_expression) for select_expression in expression.args["expressions"]]))
+        sql.append("FROM " + str(expression.args["from"].expressions[0]))
+        for join_table in join_tables:
+            sql.append("LEFT JOIN " + str(join_table["table_expression"]))
+            if join_table["on_expressions"]:
+                sql.append("ON " + " AND ".join([str(on_expression) for on_expression in join_table["on_expressions"]]))
+
+        where_expressions = []
+        for join_table in join_tables:
+            for const_expression in join_table["const_expressions"]:
+                if const_expression not in where_expressions:
+                    where_expressions.append(const_expression)
+        for join_table in join_tables:
+            for calcuate_expression in join_table["calcuate_expressions"]:
+                if calcuate_expression not in where_expressions:
+                    where_expressions.append(calcuate_expression)
+        if where_expressions:
+            sql.append("WHERE " + " AND ".join([("(" + str(where_expression) + ")")
+                                                if isinstance(where_expression, sqlglot_expressions.Or)
+                                                else str(where_expression)
+                                                for where_expression in where_expressions]))
+        if expression.args.get("group"):
+            sql.append(str(expression.args["group"]))
+        if expression.args.get("having"):
+            sql.append(str(expression.args["having"]))
+        if expression.args.get("order"):
+            sql.append(str(expression.args["order"]))
+        if expression.args.get("offset"):
+            offset_expression, limit_expression = expression.args.get("limit"), expression.args.get("offset")
+        else:
+            offset_expression, limit_expression = None, expression.args.get("limit")
+        if limit_expression:
+            offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
+            limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
+            sql.append(("LIMIT %d, %d" % (offset_value, limit_value)) if offset_value > 0 else ("LIMIT %d" % limit_value))
+        return maybe_parse(" ".join(sql), dialect=CompilerDialect)
+
+    def optimize_rewrite_right_join(self, expression, config, arguments):
+        primary_table = self.optimize_rewrite_parse_table(expression, config, arguments,
+                                                          expression.args["from"].expressions[0])
+        if not primary_table["table_name"]:
+            return expression
+        primary_table.update({"related_tables": set([]), "on_expressions": [], "const_expressions": [],
+                              "calcuate_expressions": [], "join_type": "primary",
+                              "table_expression": expression.args["from"].args["expressions"][0]})
+        if expression.args.get("where"):
+            self.optimize_rewrite_parse_condition(expression, config, arguments, primary_table,
+                                                  expression.args["where"].args["this"], primary_table["table_name"],
+                                                  primary_table["related_tables"], primary_table["calcuate_expressions"],
+                                                  primary_table["calcuate_expressions"], primary_table["calcuate_expressions"])
+        join_tables = []
+        for join_expression in expression.args["joins"]:
+            join_table = {"table_name": self.optimize_rewrite_parse_table(expression, config, arguments,
+                                                                          join_expression.args["this"])["table_name"],
+                          "related_tables": set([]), "on_expressions": [], "const_expressions": [],
+                          "calcuate_expressions": [], "join_expression": join_expression, "join_type": join_expression.side.lower(),
+                          "table_expression": join_expression.args["this"]}
+            if join_expression.args.get("on"):
+                self.optimize_rewrite_parse_condition(expression, config, arguments, primary_table, join_expression.args["on"],
+                                                      join_table["table_name"], join_table["related_tables"],
+                                                      join_table["on_expressions"], join_table["const_expressions"],
+                                                      join_table["calcuate_expressions"])
+            join_tables.append(join_table)
+
+        selected_table = primary_table
+        while True:
+            new_primary_table_table = None
+            for join_table in join_tables:
+                if join_table["join_type"] == "right" and selected_table["table_name"] in join_table["related_tables"]:
+                    new_primary_table_table = join_table
+            if not new_primary_table_table:
+                break
+            selected_table = new_primary_table_table
+        if selected_table["join_type"] == "primary":
+            return expression
+        join_tables.remove(selected_table)
+        join_tables.append(primary_table)
+
+        def resort_join_tables(current_table, on_expressions, join_tables):
+            related_tables = []
+            for table_name in current_table["related_tables"]:
+                if table_name not in join_tables:
+                    continue
+                related_table = join_tables.pop(table_name)
+                related_tables.append(related_table)
+                if related_table["join_type"] == "right":
+                    related_tables.extend(resort_join_tables(related_table, related_table["on_expressions"], join_tables))
+                    related_table["on_expressions"] = on_expressions
+                    related_table["join_type"] = "left"
+                else:
+                    related_table["on_expressions"].extend(on_expressions)
+            return related_tables
+        join_table_names = {join_table["table_name"]: join_table for join_table in join_tables}
+        join_tables = resort_join_tables(selected_table, selected_table["on_expressions"],
+                                         join_table_names) + list(join_table_names.values())
+
+        sql = ["SELECT"]
+        if expression.args.get("distinct"):
+            sql.append(str(expression.args["distinct"]))
+        sql.append(", ".join([str(select_expression) for select_expression in expression.args["expressions"]]))
+        sql.append("FROM " + str(selected_table["table_expression"]))
+        for join_table in join_tables:
+            if join_table["join_type"] == "right":
+                return expression
+            sql.append("LEFT JOIN " + str(join_table["table_expression"]))
+            on_expressions = join_table["on_expressions"] + join_table["const_expressions"]
+            if on_expressions:
+                sql.append("ON " + " AND ".join([str(on_expression) for on_expression in on_expressions]))
+
+        where_expressions = selected_table["const_expressions"] + primary_table["calcuate_expressions"] + selected_table["calcuate_expressions"]
+        if where_expressions:
+            sql.append("WHERE " + " AND ".join([("(" + str(where_expression) + ")")
+                                                if isinstance(where_expression, sqlglot_expressions.Or)
+                                                else str(where_expression)
+                                                for where_expression in where_expressions]))
+        if expression.args.get("group"):
+            sql.append(str(expression.args["group"]))
+        if expression.args.get("having"):
+            sql.append(str(expression.args["having"]))
+        if expression.args.get("order"):
+            sql.append(str(expression.args["order"]))
+        if expression.args.get("offset"):
+            offset_expression, limit_expression = expression.args.get("limit"), expression.args.get("offset")
+        else:
+            offset_expression, limit_expression = None, expression.args.get("limit")
+        if limit_expression:
+            offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
+            limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
+            sql.append(("LIMIT %d, %d" % (offset_value, limit_value)) if offset_value > 0 else ("LIMIT %d" % limit_value))
+        return maybe_parse(" ".join(sql), dialect=CompilerDialect)
+
+    def optimize_rewrite_inner_join(self, expression, config, arguments):
+        primary_table = self.optimize_rewrite_parse_table(expression, config, arguments,
+                                                          expression.args["from"].expressions[0])
+        if not primary_table["table_name"]:
+            return expression
+
+        inner_calculate_fields = []
+        for join_expression in expression.args["joins"]:
+            join_table = {"table_name": self.optimize_rewrite_parse_table(expression, config, arguments,
+                                                                          join_expression.args["this"])["table_name"],
+                          "related_tables": set([]), "on_expressions": [], "const_expressions": [],
+                          "calcuate_expressions": [], "join_expression": join_expression, "join_kind": join_expression.kind.lower(),
+                          "table_expression": join_expression.args["this"]}
+            if join_expression.args.get("on"):
+                self.optimize_rewrite_parse_condition(expression, config, arguments, primary_table,
+                                                      join_expression.args["on"],
+                                                      join_table["table_name"], join_table["related_tables"],
+                                                      join_table["on_expressions"], join_table["const_expressions"],
+                                                      join_table["calcuate_expressions"])
+            if primary_table["table_name"] in join_table["related_tables"]:
+                for on_expression in join_table["on_expressions"]:
+                    self.parse_calculate(on_expression, config, arguments, primary_table, inner_calculate_fields)
+        inner_calculate_fields = [calculate_field for calculate_field in inner_calculate_fields
+                                  if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]]
+        if not inner_calculate_fields:
+            return expression
+
+        sql = ["SELECT"]
+        if expression.args.get("distinct"):
+            sql.append(str(expression.args["distinct"]))
+        sql.append(", ".join([str(select_expression) for select_expression in expression.args["expressions"]]))
+        sql.append(str(expression.args["from"]))
+        for join_expression in expression.args["joins"]:
+            sql.append("LEFT JOIN " + str(join_expression.args["this"]))
+            if join_expression.args.get("on"):
+                sql.append("ON " + str(join_expression.args["on"]))
+
+        inner_condition_sql = " AND ".join(["`%s`.`%s` IS NOT NULL" % (calculate_field["table_name"], calculate_field["column_name"])
+                                            for calculate_field in inner_calculate_fields])
+        if expression.args.get("where"):
+            if isinstance(expression.args["where"].args["this"], sqlglot_expressions.Or):
+                sql.append("WHERE (" + str(expression.args["where"].args["this"]) + ") AND " + inner_condition_sql)
+            else:
+                sql.append("WHERE " + str(expression.args["where"].args["this"]) + " AND " + inner_condition_sql)
+        else:
+            sql.append("WHERE " + inner_condition_sql)
+        if expression.args.get("group"):
+            sql.append(str(expression.args["group"]))
+        if expression.args.get("having"):
+            sql.append(str(expression.args["having"]))
+        if expression.args.get("order"):
+            sql.append(str(expression.args["order"]))
+        if expression.args.get("offset"):
+            offset_expression, limit_expression = expression.args.get("limit"), expression.args.get("offset")
+        else:
+            offset_expression, limit_expression = None, expression.args.get("limit")
+        if limit_expression:
+            offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
+            limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
+            sql.append(
+                ("LIMIT %d, %d" % (offset_value, limit_value)) if offset_value > 0 else ("LIMIT %d" % limit_value))
+        return maybe_parse(" ".join(sql), dialect=CompilerDialect)
+
+    def optimize_rewrite_aggregate(self, expression, config, arguments, aggregate_expressions):
+        primary_table = self.optimize_rewrite_parse_table(expression, config, arguments,
+                                                          expression.args["from"].expressions[0])
+        if not primary_table["table_name"]:
+            return expression
+        aggregate_calculate_fields = []
+        for aggregate_expression in aggregate_expressions:
+            self.parse_calculate(aggregate_expression, config, arguments, primary_table, aggregate_calculate_fields)
+        aggregate_calculate_fields = [calculate_field for calculate_field in aggregate_calculate_fields
+                                      if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]]
+        if not aggregate_calculate_fields:
+            if not expression.args.get("group"):
+                return expression
+            group_calculate_fields = []
+            for group_expression in expression.args["group"].args["expressions"]:
+                self.parse_calculate(group_expression, config, arguments, primary_table, aggregate_calculate_fields)
+            group_calculate_fields = [calculate_field for calculate_field in group_calculate_fields
+                                      if calculate_field["table_name"] and calculate_field["table_name"] != primary_table["table_name"]]
+            if not group_calculate_fields:
+                return expression
+
+        sub_sql = ["SELECT"]
+        calculate_fields, sub_columns = [], []
+        for select_expression in expression.args["expressions"]:
+            if isinstance(select_expression, sqlglot_expressions.Column) \
+                    and isinstance(select_expression.args.get("this"), sqlglot_expressions.Star):
+                sub_columns.append(str(select_expression))
+            else:
+                self.parse_calculate(select_expression, config, arguments, primary_table, calculate_fields)
+        if expression.args.get("group"):
+            for group_expression in expression.args["group"].args["expressions"]:
+                self.parse_calculate(group_expression, config, arguments, primary_table, calculate_fields)
+        if expression.args.get("order"):
+            for order_expression in expression.args["order"].args["expressions"]:
+                self.parse_calculate(order_expression.args["this"], config, arguments, primary_table, calculate_fields)
+        for calculate_field in calculate_fields:
+            sub_column = "%s as `%s`" % (str(calculate_field["expression"]), calculate_field["column_name"])
+            if sub_column not in sub_columns:
+                sub_columns.append(sub_column)
+        sub_sql.append(", ".join(sub_columns))
+        sub_sql.append(str(expression.args["from"]))
+        for join_expression in expression.args["joins"]:
+            sub_sql.append(str(join_expression))
+        if expression.args.get("where"):
+            sub_sql.append(str(expression.args["where"]))
+
+        sql = ["SELECT"]
+        if expression.args.get("distinct"):
+            sql.append(str(expression.args["distinct"]))
+        sql.append(", ".join([str(self.optimize_rewrite_except_table(select_expression, config, arguments))
+                              for select_expression in expression.args["expressions"]]))
+        sql.append("FROM (%s) `__subquery_%s`" % (" ".join(sub_sql), str(uuid.uuid1().int)))
+        if expression.args.get("group"):
+            sql.append(str(self.optimize_rewrite_except_table(expression.args["group"], config, arguments)))
+        if expression.args.get("having"):
+            sql.append(str(expression.args["having"]))
+        if expression.args.get("order"):
+            sql.append(str(self.optimize_rewrite_except_table(expression.args["order"], config, arguments)))
+        if expression.args.get("offset"):
+            offset_expression, limit_expression = expression.args.get("limit"), expression.args.get("offset")
+        else:
+            offset_expression, limit_expression = None, expression.args.get("limit")
+        if limit_expression:
+            offset_value = max(int(offset_expression.args["expression"].args["this"]), 0) if offset_expression else 0
+            limit_value = max(int(limit_expression.args["expression"].args["this"]), 1)
+            sql.append(("LIMIT %d, %d" % (offset_value, limit_value)) if offset_value > 0 else ("LIMIT %d" % limit_value))
+        return maybe_parse(" ".join(sql), dialect=CompilerDialect)
+
+    def optimize_rewrite_parse_table(self, expression, config, arguments, table_expression):
+        table = {"table_name": None, "columns": {}}
+        if isinstance(table_expression, sqlglot_expressions.Table):
+            table["table_name"] = self.parse_table(table_expression, config, arguments)["table_name"]
+        elif isinstance(table_expression, sqlglot_expressions.Subquery):
+            if "alias" not in table_expression.args:
+                return table
+            table["table_name"] = table_expression.args["alias"].args["this"].name \
+                if table_expression.args.get("alias") else None
+        return table
+
+    def optimize_rewrite_parse_condition(self, expression, config, arguments, primary_table, condition_expression,
+                                         table_name, related_tables, on_expressions, const_expressions, calcuate_expressions):
+        if isinstance(condition_expression, sqlglot_expressions.And):
+            self.optimize_rewrite_parse_condition(expression, config, arguments, primary_table, condition_expression.args.get("this"),
+                                                  table_name, related_tables, on_expressions, const_expressions, calcuate_expressions)
+            self.optimize_rewrite_parse_condition(expression, config, arguments, primary_table, condition_expression.args.get("expression"),
+                                                  table_name, related_tables, on_expressions, const_expressions, calcuate_expressions)
+        elif isinstance(condition_expression, (sqlglot_expressions.EQ, sqlglot_expressions.NEQ, sqlglot_expressions.GT,
+                                               sqlglot_expressions.GTE, sqlglot_expressions.LT, sqlglot_expressions.LTE,
+                                               sqlglot_expressions.In)):
+            if condition_expression.args.get("expressions"):
+                left_expression, right_expression = condition_expression.args["this"], condition_expression.args[
+                    "expressions"]
+            elif condition_expression.args.get("query"):
+                left_expression, right_expression = condition_expression.args["this"], condition_expression.args[
+                    "query"]
+            else:
+                left_expression, right_expression = condition_expression.args["this"], condition_expression.args[
+                    "expression"]
+
+            condition_column, value_expression = None, left_expression
+            if self.is_column(left_expression, config, arguments):
+                left_column = self.parse_column(left_expression, config, arguments)
+                if left_column["table_name"] == table_name:
+                    condition_column, value_expression = left_column, right_expression
+            if not condition_column and self.is_column(right_expression, config, arguments):
+                right_column = self.parse_column(right_expression, config, arguments)
+                if right_column["table_name"] == table_name:
+                    condition_column, value_expression = right_column, left_expression
+            if not condition_column or isinstance(value_expression, (sqlglot_expressions.Select,
+                                                                     sqlglot_expressions.Subquery,
+                                                                     sqlglot_expressions.Union, list)):
+                calcuate_expressions.append(condition_expression)
+                return
+
+            calculate_fields = []
+            self.parse_calculate(value_expression, config, arguments, primary_table, calculate_fields)
+            if not calculate_fields:
+                const_expressions.append(condition_expression)
+                return
+            on_expressions.append(condition_expression)
+            for calculate_field in calculate_fields:
+                related_tables.add(calculate_field["table_name"])
+        else:
+            calcuate_expressions.append(condition_expression)
+
+    def optimize_rewrite_except_table(self, expression, config, arguments):
+        def parse_except_table(arg_expression):
+            if not isinstance(arg_expression, sqlglot_expressions.Expression):
+                return arg_expression
+            if isinstance(arg_expression, sqlglot_expressions.Column):
+                if arg_expression.args.get("db"):
+                    arg_expression.args["db"] = None
+                if arg_expression.args.get("table"):
+                    arg_expression.args["table"] = None
+                return arg_expression
+            for child_arg_expression in arg_expression.args.values():
+                if isinstance(child_arg_expression, list):
+                    for child_item_arg_expression in child_arg_expression:
+                        parse_except_table(child_item_arg_expression)
+                else:
+                    parse_except_table(child_arg_expression)
+            return arg_expression
+        return parse_except_table(expression)
+
     def to_sql(self, expression_sql):
         if not isinstance(expression_sql, str):
             expression_sql = str(expression_sql)
         parser = SqlParser(expression_sql)
         segments = []
         last_start_index, last_end_index = 0, 0
         while True:
```

### Comparing `syncanysql-0.1.3/syncanysql/config.py` & `syncanysql-0.1.4/syncanysql/config.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/executor.py` & `syncanysql-0.1.4/syncanysql/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -116,28 +116,30 @@
                 if isinstance(value, (list, tuple, set)):
                     return "(" + ",".join([format_variable_value(v) for v in value]) + ")"
                 return str(value)
             sql = sql.replace(variable, format_variable_value(variable_value))
         return sql
 
     def run(self, name, sqls):
+        self._thread_local.current_executor = self
         for sql in sqls:
             lineno = sql.lineno
             sql = self.compile_variable(str(sql))
             raw_sqls = RAW_SQL_RE.findall(sql)
             for raw, raw_name, _, raw_sql, _ in raw_sqls:
                 raw_name_info = raw_name.split(".")
                 if len(raw_name_info) != 2:
                     raise SyncanySqlCompileException("raw sql name error: %s", raw)
                 raw_sql = "set @config.databases." + raw_name_info[0] + ".virtual_views." + raw_name_info[1] + "='''\n" + raw_sql.strip() + "\n'''"
                 self.compile(name + "(" + str(lineno) + ")#set_virtual_view", raw_sql)
                 sql = sql.replace(raw, raw_name)
             self.compile(name + "(" + str(lineno) + ")", sql)
 
     def compile(self, name, sql):
+        self._thread_local.current_executor = self
         config = self.session_config.get()
         config["name"] = name
         try:
             compiler = Compiler(config, self.env_variables)
             arguments = {"@verbose": self.env_variables.get("@verbose", False), "@timeout": self.env_variables.get("@timeout", 0),
                          "@limit": self.env_variables.get("@limit", 0), "@batch": self.env_variables.get("@batch", 0),
                          "@streaming": self.env_variables.get("@streaming", False), "@recovery": self.env_variables.get("@recovery", False),
@@ -145,14 +147,15 @@
                          "@primary_order": False}
             tasker = compiler.compile(sql, arguments)
         finally:
             config["name"] = ""
         self.runners.extend(tasker.start(name, self, self.session_config, self.manager, arguments))
 
     def execute(self):
+        self._thread_local.current_executor = self
         while self.runners:
             self.tasker = self.runners.popleft()
             try:
                 exit_code = self.tasker.run(self, self.session_config, self.manager)
                 if exit_code is not None and exit_code != 0:
                     return exit_code
             finally:
```

### Comparing `syncanysql-0.1.3/syncanysql/main.py` & `syncanysql-0.1.4/syncanysql/main.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/parser.py` & `syncanysql-0.1.4/syncanysql/parser.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/prompt.py` & `syncanysql-0.1.4/syncanysql/prompt.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/taskers/delete.py` & `syncanysql-0.1.4/syncanysql/taskers/delete.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/taskers/execute.py` & `syncanysql-0.1.4/syncanysql/taskers/execute.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/taskers/explain.py` & `syncanysql-0.1.4/syncanysql/taskers/explain.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/taskers/into.py` & `syncanysql-0.1.4/syncanysql/taskers/into.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/taskers/query.py` & `syncanysql-0.1.4/syncanysql/taskers/query.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,19 +194,14 @@
         config = copy.deepcopy(self.config)
         config.pop("loader", None)
         config.pop("loader_arguments", None)
         config.update({
             "input": "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0],
             "output": self.config["output"],
             "querys": [],
-            "caches": [],
-            "imports": {},
-            "sources": {},
-            "defines": {},
-            "variables": {},
             "intercepts": [],
             "schema": {},
             "orders": [],
             "pipelines": [],
             "options": {},
             "dependencys": [],
             "states": [],
@@ -269,19 +264,14 @@
         config = copy.deepcopy(self.config)
         config.pop("loader", None)
         config.pop("loader_arguments", None)
         config.update({
             "input": "&.--." + subquery_name + "::" + self.config["output"].split("::")[-1].split(" ")[0],
             "output": self.config["output"],
             "querys": [],
-            "caches": [],
-            "imports": {},
-            "sources": {},
-            "defines": {},
-            "variables": {},
             "intercepts": [],
             "schema": {},
             "orders": [],
             "pipelines": [],
             "options": {},
             "dependencys": [],
             "states": [],
@@ -304,15 +294,15 @@
     def run_reduce(self, executor, session_config, manager, arguments, final_reduce=False):
         config, arguments = copy.deepcopy(self.reduce_config), copy.deepcopy(arguments)
         where_schema, aggregate = config.pop("where_schema", None), config.pop("aggregate", None)
         if final_reduce:
             config["schema"].pop("_aggregate_key_", None)
             if where_schema:
                 for key in where_schema:
-                    config.pop(key, None)
+                    config["schema"].pop(key, None)
             for key, column in config["schema"].items():
                 if key in aggregate["schema"] and aggregate["schema"][key]["final_value"]:
                     config["schema"][key] = aggregate["schema"][key]["final_value"]
                 else:
                     config["schema"][key] = "$." + key
             config["name"] = config["name"] + "#select@final"
         else:
```

### Comparing `syncanysql-0.1.3/syncanysql/taskers/set.py` & `syncanysql-0.1.4/syncanysql/taskers/set.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/taskers/show.py` & `syncanysql-0.1.4/syncanysql/taskers/show.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/taskers/use.py` & `syncanysql-0.1.4/syncanysql/taskers/use.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql/utils.py` & `syncanysql-0.1.4/syncanysql/utils.py`

 * *Files identical despite different names*

### Comparing `syncanysql-0.1.3/syncanysql.egg-info/PKG-INFO` & `syncanysql-0.1.4/syncanysql.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syncanysql
-Version: 0.1.3
+Version: 0.1.4
 Summary: Simple and easy-to-use sql execution engine
 Home-page: https://github.com/snower/syncany-sql
 Author: snower
 Author-email: sujian199@gmail.com
 License: MIT
 Description: # Syncany-SQL
         [![Tests](https://img.shields.io/github/actions/workflow/status/snower/syncany-sql/ci.yml?label=tests)](https://github.com/snower/syncany-sql/actions/workflows/ci.yml)
```

### Comparing `syncanysql-0.1.3/syncanysql.egg-info/SOURCES.txt` & `syncanysql-0.1.4/syncanysql.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 syncanysql.egg-info/dependency_links.txt
 syncanysql.egg-info/entry_points.txt
 syncanysql.egg-info/not-zip-safe
 syncanysql.egg-info/requires.txt
 syncanysql.egg-info/top_level.txt
 syncanysql/calculaters/__init__.py
 syncanysql/calculaters/aggregate_calculater.py
+syncanysql/calculaters/env_variable_calculater.py
 syncanysql/calculaters/mysql_calculater.py
 syncanysql/calculaters/mysql_funcs/__init__.py
 syncanysql/calculaters/mysql_funcs/datetime_funcs.py
 syncanysql/calculaters/mysql_funcs/json_funcs.py
 syncanysql/calculaters/mysql_funcs/number_funcs.py
 syncanysql/calculaters/mysql_funcs/string_funcs.py
 syncanysql/taskers/__init__.py
```

