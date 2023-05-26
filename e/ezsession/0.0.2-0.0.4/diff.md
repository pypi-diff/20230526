# Comparing `tmp/ezsession-0.0.2.tar.gz` & `tmp/ezsession-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ezsession-0.0.2.tar", last modified: Thu May 18 21:43:43 2023, max compression
+gzip compressed data, was "ezsession-0.0.4.tar", last modified: Fri May 26 14:45:39 2023, max compression
```

## Comparing `ezsession-0.0.2.tar` & `ezsession-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:43:43.463143 ezsession-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-18 21:43:43.463143 ezsession-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-18 21:43:29.000000 ezsession-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-18 21:43:29.000000 ezsession-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-18 21:43:43.463143 ezsession-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-18 21:43:29.000000 ezsession-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:43:43.463143 ezsession-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:43:43.463143 ezsession-0.0.2/src/ezsession/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-18 21:43:29.000000 ezsession-0.0.2/src/ezsession/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 21:43:43.463143 ezsession-0.0.2/src/ezsession.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-18 21:43:43.000000 ezsession-0.0.2/src/ezsession.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-18 21:43:43.000000 ezsession-0.0.2/src/ezsession.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 21:43:43.000000 ezsession-0.0.2/src/ezsession.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-18 21:43:43.000000 ezsession-0.0.2/src/ezsession.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:45:39.253608 ezsession-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-26 14:45:39.253608 ezsession-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-26 14:45:28.000000 ezsession-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 14:45:28.000000 ezsession-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-26 14:45:39.253608 ezsession-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 14:45:28.000000 ezsession-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:45:39.249608 ezsession-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:45:39.249608 ezsession-0.0.4/src/ezsession/
+-rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-26 14:45:28.000000 ezsession-0.0.4/src/ezsession/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:45:39.253608 ezsession-0.0.4/src/ezsession.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-26 14:45:39.000000 ezsession-0.0.4/src/ezsession.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-26 14:45:39.000000 ezsession-0.0.4/src/ezsession.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:45:39.000000 ezsession-0.0.4/src/ezsession.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 14:45:39.000000 ezsession-0.0.4/src/ezsession.egg-info/top_level.txt
```

### Comparing `ezsession-0.0.2/PKG-INFO` & `ezsession-0.0.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.2
+Version: 0.0.4
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
@@ -20,39 +20,33 @@
 3. **oauth_password** - `auth_uri`, `username`, `password`
 4. **basic** - `username`, `password`, `auth_uri` (optional)
 5. **bearer** - `api_key`
 6. **ApiToken** - `api_key`
 7. **dell** - `auth_uri`, `client_id`, `client_secret`
 
 ## Examples
-Example usage for getting a Datto RMM or Huntress session:
+Example usage for getting a Datto RMM session:
 
 ```python
 from ezsession import get_session
-def datto_rmm_auth(api_key, api_secret):
+def datto_rmm_session(api_key, api_secret, server):
+    base_uri = f"https://{server}-api.centrastage.net"
     auth = {
         "type": "oauth_basic",
         "auth_uri": f"{base_uri}/auth/oauth/token",
         "username": api_key,
         "password": api_secret,
-        "server": "concord",
+        "server": server,
     }
-    return get_session(auth)
- 
-def huntress_auth(api_key, api_secret):
-  auth = {
-    "type": "basic",
-    "username": auth_data["api_key"],
-    "password": auth_data["api_secret"],
-  }
-  return get_session(auth)
+    return get_session(auth), base_uri
 ```
 
 Example to initialize a Datto RMM session then get account variables.
 
 ```python
-server = "merlot" # Change to your Datto RMM server.
-base_uri = f"https://{server}-api.centrastage.net"
-session = datto_rmm_auth(drmm_user, drmm_pass)
-response = session.get(f"https://{base_uri}/api/v2/account/variables")
+drmm_user = "Your Datto RMM API Key"
+drmm_pass = "Your Datto RMM API Secret"
+drmm_server = "merlot" # Change to your Datto RMM server.
+session, base_uri = datto_rmm_auth(drmm_user, drmm_pass, drmm_server)
+response = session.get(f"{base_uri}/api/v2/account/variables")
 variables = response.json()["variables"]
 ```
```

### Comparing `ezsession-0.0.2/README.md` & `ezsession-0.0.4/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -12,39 +12,33 @@
 3. **oauth_password** - `auth_uri`, `username`, `password`
 4. **basic** - `username`, `password`, `auth_uri` (optional)
 5. **bearer** - `api_key`
 6. **ApiToken** - `api_key`
 7. **dell** - `auth_uri`, `client_id`, `client_secret`
 
 ## Examples
-Example usage for getting a Datto RMM or Huntress session:
+Example usage for getting a Datto RMM session:
 
 ```python
 from ezsession import get_session
-def datto_rmm_auth(api_key, api_secret):
+def datto_rmm_session(api_key, api_secret, server):
+    base_uri = f"https://{server}-api.centrastage.net"
     auth = {
         "type": "oauth_basic",
         "auth_uri": f"{base_uri}/auth/oauth/token",
         "username": api_key,
         "password": api_secret,
-        "server": "concord",
+        "server": server,
     }
-    return get_session(auth)
- 
-def huntress_auth(api_key, api_secret):
-  auth = {
-    "type": "basic",
-    "username": auth_data["api_key"],
-    "password": auth_data["api_secret"],
-  }
-  return get_session(auth)
+    return get_session(auth), base_uri
 ```
 
 Example to initialize a Datto RMM session then get account variables.
 
 ```python
-server = "merlot" # Change to your Datto RMM server.
-base_uri = f"https://{server}-api.centrastage.net"
-session = datto_rmm_auth(drmm_user, drmm_pass)
-response = session.get(f"https://{base_uri}/api/v2/account/variables")
+drmm_user = "Your Datto RMM API Key"
+drmm_pass = "Your Datto RMM API Secret"
+drmm_server = "merlot" # Change to your Datto RMM server.
+session, base_uri = datto_rmm_auth(drmm_user, drmm_pass, drmm_server)
+response = session.get(f"{base_uri}/api/v2/account/variables")
 variables = response.json()["variables"]
 ```
```

### Comparing `ezsession-0.0.2/setup.py` & `ezsession-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of your README file
 this_directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="ezsession",
-    version="0.0.2",
+    version="0.0.4",
     description="A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Josh XT",
     author_email="josh@devxt.com",
     package_dir={"": "src"},
     packages=find_packages(where="src"),
```

### Comparing `ezsession-0.0.2/src/ezsession/__init__.py` & `ezsession-0.0.4/src/ezsession/__init__.py`

 * *Files identical despite different names*

### Comparing `ezsession-0.0.2/src/ezsession.egg-info/PKG-INFO` & `ezsession-0.0.4/src/ezsession.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezsession
-Version: 0.0.2
+Version: 0.0.4
 Summary: A small useful Python module to abstract away the common auth header methods used by different software vendors. The output is a requests session with the authentication headers built in.
 Author: Josh XT
 Author-email: josh@devxt.com
 Description-Content-Type: text/markdown
 
 # ezsession
 A small useful Python module to abstract away the common auth header methods used by different software vendors.  The output is a requests session with the authentication headers built in.
@@ -20,39 +20,33 @@
 3. **oauth_password** - `auth_uri`, `username`, `password`
 4. **basic** - `username`, `password`, `auth_uri` (optional)
 5. **bearer** - `api_key`
 6. **ApiToken** - `api_key`
 7. **dell** - `auth_uri`, `client_id`, `client_secret`
 
 ## Examples
-Example usage for getting a Datto RMM or Huntress session:
+Example usage for getting a Datto RMM session:
 
 ```python
 from ezsession import get_session
-def datto_rmm_auth(api_key, api_secret):
+def datto_rmm_session(api_key, api_secret, server):
+    base_uri = f"https://{server}-api.centrastage.net"
     auth = {
         "type": "oauth_basic",
         "auth_uri": f"{base_uri}/auth/oauth/token",
         "username": api_key,
         "password": api_secret,
-        "server": "concord",
+        "server": server,
     }
-    return get_session(auth)
- 
-def huntress_auth(api_key, api_secret):
-  auth = {
-    "type": "basic",
-    "username": auth_data["api_key"],
-    "password": auth_data["api_secret"],
-  }
-  return get_session(auth)
+    return get_session(auth), base_uri
 ```
 
 Example to initialize a Datto RMM session then get account variables.
 
 ```python
-server = "merlot" # Change to your Datto RMM server.
-base_uri = f"https://{server}-api.centrastage.net"
-session = datto_rmm_auth(drmm_user, drmm_pass)
-response = session.get(f"https://{base_uri}/api/v2/account/variables")
+drmm_user = "Your Datto RMM API Key"
+drmm_pass = "Your Datto RMM API Secret"
+drmm_server = "merlot" # Change to your Datto RMM server.
+session, base_uri = datto_rmm_auth(drmm_user, drmm_pass, drmm_server)
+response = session.get(f"{base_uri}/api/v2/account/variables")
 variables = response.json()["variables"]
 ```
```

