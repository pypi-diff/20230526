# Comparing `tmp/jawasCalcul-0.1-py3-none-any.whl.zip` & `tmp/jawasCalcul-0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2112 bytes, number of entries: 6
--rw-r--r--  2.0 unx       28 b- defN 23-May-26 07:18 jawasCalcul/__init__.py
--rw-rw-r--  2.0 unx     1053 b- defN 23-May-26 07:20 jawasCalcul-0.1.dist-info/LICENSE.TXT
--rw-r--r--  2.0 unx      291 b- defN 23-May-26 07:20 jawasCalcul-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 07:20 jawasCalcul-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-26 07:20 jawasCalcul-0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      477 b- defN 23-May-26 07:20 jawasCalcul-0.1.dist-info/RECORD
-6 files, 1953 bytes uncompressed, 1242 bytes compressed:  36.4%
+Zip file size: 2150 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       82 b- defN 23-May-26 08:10 jawasCalcul/__init__.py
+-rw-rw-r--  2.0 unx     1053 b- defN 23-May-26 08:10 jawasCalcul-0.2.dist-info/LICENSE.TXT
+-rw-r--r--  2.0 unx      291 b- defN 23-May-26 08:10 jawasCalcul-0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 08:10 jawasCalcul-0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-26 08:10 jawasCalcul-0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      477 b- defN 23-May-26 08:10 jawasCalcul-0.2.dist-info/RECORD
+6 files, 2007 bytes uncompressed, 1280 bytes compressed:  36.2%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: jawasCalcul/__init__.py
 Comment: 
 
-Filename: jawasCalcul-0.1.dist-info/LICENSE.TXT
+Filename: jawasCalcul-0.2.dist-info/LICENSE.TXT
 Comment: 
 
-Filename: jawasCalcul-0.1.dist-info/METADATA
+Filename: jawasCalcul-0.2.dist-info/METADATA
 Comment: 
 
-Filename: jawasCalcul-0.1.dist-info/WHEEL
+Filename: jawasCalcul-0.2.dist-info/WHEEL
 Comment: 
 
-Filename: jawasCalcul-0.1.dist-info/top_level.txt
+Filename: jawasCalcul-0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: jawasCalcul-0.1.dist-info/RECORD
+Filename: jawasCalcul-0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## jawasCalcul/__init__.py

```diff
@@ -1,2 +1,7 @@
 def add(a,b):
-    return a+b
+    return a+b
+
+input("enter the num")
+
+def sub(a,b):
+    return a-b
```

## Comparing `jawasCalcul-0.1.dist-info/LICENSE.TXT` & `jawasCalcul-0.2.dist-info/LICENSE.TXT`

 * *Files identical despite different names*

