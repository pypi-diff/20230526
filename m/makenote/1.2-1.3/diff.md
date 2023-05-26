# Comparing `tmp/makenote-1.2-py3-none-any.whl.zip` & `tmp/makenote-1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 17379 bytes, number of entries: 7
--rw-rw-r--  2.0 unx       20 b- defN 23-May-25 11:55 makenote/__init__.py
--rwxrwxr-x  2.0 unx     8459 b- defN 23-May-25 11:57 makenote-1.2.data/scripts/makenote
--rw-rw-r--  2.0 unx    35099 b- defN 23-May-25 11:57 makenote-1.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3046 b- defN 23-May-25 11:57 makenote-1.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-25 11:57 makenote-1.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx        9 b- defN 23-May-25 11:57 makenote-1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      547 b- defN 23-May-25 11:57 makenote-1.2.dist-info/RECORD
-7 files, 47272 bytes uncompressed, 16409 bytes compressed:  65.3%
+Zip file size: 17362 bytes, number of entries: 7
+-rw-rw-r--  2.0 unx       20 b- defN 23-May-26 10:04 makenote/__init__.py
+-rwxrwxr-x  2.0 unx     8459 b- defN 23-May-26 10:04 makenote-1.3.data/scripts/makenote
+-rw-rw-r--  2.0 unx    35099 b- defN 23-May-26 10:04 makenote-1.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3022 b- defN 23-May-26 10:04 makenote-1.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 10:04 makenote-1.3.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        9 b- defN 23-May-26 10:04 makenote-1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      547 b- defN 23-May-26 10:04 makenote-1.3.dist-info/RECORD
+7 files, 47248 bytes uncompressed, 16392 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: makenote/__init__.py
 Comment: 
 
-Filename: makenote-1.2.data/scripts/makenote
+Filename: makenote-1.3.data/scripts/makenote
 Comment: 
 
-Filename: makenote-1.2.dist-info/LICENSE
+Filename: makenote-1.3.dist-info/LICENSE
 Comment: 
 
-Filename: makenote-1.2.dist-info/METADATA
+Filename: makenote-1.3.dist-info/METADATA
 Comment: 
 
-Filename: makenote-1.2.dist-info/WHEEL
+Filename: makenote-1.3.dist-info/WHEEL
 Comment: 
 
-Filename: makenote-1.2.dist-info/top_level.txt
+Filename: makenote-1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: makenote-1.2.dist-info/RECORD
+Filename: makenote-1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## makenote/__init__.py

```diff
@@ -1 +1 @@
-__version__ = "1.2"
+__version__ = "1.3"
```

## Comparing `makenote-1.2.data/scripts/makenote` & `makenote-1.3.data/scripts/makenote`

 * *Files identical despite different names*

## Comparing `makenote-1.2.dist-info/LICENSE` & `makenote-1.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `makenote-1.2.dist-info/METADATA` & `makenote-1.3.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: makenote
-Version: 1.2
+Version: 1.3
 Summary: command line tool for quickly writing journals
 Home-page: https://github.com/ekm507/makenote
 Author: Erfan Kheirollahi
 Author-email: ekm507@gmail.com
 License: UNKNOWN
 Keywords: makenote
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: argparse
 
 [نسخه فارسی این سند](./fa.README.md)
 
 makenote
 ---
 
 a command line tool for making diary or journals.
```

