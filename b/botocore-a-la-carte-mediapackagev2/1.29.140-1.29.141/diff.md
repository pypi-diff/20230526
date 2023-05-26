# Comparing `tmp/botocore-a-la-carte-mediapackagev2-1.29.140.tar.gz` & `tmp/botocore-a-la-carte-mediapackagev2-1.29.141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-mediapackagev2-1.29.140.tar", last modified: Thu May 25 01:17:46 2023, max compression
+gzip compressed data, was "botocore-a-la-carte-mediapackagev2-1.29.141.tar", last modified: Fri May 26 01:17:26 2023, max compression
```

## Comparing `botocore-a-la-carte-mediapackagev2-1.29.140.tar` & `botocore-a-la-carte-mediapackagev2-1.29.141.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:46.621184 botocore-a-la-carte-mediapackagev2-1.29.140/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-25 01:17:46.000000 botocore-a-la-carte-mediapackagev2-1.29.140/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-25 01:17:46.621184 botocore-a-la-carte-mediapackagev2-1.29.140/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:46.617184 botocore-a-la-carte-mediapackagev2-1.29.140/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:46.617184 botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:46.617184 botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:46.621184 botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/2022-12-25/
--rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-05-25 01:17:10.000000 botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/2022-12-25/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-25 01:17:10.000000 botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/2022-12-25/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (123)   109426 2023-05-25 01:17:10.000000 botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/2022-12-25/service-2.json
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-25 01:17:10.000000 botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/2022-12-25/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 01:17:46.621184 botocore-a-la-carte-mediapackagev2-1.29.140/botocore_a_la_carte_mediapackagev2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-25 01:17:46.000000 botocore-a-la-carte-mediapackagev2-1.29.140/botocore_a_la_carte_mediapackagev2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-25 01:17:46.000000 botocore-a-la-carte-mediapackagev2-1.29.140/botocore_a_la_carte_mediapackagev2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 01:17:46.000000 botocore-a-la-carte-mediapackagev2-1.29.140/botocore_a_la_carte_mediapackagev2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-25 01:17:46.000000 botocore-a-la-carte-mediapackagev2-1.29.140/botocore_a_la_carte_mediapackagev2.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 01:17:46.621184 botocore-a-la-carte-mediapackagev2-1.29.140/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-25 01:17:46.000000 botocore-a-la-carte-mediapackagev2-1.29.140/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:17:26.071740 botocore-a-la-carte-mediapackagev2-1.29.141/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-05-26 01:17:25.000000 botocore-a-la-carte-mediapackagev2-1.29.141/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-26 01:17:26.071740 botocore-a-la-carte-mediapackagev2-1.29.141/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:17:26.071740 botocore-a-la-carte-mediapackagev2-1.29.141/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:17:26.071740 botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:17:26.071740 botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:17:26.071740 botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/2022-12-25/
+-rw-r--r--   0 runner    (1001) docker     (123)    17656 2023-05-26 01:16:49.000000 botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/2022-12-25/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-26 01:16:49.000000 botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/2022-12-25/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (123)   109426 2023-05-26 01:16:49.000000 botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/2022-12-25/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 01:16:49.000000 botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/2022-12-25/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:17:26.071740 botocore-a-la-carte-mediapackagev2-1.29.141/botocore_a_la_carte_mediapackagev2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-26 01:17:26.000000 botocore-a-la-carte-mediapackagev2-1.29.141/botocore_a_la_carte_mediapackagev2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-26 01:17:26.000000 botocore-a-la-carte-mediapackagev2-1.29.141/botocore_a_la_carte_mediapackagev2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:17:26.000000 botocore-a-la-carte-mediapackagev2-1.29.141/botocore_a_la_carte_mediapackagev2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 01:17:26.000000 botocore-a-la-carte-mediapackagev2-1.29.141/botocore_a_la_carte_mediapackagev2.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:17:26.071740 botocore-a-la-carte-mediapackagev2-1.29.141/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 01:17:25.000000 botocore-a-la-carte-mediapackagev2-1.29.141/setup.py
```

### Comparing `botocore-a-la-carte-mediapackagev2-1.29.140/LICENSE.txt` & `botocore-a-la-carte-mediapackagev2-1.29.141/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-mediapackagev2-1.29.140/PKG-INFO` & `botocore-a-la-carte-mediapackagev2-1.29.141/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-mediapackagev2
-Version: 1.29.140
+Version: 1.29.141
 Summary: mediapackagev2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/2022-12-25/endpoint-rule-set-1.json` & `botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/2022-12-25/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/2022-12-25/paginators-1.json` & `botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/2022-12-25/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-mediapackagev2-1.29.140/botocore/data/mediapackagev2/2022-12-25/service-2.json` & `botocore-a-la-carte-mediapackagev2-1.29.141/botocore/data/mediapackagev2/2022-12-25/service-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-mediapackagev2-1.29.140/botocore_a_la_carte_mediapackagev2.egg-info/PKG-INFO` & `botocore-a-la-carte-mediapackagev2-1.29.141/botocore_a_la_carte_mediapackagev2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-mediapackagev2
-Version: 1.29.140
+Version: 1.29.141
 Summary: mediapackagev2 data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-mediapackagev2-1.29.140/setup.py` & `botocore-a-la-carte-mediapackagev2-1.29.141/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-mediapackagev2',
-    version="1.29.140",
+    version="1.29.141",
     description='mediapackagev2 data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/mediapackagev2/*/*.json'],
```

