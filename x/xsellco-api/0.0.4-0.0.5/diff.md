# Comparing `tmp/xsellco_api-0.0.4.tar.gz` & `tmp/xsellco_api-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xsellco_api-0.0.4.tar", last modified: Mon Feb 13 22:12:29 2023, max compression
+gzip compressed data, was "xsellco_api-0.0.5.tar", last modified: Fri May 26 03:15:15 2023, max compression
```

## Comparing `xsellco_api-0.0.4.tar` & `xsellco_api-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:12:29.889141 xsellco_api-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-13 22:12:29.889141 xsellco_api-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-02-13 22:12:29.889141 xsellco_api-0.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:12:29.889141 xsellco_api-0.0.4/xsellco_api/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/xsellco_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:12:29.889141 xsellco_api-0.0.4/xsellco_api/api/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/xsellco_api/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/xsellco_api/api/channels.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/xsellco_api/api/repricers.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/xsellco_api/api/users.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/xsellco_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-02-13 22:12:12.000000 xsellco_api-0.0.4/xsellco_api/info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 22:12:29.889141 xsellco_api-0.0.4/xsellco_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-02-13 22:12:29.000000 xsellco_api-0.0.4/xsellco_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-13 22:12:29.000000 xsellco_api-0.0.4/xsellco_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 22:12:29.000000 xsellco_api-0.0.4/xsellco_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-13 22:12:29.000000 xsellco_api-0.0.4/xsellco_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-13 22:12:29.000000 xsellco_api-0.0.4/xsellco_api.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:15:15.980592 xsellco_api-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-26 03:15:15.980592 xsellco_api-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-26 03:15:15.980592 xsellco_api-0.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:15:15.980592 xsellco_api-0.0.5/xsellco_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/xsellco_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:15:15.980592 xsellco_api-0.0.5/xsellco_api/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/xsellco_api/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/xsellco_api/api/channels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/xsellco_api/api/repricers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/xsellco_api/api/users.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1601 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/xsellco_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-26 03:15:00.000000 xsellco_api-0.0.5/xsellco_api/info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 03:15:15.980592 xsellco_api-0.0.5/xsellco_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-26 03:15:15.000000 xsellco_api-0.0.5/xsellco_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-26 03:15:15.000000 xsellco_api-0.0.5/xsellco_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 03:15:15.000000 xsellco_api-0.0.5/xsellco_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 03:15:15.000000 xsellco_api-0.0.5/xsellco_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 03:15:15.000000 xsellco_api-0.0.5/xsellco_api.egg-info/top_level.txt
```

### Comparing `xsellco_api-0.0.4/LICENSE` & `xsellco_api-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `xsellco_api-0.0.4/setup.py` & `xsellco_api-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `xsellco_api-0.0.4/xsellco_api/api/channels.py` & `xsellco_api-0.0.5/xsellco_api/api/channels.py`

 * *Files identical despite different names*

### Comparing `xsellco_api-0.0.4/xsellco_api/api/repricers.py` & `xsellco_api-0.0.5/xsellco_api/api/repricers.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 from io import StringIO
 from typing import Dict, List
 
 from xsellco_api.base import BaseClient
 
 
 class Repricers(BaseClient):
+    # Repricer have separate HOST for api calls
+    HOST = "api.repricer.com"
     endpoint = "repricers"
     header_text = "text/plain"
 
     def get_report(self) -> List[Dict]:
         headers = self.headers
         headers.update({"accept": self.header_text})
```

### Comparing `xsellco_api-0.0.4/xsellco_api/base.py` & `xsellco_api-0.0.5/xsellco_api/base.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 
 
 class BaseClient:
     SCHEME = "https://"
     HOST = "api.xsellco.com"
     API_VERSION = "v1"
     USER_AGENT = f"python-{__package_name__}-{__version__}"
-    URL = f"{SCHEME}{HOST}/{API_VERSION}"
 
     def __init__(self, user_name: str, password: str) -> None:
         self.user_name = user_name
         self.password = password
 
     @property
     def basic_auth(self) -> HTTPBasicAuth:
@@ -28,14 +27,18 @@
     def headers(self) -> Dict[str, str]:
         return {
             "user-agent": self.USER_AGENT,
             "accept": "application/json",
             "content-type": "application/json",
         }
 
+    @property
+    def url(self) -> str:
+        return f"{self.SCHEME}{self.HOST}/{self.API_VERSION}"
+
     def _request(
         self,
         method: str,
         endpoint: str,
         data=None,
         params: dict | None = None,
         headers: dict | None = None,
@@ -44,15 +47,15 @@
         if params is None:
             params = {}
         if data is None:
             data = {}
 
         resp = request(
             method,
-            f"{self.URL}/{endpoint}",
+            f"{self.url}/{endpoint}",
             params=params,
             data=data if data and method in ("POST", "PUT", "PATCH") else None,
             headers=headers or self.headers,
             auth=self.basic_auth,
             timeout=timeout,
         )
         return resp
```

