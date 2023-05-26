# Comparing `tmp/overwatch_client-0.1.2.tar.gz` & `tmp/overwatch_client-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overwatch_client-0.1.2.tar", max compression
+gzip compressed data, was "overwatch_client-0.1.3.tar", max compression
```

## Comparing `overwatch_client-0.1.2.tar` & `overwatch_client-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1209 2023-05-19 13:50:48.938301 overwatch_client-0.1.2/README.md
--rw-r--r--   0        0        0       32 2023-05-19 13:50:48.938301 overwatch_client-0.1.2/overwatch_client/__init__.py
--rw-r--r--   0        0        0    10311 2023-05-19 13:50:48.938301 overwatch_client-0.1.2/overwatch_client/client.py
--rw-r--r--   0        0        0      378 2023-05-19 13:50:48.938301 overwatch_client-0.1.2/overwatch_client/utils.py
--rw-r--r--   0        0        0     1044 2023-05-19 13:50:48.942301 overwatch_client-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 overwatch_client-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1209 2023-05-16 18:44:30.690073 overwatch_client-0.1.3/README.md
+-rw-r--r--   0        0        0       32 2023-05-09 14:55:50.728909 overwatch_client-0.1.3/overwatch_client/__init__.py
+-rw-r--r--   0        0        0    12657 2023-05-26 14:59:05.617457 overwatch_client-0.1.3/overwatch_client/client.py
+-rw-r--r--   0        0        0      378 2023-05-26 14:59:05.621457 overwatch_client-0.1.3/overwatch_client/utils.py
+-rw-r--r--   0        0        0     1044 2023-05-26 14:59:05.621457 overwatch_client-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1713 1970-01-01 00:00:00.000000 overwatch_client-0.1.3/PKG-INFO
```

### Comparing `overwatch_client-0.1.2/README.md` & `overwatch_client-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `overwatch_client-0.1.2/overwatch_client/client.py` & `overwatch_client-0.1.3/overwatch_client/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os, sys
 import requests
 import time
-from typing import Optional, Sequence, Dict
+from typing import Optional, Sequence, Dict, Union
 from .utils import generate_uuid
 
 
 class HTTPClient:
     """The base client for communicating with an overwatch server and it's model registry.
 
     The client is used to register, patch, delete and infer on models with the overwatch server.
@@ -35,23 +35,27 @@
         """
         self.ow_server_url = overwatch_server_url
         self.model_registry_url = model_registry_url
         self.header_payload = {"key": header_key}
         self.inference_timer = []
         self.inference_counter = []
 
+        self.request_session = requests.Session()
+        self.request_session.headers.update(self.header_payload)
+        self.request_session.headers.update({"prediction-key": self.header_payload["key"]})
+
     def check_overwatch_server_connection(self) -> bool:
         """
         Checks if the Overwatch server is reachable.
 
         Returns:
             Bool: True if the Overwatch server is reachable.
         """
         try:
-            response = requests.get(f"{self.ow_server_url}/status", headers=self.header_payload)
+            response = self.request_session.get(f"{self.ow_server_url}/status")
             response.raise_for_status()
             return True
         except requests.exceptions.ConnectionError:
             return False
 
     def __get_file__(self, file_path: str) -> bytes:
         """
@@ -63,14 +67,67 @@
         Returns:
             bytes: The contents of the file as bytes.
         """
         with open(file_path, "rb") as f:
             ret_bytes: bytes = f.read()
         return ret_bytes
 
+    def signup(self, email: str, password: str) -> requests.Response:
+
+        url = f"{self.model_registry_url}/users/signup"
+
+        resp = self.request_session.post(
+            url = url,
+            data={
+                "email": email,
+                "password": password
+            }
+        )
+
+        self._email = email
+        self._password = password
+
+        self._session = resp.json()
+        self.request_session.headers.update({'Authorization': f'Bearer {self._session["session"]["access_token"]}'})
+
+        resp.raise_for_status()
+
+        return resp
+
+    def signin(self, email: Optional[str] = None, password: Optional[str] = None) -> requests.Response:
+
+        if email is None:
+            email = self._email
+        else:
+            self._email = email
+
+        if password is None:
+            password = self._password
+        else:
+            self._password = password
+
+
+        if email is None or password is None:
+            raise ValueError("Email and password are required. Make sure to sign in or sign up before running any other methods.")
+
+        url = f"{self.model_registry_url}/users/signin"
+
+        resp = self.request_session.post(
+            url = url,
+            data = {
+                "email": email,
+                "password": password
+            }
+        )
+
+        self._session = resp.json()
+        self.request_session.headers.update({'Authorization': f'Bearer {self._session["session"]["access_token"]}'})        
+
+        return resp
+
     def register_model_with_bytes(
         self,
         model_name: str,
         model_bytes: bytes,
         preprocess_bytes: bytes,
         postprocess_bytes: bytes,
         password: str = "DefaultPassword",
@@ -103,17 +160,16 @@
 
         files_payload = {
             "model": model_bytes,
             "preprocess": preprocess_bytes,
             "postprocess": postprocess_bytes,
         }
 
-        response = requests.post(
+        response = self.request_session.post(
             url,
-            headers=self.header_payload,
             data=data_payload,
             files=files_payload,
         )
         return response 
 
     def register_model(
         self,
@@ -186,17 +242,16 @@
 
         files_payload = {
             "model": self.__get_file__(model_path),
             "preprocess": self.__get_file__(preprocess_path),
             "postprocess": self.__get_file__(postprocess_path),
         }
 
-        response = requests.patch(
+        response = self.request_session.patch(
             url,
-            headers=self.header_payload,
             data=data_payload,
             files=files_payload,
         )
 
         response.raise_for_status()
 
         return response
@@ -212,24 +267,22 @@
             password (str): The associated password for the modelself.
 
         Returns:
             requests.Response: The response object from the model registry after deleting the model.
         """
         url = f"{self.model_registry_url}/models/{model_name}"
 
-        header_payload = {
-            "key": self.header_payload["key"],
-            "password": password,
-        }
+        self.request_session.headers.update({ 'password': password })
 
-        response = requests.delete(
+        response = self.request_session.delete(
             url,
-            headers=header_payload,
         )
 
+        self.request_session.headers.pop("password")
+
         response.raise_for_status()
 
         return response
 
     def get_model(self, model_name: str) -> requests.Response:
         """
         Retrieves a model from the model registry.
@@ -238,23 +291,23 @@
             model_name (str): The name of the model to retrieve.
 
         Returns:
             requests.Response: The response object from the model registry.
         """
         url = f"{self.model_registry_url}/models/{model_name}"
 
-        response = requests.get(url, headers=self.header_payload)
+        response = self.request_session.get(url)
 
         response.raise_for_status()
 
         return response
 
     def infer(
         self,
-        inputs: Sequence[bytes],
+        inputs: Union[Dict, Sequence[bytes]],
         model_name: str,
         slice_batch: int = 1,
         inference_id: Optional[str] = None,
         compute_group_info: Optional[str] = None,
     ) -> Dict:
         """
         Performs an inference on the provided inputs using the model specified. Returns 
@@ -274,26 +327,44 @@
             inference_id
             if inference_id is not None
             else f"{model_name}_{generate_uuid()}"
         )
         url = f"{self.ow_server_url}/Prediction/{inference_id}/detect/iterations/{model_name}/{slice_batch}"
         if compute_group_info is not None:
             url = f"{url}/{compute_group_info}"
-
+        
         files = {}
-        for ind, elem in enumerate(inputs):
-            files[f"{ind}"] = elem
+        if type(inputs) is dict:
+            files = inputs
+            for key in files:
+                assert type(files[key]) is bytes, f"Inputs must be bytes but got {type(files[key])} for key {key}"
+        elif type(inputs) is list:
+            for ind, elem in enumerate(inputs):
+                assert type(elem) is bytes, f"Inputs must be bytes but got {type(elem)} for index {ind}"
+                files[f"{ind}"] = elem
+        else:
+            raise TypeError("inputs must be a list or dict")
 
         start_time = time.time()
+        
+        if self._password is None and self._email is None:
+            response = self.request_session.post(
+                url,
+                files=files,
+            )
+        else:
+            response = self.request_session.post(
+                url,
+                data={
+                    "email": self._email,
+                    "password": self._password
+                },
+                files = files,
+            )
 
-        response = requests.post(
-            url,
-            headers= { "prediction-key": self.header_payload["key"] },
-            files=files,
-        )
 
         response.raise_for_status()
 
         end_time = time.time()
 
         self.inference_timer.append(end_time - start_time)
         self.inference_counter.append(len(inputs))
```

### Comparing `overwatch_client-0.1.2/pyproject.toml` & `overwatch_client-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overwatch-client"
-version = "0.1.2"
+version = "0.1.3"
 description = "A python based Overwatch Client for interacting with the overwatch server with higher level apis."
 authors = ["Hamada Gasmallah <hamada@distributive.network>"]
 readme = "README.md"
 packages = [{include = "overwatch_client"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `overwatch_client-0.1.2/PKG-INFO` & `overwatch_client-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overwatch-client
-Version: 0.1.2
+Version: 0.1.3
 Summary: A python based Overwatch Client for interacting with the overwatch server with higher level apis.
 Author: Hamada Gasmallah
 Author-email: hamada@distributive.network
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

