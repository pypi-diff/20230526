# Comparing `tmp/scrapy-zyte-api-0.8.3.tar.gz` & `tmp/scrapy-zyte-api-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scrapy-zyte-api-0.8.3.tar", last modified: Wed May 17 15:47:31 2023, max compression
+gzip compressed data, was "scrapy-zyte-api-0.8.4.tar", last modified: Fri May 26 09:15:17 2023, max compression
```

## Comparing `scrapy-zyte-api-0.8.3.tar` & `scrapy-zyte-api-0.8.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:31.454481 scrapy-zyte-api-0.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-17 15:47:31.454481 scrapy-zyte-api-0.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28637 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:31.454481 scrapy-zyte-api-0.8.3/scrapy_zyte_api/
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api/_cookies.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api/_downloader_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)    20969 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api/_request_fingerprinter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 15:47:31.454481 scrapy-zyte-api-0.8.3/scrapy_zyte_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-17 15:47:31.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-17 15:47:31.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 15:47:31.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-17 15:47:31.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 15:47:31.000000 scrapy-zyte-api-0.8.3/scrapy_zyte_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-17 15:47:31.454481 scrapy-zyte-api-0.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-17 15:47:19.000000 scrapy-zyte-api-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:15:17.082589 scrapy-zyte-api-0.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-26 09:15:17.082589 scrapy-zyte-api-0.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28637 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:15:17.078590 scrapy-zyte-api-0.8.4/scrapy_zyte_api/
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/_cookies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/_downloader_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20969 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/_request_fingerprinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9421 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7583 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:15:17.082589 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29454 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 09:15:17.000000 scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-26 09:15:17.082589 scrapy-zyte-api-0.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-26 09:15:03.000000 scrapy-zyte-api-0.8.4/setup.py
```

### Comparing `scrapy-zyte-api-0.8.3/LICENSE.txt` & `scrapy-zyte-api-0.8.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.3/PKG-INFO` & `scrapy-zyte-api-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-zyte-api
-Version: 0.8.3
+Version: 0.8.4
 Summary: Client library to process URLs through Zyte API
 Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy-zyte-api-0.8.3/README.rst` & `scrapy-zyte-api-0.8.4/README.rst`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.3/scrapy_zyte_api/_cookies.py` & `scrapy-zyte-api-0.8.4/scrapy_zyte_api/_cookies.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.3/scrapy_zyte_api/_downloader_middleware.py` & `scrapy-zyte-api-0.8.4/scrapy_zyte_api/_downloader_middleware.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     _slot_prefix = "zyte-api@"
 
     @classmethod
     def from_crawler(cls, crawler):
         return cls(crawler)
 
     def __init__(self, crawler) -> None:
-        self._param_parser = _ParamParser(crawler)
+        self._param_parser = _ParamParser(crawler, cookies_enabled=False)
         self._crawler = crawler
 
     def process_request(self, request, spider):
         if self._param_parser.parse(request) is None:
             return
 
         downloader = self._crawler.engine.downloader
```

### Comparing `scrapy-zyte-api-0.8.3/scrapy_zyte_api/_params.py` & `scrapy-zyte-api-0.8.4/scrapy_zyte_api/_params.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.3/scrapy_zyte_api/_request_fingerprinter.py` & `scrapy-zyte-api-0.8.4/scrapy_zyte_api/_request_fingerprinter.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.3/scrapy_zyte_api/handler.py` & `scrapy-zyte-api-0.8.4/scrapy_zyte_api/handler.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.3/scrapy_zyte_api/responses.py` & `scrapy-zyte-api-0.8.4/scrapy_zyte_api/responses.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.3/scrapy_zyte_api/utils.py` & `scrapy-zyte-api-0.8.4/scrapy_zyte_api/utils.py`

 * *Files identical despite different names*

### Comparing `scrapy-zyte-api-0.8.3/scrapy_zyte_api.egg-info/PKG-INFO` & `scrapy-zyte-api-0.8.4/scrapy_zyte_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scrapy-zyte-api
-Version: 0.8.3
+Version: 0.8.4
 Summary: Client library to process URLs through Zyte API
 Home-page: https://github.com/scrapy-plugins/scrapy-zyte-api
 Author: Zyte Group Ltd
 Author-email: info@zyte.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `scrapy-zyte-api-0.8.3/setup.py` & `scrapy-zyte-api-0.8.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="scrapy-zyte-api",
-    version="0.8.3",
+    version="0.8.4",
     description="Client library to process URLs through Zyte API",
     long_description=open("README.rst").read(),
     long_description_content_type="text/x-rst",
     author="Zyte Group Ltd",
     author_email="info@zyte.com",
     url="https://github.com/scrapy-plugins/scrapy-zyte-api",
     packages=["scrapy_zyte_api"],
```

