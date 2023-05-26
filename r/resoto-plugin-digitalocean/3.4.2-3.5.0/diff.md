# Comparing `tmp/resoto-plugin-digitalocean-3.4.2.tar.gz` & `tmp/resoto-plugin-digitalocean-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-digitalocean-3.4.2.tar", last modified: Wed May 10 12:22:16 2023, max compression
+gzip compressed data, was "resoto-plugin-digitalocean-3.5.0.tar", last modified: Fri May 26 18:24:03 2023, max compression
```

## Comparing `resoto-plugin-digitalocean-3.4.2.tar` & `resoto-plugin-digitalocean-3.5.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:16.114955 resoto-plugin-digitalocean-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-10 12:22:16.114955 resoto-plugin-digitalocean-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:16.110954 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15004 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    43556 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:16.110954 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-10 12:22:16.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-10 12:22:16.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:16.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-10 12:22:16.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:22:16.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-10 12:22:16.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-10 12:22:16.000000 resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-10 12:22:16.114955 resoto-plugin-digitalocean-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:16.110954 resoto-plugin-digitalocean-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:16.114955 resoto-plugin-digitalocean-3.4.2/test/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/alerts.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/cdns.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/certificates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/domain_records.py
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/domains.py
--rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/droplets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/firewalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/floatingip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/k8s.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/loadbalancers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/projectresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/projects.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/registry_repositories.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/registry_repository_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/snapshots.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/spaces.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/ssh_keys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/volumes.py
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/fixtures/vpcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/test_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 12:19:34.000000 resoto-plugin-digitalocean-3.4.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.665267 resoto-plugin-digitalocean-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 18:24:03.665267 resoto-plugin-digitalocean-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.657267 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15090 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43809 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19972 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.657267 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-26 18:24:03.000000 resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-26 18:24:03.665267 resoto-plugin-digitalocean-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.661267 resoto-plugin-digitalocean-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:03.665267 resoto-plugin-digitalocean-3.5.0/test/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/alerts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/cdns.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/certificates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1442 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/domain_records.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/domains.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10579 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/droplets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1436 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8942 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/floatingip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2064 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/k8s.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/loadbalancers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/projectresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/projects.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/registry_repositories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/registry_repository_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/snapshots.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/spaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/ssh_keys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3077 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/volumes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/fixtures/vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23723 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/test_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 18:21:36.000000 resoto-plugin-digitalocean-3.5.0/test/test_config.py
```

### Comparing `resoto-plugin-digitalocean-3.4.2/PKG-INFO` & `resoto-plugin-digitalocean-3.5.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto DigitalOcean Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/__init__.py` & `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/client.py` & `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import lru_cache
 from typing import List, Any, Optional, Union, TypeVar, Callable
 
 import boto3
 import requests
 from botocore.exceptions import EndpointConnectionError, HTTPClientError
 from retrying import retry as retry_decorator
+from urllib.parse import urljoin
 
 from resoto_plugin_digitalocean.utils import RetryableHttpError
 from resoto_plugin_digitalocean.utils import retry_on_error
 from resotolib.config import Config
 from resotolib.core.actions import CoreFeedback
 from resotolib.types import Json
 
@@ -102,14 +103,15 @@
         payload = json_response.get(payload_object_name, [])
         result.extend(payload if isinstance(payload, list) else [payload])
 
         while json_response.get("links", {}).get("pages", {}).get("last", "") != url:
             url = json_response.get("links", {}).get("pages", {}).get("next", "")
             if url == "":
                 break
+            url = urljoin(self.do_api_endpoint, url)
             log.debug(f"fetching {url}")
             json_response = validate_status(requests.get(url, headers=self.headers, allow_redirects=True)).json()
             payload = json_response.get(payload_object_name, [])
             result.extend(payload if isinstance(payload, list) else [payload])
 
         log.debug(f"DO request {path} returned {len(result)} items")
         return result
```

### Comparing `resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/collector.py` & `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -577,15 +577,15 @@
             search_map={
                 "__users": [
                     "urn",
                     lambda vol: list(map(lambda id: droplet_id(id), vol["droplet_ids"])),
                 ],
                 "__tags": [
                     "urn",
-                    lambda v: list(map(lambda tag: tag_id(tag), v.get("tags", []))),
+                    lambda v: list(map(lambda tag: tag_id(tag), v.get("tags", []) or [])),
                 ],
             },
             predecessors={EdgeType.default: ["__users", "__tags"]},
             successors={EdgeType.delete: ["__users"]},
         )
 
     @metrics_collect_databases.time()  # type: ignore
@@ -736,14 +736,18 @@
                 return droplet_id(snapshot["resource_id"])
             else:
                 return volume_id(snapshot["resource_id"])
 
         def get_region(snapshot: Json) -> str:
             resource_id = get_resource_id(snapshot)
             resource = self.graph.search_first("urn", resource_id)
+            if resource is None:
+                # we can't find the instance for the snapshot,
+                # se we use the first region in the list returned by the API
+                return next(iter(snapshot.get("regions", [])), "unknown")
             region = region_id(resource.region().id)
             return region
 
         snapshots = self.client.list_snapshots()
         self.collect_resource(
             snapshots,
             resource_class=DigitalOceanSnapshot,
```

### Comparing `resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/resources.py` & `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean/utils.py` & `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/PKG-INFO` & `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-digitalocean
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto DigitalOcean Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/digitalocean
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-digitalocean-3.4.2/resoto_plugin_digitalocean.egg-info/SOURCES.txt` & `resoto-plugin-digitalocean-3.5.0/resoto_plugin_digitalocean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/setup.py` & `resoto-plugin-digitalocean-3.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-digitalocean",
-    version="3.4.2",
+    version="3.5.0",
     description="Resoto DigitalOcean Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={
         "resoto.plugins": ["digitalocean_collector = resoto_plugin_digitalocean:DigitalOceanCollectorPlugin"]
```

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/__init__.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/apps.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/apps.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/databases.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/databases.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/domain_records.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/domain_records.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/droplets.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/droplets.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/firewalls.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/firewalls.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/floatingip.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/floatingip.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/k8s.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/k8s.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/loadbalancers.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/loadbalancers.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/projectresources.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/projectresources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/projects.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/projects.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/regions.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/regions.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/registry_repositories.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/registry_repositories.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/tags.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/tags.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/fixtures/volumes.py` & `resoto-plugin-digitalocean-3.5.0/test/fixtures/volumes.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-digitalocean-3.4.2/test/test_collector.py` & `resoto-plugin-digitalocean-3.5.0/test/test_collector.py`

 * *Files identical despite different names*

