# Comparing `tmp/graham_client-0.0.2-py3.10.egg` & `tmp/graham_client-0.0.3-py3.10.egg`

## zipinfo {}

```diff
@@ -1,20 +1,20 @@
-Zip file size: 9354 bytes, number of entries: 18
--rw-r--r--  2.0 unx      282 b- defN 23-May-26 07:35 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      338 b- defN 23-May-26 07:35 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-26 07:35 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       42 b- defN 23-May-26 07:35 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-26 07:35 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-26 07:35 EGG-INFO/zip-safe
+Zip file size: 9574 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      282 b- defN 23-May-26 10:26 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      338 b- defN 23-May-26 10:26 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-26 10:26 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       42 b- defN 23-May-26 10:26 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-26 10:26 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-26 10:27 EGG-INFO/zip-safe
 -rw-r--r--  2.0 unx        0 b- defN 23-May-24 07:26 examples/__init__.py
 -rw-r--r--  2.0 unx      549 b- defN 23-May-26 07:25 examples/demo-financials.py
 -rw-r--r--  2.0 unx      356 b- defN 23-May-25 10:17 examples/demo-tables.py
--rw-r--r--  2.0 unx      152 b- defN 23-May-26 07:35 examples/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx      587 b- defN 23-May-26 07:35 examples/__pycache__/demo-financials.cpython-310.pyc
--rw-r--r--  2.0 unx      478 b- defN 23-May-26 07:35 examples/__pycache__/demo-tables.cpython-310.pyc
+-rw-r--r--  2.0 unx      152 b- defN 23-May-26 10:26 examples/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx      587 b- defN 23-May-26 10:26 examples/__pycache__/demo-financials.cpython-310.pyc
+-rw-r--r--  2.0 unx      478 b- defN 23-May-26 10:26 examples/__pycache__/demo-tables.cpython-310.pyc
 -rw-r--r--  2.0 unx      498 b- defN 23-May-25 10:17 graham/__init__.py
--rw-r--r--  2.0 unx     6199 b- defN 23-May-26 07:33 graham/equities.py
--rw-r--r--  2.0 unx     4364 b- defN 23-May-26 07:18 graham/tables.py
--rw-r--r--  2.0 unx      975 b- defN 23-May-26 07:35 graham/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     3638 b- defN 23-May-26 07:35 graham/__pycache__/equities.cpython-310.pyc
--rw-r--r--  2.0 unx     2938 b- defN 23-May-26 07:35 graham/__pycache__/tables.cpython-310.pyc
-18 files, 21414 bytes uncompressed, 6924 bytes compressed:  67.7%
+-rw-r--r--  2.0 unx     6547 b- defN 23-May-26 10:22 graham/equities.py
+-rw-r--r--  2.0 unx     4596 b- defN 23-May-26 10:24 graham/tables.py
+-rw-r--r--  2.0 unx      975 b- defN 23-May-26 10:26 graham/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     3936 b- defN 23-May-26 10:26 graham/__pycache__/equities.cpython-310.pyc
+-rw-r--r--  2.0 unx     3131 b- defN 23-May-26 10:26 graham/__pycache__/tables.cpython-310.pyc
+18 files, 22485 bytes uncompressed, 7144 bytes compressed:  68.2%
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graham-client
-Version: 0.0.2
+Version: 0.0.3
 Summary: A Python client for withgraham.io
 Author: WithGraham
 Author-email: support@withgraham.io
 Keywords: python,financial,data,api,withgraham,graham,value investing
 License-File: LICENSE
 
 A Python client for withgraham.io
```

## graham/equities.py

```diff
@@ -3,14 +3,18 @@
 
 class Financials:
     def __init__(self, rate_limiter, api_key, company_id, return_raw=False):
         self.rate_limiter = rate_limiter
         self.api_key = api_key
         self.company_id = company_id
         self.return_raw = return_raw
+        self.timeout = 15
+    
+    def _get_timeout(self):
+        return self.timeout
     
     def _get_headers(self):
         return {
             'Authorization': 'Bearer ' + self.api_key,
             'Company': self.company_id,
             'Content-Type': 'application/json'
         }
@@ -18,15 +22,15 @@
     def ListSummary(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
             url = 'https://api.withgraham.io/v1/equities/' + str(equity_id) + '/financials'
             if query_str != '':
                 url += '?' + query_str
             
-            r = requests.get(url, headers=self._get_headers(), json=None)
+            r = requests.get(url, headers=self._get_headers(), json=None, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to get financials for equity'
                 }
             
@@ -41,15 +45,15 @@
     def ListSECForms(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
             url = 'https://api.withgraham.io/v1/equities/' + str(equity_id) + '/financials/sec-forms'
             if query_str != '':
                 url += '?' + query_str
             
-            r = requests.get(url, headers=self._get_headers(), json=None)
+            r = requests.get(url, headers=self._get_headers(), json=None, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to get SEC forms for equity'
                 }
             
@@ -64,14 +68,18 @@
 
 class Equities:
     def __init__(self, rate_limiter, api_key, company_id, return_raw=False):
         self.rate_limiter = rate_limiter
         self.api_key = api_key
         self.company_id = company_id
         self.return_raw = return_raw
+        self.timeout = 15
+    
+    def _get_timeout(self):
+        return self.timeout
     
     def _get_headers(self):
         return {
             'Authorization': 'Bearer ' + self.api_key,
             'Company': self.company_id,
             'Content-Type': 'application/json'
         }
@@ -79,15 +87,15 @@
     def List(self, query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
             url = 'https://api.withgraham.io/v1/equities'
             if query_str != '':
                 url += '?' + query_str
             
-            r = requests.get(url, headers=self._get_headers(), json=None)
+            r = requests.get(url, headers=self._get_headers(), json=None, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to list equities'
                 }
             
@@ -102,15 +110,15 @@
     def Get(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
             url = 'https://api.withgraham.io/v1/equities/' + str(equity_id)
             if query_str != '':
                 url += '?' + query_str
             
-            r = requests.get(url, headers=self._get_headers(), json=None)
+            r = requests.get(url, headers=self._get_headers(), json=None, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to get equity'
                 }
             
@@ -125,15 +133,15 @@
     def Daily(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
             url = 'https://api.withgraham.io/v1/equities/' + str(equity_id) + '/daily'
             if query_str != '':
                 url += '?' + query_str
             
-            r = requests.get(url, headers=self._get_headers(), json=None)
+            r = requests.get(url, headers=self._get_headers(), json=None, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to get daily snapshot for equity'
                 }
             
@@ -151,15 +159,15 @@
     def Dividends(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
             url = 'https://api.withgraham.io/v1/equities/' + str(equity_id) + '/dividends'
             if query_str != '':
                 url += '?' + query_str
             
-            r = requests.get(url, headers=self._get_headers(), json=None)
+            r = requests.get(url, headers=self._get_headers(), json=None, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to get equity'
                 }
```

## graham/tables.py

```diff
@@ -7,14 +7,18 @@
                 'status_code': 400,
                 'error_message': 'Table ID is required'
             }
         self.rate_limiter = rate_limiter
         self.table_id = table_id
         self.api_key = api_key
         self.company_id = company_id
+        self.timeout = 15
+    
+    def _get_timeout(self):
+        return self.timeout
     
     def _get_headers(self):
         return {
             'Authorization': 'Bearer ' + self.api_key,
             'Company': self.company_id,
             'Content-Type': 'application/json'
         }
@@ -26,15 +30,15 @@
                 "query": query,
             }
             if limit != None:
                 payload['limit'] = limit
             if selectedColumns != None:
                 payload['selectedColumns'] = selectedColumns
             
-            r = requests.post(url, headers=self._get_headers(), json=payload)
+            r = requests.post(url, headers=self._get_headers(), json=payload, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to read from table'
                 }
             return r.json()['results'], None
@@ -46,15 +50,15 @@
     def Write(self, data = {}):
         with self.rate_limiter:
             url = 'https://api.withgraham.io/v1/tables/' + str(self.table_id) + '/data'
             payload = {
                 "data": data,
             }
             
-            r = requests.post(url, headers=self._get_headers(), json=payload)
+            r = requests.post(url, headers=self._get_headers(), json=payload, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to write to table'
                 }
             return r.json()['results'], None
@@ -66,15 +70,15 @@
     def Delete(self, query = {}):
         with self.rate_limiter:
             url = 'https://api.withgraham.io/v1/tables/' + str(self.table_id) + '/data'
             payload = {
                 "query": query,
             }
             
-            r = requests.delete(url, headers=self._get_headers(), json=payload)
+            r = requests.delete(url, headers=self._get_headers(), json=payload, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to delete from table'
                 }
             return r.json()['results'], None
@@ -83,15 +87,15 @@
             'error_message': 'rate limit exceeded'
         }
     
     def DeleteAll(self):
         with self.rate_limiter:
             url = 'https://api.withgraham.io/v1/tables/' + str(self.table_id) + '/data/all'
 
-            r = requests.delete(url, headers=self._get_headers(), json={})
+            r = requests.delete(url, headers=self._get_headers(), json={}, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to delete from table'
                 }
             return r.json()['results'], None
@@ -104,15 +108,15 @@
         with self.rate_limiter:
             url = 'https://api.withgraham.io/v1/tables/' + str(self.table_id) + '/data'
             payload = {
                 "data": data,
                 "query": query,
             }
             
-            r = requests.patch(url, headers=self._get_headers(), json=payload)
+            r = requests.patch(url, headers=self._get_headers(), json=payload, timeout=self._get_timeout())
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to update table'
                 }
             return r.json()['results'], None
```

## graham/__pycache__/equities.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 11:33:31 2023 UTC, .py size: 6199 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,228 +1,246 @@
-00000000: 6f0d 0d0a 0000 0000 0b99 7064 3718 0000  o.........pd7...
+00000000: 6f0d 0d0a 0000 0000 8dc0 7064 9319 0000  o.........pd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 8302 5a03  ..G.d.d...d...Z.
 00000050: 4700 6405 6406 8400 6406 8302 5a04 6401  G.d.d...d...Z.d.
 00000060: 5300 2907 e900 0000 004e 2901 da09 7572  S.)......N)...ur
 00000070: 6c65 6e63 6f64 6563 0000 0000 0000 0000  lencodec........
 00000080: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
-00000090: 733a 0000 0065 005a 0164 005a 0264 0c64  s:...e.Z.d.Z.d.d
+00000090: 7342 0000 0065 005a 0164 005a 0264 0e64  sB...e.Z.d.Z.d.d
 000000a0: 0264 0384 015a 0364 0464 0584 005a 0464  .d...Z.d.d...Z.d
-000000b0: 0669 0066 0264 0764 0884 015a 0564 0669  .i.f.d.d...Z.d.i
-000000c0: 0066 0264 0964 0a84 015a 0664 0b53 0029  .f.d.d...Z.d.S.)
-000000d0: 0dda 0a46 696e 616e 6369 616c 7346 6305  ...FinancialsFc.
-000000e0: 0000 0000 0000 0000 0000 0005 0000 0002  ................
-000000f0: 0000 0043 0000 00f3 1c00 0000 7c01 7c00  ...C........|.|.
-00000100: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 7c04  _.|.|._.|.|._.|.
-00000110: 7c00 5f03 6400 5300 a901 4ea9 04da 0c72  |._.d.S...N....r
-00000120: 6174 655f 6c69 6d69 7465 72da 0761 7069  ate_limiter..api
-00000130: 5f6b 6579 da0a 636f 6d70 616e 795f 6964  _key..company_id
-00000140: da0a 7265 7475 726e 5f72 6177 a905 da04  ..return_raw....
-00000150: 7365 6c66 7207 0000 0072 0800 0000 7209  selfr....r....r.
-00000160: 0000 0072 0a00 0000 a900 720d 0000 00fa  ...r......r.....
-00000170: 3962 7569 6c64 2f62 6469 7374 2e6d 6163  9build/bdist.mac
-00000180: 6f73 782d 3130 2e39 2d75 6e69 7665 7273  osx-10.9-univers
-00000190: 616c 322f 6567 672f 6772 6168 616d 2f65  al2/egg/graham/e
-000001a0: 7175 6974 6965 732e 7079 da08 5f5f 696e  quities.py..__in
-000001b0: 6974 5f5f 0500 0000 f308 0000 0006 0106  it__............
-000001c0: 0106 010a 017a 1346 696e 616e 6369 616c  .....z.Financial
-000001d0: 732e 5f5f 696e 6974 5f5f 6301 0000 0000  s.__init__c.....
-000001e0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
-000001f0: 0000 00f3 1400 0000 6401 7c00 6a00 1700  ........d.|.j...
-00000200: 7c00 6a01 6402 6403 9c03 5300 a904 4e7a  |.j.d.d...S...Nz
-00000210: 0742 6561 7265 7220 7a10 6170 706c 6963  .Bearer z.applic
-00000220: 6174 696f 6e2f 6a73 6f6e 2903 da0d 4175  ation/json)...Au
-00000230: 7468 6f72 697a 6174 696f 6e5a 0743 6f6d  thorizationZ.Com
-00000240: 7061 6e79 7a0c 436f 6e74 656e 742d 5479  panyz.Content-Ty
-00000250: 7065 a902 7208 0000 0072 0900 0000 a901  pe..r....r......
-00000260: 720c 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
-00000270: 0e00 0000 da0c 5f67 6574 5f68 6561 6465  ......_get_heade
-00000280: 7273 0b00 0000 f308 0000 0008 0204 0102  rs..............
-00000290: 0106 fd7a 1746 696e 616e 6369 616c 732e  ...z.Financials.
-000002a0: 5f67 6574 5f68 6561 6465 7273 da00 6303  _get_headers..c.
-000002b0: 0000 0000 0000 0000 0000 0006 0000 0008  ................
-000002c0: 0000 0043 0000 00f3 d000 0000 7c00 6a00  ...C........|.j.
-000002d0: 8f56 0100 7401 7c02 8301 7d03 6401 7402  .V..t.|...}.d.t.
-000002e0: 7c01 8301 1700 6402 1700 7d04 7c03 6403  |.....d...}.|.d.
-000002f0: 6b03 721a 7c04 6404 7c03 1700 3700 7d04  k.r.|.d.|...7.}.
-00000300: 7403 6a04 7c04 7c00 a005 a100 6400 6405  t.j.|.|.....d.d.
-00000310: 8d03 7d05 7c05 6a06 6406 6b03 723a 6400  ..}.|.j.d.k.r:d.
-00000320: 7c05 6a06 7c05 6a07 6407 6408 9c03 6602  |.j.|.j.d.d...f.
-00000330: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
-00000340: 7c00 6a08 724a 7c05 a009 a100 6400 6602  |.j.rJ|.....d.f.
-00000350: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
-00000360: 7c05 a009 a100 6409 1900 6400 6602 5700  |.....d...d.f.W.
-00000370: 0200 6400 0400 0400 8303 0100 5300 3100  ..d.........S.1.
-00000380: 735c 7701 0100 0100 0100 5900 0100 6400  s\w.......Y...d.
-00000390: 640a 640b 640c 9c02 6602 5300 290d 4efa  d.d.d...f.S.).N.
-000003a0: 2668 7474 7073 3a2f 2f61 7069 2e77 6974  &https://api.wit
-000003b0: 6867 7261 6861 6d2e 696f 2f76 312f 6571  hgraham.io/v1/eq
-000003c0: 7569 7469 6573 2f7a 0b2f 6669 6e61 6e63  uities/z./financ
-000003d0: 6961 6c73 7218 0000 00fa 013f a902 da07  ialsr......?....
-000003e0: 6865 6164 6572 73da 046a 736f 6ee9 c800  headers..json...
-000003f0: 0000 7a23 6661 696c 6564 2074 6f20 6765  ..z#failed to ge
-00000400: 7420 6669 6e61 6e63 6961 6c73 2066 6f72  t financials for
-00000410: 2065 7175 6974 79a9 03da 0b73 7461 7475   equity....statu
-00000420: 735f 636f 6465 da04 7465 7874 da0d 6572  s_code..text..er
-00000430: 726f 725f 6d65 7373 6167 655a 0a66 696e  ror_messageZ.fin
-00000440: 616e 6369 616c 73e9 ad01 0000 fa13 7261  ancials.......ra
-00000450: 7465 206c 696d 6974 2065 7863 6565 6465  te limit exceede
-00000460: 64a9 0272 2100 0000 7223 0000 00a9 0a72  d..r!...r#.....r
-00000470: 0700 0000 7202 0000 00da 0373 7472 da08  ....r......str..
-00000480: 7265 7175 6573 7473 da03 6765 7472 1600  requests..getr..
-00000490: 0000 7221 0000 0072 2200 0000 720a 0000  ..r!...r"...r...
-000004a0: 0072 1e00 0000 a906 720c 0000 00da 0965  .r......r......e
-000004b0: 7175 6974 795f 6964 da05 7175 6572 79da  quity_id..query.
-000004c0: 0971 7565 7279 5f73 7472 da03 7572 6cda  .query_str..url.
-000004d0: 0172 720d 0000 0072 0d00 0000 720e 0000  .rr....r....r...
-000004e0: 00da 0b4c 6973 7453 756d 6d61 7279 1200  ...ListSummary..
-000004f0: 0000 f32c 0000 0008 0108 0110 0108 010c  ...,............
-00000500: 0114 020a 0102 0104 0104 0102 0106 fd10  ................
-00000510: f806 0e0a 0110 f10e 1020 f002 1102 0102  ......... ......
-00000520: 0108 fe7a 1646 696e 616e 6369 616c 732e  ...z.Financials.
-00000530: 4c69 7374 5375 6d6d 6172 7963 0300 0000  ListSummaryc....
-00000540: 0000 0000 0000 0000 0600 0000 0800 0000  ................
-00000550: 4300 0000 7219 0000 0029 0d4e 721a 0000  C...r....).Nr...
-00000560: 007a 152f 6669 6e61 6e63 6961 6c73 2f73  .z./financials/s
-00000570: 6563 2d66 6f72 6d73 7218 0000 0072 1b00  ec-formsr....r..
-00000580: 0000 721c 0000 0072 1f00 0000 7a22 6661  ..r....r....z"fa
-00000590: 696c 6564 2074 6f20 6765 7420 5345 4320  iled to get SEC 
-000005a0: 666f 726d 7320 666f 7220 6571 7569 7479  forms for equity
-000005b0: 7220 0000 005a 0566 6f72 6d73 7224 0000  r ...Z.formsr$..
-000005c0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
-000005d0: 722b 0000 0072 0d00 0000 720d 0000 0072  r+...r....r....r
-000005e0: 0e00 0000 da0c 4c69 7374 5345 4346 6f72  ......ListSECFor
-000005f0: 6d73 2900 0000 7232 0000 007a 1746 696e  ms)...r2...z.Fin
-00000600: 616e 6369 616c 732e 4c69 7374 5345 4346  ancials.ListSECF
-00000610: 6f72 6d73 4ea9 0146 2907 da08 5f5f 6e61  ormsN..F)...__na
-00000620: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
-00000630: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720f  ..__qualname__r.
-00000640: 0000 0072 1600 0000 7231 0000 0072 3300  ...r....r1...r3.
-00000650: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-00000660: 0072 0e00 0000 7203 0000 0004 0000 0073  .r....r........s
-00000670: 0a00 0000 0800 0a01 0806 0e07 1217 7203  ..............r.
-00000680: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
-00000690: 0000 0000 0300 0000 4000 0000 7362 0000  ........@...sb..
-000006a0: 0065 005a 0164 005a 0264 1264 0264 0384  .e.Z.d.Z.d.d.d..
-000006b0: 015a 0364 0464 0584 005a 0469 0066 0164  .Z.d.d...Z.i.f.d
-000006c0: 0664 0784 015a 0564 0869 0066 0264 0964  .d...Z.d.i.f.d.d
-000006d0: 0a84 015a 0664 0869 0066 0264 0b64 0c84  ...Z.d.i.f.d.d..
-000006e0: 015a 0764 0869 0066 0264 0d64 0e84 015a  .Z.d.i.f.d.d...Z
-000006f0: 0864 0869 0066 0264 0f64 1084 015a 0964  .d.i.f.d.d...Z.d
-00000700: 1153 0029 13da 0845 7175 6974 6965 7346  .S.)...EquitiesF
-00000710: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
-00000720: 0002 0000 0043 0000 0072 0400 0000 7205  .....C...r....r.
-00000730: 0000 0072 0600 0000 720b 0000 0072 0d00  ...r....r....r..
-00000740: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
-00000750: 0042 0000 0072 1000 0000 7a11 4571 7569  .B...r....z.Equi
-00000760: 7469 6573 2e5f 5f69 6e69 745f 5f63 0100  ties.__init__c..
-00000770: 0000 0000 0000 0000 0000 0100 0000 0400  ................
-00000780: 0000 4300 0000 7211 0000 0072 1200 0000  ..C...r....r....
-00000790: 7214 0000 0072 1500 0000 720d 0000 0072  r....r....r....r
-000007a0: 0d00 0000 720e 0000 0072 1600 0000 4800  ....r....r....H.
-000007b0: 0000 7217 0000 007a 1545 7175 6974 6965  ..r....z.Equitie
-000007c0: 732e 5f67 6574 5f68 6561 6465 7273 6302  s._get_headersc.
-000007d0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
-000007e0: 0000 0043 0000 0073 c400 0000 7c00 6a00  ...C...s....|.j.
-000007f0: 8f50 0100 7401 7c01 8301 7d02 6401 7d03  .P..t.|...}.d.}.
-00000800: 7c02 6402 6b03 7214 7c03 6403 7c02 1700  |.d.k.r.|.d.|...
-00000810: 3700 7d03 7402 6a03 7c03 7c00 a004 a100  7.}.t.j.|.|.....
-00000820: 6400 6404 8d03 7d04 7c04 6a05 6405 6b03  d.d...}.|.j.d.k.
-00000830: 7234 6400 7c04 6a05 7c04 6a06 6406 6407  r4d.|.j.|.j.d.d.
-00000840: 9c03 6602 5700 0200 6400 0400 0400 8303  ..f.W...d.......
-00000850: 0100 5300 7c00 6a07 7244 7c04 a008 a100  ..S.|.j.rD|.....
-00000860: 6400 6602 5700 0200 6400 0400 0400 8303  d.f.W...d.......
-00000870: 0100 5300 7c04 a008 a100 6408 1900 6400  ..S.|.....d...d.
-00000880: 6602 5700 0200 6400 0400 0400 8303 0100  f.W...d.........
-00000890: 5300 3100 7356 7701 0100 0100 0100 5900  S.1.sVw.......Y.
-000008a0: 0100 6400 6409 640a 640b 9c02 6602 5300  ..d.d.d.d...f.S.
-000008b0: 290c 4e7a 2568 7474 7073 3a2f 2f61 7069  ).Nz%https://api
-000008c0: 2e77 6974 6867 7261 6861 6d2e 696f 2f76  .withgraham.io/v
-000008d0: 312f 6571 7569 7469 6573 7218 0000 0072  1/equitiesr....r
-000008e0: 1b00 0000 721c 0000 0072 1f00 0000 7a17  ....r....r....z.
-000008f0: 6661 696c 6564 2074 6f20 6c69 7374 2065  failed to list e
-00000900: 7175 6974 6965 7372 2000 0000 5a08 6571  quitiesr ...Z.eq
-00000910: 7569 7469 6573 7224 0000 0072 2500 0000  uitiesr$...r%...
-00000920: 7226 0000 0029 0972 0700 0000 7202 0000  r&...).r....r...
-00000930: 0072 2900 0000 722a 0000 0072 1600 0000  .r)...r*...r....
-00000940: 7221 0000 0072 2200 0000 720a 0000 0072  r!...r"...r....r
-00000950: 1e00 0000 2905 720c 0000 0072 2d00 0000  ....).r....r-...
-00000960: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
-00000970: 0d00 0000 720d 0000 0072 0e00 0000 da04  ....r....r......
-00000980: 4c69 7374 4f00 0000 732c 0000 0008 0108  ListO...s,......
-00000990: 0104 0108 010c 0114 020a 0102 0104 0104  ................
-000009a0: 0102 0106 fd10 f806 0e0a 0110 f10e 1020  ............... 
-000009b0: f002 1102 0102 0108 fe7a 0d45 7175 6974  .........z.Equit
-000009c0: 6965 732e 4c69 7374 7218 0000 0063 0300  ies.Listr....c..
-000009d0: 0000 0000 0000 0000 0000 0600 0000 0800  ................
-000009e0: 0000 4300 0000 73cc 0000 007c 006a 008f  ..C...s....|.j..
-000009f0: 5401 0074 017c 0283 017d 0364 0174 027c  T..t.|...}.d.t.|
-00000a00: 0183 0117 007d 047c 0364 026b 0372 187c  .....}.|.d.k.r.|
-00000a10: 0464 037c 0317 0037 007d 0474 036a 047c  .d.|...7.}.t.j.|
-00000a20: 047c 00a0 05a1 0064 0064 048d 037d 057c  .|.....d.d...}.|
-00000a30: 056a 0664 056b 0372 3864 007c 056a 067c  .j.d.k.r8d.|.j.|
-00000a40: 056a 0764 0664 079c 0366 0257 0002 0064  .j.d.d...f.W...d
-00000a50: 0004 0004 0083 0301 0053 007c 006a 0872  .........S.|.j.r
-00000a60: 487c 05a0 09a1 0064 0066 0257 0002 0064  H|.....d.f.W...d
-00000a70: 0004 0004 0083 0301 0053 007c 05a0 09a1  .........S.|....
-00000a80: 0064 0819 0064 0066 0257 0002 0064 0004  .d...d.f.W...d..
-00000a90: 0004 0083 0301 0053 0031 0073 5a77 0101  .......S.1.sZw..
-00000aa0: 0001 0001 0059 0001 0064 0064 0964 0a64  .....Y...d.d.d.d
-00000ab0: 0b9c 0266 0253 0029 0c4e 721a 0000 0072  ...f.S.).Nr....r
-00000ac0: 1800 0000 721b 0000 0072 1c00 0000 721f  ....r....r....r.
-00000ad0: 0000 00fa 1466 6169 6c65 6420 746f 2067  .....failed to g
-00000ae0: 6574 2065 7175 6974 7972 2000 0000 5a06  et equityr ...Z.
-00000af0: 6571 7569 7479 7224 0000 0072 2500 0000  equityr$...r%...
-00000b00: 7226 0000 0072 2700 0000 722b 0000 0072  r&...r'...r+...r
-00000b10: 0d00 0000 720d 0000 0072 0e00 0000 da03  ....r....r......
-00000b20: 4765 7466 0000 0073 2c00 0000 0801 0801  Getf...s,.......
-00000b30: 0c01 0801 0c01 1402 0a01 0201 0401 0401  ................
-00000b40: 0201 06fd 10f8 060e 0a01 10f1 0e10 20f0  .............. .
-00000b50: 0211 0201 0201 08fe 7a0c 4571 7569 7469  ........z.Equiti
-00000b60: 6573 2e47 6574 6303 0000 0000 0000 0000  es.Getc.........
-00000b70: 0000 0006 0000 0008 0000 0043 0000 0072  ...........C...r
-00000b80: 1900 0000 290d 4e72 1a00 0000 7a06 2f64  ....).Nr....z./d
-00000b90: 6169 6c79 7218 0000 0072 1b00 0000 721c  ailyr....r....r.
-00000ba0: 0000 0072 1f00 0000 7a27 6661 696c 6564  ...r....z'failed
-00000bb0: 2074 6f20 6765 7420 6461 696c 7920 736e   to get daily sn
-00000bc0: 6170 7368 6f74 2066 6f72 2065 7175 6974  apshot for equit
-00000bd0: 7972 2000 0000 5a0e 6461 696c 7953 6e61  yr ...Z.dailySna
-00000be0: 7073 686f 7473 7224 0000 0072 2500 0000  pshotsr$...r%...
-00000bf0: 7226 0000 0072 2700 0000 722b 0000 0072  r&...r'...r+...r
-00000c00: 0d00 0000 720d 0000 0072 0e00 0000 da05  ....r....r......
-00000c10: 4461 696c 797d 0000 0072 3200 0000 7a0e  Daily}...r2...z.
-00000c20: 4571 7569 7469 6573 2e44 6169 6c79 6303  Equities.Dailyc.
-00000c30: 0000 0000 0000 0000 0000 0003 0000 0005  ................
-00000c40: 0000 0043 0000 0073 1600 0000 7400 7c00  ...C...s....t.|.
-00000c50: 6a01 7c00 6a02 7c00 6a03 7c00 6a04 8304  j.|.j.|.j.|.j...
-00000c60: 5300 7205 0000 0029 0572 0300 0000 7207  S.r....).r....r.
-00000c70: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
-00000c80: 0000 2903 720c 0000 0072 2c00 0000 722d  ..).r....r,...r-
-00000c90: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
-00000ca0: 0000 7203 0000 0094 0000 0073 0200 0000  ..r........s....
-00000cb0: 1601 7a13 4571 7569 7469 6573 2e46 696e  ..z.Equities.Fin
-00000cc0: 616e 6369 616c 7363 0300 0000 0000 0000  ancialsc........
-00000cd0: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
-00000ce0: 7219 0000 0029 0d4e 721a 0000 007a 0a2f  r....).Nr....z./
-00000cf0: 6469 7669 6465 6e64 7372 1800 0000 721b  dividendsr....r.
-00000d00: 0000 0072 1c00 0000 721f 0000 0072 3a00  ...r....r....r:.
-00000d10: 0000 7220 0000 005a 0964 6976 6964 656e  ..r ...Z.dividen
-00000d20: 6473 7224 0000 0072 2500 0000 7226 0000  dsr$...r%...r&..
-00000d30: 0072 2700 0000 722b 0000 0072 0d00 0000  .r'...r+...r....
-00000d40: 720d 0000 0072 0e00 0000 da09 4469 7669  r....r......Divi
-00000d50: 6465 6e64 7397 0000 0072 3200 0000 7a12  dends....r2...z.
-00000d60: 4571 7569 7469 6573 2e44 6976 6964 656e  Equities.Dividen
-00000d70: 6473 4e72 3400 0000 290a 7235 0000 0072  dsNr4...).r5...r
-00000d80: 3600 0000 7237 0000 0072 0f00 0000 7216  6...r7...r....r.
-00000d90: 0000 0072 3900 0000 723b 0000 0072 3c00  ...r9...r;...r<.
-00000da0: 0000 7203 0000 0072 3d00 0000 720d 0000  ..r....r=...r...
-00000db0: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
-00000dc0: 7238 0000 0041 0000 0073 1000 0000 0800  r8...A...s......
-00000dd0: 0a01 0806 0c07 0e17 0e17 0e17 1203 7238  ..............r8
-00000de0: 0000 0029 0572 2900 0000 da0c 7572 6c6c  ...).r).....urll
-00000df0: 6962 2e70 6172 7365 7202 0000 0072 0300  ib.parser....r..
-00000e00: 0000 7238 0000 0072 0d00 0000 720d 0000  ..r8...r....r...
-00000e10: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
-00000e20: 6475 6c65 3e01 0000 0073 0800 0000 0800  dule>....s......
-00000e30: 0c01 0e02 123d                           .....=
+000000b0: 0664 0784 005a 0564 0869 0066 0264 0964  .d...Z.d.i.f.d.d
+000000c0: 0a84 015a 0664 0869 0066 0264 0b64 0c84  ...Z.d.i.f.d.d..
+000000d0: 015a 0764 0d53 0029 0fda 0a46 696e 616e  .Z.d.S.)...Finan
+000000e0: 6369 616c 7346 6305 0000 0000 0000 0000  cialsFc.........
+000000f0: 0000 0005 0000 0002 0000 0043 0000 00f3  ...........C....
+00000100: 2200 0000 7c01 7c00 5f00 7c02 7c00 5f01  "...|.|._.|.|._.
+00000110: 7c03 7c00 5f02 7c04 7c00 5f03 6401 7c00  |.|._.|.|._.d.|.
+00000120: 5f04 6400 5300 a902 4ee9 0f00 0000 a905  _.d.S...N.......
+00000130: da0c 7261 7465 5f6c 696d 6974 6572 da07  ..rate_limiter..
+00000140: 6170 695f 6b65 79da 0a63 6f6d 7061 6e79  api_key..company
+00000150: 5f69 64da 0a72 6574 7572 6e5f 7261 77da  _id..return_raw.
+00000160: 0774 696d 656f 7574 a905 da04 7365 6c66  .timeout....self
+00000170: 7208 0000 0072 0900 0000 720a 0000 0072  r....r....r....r
+00000180: 0b00 0000 a900 720f 0000 00fa 3962 7569  ......r.....9bui
+00000190: 6c64 2f62 6469 7374 2e6d 6163 6f73 782d  ld/bdist.macosx-
+000001a0: 3130 2e39 2d75 6e69 7665 7273 616c 322f  10.9-universal2/
+000001b0: 6567 672f 6772 6168 616d 2f65 7175 6974  egg/graham/equit
+000001c0: 6965 732e 7079 da08 5f5f 696e 6974 5f5f  ies.py..__init__
+000001d0: 0500 0000 f30a 0000 0006 0106 0106 0106  ................
+000001e0: 010a 017a 1346 696e 616e 6369 616c 732e  ...z.Financials.
+000001f0: 5f5f 696e 6974 5f5f 6301 0000 0000 0000  __init__c.......
+00000200: 0000 0000 0001 0000 0001 0000 0043 0000  .............C..
+00000210: 00f3 0600 0000 7c00 6a00 5300 a901 4ea9  ......|.j.S...N.
+00000220: 0172 0c00 0000 a901 720e 0000 0072 0f00  .r......r....r..
+00000230: 0000 720f 0000 0072 1000 0000 da0c 5f67  ..r....r......_g
+00000240: 6574 5f74 696d 656f 7574 0c00 0000 f302  et_timeout......
+00000250: 0000 0006 017a 1746 696e 616e 6369 616c  .....z.Financial
+00000260: 732e 5f67 6574 5f74 696d 656f 7574 6301  s._get_timeoutc.
+00000270: 0000 0000 0000 0000 0000 0001 0000 0004  ................
+00000280: 0000 0043 0000 00f3 1400 0000 6401 7c00  ...C........d.|.
+00000290: 6a00 1700 7c00 6a01 6402 6403 9c03 5300  j...|.j.d.d...S.
+000002a0: a904 4e7a 0742 6561 7265 7220 7a10 6170  ..Nz.Bearer z.ap
+000002b0: 706c 6963 6174 696f 6e2f 6a73 6f6e 2903  plication/json).
+000002c0: da0d 4175 7468 6f72 697a 6174 696f 6e5a  ..AuthorizationZ
+000002d0: 0743 6f6d 7061 6e79 7a0c 436f 6e74 656e  .Companyz.Conten
+000002e0: 742d 5479 7065 a902 7209 0000 0072 0a00  t-Type..r....r..
+000002f0: 0000 7216 0000 0072 0f00 0000 720f 0000  ..r....r....r...
+00000300: 0072 1000 0000 da0c 5f67 6574 5f68 6561  .r......_get_hea
+00000310: 6465 7273 0f00 0000 f308 0000 0008 0204  ders............
+00000320: 0102 0106 fd7a 1746 696e 616e 6369 616c  .....z.Financial
+00000330: 732e 5f67 6574 5f68 6561 6465 7273 da00  s._get_headers..
+00000340: 6303 0000 0000 0000 0000 0000 0006 0000  c...............
+00000350: 0008 0000 0043 0000 00f3 d600 0000 7c00  .....C........|.
+00000360: 6a00 8f59 0100 7401 7c02 8301 7d03 6401  j..Y..t.|...}.d.
+00000370: 7402 7c01 8301 1700 6402 1700 7d04 7c03  t.|.....d...}.|.
+00000380: 6403 6b03 721a 7c04 6404 7c03 1700 3700  d.k.r.|.d.|...7.
+00000390: 7d04 7403 6a04 7c04 7c00 a005 a100 6400  }.t.j.|.|.....d.
+000003a0: 7c00 a006 a100 6405 8d04 7d05 7c05 6a07  |.....d...}.|.j.
+000003b0: 6406 6b03 723d 6400 7c05 6a07 7c05 6a08  d.k.r=d.|.j.|.j.
+000003c0: 6407 6408 9c03 6602 5700 0200 6400 0400  d.d...f.W...d...
+000003d0: 0400 8303 0100 5300 7c00 6a09 724d 7c05  ......S.|.j.rM|.
+000003e0: a00a a100 6400 6602 5700 0200 6400 0400  ....d.f.W...d...
+000003f0: 0400 8303 0100 5300 7c05 a00a a100 6409  ......S.|.....d.
+00000400: 1900 6400 6602 5700 0200 6400 0400 0400  ..d.f.W...d.....
+00000410: 8303 0100 5300 3100 735f 7701 0100 0100  ....S.1.s_w.....
+00000420: 0100 5900 0100 6400 640a 640b 640c 9c02  ..Y...d.d.d.d...
+00000430: 6602 5300 290d 4efa 2668 7474 7073 3a2f  f.S.).N.&https:/
+00000440: 2f61 7069 2e77 6974 6867 7261 6861 6d2e  /api.withgraham.
+00000450: 696f 2f76 312f 6571 7569 7469 6573 2f7a  io/v1/equities/z
+00000460: 0b2f 6669 6e61 6e63 6961 6c73 721f 0000  ./financialsr...
+00000470: 00fa 013f a903 da07 6865 6164 6572 73da  ...?....headers.
+00000480: 046a 736f 6e72 0c00 0000 e9c8 0000 007a  .jsonr.........z
+00000490: 2366 6169 6c65 6420 746f 2067 6574 2066  #failed to get f
+000004a0: 696e 616e 6369 616c 7320 666f 7220 6571  inancials for eq
+000004b0: 7569 7479 a903 da0b 7374 6174 7573 5f63  uity....status_c
+000004c0: 6f64 65da 0474 6578 74da 0d65 7272 6f72  ode..text..error
+000004d0: 5f6d 6573 7361 6765 5a0a 6669 6e61 6e63  _messageZ.financ
+000004e0: 6961 6c73 e9ad 0100 00fa 1372 6174 6520  ials.......rate 
+000004f0: 6c69 6d69 7420 6578 6365 6564 6564 a902  limit exceeded..
+00000500: 7228 0000 0072 2a00 0000 a90b 7208 0000  r(...r*.....r...
+00000510: 0072 0200 0000 da03 7374 72da 0872 6571  .r......str..req
+00000520: 7565 7374 73da 0367 6574 721d 0000 0072  uests..getr....r
+00000530: 1700 0000 7228 0000 0072 2900 0000 720b  ....r(...r)...r.
+00000540: 0000 0072 2500 0000 a906 720e 0000 00da  ...r%.....r.....
+00000550: 0965 7175 6974 795f 6964 da05 7175 6572  .equity_id..quer
+00000560: 79da 0971 7565 7279 5f73 7472 da03 7572  y..query_str..ur
+00000570: 6cda 0172 720f 0000 0072 0f00 0000 7210  l..rr....r....r.
+00000580: 0000 00da 0b4c 6973 7453 756d 6d61 7279  .....ListSummary
+00000590: 1600 0000 f32c 0000 0008 0108 0110 0108  .....,..........
+000005a0: 010c 011a 020a 0102 0104 0104 0102 0106  ................
+000005b0: fd10 f806 0e0a 0110 f10e 1020 f002 1102  ........... ....
+000005c0: 0102 0108 fe7a 1646 696e 616e 6369 616c  .....z.Financial
+000005d0: 732e 4c69 7374 5375 6d6d 6172 7963 0300  s.ListSummaryc..
+000005e0: 0000 0000 0000 0000 0000 0600 0000 0800  ................
+000005f0: 0000 4300 0000 7220 0000 0029 0d4e 7221  ..C...r ...).Nr!
+00000600: 0000 007a 152f 6669 6e61 6e63 6961 6c73  ...z./financials
+00000610: 2f73 6563 2d66 6f72 6d73 721f 0000 0072  /sec-formsr....r
+00000620: 2200 0000 7223 0000 0072 2600 0000 7a22  "...r#...r&...z"
+00000630: 6661 696c 6564 2074 6f20 6765 7420 5345  failed to get SE
+00000640: 4320 666f 726d 7320 666f 7220 6571 7569  C forms for equi
+00000650: 7479 7227 0000 005a 0566 6f72 6d73 722b  tyr'...Z.formsr+
+00000660: 0000 0072 2c00 0000 722d 0000 0072 2e00  ...r,...r-...r..
+00000670: 0000 7232 0000 0072 0f00 0000 720f 0000  ..r2...r....r...
+00000680: 0072 1000 0000 da0c 4c69 7374 5345 4346  .r......ListSECF
+00000690: 6f72 6d73 2d00 0000 7239 0000 007a 1746  orms-...r9...z.F
+000006a0: 696e 616e 6369 616c 732e 4c69 7374 5345  inancials.ListSE
+000006b0: 4346 6f72 6d73 4ea9 0146 2908 da08 5f5f  CFormsN..F)...__
+000006c0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000006d0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+000006e0: 7211 0000 0072 1700 0000 721d 0000 0072  r....r....r....r
+000006f0: 3800 0000 723a 0000 0072 0f00 0000 720f  8...r:...r....r.
+00000700: 0000 0072 0f00 0000 7210 0000 0072 0300  ...r....r....r..
+00000710: 0000 0400 0000 730c 0000 0008 000a 0108  ......s.........
+00000720: 0708 030e 0712 1772 0300 0000 6300 0000  .......r....c...
+00000730: 0000 0000 0000 0000 0000 0000 0003 0000  ................
+00000740: 0040 0000 0073 6a00 0000 6500 5a01 6400  .@...sj...e.Z.d.
+00000750: 5a02 6414 6402 6403 8401 5a03 6404 6405  Z.d.d.d...Z.d.d.
+00000760: 8400 5a04 6406 6407 8400 5a05 6900 6601  ..Z.d.d...Z.i.f.
+00000770: 6408 6409 8401 5a06 640a 6900 6602 640b  d.d...Z.d.i.f.d.
+00000780: 640c 8401 5a07 640a 6900 6602 640d 640e  d...Z.d.i.f.d.d.
+00000790: 8401 5a08 640a 6900 6602 640f 6410 8401  ..Z.d.i.f.d.d...
+000007a0: 5a09 640a 6900 6602 6411 6412 8401 5a0a  Z.d.i.f.d.d...Z.
+000007b0: 6413 5300 2915 da08 4571 7569 7469 6573  d.S.)...Equities
+000007c0: 4663 0500 0000 0000 0000 0000 0000 0500  Fc..............
+000007d0: 0000 0200 0000 4300 0000 7204 0000 0072  ......C...r....r
+000007e0: 0500 0000 7207 0000 0072 0d00 0000 720f  ....r....r....r.
+000007f0: 0000 0072 0f00 0000 7210 0000 0072 1100  ...r....r....r..
+00000800: 0000 4600 0000 7212 0000 007a 1145 7175  ..F...r....z.Equ
+00000810: 6974 6965 732e 5f5f 696e 6974 5f5f 6301  ities.__init__c.
+00000820: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000830: 0000 0043 0000 0072 1300 0000 7214 0000  ...C...r....r...
+00000840: 0072 1500 0000 7216 0000 0072 0f00 0000  .r....r....r....
+00000850: 720f 0000 0072 1000 0000 7217 0000 004d  r....r....r....M
+00000860: 0000 0072 1800 0000 7a15 4571 7569 7469  ...r....z.Equiti
+00000870: 6573 2e5f 6765 745f 7469 6d65 6f75 7463  es._get_timeoutc
+00000880: 0100 0000 0000 0000 0000 0000 0100 0000  ................
+00000890: 0400 0000 4300 0000 7219 0000 0072 1a00  ....C...r....r..
+000008a0: 0000 721c 0000 0072 1600 0000 720f 0000  ..r....r....r...
+000008b0: 0072 0f00 0000 7210 0000 0072 1d00 0000  .r....r....r....
+000008c0: 5000 0000 721e 0000 007a 1545 7175 6974  P...r....z.Equit
+000008d0: 6965 732e 5f67 6574 5f68 6561 6465 7273  ies._get_headers
+000008e0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
+000008f0: 0008 0000 0043 0000 0073 ca00 0000 7c00  .....C...s....|.
+00000900: 6a00 8f53 0100 7401 7c01 8301 7d02 6401  j..S..t.|...}.d.
+00000910: 7d03 7c02 6402 6b03 7214 7c03 6403 7c02  }.|.d.k.r.|.d.|.
+00000920: 1700 3700 7d03 7402 6a03 7c03 7c00 a004  ..7.}.t.j.|.|...
+00000930: a100 6400 7c00 a005 a100 6404 8d04 7d04  ..d.|.....d...}.
+00000940: 7c04 6a06 6405 6b03 7237 6400 7c04 6a06  |.j.d.k.r7d.|.j.
+00000950: 7c04 6a07 6406 6407 9c03 6602 5700 0200  |.j.d.d...f.W...
+00000960: 6400 0400 0400 8303 0100 5300 7c00 6a08  d.........S.|.j.
+00000970: 7247 7c04 a009 a100 6400 6602 5700 0200  rG|.....d.f.W...
+00000980: 6400 0400 0400 8303 0100 5300 7c04 a009  d.........S.|...
+00000990: a100 6408 1900 6400 6602 5700 0200 6400  ..d...d.f.W...d.
+000009a0: 0400 0400 8303 0100 5300 3100 7359 7701  ........S.1.sYw.
+000009b0: 0100 0100 0100 5900 0100 6400 6409 640a  ......Y...d.d.d.
+000009c0: 640b 9c02 6602 5300 290c 4e7a 2568 7474  d...f.S.).Nz%htt
+000009d0: 7073 3a2f 2f61 7069 2e77 6974 6867 7261  ps://api.withgra
+000009e0: 6861 6d2e 696f 2f76 312f 6571 7569 7469  ham.io/v1/equiti
+000009f0: 6573 721f 0000 0072 2200 0000 7223 0000  esr....r"...r#..
+00000a00: 0072 2600 0000 7a17 6661 696c 6564 2074  .r&...z.failed t
+00000a10: 6f20 6c69 7374 2065 7175 6974 6965 7372  o list equitiesr
+00000a20: 2700 0000 5a08 6571 7569 7469 6573 722b  '...Z.equitiesr+
+00000a30: 0000 0072 2c00 0000 722d 0000 0029 0a72  ...r,...r-...).r
+00000a40: 0800 0000 7202 0000 0072 3000 0000 7231  ....r....r0...r1
+00000a50: 0000 0072 1d00 0000 7217 0000 0072 2800  ...r....r....r(.
+00000a60: 0000 7229 0000 0072 0b00 0000 7225 0000  ..r)...r....r%..
+00000a70: 0029 0572 0e00 0000 7234 0000 0072 3500  .).r....r4...r5.
+00000a80: 0000 7236 0000 0072 3700 0000 720f 0000  ..r6...r7...r...
+00000a90: 0072 0f00 0000 7210 0000 00da 044c 6973  .r....r......Lis
+00000aa0: 7457 0000 0073 2c00 0000 0801 0801 0401  tW...s,.........
+00000ab0: 0801 0c01 1a02 0a01 0201 0401 0401 0201  ................
+00000ac0: 06fd 10f8 060e 0a01 10f1 0e10 20f0 0211  ............ ...
+00000ad0: 0201 0201 08fe 7a0d 4571 7569 7469 6573  ......z.Equities
+00000ae0: 2e4c 6973 7472 1f00 0000 6303 0000 0000  .Listr....c.....
+00000af0: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00000b00: 0000 0073 d200 0000 7c00 6a00 8f57 0100  ...s....|.j..W..
+00000b10: 7401 7c02 8301 7d03 6401 7402 7c01 8301  t.|...}.d.t.|...
+00000b20: 1700 7d04 7c03 6402 6b03 7218 7c04 6403  ..}.|.d.k.r.|.d.
+00000b30: 7c03 1700 3700 7d04 7403 6a04 7c04 7c00  |...7.}.t.j.|.|.
+00000b40: a005 a100 6400 7c00 a006 a100 6404 8d04  ....d.|.....d...
+00000b50: 7d05 7c05 6a07 6405 6b03 723b 6400 7c05  }.|.j.d.k.r;d.|.
+00000b60: 6a07 7c05 6a08 6406 6407 9c03 6602 5700  j.|.j.d.d...f.W.
+00000b70: 0200 6400 0400 0400 8303 0100 5300 7c00  ..d.........S.|.
+00000b80: 6a09 724b 7c05 a00a a100 6400 6602 5700  j.rK|.....d.f.W.
+00000b90: 0200 6400 0400 0400 8303 0100 5300 7c05  ..d.........S.|.
+00000ba0: a00a a100 6408 1900 6400 6602 5700 0200  ....d...d.f.W...
+00000bb0: 6400 0400 0400 8303 0100 5300 3100 735d  d.........S.1.s]
+00000bc0: 7701 0100 0100 0100 5900 0100 6400 6409  w.......Y...d.d.
+00000bd0: 640a 640b 9c02 6602 5300 290c 4e72 2100  d.d...f.S.).Nr!.
+00000be0: 0000 721f 0000 0072 2200 0000 7223 0000  ..r....r"...r#..
+00000bf0: 0072 2600 0000 fa14 6661 696c 6564 2074  .r&.....failed t
+00000c00: 6f20 6765 7420 6571 7569 7479 7227 0000  o get equityr'..
+00000c10: 005a 0665 7175 6974 7972 2b00 0000 722c  .Z.equityr+...r,
+00000c20: 0000 0072 2d00 0000 722e 0000 0072 3200  ...r-...r....r2.
+00000c30: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000c40: 00da 0347 6574 6e00 0000 732c 0000 0008  ...Getn...s,....
+00000c50: 0108 010c 0108 010c 011a 020a 0102 0104  ................
+00000c60: 0104 0102 0106 fd10 f806 0e0a 0110 f10e  ................
+00000c70: 1020 f002 1102 0102 0108 fe7a 0c45 7175  . .........z.Equ
+00000c80: 6974 6965 732e 4765 7463 0300 0000 0000  ities.Getc......
+00000c90: 0000 0000 0000 0600 0000 0800 0000 4300  ..............C.
+00000ca0: 0000 7220 0000 0029 0d4e 7221 0000 007a  ..r ...).Nr!...z
+00000cb0: 062f 6461 696c 7972 1f00 0000 7222 0000  ./dailyr....r"..
+00000cc0: 0072 2300 0000 7226 0000 007a 2766 6169  .r#...r&...z'fai
+00000cd0: 6c65 6420 746f 2067 6574 2064 6169 6c79  led to get daily
+00000ce0: 2073 6e61 7073 686f 7420 666f 7220 6571   snapshot for eq
+00000cf0: 7569 7479 7227 0000 005a 0e64 6169 6c79  uityr'...Z.daily
+00000d00: 536e 6170 7368 6f74 7372 2b00 0000 722c  Snapshotsr+...r,
+00000d10: 0000 0072 2d00 0000 722e 0000 0072 3200  ...r-...r....r2.
+00000d20: 0000 720f 0000 0072 0f00 0000 7210 0000  ..r....r....r...
+00000d30: 00da 0544 6169 6c79 8500 0000 7239 0000  ...Daily....r9..
+00000d40: 007a 0e45 7175 6974 6965 732e 4461 696c  .z.Equities.Dail
+00000d50: 7963 0300 0000 0000 0000 0000 0000 0300  yc..............
+00000d60: 0000 0500 0000 4300 0000 7316 0000 0074  ......C...s....t
+00000d70: 007c 006a 017c 006a 027c 006a 037c 006a  .|.j.|.j.|.j.|.j
+00000d80: 0483 0453 0072 1400 0000 2905 7203 0000  ...S.r....).r...
+00000d90: 0072 0800 0000 7209 0000 0072 0a00 0000  .r....r....r....
+00000da0: 720b 0000 0029 0372 0e00 0000 7233 0000  r....).r....r3..
+00000db0: 0072 3400 0000 720f 0000 0072 0f00 0000  .r4...r....r....
+00000dc0: 7210 0000 0072 0300 0000 9c00 0000 7302  r....r........s.
+00000dd0: 0000 0016 017a 1345 7175 6974 6965 732e  .....z.Equities.
+00000de0: 4669 6e61 6e63 6961 6c73 6303 0000 0000  Financialsc.....
+00000df0: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+00000e00: 0000 0072 2000 0000 290d 4e72 2100 0000  ...r ...).Nr!...
+00000e10: 7a0a 2f64 6976 6964 656e 6473 721f 0000  z./dividendsr...
+00000e20: 0072 2200 0000 7223 0000 0072 2600 0000  .r"...r#...r&...
+00000e30: 7241 0000 0072 2700 0000 5a09 6469 7669  rA...r'...Z.divi
+00000e40: 6465 6e64 7372 2b00 0000 722c 0000 0072  dendsr+...r,...r
+00000e50: 2d00 0000 722e 0000 0072 3200 0000 720f  -...r....r2...r.
+00000e60: 0000 0072 0f00 0000 7210 0000 00da 0944  ...r....r......D
+00000e70: 6976 6964 656e 6473 9f00 0000 7239 0000  ividends....r9..
+00000e80: 007a 1245 7175 6974 6965 732e 4469 7669  .z.Equities.Divi
+00000e90: 6465 6e64 734e 723b 0000 0029 0b72 3c00  dendsNr;...).r<.
+00000ea0: 0000 723d 0000 0072 3e00 0000 7211 0000  ..r=...r>...r...
+00000eb0: 0072 1700 0000 721d 0000 0072 4000 0000  .r....r....r@...
+00000ec0: 7242 0000 0072 4300 0000 7203 0000 0072  rB...rC...r....r
+00000ed0: 4400 0000 720f 0000 0072 0f00 0000 720f  D...r....r....r.
+00000ee0: 0000 0072 1000 0000 723f 0000 0045 0000  ...r....r?...E..
+00000ef0: 0073 1200 0000 0800 0a01 0807 0803 0c07  .s..............
+00000f00: 0e17 0e17 0e17 1203 723f 0000 0029 0572  ........r?...).r
+00000f10: 3000 0000 da0c 7572 6c6c 6962 2e70 6172  0.....urllib.par
+00000f20: 7365 7202 0000 0072 0300 0000 723f 0000  ser....r....r?..
+00000f30: 0072 0f00 0000 720f 0000 0072 0f00 0000  .r....r....r....
+00000f40: 7210 0000 00da 083c 6d6f 6475 6c65 3e01  r......<module>.
+00000f50: 0000 0073 0800 0000 0800 0c01 0e02 1241  ...s...........A
```

## graham/__pycache__/tables.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 11:18:06 2023 UTC, .py size: 4364 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,184 +1,196 @@
-00000000: 6f0d 0d0a 0000 0000 6e95 7064 0c11 0000  o.......n.pd....
+00000000: 6f0d 0d0a 0000 0000 32c1 7064 f411 0000  o.......2.pd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a01 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-00000060: 0003 0000 0040 0000 0073 5a00 0000 6500  .....@...sZ...e.
+00000060: 0003 0000 0040 0000 0073 6200 0000 6500  .....@...sb...e.
 00000070: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
-00000080: 6404 8400 5a04 6900 6405 6405 6603 6406  d...Z.i.d.d.f.d.
-00000090: 6407 8401 5a05 6900 6601 6408 6409 8401  d...Z.i.f.d.d...
-000000a0: 5a06 6900 6601 640a 640b 8401 5a07 640c  Z.i.f.d.d...Z.d.
-000000b0: 640d 8400 5a08 6900 6900 6602 640e 640f  d...Z.i.i.f.d.d.
-000000c0: 8401 5a09 6405 5300 2910 da06 5461 626c  ..Z.d.S.)...Tabl
-000000d0: 6573 6305 0000 0000 0000 0000 0000 0005  esc.............
-000000e0: 0000 0004 0000 0043 0000 0073 3a00 0000  .......C...s:...
-000000f0: 7c04 6400 6b02 7308 7c04 6401 6b02 720f  |.d.k.s.|.d.k.r.
-00000100: 6400 6402 6403 6404 9c02 6602 5300 7c01  d.d.d.d...f.S.|.
-00000110: 7c00 5f00 7c04 7c00 5f01 7c02 7c00 5f02  |._.|.|._.|.|._.
-00000120: 7c03 7c00 5f03 6400 5300 2905 4eda 0069  |.|._.d.S.).N..i
-00000130: 9001 0000 7a14 5461 626c 6520 4944 2069  ....z.Table ID i
-00000140: 7320 7265 7175 6972 6564 a902 da0b 7374  s required....st
-00000150: 6174 7573 5f63 6f64 65da 0d65 7272 6f72  atus_code..error
-00000160: 5f6d 6573 7361 6765 2904 da0c 7261 7465  _message)...rate
-00000170: 5f6c 696d 6974 6572 da08 7461 626c 655f  _limiter..table_
-00000180: 6964 da07 6170 695f 6b65 79da 0a63 6f6d  id..api_key..com
-00000190: 7061 6e79 5f69 6429 05da 0473 656c 6672  pany_id)...selfr
-000001a0: 0700 0000 7209 0000 0072 0a00 0000 7208  ....r....r....r.
-000001b0: 0000 00a9 0072 0c00 0000 fa37 6275 696c  .....r.....7buil
-000001c0: 642f 6264 6973 742e 6d61 636f 7378 2d31  d/bdist.macosx-1
-000001d0: 302e 392d 756e 6976 6572 7361 6c32 2f65  0.9-universal2/e
-000001e0: 6767 2f67 7261 6861 6d2f 7461 626c 6573  gg/graham/tables
-000001f0: 2e70 79da 085f 5f69 6e69 745f 5f04 0000  .py..__init__...
-00000200: 0073 1200 0000 1001 0201 0201 0201 08fe  .s..............
-00000210: 0604 0601 0601 0a01 7a0f 5461 626c 6573  ........z.Tables
-00000220: 2e5f 5f69 6e69 745f 5f63 0100 0000 0000  .__init__c......
-00000230: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
-00000240: 0000 7314 0000 0064 017c 006a 0017 007c  ..s....d.|.j...|
-00000250: 006a 0164 0264 039c 0353 0029 044e 7a07  .j.d.d...S.).Nz.
-00000260: 4265 6172 6572 207a 1061 7070 6c69 6361  Bearer z.applica
-00000270: 7469 6f6e 2f6a 736f 6e29 03da 0d41 7574  tion/json)...Aut
-00000280: 686f 7269 7a61 7469 6f6e 5a07 436f 6d70  horizationZ.Comp
-00000290: 616e 797a 0c43 6f6e 7465 6e74 2d54 7970  anyz.Content-Typ
-000002a0: 6529 0272 0900 0000 720a 0000 0029 0172  e).r....r....).r
-000002b0: 0b00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-000002c0: 0000 00da 0c5f 6765 745f 6865 6164 6572  ....._get_header
-000002d0: 730f 0000 0073 0800 0000 0802 0401 0201  s....s..........
-000002e0: 06fd 7a13 5461 626c 6573 2e5f 6765 745f  ..z.Tables._get_
-000002f0: 6865 6164 6572 734e 6304 0000 0000 0000  headersNc.......
-00000300: 0000 0000 0007 0000 0008 0000 0043 0000  .............C..
-00000310: 0073 be00 0000 7c00 6a00 8f4d 0100 6401  .s....|.j..M..d.
-00000320: 7401 7c00 6a02 8301 1700 6402 1700 7d04  t.|.j.....d...}.
-00000330: 6403 7c01 6901 7d05 7c02 6400 6b03 7219  d.|.i.}.|.d.k.r.
-00000340: 7c02 7c05 6404 3c00 7c03 6400 6b03 7221  |.|.d.<.|.d.k.r!
-00000350: 7c03 7c05 6405 3c00 7403 6a04 7c04 7c00  |.|.d.<.t.j.|.|.
-00000360: a005 a100 7c05 6406 8d03 7d06 7c06 6a06  ....|.d...}.|.j.
-00000370: 6407 6b03 7241 6400 7c06 6a06 7c06 6a07  d.k.rAd.|.j.|.j.
-00000380: 6408 6409 9c03 6602 5700 0200 6400 0400  d.d...f.W...d...
-00000390: 0400 8303 0100 5300 7c06 a008 a100 640a  ......S.|.....d.
-000003a0: 1900 6400 6602 5700 0200 6400 0400 0400  ..d.f.W...d.....
-000003b0: 8303 0100 5300 3100 7353 7701 0100 0100  ....S.1.sSw.....
-000003c0: 0100 5900 0100 6400 640b 640c 640d 9c02  ..Y...d.d.d.d...
-000003d0: 6602 5300 290e 4efa 2468 7474 7073 3a2f  f.S.).N.$https:/
-000003e0: 2f61 7069 2e77 6974 6867 7261 6861 6d2e  /api.withgraham.
-000003f0: 696f 2f76 312f 7461 626c 6573 2f7a 0a2f  io/v1/tables/z./
-00000400: 6461 7461 2f72 6561 64da 0571 7565 7279  data/read..query
-00000410: da05 6c69 6d69 74da 0f73 656c 6563 7465  ..limit..selecte
-00000420: 6443 6f6c 756d 6e73 a902 da07 6865 6164  dColumns....head
-00000430: 6572 73da 046a 736f 6ee9 c800 0000 7a19  ers..json.....z.
-00000440: 6661 696c 6564 2074 6f20 7265 6164 2066  failed to read f
-00000450: 726f 6d20 7461 626c 65a9 0372 0500 0000  rom table..r....
-00000460: da04 7465 7874 7206 0000 00da 0772 6573  ..textr......res
-00000470: 756c 7473 e9ad 0100 00fa 1372 6174 6520  ults.......rate 
-00000480: 6c69 6d69 7420 6578 6365 6564 6564 7204  limit exceededr.
-00000490: 0000 00a9 0972 0700 0000 da03 7374 7272  .....r......strr
-000004a0: 0800 0000 da08 7265 7175 6573 7473 da04  ......requests..
-000004b0: 706f 7374 7210 0000 0072 0500 0000 721a  postr....r....r.
-000004c0: 0000 0072 1700 0000 2907 720b 0000 0072  ...r....).r....r
-000004d0: 1200 0000 7213 0000 0072 1400 0000 da03  ....r....r......
-000004e0: 7572 6cda 0770 6179 6c6f 6164 da01 7272  url..payload..rr
-000004f0: 0c00 0000 720c 0000 0072 0d00 0000 da04  ....r....r......
-00000500: 5265 6164 1600 0000 732c 0000 0008 0112  Read....s,......
-00000510: 0104 0204 ff08 0308 0108 0108 0114 020a  ................
-00000520: 0102 0104 0104 0102 0106 fd10 f40e 1120  ............... 
-00000530: ef02 1202 0102 0108 fe7a 0b54 6162 6c65  .........z.Table
-00000540: 732e 5265 6164 6302 0000 0000 0000 0000  s.Readc.........
-00000550: 0000 0005 0000 0008 0000 0043 0000 00f3  ...........C....
-00000560: 9e00 0000 7c00 6a00 8f3d 0100 6401 7401  ....|.j..=..d.t.
-00000570: 7c00 6a02 8301 1700 6402 1700 7d02 6403  |.j.....d...}.d.
-00000580: 7c01 6901 7d03 7403 6a04 7c02 7c00 a005  |.i.}.t.j.|.|...
-00000590: a100 7c03 6404 8d03 7d04 7c04 6a06 6405  ..|.d...}.|.j.d.
-000005a0: 6b03 7231 6400 7c04 6a06 7c04 6a07 6406  k.r1d.|.j.|.j.d.
-000005b0: 6407 9c03 6602 5700 0200 6400 0400 0400  d...f.W...d.....
-000005c0: 8303 0100 5300 7c04 a008 a100 6408 1900  ....S.|.....d...
-000005d0: 6400 6602 5700 0200 6400 0400 0400 8303  d.f.W...d.......
-000005e0: 0100 5300 3100 7343 7701 0100 0100 0100  ..S.1.sCw.......
-000005f0: 5900 0100 6400 6409 640a 640b 9c02 6602  Y...d.d.d.d...f.
-00000600: 5300 290c 4e72 1100 0000 fa05 2f64 6174  S.).Nr....../dat
-00000610: 61da 0464 6174 6172 1500 0000 7218 0000  a..datar....r...
-00000620: 007a 1866 6169 6c65 6420 746f 2077 7269  .z.failed to wri
-00000630: 7465 2074 6f20 7461 626c 6572 1900 0000  te to tabler....
-00000640: 721b 0000 0072 1c00 0000 721d 0000 0072  r....r....r....r
-00000650: 0400 0000 721e 0000 0029 0572 0b00 0000  ....r....).r....
-00000660: 7228 0000 0072 2200 0000 7223 0000 0072  r(...r"...r#...r
-00000670: 2400 0000 720c 0000 0072 0c00 0000 720d  $...r....r....r.
-00000680: 0000 00da 0557 7269 7465 2e00 0000 f324  .....Write.....$
-00000690: 0000 0008 0112 0104 0204 ff14 040a 0102  ................
-000006a0: 0104 0104 0102 0106 fd10 f80e 0d20 f302  ............. ..
-000006b0: 0e02 0102 0108 fe7a 0c54 6162 6c65 732e  .......z.Tables.
-000006c0: 5772 6974 6563 0200 0000 0000 0000 0000  Writec..........
-000006d0: 0000 0500 0000 0800 0000 4300 0000 7226  ..........C...r&
-000006e0: 0000 0029 0c4e 7211 0000 0072 2700 0000  ...).Nr....r'...
-000006f0: 7212 0000 0072 1500 0000 7218 0000 00fa  r....r....r.....
-00000700: 1b66 6169 6c65 6420 746f 2064 656c 6574  .failed to delet
-00000710: 6520 6672 6f6d 2074 6162 6c65 7219 0000  e from tabler...
-00000720: 0072 1b00 0000 721c 0000 0072 1d00 0000  .r....r....r....
-00000730: 7204 0000 00a9 0972 0700 0000 721f 0000  r......r....r...
-00000740: 0072 0800 0000 7220 0000 00da 0664 656c  .r....r .....del
-00000750: 6574 6572 1000 0000 7205 0000 0072 1a00  eter....r....r..
-00000760: 0000 7217 0000 0029 0572 0b00 0000 7212  ..r....).r....r.
-00000770: 0000 0072 2200 0000 7223 0000 0072 2400  ...r"...r#...r$.
-00000780: 0000 720c 0000 0072 0c00 0000 720d 0000  ..r....r....r...
-00000790: 00da 0644 656c 6574 6542 0000 0072 2a00  ...DeleteB...r*.
-000007a0: 0000 7a0d 5461 626c 6573 2e44 656c 6574  ..z.Tables.Delet
-000007b0: 6563 0100 0000 0000 0000 0000 0000 0300  ec..............
-000007c0: 0000 0800 0000 4300 0000 7396 0000 007c  ......C...s....|
-000007d0: 006a 008f 3901 0064 0174 017c 006a 0283  .j..9..d.t.|.j..
-000007e0: 0117 0064 0217 007d 0174 036a 047c 017c  ...d...}.t.j.|.|
-000007f0: 00a0 05a1 0069 0064 038d 037d 027c 026a  .....i.d...}.|.j
-00000800: 0664 046b 0372 2d64 007c 026a 067c 026a  .d.k.r-d.|.j.|.j
-00000810: 0764 0564 069c 0366 0257 0002 0064 0004  .d.d...f.W...d..
-00000820: 0004 0083 0301 0053 007c 02a0 08a1 0064  .......S.|.....d
-00000830: 0719 0064 0066 0257 0002 0064 0004 0004  ...d.f.W...d....
-00000840: 0083 0301 0053 0031 0073 3f77 0101 0001  .....S.1.s?w....
-00000850: 0001 0059 0001 0064 0064 0864 0964 0a9c  ...Y...d.d.d.d..
-00000860: 0266 0253 0029 0b4e 7211 0000 007a 092f  .f.S.).Nr....z./
-00000870: 6461 7461 2f61 6c6c 7215 0000 0072 1800  data/allr....r..
-00000880: 0000 722b 0000 0072 1900 0000 721b 0000  ..r+...r....r...
-00000890: 0072 1c00 0000 721d 0000 0072 0400 0000  .r....r....r....
-000008a0: 722c 0000 0029 0372 0b00 0000 7222 0000  r,...).r....r"..
-000008b0: 0072 2400 0000 720c 0000 0072 0c00 0000  .r$...r....r....
-000008c0: 720d 0000 00da 0944 656c 6574 6541 6c6c  r......DeleteAll
-000008d0: 5600 0000 7320 0000 0008 0112 0114 020a  V...s ..........
-000008e0: 0102 0104 0104 0102 0106 fd10 fb0e 0a20  ............... 
-000008f0: f602 0b02 0102 0108 fe7a 1054 6162 6c65  .........z.Table
-00000900: 732e 4465 6c65 7465 416c 6c63 0300 0000  s.DeleteAllc....
-00000910: 0000 0000 0000 0000 0600 0000 0800 0000  ................
-00000920: 4300 0000 73a0 0000 007c 006a 008f 3e01  C...s....|.j..>.
-00000930: 0064 0174 017c 006a 0283 0117 0064 0217  .d.t.|.j.....d..
-00000940: 007d 037c 027c 0164 039c 027d 0474 036a  .}.|.|.d...}.t.j
-00000950: 047c 037c 00a0 05a1 007c 0464 048d 037d  .|.|.....|.d...}
-00000960: 057c 056a 0664 056b 0372 3264 007c 056a  .|.j.d.k.r2d.|.j
-00000970: 067c 056a 0764 0664 079c 0366 0257 0002  .|.j.d.d...f.W..
-00000980: 0064 0004 0004 0083 0301 0053 007c 05a0  .d.........S.|..
-00000990: 08a1 0064 0819 0064 0066 0257 0002 0064  ...d...d.f.W...d
-000009a0: 0004 0004 0083 0301 0053 0031 0073 4477  .........S.1.sDw
-000009b0: 0101 0001 0001 0059 0001 0064 0064 0964  .......Y...d.d.d
-000009c0: 0a64 0b9c 0266 0253 0029 0c4e 7211 0000  .d...f.S.).Nr...
-000009d0: 0072 2700 0000 2902 7228 0000 0072 1200  .r'...).r(...r..
-000009e0: 0000 7215 0000 0072 1800 0000 7a16 6661  ..r....r....z.fa
-000009f0: 696c 6564 2074 6f20 7570 6461 7465 2074  iled to update t
-00000a00: 6162 6c65 7219 0000 0072 1b00 0000 721c  abler....r....r.
-00000a10: 0000 0072 1d00 0000 7204 0000 0029 0972  ...r....r....).r
-00000a20: 0700 0000 721f 0000 0072 0800 0000 7220  ....r....r....r 
-00000a30: 0000 005a 0570 6174 6368 7210 0000 0072  ...Z.patchr....r
-00000a40: 0500 0000 721a 0000 0072 1700 0000 2906  ....r....r....).
-00000a50: 720b 0000 0072 1200 0000 7228 0000 0072  r....r....r(...r
-00000a60: 2200 0000 7223 0000 0072 2400 0000 720c  "...r#...r$...r.
-00000a70: 0000 0072 0c00 0000 720d 0000 00da 0655  ...r....r......U
-00000a80: 7064 6174 6567 0000 0073 2600 0000 0801  pdateg...s&.....
-00000a90: 1201 0202 0201 06fe 1405 0a01 0201 0401  ................
-00000aa0: 0401 0201 06fd 10f7 0e0e 20f2 020f 0201  .......... .....
-00000ab0: 0201 08fe 7a0d 5461 626c 6573 2e55 7064  ....z.Tables.Upd
-00000ac0: 6174 6529 0ada 085f 5f6e 616d 655f 5fda  ate)...__name__.
-00000ad0: 0a5f 5f6d 6f64 756c 655f 5fda 0c5f 5f71  .__module__..__q
-00000ae0: 7561 6c6e 616d 655f 5f72 0e00 0000 7210  ualname__r....r.
-00000af0: 0000 0072 2500 0000 7229 0000 0072 2e00  ...r%...r)...r..
-00000b00: 0000 722f 0000 0072 3000 0000 720c 0000  ..r/...r0...r...
-00000b10: 0072 0c00 0000 720c 0000 0072 0d00 0000  .r....r....r....
-00000b20: 7202 0000 0003 0000 0073 1000 0000 0800  r........s......
-00000b30: 0801 080b 1007 0c18 0c14 0814 1211 7202  ..............r.
-00000b40: 0000 0029 0272 2000 0000 7202 0000 0072  ...).r ...r....r
-00000b50: 0c00 0000 720c 0000 0072 0c00 0000 720d  ....r....r....r.
-00000b60: 0000 00da 083c 6d6f 6475 6c65 3e01 0000  .....<module>...
-00000b70: 0073 0400 0000 0800 1202                 .s........
+00000080: 6404 8400 5a04 6405 6406 8400 5a05 6900  d...Z.d.d...Z.i.
+00000090: 6407 6407 6603 6408 6409 8401 5a06 6900  d.d.f.d.d...Z.i.
+000000a0: 6601 640a 640b 8401 5a07 6900 6601 640c  f.d.d...Z.i.f.d.
+000000b0: 640d 8401 5a08 640e 640f 8400 5a09 6900  d...Z.d.d...Z.i.
+000000c0: 6900 6602 6410 6411 8401 5a0a 6407 5300  i.f.d.d...Z.d.S.
+000000d0: 2912 da06 5461 626c 6573 6305 0000 0000  )...Tablesc.....
+000000e0: 0000 0000 0000 0005 0000 0004 0000 0043  ...............C
+000000f0: 0000 0073 4000 0000 7c04 6400 6b02 7308  ...s@...|.d.k.s.
+00000100: 7c04 6401 6b02 720f 6400 6402 6403 6404  |.d.k.r.d.d.d.d.
+00000110: 9c02 6602 5300 7c01 7c00 5f00 7c04 7c00  ..f.S.|.|._.|.|.
+00000120: 5f01 7c02 7c00 5f02 7c03 7c00 5f03 6405  _.|.|._.|.|._.d.
+00000130: 7c00 5f04 6400 5300 2906 4eda 0069 9001  |._.d.S.).N..i..
+00000140: 0000 7a14 5461 626c 6520 4944 2069 7320  ..z.Table ID is 
+00000150: 7265 7175 6972 6564 a902 da0b 7374 6174  required....stat
+00000160: 7573 5f63 6f64 65da 0d65 7272 6f72 5f6d  us_code..error_m
+00000170: 6573 7361 6765 e90f 0000 0029 05da 0c72  essage.....)...r
+00000180: 6174 655f 6c69 6d69 7465 72da 0874 6162  ate_limiter..tab
+00000190: 6c65 5f69 64da 0761 7069 5f6b 6579 da0a  le_id..api_key..
+000001a0: 636f 6d70 616e 795f 6964 da07 7469 6d65  company_id..time
+000001b0: 6f75 7429 05da 0473 656c 6672 0800 0000  out)...selfr....
+000001c0: 720a 0000 0072 0b00 0000 7209 0000 00a9  r....r....r.....
+000001d0: 0072 0e00 0000 fa37 6275 696c 642f 6264  .r.....7build/bd
+000001e0: 6973 742e 6d61 636f 7378 2d31 302e 392d  ist.macosx-10.9-
+000001f0: 756e 6976 6572 7361 6c32 2f65 6767 2f67  universal2/egg/g
+00000200: 7261 6861 6d2f 7461 626c 6573 2e70 79da  raham/tables.py.
+00000210: 085f 5f69 6e69 745f 5f04 0000 0073 1400  .__init__....s..
+00000220: 0000 1001 0201 0201 0201 08fe 0604 0601  ................
+00000230: 0601 0601 0a01 7a0f 5461 626c 6573 2e5f  ......z.Tables._
+00000240: 5f69 6e69 745f 5f63 0100 0000 0000 0000  _init__c........
+00000250: 0000 0000 0100 0000 0100 0000 4300 0000  ............C...
+00000260: 7306 0000 007c 006a 0053 0029 014e 2901  s....|.j.S.).N).
+00000270: 720c 0000 00a9 0172 0d00 0000 720e 0000  r......r....r...
+00000280: 0072 0e00 0000 720f 0000 00da 0c5f 6765  .r....r......_ge
+00000290: 745f 7469 6d65 6f75 7410 0000 0073 0200  t_timeout....s..
+000002a0: 0000 0601 7a13 5461 626c 6573 2e5f 6765  ....z.Tables._ge
+000002b0: 745f 7469 6d65 6f75 7463 0100 0000 0000  t_timeoutc......
+000002c0: 0000 0000 0000 0100 0000 0400 0000 4300  ..............C.
+000002d0: 0000 7314 0000 0064 017c 006a 0017 007c  ..s....d.|.j...|
+000002e0: 006a 0164 0264 039c 0353 0029 044e 7a07  .j.d.d...S.).Nz.
+000002f0: 4265 6172 6572 207a 1061 7070 6c69 6361  Bearer z.applica
+00000300: 7469 6f6e 2f6a 736f 6e29 03da 0d41 7574  tion/json)...Aut
+00000310: 686f 7269 7a61 7469 6f6e 5a07 436f 6d70  horizationZ.Comp
+00000320: 616e 797a 0c43 6f6e 7465 6e74 2d54 7970  anyz.Content-Typ
+00000330: 6529 0272 0a00 0000 720b 0000 0072 1100  e).r....r....r..
+00000340: 0000 720e 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000350: 00da 0c5f 6765 745f 6865 6164 6572 7313  ..._get_headers.
+00000360: 0000 0073 0800 0000 0802 0401 0201 06fd  ...s............
+00000370: 7a13 5461 626c 6573 2e5f 6765 745f 6865  z.Tables._get_he
+00000380: 6164 6572 734e 6304 0000 0000 0000 0000  adersNc.........
+00000390: 0000 0007 0000 0008 0000 0043 0000 0073  ...........C...s
+000003a0: c400 0000 7c00 6a00 8f50 0100 6401 7401  ....|.j..P..d.t.
+000003b0: 7c00 6a02 8301 1700 6402 1700 7d04 6403  |.j.....d...}.d.
+000003c0: 7c01 6901 7d05 7c02 6400 6b03 7219 7c02  |.i.}.|.d.k.r.|.
+000003d0: 7c05 6404 3c00 7c03 6400 6b03 7221 7c03  |.d.<.|.d.k.r!|.
+000003e0: 7c05 6405 3c00 7403 6a04 7c04 7c00 a005  |.d.<.t.j.|.|...
+000003f0: a100 7c05 7c00 a006 a100 6406 8d04 7d06  ..|.|.....d...}.
+00000400: 7c06 6a07 6407 6b03 7244 6400 7c06 6a07  |.j.d.k.rDd.|.j.
+00000410: 7c06 6a08 6408 6409 9c03 6602 5700 0200  |.j.d.d...f.W...
+00000420: 6400 0400 0400 8303 0100 5300 7c06 a009  d.........S.|...
+00000430: a100 640a 1900 6400 6602 5700 0200 6400  ..d...d.f.W...d.
+00000440: 0400 0400 8303 0100 5300 3100 7356 7701  ........S.1.sVw.
+00000450: 0100 0100 0100 5900 0100 6400 640b 640c  ......Y...d.d.d.
+00000460: 640d 9c02 6602 5300 290e 4efa 2468 7474  d...f.S.).N.$htt
+00000470: 7073 3a2f 2f61 7069 2e77 6974 6867 7261  ps://api.withgra
+00000480: 6861 6d2e 696f 2f76 312f 7461 626c 6573  ham.io/v1/tables
+00000490: 2f7a 0a2f 6461 7461 2f72 6561 64da 0571  /z./data/read..q
+000004a0: 7565 7279 da05 6c69 6d69 74da 0f73 656c  uery..limit..sel
+000004b0: 6563 7465 6443 6f6c 756d 6e73 a903 da07  ectedColumns....
+000004c0: 6865 6164 6572 73da 046a 736f 6e72 0c00  headers..jsonr..
+000004d0: 0000 e9c8 0000 007a 1966 6169 6c65 6420  .......z.failed 
+000004e0: 746f 2072 6561 6420 6672 6f6d 2074 6162  to read from tab
+000004f0: 6c65 a903 7205 0000 00da 0474 6578 7472  le..r......textr
+00000500: 0600 0000 da07 7265 7375 6c74 73e9 ad01  ......results...
+00000510: 0000 fa13 7261 7465 206c 696d 6974 2065  ....rate limit e
+00000520: 7863 6565 6465 6472 0400 0000 a90a 7208  xceededr......r.
+00000530: 0000 00da 0373 7472 7209 0000 00da 0872  .....strr......r
+00000540: 6571 7565 7374 73da 0470 6f73 7472 1400  equests..postr..
+00000550: 0000 7212 0000 0072 0500 0000 721e 0000  ..r....r....r...
+00000560: 0072 1b00 0000 2907 720d 0000 0072 1600  .r....).r....r..
+00000570: 0000 7217 0000 0072 1800 0000 da03 7572  ..r....r......ur
+00000580: 6cda 0770 6179 6c6f 6164 da01 7272 0e00  l..payload..rr..
+00000590: 0000 720e 0000 0072 0f00 0000 da04 5265  ..r....r......Re
+000005a0: 6164 1a00 0000 732c 0000 0008 0112 0104  ad....s,........
+000005b0: 0204 ff08 0308 0108 0108 011a 020a 0102  ................
+000005c0: 0104 0104 0102 0106 fd10 f40e 1120 ef02  ............. ..
+000005d0: 1202 0102 0108 fe7a 0b54 6162 6c65 732e  .......z.Tables.
+000005e0: 5265 6164 6302 0000 0000 0000 0000 0000  Readc...........
+000005f0: 0005 0000 0008 0000 0043 0000 00f3 a400  .........C......
+00000600: 0000 7c00 6a00 8f40 0100 6401 7401 7c00  ..|.j..@..d.t.|.
+00000610: 6a02 8301 1700 6402 1700 7d02 6403 7c01  j.....d...}.d.|.
+00000620: 6901 7d03 7403 6a04 7c02 7c00 a005 a100  i.}.t.j.|.|.....
+00000630: 7c03 7c00 a006 a100 6404 8d04 7d04 7c04  |.|.....d...}.|.
+00000640: 6a07 6405 6b03 7234 6400 7c04 6a07 7c04  j.d.k.r4d.|.j.|.
+00000650: 6a08 6406 6407 9c03 6602 5700 0200 6400  j.d.d...f.W...d.
+00000660: 0400 0400 8303 0100 5300 7c04 a009 a100  ........S.|.....
+00000670: 6408 1900 6400 6602 5700 0200 6400 0400  d...d.f.W...d...
+00000680: 0400 8303 0100 5300 3100 7346 7701 0100  ......S.1.sFw...
+00000690: 0100 0100 5900 0100 6400 6409 640a 640b  ....Y...d.d.d.d.
+000006a0: 9c02 6602 5300 290c 4e72 1500 0000 fa05  ..f.S.).Nr......
+000006b0: 2f64 6174 61da 0464 6174 6172 1900 0000  /data..datar....
+000006c0: 721c 0000 007a 1866 6169 6c65 6420 746f  r....z.failed to
+000006d0: 2077 7269 7465 2074 6f20 7461 626c 6572   write to tabler
+000006e0: 1d00 0000 721f 0000 0072 2000 0000 7221  ....r....r ...r!
+000006f0: 0000 0072 0400 0000 7222 0000 0029 0572  ...r....r"...).r
+00000700: 0d00 0000 722c 0000 0072 2600 0000 7227  ....r,...r&...r'
+00000710: 0000 0072 2800 0000 720e 0000 0072 0e00  ...r(...r....r..
+00000720: 0000 720f 0000 00da 0557 7269 7465 3200  ..r......Write2.
+00000730: 0000 f324 0000 0008 0112 0104 0204 ff1a  ...$............
+00000740: 040a 0102 0104 0104 0102 0106 fd10 f80e  ................
+00000750: 0d20 f302 0e02 0102 0108 fe7a 0c54 6162  . .........z.Tab
+00000760: 6c65 732e 5772 6974 6563 0200 0000 0000  les.Writec......
+00000770: 0000 0000 0000 0500 0000 0800 0000 4300  ..............C.
+00000780: 0000 722a 0000 0029 0c4e 7215 0000 0072  ..r*...).Nr....r
+00000790: 2b00 0000 7216 0000 0072 1900 0000 721c  +...r....r....r.
+000007a0: 0000 00fa 1b66 6169 6c65 6420 746f 2064  .....failed to d
+000007b0: 656c 6574 6520 6672 6f6d 2074 6162 6c65  elete from table
+000007c0: 721d 0000 0072 1f00 0000 7220 0000 0072  r....r....r ...r
+000007d0: 2100 0000 7204 0000 00a9 0a72 0800 0000  !...r......r....
+000007e0: 7223 0000 0072 0900 0000 7224 0000 00da  r#...r....r$....
+000007f0: 0664 656c 6574 6572 1400 0000 7212 0000  .deleter....r...
+00000800: 0072 0500 0000 721e 0000 0072 1b00 0000  .r....r....r....
+00000810: 2905 720d 0000 0072 1600 0000 7226 0000  ).r....r....r&..
+00000820: 0072 2700 0000 7228 0000 0072 0e00 0000  .r'...r(...r....
+00000830: 720e 0000 0072 0f00 0000 da06 4465 6c65  r....r......Dele
+00000840: 7465 4600 0000 722e 0000 007a 0d54 6162  teF...r....z.Tab
+00000850: 6c65 732e 4465 6c65 7465 6301 0000 0000  les.Deletec.....
+00000860: 0000 0000 0000 0003 0000 0008 0000 0043  ...............C
+00000870: 0000 0073 9c00 0000 7c00 6a00 8f3c 0100  ...s....|.j..<..
+00000880: 6401 7401 7c00 6a02 8301 1700 6402 1700  d.t.|.j.....d...
+00000890: 7d01 7403 6a04 7c01 7c00 a005 a100 6900  }.t.j.|.|.....i.
+000008a0: 7c00 a006 a100 6403 8d04 7d02 7c02 6a07  |.....d...}.|.j.
+000008b0: 6404 6b03 7230 6400 7c02 6a07 7c02 6a08  d.k.r0d.|.j.|.j.
+000008c0: 6405 6406 9c03 6602 5700 0200 6400 0400  d.d...f.W...d...
+000008d0: 0400 8303 0100 5300 7c02 a009 a100 6407  ......S.|.....d.
+000008e0: 1900 6400 6602 5700 0200 6400 0400 0400  ..d.f.W...d.....
+000008f0: 8303 0100 5300 3100 7342 7701 0100 0100  ....S.1.sBw.....
+00000900: 0100 5900 0100 6400 6408 6409 640a 9c02  ..Y...d.d.d.d...
+00000910: 6602 5300 290b 4e72 1500 0000 7a09 2f64  f.S.).Nr....z./d
+00000920: 6174 612f 616c 6c72 1900 0000 721c 0000  ata/allr....r...
+00000930: 0072 2f00 0000 721d 0000 0072 1f00 0000  .r/...r....r....
+00000940: 7220 0000 0072 2100 0000 7204 0000 0072  r ...r!...r....r
+00000950: 3000 0000 2903 720d 0000 0072 2600 0000  0...).r....r&...
+00000960: 7228 0000 0072 0e00 0000 720e 0000 0072  r(...r....r....r
+00000970: 0f00 0000 da09 4465 6c65 7465 416c 6c5a  ......DeleteAllZ
+00000980: 0000 0073 2000 0000 0801 1201 1a02 0a01  ...s ...........
+00000990: 0201 0401 0401 0201 06fd 10fb 0e0a 20f6  .............. .
+000009a0: 020b 0201 0201 08fe 7a10 5461 626c 6573  ........z.Tables
+000009b0: 2e44 656c 6574 6541 6c6c 6303 0000 0000  .DeleteAllc.....
+000009c0: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
+000009d0: 0000 0073 a600 0000 7c00 6a00 8f41 0100  ...s....|.j..A..
+000009e0: 6401 7401 7c00 6a02 8301 1700 6402 1700  d.t.|.j.....d...
+000009f0: 7d03 7c02 7c01 6403 9c02 7d04 7403 6a04  }.|.|.d...}.t.j.
+00000a00: 7c03 7c00 a005 a100 7c04 7c00 a006 a100  |.|.....|.|.....
+00000a10: 6404 8d04 7d05 7c05 6a07 6405 6b03 7235  d...}.|.j.d.k.r5
+00000a20: 6400 7c05 6a07 7c05 6a08 6406 6407 9c03  d.|.j.|.j.d.d...
+00000a30: 6602 5700 0200 6400 0400 0400 8303 0100  f.W...d.........
+00000a40: 5300 7c05 a009 a100 6408 1900 6400 6602  S.|.....d...d.f.
+00000a50: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
+00000a60: 3100 7347 7701 0100 0100 0100 5900 0100  1.sGw.......Y...
+00000a70: 6400 6409 640a 640b 9c02 6602 5300 290c  d.d.d.d...f.S.).
+00000a80: 4e72 1500 0000 722b 0000 0029 0272 2c00  Nr....r+...).r,.
+00000a90: 0000 7216 0000 0072 1900 0000 721c 0000  ..r....r....r...
+00000aa0: 007a 1666 6169 6c65 6420 746f 2075 7064  .z.failed to upd
+00000ab0: 6174 6520 7461 626c 6572 1d00 0000 721f  ate tabler....r.
+00000ac0: 0000 0072 2000 0000 7221 0000 0072 0400  ...r ...r!...r..
+00000ad0: 0000 290a 7208 0000 0072 2300 0000 7209  ..).r....r#...r.
+00000ae0: 0000 0072 2400 0000 5a05 7061 7463 6872  ...r$...Z.patchr
+00000af0: 1400 0000 7212 0000 0072 0500 0000 721e  ....r....r....r.
+00000b00: 0000 0072 1b00 0000 2906 720d 0000 0072  ...r....).r....r
+00000b10: 1600 0000 722c 0000 0072 2600 0000 7227  ....r,...r&...r'
+00000b20: 0000 0072 2800 0000 720e 0000 0072 0e00  ...r(...r....r..
+00000b30: 0000 720f 0000 00da 0655 7064 6174 656b  ..r......Updatek
+00000b40: 0000 0073 2600 0000 0801 1201 0202 0201  ...s&...........
+00000b50: 06fe 1a05 0a01 0201 0401 0401 0201 06fd  ................
+00000b60: 10f7 0e0e 20f2 020f 0201 0201 08fe 7a0d  .... .........z.
+00000b70: 5461 626c 6573 2e55 7064 6174 6529 0bda  Tables.Update)..
+00000b80: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
+00000b90: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
+00000ba0: 655f 5f72 1000 0000 7212 0000 0072 1400  e__r....r....r..
+00000bb0: 0000 7229 0000 0072 2d00 0000 7232 0000  ..r)...r-...r2..
+00000bc0: 0072 3300 0000 7234 0000 0072 0e00 0000  .r3...r4...r....
+00000bd0: 720e 0000 0072 0e00 0000 720f 0000 0072  r....r....r....r
+00000be0: 0200 0000 0300 0000 7312 0000 0008 0008  ........s.......
+00000bf0: 0108 0c08 0310 070c 180c 1408 1412 1172  ...............r
+00000c00: 0200 0000 2902 7224 0000 0072 0200 0000  ....).r$...r....
+00000c10: 720e 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+00000c20: 0f00 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00000c30: 0000 7304 0000 0008 0012 02              ..s........
```

