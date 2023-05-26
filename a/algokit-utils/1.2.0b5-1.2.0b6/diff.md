# Comparing `tmp/algokit_utils-1.2.0b5-py3-none-any.whl.zip` & `tmp/algokit_utils-1.2.0b6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 34605 bytes, number of entries: 15
+Zip file size: 34815 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    54567 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx    55309 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    34168 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
--rw-r--r--  2.0 unx     2475 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
+-rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     5876 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b5.dist-info/LICENSE
--rw-r--r--  2.0 unx     2038 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b5.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b5.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b5.dist-info/RECORD
-15 files, 133292 bytes uncompressed, 32513 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b6.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2065 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b6.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b6.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b6.dist-info/RECORD
+15 files, 134136 bytes uncompressed, 32723 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.2.0b5.dist-info/LICENSE
+Filename: algokit_utils-1.2.0b6.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.2.0b5.dist-info/METADATA
+Filename: algokit_utils-1.2.0b6.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.2.0b5.dist-info/WHEEL
+Filename: algokit_utils-1.2.0b6.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.2.0b5.dist-info/RECORD
+Filename: algokit_utils-1.2.0b6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/application_client.py

```diff
@@ -1,9 +1,10 @@
 import base64
 import copy
+import json
 import logging
 import re
 import typing
 from math import ceil
 from pathlib import Path
 from typing import Any, Literal, cast, overload
 
@@ -946,14 +947,32 @@
 
         try:
             approval, _ = self._check_is_compiled()
         except au_deploy.DeploymentFailedError:
             return None
         return approval.source_map
 
+    def export_source_map(self) -> str | None:
+        """Export approval source map to JSON, can be later re-imported with `import_source_map`"""
+        source_map = self._get_approval_source_map()
+        if source_map:
+            return json.dumps(
+                {
+                    "version": source_map.version,
+                    "sources": source_map.sources,
+                    "mappings": source_map.mappings,
+                }
+            )
+        return None
+
+    def import_source_map(self, source_map_json: str) -> None:
+        """Import approval source from JSON exported by `export_source_map`"""
+        source_map = json.loads(source_map_json)
+        self._approval_source_map = SourceMap(source_map)
+
     def add_method_call(
         self,
         atc: AtomicTransactionComposer,
         abi_method: ABIMethod | bool | None = None,
         *,
         abi_args: ABIArgsDict | None = None,
         app_id: int | None = None,
```

## algokit_utils/logic_error.py

```diff
@@ -68,14 +68,15 @@
 
     def trace(self, lines: int = 5) -> str:
         if self.line_no is None:
             return """
 Could not determine TEAL source line for the error as no approval source map was provided, to receive a trace of the
 error please provide an approval SourceMap. Either by:
     1.) Providing template_values when creating the ApplicationClient, so a SourceMap can be obtained automatically OR
-    2.) Set approval_source_map from a previously compiled approval program"""
+    2.) Set approval_source_map from a previously compiled approval program OR
+    3.) Import a previously exported source map using import_source_map"""
 
         program_lines = copy(self.lines)
         program_lines[self.line_no] += "\t\t<-- Error"
         lines_before = max(0, self.line_no - lines)
         lines_after = min(len(program_lines), self.line_no + lines)
         return "\n\t" + "\n\t".join(program_lines[lines_before:lines_after])
```

## Comparing `algokit_utils-1.2.0b5.dist-info/LICENSE` & `algokit_utils-1.2.0b6.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.2.0b5.dist-info/METADATA` & `algokit_utils-1.2.0b6.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.2.0b5
+Version: 1.2.0b6
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -32,19 +32,20 @@
 
 ```
 pip install algokit-utils
 ```
 
 ## Guiding principles
 
-This library follows the [Guiding Principles of AlgoKit](https://github.com/algorandfoundation/algokit-cli#guiding-principles).
+This library follows the [Guiding Principles of AlgoKit](https://github.com/algorandfoundation/algokit-cli/blob/main/docs/algokit.md#guiding-principles).
 
 ## Contributing
 
 This is an open source project managed by the Algorand Foundation. 
 See the [AlgoKit contributing page](https://github.com/algorandfoundation/algokit-cli/blob/main/CONTRIBUTING.MD) to learn about making improvements.
 
 To successfully run the tests in this repository you need to be running LocalNet via [AlgoKit](https://github.com/algorandfoundation/algokit-cli):
 
 ```
 algokit localnet start
 ```
+
```

## Comparing `algokit_utils-1.2.0b5.dist-info/RECORD` & `algokit_utils-1.2.0b6.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 algokit_utils/__init__.py,sha256=wuh-p9PubCj9Bj2tpxP3tQ5qZPs_nUHzB16BHi9Aq2c,4091
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
-algokit_utils/application_client.py,sha256=EH3UoVoo56Vmg6_ji96IvYIJSzFAe96OfeGsDzI1T1w,54567
+algokit_utils/application_client.py,sha256=G0ENU11FUL3Ty69hpnJ_FtBkpVA_S_yxYMmhZeAEakg,55309
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=UmVlJ-0vo91EjPXRC1EjkFBh5frJ0R4nCnlyZABhcRg,34168
-algokit_utils/logic_error.py,sha256=-04aGw8OG4wY3T42mKU6TezNlkxjtMr6CtHVDWLpS5s,2475
+algokit_utils/logic_error.py,sha256=8O_4rJ1t57JEG81ucRNih2ojc1-EOm2fVxW6m-1ZXI8,2550
 algokit_utils/models.py,sha256=1IXNhibqtZ7cmuH31mLvNLcpJzaMl9lOD0EqsTPyglU,5876
 algokit_utils/network_clients.py,sha256=0cbUHCEWycFnduEu5cJ4dY6pfDOOzvHO1cXmcxAe83M,4841
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.2.0b5.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.2.0b5.dist-info/METADATA,sha256=hOL2d9pwN66F9-5THnKOveGrHd2GRhznRUaU3M7UwTw,2038
-algokit_utils-1.2.0b5.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-algokit_utils-1.2.0b5.dist-info/RECORD,,
+algokit_utils-1.2.0b6.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.2.0b6.dist-info/METADATA,sha256=w48b-TK6KE3tutjPOux4EUz46ZNp4ay3YL5OAufsosw,2065
+algokit_utils-1.2.0b6.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+algokit_utils-1.2.0b6.dist-info/RECORD,,
```

