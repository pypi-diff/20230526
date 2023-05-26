# Comparing `tmp/peakventures-1.0.5.tar.gz` & `tmp/peakventures-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakventures-1.0.5.tar", max compression
+gzip compressed data, was "peakventures-1.1.0.tar", max compression
```

## Comparing `peakventures-1.0.5.tar` & `peakventures-1.1.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.0.5/peakventures/__init__.py
--rw-r--r--   0        0        0     2009 2023-05-26 08:53:42.012180 peakventures-1.0.5/peakventures/api.py
--rw-r--r--   0        0        0     1086 2023-05-26 10:15:43.554430 peakventures-1.0.5/peakventures/credentials.py
--rw-r--r--   0        0        0     1388 2023-05-26 08:53:41.460452 peakventures-1.0.5/peakventures/storage.py
--rw-r--r--   0        0        0      442 2023-05-26 10:17:04.500340 peakventures-1.0.5/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.0.5/setup.py
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.1.0/peakventures/__init__.py
+-rw-r--r--   0        0        0     1980 2023-05-26 10:32:01.899728 peakventures-1.1.0/peakventures/api.py
+-rw-r--r--   0        0        0     1153 2023-05-26 10:31:37.185812 peakventures-1.1.0/peakventures/credentials.py
+-rw-r--r--   0        0        0     1336 2023-05-26 10:32:19.525020 peakventures-1.1.0/peakventures/storage.py
+-rw-r--r--   0        0        0      376 2023-05-26 10:30:01.793196 peakventures-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.1.0/setup.py
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.1.0/PKG-INFO
```

### Comparing `peakventures-1.0.5/peakventures/api.py` & `peakventures-1.1.0/peakventures/api.py`

 * *Files 9% similar despite different names*

```diff
@@ -54,23 +54,24 @@
         "type": "sellside",
         "weights": weights
     })
 
     v2_response.raise_for_status()
 
 
-def get_topic_domains(topic: str) -> list:
-    """Get topic domains."""
+def get_topic_afd_domains(topic: str) -> list:
+    """Get topic AFD domains."""
     session = _get_session()
 
     response = session.get(f"{BASE_URL_V2}/topics/{topic}")
     response.raise_for_status()
 
     topic = response.json()
 
-    return topic["campaigns"]
+    return topic["properties"]["afdMappings"]
 
 
-if __name__ == "__main__":
-    get_topic_domains("a:b:c:d")
-    update_sellside_keywords_weights\
-        ("a:b:c:d", {"a": 1, "b": 2, "c": 3, "d": 4})
+__all__ = [
+    "get_topic",
+    "get_topic_afd_domains",
+    "update_sellside_keywords_weights"
+]
```

### Comparing `peakventures-1.0.5/peakventures/credentials.py` & `peakventures-1.1.0/peakventures/credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,7 +34,13 @@
     """Get credentials from the remote storage."""
     return _get_credential(name)
 
 
 def get_credentials_json(name: str) -> Any:
     """Get credentials from the remote storage."""
     return json.loads(get_credentials(name))
+
+
+__all__ = [
+    "get_credentials",
+    "get_credentials_json",
+]
```

### Comparing `peakventures-1.0.5/peakventures/storage.py` & `peakventures-1.1.0/peakventures/storage.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
-from typing import Any
 from io import BytesIO
+from typing import Any
 
 import boto3
-
 from azure.storage.blob import BlobClient, BlobServiceClient
 
 from peakventures.credentials import get_credentials, get_credentials_json, AZURE_CREDENTIALS_NAME, S3_CREDENTIALS_NAME
 
 CONTAINER_NAME = "models"
 
 
@@ -41,9 +40,10 @@
     """Store model on the remote storage."""
     json_payload = json.dumps(payload)
 
     _store_model_azure(name, json_payload)
     _store_model_s3(name, json_payload)
 
 
-if __name__ == "__main__":
-    store_model("test-model.json", dict(hello="world"))
+__all__ = [
+    "store_model"
+]
```

### Comparing `peakventures-1.0.5/setup.py` & `peakventures-1.1.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['azure-storage-blob>=12.16.0,<13.0.0',
  'boto3>=1.26.141,<2.0.0',
  'tenacity>=8.2.2,<9.0.0']
 
 setup_kwargs = {
     'name': 'peakventures',
-    'version': '1.0.5',
+    'version': '1.1.0',
     'description': 'PeakVentures Python Utilities for DataBricks',
     'long_description': 'None',
     'author': 'Volodymyr Smirnov',
     'author_email': 'volodymyr@peakventures.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `peakventures-1.0.5/PKG-INFO` & `peakventures-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakventures
-Version: 1.0.5
+Version: 1.1.0
 Summary: PeakVentures Python Utilities for DataBricks
 Author: Volodymyr Smirnov
 Author-email: volodymyr@peakventures.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

