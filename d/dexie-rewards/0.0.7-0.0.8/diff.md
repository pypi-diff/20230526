# Comparing `tmp/dexie_rewards-0.0.7.tar.gz` & `tmp/dexie_rewards-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexie_rewards-0.0.7.tar", max compression
+gzip compressed data, was "dexie_rewards-0.0.8.tar", max compression
```

## Comparing `dexie_rewards-0.0.7.tar` & `dexie_rewards-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.7/LICENSE
--rw-r--r--   0        0        0    12037 2023-05-16 00:41:25.101677 dexie_rewards-0.0.7/README.md
--rw-r--r--   0        0        0      768 2023-05-16 01:44:16.901401 dexie_rewards-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-0.0.7/src/dexie_rewards/__init__.py
--rw-r--r--   0        0        0     1126 2023-05-13 02:26:45.947358 dexie_rewards-0.0.7/src/dexie_rewards/config.py
--rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-0.0.7/src/dexie_rewards/decorators/with_db_connection.py
--rw-r--r--   0        0        0     1207 2023-05-11 04:12:56.210275 dexie_rewards-0.0.7/src/dexie_rewards/decorators/with_wallet_rpc_client.py
--rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-0.0.7/src/dexie_rewards/main.py
--rw-r--r--   0        0        0     3505 2023-05-13 03:54:19.525074 dexie_rewards-0.0.7/src/dexie_rewards/rewards/claim.py
--rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-0.0.7/src/dexie_rewards/rewards/list.py
--rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-0.0.7/src/dexie_rewards/rewards/main.py
--rw-r--r--   0        0        0     4839 2023-05-16 01:41:53.653083 dexie_rewards-0.0.7/src/dexie_rewards/rewards/utils.py
--rw-r--r--   0        0        0     2293 2023-05-16 00:50:15.508487 dexie_rewards-0.0.7/src/dexie_rewards/services/dexie_api.py
--rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-0.0.7/src/dexie_rewards/services/dexie_db.py
--rw-r--r--   0        0        0     1713 2023-05-11 04:36:56.173403 dexie_rewards-0.0.7/src/dexie_rewards/services/wallet_rpc_client.py
--rw-r--r--   0        0        0      801 2023-05-16 00:41:08.479451 dexie_rewards-0.0.7/src/dexie_rewards/types/offer_reward.py
--rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-0.0.7/src/dexie_rewards/types/utils.py
--rw-r--r--   0        0        0     1851 2023-05-12 13:28:19.018840 dexie_rewards-0.0.7/src/dexie_rewards/utils.py
--rw-r--r--   0        0        0    12792 1970-01-01 00:00:00.000000 dexie_rewards-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-02 08:44:23.355168 dexie_rewards-0.0.8/LICENSE
+-rw-r--r--   0        0        0     5641 2023-05-26 14:42:14.551472 dexie_rewards-0.0.8/README.md
+-rw-r--r--   0        0        0      768 2023-05-26 14:46:27.159293 dexie_rewards-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-04 04:23:21.607369 dexie_rewards-0.0.8/src/dexie_rewards/__init__.py
+-rw-r--r--   0        0        0     1126 2023-05-13 02:26:45.947358 dexie_rewards-0.0.8/src/dexie_rewards/config.py
+-rw-r--r--   0        0        0      822 2023-05-12 12:18:23.796037 dexie_rewards-0.0.8/src/dexie_rewards/decorators/with_db_connection.py
+-rw-r--r--   0        0        0     1207 2023-05-11 04:12:56.210275 dexie_rewards-0.0.8/src/dexie_rewards/decorators/with_wallet_rpc_client.py
+-rw-r--r--   0        0        0      234 2023-05-08 10:51:08.009870 dexie_rewards-0.0.8/src/dexie_rewards/main.py
+-rw-r--r--   0        0        0     3505 2023-05-13 03:54:19.525074 dexie_rewards-0.0.8/src/dexie_rewards/rewards/claim.py
+-rw-r--r--   0        0        0     1921 2023-05-13 03:55:02.188725 dexie_rewards-0.0.8/src/dexie_rewards/rewards/list.py
+-rw-r--r--   0        0        0      272 2023-05-08 10:18:31.545940 dexie_rewards-0.0.8/src/dexie_rewards/rewards/main.py
+-rw-r--r--   0        0        0     4791 2023-05-19 15:21:53.340874 dexie_rewards-0.0.8/src/dexie_rewards/rewards/utils.py
+-rw-r--r--   0        0        0     2294 2023-05-19 15:21:53.341294 dexie_rewards-0.0.8/src/dexie_rewards/services/dexie_api.py
+-rw-r--r--   0        0        0     3756 2023-05-13 03:51:52.828154 dexie_rewards-0.0.8/src/dexie_rewards/services/dexie_db.py
+-rw-r--r--   0        0        0     1759 2023-05-26 14:42:14.553106 dexie_rewards-0.0.8/src/dexie_rewards/services/wallet_rpc_client.py
+-rw-r--r--   0        0        0      801 2023-05-16 00:41:08.479451 dexie_rewards-0.0.8/src/dexie_rewards/types/offer_reward.py
+-rw-r--r--   0        0        0      229 2023-05-09 11:06:14.984159 dexie_rewards-0.0.8/src/dexie_rewards/types/utils.py
+-rw-r--r--   0        0        0     1851 2023-05-12 13:28:19.018840 dexie_rewards-0.0.8/src/dexie_rewards/utils.py
+-rw-r--r--   0        0        0     6396 1970-01-01 00:00:00.000000 dexie_rewards-0.0.8/PKG-INFO
```

### Comparing `dexie_rewards-0.0.7/LICENSE` & `dexie_rewards-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.7/pyproject.toml` & `dexie_rewards-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dexie-rewards"
-version = "0.0.7"
+version = "0.0.8"
 description = "An open source Python tool which runs locally and will automatically claim rewards for all your created offers on dexie."
 authors = ["Dexie Contributors <pypi@dexie.space>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{ include = "dexie_rewards", from = "src" }]
 
 [tool.poetry.dependencies]
```

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/config.py` & `dexie_rewards-0.0.8/src/dexie_rewards/config.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/decorators/with_db_connection.py` & `dexie_rewards-0.0.8/src/dexie_rewards/decorators/with_db_connection.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/decorators/with_wallet_rpc_client.py` & `dexie_rewards-0.0.8/src/dexie_rewards/decorators/with_wallet_rpc_client.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/rewards/claim.py` & `dexie_rewards-0.0.8/src/dexie_rewards/rewards/claim.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/rewards/list.py` & `dexie_rewards-0.0.8/src/dexie_rewards/rewards/list.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/rewards/utils.py` & `dexie_rewards-0.0.8/src/dexie_rewards/rewards/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 from rich import box
 from rich.console import Console
 from rich.table import Table
 from rich.text import Text
 from typing import Any, Dict, List, Tuple
-import datetime
-import json
+import time
 import traceback
 
 from chia.types.blockchain_format.sized_bytes import bytes32
 from chia.wallet.trading.offer import Offer
 
 from ..config import dexie_api_url, dexie_blue, dexie_url
 from ..services import wallet_rpc_client as wallet_rpc_client
 from ..services.dexie_api import Api, get_dexie_bs58_offer_hash
 from ..services import dexie_db as dexie_db
 from ..types.offer_reward import OfferReward
-from ..types.utils import from_datetime
 
 
 async def create_claims(offers_rewards: List[OfferReward]) -> List[Any]:
-    date = from_datetime(datetime.datetime.now())
+    timestamp = int(time.time())
     claims = []
     for offer_reward in offers_rewards:
         (
             public_key,
             signature,
             signing_mode,
         ) = await sign_claim(
             offer_reward.offer_id,
-            date,
+            timestamp,
             offer_reward.maker_puzzle_hash,
         )
 
         # return offer hash, signature, pk, and puzzle hash
         claim_info = {
             "offer_id": offer_reward.offer_id,
             "signature": signature,
             "public_key": public_key,
-            "date": date,
+            "timestamp": timestamp,
         }
         claims.append(claim_info)
     return claims
 
 
 async def get_offers_with_claimable_rewards(
     synced_fingerprint: int, console: Console = Console()
@@ -91,17 +89,17 @@
         traceback_string = traceback.format_exc()
         console.print(traceback_string)
         console.print(e)
         return []
 
 
 async def sign_claim(
-    offer_id: str, date: str, maker_puzzle_hash: bytes32
+    offer_id: str, timestamp: int, maker_puzzle_hash: bytes32
 ) -> Tuple[str, str, str]:
-    message = f"Claim dexie liquidity rewards for offer {offer_id} ({date})"
+    message = f"Claim dexie liquidity rewards for offer {offer_id} ({timestamp})"
     return await wallet_rpc_client.sign_message_by_puzzle_hash(
         maker_puzzle_hash, message
     )
 
 
 async def claim_rewards(claims_payload: Any) -> Dict[str, Any]:
     result = await Api(dexie_api_url).claim_rewards(claims_payload)
```

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/services/dexie_api.py` & `dexie_rewards-0.0.8/src/dexie_rewards/services/dexie_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
 
     async def get_offers_with_claimable_rewards(
         self, offer_ids: list[str]
     ) -> Dict[str, Any]:
         async with (
             aiohttp.ClientSession() as session,
             session.post(
-                f"{self.base_url}/checkRewards", json={"ids": offer_ids}
+                f"{self.base_url}/rewards/check", json={"ids": offer_ids}
             ) as rep,
         ):
             if not rep.ok:
                 raise RuntimeError(rep.reason)
             return await rep.json()
 
     # claim rewards
```

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/services/dexie_db.py` & `dexie_rewards-0.0.8/src/dexie_rewards/services/dexie_db.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/services/wallet_rpc_client.py` & `dexie_rewards-0.0.8/src/dexie_rewards/services/wallet_rpc_client.py`

 * *Files 14% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 async def get_synced(wallet_rpc_client: WalletRpcClient) -> bool:
     return await wallet_rpc_client.get_synced()
 
 
 @with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
 async def get_all_offers(wallet_rpc_client: WalletRpcClient) -> List[TradeRecord]:
     return await wallet_rpc_client.get_all_offers(
-        include_completed=True, file_contents=True
+        include_completed=True, exclude_taken_offers=True, file_contents=True, start=0, end=1000
     )
 
 
 @with_wallet_rpc_client(self_hostname, wallet_rpc_port, chia_root, chia_config)
 async def sign_message_by_puzzle_hash(
     wallet_rpc_client: WalletRpcClient, puzzle_hash: bytes32, message: str
 ) -> Tuple[str, str, str]:
```

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/types/offer_reward.py` & `dexie_rewards-0.0.8/src/dexie_rewards/types/offer_reward.py`

 * *Files identical despite different names*

### Comparing `dexie_rewards-0.0.7/src/dexie_rewards/utils.py` & `dexie_rewards-0.0.8/src/dexie_rewards/utils.py`

 * *Files identical despite different names*

