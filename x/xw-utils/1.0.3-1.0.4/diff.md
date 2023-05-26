# Comparing `tmp/xw_utils-1.0.3-cp39-cp39-win_amd64.whl.zip` & `tmp/xw_utils-1.0.4-cp39-cp39-musllinux_1_1_aarch64.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,12 @@
-Zip file size: 62558 bytes, number of entries: 6
--rw-rw-rw-  2.0 fat   145408 b- defN 23-May-25 07:21 xw_utils.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 fat     2182 b- defN 23-May-25 07:21 xw_utils-1.0.3.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      296 b- defN 23-May-25 07:21 xw_utils-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-May-25 07:21 xw_utils-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        9 b- defN 23-May-25 07:21 xw_utils-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      476 b- defN 23-May-25 07:21 xw_utils-1.0.3.dist-info/RECORD
-6 files, 148471 bytes uncompressed, 61698 bytes compressed:  58.4%
+Zip file size: 602476 bytes, number of entries: 10
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 04:11 xw_utils-1.0.4.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-26 04:11 xw_utils.libs/
+-rwxr-xr-x  2.0 unx   334345 b- defN 23-May-26 04:11 xw_utils.cpython-39-aarch64-linux-gnu.so
+-rw-rw-r--  2.0 unx      694 b- defN 23-May-26 04:11 xw_utils-1.0.4.dist-info/RECORD
+-rw-r--r--  2.0 unx        9 b- defN 23-May-26 04:11 xw_utils-1.0.4.dist-info/top_level.txt
+-rw-r--r--  2.0 unx      283 b- defN 23-May-26 04:11 xw_utils-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      112 b- defN 23-May-26 04:11 xw_utils-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx     2182 b- defN 23-May-26 04:11 xw_utils-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx   134393 b- defN 23-May-26 04:11 xw_utils.libs/libgcc_s-4e37474d.so.1
+-rwxr-xr-x  2.0 unx  2599041 b- defN 23-May-26 04:11 xw_utils.libs/libstdc++-fd9f4683.so.6.0.28
+10 files, 3071059 bytes uncompressed, 601052 bytes compressed:  80.4%
```

## zipnote {}

```diff
@@ -1,19 +1,31 @@
-Filename: xw_utils.cp39-win_amd64.pyd
+Filename: xw_utils-1.0.4.dist-info/
 Comment: 
 
-Filename: xw_utils-1.0.3.dist-info/LICENSE
+Filename: xw_utils.libs/
 Comment: 
 
-Filename: xw_utils-1.0.3.dist-info/METADATA
+Filename: xw_utils.cpython-39-aarch64-linux-gnu.so
 Comment: 
 
-Filename: xw_utils-1.0.3.dist-info/WHEEL
+Filename: xw_utils-1.0.4.dist-info/RECORD
 Comment: 
 
-Filename: xw_utils-1.0.3.dist-info/top_level.txt
+Filename: xw_utils-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xw_utils-1.0.3.dist-info/RECORD
+Filename: xw_utils-1.0.4.dist-info/METADATA
+Comment: 
+
+Filename: xw_utils-1.0.4.dist-info/WHEEL
+Comment: 
+
+Filename: xw_utils-1.0.4.dist-info/LICENSE
+Comment: 
+
+Filename: xw_utils.libs/libgcc_s-4e37474d.so.1
+Comment: 
+
+Filename: xw_utils.libs/libstdc++-fd9f4683.so.6.0.28
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `xw_utils-1.0.3.dist-info/LICENSE` & `xw_utils-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

