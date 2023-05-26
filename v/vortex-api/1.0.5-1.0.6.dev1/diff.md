# Comparing `tmp/vortex_api-1.0.5.tar.gz` & `tmp/vortex_api-1.0.6.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-pdch_rig/vortex_api-1.0.5.tar", last modified: Thu May 11 05:00:36 2023, max compression
+gzip compressed data, was "/Users/shauryamgupta/sdks/pyvortex/dist/.tmp-86slbcnf/vortex_api-1.0.6.dev1.tar", last modified: Fri May 26 07:29:28 2023, max compression
```

## Comparing `vortex_api-1.0.5.tar` & `vortex_api-1.0.6.dev1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-11 05:00:36.275211 vortex_api-1.0.5/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.5/LICENSE
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1771 2023-05-11 05:00:36.275314 vortex_api-1.0.5/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      915 2023-05-10 20:08:17.000000 vortex_api-1.0.5/README.md
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-11 05:00:36.275603 vortex_api-1.0.5/setup.cfg
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1409 2023-05-11 04:56:57.000000 vortex_api-1.0.5/setup.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-11 05:00:36.272567 vortex_api-1.0.5/vortex_api/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1331 2023-05-10 17:24:32.000000 vortex_api-1.0.5/vortex_api/__init__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      336 2023-05-11 04:59:05.000000 vortex_api-1.0.5/vortex_api/__version__.py
--rw-r--r--   0 shauryamgupta   (501) staff       (20)    24579 2023-05-10 20:13:55.000000 vortex_api-1.0.5/vortex_api/api.py
-drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-11 05:00:36.275046 vortex_api-1.0.5/vortex_api.egg-info/
--rw-r--r--   0 shauryamgupta   (501) staff       (20)     1771 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/PKG-INFO
--rw-r--r--   0 shauryamgupta   (501) staff       (20)      272 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/SOURCES.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/dependency_links.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       31 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/requires.txt
--rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-11 05:00:36.000000 vortex_api-1.0.5/vortex_api.egg-info/top_level.txt
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:29:28.019294 vortex_api-1.0.6.dev1/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1102 2023-05-03 14:47:10.000000 vortex_api-1.0.6.dev1/LICENSE
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1776 2023-05-26 07:29:28.019433 vortex_api-1.0.6.dev1/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      915 2023-05-10 20:08:17.000000 vortex_api-1.0.6.dev1/README.md
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       38 2023-05-26 07:29:28.019820 vortex_api-1.0.6.dev1/setup.cfg
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1533 2023-05-26 07:20:10.000000 vortex_api-1.0.6.dev1/setup.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:29:28.017553 vortex_api-1.0.6.dev1/vortex_api/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1388 2023-05-18 10:37:38.000000 vortex_api-1.0.6.dev1/vortex_api/__init__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      341 2023-05-26 07:27:02.000000 vortex_api-1.0.6.dev1/vortex_api/__version__.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    24519 2023-05-26 07:24:30.000000 vortex_api-1.0.6.dev1/vortex_api/api.py
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)    22309 2023-05-26 07:18:33.000000 vortex_api-1.0.6.dev1/vortex_api/vortex_feed.py
+drwxr-xr-x   0 shauryamgupta   (501) staff       (20)        0 2023-05-26 07:29:28.019138 vortex_api-1.0.6.dev1/vortex_api.egg-info/
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)     1776 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/PKG-INFO
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      298 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/SOURCES.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)        1 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/dependency_links.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)      111 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/requires.txt
+-rw-r--r--   0 shauryamgupta   (501) staff       (20)       11 2023-05-26 07:29:28.000000 vortex_api-1.0.6.dev1/vortex_api.egg-info/top_level.txt
```

### Comparing `vortex_api-1.0.5/LICENSE` & `vortex_api-1.0.6.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.5/PKG-INFO` & `vortex_api-1.0.6.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex_api
-Version: 1.0.5
+Version: 1.0.6.dev1
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

### Comparing `vortex_api-1.0.5/README.md` & `vortex_api-1.0.6.dev1/README.md`

 * *Files identical despite different names*

### Comparing `vortex_api-1.0.5/setup.py` & `vortex_api-1.0.6.dev1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -28,15 +28,19 @@
     author_email=about["__author_email__"],
     url=about["__url__"],
     download_url=about["__download_url__"],
     license=about["__license__"],
     packages=["vortex_api"],
     install_requires=[
         "requests>=2.25.1",
-        "wrapt>=1.15.0"
+        "wrapt>=1.15.0",
+        "six>=1.11.0",
+        "pyOpenSSL>=17.5.0",
+        "python-dateutil>=2.6.1",
+        "autobahn[twisted]==19.11.2"
     ],
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Financial and Insurance Industry",
         "Natural Language :: English",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

### Comparing `vortex_api-1.0.5/vortex_api/__init__.py` & `vortex_api-1.0.6.dev1/vortex_api/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -30,8 +30,9 @@
 
     #Get order book 
     client.orders(limit=20,offset=1)
 
 """
 from __future__ import unicode_literals, absolute_import
 from vortex_api.api import AsthaTradeVortexAPI,Constants
-__all__ = [AsthaTradeVortexAPI,Constants]
+from vortex_api.vortex_feed import VortexFeed
+__all__ = [AsthaTradeVortexAPI,Constants,VortexFeed]
```

### Comparing `vortex_api-1.0.5/vortex_api/api.py` & `vortex_api-1.0.6.dev1/vortex_api/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import requests
 import csv
 import datetime
 import logging
 from enum import Enum
-from functools import wraps
-from typing import Type
 import inspect
 import wrapt
 
 class Constants: 
     """
     Constants used in the API
     """
@@ -567,10 +565,7 @@
 
         if (('data' in login_object ) and login_object["data"] != None and login_object["data"]["access_token"] != None): 
             self.access_token = login_object["data"]["access_token"]
             return True
         
         return False
     
-
-
-
```

### Comparing `vortex_api-1.0.5/vortex_api.egg-info/PKG-INFO` & `vortex_api-1.0.6.dev1/vortex_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vortex-api
-Version: 1.0.5
+Version: 1.0.6.dev1
 Summary: Vortex APIs to place orders in AsthaTrade Flow application
 Home-page: https://vortex.asthatrade.com
 Download-URL: https://github.com/AsthaTech/pyvortex
 Author: Astha Credit & Securities Pvt Ltd.
 Author-email: tech@asthatrade.com
 License: MIT
 Classifier: Intended Audience :: Developers
```

