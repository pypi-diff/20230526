# Comparing `tmp/coinmetrics_api_client-2023.5.2.20.tar.gz` & `tmp/coinmetrics_api_client-2023.5.26.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coinmetrics_api_client-2023.5.2.20.tar", max compression
+gzip compressed data, was "coinmetrics_api_client-2023.5.26.17.tar", max compression
```

## Comparing `coinmetrics_api_client-2023.5.2.20.tar` & `coinmetrics_api_client-2023.5.26.17.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1088 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/LICENSE
--rw-r--r--   0        0        0    20460 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/README.md
--rw-r--r--   0        0        0       28 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/coinmetrics/__init__.py
--rw-r--r--   0        0        0    21093 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_catalogs.py
--rw-r--r--   0        0        0     9947 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_data_collection.py
--rw-r--r--   0        0        0     2328 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_exceptions.py
--rw-r--r--   0        0        0     1181 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_models.py
--rw-r--r--   0        0        0      699 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_typing.py
--rw-r--r--   0        0        0     3951 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/_utils.py
--rw-r--r--   0        0        0   233224 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/coinmetrics/api_client.py
--rw-r--r--   0        0        0        0 2023-05-02 20:44:04.348483 coinmetrics_api_client-2023.5.2.20/coinmetrics/build.py
--rw-r--r--   0        0        0      148 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/constants.py
--rw-r--r--   0        0        0    20520 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/data_exporter.py
--rw-r--r--   0        0        0     8669 2023-04-28 17:38:26.499618 coinmetrics_api_client-2023.5.2.20/coinmetrics/typer_cli.py
--rw-r--r--   0        0        0     1236 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-02 20:44:04.352483 coinmetrics_api_client-2023.5.2.20/test/__init__.py
--rw-r--r--   0        0        0     1640 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pair_candles.csv
--rw-r--r--   0        0        0      412 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pairs.csv
--rw-r--r--   0        0        0     2097 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_markets.csv
--rw-r--r--   0        0        0      605 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_metrics.csv
--rw-r--r--   0        0        0      436 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchange_assets.csv
--rw-r--r--   0        0        0     3595 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_markets.csv
--rw-r--r--   0        0        0      822 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_metrics.csv
--rw-r--r--   0        0        0      556 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_indexes.csv
--rw-r--r--   0        0        0      223 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_institutions.csv
--rw-r--r--   0        0        0      178 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_orderbooks.csv
--rw-r--r--   0        0        0      254 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_quotes.csv
--rw-r--r--   0        0        0      297 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_market_trades.csv
--rw-r--r--   0        0        0      579 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_markets.csv
--rw-r--r--   0        0        0     2557 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/data/catalog_metrics.csv
--rw-r--r--   0        0        0    28915 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_api_client.py
--rw-r--r--   0        0        0    10311 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_api_methods.py
--rw-r--r--   0        0        0     2910 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_as_list.py
--rw-r--r--   0        0        0     1788 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_blockchain_methods.py
--rw-r--r--   0        0        0     2273 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_custom_exceptions.py
--rw-r--r--   0        0        0    13462 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_data_exporter.py
--rw-r--r--   0        0        0     1015 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_debugging.py
--rw-r--r--   0        0        0     2142 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_models.py
--rw-r--r--   0        0        0     1193 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/test/test_rate_limits.py
--rw-r--r--   0        0        0    14167 2023-04-28 17:38:26.519618 coinmetrics_api_client-2023.5.2.20/test/test_to_dataframe.py
--rw-r--r--   0        0        0     5829 2023-05-02 20:38:43.207920 coinmetrics_api_client-2023.5.2.20/test/test_websocket_methods.py
--rw-r--r--   0        0        0    21648 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.5.2.20/PKG-INFO
+-rw-r--r--   0        0        0     1088 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/LICENSE
+-rw-r--r--   0        0        0    20460 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/README.md
+-rw-r--r--   0        0        0       29 2023-05-26 17:44:05.653887 coinmetrics_api_client-2023.5.26.17/coinmetrics/__init__.py
+-rw-r--r--   0        0        0    20751 2023-05-26 17:43:04.970269 coinmetrics_api_client-2023.5.26.17/coinmetrics/_catalogs.py
+-rw-r--r--   0        0        0     9947 2023-04-21 16:07:42.661803 coinmetrics_api_client-2023.5.26.17/coinmetrics/_data_collection.py
+-rw-r--r--   0        0        0     2328 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/coinmetrics/_exceptions.py
+-rw-r--r--   0        0        0     1286 2023-05-26 17:43:04.970269 coinmetrics_api_client-2023.5.26.17/coinmetrics/_models.py
+-rw-r--r--   0        0        0      699 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/coinmetrics/_typing.py
+-rw-r--r--   0        0        0     3951 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/coinmetrics/_utils.py
+-rw-r--r--   0        0        0   233688 2023-05-26 17:43:04.970269 coinmetrics_api_client-2023.5.26.17/coinmetrics/api_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 17:52:06.838675 coinmetrics_api_client-2023.5.26.17/coinmetrics/build.py
+-rw-r--r--   0        0        0      148 2023-03-15 16:25:45.282233 coinmetrics_api_client-2023.5.26.17/coinmetrics/constants.py
+-rw-r--r--   0        0        0    20520 2023-03-15 18:54:39.226986 coinmetrics_api_client-2023.5.26.17/coinmetrics/data_exporter.py
+-rw-r--r--   0        0        0     8669 2023-03-15 16:25:45.286233 coinmetrics_api_client-2023.5.26.17/coinmetrics/typer_cli.py
+-rw-r--r--   0        0        0     1237 2023-05-26 17:44:05.657887 coinmetrics_api_client-2023.5.26.17/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 17:52:06.842675 coinmetrics_api_client-2023.5.26.17/test/__init__.py
+-rw-r--r--   0        0        0     1640 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_asset_pair_candles.csv
+-rw-r--r--   0        0        0      412 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_asset_pairs.csv
+-rw-r--r--   0        0        0     2097 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_assets_markets.csv
+-rw-r--r--   0        0        0      605 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_assets_metrics.csv
+-rw-r--r--   0        0        0      436 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchange_assets.csv
+-rw-r--r--   0        0        0     3595 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchanges_markets.csv
+-rw-r--r--   0        0        0      822 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchanges_metrics.csv
+-rw-r--r--   0        0        0      556 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_indexes.csv
+-rw-r--r--   0        0        0      223 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_institutions.csv
+-rw-r--r--   0        0        0      178 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_market_orderbooks.csv
+-rw-r--r--   0        0        0      254 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_market_quotes.csv
+-rw-r--r--   0        0        0      297 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_market_trades.csv
+-rw-r--r--   0        0        0      579 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_markets.csv
+-rw-r--r--   0        0        0     2557 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/data/catalog_metrics.csv
+-rw-r--r--   0        0        0    28915 2023-03-15 16:25:45.302233 coinmetrics_api_client-2023.5.26.17/test/test_api_client.py
+-rw-r--r--   0        0        0    10311 2023-04-10 18:58:58.715180 coinmetrics_api_client-2023.5.26.17/test/test_api_methods.py
+-rw-r--r--   0        0        0     2910 2023-03-16 17:53:46.528810 coinmetrics_api_client-2023.5.26.17/test/test_as_list.py
+-rw-r--r--   0        0        0     1788 2023-04-10 18:58:58.715180 coinmetrics_api_client-2023.5.26.17/test/test_blockchain_methods.py
+-rw-r--r--   0        0        0     2273 2023-03-15 16:25:45.306233 coinmetrics_api_client-2023.5.26.17/test/test_custom_exceptions.py
+-rw-r--r--   0        0        0    13462 2023-03-15 16:25:45.306233 coinmetrics_api_client-2023.5.26.17/test/test_data_exporter.py
+-rw-r--r--   0        0        0     1015 2023-03-15 16:25:45.306233 coinmetrics_api_client-2023.5.26.17/test/test_debugging.py
+-rw-r--r--   0        0        0     2142 2023-04-21 16:07:42.665803 coinmetrics_api_client-2023.5.26.17/test/test_models.py
+-rw-r--r--   0        0        0     1193 2023-05-02 20:36:52.152834 coinmetrics_api_client-2023.5.26.17/test/test_rate_limits.py
+-rw-r--r--   0        0        0    14167 2023-04-25 18:16:09.653330 coinmetrics_api_client-2023.5.26.17/test/test_to_dataframe.py
+-rw-r--r--   0        0        0     5829 2023-05-02 20:36:52.152834 coinmetrics_api_client-2023.5.26.17/test/test_websocket_methods.py
+-rw-r--r--   0        0        0    21649 1970-01-01 00:00:00.000000 coinmetrics_api_client-2023.5.26.17/PKG-INFO
```

### Comparing `coinmetrics_api_client-2023.5.2.20/LICENSE` & `coinmetrics_api_client-2023.5.26.17/LICENSE`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/README.md` & `coinmetrics_api_client-2023.5.26.17/README.md`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/_catalogs.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/_catalogs.py`

 * *Files 4% similar despite different names*

```diff
@@ -399,25 +399,19 @@
     """
     Transforms catalog data in list form into a dataframe
     :return: Catalog Data
     """
 
     def to_dataframe(self) -> DataFrameType:
         df_markets = pd.DataFrame(self)
-        df_markets = df_markets.join(
-            df_markets["trades"].apply(pd.Series).drop(0, axis=1, errors="ignore"),
-            rsuffix="_trades",
-        )
-        metadata = ["funding_rates", "openinterest", "liquidations"]
+        metadata = ["trades", "funding_rates", "openinterest", "liquidations"]
         for col in metadata:
             if col in df_markets.columns:
-                df_markets = df_markets.join(
-                    df_markets[col].apply(pd.Series).drop(0, axis=1, errors="ignore"),
-                    rsuffix=f"_{col}",
-                )
+                for time_col in ["min_time", "max_time"]:
+                    df_markets[f'{time_col}_{col}'] = df_markets[col].apply(lambda item: None if isinstance(item, float) else item.get(time_col, None))
 
         df_markets = df_markets.drop(
             ["trades", "funding_rates", "openinterest", "liquidations"],
             axis=1,
             errors="ignore",
         )
         return convert_catalog_dtypes(df_markets)
@@ -527,37 +521,23 @@
     """
     Transforms catalog data in list form into a dataframe
     :return: Catalog Data
     """
 
     def to_dataframe(self) -> DataFrameType:
         df_catalog_market_metrics = pd.DataFrame(self)
-        df_catalog_market_metrics = (
-            df_catalog_market_metrics.explode("metrics")
-            .assign(metric=lambda df: _expand_df(key="metric", iterable=df.metrics))
-            .assign(
-                frequencies=lambda df: _expand_df(
-                    key="frequencies", iterable=df.metrics
-                )
-            )
-            .explode("frequencies")
-            .assign(
-                frequency=lambda df: _expand_df(
-                    key="frequency", iterable=df.frequencies
-                )
-            )
-            .assign(
-                min_time=lambda df: _expand_df(key="min_time", iterable=df.frequencies)
-            )
-            .assign(
-                max_time=lambda df: _expand_df(key="max_time", iterable=df.frequencies)
-            )
-            .reset_index(drop=True)
-            .drop(["metrics", "frequencies"], axis=1)
-        )
+        df_catalog_market_metrics = df_catalog_market_metrics.explode("metrics")
+        df_metrics = pd.json_normalize(df_catalog_market_metrics['metrics'])
+        df_catalog_market_metrics = df_catalog_market_metrics.join(df_metrics)
+        df_catalog_market_metrics = df_catalog_market_metrics.explode("frequencies")
+        df_frequencies = pd.json_normalize(df_catalog_market_metrics['frequencies'])
+        df_catalog_market_metrics = df_catalog_market_metrics.join(df_frequencies)
+        df_catalog_market_metrics = df_catalog_market_metrics.drop(["metrics", "frequencies"], axis=1)
+        df_catalog_market_metrics = df_catalog_market_metrics.reset_index(drop=True)
+
         return convert_catalog_dtypes(df_catalog_market_metrics)
 
 
 class CatalogMarketCandlesData(List[Any]):
     """
     Transforms catalog data in list form into a dataframe
     :return: Catalog Data
```

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/_data_collection.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/_data_collection.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/_exceptions.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/_models.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/_models.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,7 +37,9 @@
     status_updates: List[str]
     details: str
     mempool_approx_queue_position: str = field(default="None")
     next_block_approx_settlement_probability_pct: str = field(default="0")
     block_hash: str = field(default="None")
     geo: str = field(default="None")
     replacement_for_txid: str = field(default="None")
+    inputs: List[str] = field(default_factory=list)
+    outputs: List[str] = field(default_factory=list)
```

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/_typing.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/_typing.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/_utils.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/_utils.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/api_client.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1911,14 +1911,15 @@
         page_size: Optional[int] = None,
         paging_from: Optional[Union[PagingFrom, str]] = "start",
         start_time: Optional[Union[datetime, date, str]] = None,
         end_time: Optional[Union[datetime, date, str]] = None,
         start_inclusive: Optional[bool] = None,
         end_inclusive: Optional[bool] = None,
         timezone: Optional[str] = None,
+        include_heartbeats: Optional[bool] = None
     ) -> DataCollection:
         """
         Returns asset alerts for the specified assets.
 
         :param assets: list of asset names, e.g. 'btc'
         :type assets: list(str), str
         :param alerts: list of asset alert names
@@ -1933,28 +1934,31 @@
         :type end_time: datetime, date, str
         :param start_inclusive: Flag to define if start timestamp must be included in the timeseries if present. True by default.
         :type start_inclusive: bool
         :param end_inclusive: Flag to define if end timestamp must be included in the timeseries if present. True by default.
         :type end_inclusive: bool
         :param timezone: timezone of the start/end times in db format for example: "America/Chicago". Default value is "UTC". For more details check out API documentation page.
         :type timezone: str
+        :param include_heartbeats:  If set to true, includes information about most recent time asset was successfully evaluated.
+        :type include_heartbeats: bool
         :return: Asset alerts timeseries.
         :rtype: DataCollection
         """
 
         params: Dict[str, Any] = {
             "assets": assets,
             "alerts": alerts,
             "page_size": page_size,
             "paging_from": paging_from,
             "start_time": start_time,
             "end_time": end_time,
             "start_inclusive": start_inclusive,
             "end_inclusive": end_inclusive,
             "timezone": timezone,
+            "include_heartbeats": include_heartbeats
         }
         return DataCollection(self._get_data, "timeseries/asset-alerts", params)
 
     def get_defi_balance_sheets(
         self,
         defi_protocols: Union[str, List[str]],
         page_size: Optional[int] = None,
@@ -4400,24 +4404,26 @@
             "next_page_token": next_page_token,
         }
         return DataCollection(self._get_data, f"blockchain-v2/{asset}/accounts/{account}/balance-updates", params)
 
     def get_transaction_tracker(
         self,
         asset: str,
+        addresses: Optional[Union[List[str], str]] = None,
         txids: Optional[Union[List[str], str]] = None,
         replacements_for_txids: Optional[Union[List[str], str]] = None,
         replacements_only: Optional[bool] = None,
         page_size: Optional[int] = None,
         paging_from: Optional[Union[PagingFrom, str]] = "start",
         start_time: Optional[Union[datetime, date, str]] = None,
         end_time: Optional[Union[datetime, date, str]] = None,
         start_inclusive: Optional[bool] = None,
         end_inclusive: Optional[bool] = None,
         timezone: Optional[str] = None,
+        unconfirmed_only: Optional[bool] = None
     ) -> TransactionTrackerDataCollection:
         """
         Returns status updates for the specified or all transactions.
 
         :param asset: Asset name
         :type asset: str
         :param txids: Optional comma separated list of transaction identifiers (txid) to track.
@@ -4441,24 +4447,26 @@
         :param timezone: timezone of the start/end times in db format for example: "America/Chicago". Default value is "UTC". For more details check out API documentation page.
         :type timezone: str
         :return: status updates for the specified or all transactions.
         :rtype: TransactionTrackerDataCollection
         """
         params: Dict[str, Any] = {
             "asset": asset,
+            "addresses": addresses,
             "txids": txids,
             "replacements_for_txids": replacements_for_txids,
             "replacements_only": replacements_only,
             "page_size": page_size,
             "paging_from": paging_from,
             "start_time": start_time,
             "end_time": end_time,
             "start_inclusive": start_inclusive,
             "end_inclusive": end_inclusive,
             "timezone": timezone,
+            "unconfirmed_only": unconfirmed_only
         }
         return TransactionTrackerDataCollection(
             self._get_data, f"blockchain/{asset}/transaction-tracker", params
         )
 
     def get_taxonomy_assets(
         self,
```

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/data_exporter.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/coinmetrics/typer_cli.py` & `coinmetrics_api_client-2023.5.26.17/coinmetrics/typer_cli.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/pyproject.toml` & `coinmetrics_api_client-2023.5.26.17/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coinmetrics-api-client"
-version = "2023.5.2.20"
+version = "2023.5.26.17"
 description = "Python client for Coin Metrics API v4."
 authors = ["Coin Metrics <info@coinmetrics.io>", "Oleksandr Buchkovskyi <oleksandr@coinmetrics.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://coinmetrics.github.io/api-client-python/site/index.html"
 repository = "https://github.com/coinmetrics/api-client-python"
 packages = [{include = "coinmetrics"}]
```

### Comparing `coinmetrics_api_client-2023.5.2.20/test/data/catalog_asset_pair_candles.csv` & `coinmetrics_api_client-2023.5.26.17/test/data/catalog_asset_pair_candles.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_markets.csv` & `coinmetrics_api_client-2023.5.26.17/test/data/catalog_assets_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/data/catalog_assets_metrics.csv` & `coinmetrics_api_client-2023.5.26.17/test/data/catalog_assets_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_markets.csv` & `coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchanges_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/data/catalog_exchanges_metrics.csv` & `coinmetrics_api_client-2023.5.26.17/test/data/catalog_exchanges_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/data/catalog_indexes.csv` & `coinmetrics_api_client-2023.5.26.17/test/data/catalog_indexes.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/data/catalog_markets.csv` & `coinmetrics_api_client-2023.5.26.17/test/data/catalog_markets.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/data/catalog_metrics.csv` & `coinmetrics_api_client-2023.5.26.17/test/data/catalog_metrics.csv`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_api_client.py` & `coinmetrics_api_client-2023.5.26.17/test/test_api_client.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_api_methods.py` & `coinmetrics_api_client-2023.5.26.17/test/test_api_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_as_list.py` & `coinmetrics_api_client-2023.5.26.17/test/test_as_list.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_blockchain_methods.py` & `coinmetrics_api_client-2023.5.26.17/test/test_blockchain_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_custom_exceptions.py` & `coinmetrics_api_client-2023.5.26.17/test/test_custom_exceptions.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_data_exporter.py` & `coinmetrics_api_client-2023.5.26.17/test/test_data_exporter.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_debugging.py` & `coinmetrics_api_client-2023.5.26.17/test/test_debugging.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_models.py` & `coinmetrics_api_client-2023.5.26.17/test/test_models.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_rate_limits.py` & `coinmetrics_api_client-2023.5.26.17/test/test_rate_limits.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_to_dataframe.py` & `coinmetrics_api_client-2023.5.26.17/test/test_to_dataframe.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/test/test_websocket_methods.py` & `coinmetrics_api_client-2023.5.26.17/test/test_websocket_methods.py`

 * *Files identical despite different names*

### Comparing `coinmetrics_api_client-2023.5.2.20/PKG-INFO` & `coinmetrics_api_client-2023.5.26.17/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coinmetrics-api-client
-Version: 2023.5.2.20
+Version: 2023.5.26.17
 Summary: Python client for Coin Metrics API v4.
 Home-page: https://coinmetrics.github.io/api-client-python/site/index.html
 License: MIT
 Keywords: coin metrics,coin,metrics,crypto,bitcoin,network-data,market-data,api,handy
 Author: Coin Metrics
 Author-email: info@coinmetrics.io
 Requires-Python: >=3.7.1,<4.0.0
```

