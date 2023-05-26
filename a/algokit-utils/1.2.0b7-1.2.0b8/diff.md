# Comparing `tmp/algokit_utils-1.2.0b7-py3-none-any.whl.zip` & `tmp/algokit_utils-1.2.0b8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,18 @@
-Zip file size: 34820 bytes, number of entries: 15
+Zip file size: 36501 bytes, number of entries: 16
 -rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
+-rw-r--r--  2.0 unx     2841 b- defN 80-Jan-01 00:00 algokit_utils/_simulate_315_compat.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
--rw-r--r--  2.0 unx    55309 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
+-rw-r--r--  2.0 unx    56488 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
 -rw-r--r--  2.0 unx    34168 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     5876 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4857 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b7.dist-info/LICENSE
--rw-r--r--  2.0 unx     2065 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b7.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b7.dist-info/RECORD
-15 files, 134152 bytes uncompressed, 32728 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b8.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2072 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b8.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1357 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b8.dist-info/RECORD
+16 files, 138273 bytes uncompressed, 34259 bytes compressed:  75.2%
```

## zipnote {}

```diff
@@ -1,13 +1,16 @@
 Filename: algokit_utils/__init__.py
 Comment: 
 
 Filename: algokit_utils/_ensure_funded.py
 Comment: 
 
+Filename: algokit_utils/_simulate_315_compat.py
+Comment: 
+
 Filename: algokit_utils/_transfer.py
 Comment: 
 
 Filename: algokit_utils/account.py
 Comment: 
 
 Filename: algokit_utils/application_client.py
@@ -27,20 +30,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.2.0b7.dist-info/LICENSE
+Filename: algokit_utils-1.2.0b8.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.2.0b7.dist-info/METADATA
+Filename: algokit_utils-1.2.0b8.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.2.0b7.dist-info/WHEEL
+Filename: algokit_utils-1.2.0b8.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.2.0b7.dist-info/RECORD
+Filename: algokit_utils-1.2.0b8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/application_client.py

```diff
@@ -1,13 +1,14 @@
 import base64
 import copy
 import json
 import logging
 import re
 import typing
+from http import HTTPStatus
 from math import ceil
 from pathlib import Path
 from typing import Any, Literal, cast, overload
 
 import algosdk
 from algosdk import transaction
 from algosdk.abi import ABIType, Method, Returns
@@ -16,23 +17,26 @@
     ABI_RETURN_HASH,
     ABIResult,
     AccountTransactionSigner,
     AtomicTransactionComposer,
     AtomicTransactionResponse,
     LogicSigTransactionSigner,
     MultisigTransactionSigner,
+    SimulateAtomicTransactionResponse,
     TransactionSigner,
     TransactionWithSigner,
 )
 from algosdk.constants import APP_PAGE_MAX_SIZE
+from algosdk.error import AlgodHTTPError
 from algosdk.logic import get_application_address
 from algosdk.source_map import SourceMap
 
 import algokit_utils.application_specification as au_spec
 import algokit_utils.deploy as au_deploy
+from algokit_utils._simulate_315_compat import simulate_atc_315
 from algokit_utils.logic_error import LogicError, parse_logic_error
 from algokit_utils.models import (
     ABIArgsDict,
     ABIArgType,
     ABIMethod,
     ABITransactionResponse,
     Account,
@@ -161,14 +165,15 @@
         self.app_spec = (
             au_spec.ApplicationSpecification.from_json(app_spec.read_text()) if isinstance(app_spec, Path) else app_spec
         )
         self._app_name = app_name
         self._approval_program: Program | None = None
         self._approval_source_map: SourceMap | None = None
         self._clear_program: Program | None = None
+        self._use_simulate_315 = False  # flag to determine if old simulate 3.15 encoding should be used
 
         self.template_values: au_deploy.TemplateValueMapping = template_values or {}
         self.existing_deployments = existing_deployments
         self._indexer_client = indexer_client
         if creator is not None:
             if not self.existing_deployments and not self._indexer_client:
                 raise Exception(
@@ -861,26 +866,44 @@
                 self.algod_client, self.app_spec, self.template_values
             )
         return self._approval_program, self._clear_program
 
     def _simulate_readonly_call(
         self, method: Method, atc: AtomicTransactionComposer
     ) -> ABITransactionResponse | TransactionResponse:
-        simulate_response = atc.simulate(self.algod_client)
+        simulate_response = self._simulate_atc(atc)
         if simulate_response.failure_message:
             raise _try_convert_to_logic_error(
                 simulate_response.failure_message,
                 self.app_spec.approval_program,
                 self._get_approval_source_map,
             ) or Exception(
                 f"Simulate failed for readonly method {method.get_signature()}: {simulate_response.failure_message}"
             )
 
         return TransactionResponse.from_atr(simulate_response)
 
+    def _simulate_atc(self, atc: AtomicTransactionComposer) -> SimulateAtomicTransactionResponse:
+        # TODO: remove this once 3.16 is in mainnet
+        # there was a breaking change in algod 3.16 to the simulate endpoint
+        # attempt to transparently handle this by calling the endpoint with the old behaviour if
+        # 3.15 is detected
+        if self._use_simulate_315:
+            return simulate_atc_315(atc, self.algod_client)
+        try:
+            return atc.simulate(self.algod_client)
+        except AlgodHTTPError as ex:
+            if ex.code == HTTPStatus.BAD_REQUEST.value and (
+                "msgpack decode error [pos 12]: no matching struct field found when decoding stream map with key "
+                "txn-groups" in ex.args
+            ):
+                self._use_simulate_315 = True
+                return simulate_atc_315(atc, self.algod_client)
+            raise ex
+
     def _load_reference_and_check_app_id(self) -> None:
         self._load_app_reference()
         self._check_app_id()
 
     def _load_app_reference(self) -> au_deploy.AppReference | au_deploy.AppMetaData:
         if not self.existing_deployments and self._creator:
             assert self._indexer_client
```

## Comparing `algokit_utils-1.2.0b7.dist-info/LICENSE` & `algokit_utils-1.2.0b8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.2.0b7.dist-info/METADATA` & `algokit_utils-1.2.0b8.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.2.0b7
+Version: 1.2.0b8
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: py-algorand-sdk (==2.1.2)
+Requires-Dist: py-algorand-sdk (>=2.2.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # AlgoKit Python Utilities
 
 A set of core Algorand utilities written in Python and released via PyPi that make it easier to build solutions on Algorand. 
 This project is part of [AlgoKit](https://github.com/algorandfoundation/algokit-cli).
```

## Comparing `algokit_utils-1.2.0b7.dist-info/RECORD` & `algokit_utils-1.2.0b8.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 algokit_utils/__init__.py,sha256=wuh-p9PubCj9Bj2tpxP3tQ5qZPs_nUHzB16BHi9Aq2c,4091
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
+algokit_utils/_simulate_315_compat.py,sha256=9qCsNnKa1FXYfCccMFiE0mGEcZJiBuPmUy7ZRvvUSqU,2841
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
-algokit_utils/application_client.py,sha256=G0ENU11FUL3Ty69hpnJ_FtBkpVA_S_yxYMmhZeAEakg,55309
+algokit_utils/application_client.py,sha256=k3eTyhY3zyfpajHffo1uJ2u1C0vlYPmdALl5jmgH1WM,56488
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
 algokit_utils/deploy.py,sha256=UmVlJ-0vo91EjPXRC1EjkFBh5frJ0R4nCnlyZABhcRg,34168
 algokit_utils/logic_error.py,sha256=8O_4rJ1t57JEG81ucRNih2ojc1-EOm2fVxW6m-1ZXI8,2550
 algokit_utils/models.py,sha256=1IXNhibqtZ7cmuH31mLvNLcpJzaMl9lOD0EqsTPyglU,5876
 algokit_utils/network_clients.py,sha256=dq8yyTLKtyb9yG3tsXV-eZLF3iqMaFWs9kNWm1V4CdU,4857
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.2.0b7.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.2.0b7.dist-info/METADATA,sha256=-wmDJEwAeak-hop4ezZZfpbnN9CPYsfiYPp76gRjJtE,2065
-algokit_utils-1.2.0b7.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-algokit_utils-1.2.0b7.dist-info/RECORD,,
+algokit_utils-1.2.0b8.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.2.0b8.dist-info/METADATA,sha256=VjqC24FemTAouDXAwiChHgbjLRMXO89jHtN0uJLSHls,2072
+algokit_utils-1.2.0b8.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+algokit_utils-1.2.0b8.dist-info/RECORD,,
```

