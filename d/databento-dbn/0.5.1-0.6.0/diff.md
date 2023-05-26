# Comparing `tmp/databento_dbn-0.5.1-cp39-none-win_amd64.whl.zip` & `tmp/databento_dbn-0.6.0-cp39-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 547876 bytes, number of entries: 8
--rw-r--r--  4.6 unx     2966 b- defN 23-May-05 09:39 databento_dbn-0.5.1.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-May-05 09:39 databento_dbn-0.5.1.dist-info/WHEEL
--rw-r--r--  4.6 unx     9868 b- defN 23-May-05 09:39 databento_dbn-0.5.1.dist-info/license_files/LICENSE
--rw-r--r--  4.6 unx      135 b- defN 23-May-05 09:39 databento_dbn/__init__.py
--rw-r--r--  4.6 unx    37073 b- defN 23-May-05 09:39 databento_dbn/__init__.pyi
--rw-r--r--  4.6 unx        0 b- defN 23-May-05 09:39 databento_dbn/py.typed
--rwxr-xr-x  4.6 unx  1566720 b- defN 23-May-05 09:39 databento_dbn/databento_dbn.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      679 b- defN 23-May-05 09:39 databento_dbn-0.5.1.dist-info/RECORD
-8 files, 1617537 bytes uncompressed, 546688 bytes compressed:  66.2%
+Zip file size: 544943 bytes, number of entries: 8
+-rw-r--r--  4.6 unx     2966 b- defN 23-May-26 20:01 databento_dbn-0.6.0.dist-info/METADATA
+-rw-r--r--  4.6 unx       95 b- defN 23-May-26 20:01 databento_dbn-0.6.0.dist-info/WHEEL
+-rw-r--r--  4.6 unx     9868 b- defN 23-May-26 20:01 databento_dbn-0.6.0.dist-info/license_files/LICENSE
+-rw-r--r--  4.6 unx      135 b- defN 23-May-26 20:01 databento_dbn/__init__.py
+-rw-r--r--  4.6 unx    37132 b- defN 23-May-26 20:01 databento_dbn/__init__.pyi
+-rw-r--r--  4.6 unx        0 b- defN 23-May-26 20:01 databento_dbn/py.typed
+-rwxr-xr-x  4.6 unx  1555968 b- defN 23-May-26 20:01 databento_dbn/databento_dbn.cp39-win_amd64.pyd
+-rw-r--r--  4.6 unx      679 b- defN 23-May-26 20:01 databento_dbn-0.6.0.dist-info/RECORD
+8 files, 1606843 bytes uncompressed, 543755 bytes compressed:  66.2%
```

## zipnote {}

```diff
@@ -1,25 +1,25 @@
-Filename: databento_dbn-0.5.1.dist-info/METADATA
+Filename: databento_dbn-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: databento_dbn-0.5.1.dist-info/WHEEL
+Filename: databento_dbn-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: databento_dbn-0.5.1.dist-info/license_files/LICENSE
+Filename: databento_dbn-0.6.0.dist-info/license_files/LICENSE
 Comment: 
 
 Filename: databento_dbn/__init__.py
 Comment: 
 
 Filename: databento_dbn/__init__.pyi
 Comment: 
 
 Filename: databento_dbn/py.typed
 Comment: 
 
 Filename: databento_dbn/databento_dbn.cp39-win_amd64.pyd
 Comment: 
 
-Filename: databento_dbn-0.5.1.dist-info/RECORD
+Filename: databento_dbn-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## databento_dbn/__init__.pyi

```diff
@@ -279,22 +279,41 @@
         The common header.
 
         Returns
         -------
         RecordHeader
 
         """
+    @classmethod
+    def size_hint(cls) -> int:
+        """
+        Return an estimated size of the record in bytes.
+
+        Returns
+        -------
+        int
+
+        See Also
+        --------
+        record_size
+
+        """
+    @property
     def record_size(self) -> int:
         """
-        Return the size of the record.
+        Return the size of the record in bytes.
 
         Returns
         -------
         int
 
+        See Also
+        --------
+        size_hint
+
         """
     @property
     def rtype(self) -> int:
         """
         The record type.
 
         Returns
@@ -329,14 +348,25 @@
         nanoseconds since the UNIX epoch.
 
         Returns
         -------
         int
 
         """
+    @property
+    def ts_out(self) -> Optional[int]:
+        """
+        The live gateway send timestamp expressed as number of nanoseconds since
+        the UNIX epoch.
+
+        Returns
+        -------
+        Optional[int]
+
+        """
 
 class _MBOBase:
     """Base for market-by-order messages."""
 
     @property
     def order_id(self) -> int:
         """
@@ -613,15 +643,15 @@
 
     """
 
 class MBP1Msg(Record, _MBPBase):
     """Market by price implementation with a known book depth of 1."""
 
     @property
-    def booklevel(self) -> List[BidAskPair]:
+    def levels(self) -> List[BidAskPair]:
         """
         The top of the order book.
 
         Returns
         -------
         List[BidAskPair]
 
@@ -631,17 +661,17 @@
 
         """
 
 class MBP10Msg(Record, _MBPBase):
     """Market by price implementation with a known book depth of 10."""
 
     @property
-    def booklevel(self) -> List[BidAskPair]:
+    def levels(self) -> List[BidAskPair]:
         """
-        The top of the order book.
+        The top 10 levels.
 
         Returns
         -------
         List[BidAskPair]
 
         Notes
         -----
@@ -854,25 +884,14 @@
 
         Returns
         -------
         int
 
         """
     @property
-    def cleared_volume(self) -> int:
-        """
-        The total cleared volume of the instrument traded during the prior
-        trading session.
-
-        Returns
-        -------
-        int
-
-        """
-    @property
     def market_depth_implied(self) -> int:
         """
         The implied book depth on the price level data feed.
 
         Returns
         -------
         int
@@ -946,25 +965,14 @@
 
         Returns
         -------
         int
 
         """
     @property
-    def open_interest_qty(self) -> int:
-        """
-        The total open interest for the market at the close of the prior
-        trading session.
-
-        Returns
-        -------
-        int
-
-        """
-    @property
     def contract_multiplier(self) -> int:
         """
         The number of deliverables per instrument, i.e. peak days.
 
         Returns
         -------
         int
@@ -1640,16 +1648,16 @@
         -------
         int
 
         """
     @property
     def update_action(self) -> int:
         """
-        Indicates if the statistic is new added or deleted. Deleted is only
-        used for a couple stat types.
+        Indicates if the statistic is newly added (1) or deleted (2). (Deleted is only
+        used with some stat types)
 
         Returns
         -------
         int
 
         """
     @property
@@ -1750,35 +1758,35 @@
 
         Returns
         -------
         bool
 
         """
 
-class DbnDecoder:
+class DBNDecoder:
     """A class for decoding DBN data to Python objects."""
 
     def buffer(self) -> bytes:
         """
         Return the internal buffer of the decoder.
 
         Returns
         -------
         bytes
 
         """
     def decode(
         self,
-    ) -> List[Tuple[_DBNRecord, Optional[int]]]:
+    ) -> List[_DBNRecord]:
         """
         Decode the buffered data into DBN records.
 
         Returns
         -------
-        List[Tuple[DBNRecord, Optional[int]]]
+        List[DBNRecord]
 
         Raises
         ------
         ValueError
             When the decoding fails.
 
         See Also
@@ -1787,15 +1795,15 @@
 
         """
     def write(
         self,
         bytes: bytes,
     ) -> None:
         """
-        Write a sequence of bytes to the internal buffer of the DbnDecoder.
+        Write a sequence of bytes to the internal buffer of the DBNDecoder.
 
         Raises
         ------
         ValueError
             When the write to the internal buffer fails.
 
         See Also
```

## Comparing `databento_dbn-0.5.1.dist-info/METADATA` & `databento_dbn-0.6.0.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: databento-dbn
-Version: 0.5.1
+Version: 0.6.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Summary: Native Databento bindings based on dbn Rust crate
 Author: Databento <support@databento.com>
 Author-email: Databento <support@databento.com>
```

## Comparing `databento_dbn-0.5.1.dist-info/license_files/LICENSE` & `databento_dbn-0.6.0.dist-info/license_files/LICENSE`

 * *Files identical despite different names*

## Comparing `databento_dbn-0.5.1.dist-info/RECORD` & `databento_dbn-0.6.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-databento_dbn-0.5.1.dist-info/METADATA,sha256=BXaXjiVKqwVSUtw0qizKHVlwoV-Jb7k7A3tAZQ_JsDY,2966
-databento_dbn-0.5.1.dist-info/WHEEL,sha256=HfbNN9yA0Gn_6VCTRBzbKHMHpOwMN7MCpAKvpT7Uqyk,96
-databento_dbn-0.5.1.dist-info/license_files/LICENSE,sha256=d69bve2VkRS216XupRiyvjZOBPT0qV-eh9mHDCdxPSQ,9868
+databento_dbn-0.6.0.dist-info/METADATA,sha256=64Ha0vD3yZXj960RsRRlHR3YPlEsKVjMpzeWWFLqZo4,2966
+databento_dbn-0.6.0.dist-info/WHEEL,sha256=an3xOxErGJeHkLgr587-bgaHQa25SvmEjtVGHxu1c38,95
+databento_dbn-0.6.0.dist-info/license_files/LICENSE,sha256=d69bve2VkRS216XupRiyvjZOBPT0qV-eh9mHDCdxPSQ,9868
 databento_dbn/__init__.py,sha256=TeY-_YtACSjQLT3FBRPqxJrcYFf8yu_11WeB5LcyEKo,135
-databento_dbn/__init__.pyi,sha256=zYEg-aNDtUm1zN7Z1I8Lhuw4ByclShdeI6h4fDwAjoM,37073
+databento_dbn/__init__.pyi,sha256=yp5BpGlaUsszqWG6DvCBT_Lle5cKRjZktvwazW0Ux4g,37132
 databento_dbn/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-databento_dbn/databento_dbn.cp39-win_amd64.pyd,sha256=OsZzskZpOWHhqdhk5bj5KFo_Dto-rSkkLtB71qb1Se4,1566720
-databento_dbn-0.5.1.dist-info/RECORD,,
+databento_dbn/databento_dbn.cp39-win_amd64.pyd,sha256=KYWSs8liRClwREvl2A5x80Vc-9SETZDWkHfQcBInjk8,1555968
+databento_dbn-0.6.0.dist-info/RECORD,,
```

