# Comparing `tmp/binance-futures-connector-4.0.0rc1.tar.gz` & `tmp/binance-futures-connector-4.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "binance-futures-connector-4.0.0rc1.tar", last modified: Thu May 18 06:40:17 2023, max compression
+gzip compressed data, was "binance-futures-connector-4.0.0rc2.tar", last modified: Fri May 26 06:01:38 2023, max compression
```

## Comparing `binance-futures-connector-4.0.0rc1.tar` & `binance-futures-connector-4.0.0rc2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.375776 binance-futures-connector-4.0.0rc1/binance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.375776 binance-futures-connector-4.0.0rc1/binance/cm_futures/
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/cm_futures/portfolio_margin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/lib/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/um_futures/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29832 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/data_stream.py
--rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/market.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/um_futures/portfolio_margin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/websocket/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/binance_socket_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/websocket/cm_futures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/cm_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/cm_futures/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance/websocket/um_futures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/um_futures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/um_futures/websocket_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/binance/websocket/websocket_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 06:40:17.000000 binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/requirements/common.txt
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-18 06:40:17.379776 binance-futures-connector-4.0.0rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-18 06:40:11.000000 binance-futures-connector-4.0.0rc1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6147 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/cm_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28001 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20057 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/cm_futures/portfolio_margin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/lib/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1501 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/lib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/um_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31509 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/data_stream.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18300 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/market.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/um_futures/portfolio_margin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/websocket/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/binance_socket_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/websocket/cm_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/cm_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11396 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/cm_futures/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance/websocket/um_futures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/um_futures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9226 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/um_futures/websocket_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/binance/websocket/websocket_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1087 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 06:01:38.000000 binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/requirements/common.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 06:01:38.904294 binance-futures-connector-4.0.0rc2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-26 06:01:36.000000 binance-futures-connector-4.0.0rc2/setup.py
```

### Comparing `binance-futures-connector-4.0.0rc1/LICENSE.md` & `binance-futures-connector-4.0.0rc2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/PKG-INFO` & `binance-futures-connector-4.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-futures-connector
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: This is a lightweight library that works as a connector to Binance Futures public API.
 Home-page: https://github.com/binance/binance-futures-connector-python
 License: MIT
 Keywords: Binance futures,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-futures-connector-4.0.0rc1/README.md` & `binance-futures-connector-4.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/api.py` & `binance-futures-connector-4.0.0rc2/binance/api.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/cm_futures/__init__.py` & `binance-futures-connector-4.0.0rc2/binance/cm_futures/__init__.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/cm_futures/account.py` & `binance-futures-connector-4.0.0rc2/binance/cm_futures/account.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/cm_futures/data_stream.py` & `binance-futures-connector-4.0.0rc2/binance/cm_futures/data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/cm_futures/market.py` & `binance-futures-connector-4.0.0rc2/binance/cm_futures/market.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/error.py` & `binance-futures-connector-4.0.0rc2/binance/error.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/lib/authentication.py` & `binance-futures-connector-4.0.0rc2/binance/lib/authentication.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/lib/utils.py` & `binance-futures-connector-4.0.0rc2/binance/lib/utils.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/um_futures/__init__.py` & `binance-futures-connector-4.0.0rc2/binance/um_futures/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     # ACCOUNT(including orders and trades)
     from binance.um_futures.account import change_position_mode
     from binance.um_futures.account import get_position_mode
     from binance.um_futures.account import change_multi_asset_mode
     from binance.um_futures.account import get_multi_asset_mode
     from binance.um_futures.account import new_order
     from binance.um_futures.account import new_order_test
+    from binance.um_futures.account import modify_order
     from binance.um_futures.account import new_batch_order
     from binance.um_futures.account import query_order
     from binance.um_futures.account import cancel_order
     from binance.um_futures.account import cancel_open_orders
     from binance.um_futures.account import cancel_batch_order
     from binance.um_futures.account import countdown_cancel_order
     from binance.um_futures.account import get_open_orders
```

### Comparing `binance-futures-connector-4.0.0rc1/binance/um_futures/account.py` & `binance-futures-connector-4.0.0rc2/binance/um_futures/account.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,14 +144,76 @@
 
     check_required_parameters([[symbol, "symbol"], [side, "side"], [type, "type"]])
     params = {"symbol": symbol, "side": side, "type": type, **kwargs}
     url_path = "/fapi/v1/order/test"
     return self.sign_request("POST", url_path, params)
 
 
+def modify_order(
+    self,
+    symbol: str,
+    side: str,
+    quantity: float,
+    price: float,
+    orderId: int = None,
+    origClientOrderId: str = None,
+    **kwargs
+):
+    """
+    |
+    | **Modify Order (TRADE)**
+    | *Order modify function, currently only LIMIT order modification is supported, modified orders will be reordered in the match queue*
+
+    :API endpoint: ``PUT /fapi/v1/order``
+    :API doc: https://binance-docs.github.io/apidocs/futures/en/#modify-order-trade
+
+    :parameter symbol: string
+    :parameter side: string
+    :parameter quantity: float
+    :parameter price: float
+    :parameter orderId: optional int
+    :parameter origClientOrderId: optional string. Either orderId or origClientOrderId must be sent, and the orderId will prevail if both are sent.
+    :parameter recvWindow: optional int
+    |
+    """
+    check_required_parameters(
+        [
+            [symbol, "symbol"],
+            [side, "side"],
+            [quantity, "quantity"],
+            [price, "price"],
+        ]
+    )
+    if (orderId is None) and (origClientOrderId is None):
+        check_required_parameters(
+            [
+                [orderId, "orderId"],
+            ]
+        )
+    elif orderId:
+        params = {
+            "symbol": symbol,
+            "side": side,
+            "quantity": quantity,
+            "orderId": orderId,
+            **kwargs,
+        }
+    else:
+        params = {
+            "symbol": symbol,
+            "side": side,
+            "quantity": quantity,
+            "origClientOrderId": origClientOrderId,
+            **kwargs,
+        }
+
+    url_path = "/fapi/v1/order"
+    return self.sign_request("PUT", url_path, params)
+
+
 def new_batch_order(self, batchOrders: list):
     """
     |
     | **Place Multiple Orders (TRADE)**
     | *Post a new batch order*
 
     :API endpoint: ``POST /fapi/v1/batchOrders``
```

### Comparing `binance-futures-connector-4.0.0rc1/binance/um_futures/data_stream.py` & `binance-futures-connector-4.0.0rc2/binance/um_futures/data_stream.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/um_futures/market.py` & `binance-futures-connector-4.0.0rc2/binance/um_futures/market.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/websocket/binance_socket_manager.py` & `binance-futures-connector-4.0.0rc2/binance/websocket/binance_socket_manager.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/websocket/cm_futures/websocket_client.py` & `binance-futures-connector-4.0.0rc2/binance/websocket/cm_futures/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/websocket/um_futures/websocket_client.py` & `binance-futures-connector-4.0.0rc2/binance/websocket/um_futures/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance/websocket/websocket_client.py` & `binance-futures-connector-4.0.0rc2/binance/websocket/websocket_client.py`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/PKG-INFO` & `binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binance-futures-connector
-Version: 4.0.0rc1
+Version: 4.0.0rc2
 Summary: This is a lightweight library that works as a connector to Binance Futures public API.
 Home-page: https://github.com/binance/binance-futures-connector-python
 License: MIT
 Keywords: Binance futures,Public API
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Financial and Insurance Industry
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `binance-futures-connector-4.0.0rc1/binance_futures_connector.egg-info/SOURCES.txt` & `binance-futures-connector-4.0.0rc2/binance_futures_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `binance-futures-connector-4.0.0rc1/setup.py` & `binance-futures-connector-4.0.0rc2/setup.py`

 * *Files identical despite different names*

