# Comparing `tmp/peakventures-1.0.2.tar.gz` & `tmp/peakventures-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakventures-1.0.2.tar", max compression
+gzip compressed data, was "peakventures-1.0.3.tar", max compression
```

## Comparing `peakventures-1.0.2.tar` & `peakventures-1.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.0.2/peakventures/__init__.py
--rw-r--r--   0        0        0     2009 2023-05-26 08:53:42.012180 peakventures-1.0.2/peakventures/api.py
--rw-r--r--   0        0        0      904 2023-05-26 07:46:12.976714 peakventures-1.0.2/peakventures/credentials.py
--rw-r--r--   0        0        0     1388 2023-05-26 08:53:41.460452 peakventures-1.0.2/peakventures/storage.py
--rw-r--r--   0        0        0      442 2023-05-26 08:53:49.745032 peakventures-1.0.2/pyproject.toml
--rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.0.2/setup.py
--rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-26 05:31:43.775672 peakventures-1.0.3/peakventures/__init__.py
+-rw-r--r--   0        0        0     2009 2023-05-26 08:53:42.012180 peakventures-1.0.3/peakventures/api.py
+-rw-r--r--   0        0        0      903 2023-05-26 08:55:31.142153 peakventures-1.0.3/peakventures/credentials.py
+-rw-r--r--   0        0        0     1388 2023-05-26 08:53:41.460452 peakventures-1.0.3/peakventures/storage.py
+-rw-r--r--   0        0        0      442 2023-05-26 08:55:50.654744 peakventures-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0      725 1970-01-01 00:00:00.000000 peakventures-1.0.3/setup.py
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 peakventures-1.0.3/PKG-INFO
```

### Comparing `peakventures-1.0.2/peakventures/api.py` & `peakventures-1.0.3/peakventures/api.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.0.2/peakventures/credentials.py` & `peakventures-1.0.3/peakventures/credentials.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     if os.getenv("DEVELOPMENT"):
         result = {
             S3_CREDENTIALS_NAME: os.getenv("S3_CREDENTIALS"),
             AZURE_CREDENTIALS_NAME: os.getenv("AZURE_CREDENTIALS"),
             API_CREDENTIALS_NAME: os.getenv("API_CREDENTIALS")
         }.get(name)
     else:
-        result = dbtutils.secrets.get("credentials", name)
+        result = dbutils.secrets.get("credentials", name)
 
     if not result:
         raise ValueError(f"Credentials {name} not found.")
 
     return result
```

### Comparing `peakventures-1.0.2/peakventures/storage.py` & `peakventures-1.0.3/peakventures/storage.py`

 * *Files identical despite different names*

### Comparing `peakventures-1.0.2/setup.py` & `peakventures-1.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['azure-storage-blob>=12.16.0,<13.0.0',
  'boto3>=1.26.141,<2.0.0',
  'tenacity>=8.2.2,<9.0.0']
 
 setup_kwargs = {
     'name': 'peakventures',
-    'version': '1.0.2',
+    'version': '1.0.3',
     'description': 'PeakVentures Python Utilities for DataBricks',
     'long_description': 'None',
     'author': 'Volodymyr Smirnov',
     'author_email': 'volodymyr@peakventures.co',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `peakventures-1.0.2/PKG-INFO` & `peakventures-1.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakventures
-Version: 1.0.2
+Version: 1.0.3
 Summary: PeakVentures Python Utilities for DataBricks
 Author: Volodymyr Smirnov
 Author-email: volodymyr@peakventures.co
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

