# Comparing `tmp/refractio-2.0.1.tar.gz` & `tmp/refractio-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "refractio-2.0.1.tar", last modified: Tue May 23 11:24:37 2023, max compression
+gzip compressed data, was "refractio-2.0.2.tar", last modified: Fri May 26 11:31:36 2023, max compression
```

## Comparing `refractio-2.0.1.tar` & `refractio-2.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-23 11:24:37.214362 refractio-2.0.1/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7560 2023-05-23 11:24:37.213362 refractio-2.0.1/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6891 2023-05-23 10:14:58.000000 refractio-2.0.1/README.md
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-23 11:24:37.212361 refractio-2.0.1/refractio/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      319 2023-05-23 10:14:58.000000 refractio-2.0.1/refractio/__init__.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-23 10:14:58.000000 refractio-2.0.1/refractio/amazons3.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-23 10:14:58.000000 refractio-2.0.1/refractio/azure.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4707 2023-05-19 12:16:37.000000 refractio-2.0.1/refractio/hive.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3875 2023-05-19 12:16:37.000000 refractio-2.0.1/refractio/manager.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-19 12:16:26.000000 refractio-2.0.1/refractio/mysql.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13446 2023-05-19 12:16:26.000000 refractio-2.0.1/refractio/refractio.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-19 12:16:37.000000 refractio-2.0.1/refractio/sftp.py
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-19 12:16:26.000000 refractio-2.0.1/refractio/snowflake.py
-drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-23 11:24:37.213362 refractio-2.0.1/refractio.egg-info/
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7560 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/PKG-INFO
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      367 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/SOURCES.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/dependency_links.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/requires.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-23 11:24:37.000000 refractio-2.0.1/refractio.egg-info/top_level.txt
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-23 11:24:37.214362 refractio-2.0.1/setup.cfg
--rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1807 2023-05-23 10:14:58.000000 refractio-2.0.1/setup.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-26 11:31:36.375791 refractio-2.0.2/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7440 2023-05-26 11:31:36.375791 refractio-2.0.2/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     6771 2023-05-26 11:30:32.000000 refractio-2.0.2/README.md
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-26 11:31:36.373791 refractio-2.0.2/refractio/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      319 2023-05-23 10:14:58.000000 refractio-2.0.2/refractio/__init__.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3742 2023-05-23 10:14:58.000000 refractio-2.0.2/refractio/amazons3.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3611 2023-05-23 10:14:58.000000 refractio-2.0.2/refractio/azure.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4707 2023-05-19 12:16:37.000000 refractio-2.0.2/refractio/hive.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     3875 2023-05-19 12:16:37.000000 refractio-2.0.2/refractio/manager.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4407 2023-05-19 12:16:26.000000 refractio-2.0.2/refractio/mysql.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)    13446 2023-05-19 12:16:26.000000 refractio-2.0.2/refractio/refractio.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     4290 2023-05-19 12:16:37.000000 refractio-2.0.2/refractio/sftp.py
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     5335 2023-05-19 12:16:26.000000 refractio-2.0.2/refractio/snowflake.py
+drwxrwxr-x   0 developer-ro  (1005) developer-ro  (1005)        0 2023-05-26 11:31:36.375791 refractio-2.0.2/refractio.egg-info/
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     7440 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/PKG-INFO
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      367 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/SOURCES.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)        1 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/dependency_links.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)      483 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/requires.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       10 2023-05-26 11:31:36.000000 refractio-2.0.2/refractio.egg-info/top_level.txt
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)       38 2023-05-26 11:31:36.376791 refractio-2.0.2/setup.cfg
+-rw-rw-r--   0 developer-ro  (1005) developer-ro  (1005)     1807 2023-05-26 11:28:00.000000 refractio-2.0.2/setup.py
```

### Comparing `refractio-2.0.1/PKG-INFO` & `refractio-2.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.1
+Version: 2.0.2
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -63,16 +63,15 @@
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
 get_dataframe("dataset_name")
 
-# For reading data from any other RDBMS connection apart from (snowflake, hive and mysql) using connector-backend's package,
-# pip install git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git
+# For reading data from any other RDBMS connection apart from snowflake, hive or mysql please pip install mosaic-connector-python package.
 ```
 ## To read dataframe with filename from local storage -
 ```python
 from refracio import get_local_dataframe
 get_local_dataframe("local_file_name_with_absolute_path")
 ```
 ## To use snowflake related operations -
```

### Comparing `refractio-2.0.1/README.md` & `refractio-2.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -40,16 +40,15 @@
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
 get_dataframe("dataset_name")
 
-# For reading data from any other RDBMS connection apart from (snowflake, hive and mysql) using connector-backend's package,
-# pip install git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git
+# For reading data from any other RDBMS connection apart from snowflake, hive or mysql please pip install mosaic-connector-python package.
 ```
 ## To read dataframe with filename from local storage -
 ```python
 from refracio import get_local_dataframe
 get_local_dataframe("local_file_name_with_absolute_path")
 ```
 ## To use snowflake related operations -
```

### Comparing `refractio-2.0.1/refractio/amazons3.py` & `refractio-2.0.2/refractio/amazons3.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.1/refractio/azure.py` & `refractio-2.0.2/refractio/azure.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.1/refractio/hive.py` & `refractio-2.0.2/refractio/hive.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.1/refractio/manager.py` & `refractio-2.0.2/refractio/manager.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.1/refractio/mysql.py` & `refractio-2.0.2/refractio/mysql.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.1/refractio/refractio.py` & `refractio-2.0.2/refractio/refractio.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.1/refractio/sftp.py` & `refractio-2.0.2/refractio/sftp.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.1/refractio/snowflake.py` & `refractio-2.0.2/refractio/snowflake.py`

 * *Files identical despite different names*

### Comparing `refractio-2.0.1/refractio.egg-info/PKG-INFO` & `refractio-2.0.2/refractio.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: refractio
-Version: 2.0.1
+Version: 2.0.2
 Summary: REFRACT-IO: To read and write dataframe from different connectors.
 Home-page: UNKNOWN
 Author: Abhishek Chaurasia
 Author-email: <abhishek1.chaurasia@fosfor.com>
 License: UNKNOWN
 Project-URL: Product, https://www.fosfor.com/refract/
 Project-URL: Source, https://git.lti-aiq.in/refract-sdk/refract-sdk
@@ -63,16 +63,15 @@
 
 # Usage:
 ## To read dataframe with dataset name only -
 ```python
 from refractio import get_dataframe
 get_dataframe("dataset_name")
 
-# For reading data from any other RDBMS connection apart from (snowflake, hive and mysql) using connector-backend's package,
-# pip install git+https://gitlab+deploy-token-14:myUpFE_XRxShG53Hs6tV@git.lti-aiq.in/mosaic-decisions-2-0/mosaic-connector-python.git
+# For reading data from any other RDBMS connection apart from snowflake, hive or mysql please pip install mosaic-connector-python package.
 ```
 ## To read dataframe with filename from local storage -
 ```python
 from refracio import get_local_dataframe
 get_local_dataframe("local_file_name_with_absolute_path")
 ```
 ## To use snowflake related operations -
```

### Comparing `refractio-2.0.1/setup.py` & `refractio-2.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # read the contents of README file
 from pathlib import Path
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.md").read_text()
 
-VERSION = '2.0.1'
+VERSION = '2.0.2'
 DESCRIPTION = 'REFRACT-IO: To read and write dataframe from different connectors.'
 
 extras_require = {
     "all": [
         "snowflake-connector-python[pandas]==3.0.2",
         "boto3==1.26.116",
         "azure==4.0.0",
```

