# Comparing `tmp/ploomes-api-client-0.1.1.tar.gz` & `tmp/ploomes-api-client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ploomes-api-client-0.1.1.tar", last modified: Thu May 25 21:21:14 2023, max compression
+gzip compressed data, was "ploomes-api-client-0.1.2.tar", last modified: Fri May 26 18:49:42 2023, max compression
```

## Comparing `ploomes-api-client-0.1.1.tar` & `ploomes-api-client-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:21:14.664690 ploomes-api-client-0.1.1/
--rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.1/LICENSE
--rw-r--r--   0 filterfeed   (501) staff       (20)     2301 2023-05-25 21:21:14.664125 ploomes-api-client-0.1.1/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)     1139 2023-05-25 21:19:00.000000 ploomes-api-client-0.1.1/README.md
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:21:14.662996 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/
--rw-r--r--   0 filterfeed   (501) staff       (20)     2301 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/PKG-INFO
--rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/SOURCES.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/dependency_links.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/requires.txt
--rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-25 21:21:14.000000 ploomes-api-client-0.1.1/ploomes_api_client.egg-info/top_level.txt
-drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-25 21:21:14.663399 ploomes-api-client-0.1.1/ploomes_client/
--rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-25 21:10:14.000000 ploomes-api-client-0.1.1/ploomes_client/__init__.py
--rw-r--r--   0 filterfeed   (501) staff       (20)    21748 2023-05-25 21:10:21.000000 ploomes-api-client-0.1.1/ploomes_client/ploomes_client.py
--rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-25 21:21:14.664777 ploomes-api-client-0.1.1/setup.cfg
--rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-25 21:19:52.000000 ploomes-api-client-0.1.1/setup.py
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-26 18:49:42.584521 ploomes-api-client-0.1.2/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1072 2023-05-25 21:00:11.000000 ploomes-api-client-0.1.2/LICENSE
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-26 18:49:42.584363 ploomes-api-client-0.1.2/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)     1137 2023-05-26 14:13:51.000000 ploomes-api-client-0.1.2/README.md
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-26 18:49:42.583297 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/
+-rw-r--r--   0 filterfeed   (501) staff       (20)     2275 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/PKG-INFO
+-rw-r--r--   0 filterfeed   (501) staff       (20)      295 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/SOURCES.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)        1 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/dependency_links.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       26 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/requires.txt
+-rw-r--r--   0 filterfeed   (501) staff       (20)       15 2023-05-26 18:49:42.000000 ploomes-api-client-0.1.2/ploomes_api_client.egg-info/top_level.txt
+drwxr-xr-x   0 filterfeed   (501) staff       (20)        0 2023-05-26 18:49:42.583691 ploomes-api-client-0.1.2/ploomes_client/
+-rw-r--r--   0 filterfeed   (501) staff       (20)       43 2023-05-26 18:47:42.000000 ploomes-api-client-0.1.2/ploomes_client/__init__.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)    22820 2023-05-26 18:41:36.000000 ploomes-api-client-0.1.2/ploomes_client/ploomes_client.py
+-rw-r--r--   0 filterfeed   (501) staff       (20)       38 2023-05-26 18:49:42.584576 ploomes-api-client-0.1.2/setup.cfg
+-rw-r--r--   0 filterfeed   (501) staff       (20)      948 2023-05-26 18:48:32.000000 ploomes-api-client-0.1.2/setup.py
```

### Comparing `ploomes-api-client-0.1.1/LICENSE` & `ploomes-api-client-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ploomes-api-client-0.1.1/PKG-INFO` & `ploomes-api-client-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
-Description: """
-        # Ploomes API Python Client
+Description: # Ploomes API Python Client
         
-        This package provides a simple Python client for the [Ploomes API](https://www.ploomes.com/).
+        This package provides a simple Python client for the [Ploomes API](https://developers.ploomes.com/).
         
         ## Installation
         
         You can install the package from PyPI:
         
         ```bash
         pip install ploomes-api-client
@@ -55,16 +54,14 @@
         )
         ```
         
         ## Contributing
         
         Contributions are welcome! Please feel free to submit a Pull Request.
         
-        """
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ploomes-api-client-0.1.1/README.md` & `ploomes-api-client-0.1.2/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-"""
 # Ploomes API Python Client
 
-This package provides a simple Python client for the [Ploomes API](https://www.ploomes.com/).
+This package provides a simple Python client for the [Ploomes API](https://developers.ploomes.com/).
 
 ## Installation
 
 You can install the package from PyPI:
 
 ```bash
 pip install ploomes-api-client
@@ -46,9 +45,7 @@
     OtherProperties={'Property': 'Value'}
 )
 ```
 
 ## Contributing
 
 Contributions are welcome! Please feel free to submit a Pull Request.
-
-"""
```

### Comparing `ploomes-api-client-0.1.1/ploomes_api_client.egg-info/PKG-INFO` & `ploomes-api-client-0.1.2/ploomes_api_client.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: ploomes-api-client
-Version: 0.1.1
+Version: 0.1.2
 Summary: Python client for the Ploomes API
 Home-page: https://github.com/victorfigueredo/ploomes-api-client
 Author: Victor Figueredo
 Author-email: cto@filterfeed.com.br
 License: UNKNOWN
-Description: """
-        # Ploomes API Python Client
+Description: # Ploomes API Python Client
         
-        This package provides a simple Python client for the [Ploomes API](https://www.ploomes.com/).
+        This package provides a simple Python client for the [Ploomes API](https://developers.ploomes.com/).
         
         ## Installation
         
         You can install the package from PyPI:
         
         ```bash
         pip install ploomes-api-client
@@ -55,16 +54,14 @@
         )
         ```
         
         ## Contributing
         
         Contributions are welcome! Please feel free to submit a Pull Request.
         
-        """
-        
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ploomes-api-client-0.1.1/ploomes_client/ploomes_client.py` & `ploomes-api-client-0.1.2/ploomes_client/ploomes_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -573,21 +573,52 @@
                           headers=self.headers)
         response = r.json()
         return response
 
     @retry
     @sleep_and_retry
     @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
-    def post_interaction_record(self, contact_id, content, date, typeId=7):
+    def get_interaction_records(self, _filter=None):
+        response = []
+        url = f"{self.host}/InteractionRecords?"
+        if _filter:
+            url += f"$filter={_filter}&"
+        url += "$expand=OtherProperties&$top=300&$orderby=Id+desc"
+        while url:
+            r = requests.get(url, headers=self.headers, timeout=5)
+            data = r.json()
+            if data.get('value'):
+                response += data["value"]
+            url = data.get("@odata.nextLink")
+        return response
+
+
+    @retry
+    @sleep_and_retry
+    @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
+    def patch_interaction_record(self,interaction_id, payload):
+        response = []
+        payload = json.dumps(payload)
+        url = f"{self.host}/InteractionRecords({interaction_id})"
+        r = requests.patch(url, headers=self.headers, data=payload, timeout=5)
+        data = r.json()
+        if data.get('value'):
+            response += data["value"]
+        return response
+
+    @retry
+    @sleep_and_retry
+    @limits(calls=MAX_REQUESTS_PER_SECOND, period=1)
+    def post_interaction_record(self, contact_id, content, date, type_id=7):
         payload = json.dumps(
             {
                 "ContactId": contact_id,
                 "Content": content,
                 "Date": date,
-                "TypeId": typeId
+                "TypeId": type_id
             }
         )
         r = requests.post(
             f"{self.host}/InteractionRecords", data=payload, headers=self.headers
         )
         response = r.json()
         return response
```

### Comparing `ploomes-api-client-0.1.1/setup.py` & `ploomes-api-client-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ploomes-api-client',
-    version='0.1.1',
+    version='0.1.2',
     packages=find_packages(),   
     url='https://github.com/victorfigueredo/ploomes-api-client',
     author='Victor Figueredo',
     author_email='cto@filterfeed.com.br',
     description='Python client for the Ploomes API',
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

