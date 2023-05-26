# Comparing `tmp/tnsp_bridge-0.3.5-py3-none-any.whl.zip` & `tmp/tnsp_bridge-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3195 bytes, number of entries: 5
--rw-r--r--  2.0 unx     5657 b- defN 23-Apr-01 11:56 bridge/__init__.py
--rw-r--r--  2.0 unx      692 b- defN 23-Apr-01 11:57 tnsp_bridge-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-01 11:57 tnsp_bridge-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 23-Apr-01 11:57 tnsp_bridge-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      387 b- defN 23-Apr-01 11:57 tnsp_bridge-0.3.5.dist-info/RECORD
-5 files, 6835 bytes uncompressed, 2469 bytes compressed:  63.9%
+Zip file size: 3180 bytes, number of entries: 5
+-rw-r--r--  2.0 unx     5657 b- defN 23-May-26 16:06 bridge/__init__.py
+-rw-r--r--  2.0 unx      672 b- defN 23-May-26 16:06 tnsp_bridge-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 16:06 tnsp_bridge-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 23-May-26 16:06 tnsp_bridge-0.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      387 b- defN 23-May-26 16:06 tnsp_bridge-0.3.6.dist-info/RECORD
+5 files, 6815 bytes uncompressed, 2454 bytes compressed:  64.0%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: bridge/__init__.py
 Comment: 
 
-Filename: tnsp_bridge-0.3.5.dist-info/METADATA
+Filename: tnsp_bridge-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: tnsp_bridge-0.3.5.dist-info/WHEEL
+Filename: tnsp_bridge-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: tnsp_bridge-0.3.5.dist-info/top_level.txt
+Filename: tnsp_bridge-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: tnsp_bridge-0.3.5.dist-info/RECORD
+Filename: tnsp_bridge-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `tnsp_bridge-0.3.5.dist-info/METADATA` & `tnsp_bridge-0.3.6.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 Metadata-Version: 2.1
 Name: tnsp-bridge
-Version: 0.3.5
+Version: 0.3.6
 Summary: bridge from TNSP to TAT
 Home-page: https://github.com/USTC-TNS/TAT/tree/TAT/tnsp_bridge
 Author: Hao Zhang
 Author-email: zh970205@mail.ustc.edu.cn
 License: GPLv3
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
-Requires-Dist: PyTAT (==0.3.5)
+Requires-Dist: PyTAT (==0.3.6)
 
 
 
 # tnsp-bridge
 
 tnsp-bridge is a small tool to convert tensor data from [tnsp](https://www.sciencedirect.com/science/article/pii/S001046551830078X) format to TAT format.
 
 The formats of TNSP between versions often vary, and this subprocject only works for TNSP 4.0.2.
 Since this subprocject is used in rare case, it will not be documented currently.
 
-
-
```

