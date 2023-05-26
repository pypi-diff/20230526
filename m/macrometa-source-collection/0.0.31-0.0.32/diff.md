# Comparing `tmp/macrometa-source-collection-0.0.31.tar.gz` & `tmp/macrometa-source-collection-0.0.32.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.31.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.32.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.31.tar` & `macrometa-source-collection-0.0.32.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8701 2023-05-26 06:41:14.698075 macrometa-source-collection-0.0.31/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     8501 2023-05-26 06:41:14.698075 macrometa-source-collection-0.0.31/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-05-26 06:41:14.946075 macrometa-source-collection-0.0.31/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.31/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.31/PKG-INFO
+-rw-r--r--   0        0        0     8789 2023-05-26 07:04:41.639348 macrometa-source-collection-0.0.32/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     8501 2023-05-26 07:04:41.639348 macrometa-source-collection-0.0.32/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-05-26 07:04:41.879350 macrometa-source-collection-0.0.32/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.32/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.32/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.31/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.32/macrometa_source_collection/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,15 +209,18 @@
 def do_sync(conn_config, catalog, default_replication_method):
     client = GDNCollectionClient(conn_config)
     client.sync(catalog.streams[0])
 
 
 def extract_gdn_host(url):
     parsed_url = urlparse(url)
-    resource_name = parsed_url.netloc.strip()
+    if parsed_url.scheme:
+        resource_name = parsed_url.netloc.strip()
+    else:
+        resource_name = parsed_url.path.strip()
     if not resource_name.startswith("api-"):
         resource_name = "api-" + resource_name
     return resource_name
 
 
 def main_impl():
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
```

### Comparing `macrometa-source-collection-0.0.31/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.32/macrometa_source_collection/client.py`

 * *Files identical despite different names*

### Comparing `macrometa-source-collection-0.0.31/pyproject.toml` & `macrometa-source-collection-0.0.32/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.31'
+version='0.0.32'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.31/setup.py` & `macrometa-source-collection-0.0.32/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.31',
+    'version': '0.0.32',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.31/PKG-INFO` & `macrometa-source-collection-0.0.32/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.31
+Version: 0.0.32
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

