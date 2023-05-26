# Comparing `tmp/macrometa-target-collection-0.0.60.tar.gz` & `tmp/macrometa-target-collection-0.0.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "macrometa-target-collection-0.0.60.tar", last modified: Tue May 16 09:31:43 2023, max compression
+gzip compressed data, was "macrometa-target-collection-0.0.61.tar", last modified: Fri May 26 06:41:45 2023, max compression
```

## Comparing `macrometa-target-collection-0.0.60.tar` & `macrometa-target-collection-0.0.61.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/
--rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-16 09:31:22.000000 macrometa-target-collection-0.0.60/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-16 09:31:22.000000 macrometa-target-collection-0.0.60/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/macrometa_target_collection/
--rw-r--r--   0 runner    (1001) docker     (123)     3754 2023-05-16 09:31:22.000000 macrometa-target-collection-0.0.60/macrometa_target_collection/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14181 2023-05-16 09:31:22.000000 macrometa-target-collection-0.0.60/macrometa_target_collection/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 09:31:43.000000 macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-16 09:31:23.000000 macrometa-target-collection-0.0.60/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 09:31:43.852820 macrometa-target-collection-0.0.60/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/
+-rw-r--r--   0 runner    (1001) docker     (123)    10765 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/macrometa_target_collection/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/macrometa_target_collection/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14458 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/macrometa_target_collection/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13259 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-26 06:41:45.000000 macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-26 06:41:19.000000 macrometa-target-collection-0.0.61/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-26 06:41:45.971866 macrometa-target-collection-0.0.61/setup.cfg
```

### Comparing `macrometa-target-collection-0.0.60/LICENSE` & `macrometa-target-collection-0.0.61/LICENSE`

 * *Files identical despite different names*

### Comparing `macrometa-target-collection-0.0.60/PKG-INFO` & `macrometa-target-collection-0.0.61/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.60
+Version: 0.0.61
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.60/macrometa_target_collection/__init__.py` & `macrometa-target-collection-0.0.61/macrometa_target_collection/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """GDN data connector target for Macrometa GDN collections."""
+from urllib.parse import urlparse
+
 import pkg_resources
 from c8connector import C8Connector, Sample, ConfigAttributeType, Schema
 from c8connector import ConfigProperty
 
 
 class GDNCollectionTargetConnector(C8Connector):
     """GDNCollectionTargetConnector's C8Connector impl."""
@@ -48,17 +50,17 @@
     def reserved_keys(self) -> list[str]:
         """List of reserved keys for the connector."""
         return ["_key", "_id", "_rev"]
 
     def config(self) -> list[ConfigProperty]:
         """Get configuration parameters for the connector."""
         return [
-            ConfigProperty('region', 'Region URL', ConfigAttributeType.STRING, True, False,
-                           description="Fully qualified region URL.",
-                           placeholder_value='api-sample-ap-west.eng.macrometa.io'),
+            ConfigProperty('gdn_host', 'GDN Host', ConfigAttributeType.STRING, True, False,
+                           description='Fully qualified GDN Host URL (note: Use Global URL for Global collections).',
+                           placeholder_value='sample-dxb.paas.macrometa.io'),
             ConfigProperty('api_key', 'API Key', ConfigAttributeType.PASSWORD, True, False,
                            description="API key.",
                            placeholder_value='my_apikey'),
             ConfigProperty('fabric', 'Fabric', ConfigAttributeType.STRING, True, False,
                            description="Fabric name.",
                            default_value='_system'),
             ConfigProperty('target_collection', 'Target Collection', ConfigAttributeType.STRING, True, True,
@@ -78,7 +80,15 @@
         ]
 
     def capabilities(self) -> list[str]:
         """Return the capabilities[1] of the connector.
         [1] https://docs.meltano.com/contribute/plugins#how-to-test-a-tap
         """
         return []
+
+
+def extract_gdn_host(url):
+    parsed_url = urlparse(url)
+    resource_name = parsed_url.netloc.strip()
+    if not resource_name.startswith("api-"):
+        resource_name = "api-" + resource_name
+    return resource_name
```

### Comparing `macrometa-target-collection-0.0.60/macrometa_target_collection/main.py` & `macrometa-target-collection-0.0.61/macrometa_target_collection/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,54 +3,61 @@
 import argparse
 import asyncio
 import hashlib
 import io
 import json
 import os
 import re
-import requests
 import sys
 import time
 from asyncio import AbstractEventLoop
 from datetime import datetime, timezone
 from threading import Thread, Lock
 
 import jsonschema
+import requests
 from adjust_precision_for_schema import adjust_decimal_precision_for_schema
 from c8 import C8Client, DocumentInsertError
 from c8.collection import StandardCollection
 from jsonschema import Draft4Validator
 from prometheus_client import Counter, Gauge, start_http_server
 from singer import get_logger
 
+from macrometa_target_collection import extract_gdn_host
+
 logger = get_logger('macrometa_target_collection')
 
 DEFAULT_BATCH_SIZE_ROWS = 100
 DEFAULT_BATCH_FLUSH_INTERVAL = 10
 DEFAULT_MIN_BATCH_FLUSH_TIME_GAP = 10
 
 # Prometheus metrics
 ingested_bytes = Counter('ingested_bytes', 'Total number of bytes ingested', ['region', 'tenant', 'fabric', 'workflow'])
-ingested_documents = Counter('ingested_documents', 'Total number of documents ingested', ['region', 'tenant', 'fabric', 'workflow'])
-ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion', ['region', 'tenant', 'fabric', 'workflow'])
-ingest_lag = Gauge('ingest_lag', 'Average time lag between data changes in GDN collections and external data sources', ['region', 'tenant', 'fabric', 'workflow'])
-scrape_complete_flag = Counter("scrape_complete_flag", "Flag to check if the last scrape has been completed", ['workflow'])
+ingested_documents = Counter('ingested_documents', 'Total number of documents ingested',
+                             ['region', 'tenant', 'fabric', 'workflow'])
+ingest_errors = Counter('ingest_errors', 'Total number of errors during ingestion',
+                        ['region', 'tenant', 'fabric', 'workflow'])
+ingest_lag = Gauge('ingest_lag', 'Average time lag between data changes in GDN collections and external data sources',
+                   ['region', 'tenant', 'fabric', 'workflow'])
+scrape_complete_flag = Counter("scrape_complete_flag", "Flag to check if the last scrape has been completed",
+                               ['workflow'])
 
 region_label = os.getenv("GDN_FEDERATION", "NA")
 tenant_label = os.getenv("GDN_TENANT", "NA")
 fabric_label = os.getenv("GDN_FABRIC", "NA")
 workflow_label = os.getenv("WORKFLOW_UUID", "NA")
 metric_service_url = os.getenv("METRIC_SERVICE_API")
 is_metrics_enabled = os.getenv("MACROMETA_TARGET_COLLECTION_IS_METRICS_ENABLED", 'False')
 
 # Start the Prometheus HTTP server for exposing metrics
 if is_metrics_enabled.lower() == 'true':
     logger.info("Target is starting the metrics server.")
     start_http_server(8000)
 
+
 class RecordBatch:
     """Class wrapping the record batch in order to make it thread safe."""
 
     def __init__(self, config: dict):
         self._list = list()
         self._lock = Lock()
         self.interval = config.get('batch_flush_interval', DEFAULT_BATCH_FLUSH_INTERVAL)
@@ -108,15 +115,16 @@
                 if type(r) is DocumentInsertError:
                     # Increment ingest_errors metric
                     ingest_errors.labels(region_label, tenant_label, fabric_label, workflow_label).inc()
                     print(f'Failed to insert/update record: {to_update[i]}. {r}')
                 else:
                     # Update ingest_lag metric
                     diff = datetime.now(timezone.utc) - ensure_datetime(to_update[i]["time_extracted"])
-                    ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(diff.total_seconds())
+                    ingest_lag.labels(region_label, tenant_label, fabric_label, workflow_label).set(
+                        diff.total_seconds())
         record_batch.last_executed_time = datetime.now(timezone.utc)
 
 
 def remove_time_extracted(records):
     return [{k: v for k, v in record.items() if k != 'time_extracted'} for record in records]
 
 
@@ -186,15 +194,16 @@
                             while True:
                                 if rec.get(new_key):
                                     new_key = "_" + new_key
                                 else:
                                     break
                             rec[new_key] = rec.pop(reserved_key)
 
-                    if _key and not (1 <= len(_key) <= 254 and bool(re.match("^[-_!\$%'\(\)\*\+,\.:;=@a-zA-Z0-9]+$", _key))):
+                    if _key and not (
+                            1 <= len(_key) <= 254 and bool(re.match("^[-_!\$%'\(\)\*\+,\.:;=@a-zA-Z0-9]+$", _key))):
                         hashed_key = hashlib.sha256(_key.encode('utf-8'))
                         _key = hashed_key.hexdigest()
                         logger.info(f"Primary key of the source doesn't satisfy the constraints of macrometa "
                                     f"document key, Hashing the key and using it in hex form to make it compliant.")
                     if _key:
                         rec['_key'] = _key
                 except:
@@ -274,21 +283,21 @@
     parser.add_argument('-c', '--config', help='Config file')
     args = parser.parse_args()
     if args.config:
         with open(args.config) as input_json:
             config = json.load(input_json)
     else:
         raise Exception("Required '--config' parameter was not provided")
-    region = config['region']
+    gdn_host = extract_gdn_host(config['gdn_host'])
     fabric = config['fabric']
     apikey = config['api_key']
     target_collection = config['target_collection']
     client = C8Client(
         protocol='https',
-        host=region,
+        host=gdn_host,
         port=443,
         apikey=apikey,
         geofabric=fabric
     )
 
     if not client.has_collection(target_collection):
         client.create_collection(name=target_collection)
@@ -301,15 +310,16 @@
 
     # There can still be records in the `record_batch` which is not processed,
     # So, we have to force process it one last time before the workflow terminates.
     try_upsert(collection, record_batch, force=True)
 
     if is_metrics_enabled.lower() == 'true':
         # Wait for Prometheus to scrape the metrics
-        while not is_scrape_complete(metric_service_url, f"{scrape_complete_flag._name}_total", f"workflow=\"{workflow_label}\""):
+        while not is_scrape_complete(metric_service_url, f"{scrape_complete_flag._name}_total",
+                                     f"workflow=\"{workflow_label}\""):
             logger.info("Waiting for metrics scrape...")
             time.sleep(15)
         logger.info("Metrics scrape complete. Exiting...")
 
     emit_state(state)
     event_loop.stop()
     logger.info("Completing normally...")
```

### Comparing `macrometa-target-collection-0.0.60/macrometa_target_collection.egg-info/PKG-INFO` & `macrometa-target-collection-0.0.61/macrometa_target_collection.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: macrometa-target-collection
-Version: 0.0.60
+Version: 0.0.61
 Summary: Singer.io target for writing to Macrometa GDN collections
 Author-email: Macrometa <info@macrometa.co>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
```

### Comparing `macrometa-target-collection-0.0.60/pyproject.toml` & `macrometa-target-collection-0.0.61/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "macrometa-target-collection"
-version = "0.0.60"
+version = "0.0.61"
 authors = [
     { name = "Macrometa", email = "info@macrometa.co" },
 ]
 description = "Singer.io target for writing to Macrometa GDN collections"
 readme = "README.md"
 license = { file = "LICENSE" }
 requires-python = ">=3.7"
```

