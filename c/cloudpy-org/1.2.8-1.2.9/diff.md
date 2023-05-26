# Comparing `tmp/cloudpy_org-1.2.8.tar.gz` & `tmp/cloudpy_org-1.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpy_org-1.2.8.tar", last modified: Fri May 26 21:14:00 2023, max compression
+gzip compressed data, was "dist\cloudpy_org-1.2.9.tar", last modified: Fri May 26 21:55:10 2023, max compression
```

## Comparing `cloudpy_org-1.2.8.tar` & `cloudpy_org-1.2.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 21:14:00.488625 cloudpy_org-1.2.8/
--rw-rw-rw-   0        0        0      936 2023-05-26 21:14:00.487982 cloudpy_org-1.2.8/PKG-INFO
--rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.2.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 21:14:00.389107 cloudpy_org-1.2.8/cloudpy_org/
--rw-rw-rw-   0        0        0      112 2023-05-26 21:13:33.000000 cloudpy_org-1.2.8/cloudpy_org/__init__.py
--rw-rw-rw-   0        0        0    20179 2023-05-26 20:42:11.000000 cloudpy_org-1.2.8/cloudpy_org/cloud_framework_api.py
--rw-rw-rw-   0        0        0    52405 2023-05-26 20:39:56.000000 cloudpy_org-1.2.8/cloudpy_org/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-26 21:14:00.466337 cloudpy_org-1.2.8/cloudpy_org.egg-info/
--rw-rw-rw-   0        0        0      936 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      272 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-26 21:13:58.000000 cloudpy_org-1.2.8/cloudpy_org.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 21:14:00.488625 cloudpy_org-1.2.8/setup.cfg
--rw-rw-rw-   0        0        0     1325 2023-05-26 04:08:34.000000 cloudpy_org-1.2.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:55:10.474299 cloudpy_org-1.2.9/
+-rw-rw-rw-   0        0        0      936 2023-05-26 21:55:10.473317 cloudpy_org-1.2.9/PKG-INFO
+-rw-rw-rw-   0        0        0      454 2023-04-14 05:11:55.000000 cloudpy_org-1.2.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 21:55:10.253651 cloudpy_org-1.2.9/cloudpy_org/
+-rw-rw-rw-   0        0        0      112 2023-05-26 21:13:33.000000 cloudpy_org-1.2.9/cloudpy_org/__init__.py
+-rw-rw-rw-   0        0        0    19947 2023-05-26 21:53:58.000000 cloudpy_org-1.2.9/cloudpy_org/cloud_framework_api.py
+-rw-rw-rw-   0        0        0    52405 2023-05-26 21:19:42.000000 cloudpy_org-1.2.9/cloudpy_org/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-26 21:55:10.426145 cloudpy_org-1.2.9/cloudpy_org.egg-info/
+-rw-rw-rw-   0        0        0      936 2023-05-26 21:55:09.000000 cloudpy_org-1.2.9/cloudpy_org.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-05-26 21:55:10.000000 cloudpy_org-1.2.9/cloudpy_org.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 21:55:09.000000 cloudpy_org-1.2.9/cloudpy_org.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-05-26 21:55:09.000000 cloudpy_org-1.2.9/cloudpy_org.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-26 21:55:09.000000 cloudpy_org-1.2.9/cloudpy_org.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 21:55:10.474299 cloudpy_org-1.2.9/setup.cfg
+-rw-rw-rw-   0        0        0     1325 2023-05-26 21:47:33.000000 cloudpy_org-1.2.9/setup.py
```

### Comparing `cloudpy_org-1.2.8/PKG-INFO` & `cloudpy_org-1.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy_org
-Version: 1.2.8
+Version: 1.2.9
 Summary: Cloud data pipeline organization and automation library. Cloud framework manager API for AWS.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.2.8/cloudpy_org/cloud_framework_api.py` & `cloudpy_org-1.2.9/cloudpy_org/cloud_framework_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,22 +14,14 @@
 import random
 import boto3
 import json
 import os
 xpt = tools.processing_tools()
 xs3 = boto3.client('s3')
 xpt.environment = "s3"
-
-access_key ="AKIAQCBCZZOOKCRB2SWI"
-secret = "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"
-
-#session = boto3.Session(
-#    aws_access_key_id=settings.AWS_SERVER_PUBLIC_KEY,
-#    aws_secret_access_key=settings.AWS_SERVER_SECRET_KEY,
-#)
 class aws_framework_manager:
     def __init__(self,secret_pair:list=[]):
         self.__cppt_construction(secret_pair)
         self.cppt.environment = "s3"
         self.general_info = {}
         self.service_name = "cloudpy-org-service-beta"
         self.delimiters = ["pZo-9xH9oEO2B2OEo","2nZzN01wtktk10N","VhMxT-9xVVZzN01w","_Shv-4F86Co981h"]
```

### Comparing `cloudpy_org-1.2.8/cloudpy_org/tools.py` & `cloudpy_org-1.2.9/cloudpy_org/tools.py`

 * *Files identical despite different names*

### Comparing `cloudpy_org-1.2.8/cloudpy_org.egg-info/PKG-INFO` & `cloudpy_org-1.2.9/cloudpy_org.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpy-org
-Version: 1.2.8
+Version: 1.2.9
 Summary: Cloud data pipeline organization and automation library. Cloud framework manager API for AWS.
 Home-page: https://www.cloudpy.org/
 Author: cloudpy.org
 Author-email: admin@cloudpy.org
 License: MIT
 Description: A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.
 Platform: UNKNOWN
```

### Comparing `cloudpy_org-1.2.8/setup.py` & `cloudpy_org-1.2.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from os import path
 
 
 long_description = 'A library to programmatically create, interact, encrypt and automate your data pipelines making it simple to scale to the most popular cloud plattforms.'
 
 setup(
     name="cloudpy_org",
-    version="1.2.8",
+    version="1.2.9",
     description="Cloud data pipeline organization and automation library. Cloud framework manager API for AWS.",
     long_description_content_type="text/markdown",
     long_description=long_description,
     url="https://www.cloudpy.org/",
     author="cloudpy.org",
     author_email="admin@cloudpy.org",
     license="MIT",
```

