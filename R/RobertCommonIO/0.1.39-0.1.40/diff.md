# Comparing `tmp/RobertCommonIO-0.1.39.tar.gz` & `tmp/RobertCommonIO-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobertCommonIO-0.1.39.tar", last modified: Thu May 25 09:55:57 2023, max compression
+gzip compressed data, was "RobertCommonIO-0.1.40.tar", last modified: Fri May 26 06:49:07 2023, max compression
```

## Comparing `RobertCommonIO-0.1.39.tar` & `RobertCommonIO-0.1.40.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 09:55:57.824900 RobertCommonIO-0.1.39/
--rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.39/LICENSE
--rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.39/MANIFEST.in
--rw-rw-rw-   0        0        0     1724 2023-05-25 09:55:57.823881 RobertCommonIO-0.1.39/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2022-01-13 06:37:11.000000 RobertCommonIO-0.1.39/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 09:55:57.774834 RobertCommonIO-0.1.39/RobertCommonIO.egg-info/
--rw-rw-rw-   0        0        0     1724 2023-05-25 09:55:57.000000 RobertCommonIO-0.1.39/RobertCommonIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1663 2023-05-25 09:55:57.000000 RobertCommonIO-0.1.39/RobertCommonIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 09:55:57.000000 RobertCommonIO-0.1.39/RobertCommonIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      255 2023-05-25 09:55:57.000000 RobertCommonIO-0.1.39/RobertCommonIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-25 09:55:57.000000 RobertCommonIO-0.1.39/RobertCommonIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      281 2023-05-25 09:15:35.000000 RobertCommonIO-0.1.39/requirements.txt
-drwxrwxrwx   0        0        0        0 2023-05-25 09:55:57.775834 RobertCommonIO-0.1.39/robertcommonio/
--rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.39/robertcommonio/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:55:57.776835 RobertCommonIO-0.1.39/robertcommonio/system/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.39/robertcommonio/system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:55:57.801780 RobertCommonIO-0.1.39/robertcommonio/system/io/
--rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/__init__.py
--rw-rw-rw-   0        0        0    19281 2023-04-04 06:29:48.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/data_storage.py
--rw-rw-rw-   0        0        0     1051 2022-11-22 07:37:12.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/email.py
--rw-rw-rw-   0        0        0     7388 2023-04-19 09:38:00.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/file.py
--rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/ftp.py
--rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/http.py
--rw-rw-rw-   0        0        0     3334 2023-01-31 09:43:08.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/ini.py
--rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/license.py
--rw-rw-rw-   0        0        0    27197 2023-05-18 07:23:32.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/mongo.py
--rw-rw-rw-   0        0        0     6883 2023-05-16 09:34:00.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/mqtt.py
--rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/mysql.py
--rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/oss.py
--rw-rw-rw-   0        0        0     7191 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/rabitmq.py
--rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/redis.py
--rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/redis_cache.py
--rw-rw-rw-   0        0        0     9779 2023-05-25 09:55:20.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/response.py
--rw-rw-rw-   0        0        0    37639 2023-02-23 08:23:07.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/socket.py
--rw-rw-rw-   0        0        0     7211 2023-01-19 14:33:43.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/sqlalche.py
--rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/transport.py
--rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.39/robertcommonio/system/io/version.py
--rw-rw-rw-   0        0        0       42 2023-05-25 09:55:57.824900 RobertCommonIO-0.1.39/setup.cfg
--rw-rw-rw-   0        0        0     3869 2023-05-25 09:15:35.000000 RobertCommonIO-0.1.39/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:55:57.803781 RobertCommonIO-0.1.39/tests/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.39/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:55:57.803781 RobertCommonIO-0.1.39/tests/test_system/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.39/tests/test_system/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-25 09:55:57.822391 RobertCommonIO-0.1.39/tests/test_system/test_io/
--rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/__init__.py
--rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test.py
--rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_data_storage.py
--rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_file.py
--rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_ftp.py
--rw-rw-rw-   0        0        0      399 2022-12-14 07:23:38.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_http.py
--rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_ini.py
--rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_license.py
--rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_mongo.py
--rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_mqtt.py
--rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_oracle.py
--rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_rabbitmq.py
--rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_socket.py
--rw-rw-rw-   0        0        0     3490 2023-04-23 02:27:39.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_sqlalche.py
--rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.39/tests/test_system/test_io/test_transport.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:49:07.846091 RobertCommonIO-0.1.40/
+-rw-rw-rw-   0        0        0     1067 2021-08-09 02:56:17.000000 RobertCommonIO-0.1.40/LICENSE
+-rw-rw-rw-   0        0        0       44 2021-08-09 07:19:42.000000 RobertCommonIO-0.1.40/MANIFEST.in
+-rw-rw-rw-   0        0        0     1724 2023-05-26 06:49:07.846091 RobertCommonIO-0.1.40/PKG-INFO
+-rw-rw-rw-   0        0        0     1051 2022-01-13 06:37:11.000000 RobertCommonIO-0.1.40/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 06:49:07.799050 RobertCommonIO-0.1.40/RobertCommonIO.egg-info/
+-rw-rw-rw-   0        0        0     1724 2023-05-26 06:49:07.000000 RobertCommonIO-0.1.40/RobertCommonIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1663 2023-05-26 06:49:07.000000 RobertCommonIO-0.1.40/RobertCommonIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 06:49:07.000000 RobertCommonIO-0.1.40/RobertCommonIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      255 2023-05-26 06:49:07.000000 RobertCommonIO-0.1.40/RobertCommonIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-26 06:49:07.000000 RobertCommonIO-0.1.40/RobertCommonIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      281 2023-05-25 09:15:35.000000 RobertCommonIO-0.1.40/requirements.txt
+drwxrwxrwx   0        0        0        0 2023-05-26 06:49:07.800050 RobertCommonIO-0.1.40/robertcommonio/
+-rw-rw-rw-   0        0        0        2 2021-08-09 03:27:49.000000 RobertCommonIO-0.1.40/robertcommonio/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:49:07.801051 RobertCommonIO-0.1.40/robertcommonio/system/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.40/robertcommonio/system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:49:07.823645 RobertCommonIO-0.1.40/robertcommonio/system/io/
+-rw-rw-rw-   0        0        0        0 2021-10-22 09:02:53.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/__init__.py
+-rw-rw-rw-   0        0        0    19281 2023-04-04 06:29:48.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/data_storage.py
+-rw-rw-rw-   0        0        0     1051 2022-11-22 07:37:12.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/email.py
+-rw-rw-rw-   0        0        0     7388 2023-04-19 09:38:00.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/file.py
+-rw-rw-rw-   0        0        0     6347 2022-10-09 08:05:49.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/ftp.py
+-rw-rw-rw-   0        0        0    10214 2023-02-21 02:59:34.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/http.py
+-rw-rw-rw-   0        0        0     3334 2023-01-31 09:43:08.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/ini.py
+-rw-rw-rw-   0        0        0     6566 2022-11-24 06:58:34.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/license.py
+-rw-rw-rw-   0        0        0    27197 2023-05-18 07:23:32.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/mongo.py
+-rw-rw-rw-   0        0        0     6883 2023-05-16 09:34:00.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/mqtt.py
+-rw-rw-rw-   0        0        0     6535 2023-01-04 05:46:19.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/mysql.py
+-rw-rw-rw-   0        0        0     3900 2022-11-22 07:50:13.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/oss.py
+-rw-rw-rw-   0        0        0     7191 2022-11-22 07:56:12.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/rabitmq.py
+-rw-rw-rw-   0        0        0    11702 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/redis.py
+-rw-rw-rw-   0        0        0     2267 2022-10-09 08:16:48.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/redis_cache.py
+-rw-rw-rw-   0        0        0     9779 2023-05-25 09:55:20.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/response.py
+-rw-rw-rw-   0        0        0    37639 2023-02-23 08:23:07.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/socket.py
+-rw-rw-rw-   0        0        0     7249 2023-05-26 06:26:38.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/sqlalche.py
+-rw-rw-rw-   0        0        0     6710 2022-11-22 07:58:41.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/transport.py
+-rw-rw-rw-   0        0        0      725 2022-12-14 08:37:33.000000 RobertCommonIO-0.1.40/robertcommonio/system/io/version.py
+-rw-rw-rw-   0        0        0       42 2023-05-26 06:49:07.846091 RobertCommonIO-0.1.40/setup.cfg
+-rw-rw-rw-   0        0        0     3869 2023-05-26 06:47:06.000000 RobertCommonIO-0.1.40/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:49:07.824651 RobertCommonIO-0.1.40/tests/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:06:01.000000 RobertCommonIO-0.1.40/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:49:07.824651 RobertCommonIO-0.1.40/tests/test_system/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:49:45.000000 RobertCommonIO-0.1.40/tests/test_system/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 06:49:07.844092 RobertCommonIO-0.1.40/tests/test_system/test_io/
+-rw-rw-rw-   0        0        0        0 2021-07-27 06:50:10.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/__init__.py
+-rw-rw-rw-   0        0        0     1322 2023-01-04 02:27:37.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test.py
+-rw-rw-rw-   0        0        0     1570 2023-01-05 05:43:17.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_data_storage.py
+-rw-rw-rw-   0        0        0     3985 2022-07-11 02:23:20.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_file.py
+-rw-rw-rw-   0        0        0      978 2022-05-25 08:49:17.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_ftp.py
+-rw-rw-rw-   0        0        0      399 2022-12-14 07:23:38.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_http.py
+-rw-rw-rw-   0        0        0      413 2022-01-13 06:50:54.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_ini.py
+-rw-rw-rw-   0        0        0     1187 2023-03-09 08:37:11.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_license.py
+-rw-rw-rw-   0        0        0     3141 2023-04-04 06:18:30.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_mongo.py
+-rw-rw-rw-   0        0        0     1582 2022-04-20 08:37:11.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_mqtt.py
+-rw-rw-rw-   0        0        0    10544 2021-12-24 13:47:06.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_oracle.py
+-rw-rw-rw-   0        0        0     1028 2022-09-07 06:12:44.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_rabbitmq.py
+-rw-rw-rw-   0        0        0     4221 2022-10-09 07:39:57.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_socket.py
+-rw-rw-rw-   0        0        0     3490 2023-04-23 02:27:39.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_sqlalche.py
+-rw-rw-rw-   0        0        0     1389 2022-10-13 09:07:08.000000 RobertCommonIO-0.1.40/tests/test_system/test_io/test_transport.py
```

### Comparing `RobertCommonIO-0.1.39/LICENSE` & `RobertCommonIO-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/PKG-INFO` & `RobertCommonIO-0.1.40/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.39
+Version: 0.1.40
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.39/README.md` & `RobertCommonIO-0.1.40/README.md`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/RobertCommonIO.egg-info/PKG-INFO` & `RobertCommonIO-0.1.40/RobertCommonIO.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobertCommonIO
-Version: 0.1.39
+Version: 0.1.40
 Summary: Robert Common IO Library
 Home-page: https://github.com/hun0423/RobertCommonIO
 Author: Robert0423
 Author-email: 851010070@qq.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `RobertCommonIO-0.1.39/RobertCommonIO.egg-info/SOURCES.txt` & `RobertCommonIO-0.1.40/RobertCommonIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/data_storage.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/data_storage.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/email.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/email.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/file.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/ftp.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/http.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/http.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/ini.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/ini.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/license.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/mongo.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/mongo.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/mqtt.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/mysql.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/mysql.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/oss.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/oss.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/rabitmq.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/rabitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/redis.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/redis.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/redis_cache.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/redis_cache.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/response.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/response.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/socket.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/sqlalche.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/sqlalche.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,24 +117,24 @@
         if action in ['replace', 'append']:
             return f"insert into {table_name} ({', '.join(filed_format.format(k) for k in colums)}) VALUES ({', '.join(':{}'.format(k) for k in colums)})"
         elif action == 'update':
             return f"update {table_name} set {', '.join(filed_format1.format(k, k) for k in colums)} where {', '.join(filed_format1.format(k, k) for k in filter_column)}"
         elif action == 'delete':
             return f"delete from {table_name} where {', '.join(filed_format1.format(k, k) for k in filter_column)}"
 
-    def generate_sql_cmds(self, table_name: str, records: list, action: str = 'replace', colums: list = None, filter_column: list = None):
+    def generate_sql_cmds(self, table_name: str, records: list, action: str = 'replace', colums: list = None, filter_column: list = None, add_syntax: bool = False):
         cmds = []
         if len(records) > 0:
             if action == 'replace':
                 if filter_column is None:
                     cmds.append((f"delete from {table_name}", None))
                 else:
                     cmds.append((self.generate_sql_format(table_name, 'delete', None, filter_column), records))
 
-            cmds.append((self.generate_sql_format(table_name, action, records[0].keys() if colums is None else colums, filter_column), records))
+            cmds.append((self.generate_sql_format(table_name, action, records[0].keys() if colums is None else colums, filter_column, add_syntax), records))
         return cmds
 
     def copy_table_struct(self, engine_name: str, table_name: str, new_table_name: str):
         crate_sql = self.get_table_struct(engine_name, table_name)
         if crate_sql is not None:
             return self.execute_sql(engine_name, crate_sql.replace("CREATE TABLE " + table_name, "CREATE TABLE if not exists " + new_table_name))
```

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/transport.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/transport.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/robertcommonio/system/io/version.py` & `RobertCommonIO-0.1.40/robertcommonio/system/io/version.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/setup.py` & `RobertCommonIO-0.1.40/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 # Package meta-data.
 NAME = 'RobertCommonIO'
 DESCRIPTION = 'Robert Common IO Library'
 URL = 'https://github.com/hun0423/RobertCommonIO'
 EMAIL = '851010070@qq.com'
 AUTHOR = 'Robert0423'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.39'
-DATE = '2023-05-25'
+VERSION = '0.1.40'
+DATE = '2023-05-26'
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
 # The rest you shouldn't have to touch too much :)
```

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_data_storage.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_data_storage.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_file.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_file.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_ftp.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_ftp.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_license.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_license.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_mongo.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_mongo.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_mqtt.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_mqtt.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_oracle.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_oracle.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_rabbitmq.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_rabbitmq.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_socket.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_socket.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_sqlalche.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_sqlalche.py`

 * *Files identical despite different names*

### Comparing `RobertCommonIO-0.1.39/tests/test_system/test_io/test_transport.py` & `RobertCommonIO-0.1.40/tests/test_system/test_io/test_transport.py`

 * *Files identical despite different names*

