# Comparing `tmp/qesdk-0.1.5.tar.gz` & `tmp/qesdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qesdk-0.1.5.tar", last modified: Fri May 26 12:43:35 2023, max compression
+gzip compressed data, was "qesdk-0.1.6.tar", last modified: Fri May 26 12:56:42 2023, max compression
```

## Comparing `qesdk-0.1.5.tar` & `qesdk-0.1.6.tar`

### file list

```diff
@@ -1,32 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.358160 qesdk-0.1.5/
--rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.5/LICENSE
--rw-rw-rw-   0        0        0       36 2022-09-22 03:32:43.000000 qesdk-0.1.5/MANIFEST.in
--rw-rw-rw-   0        0        0     6225 2023-05-26 12:43:35.358160 qesdk-0.1.5/PKG-INFO
--rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.5/README.md
--rw-rw-rw-   0        0        0      751 2023-05-26 12:41:35.000000 qesdk-0.1.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 12:43:35.358160 qesdk-0.1.5/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.339160 qesdk-0.1.5/src/
-drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.346160 qesdk-0.1.5/src/qesdk/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.5/src/qesdk/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.5/src/qesdk/aio_api.py
--rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.5/src/qesdk/api.py
--rw-rw-rw-   0        0        0     6805 2023-05-26 12:41:18.000000 qesdk-0.1.5/src/qesdk/client.py
--rw-rw-rw-   0        0        0      237 2023-05-26 12:40:26.000000 qesdk-0.1.5/src/qesdk/config.py
--rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.5/src/qesdk/qedata.thrift
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.5/src/qesdk/utils.py
-drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.351163 qesdk-0.1.5/src/qesdk.egg-info/
--rw-rw-rw-   0        0        0     6225 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       24 2023-05-26 12:43:35.000000 qesdk-0.1.5/src/qesdk.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-26 12:43:35.357159 qesdk-0.1.5/src/qesdk2/
--rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.5/src/qesdk2/__init__.py
--rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.5/src/qesdk2/aio_api.py
--rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.5/src/qesdk2/api.py
--rw-rw-rw-   0        0        0     4929 2023-05-15 05:31:36.000000 qesdk-0.1.5/src/qesdk2/client.py
--rw-rw-rw-   0        0        0     5339 2023-05-15 05:35:29.000000 qesdk-0.1.5/src/qesdk2/clienttest.py
--rw-rw-rw-   0        0        0      183 2023-05-19 14:14:05.000000 qesdk-0.1.5/src/qesdk2/config.py
--rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.5/src/qesdk2/utils.py
--rw-rw-rw-   0        0        0     2092 2023-05-24 14:13:05.000000 qesdk-0.1.5/src/test.py
--rw-rw-rw-   0        0        0     2219 2023-05-26 11:43:19.000000 qesdk-0.1.5/src/test2.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:56:42.610748 qesdk-0.1.6/
+-rw-rw-rw-   0        0        0     1087 2022-09-03 13:01:01.000000 qesdk-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0       38 2023-05-26 12:51:28.000000 qesdk-0.1.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     6225 2023-05-26 12:56:42.610748 qesdk-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     4459 2022-11-07 05:15:24.000000 qesdk-0.1.6/README.md
+-rw-rw-rw-   0        0        0      751 2023-05-26 12:56:27.000000 qesdk-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 12:56:42.610748 qesdk-0.1.6/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-26 12:56:42.594750 qesdk-0.1.6/src/
+drwxrwxrwx   0        0        0        0 2023-05-26 12:56:42.604747 qesdk-0.1.6/src/qesdk/
+-rw-rw-rw-   0        0        0      511 2023-02-01 03:17:15.000000 qesdk-0.1.6/src/qesdk/__init__.py
+-rw-rw-rw-   0        0        0     4561 2022-09-22 05:16:12.000000 qesdk-0.1.6/src/qesdk/aio_api.py
+-rw-rw-rw-   0        0        0    29263 2023-04-21 15:11:52.000000 qesdk-0.1.6/src/qesdk/api.py
+-rw-rw-rw-   0        0        0     6805 2023-05-26 12:56:12.000000 qesdk-0.1.6/src/qesdk/client.py
+-rw-rw-rw-   0        0        0      237 2023-05-26 12:40:26.000000 qesdk-0.1.6/src/qesdk/config.py
+-rw-rw-rw-   0        0        0      599 2022-10-09 06:46:09.000000 qesdk-0.1.6/src/qesdk/qedata.thrift
+-rw-rw-rw-   0        0        0      793 2022-10-09 07:50:13.000000 qesdk-0.1.6/src/qesdk/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-26 12:56:42.609749 qesdk-0.1.6/src/qesdk.egg-info/
+-rw-rw-rw-   0        0        0     6225 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      351 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       88 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-26 12:56:42.000000 qesdk-0.1.6/src/qesdk.egg-info/top_level.txt
```

### Comparing `qesdk-0.1.5/LICENSE` & `qesdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.5/PKG-INFO` & `qesdk-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `qesdk-0.1.5/README.md` & `qesdk-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.5/pyproject.toml` & `qesdk-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qesdk"
-version = "0.1.5"
+version = "0.1.6"
 authors = [
   { name="Scott Zhang", email="scott2011@qq.com" },
 ]
 description = "Quantease SDK for quants"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `qesdk-0.1.5/src/qesdk/aio_api.py` & `qesdk-0.1.6/src/qesdk/aio_api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.5/src/qesdk/api.py` & `qesdk-0.1.6/src/qesdk/api.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.5/src/qesdk/client.py` & `qesdk-0.1.6/src/qesdk/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     server_index = 0
 except ImportError:
     server_config = {'host' : '192.168.123.199',
                      'port' : 6001}  
     
 
 
-__version__='0.1.5'
+__version__='0.1.6'
 
 thrift_path = path.join(sys.modules["ROOT_DIR"], "qedata.thrift")
 thrift_path = path.abspath(thrift_path)
 #print(thrift_path)
 qedata_thrift = thriftpy2.load(thrift_path, module_name="qedata_thrift")
 loop = asyncio.get_event_loop()
 def setTimeout(client, timeout):
```

### Comparing `qesdk-0.1.5/src/qesdk/qedata.thrift` & `qesdk-0.1.6/src/qesdk/qedata.thrift`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.5/src/qesdk/utils.py` & `qesdk-0.1.6/src/qesdk/utils.py`

 * *Files identical despite different names*

### Comparing `qesdk-0.1.5/src/qesdk.egg-info/PKG-INFO` & `qesdk-0.1.6/src/qesdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qesdk
-Version: 0.1.5
+Version: 0.1.6
 Summary: Quantease SDK for quants
 Author-email: Scott Zhang <scott2011@qq.com>
 License: MIT License
         
         Copyright (c) 2022 quantease
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

