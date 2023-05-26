# Comparing `tmp/dxsp-2.5.0.tar.gz` & `tmp/dxsp-2.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.5.0.tar", max compression
+gzip compressed data, was "dxsp-2.5.1.tar", max compression
```

## Comparing `dxsp-2.5.0.tar` & `dxsp-2.5.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1064 2023-05-26 17:44:13.615122 dxsp-2.5.0/LICENSE
--rw-r--r--   0        0        0     2439 2023-05-26 17:44:13.615122 dxsp-2.5.0/README.md
--rw-r--r--   0        0        0       86 2023-05-26 17:44:14.287126 dxsp-2.5.0/dxsp/__init__.py
--rw-r--r--   0        0        0        1 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/assets/__init__.py
--rw-r--r--   0        0        0     8887 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/assets/blockchains.py
--rw-r--r--   0        0        0      388 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/config.py
--rw-r--r--   0        0        0     3583 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/default_settings.toml
--rw-r--r--   0        0        0    20431 2023-05-26 17:44:13.615122 dxsp-2.5.0/dxsp/main.py
--rw-r--r--   0        0        0     1973 2023-05-26 17:44:14.287126 dxsp-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-05-26 20:52:25.218305 dxsp-2.5.1/LICENSE
+-rw-r--r--   0        0        0     2439 2023-05-26 20:52:25.218305 dxsp-2.5.1/README.md
+-rw-r--r--   0        0        0       86 2023-05-26 20:52:25.966339 dxsp-2.5.1/dxsp/__init__.py
+-rw-r--r--   0        0        0        1 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/assets/__init__.py
+-rw-r--r--   0        0        0     8887 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/assets/blockchains.py
+-rw-r--r--   0        0        0      388 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/config.py
+-rw-r--r--   0        0        0     3500 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    20467 2023-05-26 20:52:25.218305 dxsp-2.5.1/dxsp/main.py
+-rw-r--r--   0        0        0     1973 2023-05-26 20:52:25.966339 dxsp-2.5.1/pyproject.toml
+-rw-r--r--   0        0        0     3229 1970-01-01 00:00:00.000000 dxsp-2.5.1/PKG-INFO
```

### Comparing `dxsp-2.5.0/LICENSE` & `dxsp-2.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.0/README.md` & `dxsp-2.5.1/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.0/dxsp/assets/blockchains.py` & `dxsp-2.5.1/dxsp/assets/blockchains.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.5.0/dxsp/default_settings.toml` & `dxsp-2.5.1/dxsp/default_settings.toml`

 * *Files 3% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 token_testnet_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/testnet.json"
 token_personal_list = "https://raw.githubusercontent.com/mraniki/tokenlist/main/TT.json"
 #📝trading setup
 trading_quote_ccy = "USDT"
 trading_risk_amount = 10 # 10% of the position
 dex_trading_slippage = 2 # 2 % slippage
 #user settings
-dex_wallet_address = "0xEeeeeEeeeEeEeeEeEeEeeEEEeeeeEeeeeeeeEEeE" #this is an example
-dex_private_key = "0x111111111117dc0aaaaaa0fa6a738034aaaa302" #this is an example
+dex_wallet_address = "" #this is an example
+dex_private_key = "" #this is an example
 #chain_1 #see below for other chain ids or use https://chainlist.org to overwrite settings
 dex_chain_id = 1
 dex_protocol_type = "uniswap_v2" #0x | 1inch | uniswap_v3
 dex_rpc = "https://rpc.ankr.com/eth"
 dex_block_explorer_url = "https://api.etherscan.io/api?"
 dex_block_explorer_api =  "798437294880920392"  #this is an example
 dex_router_contract_addr = "0x7a250d5630B4cF539739dF2C5dAcb4c659F2488D" #UNI_V2
```

### Comparing `dxsp-2.5.0/dxsp/main.py` & `dxsp-2.5.1/dxsp/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             self.logger.error(f"connectivity failed {e}")
             return
 
         self.protocol_type = settings.dex_protocol_type
         self.chain_id = settings.dex_chain_id
         self.wallet_address = self.w3.to_checksum_address(
             settings.dex_wallet_address)
-        self.account = self.wallet_address
+        self.account = str(self.chain_id) + " - "+str(self.wallet_address[-8])
         self.private_key = settings.dex_private_key
 
         try:
             self.cg = CoinGeckoAPI()
             asset_platforms = self.cg.get_asset_platforms()
             output_dict = next(
                 x for x in asset_platforms if x["chain_identifier"] == int(self.chain_id)
```

### Comparing `dxsp-2.5.0/pyproject.toml` & `dxsp-2.5.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.5.0"
+version = "2.5.1"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 
 
 [tool.poetry.urls]
```

### Comparing `dxsp-2.5.0/PKG-INFO` & `dxsp-2.5.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.5.0
+Version: 2.5.1
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

