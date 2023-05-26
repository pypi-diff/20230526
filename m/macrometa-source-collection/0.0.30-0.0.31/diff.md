# Comparing `tmp/macrometa-source-collection-0.0.30.tar.gz` & `tmp/macrometa-source-collection-0.0.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-source-collection-0.0.30.tar", max compression
+gzip compressed data, was "macrometa-source-collection-0.0.31.tar", max compression
```

## Comparing `macrometa-source-collection-0.0.30.tar` & `macrometa-source-collection-0.0.31.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8346 2023-05-15 08:26:35.052074 macrometa-source-collection-0.0.30/macrometa_source_collection/__init__.py
--rw-r--r--   0        0        0     8499 2023-05-15 08:26:35.052074 macrometa-source-collection-0.0.30/macrometa_source_collection/client.py
--rw-r--r--   0        0        0     1623 2023-05-15 08:26:35.312074 macrometa-source-collection-0.0.30/pyproject.toml
--rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.30/setup.py
--rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.30/PKG-INFO
+-rw-r--r--   0        0        0     8701 2023-05-26 06:41:14.698075 macrometa-source-collection-0.0.31/macrometa_source_collection/__init__.py
+-rw-r--r--   0        0        0     8501 2023-05-26 06:41:14.698075 macrometa-source-collection-0.0.31/macrometa_source_collection/client.py
+-rw-r--r--   0        0        0     1623 2023-05-26 06:41:14.946075 macrometa-source-collection-0.0.31/pyproject.toml
+-rw-r--r--   0        0        0     1074 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.31/setup.py
+-rw-r--r--   0        0        0     1157 1970-01-01 00:00:00.000000 macrometa-source-collection-0.0.31/PKG-INFO
```

### Comparing `macrometa-source-collection-0.0.30/macrometa_source_collection/__init__.py` & `macrometa-source-collection-0.0.31/macrometa_source_collection/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """GDN data connector source for GDN Collections."""
 from collections import defaultdict
+from urllib.parse import urlparse
 
 import pkg_resources
 import singer
 from c8 import C8Client
 from c8connector import C8Connector, Sample, ConfigProperty, ConfigAttributeType, Schema, SchemaAttributeType, \
     SchemaAttribute
-from macrometa_source_collection.client import GDNCollectionClient, get_singer_data_type
 from singer import utils
 from singer.catalog import Catalog, CatalogEntry
 from singer.schema import Schema as SingerSchema
 
+from macrometa_source_collection.client import GDNCollectionClient, get_singer_data_type
+
 LOGGER = singer.get_logger('macrometa_source_collection')
 
 REQUIRED_CONFIG_KEYS = [
-    'region',
+    'gdn_host',
     'fabric',
     'api_key',
     'source_collection'
 ]
 
 
 class GDNCollectionSourceConnector(C8Connector):
@@ -51,27 +53,27 @@
     def validate(self, integration: dict) -> None:
         """Validate given configurations against the connector.
         If invalid, throw an exception with the cause.
         """
         config = self.get_config(integration)
         C8Client(
             "https",
-            host=config["region"],
+            host=config["gdn_host"],
             port=443,
             geofabric=config["fabric"],
             apikey=config["api_key"]
         ).collection(config["source_collection"])
         pass
 
     def samples(self, integration: dict) -> list[Sample]:
         """Fetch sample data using the given configurations."""
         config = self.get_config(integration)
         schema, data = get_schema_and_data(C8Client(
             "https",
-            host=config["region"],
+            host=config["gdn_host"],
             port=443,
             geofabric=config["fabric"],
             apikey=config["api_key"]
         ), config["source_collection"], 50)
         data = data[:10]
         return [Sample(
             schema=Schema(config["source_collection"],
@@ -80,38 +82,38 @@
         )]
 
     def schemas(self, integration: dict) -> list[Schema]:
         """Get supported schemas using the given configurations."""
         config = self.get_config(integration)
         schema, _ = get_schema_and_data(C8Client(
             "https",
-            host=config["region"],
+            host=config["gdn_host"],
             port=443,
             geofabric=config["fabric"],
             apikey=config["api_key"]
         ), config["source_collection"], 50)
         return [Schema(config["source_collection"],
                        [SchemaAttribute(k, get_attribute_type(v)) for k, v in schema.items()])]
 
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
         return []
 
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
-            ConfigProperty('region', 'Region URL', ConfigAttributeType.STRING, True, False,
-                           description='Fully qualified region URL.',
-                           placeholder_value='api-sample-ap-west.eng.macrometa.io'),
+            ConfigProperty('gdn_host', 'GDN Host', ConfigAttributeType.STRING, True, False,
+                           description='Fully qualified GDN Host URL (note: Use Global URL for Global collections).',
+                           placeholder_value='sample-dxb.paas.macrometa.io'),
+            ConfigProperty('api_key', 'API Key', ConfigAttributeType.PASSWORD, True, False,
+                           description='API key.',
+                           placeholder_value='my_apikey'),
             ConfigProperty('fabric', 'Fabric', ConfigAttributeType.STRING, True, False,
                            description='Fabric name.',
                            default_value='_system'),
-            ConfigProperty('api_key', 'API Key', ConfigAttributeType.STRING, True, False,
-                           description='API key.',
-                           placeholder_value='my_apikey'),
             ConfigProperty('source_collection', 'Source Collection', ConfigAttributeType.STRING, True, True,
                            description='Source collection name.',
                            placeholder_value='my_collection')
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
@@ -120,15 +122,15 @@
         return ['catalog', 'discover', 'state']
 
     @staticmethod
     def get_config(integration: dict) -> dict:
         try:
             return {
                 # Required config keys
-                'region': integration['region'],
+                'gdn_host': extract_gdn_host(integration['gdn_host']),
                 'api_key': integration['api_key'],
                 'fabric': integration['fabric'],
                 'source_collection': integration['source_collection']
             }
         except KeyError as e:
             raise KeyError(f'Integration property `{e}` not found.')
 
@@ -176,15 +178,15 @@
         return SchemaAttributeType.OBJECT
 
 
 def do_discovery(config):
     collection_name = config['source_collection']
     schema, _ = get_schema_and_data(C8Client(
         "https",
-        host=config["region"],
+        host=config["gdn_host"],
         port=443,
         geofabric=config["fabric"],
         apikey=config["api_key"]
     ), collection_name, 50)
     schema_properties = {k: SingerSchema(type=v, format=None) for k, v in schema.items()}
     # inject `_sdc_deleted_at` prop to the schema.
     schema_properties['_sdc_deleted_at'] = SingerSchema(type=['null', 'string'], format='date-time')
@@ -205,18 +207,26 @@
 
 
 def do_sync(conn_config, catalog, default_replication_method):
     client = GDNCollectionClient(conn_config)
     client.sync(catalog.streams[0])
 
 
+def extract_gdn_host(url):
+    parsed_url = urlparse(url)
+    resource_name = parsed_url.netloc.strip()
+    if not resource_name.startswith("api-"):
+        resource_name = "api-" + resource_name
+    return resource_name
+
+
 def main_impl():
     args = utils.parse_args(REQUIRED_CONFIG_KEYS)
     conn_config = {'api_key': args.config['api_key'],
-                   'region': args.config['region'],
+                   'gdn_host': extract_gdn_host(args.config['gdn_host']),
                    'fabric': args.config['fabric'],
                    'source_collection': args.config['source_collection']}
 
     if args.discover:
         do_discovery(conn_config)
     elif args.catalog:
         do_sync(conn_config, args.catalog, args.config.get('default_replication_method'))
```

### Comparing `macrometa-source-collection-0.0.30/macrometa_source_collection/client.py` & `macrometa-source-collection-0.0.31/macrometa_source_collection/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 is_metrics_enabled = os.getenv("MACROMETA_SOURCE_COLLECTION_IS_METRICS_ENABLED", 'False')
 
 class GDNCollectionClient:
     """Client for handling GDN collection streams."""
 
     def __init__(self, config) -> None:
         """Init new GDN Collection Client."""
-        self._host = config.get("region")
+        self._host = config.get("gdn_host")
         self._fabric = config.get("fabric")
         _apikey = config.get("api_key")
         self._wf_uuid = os.getenv('WORKFLOW_UUID')
         self._collection = config.get("source_collection")
         self._c8_client = C8Client(
             "https",
             host=self._host,
```

### Comparing `macrometa-source-collection-0.0.30/pyproject.toml` & `macrometa-source-collection-0.0.31/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core", "wheel"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "macrometa-source-collection"
-version='0.0.30'
+version='0.0.31'
 description = "Pipelinewise tap for reading from GDN Collections"
 license = "Apache-2.0"
 authors = ["Macrometa <info@macrometa.com>"]
 keywords = [
     "ELT",
     "Connectors",
     "Workflows",
```

### Comparing `macrometa-source-collection-0.0.30/setup.py` & `macrometa-source-collection-0.0.31/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 entry_points = \
 {'console_scripts': ['macrometa-source-collection = '
                      'macrometa_source_collection:main']}
 
 setup_kwargs = {
     'name': 'macrometa-source-collection',
-    'version': '0.0.30',
+    'version': '0.0.31',
     'description': 'Pipelinewise tap for reading from GDN Collections',
     'long_description': 'None',
     'author': 'Macrometa',
     'author_email': 'info@macrometa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `macrometa-source-collection-0.0.30/PKG-INFO` & `macrometa-source-collection-0.0.31/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-source-collection
-Version: 0.0.30
+Version: 0.0.31
 Summary: Pipelinewise tap for reading from GDN Collections
 License: Apache-2.0
 Keywords: ELT,Connectors,Workflows,Macrometa,GDN,Collection,Tap
 Author: Macrometa
 Author-email: info@macrometa.com
 Requires-Python: >=3.8.1,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
```

