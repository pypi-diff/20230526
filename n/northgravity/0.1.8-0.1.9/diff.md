# Comparing `tmp/northgravity-0.1.8.tar.gz` & `tmp/northgravity-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "northgravity-0.1.8.tar", last modified: Tue May 23 15:51:06 2023, max compression
+gzip compressed data, was "northgravity-0.1.9.tar", last modified: Wed May 24 10:39:49 2023, max compression
```

## Comparing `northgravity-0.1.8.tar` & `northgravity-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:51:06.645182 northgravity-0.1.8/
--rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)    29830 2023-05-23 15:51:06.645182 northgravity-0.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    29397 2023-05-23 15:51:06.000000 northgravity-0.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:51:06.645182 northgravity-0.1.8/northgravity/
--rw-rw-r--   0 root         (0) root         (0)     1327 2023-05-18 09:33:33.000000 northgravity-0.1.8/northgravity/Authenticator.py
--rw-rw-r--   0 root         (0) root         (0)    10526 2023-05-23 15:34:39.000000 northgravity-0.1.8/northgravity/DatalakeHandler.py
--rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/ExceptionHandler.py
--rw-rw-r--   0 root         (0) root         (0)     6567 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/HTTPCalller.py
--rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/StatusHandler.py
--rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/TaskHandler.py
--rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/Timeseries.py
--rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.8/northgravity/__init__.py
--rw-r--r--   0 root         (0) root         (0)      122 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-23 15:51:06.645182 northgravity-0.1.8/northgravity.egg-info/
--rw-r--r--   0 root         (0) root         (0)    29830 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      464 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-23 15:51:06.000000 northgravity-0.1.8/northgravity.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-23 15:51:06.645182 northgravity-0.1.8/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:39:49.541800 northgravity-0.1.9/
+-rw-rw-r--   0 root         (0) root         (0)     1055 2023-04-18 12:31:14.000000 northgravity-0.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    29830 2023-05-24 10:39:49.541800 northgravity-0.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    29397 2023-05-24 10:39:49.000000 northgravity-0.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:39:49.541800 northgravity-0.1.9/northgravity/
+-rw-rw-r--   0 root         (0) root         (0)     1327 2023-05-18 09:33:33.000000 northgravity-0.1.9/northgravity/Authenticator.py
+-rw-rw-r--   0 root         (0) root         (0)    11447 2023-05-24 10:39:39.000000 northgravity-0.1.9/northgravity/DatalakeHandler.py
+-rw-rw-r--   0 root         (0) root         (0)      309 2023-04-18 12:31:14.000000 northgravity-0.1.9/northgravity/ExceptionHandler.py
+-rw-rw-r--   0 root         (0) root         (0)     7273 2023-05-24 10:39:39.000000 northgravity-0.1.9/northgravity/HTTPCalller.py
+-rw-rw-r--   0 root         (0) root         (0)     1792 2023-04-18 12:31:14.000000 northgravity-0.1.9/northgravity/StatusHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    10261 2023-04-18 12:31:14.000000 northgravity-0.1.9/northgravity/TaskHandler.py
+-rw-rw-r--   0 root         (0) root         (0)    13042 2023-04-18 12:31:14.000000 northgravity-0.1.9/northgravity/Timeseries.py
+-rw-rw-r--   0 root         (0) root         (0)      567 2023-04-18 12:31:14.000000 northgravity-0.1.9/northgravity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      122 2023-05-24 10:39:49.000000 northgravity-0.1.9/northgravity/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-24 10:39:49.541800 northgravity-0.1.9/northgravity.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    29830 2023-05-24 10:39:49.000000 northgravity-0.1.9/northgravity.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      464 2023-05-24 10:39:49.000000 northgravity-0.1.9/northgravity.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-24 10:39:49.000000 northgravity-0.1.9/northgravity.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-05-24 10:39:49.000000 northgravity-0.1.9/northgravity.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2023-05-24 10:39:49.000000 northgravity-0.1.9/northgravity.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-24 10:39:49.541800 northgravity-0.1.9/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      829 2023-04-18 12:31:14.000000 northgravity-0.1.9/setup.py
```

### Comparing `northgravity-0.1.8/LICENSE` & `northgravity-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.8/PKG-INFO` & `northgravity-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,19 +40,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.8
+pip3 install northgravity==0.1.9
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.8
+northgravity==0.1.9
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.8/README.md` & `northgravity-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,19 +26,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.8
+pip3 install northgravity==0.1.9
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.8
+northgravity==0.1.9
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.8/northgravity/Authenticator.py` & `northgravity-0.1.9/northgravity/Authenticator.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.8/northgravity/DatalakeHandler.py` & `northgravity-0.1.9/northgravity/DatalakeHandler.py`

 * *Files 5% similar despite different names*

```diff
@@ -204,14 +204,33 @@
                    "fileName": file_name,
                    "fileType": file_type,
                    "fields": metadata_fields}
 
         log.debug(f'Payload: {payload}')
 
         return self.caller.file_uploader(payload, file), file_name
+    
+    def update_file_metadata(self, file_id, metadata_field=None, metadata_value=None):
+        
+        if metadata_field not in ['', None]:
+            assert metadata_value not in ['', None], 'If metadata_field is passed, the metadata_value should also exist. Please add metadata_value parameter'
+        if metadata_value not in ['', None]:
+            assert metadata_field not in ['', None], 'If metadata_field is passed, the metadata_value should also exist. Please add metadata_field parameter'
+
+        if metadata_field not in ['', None]:
+            metadata_fields = [{"name":metadata_field,"value":metadata_value}]
+        
+        # Retrieve the file on the Datalake (S3)
+        path = '/file/' + file_id
+
+        # PAYLOAD for the metadata update of the file
+        payload = {"fields": metadata_fields}
+        log.debug(f'Payload: {payload}')
+
+        return self.caller.put(path, payload=payload)
 
 
 # ---------------------
 # HELPER functions
 # --------------------
 def format_query(init_query):
     '''Properly Format the query dictionary for the API Call'''
```

### Comparing `northgravity-0.1.8/northgravity/HTTPCalller.py` & `northgravity-0.1.9/northgravity/HTTPCalller.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,31 @@
             log.info('Posting with message {} was successful with response: {}'.format(payload, r.text))
             return r
 
         else:
             log.error('Posting with message {} ended with error (error code: {}). Response: {}'.format(payload, r.status_code, r.text))
             return r
 
+    def put(self, path, payload=None, data=None, headers=None):
+        headers = self.set_headers(headers)
+        
+        # Request URL
+        full_path = self.url + path
+        log.debug('PUT request before sending: {}, {}'.format(full_path, headers))
+
+        r = requests.put(full_path, json=payload, data=data, headers=headers)
+        if (r.status_code >= 200) and (r.status_code < 300):
+            log.info('Put request with message {} was successful with response: {}'.format(payload, r.text))
+            return r
+
+        else:
+            log.error('Put request with message {} ended with error (error code: {}). Response: {}'.format(payload, r.status_code, r.text))
+            return r
+
+
     def get(self, path, headers=None):
         headers = self.set_headers(headers)
 
         # Request URL
         full_path = self.url + path
         log.debug('GET request before sending: {}, {}'.format(full_path, headers))
```

### Comparing `northgravity-0.1.8/northgravity/StatusHandler.py` & `northgravity-0.1.9/northgravity/StatusHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.8/northgravity/TaskHandler.py` & `northgravity-0.1.9/northgravity/TaskHandler.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.8/northgravity/Timeseries.py` & `northgravity-0.1.9/northgravity/Timeseries.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.8/northgravity/__init__.py` & `northgravity-0.1.9/northgravity/__init__.py`

 * *Files identical despite different names*

### Comparing `northgravity-0.1.8/northgravity.egg-info/PKG-INFO` & `northgravity-0.1.9/northgravity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: northgravity
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python SDK for NorthGravity platform
 Home-page: https://www.northgravity.com/
 Author: NorthGravity
 Author-email: info@northgravity.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -40,19 +40,19 @@
 - **Time Series Handler** - retrieves data directly from the time series database
 
 
 
 ## How to install and set the package: 
 ### Install
 ```text
-pip3 install northgravity==0.1.8
+pip3 install northgravity==0.1.9
 ```
 As the library is available from pip, it can be installed as a specific version within a Python Task from within requirements.txt just by adding:
 ```text
-northgravity==0.1.8
+northgravity==0.1.9
 ```
 The package relies on the requests library so, in the project, the user must install this library in the requirements.txt file.
 ```text
 pip3 install requests==2.25.1
 ```
```

### Comparing `northgravity-0.1.8/setup.py` & `northgravity-0.1.9/setup.py`

 * *Files identical despite different names*

