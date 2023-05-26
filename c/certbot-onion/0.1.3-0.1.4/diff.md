# Comparing `tmp/certbot-onion-0.1.3.tar.gz` & `tmp/certbot-onion-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "certbot-onion-0.1.3.tar", last modified: Wed Apr 26 18:55:55 2023, max compression
+gzip compressed data, was "certbot-onion-0.1.4.tar", last modified: Fri May 26 09:07:44 2023, max compression
```

## Comparing `certbot-onion-0.1.3.tar` & `certbot-onion-0.1.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/rust/
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/rust/Cargo.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/rust/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/rust/src/lib.rs
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.444924 certbot-onion-0.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/src/certbot_onion/
--rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-04-26 18:55:43.000000 certbot-onion-0.1.3/src/certbot_onion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 18:55:55.448924 certbot-onion-0.1.3/src/certbot_onion.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-26 18:55:55.000000 certbot-onion-0.1.3/src/certbot_onion.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.564749 certbot-onion-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 09:07:44.564749 certbot-onion-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.560749 certbot-onion-0.1.4/rust/
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/rust/Cargo.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.560749 certbot-onion-0.1.4/rust/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     2710 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/rust/src/lib.rs
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:07:44.564749 certbot-onion-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.560749 certbot-onion-0.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.560749 certbot-onion-0.1.4/src/certbot_onion/
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-26 09:07:35.000000 certbot-onion-0.1.4/src/certbot_onion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:07:44.564749 certbot-onion-0.1.4/src/certbot_onion.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 09:07:44.000000 certbot-onion-0.1.4/src/certbot_onion.egg-info/top_level.txt
```

### Comparing `certbot-onion-0.1.3/LICENSE.md` & `certbot-onion-0.1.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.3/PKG-INFO` & `certbot-onion-0.1.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.3
+Version: 0.1.4
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -28,19 +28,7 @@
 certbot --server https://acme.api.acmeforonions.org/directory certonly -d 5anebu2glyc235wbbop3m2ukzlaptpkq333vdtdvcjpigyb7x2i2m2qd.onion --authenticator onion-csr --onion-csr-hs-dir /var/lib/tor/example_hs/
 ```
 
 The important arguments here are:
 
 * `--authenticator onion-csr` - Tells certbot to use this plugin for domain authentication
 * `--onion-csr-hs-dir /var/lib/tor/example_hs/` - Provides the path to the hidden service directory, this can be specified multiple times for multiple domains.
-
-## ⚠️ WARNING ⚠️
-
-This plugin is currently non-functional, it will not work until Certbot version 
-2.6.0 is released.
-
-In the meantime you update Certbot to the commit incorporating the changes required for this plugin to work:
-
-```shell 
-pip install git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=certbot \
-  git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=acme
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `certbot-onion-0.1.3/pyproject.toml` & `certbot-onion-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [project]
 name = "certbot-onion"
-version = "0.1.3"
+version = "0.1.4"
 description = "Certbot authenticator plugin for the onion-csr-01 challenge"
 authors = [
     {name = "Q Misell", email = "q@as207960.net"}
 ]
 license = {text = "MIT"}
 dependencies = [
-    "certbot==2.6.0dev0"
+    "certbot>=2.6.0"
 ]
 readme = "README.md"
 
 [project.urls]
 "Homepage" = "https://acmeforonions.org"
 "Bug Tracker" = "https://github.com/AS207960/certbot-onion"
 
@@ -28,10 +28,8 @@
 package-dir = {"" = "src"}
 
 [project.entry-points."certbot.plugins"]
 onion-csr = "certbot_onion:Authenticator"
 
 [tool.cibuildwheel]
 before-all = """curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh -s -- -y;
-pip install cryptography;
-pip install git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=certbot \
-git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=acme"""
+pip install cryptography"""
```

### Comparing `certbot-onion-0.1.3/rust/src/lib.rs` & `certbot-onion-0.1.4/rust/src/lib.rs`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.3/src/certbot_onion/__init__.py` & `certbot-onion-0.1.4/src/certbot_onion/__init__.py`

 * *Files identical despite different names*

### Comparing `certbot-onion-0.1.3/src/certbot_onion.egg-info/PKG-INFO` & `certbot-onion-0.1.4/src/certbot_onion.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: certbot-onion
-Version: 0.1.3
+Version: 0.1.4
 Summary: Certbot authenticator plugin for the onion-csr-01 challenge
 Author-email: Q Misell <q@as207960.net>
 License: MIT
 Project-URL: Homepage, https://acmeforonions.org
 Project-URL: Bug Tracker, https://github.com/AS207960/certbot-onion
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
@@ -28,19 +28,7 @@
 certbot --server https://acme.api.acmeforonions.org/directory certonly -d 5anebu2glyc235wbbop3m2ukzlaptpkq333vdtdvcjpigyb7x2i2m2qd.onion --authenticator onion-csr --onion-csr-hs-dir /var/lib/tor/example_hs/
 ```
 
 The important arguments here are:
 
 * `--authenticator onion-csr` - Tells certbot to use this plugin for domain authentication
 * `--onion-csr-hs-dir /var/lib/tor/example_hs/` - Provides the path to the hidden service directory, this can be specified multiple times for multiple domains.
-
-## ⚠️ WARNING ⚠️
-
-This plugin is currently non-functional, it will not work until Certbot version 
-2.6.0 is released.
-
-In the meantime you update Certbot to the commit incorporating the changes required for this plugin to work:
-
-```shell 
-pip install git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=certbot \
-  git+https://github.com/certbot/certbot.git@8a0b0f6#subdirectory=acme
-```
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

