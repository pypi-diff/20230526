# Comparing `tmp/Log_Api-0.0.7.tar.gz` & `tmp/Log_Api-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Log_Api-0.0.7.tar", last modified: Thu May 18 20:03:40 2023, max compression
+gzip compressed data, was "Log_Api-0.0.8.tar", last modified: Fri May 26 15:17:05 2023, max compression
```

## Comparing `Log_Api-0.0.7.tar` & `Log_Api-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 20:03:40.456967 Log_Api-0.0.7/
-drwxrwxrwx   0        0        0        0 2023-05-18 20:03:40.394709 Log_Api-0.0.7/Log_Api/
-drwxrwxrwx   0        0        0        0 2023-05-18 20:03:40.422061 Log_Api-0.0.7/Log_Api/Class/
--rw-rw-rw-   0        0        0     2050 2023-05-16 21:33:41.000000 Log_Api-0.0.7/Log_Api/Class/Database.py
--rw-rw-rw-   0        0        0     3212 2023-05-15 16:56:09.000000 Log_Api-0.0.7/Log_Api/Class/LogAPI.py
--rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.7/Log_Api/Class/__init__.py
--rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.7/Log_Api/Class/response..py
-drwxrwxrwx   0        0        0        0 2023-05-18 20:03:40.425052 Log_Api-0.0.7/Log_Api/Models/
--rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.7/Log_Api/Models/LogAPI.py
--rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.7/Log_Api/Models/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 20:03:40.454973 Log_Api-0.0.7/Log_Api/Utils/
--rw-rw-rw-   0        0        0     8335 2023-05-18 17:25:34.000000 Log_Api-0.0.7/Log_Api/Utils/Aws.py
--rw-rw-rw-   0        0        0     3494 2023-05-15 20:49:03.000000 Log_Api-0.0.7/Log_Api/Utils/ModelsType.py
--rw-rw-rw-   0        0        0     4104 2023-05-18 20:02:31.000000 Log_Api-0.0.7/Log_Api/Utils/Response.py
--rw-rw-rw-   0        0        0     1181 2023-05-15 20:49:32.000000 Log_Api-0.0.7/Log_Api/Utils/Template.py
--rw-rw-rw-   0        0        0      117 2023-05-15 20:43:57.000000 Log_Api-0.0.7/Log_Api/Utils/__init__.py
--rw-rw-rw-   0        0        0       47 2023-05-15 20:44:12.000000 Log_Api-0.0.7/Log_Api/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 20:03:40.415078 Log_Api-0.0.7/Log_Api.egg-info/
--rw-rw-rw-   0        0        0      284 2023-05-18 20:03:40.000000 Log_Api-0.0.7/Log_Api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      530 2023-05-18 20:03:40.000000 Log_Api-0.0.7/Log_Api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 20:03:40.000000 Log_Api-0.0.7/Log_Api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.7/Log_Api.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       44 2023-05-18 20:03:40.000000 Log_Api-0.0.7/Log_Api.egg-info/requires.txt
--rw-rw-rw-   0        0        0       31 2023-05-18 20:03:40.000000 Log_Api-0.0.7/Log_Api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      284 2023-05-18 20:03:40.455969 Log_Api-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.7/README.md
--rw-rw-rw-   0        0        0    14763 2023-05-18 20:03:36.000000 Log_Api-0.0.7/aws_handler_decorators.py
--rw-rw-rw-   0        0        0       42 2023-05-18 20:03:40.456967 Log_Api-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      665 2023-05-17 17:23:19.000000 Log_Api-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:17:05.322738 Log_Api-0.0.8/
+drwxrwxrwx   0        0        0        0 2023-05-26 15:17:05.285831 Log_Api-0.0.8/Log_Api/
+drwxrwxrwx   0        0        0        0 2023-05-26 15:17:05.310765 Log_Api-0.0.8/Log_Api/Class/
+-rw-rw-rw-   0        0        0     2050 2023-05-16 21:33:41.000000 Log_Api-0.0.8/Log_Api/Class/Database.py
+-rw-rw-rw-   0        0        0     3191 2023-05-18 21:24:45.000000 Log_Api-0.0.8/Log_Api/Class/LogAPI.py
+-rw-rw-rw-   0        0        0       73 2023-05-15 16:56:09.000000 Log_Api-0.0.8/Log_Api/Class/__init__.py
+-rw-rw-rw-   0        0        0     4071 2023-05-15 16:56:09.000000 Log_Api-0.0.8/Log_Api/Class/response..py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:17:05.313762 Log_Api-0.0.8/Log_Api/Models/
+-rw-rw-rw-   0        0        0     2056 2023-05-15 16:56:09.000000 Log_Api-0.0.8/Log_Api/Models/LogAPI.py
+-rw-rw-rw-   0        0        0       26 2023-05-15 16:56:09.000000 Log_Api-0.0.8/Log_Api/Models/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:17:05.320747 Log_Api-0.0.8/Log_Api/Utils/
+-rw-rw-rw-   0        0        0     9276 2023-05-26 15:15:57.000000 Log_Api-0.0.8/Log_Api/Utils/Aws.py
+-rw-rw-rw-   0        0        0     3494 2023-05-15 20:49:03.000000 Log_Api-0.0.8/Log_Api/Utils/ModelsType.py
+-rw-rw-rw-   0        0        0     4104 2023-05-18 20:02:31.000000 Log_Api-0.0.8/Log_Api/Utils/Response.py
+-rw-rw-rw-   0        0        0     1181 2023-05-15 20:49:32.000000 Log_Api-0.0.8/Log_Api/Utils/Template.py
+-rw-rw-rw-   0        0        0      117 2023-05-15 20:43:57.000000 Log_Api-0.0.8/Log_Api/Utils/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-05-15 20:44:12.000000 Log_Api-0.0.8/Log_Api/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:17:05.304796 Log_Api-0.0.8/Log_Api.egg-info/
+-rw-rw-rw-   0        0        0      284 2023-05-26 15:17:05.000000 Log_Api-0.0.8/Log_Api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      530 2023-05-26 15:17:05.000000 Log_Api-0.0.8/Log_Api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:17:05.000000 Log_Api-0.0.8/Log_Api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-15 17:00:00.000000 Log_Api-0.0.8/Log_Api.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       44 2023-05-26 15:17:05.000000 Log_Api-0.0.8/Log_Api.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       31 2023-05-26 15:17:05.000000 Log_Api-0.0.8/Log_Api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      284 2023-05-26 15:17:05.321737 Log_Api-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     3618 2023-05-15 16:56:09.000000 Log_Api-0.0.8/README.md
+-rw-rw-rw-   0        0        0    14763 2023-05-26 15:16:57.000000 Log_Api-0.0.8/aws_handler_decorators.py
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:17:05.323731 Log_Api-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      665 2023-05-17 17:23:19.000000 Log_Api-0.0.8/setup.py
```

### Comparing `Log_Api-0.0.7/Log_Api/Class/Database.py` & `Log_Api-0.0.8/Log_Api/Class/Database.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.7/Log_Api/Class/LogAPI.py` & `Log_Api-0.0.8/Log_Api/Class/LogAPI.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,14 @@
     """
     Log response
     request: SQLAlchemy object
         Object of the request to log
     response: dict
         Response of the API
     """
-    print(response)
     session = Database('dbw').session
     try:
         if response:
             log_api = session.merge(request)
             log_api.STATUS_CODE = response.get('statusCode')
             log_api.HEADERS_RESPONSE = dumps(response.get('headers', None))
             log_api.BODY_RESPONSE = dumps(response.get('body', None))
```

### Comparing `Log_Api-0.0.7/Log_Api/Class/response..py` & `Log_Api-0.0.8/Log_Api/Class/response..py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.7/Log_Api/Models/LogAPI.py` & `Log_Api-0.0.8/Log_Api/Models/LogAPI.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.7/Log_Api/Utils/Aws.py` & `Log_Api-0.0.8/Log_Api/Utils/Aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import json
 import boto3
 import base64
 import logging
+from datetime import datetime
 from botocore.exceptions import NoCredentialsError
 from botocore.exceptions import ClientError
 
 class Aws:
 
     def __init__(self, secret_name: str):
         self.__secret_name = secret_name
@@ -184,14 +185,39 @@
         except FileNotFoundError:
             raise ValueError("Error al eliminar el archivo")
         except NoCredentialsError:
             raise ValueError("Credenciales invalidas")
         except Exception as e:
             raise e
     
+    def upload_fileobj(self, file_route, filename):
+        """
+        Subir archivo a S3
+        :param: file 
+            archivo a subir (BufferedReader)
+        :param: filename
+            nombre del archivo, debe tener esta estructura:
+                carpeta/nombre_archivo.extension
+        """
+        try:
+            filename = f"{datetime.now().strftime('%d-%m-%Y')}_{filename}"
+            secrets = self.get_secret()
+
+            bucket_name = secrets["bucket_name"]
+
+            s3_client = boto3.client('s3')
+            with open(file_route, 'rb') as file:
+                s3_client.upload_fileobj(file, bucket_name, filename)
+        except FileNotFoundError:
+            raise ValueError("Error al guardar el archivo")
+        except NoCredentialsError:
+            raise ValueError("Credenciales invalidas")
+        except Exception as e:
+            raise e
+    
     @classmethod
     def get_object(cls, bucket_name: str, object_name: str):
         """Get an object from an S3 bucket
 
         :param bucket_name: string
         :param object_name: string
         :return: Boto3 S3 object. If error, returns None.
```

### Comparing `Log_Api-0.0.7/Log_Api/Utils/ModelsType.py` & `Log_Api-0.0.8/Log_Api/Utils/ModelsType.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.7/Log_Api/Utils/Response.py` & `Log_Api-0.0.8/Log_Api/Utils/Response.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.7/Log_Api/Utils/Template.py` & `Log_Api-0.0.8/Log_Api/Utils/Template.py`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.7/Log_Api.egg-info/SOURCES.txt` & `Log_Api-0.0.8/Log_Api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.7/README.md` & `Log_Api-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `Log_Api-0.0.7/aws_handler_decorators.py` & `Log_Api-0.0.8/aws_handler_decorators.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 try:
     basestring
 except NameError:
     basestring = str
 
 logger = logging.getLogger(__name__)
 
-__version__ = '0.0.7'
+__version__ = '0.0.8'
 
 class AwsHandlerDecorator(object):
     def __init__(self, func):
         update_wrapper(self, func)
         self.func = func
 
     def __call__(self, event, context):
```

### Comparing `Log_Api-0.0.7/setup.py` & `Log_Api-0.0.8/setup.py`

 * *Files identical despite different names*

