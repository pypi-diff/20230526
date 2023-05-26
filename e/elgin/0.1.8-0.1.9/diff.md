# Comparing `tmp/elgin-0.1.8.tar.gz` & `tmp/elgin-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elgin-0.1.8.tar", last modified: Fri May 26 12:52:04 2023, max compression
+gzip compressed data, was "elgin-0.1.9.tar", last modified: Fri May 26 13:17:03 2023, max compression
```

## Comparing `elgin-0.1.8.tar` & `elgin-0.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:52:04.415450 elgin-0.1.8/
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     2341 2023-05-26 12:52:04.415450 elgin-0.1.8/PKG-INFO
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     1625 2023-05-25 14:57:03.000000 elgin-0.1.8/README.md
-drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:52:04.415450 elgin-0.1.8/elgin/
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-24 18:41:57.000000 elgin-0.1.8/elgin/__init__.py
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)    11967 2023-05-25 16:12:16.000000 elgin-0.1.8/elgin/monitoramento.py
-drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:52:04.415450 elgin-0.1.8/elgin/templates/
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     3978 2023-05-24 18:09:12.000000 elgin-0.1.8/elgin/templates/template_email_log.html
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     4019 2023-05-24 20:41:00.000000 elgin-0.1.8/elgin/templates/template_teams.json
-drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 12:52:04.415450 elgin-0.1.8/elgin.egg-info/
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     2341 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/PKG-INFO
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)      279 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/SOURCES.txt
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        1 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/dependency_links.txt
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        9 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/requires.txt
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        6 2023-05-26 12:52:04.000000 elgin-0.1.8/elgin.egg-info/top_level.txt
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)       38 2023-05-26 12:52:04.415450 elgin-0.1.8/setup.cfg
--rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     1020 2023-05-26 12:51:55.000000 elgin-0.1.8/setup.py
+drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 13:17:03.755442 elgin-0.1.9/
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     2341 2023-05-26 13:17:03.755442 elgin-0.1.9/PKG-INFO
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     1625 2023-05-25 14:57:03.000000 elgin-0.1.9/README.md
+drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 13:17:03.755442 elgin-0.1.9/elgin/
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-24 18:41:57.000000 elgin-0.1.9/elgin/__init__.py
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)    12017 2023-05-26 13:14:38.000000 elgin-0.1.9/elgin/monitoramento.py
+drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 13:17:03.755442 elgin-0.1.9/elgin/templates/
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     3978 2023-05-24 18:09:12.000000 elgin-0.1.9/elgin/templates/template_email_log.html
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     4019 2023-05-24 20:41:00.000000 elgin-0.1.9/elgin/templates/template_teams.json
+drwxr-xr-x   0 joao-soares  (1000) joao-soares  (1000)        0 2023-05-26 13:17:03.755442 elgin-0.1.9/elgin.egg-info/
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     2341 2023-05-26 13:17:03.000000 elgin-0.1.9/elgin.egg-info/PKG-INFO
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)      279 2023-05-26 13:17:03.000000 elgin-0.1.9/elgin.egg-info/SOURCES.txt
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        1 2023-05-26 13:17:03.000000 elgin-0.1.9/elgin.egg-info/dependency_links.txt
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)       17 2023-05-26 13:17:03.000000 elgin-0.1.9/elgin.egg-info/requires.txt
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)        6 2023-05-26 13:17:03.000000 elgin-0.1.9/elgin.egg-info/top_level.txt
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)       38 2023-05-26 13:17:03.755442 elgin-0.1.9/setup.cfg
+-rw-r--r--   0 joao-soares  (1000) joao-soares  (1000)     1030 2023-05-26 13:16:20.000000 elgin-0.1.9/setup.py
```

### Comparing `elgin-0.1.8/PKG-INFO` & `elgin-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Biblioteca responsavel por gerar o monitoramento dos processos da empresa elgin.
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `elgin-0.1.8/README.md` & `elgin-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `elgin-0.1.8/elgin/monitoramento.py` & `elgin-0.1.9/elgin/monitoramento.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 from datetime import datetime
 from email.message import EmailMessage
 from contextlib import contextmanager
+from pymysql.cursors import DictCursor
 
 import awswrangler as wr
 import boto3
 import enum
 import getpass
 import platform
 import logging
 import pytz
 import smtplib
 import ssl
 import mysql.connector
 import json
 import requests
 import os
+import pymysql
 
 # -- Criando uma sessao com a AWS -- #
 awsSession = boto3.Session()
 
 @contextmanager
 def rds_conector() -> any:
     try:
         credentials = wr.secretsmanager.get_secret_json('/rpa/mysql/credentials', boto3_session=awsSession)
-        conn = mysql.connector.connect(
+        conn = pymysql.connect(
             host=credentials['host'],
             user=credentials['username'],
             password=credentials['password'],
             port=3306
         )
         yield conn 
     except mysql.connector.Error as e:
@@ -60,15 +62,15 @@
         self.query += f" Where {condition}"
         return self
    
     def executar(self) -> any:
         try:
             with rds_conector() as conn:
 
-                cursor = conn.cursor(dictionary=True)   
+                cursor = conn.cursor(cursor=DictCursor)   
 
                 if self.dml == 'insert':
                     cursor.execute(self.INSERT_QUERY, self.kwargs)
                     conn.commit()
                     result = cursor.lastrowid
                 else:                
                     cursor.execute(self.query)
@@ -136,15 +138,15 @@
     def filtrar(self, condition:str) -> 'TbResponsaveis':
         self.query += f" Where {condition}"
         return self
 
     def executar(self) -> dict:
         try:
             with rds_conector() as conn:
-                cursor = conn.cursor(dictionary=True)                          
+                cursor = conn.cursor(cursor=DictCursor)                          
                 cursor.execute(self.query)
                 result = cursor.fetchall()
                 return result
         except mysql.connector.Error as e:
             conn.rollback()
             raise e
         finally:
```

### Comparing `elgin-0.1.8/elgin/templates/template_email_log.html` & `elgin-0.1.9/elgin/templates/template_email_log.html`

 * *Files identical despite different names*

### Comparing `elgin-0.1.8/elgin/templates/template_teams.json` & `elgin-0.1.9/elgin/templates/template_teams.json`

 * *Files identical despite different names*

### Comparing `elgin-0.1.8/elgin.egg-info/PKG-INFO` & `elgin-0.1.9/elgin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elgin
-Version: 0.1.8
+Version: 0.1.9
 Summary: Biblioteca responsavel por gerar o monitoramento dos processos da empresa elgin.
 Home-page: UNKNOWN
 License: MIT
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `elgin-0.1.8/setup.py` & `elgin-0.1.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open('./README.md') as f:
     long_desc = f.read()
 
 setup(
      name='elgin'
-    ,version='0.1.8'
+    ,version='0.1.9'
     ,description='Biblioteca responsavel por gerar o monitoramento dos processos da empresa elgin.'
     ,long_description=long_desc
     ,long_description_content_type='text/markdown'
     ,license="MIT"
     ,classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
@@ -22,9 +22,9 @@
         "Programming Language :: Python :: 3.10",
         "Operating System :: OS Independent"
     ]
     ,packages=['elgin']
     ,package_dir={'elgin': 'elgin'}
     ,package_data={'elgin': ['templates/*']}
     ,include_package_data=True
-    ,install_requires=["requests"]
+    ,install_requires=["requests","pymysql"]
 )
```

