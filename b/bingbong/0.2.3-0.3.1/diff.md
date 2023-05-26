# Comparing `tmp/bingbong-0.2.3-py3-none-any.whl.zip` & `tmp/bingbong-0.3.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,27 +1,28 @@
-Zip file size: 16805 bytes, number of entries: 25
--rw-r--r--  2.0 unx       54 b- defN 23-May-25 12:44 pingpong/__init__.py
+Zip file size: 17324 bytes, number of entries: 26
+-rw-r--r--  2.0 unx       54 b- defN 23-May-26 00:43 pingpong/__init__.py
 -rw-r--r--  2.0 unx      961 b- defN 23-May-25 09:39 pingpong/alpaca.py
 -rw-r--r--  2.0 unx     1025 b- defN 23-May-25 12:43 pingpong/baize.py
 -rw-r--r--  2.0 unx     1287 b- defN 23-May-25 09:39 pingpong/dolly.py
 -rw-r--r--  2.0 unx      957 b- defN 23-May-25 09:39 pingpong/flan.py
 -rw-r--r--  2.0 unx     5121 b- defN 23-May-25 09:40 pingpong/gradio.py
+-rw-r--r--  2.0 unx     1286 b- defN 23-May-26 00:43 pingpong/group.py
 -rw-r--r--  2.0 unx      958 b- defN 23-May-25 09:39 pingpong/koalpaca.py
 -rw-r--r--  2.0 unx      983 b- defN 23-May-25 09:39 pingpong/mpt.py
 -rw-r--r--  2.0 unx      940 b- defN 23-May-25 09:39 pingpong/os_stablelm.py
 -rw-r--r--  2.0 unx     1696 b- defN 23-May-25 09:39 pingpong/pingpong.py
 -rw-r--r--  2.0 unx      965 b- defN 23-May-25 09:39 pingpong/redpajama.py
 -rw-r--r--  2.0 unx      940 b- defN 23-May-25 09:39 pingpong/stable_vicuna.py
 -rw-r--r--  2.0 unx      917 b- defN 23-May-25 09:39 pingpong/stablelm.py
 -rw-r--r--  2.0 unx      963 b- defN 23-May-25 09:39 pingpong/starchat.py
 -rw-r--r--  2.0 unx     1091 b- defN 23-May-25 09:39 pingpong/vicuna.py
 -rw-r--r--  2.0 unx      173 b- defN 23-May-25 09:39 pingpong/context/__init__.py
 -rw-r--r--  2.0 unx      589 b- defN 23-May-25 09:39 pingpong/context/auto_summary_strategy.py
 -rw-r--r--  2.0 unx      789 b- defN 23-May-25 09:39 pingpong/context/last_window_strategy.py
 -rw-r--r--  2.0 unx      840 b- defN 23-May-25 09:39 pingpong/context/search_window_strategy.py
 -rw-r--r--  2.0 unx      119 b- defN 23-May-25 09:39 pingpong/context/strategy.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-25 12:44 bingbong-0.2.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     3346 b- defN 23-May-25 12:44 bingbong-0.2.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-25 12:44 bingbong-0.2.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        9 b- defN 23-May-25 12:44 bingbong-0.2.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1982 b- defN 23-May-25 12:44 bingbong-0.2.3.dist-info/RECORD
-25 files, 38154 bytes uncompressed, 13621 bytes compressed:  64.3%
+-rw-r--r--  2.0 unx    11357 b- defN 23-May-26 00:44 bingbong-0.3.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3346 b- defN 23-May-26 00:44 bingbong-0.3.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 00:44 bingbong-0.3.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        9 b- defN 23-May-26 00:44 bingbong-0.3.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2056 b- defN 23-May-26 00:44 bingbong-0.3.1.dist-info/RECORD
+26 files, 39514 bytes uncompressed, 14030 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -12,14 +12,17 @@
 
 Filename: pingpong/flan.py
 Comment: 
 
 Filename: pingpong/gradio.py
 Comment: 
 
+Filename: pingpong/group.py
+Comment: 
+
 Filename: pingpong/koalpaca.py
 Comment: 
 
 Filename: pingpong/mpt.py
 Comment: 
 
 Filename: pingpong/os_stablelm.py
@@ -54,23 +57,23 @@
 
 Filename: pingpong/context/search_window_strategy.py
 Comment: 
 
 Filename: pingpong/context/strategy.py
 Comment: 
 
-Filename: bingbong-0.2.3.dist-info/LICENSE
+Filename: bingbong-0.3.1.dist-info/LICENSE
 Comment: 
 
-Filename: bingbong-0.2.3.dist-info/METADATA
+Filename: bingbong-0.3.1.dist-info/METADATA
 Comment: 
 
-Filename: bingbong-0.2.3.dist-info/WHEEL
+Filename: bingbong-0.3.1.dist-info/WHEEL
 Comment: 
 
-Filename: bingbong-0.2.3.dist-info/top_level.txt
+Filename: bingbong-0.3.1.dist-info/top_level.txt
 Comment: 
 
-Filename: bingbong-0.2.3.dist-info/RECORD
+Filename: bingbong-0.3.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pingpong/__init__.py

```diff
@@ -1,3 +1,3 @@
-__version__ = '0.2.3'
+__version__ = '0.3.1'
 
 from .pingpong import PingPong
```

## Comparing `bingbong-0.2.3.dist-info/LICENSE` & `bingbong-0.3.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `bingbong-0.2.3.dist-info/METADATA` & `bingbong-0.3.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingbong
-Version: 0.2.3
+Version: 0.3.1
 Summary: Ping pong management library for LLM applied application
 Home-page: https://github.com/deep-diver/PingPong
 Author: chansung park
 Author-email: deep.diver.csp@gmail.com
 Keywords: LLM,pingpong,prompt,context,management
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

## Comparing `bingbong-0.2.3.dist-info/RECORD` & `bingbong-0.3.1.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
-pingpong/__init__.py,sha256=TVtlyQWirSshMApPZ3YNsZWPSG3XXa4jbwgg_eaehxE,54
+pingpong/__init__.py,sha256=qNjHzmyLbJQwhCuz2purV43gAXg3CPPlz_mDht9KUUQ,54
 pingpong/alpaca.py,sha256=adfuI8gOqREf1P29hXjPMezUSBZOec_eTY82UrjpYnQ,961
 pingpong/baize.py,sha256=xIATn7vaplZyxKjfPerXkyL5V-WfhT5hJqwGVufalGM,1025
 pingpong/dolly.py,sha256=vMbHiwgeewzRAsruuMVnQc2w3KEKhWJUdOmaBbyazQo,1287
 pingpong/flan.py,sha256=5sjdGDva_d1ZtynkPmXPV2WDB3W1IYWzhrlsK6y5wgc,957
 pingpong/gradio.py,sha256=1PK3RzYdlWda3sWLV9sgPhFqCuyzlzFCb4s-7KBqfGg,5121
+pingpong/group.py,sha256=KE4WPF5kpQxogEFO-cA7Jilt9fKsg59R-FcOkLNTDg8,1286
 pingpong/koalpaca.py,sha256=tjpWeCslo2RoOC9hlgaFD3QF7uRSk2hFeOxXb86FocQ,958
 pingpong/mpt.py,sha256=y65bsfaMTu8McMGvYjiBpSo5pgy3zxx12G9cKc_jAjg,983
 pingpong/os_stablelm.py,sha256=UQD9WcLsIVNml5Q9kVIDSWTRrw5_fJHpdZuujCmORpY,940
 pingpong/pingpong.py,sha256=LnareHdYTXvVQ4qT38hiFIGqRCUruWK3fvIC9tdoQW0,1696
 pingpong/redpajama.py,sha256=a537Nb6R4LfX063EtDXqVwKDQUQQIs7KkFG9cVMnOrY,965
 pingpong/stable_vicuna.py,sha256=GtwmumYBwbvcLHopfcLW2xQ5HkMUJN1cWCshtddQqHk,940
 pingpong/stablelm.py,sha256=JryIrvcTxYVqQGv4pHVqM3fLdkLG4PUR8AXD0zZi3FI,917
 pingpong/starchat.py,sha256=VoRm2ND5Ivej-H2-o7qWfdJP9DEFR2fLUoqINHaJ8Lg,963
 pingpong/vicuna.py,sha256=wp_XPw20Gz5k8N6INAy6nOypfxrv4xm8bn6wV8pu5vU,1091
 pingpong/context/__init__.py,sha256=ksYP7nq8inYK7SHDwpd7Hs_h87gPKdP9Ac6E5w0X6zM,173
 pingpong/context/auto_summary_strategy.py,sha256=s2lrlGKzLFNBGdLMAkaC6d2VY8aJSdgtrwa_Rvmt3Fc,589
 pingpong/context/last_window_strategy.py,sha256=JN7pFDD2C8nGMUx-H3aHNQrXCT0E0S-FlBunOrQGX-w,789
 pingpong/context/search_window_strategy.py,sha256=OPd2xxiI9FrzU4w2R5luaDEKiNEj4KYr_EF53Qi6l_Q,840
 pingpong/context/strategy.py,sha256=xGoy7T92gYubrwekz0Kz2Vxv10njgXG44K48bC9BqAU,119
-bingbong-0.2.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-bingbong-0.2.3.dist-info/METADATA,sha256=PmDlp1D0CEyTYqGKDRz6cxk7irPOa8v7BNveIpGfQ_g,3346
-bingbong-0.2.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-bingbong-0.2.3.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
-bingbong-0.2.3.dist-info/RECORD,,
+bingbong-0.3.1.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+bingbong-0.3.1.dist-info/METADATA,sha256=JzAn_oMU0ZgNCIyNdW4fkMRYGAuo3heS7uN4eKf9GMY,3346
+bingbong-0.3.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+bingbong-0.3.1.dist-info/top_level.txt,sha256=gEn53k5ARNLZodzDYx4bPsQ-F69t7ln5s4vJGgc3dgo,9
+bingbong-0.3.1.dist-info/RECORD,,
```

