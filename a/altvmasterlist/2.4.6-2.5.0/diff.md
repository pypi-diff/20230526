# Comparing `tmp/altvmasterlist-2.4.6.tar.gz` & `tmp/altvmasterlist-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "altvmasterlist-2.4.6.tar", max compression
+gzip compressed data, was "altvmasterlist-2.5.0.tar", max compression
```

## Comparing `altvmasterlist-2.4.6.tar` & `altvmasterlist-2.5.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    16725 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/LICENSE
--rw-r--r--   0        0        0      425 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/README.md
--rw-r--r--   0        0        0     1053 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/pyproject.toml
--rw-r--r--   0        0        0      402 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/src/altvmasterlist/__init__.py
--rw-r--r--   0        0        0     6960 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/src/altvmasterlist/altstats.py
--rw-r--r--   0        0        0     9658 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/src/altvmasterlist/masterlist.py
--rw-r--r--   0        0        0    10974 2023-04-25 08:50:27.617214 altvmasterlist-2.4.6/src/altvmasterlist/shared.py
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 altvmasterlist-2.4.6/PKG-INFO
+-rw-r--r--   0        0        0    16725 2023-05-26 12:19:41.827143 altvmasterlist-2.5.0/LICENSE
+-rw-r--r--   0        0        0      425 2023-05-26 12:19:41.827143 altvmasterlist-2.5.0/README.md
+-rw-r--r--   0        0        0     1073 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0      402 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/src/altvmasterlist/__init__.py
+-rw-r--r--   0        0        0     6960 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/src/altvmasterlist/altstats.py
+-rw-r--r--   0        0        0     9658 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/src/altvmasterlist/masterlist.py
+-rw-r--r--   0        0        0    11294 2023-05-26 12:19:41.831143 altvmasterlist-2.5.0/src/altvmasterlist/shared.py
+-rw-r--r--   0        0        0     1367 1970-01-01 00:00:00.000000 altvmasterlist-2.5.0/PKG-INFO
```

### Comparing `altvmasterlist-2.4.6/LICENSE` & `altvmasterlist-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.6/pyproject.toml` & `altvmasterlist-2.5.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "altvmasterlist"
-version = "2.4.6"
+version = "2.5.0"
 description = "A package to use the alt:V Masterlist api."
 authors = ["Nickwasused <contact.nickwasused.fa6c8@simplelogin.co>"]
 license = "MPL-2.0"
 readme = "README.md"
 repository = "https://github.com/Nickwasused/altv-python-masterlist"
 documentation = "https://nickwasused.github.io/altv-python-masterlist/"
 classifiers = [
@@ -15,14 +15,15 @@
 ]
 packages = [
     { include = "altvmasterlist", from = "src" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.11"
+requests= "^2.31.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.0"
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
```

### Comparing `altvmasterlist-2.4.6/src/altvmasterlist/altstats.py` & `altvmasterlist-2.5.0/src/altvmasterlist/altstats.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.6/src/altvmasterlist/masterlist.py` & `altvmasterlist-2.5.0/src/altvmasterlist/masterlist.py`

 * *Files identical despite different names*

### Comparing `altvmasterlist-2.4.6/src/altvmasterlist/shared.py` & `altvmasterlist-2.5.0/src/altvmasterlist/shared.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
-from urllib.request import urlopen, Request
+from requests.adapters import HTTPAdapter, Retry
 from dataclasses import dataclass
-from json import dumps, loads
+from json import dumps
 from io import StringIO
 from enum import Enum
+import requests
 import logging
 import secrets
 
 logging.basicConfig(level=logging.INFO)
 logging.getLogger().setLevel(logging.INFO)
 
 
@@ -83,33 +84,36 @@
 
     Returns:
         None: When an error occurred. But exceptions will still be logged!
         json: As data
     """
     # Use the User-Agent: AltPublicAgent, because some servers protect their CDN with
     # a simple User-Agent check e.g. https://luckyv.de does that
-    if "http://" in url and cdn:
-        req_headers = RequestHeaders(server.version, server.branch)
-    else:
-        req_headers = {
-            'User-Agent': Extra.user_agent.value,
-            'content-type': 'application/json; charset=utf-8'
-        }
-
-    try:
-        api_request = Request(url, headers=req_headers, method="GET")
-        with urlopen(api_request, timeout=60) as api_data:
-            if api_data.status != 200:
+    with requests.session() as session:
+        retries = Retry(total=5, backoff_factor=1, status_forcelist=[502, 503, 504])
+        session.mount('http', HTTPAdapter(max_retries=retries))
+
+        if "http://" in url and cdn:
+            session.headers = RequestHeaders(server.version, server.branch)
+        else:
+            session.headers = {
+                'User-Agent': Extra.user_agent.value,
+                'content-type': 'application/json; charset=utf-8'
+            }
+
+        try:
+            api_request = session.get(url, timeout=20)
+            if api_request.status_code != 200:
                 logging.warning(f"the request returned nothing.")
                 return None
             else:
-                return loads(api_data.read().decode("utf-8", errors='ignore'))
-    except Exception as e:
-        logging.error(e)
-        return None
+                return api_request.json()
+        except Exception as e:
+            logging.error(e)
+            return None
 
 
 def get_dtc_url(use_cdn: bool, cdn_url: str, host: str, port: int, locked: bool, password: str = None) -> str | None:
     """This function gets the direct connect protocol url of an alt:V Server.
         (https://docs.altv.mp/articles/connectprotocol.html)
 
     Args:
@@ -289,14 +293,18 @@
         float: The size of the resource.
     """
     if use_cdn:
         resource_url = f"{cdn_url}/{resource}.resource"
     else:
         resource_url = f"http://{host}:{port}/{resource}.resource"
 
-    size_request = Request(resource_url, headers={"User-Agent": Extra.user_agent.value}, method="HEAD")
+    with requests.session() as session:
+        retries = Retry(total=5, backoff_factor=1, status_forcelist=[502, 503, 504])
+        session.mount('http', HTTPAdapter(max_retries=retries))
+        session.headers = {"User-Agent": Extra.user_agent.value}
+
+        size_request = session.head(resource_url, timeout=20)
 
-    with urlopen(size_request, timeout=60) as size_data:
-        if size_data.status == 200:
-            return round((int(size_data.headers["Content-Length"]) / 1048576), decimal)
+        if size_request.status_code == 200:
+            return round((int(size_request.headers["Content-Length"]) / 1048576), decimal)
         else:
             return None
```

### Comparing `altvmasterlist-2.4.6/PKG-INFO` & `altvmasterlist-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: altvmasterlist
-Version: 2.4.6
+Version: 2.5.0
 Summary: A package to use the alt:V Masterlist api.
 Home-page: https://github.com/Nickwasused/altv-python-masterlist
 License: MPL-2.0
 Author: Nickwasused
 Author-email: contact.nickwasused.fa6c8@simplelogin.co
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/Nickwasused/altv-python-masterlist/issues
 Project-URL: Documentation, https://nickwasused.github.io/altv-python-masterlist/
 Project-URL: Repository, https://github.com/Nickwasused/altv-python-masterlist
 Description-Content-Type: text/markdown
 
 # alt:V Masterlist for Python
```

