# Comparing `tmp/autonity-0.2.dev3-py3-none-any.whl.zip` & `tmp/autonity-1.0.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 28062 bytes, number of entries: 31
+Zip file size: 28044 bytes, number of entries: 31
 -rw-r--r--  2.0 unx      530 b- defN 20-Feb-02 00:00 autonity/__init__.py
--rw-r--r--  2.0 unx       72 b- defN 20-Feb-02 00:00 autonity/__version__.py
+-rw-r--r--  2.0 unx       69 b- defN 20-Feb-02 00:00 autonity/__version__.py
 -rw-r--r--  2.0 unx      929 b- defN 20-Feb-02 00:00 autonity/abi_manager.py
--rw-r--r--  2.0 unx     5675 b- defN 20-Feb-02 00:00 autonity/abi_parser.py
+-rw-r--r--  2.0 unx     5768 b- defN 20-Feb-02 00:00 autonity/abi_parser.py
 -rw-r--r--  2.0 unx    13618 b- defN 20-Feb-02 00:00 autonity/autonity.py
 -rw-r--r--  2.0 unx      699 b- defN 20-Feb-02 00:00 autonity/committee_member.py
 -rw-r--r--  2.0 unx     1582 b- defN 20-Feb-02 00:00 autonity/config.py
 -rw-r--r--  2.0 unx     5620 b- defN 20-Feb-02 00:00 autonity/erc20.py
 -rw-r--r--  2.0 unx     1500 b- defN 20-Feb-02 00:00 autonity/liquid_newton.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 autonity/py.typed
 -rw-r--r--  2.0 unx     3432 b- defN 20-Feb-02 00:00 autonity/tendermint.py
@@ -22,12 +22,12 @@
 -rw-r--r--  2.0 unx       40 b- defN 20-Feb-02 00:00 autonity/abi/autonity-commit.txt
 -rw-r--r--  2.0 unx       92 b- defN 20-Feb-02 00:00 autonity/abi/solc-version.txt
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 autonity/utils/__init__.py
 -rw-r--r--  2.0 unx     1173 b- defN 20-Feb-02 00:00 autonity/utils/denominations.py
 -rw-r--r--  2.0 unx     1814 b- defN 20-Feb-02 00:00 autonity/utils/keyfile.py
 -rw-r--r--  2.0 unx     5728 b- defN 20-Feb-02 00:00 autonity/utils/tx.py
 -rw-r--r--  2.0 unx     3061 b- defN 20-Feb-02 00:00 autonity/utils/web3.py
-?rw-r--r--  2.0 unx     6931 b- defN 20-Feb-02 00:00 autonity-0.2.dev3.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 autonity-0.2.dev3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1065 b- defN 20-Feb-02 00:00 autonity-0.2.dev3.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     2473 b- defN 20-Feb-02 00:00 autonity-0.2.dev3.dist-info/RECORD
-31 files, 97370 bytes uncompressed, 24108 bytes compressed:  75.2%
+?rw-r--r--  2.0 unx     6928 b- defN 20-Feb-02 00:00 autonity-1.0.0.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 autonity-1.0.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1065 b- defN 20-Feb-02 00:00 autonity-1.0.0.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     2461 b- defN 20-Feb-02 00:00 autonity-1.0.0.dist-info/RECORD
+31 files, 97445 bytes uncompressed, 24114 bytes compressed:  75.3%
```

## zipnote {}

```diff
@@ -75,20 +75,20 @@
 
 Filename: autonity/utils/tx.py
 Comment: 
 
 Filename: autonity/utils/web3.py
 Comment: 
 
-Filename: autonity-0.2.dev3.dist-info/METADATA
+Filename: autonity-1.0.0.dist-info/METADATA
 Comment: 
 
-Filename: autonity-0.2.dev3.dist-info/WHEEL
+Filename: autonity-1.0.0.dist-info/WHEEL
 Comment: 
 
-Filename: autonity-0.2.dev3.dist-info/licenses/LICENSE
+Filename: autonity-1.0.0.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: autonity-0.2.dev3.dist-info/RECORD
+Filename: autonity-1.0.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## autonity/__version__.py

```diff
@@ -1,5 +1,5 @@
 """
 Release version of autonity package.
 """
 
-__version__ = "v0.2.dev3"
+__version__ = "v1.0.0"
```

## autonity/abi_parser.py

```diff
@@ -1,22 +1,22 @@
 # Copyright (C) 2015-2022 Clearmatics Technologies Ltd - All Rights Reserved.
 
 """
 Functions for working with contract ABIs.
 """
 
-
 from __future__ import annotations
 from web3 import Web3
 from web3.types import (
     ABI,
     ABIFunction,
     ABIFunctionParams,
 )
 from typing import Dict, List, Tuple, Sequence, Any, Union, Callable, cast
+import json
 
 
 def find_abi_constructor(abi: ABI) -> ABIFunction:
     """
     Given an ABI and function name, find the ABIFunction element.
     """
 
@@ -98,36 +98,38 @@
     """
     if bool_str in ["False", "false", "0", ""]:
         return False
 
     return True
 
 
+def _parse_complex(value: str) -> Any:
+    """
+    Parse a complex type, such as an array or tuple.
+    """
+    return json.loads(value)
+
+
 def _string_to_argument_fn_for_type(arg_type: str) -> ParamParser:
     """
     Return a function which parses a string into a type suitable for
     function arguments.
     """
-
-    # TODO: support complex types
-
-    if "[" in arg_type:
-        raise ValueError(f"cannot convert array type '{arg_type}' from string")
-
+    if arg_type.endswith("[]") or arg_type == "tuple":
+        return _parse_complex
     if arg_type.startswith("uint") or arg_type.startswith("int"):
         return int
     if arg_type == "bool":
         return _parse_bool
     if arg_type == "address":
         return Web3.to_checksum_address
     if arg_type.startswith("bytes") or arg_type == "string":
         return _parse_string
     if arg_type.startswith("fixed") or arg_type.startswith("ufixed"):
         return float
-
     raise ValueError(f"cannot convert '{arg_type}' from string")
 
 
 def _argument_parsers_for_params(
     outputs: Sequence[ABIFunctionParams],
 ) -> List[ParamParser]:
     """
```

## Comparing `autonity-0.2.dev3.dist-info/METADATA` & `autonity-1.0.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autonity
-Version: 0.2.dev3
+Version: 1.0.0
 Summary: Python library for interacting with Autonity
 License-Expression: MIT
 License-File: LICENSE
 Keywords: autonity,client,library,rpc,web3
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

## Comparing `autonity-0.2.dev3.dist-info/licenses/LICENSE` & `autonity-1.0.0.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `autonity-0.2.dev3.dist-info/RECORD` & `autonity-1.0.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 autonity/__init__.py,sha256=_arYrxLVsIaga7y3TzRM-I44xWF1xo7ZJyTBwaQuYJY,530
-autonity/__version__.py,sha256=vI4Go9Rgp0M_I6uZdzjT6_KDw2-g2jdTWO6F-w42In0,72
+autonity/__version__.py,sha256=umKXolbityZNFFkEP5Eg2YNp8RSsUWB4mT7cmT_pYxU,69
 autonity/abi_manager.py,sha256=ogPaRBb0MaAJ-arsGZZk9C4Zih1EkcGdAAPZOz5ShDI,929
-autonity/abi_parser.py,sha256=FlwdnYI4fAF2hLmzQYXARyNlsyMMtWpAPyBIiaoOFd0,5675
+autonity/abi_parser.py,sha256=0katCkS2t8DOfoOZzPBgwmMfzqtUtsdPXzH_umqnZJM,5768
 autonity/autonity.py,sha256=scq8IrsF7ZGfYUlwcMg7YgnXBY_kkJlrWbqE7HFj64Y,13618
 autonity/committee_member.py,sha256=IyIMqp9yxXOniZlkLsAZnp-y23WobaurFdns_4Xzpx0,699
 autonity/config.py,sha256=HSWUEZHXkk6-rrftFA6HdZ-IfzNevUAk2Pz6L3CJ2JU,1582
 autonity/erc20.py,sha256=DGbmozuM2QDwlcv9V-whHhiq4dH82ErQ8KA8PUBj5wQ,5620
 autonity/liquid_newton.py,sha256=JLI2MamvntQpj6eoVOzk1WlJsovR5iuI72favMUPIfU,1500
 autonity/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autonity/tendermint.py,sha256=asiR6bsb5cK4XwSkLRrv-ybplxHjBYLOLjMG3Q403dc,3432
@@ -21,11 +21,11 @@
 autonity/abi/autonity-commit.txt,sha256=xWQPY94otC7QPdRYNOHTNJy7-gOpeOuw9GU5RnIholY,40
 autonity/abi/solc-version.txt,sha256=BEwPRa_nyw3CFP5VlCGIazmZefItYDUBddR2lwpeJoM,92
 autonity/utils/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 autonity/utils/denominations.py,sha256=gsJme6ZNlCKA073NfBWJ6u0Ka5KZR2M2bxbyoR0wrWk,1173
 autonity/utils/keyfile.py,sha256=HCT8hTlJdF9-j6h5YmYupJjGYiVrpPx4aVNtYaCKzsM,1814
 autonity/utils/tx.py,sha256=fkrYp-GvYZ2AB-bIoqsFBujh30lmMQWUwI1RRyU3s1s,5728
 autonity/utils/web3.py,sha256=U0diDJvK1zX3JrBWCYRJkxwRCDIwLk-O5J50Gydyrhw,3061
-autonity-0.2.dev3.dist-info/METADATA,sha256=Lgar33WRmDMBGn4wruxxmdbxSWmN96PnXVI6UPGn0Tc,6931
-autonity-0.2.dev3.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
-autonity-0.2.dev3.dist-info/licenses/LICENSE,sha256=g9cJ2Md1MlI9a2915dqvKbwFwLAjTCb8gbu00TkEzVc,1065
-autonity-0.2.dev3.dist-info/RECORD,,
+autonity-1.0.0.dist-info/METADATA,sha256=QOe01fMjOxg8vCZ3Leh4q1P4Igmn1mieSscx7yeHkYQ,6928
+autonity-1.0.0.dist-info/WHEEL,sha256=9MIigYJ7D5sOqAPqr0-o6tSMY_nQ7c6kvtvyeUB99YQ,87
+autonity-1.0.0.dist-info/licenses/LICENSE,sha256=g9cJ2Md1MlI9a2915dqvKbwFwLAjTCb8gbu00TkEzVc,1065
+autonity-1.0.0.dist-info/RECORD,,
```

