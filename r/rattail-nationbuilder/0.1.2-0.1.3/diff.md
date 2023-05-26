# Comparing `tmp/rattail-nationbuilder-0.1.2.tar.gz` & `tmp/rattail-nationbuilder-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/lance/src/rattail-nationbuilder/dist/.tmp-qbjl5toy/rattail-nationbuilder-0.1.2.tar", last modified: Wed May 17 12:02:10 2023, max compression
+gzip compressed data, was "/home/lance/src/rattail-nationbuilder/dist/.tmp-tnv8ppgs/rattail-nationbuilder-0.1.3.tar", last modified: Fri May 26 02:38:07 2023, max compression
```

## Comparing `rattail-nationbuilder-0.1.2.tar` & `rattail-nationbuilder-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/
--rw-r--r--   0 lance     (1000) lance     (1000)      569 2023-05-17 12:01:36.000000 rattail-nationbuilder-0.1.2/CHANGELOG.md
--rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.2/MANIFEST.in
--rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      290 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.2/README.md
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/
--rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-05-05 19:43:26.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-17 12:01:39.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/_version.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/nationbuilder/
--rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-05-05 19:45:56.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/nationbuilder/__init__.py
--rw-r--r--   0 lance     (1000) lance     (1000)     4578 2023-05-09 23:33:43.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder/nationbuilder/webapi.py
-drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/
--rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/PKG-INFO
--rw-r--r--   0 lance     (1000) lance     (1000)      439 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/SOURCES.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/dependency_links.txt
--rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/requires.txt
--rw-r--r--   0 lance     (1000) lance     (1000)       22 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/top_level.txt
--rw-r--r--   0 lance     (1000) lance     (1000)      794 2023-05-17 12:02:10.000000 rattail-nationbuilder-0.1.2/setup.cfg
--rw-r--r--   0 lance     (1000) lance     (1000)     1017 2023-05-17 12:01:08.000000 rattail-nationbuilder-0.1.2/setup.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/
+-rw-r--r--   0 lance     (1000) lance     (1000)      658 2023-05-26 02:37:12.000000 rattail-nationbuilder-0.1.3/CHANGELOG.md
+-rw-r--r--   0 lance     (1000) lance     (1000)       27 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.3/MANIFEST.in
+-rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      290 2023-05-05 18:32:20.000000 rattail-nationbuilder-0.1.3/README.md
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder/
+-rw-r--r--   0 lance     (1000) lance     (1000)     1013 2023-05-05 19:43:26.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)       48 2023-05-26 02:37:16.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder/_version.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder/nationbuilder/
+-rw-r--r--   0 lance     (1000) lance     (1000)        0 2023-05-05 19:45:56.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder/nationbuilder/__init__.py
+-rw-r--r--   0 lance     (1000) lance     (1000)     4558 2023-05-26 02:36:23.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder/nationbuilder/webapi.py
+drwxr-xr-x   0 lance     (1000) lance     (1000)        0 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder.egg-info/
+-rw-r--r--   0 lance     (1000) lance     (1000)      982 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder.egg-info/PKG-INFO
+-rw-r--r--   0 lance     (1000) lance     (1000)      439 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder.egg-info/SOURCES.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        1 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder.egg-info/dependency_links.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)        8 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder.egg-info/requires.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)       22 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/rattail_nationbuilder.egg-info/top_level.txt
+-rw-r--r--   0 lance     (1000) lance     (1000)      794 2023-05-26 02:38:07.000000 rattail-nationbuilder-0.1.3/setup.cfg
+-rw-r--r--   0 lance     (1000) lance     (1000)     1017 2023-05-17 12:01:08.000000 rattail-nationbuilder-0.1.3/setup.py
```

### Comparing `rattail-nationbuilder-0.1.2/PKG-INFO` & `rattail-nationbuilder-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-nationbuilder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Rattail integration package for NationBuilder
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-nationbuilder-0.1.2/rattail_nationbuilder/__init__.py` & `rattail-nationbuilder-0.1.3/rattail_nationbuilder/__init__.py`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.2/rattail_nationbuilder/nationbuilder/webapi.py` & `rattail-nationbuilder-0.1.3/rattail_nationbuilder/nationbuilder/webapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,14 @@
     https://nationbuilder.com/api_documentation
     """
 
     def __init__(self, config, base_url=None, access_token=None,
                  max_retries=None, **kwargs):
         self.config = config
         self.app = self.config.get_app()
-        self.session = None
 
         self.base_url = base_url or self.config.require(
             'nationbuilder', 'api.base_url')
         self.base_url = self.base_url.rstrip('/')
 
         self.access_token = access_token or self.config.require(
             'nationbuilder', 'api.access_token')
@@ -65,16 +64,16 @@
         """
         api_method = api_method.lstrip('/')
 
         params = params or {}
         params['access_token'] = self.access_token
 
         if request_method == 'GET':
-            response = requests.get('{}/{}'.format(self.base_url, api_method),
-                                    params=params)
+            response = self.session.get('{}/{}'.format(self.base_url, api_method),
+                                        params=params)
 
         else:
             raise NotImplementedError("unknown request method: {}".format(
                 request_method))
 
         response.raise_for_status()
         return response
```

### Comparing `rattail-nationbuilder-0.1.2/rattail_nationbuilder.egg-info/PKG-INFO` & `rattail-nationbuilder-0.1.3/rattail_nationbuilder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattail-nationbuilder
-Version: 0.1.2
+Version: 0.1.3
 Summary: Rattail integration package for NationBuilder
 Home-page: https://rattailproject.org/
 Author: Lance Edgar
 Author-email: lance@edbob.org
 License: GNU GPL v3
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `rattail-nationbuilder-0.1.2/setup.cfg` & `rattail-nationbuilder-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `rattail-nationbuilder-0.1.2/setup.py` & `rattail-nationbuilder-0.1.3/setup.py`

 * *Files identical despite different names*

