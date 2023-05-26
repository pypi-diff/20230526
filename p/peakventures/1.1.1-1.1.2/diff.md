# Comparing `tmp/peakventures-1.1.1.tar.gz` & `tmp/peakventures-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakventures-1.1.1.tar", max compression
+gzip compressed data, was "peakventures-1.1.2.tar", max compression
```

## Comparing `peakventures-1.1.1.tar` & `peakventures-1.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.1.1/peakventures/__init__.py
--rw-r--r--   0        0        0     1980 2023-05-26 10:32:01.899728 peakventures-1.1.1/peakventures/api.py
--rw-r--r--   0        0        0     1153 2023-05-26 10:31:37.185812 peakventures-1.1.1/peakventures/credentials.py
--rw-r--r--   0        0        0     1336 2023-05-26 10:32:19.525020 peakventures-1.1.1/peakventures/storage.py
--rw-r--r--   0        0        0      376 2023-05-26 10:48:52.026638 peakventures-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.1.1/setup.py
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.1.2/peakventures/__init__.py
+-rw-r--r--   0        0        0     2041 2023-05-26 10:51:38.348267 peakventures-1.1.2/peakventures/api.py
+-rw-r--r--   0        0        0     1153 2023-05-26 10:31:37.185812 peakventures-1.1.2/peakventures/credentials.py
+-rw-r--r--   0        0        0     1336 2023-05-26 10:32:19.525020 peakventures-1.1.2/peakventures/storage.py
+-rw-r--r--   0        0        0      376 2023-05-26 10:51:47.258190 peakventures-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.1.2/setup.py
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.1.2/PKG-INFO
```

### Comparing `peakventures-1.1.1/peakventures/api.py` & `peakventures-1.1.2/peakventures/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -54,14 +54,15 @@
         "type": "sellside",
         "weights": weights
     })
 
     v2_response.raise_for_status()
 
 
+@retry(wait=wait_exponential(1), stop=stop_after_attempt(3))
 def get_topic_afd_domains(topic: str) -> list:
     """Get topic AFD domains."""
     session = _get_session()
 
     response = session.get(f"{BASE_URL_V2}/topics/{topic}")
     response.raise_for_status()
```

### Comparing `peakventures-1.1.1/peakventures/credentials.py` & `peakventures-1.1.2/peakventures/credentials.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.1.1/peakventures/storage.py` & `peakventures-1.1.2/peakventures/storage.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.1.1/setup.py` & `peakventures-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['azure-storage-blob>=12.16.0,<13.0.0',
  'boto3>=1.26.141,<2.0.0',
  'tenacity>=8.2.2,<9.0.0']
 
 setup_kwargs = {
     'name': 'peakventures',
-    'version': '1.1.1',
+    'version': '1.1.2',
     'description': 'PeakVentures Python Utilities for DataBricks',
     'long_description': 'None',
     'author': 'Volodymyr Smirnov',
     'author_email': 'volodymyr@peakventures.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `peakventures-1.1.1/PKG-INFO` & `peakventures-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakventures
-Version: 1.1.1
+Version: 1.1.2
 Summary: PeakVentures Python Utilities for DataBricks
 Author: Volodymyr Smirnov
 Author-email: volodymyr@peakventures.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

