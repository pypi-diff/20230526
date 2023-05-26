# Comparing `tmp/range_digit-0.0.4-py3-none-any.whl.zip` & `tmp/range_digit-0.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 3194 bytes, number of entries: 5
+Zip file size: 3198 bytes, number of entries: 5
 -rw-r--r--  2.0 unx     4678 b- defN 80-Jan-01 00:00 range_digit/__init__.py
--rw-r--r--  2.0 unx     1070 b- defN 80-Jan-01 00:00 range_digit-0.0.4.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 range_digit-0.0.4.dist-info/WHEEL
-?rw-r--r--  2.0 unx      923 b- defN 16-Jan-01 00:00 range_digit-0.0.4.dist-info/METADATA
-?rw-r--r--  2.0 unx      389 b- defN 16-Jan-01 00:00 range_digit-0.0.4.dist-info/RECORD
-5 files, 7143 bytes uncompressed, 2470 bytes compressed:  65.4%
+-rw-r--r--  2.0 unx     1070 b- defN 80-Jan-01 00:00 range_digit-0.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      875 b- defN 80-Jan-01 00:00 range_digit-0.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 range_digit-0.1.0.dist-info/WHEEL
+?rw-r--r--  2.0 unx      389 b- defN 16-Jan-01 00:00 range_digit-0.1.0.dist-info/RECORD
+5 files, 7100 bytes uncompressed, 2474 bytes compressed:  65.2%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: range_digit/__init__.py
 Comment: 
 
-Filename: range_digit-0.0.4.dist-info/LICENSE
+Filename: range_digit-0.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: range_digit-0.0.4.dist-info/WHEEL
+Filename: range_digit-0.1.0.dist-info/METADATA
 Comment: 
 
-Filename: range_digit-0.0.4.dist-info/METADATA
+Filename: range_digit-0.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: range_digit-0.0.4.dist-info/RECORD
+Filename: range_digit-0.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `range_digit-0.0.4.dist-info/LICENSE` & `range_digit-0.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `range_digit-0.0.4.dist-info/METADATA` & `range_digit-0.1.0.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 Metadata-Version: 2.1
 Name: range-digit
-Version: 0.0.4
+Version: 0.1.0
 Summary: 
 Home-page: https://github.com/SaitoTsutomu/range-digit
 License: MIT
 Author: SaitoTsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 
 ## description
 
 `range-digit` is library of decimal digit which has `low` and `sup`.
```

