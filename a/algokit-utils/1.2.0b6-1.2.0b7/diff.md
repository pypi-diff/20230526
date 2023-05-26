# Comparing `tmp/algokit_utils-1.2.0b6-py3-none-any.whl.zip` & `tmp/algokit_utils-1.2.0b7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 34815 bytes, number of entries: 15
+Zip file size: 34820 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    55309 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    34168 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     5876 b- defN 80-Jan-01 00:00 algokit_utils/models.py
--rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
+-rw-r--r--  2.0 unx     4857 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b6.dist-info/LICENSE
--rw-r--r--  2.0 unx     2065 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b6.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b6.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b6.dist-info/RECORD
-15 files, 134136 bytes uncompressed, 32723 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2065 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b7.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b7.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b7.dist-info/RECORD
+15 files, 134152 bytes uncompressed, 32728 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.2.0b6.dist-info/LICENSE
+Filename: algokit_utils-1.2.0b7.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.2.0b6.dist-info/METADATA
+Filename: algokit_utils-1.2.0b7.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.2.0b6.dist-info/WHEEL
+Filename: algokit_utils-1.2.0b7.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.2.0b6.dist-info/RECORD
+Filename: algokit_utils-1.2.0b7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/network_clients.py

```diff
@@ -75,15 +75,15 @@
     headers = _get_headers(config, "X-Indexer-API-Token")
     return IndexerClient(config.token, config.server, headers)  # type: ignore[no-untyped-call]
 
 
 def is_localnet(client: AlgodClient) -> bool:
     """Returns True if client genesis is `devnet-v1` or `sandnet-v1`"""
     params = client.suggested_params()
-    return params.gen in ["devnet-v1", "sandnet-v1"]
+    return params.gen in ["devnet-v1", "sandnet-v1", "dockernet-v1"]
 
 
 def get_kmd_client_from_algod_client(client: AlgodClient) -> KMDClient:
     """Returns an {py:class}`algosdk.kmd.KMDClient` from supplied `client`
 
     Will use the same address as provided `client` but on port specified by `KMD_PORT` environment variable,
     or 4002 by default"""
```

## Comparing `algokit_utils-1.2.0b6.dist-info/LICENSE` & `algokit_utils-1.2.0b7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.2.0b6.dist-info/METADATA` & `algokit_utils-1.2.0b7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.2.0b6
+Version: 1.2.0b7
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

## Comparing `algokit_utils-1.2.0b6.dist-info/RECORD` & `algokit_utils-1.2.0b7.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=G0ENU11FUL3Ty69hpnJ_FtBkpVA_S_yxYMmhZeAEakg,55309
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=UmVlJ-0vo91EjPXRC1EjkFBh5frJ0R4nCnlyZABhcRg,34168
 algokit_utils/logic_error.py,sha256=8O_4rJ1t57JEG81ucRNih2ojc1-EOm2fVxW6m-1ZXI8,2550
 algokit_utils/models.py,sha256=1IXNhibqtZ7cmuH31mLvNLcpJzaMl9lOD0EqsTPyglU,5876
-algokit_utils/network_clients.py,sha256=0cbUHCEWycFnduEu5cJ4dY6pfDOOzvHO1cXmcxAe83M,4841
+algokit_utils/network_clients.py,sha256=dq8yyTLKtyb9yG3tsXV-eZLF3iqMaFWs9kNWm1V4CdU,4857
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.2.0b6.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.2.0b6.dist-info/METADATA,sha256=w48b-TK6KE3tutjPOux4EUz46ZNp4ay3YL5OAufsosw,2065
-algokit_utils-1.2.0b6.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-algokit_utils-1.2.0b6.dist-info/RECORD,,
+algokit_utils-1.2.0b7.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.2.0b7.dist-info/METADATA,sha256=-wmDJEwAeak-hop4ezZZfpbnN9CPYsfiYPp76gRjJtE,2065
+algokit_utils-1.2.0b7.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+algokit_utils-1.2.0b7.dist-info/RECORD,,
```

