# Comparing `tmp/graham_client-0.0.1-py3.10.egg` & `tmp/graham_client-0.0.2-py3.10.egg`

## zipinfo {}

```diff
@@ -1,18 +1,20 @@
-Zip file size: 7934 bytes, number of entries: 16
--rw-r--r--  2.0 unx      282 b- defN 23-May-25 10:19 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      310 b- defN 23-May-25 10:19 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-25 10:19 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx       42 b- defN 23-May-25 10:19 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-25 10:19 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-25 10:19 EGG-INFO/zip-safe
+Zip file size: 9354 bytes, number of entries: 18
+-rw-r--r--  2.0 unx      282 b- defN 23-May-26 07:35 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      338 b- defN 23-May-26 07:35 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-26 07:35 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx       42 b- defN 23-May-26 07:35 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-26 07:35 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-26 07:35 EGG-INFO/zip-safe
 -rw-r--r--  2.0 unx        0 b- defN 23-May-24 07:26 examples/__init__.py
+-rw-r--r--  2.0 unx      549 b- defN 23-May-26 07:25 examples/demo-financials.py
 -rw-r--r--  2.0 unx      356 b- defN 23-May-25 10:17 examples/demo-tables.py
--rw-r--r--  2.0 unx      152 b- defN 23-May-25 10:19 examples/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx      478 b- defN 23-May-25 10:19 examples/__pycache__/demo-tables.cpython-310.pyc
+-rw-r--r--  2.0 unx      152 b- defN 23-May-26 07:35 examples/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx      587 b- defN 23-May-26 07:35 examples/__pycache__/demo-financials.cpython-310.pyc
+-rw-r--r--  2.0 unx      478 b- defN 23-May-26 07:35 examples/__pycache__/demo-tables.cpython-310.pyc
 -rw-r--r--  2.0 unx      498 b- defN 23-May-25 10:17 graham/__init__.py
--rw-r--r--  2.0 unx     4757 b- defN 23-May-25 07:44 graham/equities.py
--rw-r--r--  2.0 unx     4364 b- defN 23-May-25 07:44 graham/tables.py
--rw-r--r--  2.0 unx      975 b- defN 23-May-25 10:19 graham/__pycache__/__init__.cpython-310.pyc
--rw-r--r--  2.0 unx     2789 b- defN 23-May-25 10:19 graham/__pycache__/equities.cpython-310.pyc
--rw-r--r--  2.0 unx     2938 b- defN 23-May-25 10:19 graham/__pycache__/tables.cpython-310.pyc
-16 files, 17959 bytes uncompressed, 5814 bytes compressed:  67.6%
+-rw-r--r--  2.0 unx     6199 b- defN 23-May-26 07:33 graham/equities.py
+-rw-r--r--  2.0 unx     4364 b- defN 23-May-26 07:18 graham/tables.py
+-rw-r--r--  2.0 unx      975 b- defN 23-May-26 07:35 graham/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--  2.0 unx     3638 b- defN 23-May-26 07:35 graham/__pycache__/equities.cpython-310.pyc
+-rw-r--r--  2.0 unx     2938 b- defN 23-May-26 07:35 graham/__pycache__/tables.cpython-310.pyc
+18 files, 21414 bytes uncompressed, 6924 bytes compressed:  67.7%
```

## zipnote «TEMP»/diffoscope_v2cplt9a_/tmptvolk4r5_.zip

```diff
@@ -15,20 +15,26 @@
 
 Filename: EGG-INFO/zip-safe
 Comment: 
 
 Filename: examples/__init__.py
 Comment: 
 
+Filename: examples/demo-financials.py
+Comment: 
+
 Filename: examples/demo-tables.py
 Comment: 
 
 Filename: examples/__pycache__/__init__.cpython-310.pyc
 Comment: 
 
+Filename: examples/__pycache__/demo-financials.cpython-310.pyc
+Comment: 
+
 Filename: examples/__pycache__/demo-tables.cpython-310.pyc
 Comment: 
 
 Filename: graham/__init__.py
 Comment: 
 
 Filename: graham/equities.py
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graham-client
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python client for withgraham.io
 Author: WithGraham
 Author-email: support@withgraham.io
 Keywords: python,financial,data,api,withgraham,graham,value investing
 License-File: LICENSE
 
 A Python client for withgraham.io
```

## EGG-INFO/SOURCES.txt

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 examples/__init__.py
+examples/demo-financials.py
 examples/demo-tables.py
 graham/__init__.py
 graham/equities.py
 graham/tables.py
 graham_client.egg-info/PKG-INFO
 graham_client.egg-info/SOURCES.txt
 graham_client.egg-info/dependency_links.txt
```

## graham/equities.py

```diff
@@ -1,120 +1,161 @@
 import requests
 from urllib.parse import urlencode
 
-class Equities:
+class Financials:
     def __init__(self, rate_limiter, api_key, company_id, return_raw=False):
         self.rate_limiter = rate_limiter
         self.api_key = api_key
         self.company_id = company_id
         self.return_raw = return_raw
     
     def _get_headers(self):
         return {
             'Authorization': 'Bearer ' + self.api_key,
             'Company': self.company_id,
             'Content-Type': 'application/json'
         }
+
+    def ListSummary(self, equity_id='', query={}):
+        with self.rate_limiter:
+            query_str = urlencode(query)
+            url = 'https://api.withgraham.io/v1/equities/' + str(equity_id) + '/financials'
+            if query_str != '':
+                url += '?' + query_str
+            
+            r = requests.get(url, headers=self._get_headers(), json=None)
+            if r.status_code != 200:
+                return None, {
+                    'status_code': r.status_code,
+                    'text': r.text,
+                    'error_message': 'failed to get financials for equity'
+                }
+            
+            if self.return_raw:
+                return r.json(), None
+            return r.json()['financials'], None
+        return None, {
+            'status_code': 429,
+            'error_message': 'rate limit exceeded'
+        }
     
-    def List(self, query={}):
+    def ListSECForms(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
-            url = 'https://api.withgraham.io/v1/equities'
+            url = 'https://api.withgraham.io/v1/equities/' + str(equity_id) + '/financials/sec-forms'
             if query_str != '':
                 url += '?' + query_str
             
             r = requests.get(url, headers=self._get_headers(), json=None)
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
-                    'error_message': 'failed to list equities'
+                    'error_message': 'failed to get SEC forms for equity'
                 }
             
             if self.return_raw:
                 return r.json(), None
-            return r.json()['equities'], None
+            return r.json()['forms'], None
         return None, {
             'status_code': 429,
             'error_message': 'rate limit exceeded'
         }
     
-    def Get(self, public_company_id='', query={}):
+
+class Equities:
+    def __init__(self, rate_limiter, api_key, company_id, return_raw=False):
+        self.rate_limiter = rate_limiter
+        self.api_key = api_key
+        self.company_id = company_id
+        self.return_raw = return_raw
+    
+    def _get_headers(self):
+        return {
+            'Authorization': 'Bearer ' + self.api_key,
+            'Company': self.company_id,
+            'Content-Type': 'application/json'
+        }
+    
+    def List(self, query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
-            url = 'https://api.withgraham.io/v1/equities/' + str(public_company_id)
+            url = 'https://api.withgraham.io/v1/equities'
             if query_str != '':
                 url += '?' + query_str
             
             r = requests.get(url, headers=self._get_headers(), json=None)
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
-                    'error_message': 'failed to get equity'
+                    'error_message': 'failed to list equities'
                 }
             
             if self.return_raw:
                 return r.json(), None
-            return r.json()['equity'], None
+            return r.json()['equities'], None
         return None, {
             'status_code': 429,
             'error_message': 'rate limit exceeded'
         }
     
-    def Daily(self, public_company_id='', query={}):
+    def Get(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
-            url = 'https://api.withgraham.io/v1/equities/' + str(public_company_id) + '/daily'
+            url = 'https://api.withgraham.io/v1/equities/' + str(equity_id)
             if query_str != '':
                 url += '?' + query_str
             
             r = requests.get(url, headers=self._get_headers(), json=None)
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
                     'error_message': 'failed to get equity'
                 }
             
             if self.return_raw:
                 return r.json(), None
-            return r.json()['dailySnapshots'], None
+            return r.json()['equity'], None
         return None, {
             'status_code': 429,
             'error_message': 'rate limit exceeded'
         }
     
-    def Financials(self, public_company_id='', query={}):
+    def Daily(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
-            url = 'https://api.withgraham.io/v1/equities/' + str(public_company_id) + '/financials'
+            url = 'https://api.withgraham.io/v1/equities/' + str(equity_id) + '/daily'
             if query_str != '':
                 url += '?' + query_str
             
             r = requests.get(url, headers=self._get_headers(), json=None)
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
                     'text': r.text,
-                    'error_message': 'failed to get equity'
+                    'error_message': 'failed to get daily snapshot for equity'
                 }
             
             if self.return_raw:
                 return r.json(), None
-            return r.json()['financials'], None
+            return r.json()['dailySnapshots'], None
         return None, {
             'status_code': 429,
             'error_message': 'rate limit exceeded'
         }
     
-    def Dividends(self, public_company_id='', query={}):
+    def Financials(self, equity_id='', query={}):
+        return Financials(self.rate_limiter, self.api_key, self.company_id, self.return_raw)
+    
+    def Dividends(self, equity_id='', query={}):
         with self.rate_limiter:
             query_str = urlencode(query)
-            url = 'https://api.withgraham.io/v1/equities/' + str(public_company_id) + '/dividends'
+            url = 'https://api.withgraham.io/v1/equities/' + str(equity_id) + '/dividends'
             if query_str != '':
                 url += '?' + query_str
             
             r = requests.get(url, headers=self._get_headers(), json=None)
             if r.status_code != 200:
                 return None, {
                     'status_code': r.status_code,
```

## graham/__pycache__/equities.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 25 11:44:26 2023 UTC, .py size: 4757 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,175 +1,228 @@
-00000000: 6f0d 0d0a 0000 0000 1a4a 6f64 9512 0000  o........Jod....
+00000000: 6f0d 0d0a 0000 0000 0b99 7064 3718 0000  o.........pd7...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 2600 0000 6400  .....@...s&...d.
+00000020: 0003 0000 0040 0000 0073 3400 0000 6400  .....@...s4...d.
 00000030: 6401 6c00 5a00 6400 6402 6c01 6d02 5a02  d.l.Z.d.d.l.m.Z.
 00000040: 0100 4700 6403 6404 8400 6404 8302 5a03  ..G.d.d...d...Z.
-00000050: 6401 5300 2905 e900 0000 004e 2901 da09  d.S.)......N)...
-00000060: 7572 6c65 6e63 6f64 6563 0000 0000 0000  urlencodec......
-00000070: 0000 0000 0000 0000 0000 0300 0000 4000  ..............@.
-00000080: 0000 7362 0000 0065 005a 0164 005a 0264  ..sb...e.Z.d.Z.d
-00000090: 1264 0264 0384 015a 0364 0464 0584 005a  .d.d...Z.d.d...Z
-000000a0: 0469 0066 0164 0664 0784 015a 0564 0869  .i.f.d.d...Z.d.i
-000000b0: 0066 0264 0964 0a84 015a 0664 0869 0066  .f.d.d...Z.d.i.f
-000000c0: 0264 0b64 0c84 015a 0764 0869 0066 0264  .d.d...Z.d.i.f.d
-000000d0: 0d64 0e84 015a 0864 0869 0066 0264 0f64  .d...Z.d.i.f.d.d
-000000e0: 1084 015a 0964 1153 0029 13da 0845 7175  ...Z.d.S.)...Equ
-000000f0: 6974 6965 7346 6305 0000 0000 0000 0000  itiesFc.........
-00000100: 0000 0005 0000 0002 0000 0043 0000 0073  ...........C...s
-00000110: 1c00 0000 7c01 7c00 5f00 7c02 7c00 5f01  ....|.|._.|.|._.
-00000120: 7c03 7c00 5f02 7c04 7c00 5f03 6400 5300  |.|._.|.|._.d.S.
-00000130: 2901 4e29 04da 0c72 6174 655f 6c69 6d69  ).N)...rate_limi
-00000140: 7465 72da 0761 7069 5f6b 6579 da0a 636f  ter..api_key..co
-00000150: 6d70 616e 795f 6964 da0a 7265 7475 726e  mpany_id..return
-00000160: 5f72 6177 2905 da04 7365 6c66 7204 0000  _raw)...selfr...
-00000170: 0072 0500 0000 7206 0000 0072 0700 0000  .r....r....r....
-00000180: a900 7209 0000 00fa 3962 7569 6c64 2f62  ..r.....9build/b
-00000190: 6469 7374 2e6d 6163 6f73 782d 3130 2e39  dist.macosx-10.9
-000001a0: 2d75 6e69 7665 7273 616c 322f 6567 672f  -universal2/egg/
-000001b0: 6772 6168 616d 2f65 7175 6974 6965 732e  graham/equities.
-000001c0: 7079 da08 5f5f 696e 6974 5f5f 0500 0000  py..__init__....
-000001d0: 7308 0000 0006 0106 0106 010a 017a 1145  s............z.E
-000001e0: 7175 6974 6965 732e 5f5f 696e 6974 5f5f  quities.__init__
-000001f0: 6301 0000 0000 0000 0000 0000 0001 0000  c...............
-00000200: 0004 0000 0043 0000 0073 1400 0000 6401  .....C...s....d.
-00000210: 7c00 6a00 1700 7c00 6a01 6402 6403 9c03  |.j...|.j.d.d...
-00000220: 5300 2904 4e7a 0742 6561 7265 7220 7a10  S.).Nz.Bearer z.
-00000230: 6170 706c 6963 6174 696f 6e2f 6a73 6f6e  application/json
-00000240: 2903 da0d 4175 7468 6f72 697a 6174 696f  )...Authorizatio
-00000250: 6e5a 0743 6f6d 7061 6e79 7a0c 436f 6e74  nZ.Companyz.Cont
-00000260: 656e 742d 5479 7065 2902 7205 0000 0072  ent-Type).r....r
-00000270: 0600 0000 2901 7208 0000 0072 0900 0000  ....).r....r....
-00000280: 7209 0000 0072 0a00 0000 da0c 5f67 6574  r....r......_get
-00000290: 5f68 6561 6465 7273 0b00 0000 7308 0000  _headers....s...
-000002a0: 0008 0204 0102 0106 fd7a 1545 7175 6974  .........z.Equit
-000002b0: 6965 732e 5f67 6574 5f68 6561 6465 7273  ies._get_headers
-000002c0: 6302 0000 0000 0000 0000 0000 0005 0000  c...............
-000002d0: 0008 0000 0043 0000 0073 c400 0000 7c00  .....C...s....|.
-000002e0: 6a00 8f50 0100 7401 7c01 8301 7d02 6401  j..P..t.|...}.d.
-000002f0: 7d03 7c02 6402 6b03 7214 7c03 6403 7c02  }.|.d.k.r.|.d.|.
-00000300: 1700 3700 7d03 7402 6a03 7c03 7c00 a004  ..7.}.t.j.|.|...
-00000310: a100 6400 6404 8d03 7d04 7c04 6a05 6405  ..d.d...}.|.j.d.
-00000320: 6b03 7234 6400 7c04 6a05 7c04 6a06 6406  k.r4d.|.j.|.j.d.
-00000330: 6407 9c03 6602 5700 0200 6400 0400 0400  d...f.W...d.....
-00000340: 8303 0100 5300 7c00 6a07 7244 7c04 a008  ....S.|.j.rD|...
-00000350: a100 6400 6602 5700 0200 6400 0400 0400  ..d.f.W...d.....
-00000360: 8303 0100 5300 7c04 a008 a100 6408 1900  ....S.|.....d...
-00000370: 6400 6602 5700 0200 6400 0400 0400 8303  d.f.W...d.......
-00000380: 0100 5300 3100 7356 7701 0100 0100 0100  ..S.1.sVw.......
-00000390: 5900 0100 6400 6409 640a 640b 9c02 6602  Y...d.d.d.d...f.
-000003a0: 5300 290c 4e7a 2568 7474 7073 3a2f 2f61  S.).Nz%https://a
-000003b0: 7069 2e77 6974 6867 7261 6861 6d2e 696f  pi.withgraham.io
-000003c0: 2f76 312f 6571 7569 7469 6573 da00 fa01  /v1/equities....
-000003d0: 3fa9 02da 0768 6561 6465 7273 da04 6a73  ?....headers..js
-000003e0: 6f6e e9c8 0000 007a 1766 6169 6c65 6420  on.....z.failed 
-000003f0: 746f 206c 6973 7420 6571 7569 7469 6573  to list equities
-00000400: a903 da0b 7374 6174 7573 5f63 6f64 65da  ....status_code.
-00000410: 0474 6578 74da 0d65 7272 6f72 5f6d 6573  .text..error_mes
-00000420: 7361 6765 5a08 6571 7569 7469 6573 e9ad  sageZ.equities..
-00000430: 0100 00fa 1372 6174 6520 6c69 6d69 7420  .....rate limit 
-00000440: 6578 6365 6564 6564 a902 7215 0000 0072  exceeded..r....r
-00000450: 1700 0000 2909 7204 0000 0072 0200 0000  ....).r....r....
-00000460: da08 7265 7175 6573 7473 da03 6765 7472  ..requests..getr
-00000470: 0d00 0000 7215 0000 0072 1600 0000 7207  ....r....r....r.
-00000480: 0000 0072 1200 0000 2905 7208 0000 00da  ...r....).r.....
-00000490: 0571 7565 7279 da09 7175 6572 795f 7374  .query..query_st
-000004a0: 72da 0375 726c da01 7272 0900 0000 7209  r..url..rr....r.
-000004b0: 0000 0072 0a00 0000 da04 4c69 7374 1200  ...r......List..
-000004c0: 0000 732c 0000 0008 0108 0104 0108 010c  ..s,............
-000004d0: 0114 020a 0102 0104 0104 0102 0106 fd10  ................
-000004e0: f806 0e0a 0110 f10e 1020 f002 1102 0102  ......... ......
-000004f0: 0108 fe7a 0d45 7175 6974 6965 732e 4c69  ...z.Equities.Li
-00000500: 7374 720e 0000 0063 0300 0000 0000 0000  str....c........
-00000510: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
-00000520: 73cc 0000 007c 006a 008f 5401 0074 017c  s....|.j..T..t.|
-00000530: 0283 017d 0364 0174 027c 0183 0117 007d  ...}.d.t.|.....}
-00000540: 047c 0364 026b 0372 187c 0464 037c 0317  .|.d.k.r.|.d.|..
-00000550: 0037 007d 0474 036a 047c 047c 00a0 05a1  .7.}.t.j.|.|....
-00000560: 0064 0064 048d 037d 057c 056a 0664 056b  .d.d...}.|.j.d.k
-00000570: 0372 3864 007c 056a 067c 056a 0764 0664  .r8d.|.j.|.j.d.d
-00000580: 079c 0366 0257 0002 0064 0004 0004 0083  ...f.W...d......
-00000590: 0301 0053 007c 006a 0872 487c 05a0 09a1  ...S.|.j.rH|....
-000005a0: 0064 0066 0257 0002 0064 0004 0004 0083  .d.f.W...d......
-000005b0: 0301 0053 007c 05a0 09a1 0064 0819 0064  ...S.|.....d...d
-000005c0: 0066 0257 0002 0064 0004 0004 0083 0301  .f.W...d........
-000005d0: 0053 0031 0073 5a77 0101 0001 0001 0059  .S.1.sZw.......Y
-000005e0: 0001 0064 0064 0964 0a64 0b9c 0266 0253  ...d.d.d.d...f.S
-000005f0: 0029 0c4e fa26 6874 7470 733a 2f2f 6170  .).N.&https://ap
-00000600: 692e 7769 7468 6772 6168 616d 2e69 6f2f  i.withgraham.io/
-00000610: 7631 2f65 7175 6974 6965 732f 720e 0000  v1/equities/r...
-00000620: 0072 0f00 0000 7210 0000 0072 1300 0000  .r....r....r....
-00000630: fa14 6661 696c 6564 2074 6f20 6765 7420  ..failed to get 
-00000640: 6571 7569 7479 7214 0000 005a 0665 7175  equityr....Z.equ
-00000650: 6974 7972 1800 0000 7219 0000 0072 1a00  ityr....r....r..
-00000660: 0000 a90a 7204 0000 0072 0200 0000 da03  ....r....r......
-00000670: 7374 7272 1b00 0000 721c 0000 0072 0d00  strr....r....r..
-00000680: 0000 7215 0000 0072 1600 0000 7207 0000  ..r....r....r...
-00000690: 0072 1200 0000 a906 7208 0000 005a 1170  .r......r....Z.p
-000006a0: 7562 6c69 635f 636f 6d70 616e 795f 6964  ublic_company_id
-000006b0: 721d 0000 0072 1e00 0000 721f 0000 0072  r....r....r....r
-000006c0: 2000 0000 7209 0000 0072 0900 0000 720a   ...r....r....r.
-000006d0: 0000 00da 0347 6574 2900 0000 732c 0000  .....Get)...s,..
-000006e0: 0008 0108 010c 0108 010c 0114 020a 0102  ................
-000006f0: 0104 0104 0102 0106 fd10 f806 0e0a 0110  ................
-00000700: f10e 1020 f002 1102 0102 0108 fe7a 0c45  ... .........z.E
-00000710: 7175 6974 6965 732e 4765 7463 0300 0000  quities.Getc....
-00000720: 0000 0000 0000 0000 0600 0000 0800 0000  ................
-00000730: 4300 0000 f3d0 0000 007c 006a 008f 5601  C........|.j..V.
-00000740: 0074 017c 0283 017d 0364 0174 027c 0183  .t.|...}.d.t.|..
-00000750: 0117 0064 0217 007d 047c 0364 036b 0372  ...d...}.|.d.k.r
-00000760: 1a7c 0464 047c 0317 0037 007d 0474 036a  .|.d.|...7.}.t.j
-00000770: 047c 047c 00a0 05a1 0064 0064 058d 037d  .|.|.....d.d...}
-00000780: 057c 056a 0664 066b 0372 3a64 007c 056a  .|.j.d.k.r:d.|.j
-00000790: 067c 056a 0764 0764 089c 0366 0257 0002  .|.j.d.d...f.W..
-000007a0: 0064 0004 0004 0083 0301 0053 007c 006a  .d.........S.|.j
-000007b0: 0872 4a7c 05a0 09a1 0064 0066 0257 0002  .rJ|.....d.f.W..
-000007c0: 0064 0004 0004 0083 0301 0053 007c 05a0  .d.........S.|..
-000007d0: 09a1 0064 0919 0064 0066 0257 0002 0064  ...d...d.f.W...d
-000007e0: 0004 0004 0083 0301 0053 0031 0073 5c77  .........S.1.s\w
-000007f0: 0101 0001 0001 0059 0001 0064 0064 0a64  .......Y...d.d.d
-00000800: 0b64 0c9c 0266 0253 0029 0d4e 7222 0000  .d...f.S.).Nr"..
-00000810: 007a 062f 6461 696c 7972 0e00 0000 720f  .z./dailyr....r.
-00000820: 0000 0072 1000 0000 7213 0000 0072 2300  ...r....r....r#.
-00000830: 0000 7214 0000 005a 0e64 6169 6c79 536e  ..r....Z.dailySn
-00000840: 6170 7368 6f74 7372 1800 0000 7219 0000  apshotsr....r...
-00000850: 0072 1a00 0000 7224 0000 0072 2600 0000  .r....r$...r&...
-00000860: 7209 0000 0072 0900 0000 720a 0000 00da  r....r....r.....
-00000870: 0544 6169 6c79 4000 0000 f32c 0000 0008  .Daily@....,....
-00000880: 0108 0110 0108 010c 0114 020a 0102 0104  ................
-00000890: 0104 0102 0106 fd10 f806 0e0a 0110 f10e  ................
-000008a0: 1020 f002 1102 0102 0108 fe7a 0e45 7175  . .........z.Equ
-000008b0: 6974 6965 732e 4461 696c 7963 0300 0000  ities.Dailyc....
-000008c0: 0000 0000 0000 0000 0600 0000 0800 0000  ................
-000008d0: 4300 0000 7228 0000 0029 0d4e 7222 0000  C...r(...).Nr"..
-000008e0: 007a 0b2f 6669 6e61 6e63 6961 6c73 720e  .z./financialsr.
-000008f0: 0000 0072 0f00 0000 7210 0000 0072 1300  ...r....r....r..
-00000900: 0000 7223 0000 0072 1400 0000 5a0a 6669  ..r#...r....Z.fi
-00000910: 6e61 6e63 6961 6c73 7218 0000 0072 1900  nancialsr....r..
-00000920: 0000 721a 0000 0072 2400 0000 7226 0000  ..r....r$...r&..
-00000930: 0072 0900 0000 7209 0000 0072 0a00 0000  .r....r....r....
-00000940: da0a 4669 6e61 6e63 6961 6c73 5700 0000  ..FinancialsW...
-00000950: 722a 0000 007a 1345 7175 6974 6965 732e  r*...z.Equities.
-00000960: 4669 6e61 6e63 6961 6c73 6303 0000 0000  Financialsc.....
-00000970: 0000 0000 0000 0006 0000 0008 0000 0043  ...............C
-00000980: 0000 0072 2800 0000 290d 4e72 2200 0000  ...r(...).Nr"...
-00000990: 7a0a 2f64 6976 6964 656e 6473 720e 0000  z./dividendsr...
-000009a0: 0072 0f00 0000 7210 0000 0072 1300 0000  .r....r....r....
-000009b0: 7223 0000 0072 1400 0000 5a09 6469 7669  r#...r....Z.divi
-000009c0: 6465 6e64 7372 1800 0000 7219 0000 0072  dendsr....r....r
-000009d0: 1a00 0000 7224 0000 0072 2600 0000 7209  ....r$...r&...r.
-000009e0: 0000 0072 0900 0000 720a 0000 00da 0944  ...r....r......D
-000009f0: 6976 6964 656e 6473 6e00 0000 722a 0000  ividendsn...r*..
-00000a00: 007a 1245 7175 6974 6965 732e 4469 7669  .z.Equities.Divi
-00000a10: 6465 6e64 734e 2901 4629 0ada 085f 5f6e  dendsN).F)...__n
-00000a20: 616d 655f 5fda 0a5f 5f6d 6f64 756c 655f  ame__..__module_
-00000a30: 5fda 0c5f 5f71 7561 6c6e 616d 655f 5f72  _..__qualname__r
-00000a40: 0b00 0000 720d 0000 0072 2100 0000 7227  ....r....r!...r'
-00000a50: 0000 0072 2900 0000 722b 0000 0072 2c00  ...r)...r+...r,.
-00000a60: 0000 7209 0000 0072 0900 0000 7209 0000  ..r....r....r...
-00000a70: 0072 0a00 0000 7203 0000 0004 0000 0073  .r....r........s
-00000a80: 1000 0000 0800 0a01 0806 0c07 0e17 0e17  ................
-00000a90: 0e17 1217 7203 0000 0029 0472 1b00 0000  ....r....).r....
-00000aa0: da0c 7572 6c6c 6962 2e70 6172 7365 7202  ..urllib.parser.
-00000ab0: 0000 0072 0300 0000 7209 0000 0072 0900  ...r....r....r..
-00000ac0: 0000 7209 0000 0072 0a00 0000 da08 3c6d  ..r....r......<m
-00000ad0: 6f64 756c 653e 0100 0000 7306 0000 0008  odule>....s.....
-00000ae0: 000c 0112 02                             .....
+00000050: 4700 6405 6406 8400 6406 8302 5a04 6401  G.d.d...d...Z.d.
+00000060: 5300 2907 e900 0000 004e 2901 da09 7572  S.)......N)...ur
+00000070: 6c65 6e63 6f64 6563 0000 0000 0000 0000  lencodec........
+00000080: 0000 0000 0000 0000 0300 0000 4000 0000  ............@...
+00000090: 733a 0000 0065 005a 0164 005a 0264 0c64  s:...e.Z.d.Z.d.d
+000000a0: 0264 0384 015a 0364 0464 0584 005a 0464  .d...Z.d.d...Z.d
+000000b0: 0669 0066 0264 0764 0884 015a 0564 0669  .i.f.d.d...Z.d.i
+000000c0: 0066 0264 0964 0a84 015a 0664 0b53 0029  .f.d.d...Z.d.S.)
+000000d0: 0dda 0a46 696e 616e 6369 616c 7346 6305  ...FinancialsFc.
+000000e0: 0000 0000 0000 0000 0000 0005 0000 0002  ................
+000000f0: 0000 0043 0000 00f3 1c00 0000 7c01 7c00  ...C........|.|.
+00000100: 5f00 7c02 7c00 5f01 7c03 7c00 5f02 7c04  _.|.|._.|.|._.|.
+00000110: 7c00 5f03 6400 5300 a901 4ea9 04da 0c72  |._.d.S...N....r
+00000120: 6174 655f 6c69 6d69 7465 72da 0761 7069  ate_limiter..api
+00000130: 5f6b 6579 da0a 636f 6d70 616e 795f 6964  _key..company_id
+00000140: da0a 7265 7475 726e 5f72 6177 a905 da04  ..return_raw....
+00000150: 7365 6c66 7207 0000 0072 0800 0000 7209  selfr....r....r.
+00000160: 0000 0072 0a00 0000 a900 720d 0000 00fa  ...r......r.....
+00000170: 3962 7569 6c64 2f62 6469 7374 2e6d 6163  9build/bdist.mac
+00000180: 6f73 782d 3130 2e39 2d75 6e69 7665 7273  osx-10.9-univers
+00000190: 616c 322f 6567 672f 6772 6168 616d 2f65  al2/egg/graham/e
+000001a0: 7175 6974 6965 732e 7079 da08 5f5f 696e  quities.py..__in
+000001b0: 6974 5f5f 0500 0000 f308 0000 0006 0106  it__............
+000001c0: 0106 010a 017a 1346 696e 616e 6369 616c  .....z.Financial
+000001d0: 732e 5f5f 696e 6974 5f5f 6301 0000 0000  s.__init__c.....
+000001e0: 0000 0000 0000 0001 0000 0004 0000 0043  ...............C
+000001f0: 0000 00f3 1400 0000 6401 7c00 6a00 1700  ........d.|.j...
+00000200: 7c00 6a01 6402 6403 9c03 5300 a904 4e7a  |.j.d.d...S...Nz
+00000210: 0742 6561 7265 7220 7a10 6170 706c 6963  .Bearer z.applic
+00000220: 6174 696f 6e2f 6a73 6f6e 2903 da0d 4175  ation/json)...Au
+00000230: 7468 6f72 697a 6174 696f 6e5a 0743 6f6d  thorizationZ.Com
+00000240: 7061 6e79 7a0c 436f 6e74 656e 742d 5479  panyz.Content-Ty
+00000250: 7065 a902 7208 0000 0072 0900 0000 a901  pe..r....r......
+00000260: 720c 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+00000270: 0e00 0000 da0c 5f67 6574 5f68 6561 6465  ......_get_heade
+00000280: 7273 0b00 0000 f308 0000 0008 0204 0102  rs..............
+00000290: 0106 fd7a 1746 696e 616e 6369 616c 732e  ...z.Financials.
+000002a0: 5f67 6574 5f68 6561 6465 7273 da00 6303  _get_headers..c.
+000002b0: 0000 0000 0000 0000 0000 0006 0000 0008  ................
+000002c0: 0000 0043 0000 00f3 d000 0000 7c00 6a00  ...C........|.j.
+000002d0: 8f56 0100 7401 7c02 8301 7d03 6401 7402  .V..t.|...}.d.t.
+000002e0: 7c01 8301 1700 6402 1700 7d04 7c03 6403  |.....d...}.|.d.
+000002f0: 6b03 721a 7c04 6404 7c03 1700 3700 7d04  k.r.|.d.|...7.}.
+00000300: 7403 6a04 7c04 7c00 a005 a100 6400 6405  t.j.|.|.....d.d.
+00000310: 8d03 7d05 7c05 6a06 6406 6b03 723a 6400  ..}.|.j.d.k.r:d.
+00000320: 7c05 6a06 7c05 6a07 6407 6408 9c03 6602  |.j.|.j.d.d...f.
+00000330: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
+00000340: 7c00 6a08 724a 7c05 a009 a100 6400 6602  |.j.rJ|.....d.f.
+00000350: 5700 0200 6400 0400 0400 8303 0100 5300  W...d.........S.
+00000360: 7c05 a009 a100 6409 1900 6400 6602 5700  |.....d...d.f.W.
+00000370: 0200 6400 0400 0400 8303 0100 5300 3100  ..d.........S.1.
+00000380: 735c 7701 0100 0100 0100 5900 0100 6400  s\w.......Y...d.
+00000390: 640a 640b 640c 9c02 6602 5300 290d 4efa  d.d.d...f.S.).N.
+000003a0: 2668 7474 7073 3a2f 2f61 7069 2e77 6974  &https://api.wit
+000003b0: 6867 7261 6861 6d2e 696f 2f76 312f 6571  hgraham.io/v1/eq
+000003c0: 7569 7469 6573 2f7a 0b2f 6669 6e61 6e63  uities/z./financ
+000003d0: 6961 6c73 7218 0000 00fa 013f a902 da07  ialsr......?....
+000003e0: 6865 6164 6572 73da 046a 736f 6ee9 c800  headers..json...
+000003f0: 0000 7a23 6661 696c 6564 2074 6f20 6765  ..z#failed to ge
+00000400: 7420 6669 6e61 6e63 6961 6c73 2066 6f72  t financials for
+00000410: 2065 7175 6974 79a9 03da 0b73 7461 7475   equity....statu
+00000420: 735f 636f 6465 da04 7465 7874 da0d 6572  s_code..text..er
+00000430: 726f 725f 6d65 7373 6167 655a 0a66 696e  ror_messageZ.fin
+00000440: 616e 6369 616c 73e9 ad01 0000 fa13 7261  ancials.......ra
+00000450: 7465 206c 696d 6974 2065 7863 6565 6465  te limit exceede
+00000460: 64a9 0272 2100 0000 7223 0000 00a9 0a72  d..r!...r#.....r
+00000470: 0700 0000 7202 0000 00da 0373 7472 da08  ....r......str..
+00000480: 7265 7175 6573 7473 da03 6765 7472 1600  requests..getr..
+00000490: 0000 7221 0000 0072 2200 0000 720a 0000  ..r!...r"...r...
+000004a0: 0072 1e00 0000 a906 720c 0000 00da 0965  .r......r......e
+000004b0: 7175 6974 795f 6964 da05 7175 6572 79da  quity_id..query.
+000004c0: 0971 7565 7279 5f73 7472 da03 7572 6cda  .query_str..url.
+000004d0: 0172 720d 0000 0072 0d00 0000 720e 0000  .rr....r....r...
+000004e0: 00da 0b4c 6973 7453 756d 6d61 7279 1200  ...ListSummary..
+000004f0: 0000 f32c 0000 0008 0108 0110 0108 010c  ...,............
+00000500: 0114 020a 0102 0104 0104 0102 0106 fd10  ................
+00000510: f806 0e0a 0110 f10e 1020 f002 1102 0102  ......... ......
+00000520: 0108 fe7a 1646 696e 616e 6369 616c 732e  ...z.Financials.
+00000530: 4c69 7374 5375 6d6d 6172 7963 0300 0000  ListSummaryc....
+00000540: 0000 0000 0000 0000 0600 0000 0800 0000  ................
+00000550: 4300 0000 7219 0000 0029 0d4e 721a 0000  C...r....).Nr...
+00000560: 007a 152f 6669 6e61 6e63 6961 6c73 2f73  .z./financials/s
+00000570: 6563 2d66 6f72 6d73 7218 0000 0072 1b00  ec-formsr....r..
+00000580: 0000 721c 0000 0072 1f00 0000 7a22 6661  ..r....r....z"fa
+00000590: 696c 6564 2074 6f20 6765 7420 5345 4320  iled to get SEC 
+000005a0: 666f 726d 7320 666f 7220 6571 7569 7479  forms for equity
+000005b0: 7220 0000 005a 0566 6f72 6d73 7224 0000  r ...Z.formsr$..
+000005c0: 0072 2500 0000 7226 0000 0072 2700 0000  .r%...r&...r'...
+000005d0: 722b 0000 0072 0d00 0000 720d 0000 0072  r+...r....r....r
+000005e0: 0e00 0000 da0c 4c69 7374 5345 4346 6f72  ......ListSECFor
+000005f0: 6d73 2900 0000 7232 0000 007a 1746 696e  ms)...r2...z.Fin
+00000600: 616e 6369 616c 732e 4c69 7374 5345 4346  ancials.ListSECF
+00000610: 6f72 6d73 4ea9 0146 2907 da08 5f5f 6e61  ormsN..F)...__na
+00000620: 6d65 5f5f da0a 5f5f 6d6f 6475 6c65 5f5f  me__..__module__
+00000630: da0c 5f5f 7175 616c 6e61 6d65 5f5f 720f  ..__qualname__r.
+00000640: 0000 0072 1600 0000 7231 0000 0072 3300  ...r....r1...r3.
+00000650: 0000 720d 0000 0072 0d00 0000 720d 0000  ..r....r....r...
+00000660: 0072 0e00 0000 7203 0000 0004 0000 0073  .r....r........s
+00000670: 0a00 0000 0800 0a01 0806 0e07 1217 7203  ..............r.
+00000680: 0000 0063 0000 0000 0000 0000 0000 0000  ...c............
+00000690: 0000 0000 0300 0000 4000 0000 7362 0000  ........@...sb..
+000006a0: 0065 005a 0164 005a 0264 1264 0264 0384  .e.Z.d.Z.d.d.d..
+000006b0: 015a 0364 0464 0584 005a 0469 0066 0164  .Z.d.d...Z.i.f.d
+000006c0: 0664 0784 015a 0564 0869 0066 0264 0964  .d...Z.d.i.f.d.d
+000006d0: 0a84 015a 0664 0869 0066 0264 0b64 0c84  ...Z.d.i.f.d.d..
+000006e0: 015a 0764 0869 0066 0264 0d64 0e84 015a  .Z.d.i.f.d.d...Z
+000006f0: 0864 0869 0066 0264 0f64 1084 015a 0964  .d.i.f.d.d...Z.d
+00000700: 1153 0029 13da 0845 7175 6974 6965 7346  .S.)...EquitiesF
+00000710: 6305 0000 0000 0000 0000 0000 0005 0000  c...............
+00000720: 0002 0000 0043 0000 0072 0400 0000 7205  .....C...r....r.
+00000730: 0000 0072 0600 0000 720b 0000 0072 0d00  ...r....r....r..
+00000740: 0000 720d 0000 0072 0e00 0000 720f 0000  ..r....r....r...
+00000750: 0042 0000 0072 1000 0000 7a11 4571 7569  .B...r....z.Equi
+00000760: 7469 6573 2e5f 5f69 6e69 745f 5f63 0100  ties.__init__c..
+00000770: 0000 0000 0000 0000 0000 0100 0000 0400  ................
+00000780: 0000 4300 0000 7211 0000 0072 1200 0000  ..C...r....r....
+00000790: 7214 0000 0072 1500 0000 720d 0000 0072  r....r....r....r
+000007a0: 0d00 0000 720e 0000 0072 1600 0000 4800  ....r....r....H.
+000007b0: 0000 7217 0000 007a 1545 7175 6974 6965  ..r....z.Equitie
+000007c0: 732e 5f67 6574 5f68 6561 6465 7273 6302  s._get_headersc.
+000007d0: 0000 0000 0000 0000 0000 0005 0000 0008  ................
+000007e0: 0000 0043 0000 0073 c400 0000 7c00 6a00  ...C...s....|.j.
+000007f0: 8f50 0100 7401 7c01 8301 7d02 6401 7d03  .P..t.|...}.d.}.
+00000800: 7c02 6402 6b03 7214 7c03 6403 7c02 1700  |.d.k.r.|.d.|...
+00000810: 3700 7d03 7402 6a03 7c03 7c00 a004 a100  7.}.t.j.|.|.....
+00000820: 6400 6404 8d03 7d04 7c04 6a05 6405 6b03  d.d...}.|.j.d.k.
+00000830: 7234 6400 7c04 6a05 7c04 6a06 6406 6407  r4d.|.j.|.j.d.d.
+00000840: 9c03 6602 5700 0200 6400 0400 0400 8303  ..f.W...d.......
+00000850: 0100 5300 7c00 6a07 7244 7c04 a008 a100  ..S.|.j.rD|.....
+00000860: 6400 6602 5700 0200 6400 0400 0400 8303  d.f.W...d.......
+00000870: 0100 5300 7c04 a008 a100 6408 1900 6400  ..S.|.....d...d.
+00000880: 6602 5700 0200 6400 0400 0400 8303 0100  f.W...d.........
+00000890: 5300 3100 7356 7701 0100 0100 0100 5900  S.1.sVw.......Y.
+000008a0: 0100 6400 6409 640a 640b 9c02 6602 5300  ..d.d.d.d...f.S.
+000008b0: 290c 4e7a 2568 7474 7073 3a2f 2f61 7069  ).Nz%https://api
+000008c0: 2e77 6974 6867 7261 6861 6d2e 696f 2f76  .withgraham.io/v
+000008d0: 312f 6571 7569 7469 6573 7218 0000 0072  1/equitiesr....r
+000008e0: 1b00 0000 721c 0000 0072 1f00 0000 7a17  ....r....r....z.
+000008f0: 6661 696c 6564 2074 6f20 6c69 7374 2065  failed to list e
+00000900: 7175 6974 6965 7372 2000 0000 5a08 6571  quitiesr ...Z.eq
+00000910: 7569 7469 6573 7224 0000 0072 2500 0000  uitiesr$...r%...
+00000920: 7226 0000 0029 0972 0700 0000 7202 0000  r&...).r....r...
+00000930: 0072 2900 0000 722a 0000 0072 1600 0000  .r)...r*...r....
+00000940: 7221 0000 0072 2200 0000 720a 0000 0072  r!...r"...r....r
+00000950: 1e00 0000 2905 720c 0000 0072 2d00 0000  ....).r....r-...
+00000960: 722e 0000 0072 2f00 0000 7230 0000 0072  r....r/...r0...r
+00000970: 0d00 0000 720d 0000 0072 0e00 0000 da04  ....r....r......
+00000980: 4c69 7374 4f00 0000 732c 0000 0008 0108  ListO...s,......
+00000990: 0104 0108 010c 0114 020a 0102 0104 0104  ................
+000009a0: 0102 0106 fd10 f806 0e0a 0110 f10e 1020  ............... 
+000009b0: f002 1102 0102 0108 fe7a 0d45 7175 6974  .........z.Equit
+000009c0: 6965 732e 4c69 7374 7218 0000 0063 0300  ies.Listr....c..
+000009d0: 0000 0000 0000 0000 0000 0600 0000 0800  ................
+000009e0: 0000 4300 0000 73cc 0000 007c 006a 008f  ..C...s....|.j..
+000009f0: 5401 0074 017c 0283 017d 0364 0174 027c  T..t.|...}.d.t.|
+00000a00: 0183 0117 007d 047c 0364 026b 0372 187c  .....}.|.d.k.r.|
+00000a10: 0464 037c 0317 0037 007d 0474 036a 047c  .d.|...7.}.t.j.|
+00000a20: 047c 00a0 05a1 0064 0064 048d 037d 057c  .|.....d.d...}.|
+00000a30: 056a 0664 056b 0372 3864 007c 056a 067c  .j.d.k.r8d.|.j.|
+00000a40: 056a 0764 0664 079c 0366 0257 0002 0064  .j.d.d...f.W...d
+00000a50: 0004 0004 0083 0301 0053 007c 006a 0872  .........S.|.j.r
+00000a60: 487c 05a0 09a1 0064 0066 0257 0002 0064  H|.....d.f.W...d
+00000a70: 0004 0004 0083 0301 0053 007c 05a0 09a1  .........S.|....
+00000a80: 0064 0819 0064 0066 0257 0002 0064 0004  .d...d.f.W...d..
+00000a90: 0004 0083 0301 0053 0031 0073 5a77 0101  .......S.1.sZw..
+00000aa0: 0001 0001 0059 0001 0064 0064 0964 0a64  .....Y...d.d.d.d
+00000ab0: 0b9c 0266 0253 0029 0c4e 721a 0000 0072  ...f.S.).Nr....r
+00000ac0: 1800 0000 721b 0000 0072 1c00 0000 721f  ....r....r....r.
+00000ad0: 0000 00fa 1466 6169 6c65 6420 746f 2067  .....failed to g
+00000ae0: 6574 2065 7175 6974 7972 2000 0000 5a06  et equityr ...Z.
+00000af0: 6571 7569 7479 7224 0000 0072 2500 0000  equityr$...r%...
+00000b00: 7226 0000 0072 2700 0000 722b 0000 0072  r&...r'...r+...r
+00000b10: 0d00 0000 720d 0000 0072 0e00 0000 da03  ....r....r......
+00000b20: 4765 7466 0000 0073 2c00 0000 0801 0801  Getf...s,.......
+00000b30: 0c01 0801 0c01 1402 0a01 0201 0401 0401  ................
+00000b40: 0201 06fd 10f8 060e 0a01 10f1 0e10 20f0  .............. .
+00000b50: 0211 0201 0201 08fe 7a0c 4571 7569 7469  ........z.Equiti
+00000b60: 6573 2e47 6574 6303 0000 0000 0000 0000  es.Getc.........
+00000b70: 0000 0006 0000 0008 0000 0043 0000 0072  ...........C...r
+00000b80: 1900 0000 290d 4e72 1a00 0000 7a06 2f64  ....).Nr....z./d
+00000b90: 6169 6c79 7218 0000 0072 1b00 0000 721c  ailyr....r....r.
+00000ba0: 0000 0072 1f00 0000 7a27 6661 696c 6564  ...r....z'failed
+00000bb0: 2074 6f20 6765 7420 6461 696c 7920 736e   to get daily sn
+00000bc0: 6170 7368 6f74 2066 6f72 2065 7175 6974  apshot for equit
+00000bd0: 7972 2000 0000 5a0e 6461 696c 7953 6e61  yr ...Z.dailySna
+00000be0: 7073 686f 7473 7224 0000 0072 2500 0000  pshotsr$...r%...
+00000bf0: 7226 0000 0072 2700 0000 722b 0000 0072  r&...r'...r+...r
+00000c00: 0d00 0000 720d 0000 0072 0e00 0000 da05  ....r....r......
+00000c10: 4461 696c 797d 0000 0072 3200 0000 7a0e  Daily}...r2...z.
+00000c20: 4571 7569 7469 6573 2e44 6169 6c79 6303  Equities.Dailyc.
+00000c30: 0000 0000 0000 0000 0000 0003 0000 0005  ................
+00000c40: 0000 0043 0000 0073 1600 0000 7400 7c00  ...C...s....t.|.
+00000c50: 6a01 7c00 6a02 7c00 6a03 7c00 6a04 8304  j.|.j.|.j.|.j...
+00000c60: 5300 7205 0000 0029 0572 0300 0000 7207  S.r....).r....r.
+00000c70: 0000 0072 0800 0000 7209 0000 0072 0a00  ...r....r....r..
+00000c80: 0000 2903 720c 0000 0072 2c00 0000 722d  ..).r....r,...r-
+00000c90: 0000 0072 0d00 0000 720d 0000 0072 0e00  ...r....r....r..
+00000ca0: 0000 7203 0000 0094 0000 0073 0200 0000  ..r........s....
+00000cb0: 1601 7a13 4571 7569 7469 6573 2e46 696e  ..z.Equities.Fin
+00000cc0: 616e 6369 616c 7363 0300 0000 0000 0000  ancialsc........
+00000cd0: 0000 0000 0600 0000 0800 0000 4300 0000  ............C...
+00000ce0: 7219 0000 0029 0d4e 721a 0000 007a 0a2f  r....).Nr....z./
+00000cf0: 6469 7669 6465 6e64 7372 1800 0000 721b  dividendsr....r.
+00000d00: 0000 0072 1c00 0000 721f 0000 0072 3a00  ...r....r....r:.
+00000d10: 0000 7220 0000 005a 0964 6976 6964 656e  ..r ...Z.dividen
+00000d20: 6473 7224 0000 0072 2500 0000 7226 0000  dsr$...r%...r&..
+00000d30: 0072 2700 0000 722b 0000 0072 0d00 0000  .r'...r+...r....
+00000d40: 720d 0000 0072 0e00 0000 da09 4469 7669  r....r......Divi
+00000d50: 6465 6e64 7397 0000 0072 3200 0000 7a12  dends....r2...z.
+00000d60: 4571 7569 7469 6573 2e44 6976 6964 656e  Equities.Dividen
+00000d70: 6473 4e72 3400 0000 290a 7235 0000 0072  dsNr4...).r5...r
+00000d80: 3600 0000 7237 0000 0072 0f00 0000 7216  6...r7...r....r.
+00000d90: 0000 0072 3900 0000 723b 0000 0072 3c00  ...r9...r;...r<.
+00000da0: 0000 7203 0000 0072 3d00 0000 720d 0000  ..r....r=...r...
+00000db0: 0072 0d00 0000 720d 0000 0072 0e00 0000  .r....r....r....
+00000dc0: 7238 0000 0041 0000 0073 1000 0000 0800  r8...A...s......
+00000dd0: 0a01 0806 0c07 0e17 0e17 0e17 1203 7238  ..............r8
+00000de0: 0000 0029 0572 2900 0000 da0c 7572 6c6c  ...).r).....urll
+00000df0: 6962 2e70 6172 7365 7202 0000 0072 0300  ib.parser....r..
+00000e00: 0000 7238 0000 0072 0d00 0000 720d 0000  ..r8...r....r...
+00000e10: 0072 0d00 0000 720e 0000 00da 083c 6d6f  .r....r......<mo
+00000e20: 6475 6c65 3e01 0000 0073 0800 0000 0800  dule>....s......
+00000e30: 0c01 0e02 123d                           .....=
```

## graham/__pycache__/tables.cpython-310.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu May 25 11:44:31 2023 UTC, .py size: 4364 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1f4a 6f64 0c11 0000  o........Jod....
+00000000: 6f0d 0d0a 0000 0000 6e95 7064 0c11 0000  o.......n.pd....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a01 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 5a00 0000 6500  .....@...sZ...e.
 00000070: 5a01 6400 5a02 6401 6402 8400 5a03 6403  Z.d.Z.d.d...Z.d.
```

