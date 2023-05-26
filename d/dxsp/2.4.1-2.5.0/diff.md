# Comparing `tmp/dxsp-2.4.1.tar.gz` & `tmp/dxsp-2.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.4.1.tar", max compression
+gzip compressed data, was "dxsp-2.5.0.tar", max compression
```

## Comparing `dxsp-2.4.1.tar` & `dxsp-2.5.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-25 17:36:55.652250 dxsp-2.4.1/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-25 17:36:55.652250 dxsp-2.4.1/README.md
--rw-r--r--   0        0        0       86 2023-05-25 17:36:56.324249 dxsp-2.4.1/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/config.py
--rw-r--r--   0        0        0     3583 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/default_settings.toml
--rw-r--r--   0        0        0    20388 2023-05-25 17:36:55.652250 dxsp-2.4.1/dxsp/main.py
--rw-r--r--   0        0        0     1973 2023-05-25 17:36:56.324249 dxsp-2.4.1/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-26 17:44:13.615122 dxsp-2.5.0/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-26 17:44:13.615122 dxsp-2.5.0/README.md
+-rw-r--r--   0        0        0       86 2023-05-26 17:44:14.287126 dxsp-2.5.0/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/config.py
+-rw-r--r--   0        0        0     3583 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    20431 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/main.py
+-rw-r--r--   0        0        0     1973 2023-05-26 17:44:14.287126 dxsp-2.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.0/PKG-INFO
```

### Comparing `dxsp-2.4.1/LICENSE` & `dxsp-2.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.4.1/README.md` & `dxsp-2.5.0/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.4.1/dxsp/assets/blockchains.py` & `dxsp-2.5.0/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.4.1/dxsp/default_settings.toml` & `dxsp-2.5.0/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.4.1/dxsp/main.py` & `dxsp-2.5.0/dxsp/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,14 +29,15 @@
             self.logger.error(f"connectivity failed {e}")
             return
 
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
+        self.account = self.wallet_address
         self.private_key = settings.dex_private_key
 
         try:
             self.cg = CoinGeckoAPI()
             asset_platforms = self.cg.get_asset_platforms()
             output_dict = next(
                 x for x in asset_platforms if x["chain_identifier"] == int(self.chain_id)
```

### Comparing `dxsp-2.4.1/pyproject.toml` & `dxsp-2.5.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.4.1"
+version = "2.5.0"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.4.1/PKG-INFO` & `dxsp-2.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.4.1
+Version: 2.5.0
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

