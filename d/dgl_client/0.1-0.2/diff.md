# Comparing `tmp/dgl_client-0.1.tar.gz` & `tmp/dgl_client-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dgl_client-0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "dgl_client-0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `dgl_client-0.1.tar` & `dgl_client-0.2.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0       36 2023-05-24 07:54:55.455568 dgl_client-0.1/.gitignore
--rw-r--r--   0        0        0       69 2023-05-24 07:54:55.456197 dgl_client-0.1/README.md
--rw-r--r--   0        0        0       62 2023-05-24 07:54:55.456771 dgl_client-0.1/dgl_client/__init__.py
--rw-r--r--   0        0        0     4502 2023-05-24 07:54:55.457252 dgl_client-0.1/dgl_client/api_cli.py
--rw-r--r--   0        0        0     3752 2023-05-24 07:54:55.457877 dgl_client-0.1/dgl_client/main.py
--rw-r--r--   0        0        0        0 2023-05-24 07:54:55.458038 dgl_client-0.1/dgl_client/utils.py
--rw-r--r--   0        0        0      438 2023-05-24 08:17:05.106570 dgl_client-0.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 07:54:55.460270 dgl_client-0.1/tests/__init__.py
--rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 dgl_client-0.1/PKG-INFO
+-rw-r--r--   0        0        0       36 2023-05-24 07:54:55.455568 dgl_client-0.2/.gitignore
+-rw-r--r--   0        0        0       69 2023-05-24 07:54:55.456197 dgl_client-0.2/README.md
+-rw-r--r--   0        0        0       62 2023-05-26 14:27:51.075075 dgl_client-0.2/dgl_client/__init__.py
+-rw-r--r--   0        0        0     5347 2023-05-26 14:29:12.176627 dgl_client-0.2/dgl_client/api_cli.py
+-rw-r--r--   0        0        0     3733 2023-05-24 08:36:13.792363 dgl_client-0.2/dgl_client/main.py
+-rw-r--r--   0        0        0        0 2023-05-24 07:54:55.458038 dgl_client-0.2/dgl_client/utils.py
+-rw-r--r--   0        0        0      438 2023-05-24 08:17:05.106570 dgl_client-0.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 07:54:55.460270 dgl_client-0.2/tests/__init__.py
+-rw-r--r--   0        0        0     1602 2023-05-26 14:26:13.928381 dgl_client-0.2/tests/test_decode.py
+-rw-r--r--   0        0        0      291 1970-01-01 00:00:00.000000 dgl_client-0.2/PKG-INFO
```

### Comparing `dgl_client-0.1/dgl_client/api_cli.py` & `dgl_client-0.2/dgl_client/api_cli.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,31 +4,67 @@
 import json
 import requests
 import sseclient
 import uuid
 
 logger = logging.getLogger(__name__)
 
+def login_check(endp, tok):
+    logger.info("Trying to login...")
+    username = None
+    try:
+      response = requests.get(
+          f"{endp}/auth/check",
+          json={},
+          headers={"Authorization": f"Bearer {tok}"},
+      )
+      response.raise_for_status()
+      username = response.json()
+    except:
+      pass
+
+    return username
+
+def refresh_token(endp, atok, rtok):
+    logger.info("Refreshing login token...")
+    new_tok = None
+    try:
+      response = requests.get(
+          f"{endp}/auth/refresh",
+          json={},
+          headers={
+              "Refresh": f"{rtok}"
+              },
+      )
+      response.raise_for_status()
+      new_tok = response.json()
+    except:
+      raise
+    logger.info("New token is %s"%str(new_tok))
+
+    return new_tok
+
 class APIClient:
     def __init__(self, backend_url, http_client=requests):
         self.backend_url = backend_url
         self.http_client = http_client
         self.auth_headers = None
         self.message_id = None
 
     def login(self, tokens):
-        self.auth_headers = {"Authorization": f"Bearer {bearer_token}"}
-        refresh_headers = {"Refresh": f"Bearer {bearer_token}"}
-        response = self.http_client.get(
-            f"{self.backend_url}/auth/check",
-            json={},
-            headers=self.auth_headers,
-        )
-        response.raise_for_status()
-        username = response.json()
+        print(tokens)
+        atok = tokens["access_token"]["access_token"] + "e"
+        rtok = tokens["refresh_token"]["access_token"]
+        self.auth_headers = {"Authorization": f"Bearer {atok}"}
+        username = login_check(self.backend_url, atok)
+        if username is None:
+          atok = refresh_token(self.backend_url, atok, rtok)
+          if atok:
+            username = login_check(self.backend_url, atok)
+
         logger.info(f"Logged in as {username}")
 
 
     def continue_chat(self, chat_id):
         self.chat_id = chat_id
         return self.chat_id
```

### Comparing `dgl_client-0.1/dgl_client/main.py` & `dgl_client-0.2/dgl_client/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,13 @@
     fileHandler = logging.FileHandler("{0}/{1}.log".format("logs", str(uuid.uuid4())))
     fileHandler.setFormatter(logFormatter)
     fileHandler.setLevel(logging.DEBUG)
     logger.addHandler(fileHandler)
 
     args.func(args)
   except Exception as e:
-    print(e)
     parser.print_help()
-    sys.exit(0)
+    raise
 
 
 if __name__ == "__main__":  
   main()
```

