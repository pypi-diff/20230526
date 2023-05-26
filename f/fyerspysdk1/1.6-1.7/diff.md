# Comparing `tmp/fyerspysdk1-1.6-py3-none-any.whl.zip` & `tmp/fyerspysdk1-1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 12619 bytes, number of entries: 9
+Zip file size: 12623 bytes, number of entries: 9
 -rw-rw-r--  2.0 unx       20 b- defN 23-May-22 12:28 fyerstest/__init__.py
 -rw-rw-r--  2.0 unx    16942 b- defN 23-May-23 12:11 fyerstest/fyersApi.py
--rw-rw-r--  2.0 unx    18823 b- defN 23-May-26 12:43 fyerstest/hsmFyers.py
--rw-rw-r--  2.0 unx     8276 b- defN 23-May-23 12:17 fyerstest/ws.py
--rwxrwxr-x  2.0 unx     1063 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/LICENSE.txt
--rw-rw-r--  2.0 unx      622 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/WHEEL
--rw-rw-r--  2.0 unx       10 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      705 b- defN 23-May-26 12:48 fyerspysdk1-1.6.dist-info/RECORD
-9 files, 46553 bytes uncompressed, 11411 bytes compressed:  75.5%
+-rw-rw-r--  2.0 unx    18823 b- defN 23-May-26 12:55 fyerstest/hsmFyers.py
+-rw-rw-r--  2.0 unx     8284 b- defN 23-May-26 12:55 fyerstest/ws.py
+-rwxrwxr-x  2.0 unx     1063 b- defN 23-May-26 12:55 fyerspysdk1-1.7.dist-info/LICENSE.txt
+-rw-rw-r--  2.0 unx      622 b- defN 23-May-26 12:55 fyerspysdk1-1.7.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 12:55 fyerspysdk1-1.7.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       10 b- defN 23-May-26 12:55 fyerspysdk1-1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      705 b- defN 23-May-26 12:55 fyerspysdk1-1.7.dist-info/RECORD
+9 files, 46561 bytes uncompressed, 11415 bytes compressed:  75.5%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: fyerstest/hsmFyers.py
 Comment: 
 
 Filename: fyerstest/ws.py
 Comment: 
 
-Filename: fyerspysdk1-1.6.dist-info/LICENSE.txt
+Filename: fyerspysdk1-1.7.dist-info/LICENSE.txt
 Comment: 
 
-Filename: fyerspysdk1-1.6.dist-info/METADATA
+Filename: fyerspysdk1-1.7.dist-info/METADATA
 Comment: 
 
-Filename: fyerspysdk1-1.6.dist-info/WHEEL
+Filename: fyerspysdk1-1.7.dist-info/WHEEL
 Comment: 
 
-Filename: fyerspysdk1-1.6.dist-info/top_level.txt
+Filename: fyerspysdk1-1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: fyerspysdk1-1.6.dist-info/RECORD
+Filename: fyerspysdk1-1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fyerstest/ws.py

```diff
@@ -205,12 +205,12 @@
 				}
 			},
 		}
         dictConfig(LOGGING)
         self.logger = logging.getLogger('fyers_socket')
 
 
-# client_id = "XC4EOD67IM-100"
-access_token=  "XC4EOD67IM-100:eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODQ4MTM5NTgsImV4cCI6MTY4NDg4ODIzOCwibmJmIjoxNjg0ODEzOTU4LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa2JEaUd1Q1BGek1uUFlXTVFxRjNvUGt0T3lsRDhpNzMyOTJfS0VVZUl6RU1oc2lKMTNLV2dfc2ZWU1BBWTFNdmxGblQtQzh0dG1VX1hqM1NYSklLLTNkaVFHMTZJVE5kTDlvVTJKSmxVbjBwNlI1UT0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.s4CJCOZCnUohVaMttSwA_Iz0p9t-HHSHNwqED5NemhQ"
+# # client_id = "XC4EOD67IM-100"
+# access_token=  "XC4EOD67IM-100:eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJpc3MiOiJhcGkuZnllcnMuaW4iLCJpYXQiOjE2ODQ4MTM5NTgsImV4cCI6MTY4NDg4ODIzOCwibmJmIjoxNjg0ODEzOTU4LCJhdWQiOlsieDowIiwieDoxIiwieDoyIiwiZDoxIiwiZDoyIiwieDoxIiwieDowIl0sInN1YiI6ImFjY2Vzc190b2tlbiIsImF0X2hhc2giOiJnQUFBQUFCa2JEaUd1Q1BGek1uUFlXTVFxRjNvUGt0T3lsRDhpNzMyOTJfS0VVZUl6RU1oc2lKMTNLV2dfc2ZWU1BBWTFNdmxGblQtQzh0dG1VX1hqM1NYSklLLTNkaVFHMTZJVE5kTDlvVTJKSmxVbjBwNlI1UT0iLCJkaXNwbGF5X25hbWUiOiJWSU5BWSBLVU1BUiBNQVVSWUEiLCJvbXMiOiJLMSIsImZ5X2lkIjoiWFYyMDk4NiIsImFwcFR5cGUiOjEwMCwicG9hX2ZsYWciOiJOIn0.s4CJCOZCnUohVaMttSwA_Iz0p9t-HHSHNwqED5NemhQ"
 
-fyers= FyersSocket(access_token,False , None)
-fyers.subscribe("OnOrders,OnTrades,OnPositions")
+# fyers= FyersSocket(access_token,False , None)
+# fyers.subscribe("OnOrders,OnTrades,OnPositions")
```

## Comparing `fyerspysdk1-1.6.dist-info/LICENSE.txt` & `fyerspysdk1-1.7.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `fyerspysdk1-1.6.dist-info/METADATA` & `fyerspysdk1-1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fyerspysdk1
-Version: 1.6
+Version: 1.7
 Summary: XX trc APIs.
 Home-page: https://github.com
 Author: my-Tech
 Author-email: support@f.in
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

