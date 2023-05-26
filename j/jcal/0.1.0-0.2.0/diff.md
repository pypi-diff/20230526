# Comparing `tmp/jcal-0.1.0-py3-none-any.whl.zip` & `tmp/jcal-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
 Zip file size: 7269 bytes, number of entries: 7
 -rw-r--r--  2.0 unx     4695 b- defN 80-Jan-01 00:00 jcal/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 jcal/__main__.py
-?rw-r--r--  2.0 unx       34 b- defN 16-Jan-01 00:00 jcal-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 jcal-0.1.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 jcal-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1364 b- defN 16-Jan-01 00:00 jcal-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      519 b- defN 16-Jan-01 00:00 jcal-0.1.0.dist-info/RECORD
+-rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 jcal-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1364 b- defN 80-Jan-01 00:00 jcal-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 jcal-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       34 b- defN 80-Jan-01 00:00 jcal-0.2.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      519 b- defN 16-Jan-01 00:00 jcal-0.2.0.dist-info/RECORD
 7 files, 17484 bytes uncompressed, 6357 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: jcal/__init__.py
 Comment: 
 
 Filename: jcal/__main__.py
 Comment: 
 
-Filename: jcal-0.1.0.dist-info/entry_points.txt
+Filename: jcal-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: jcal-0.1.0.dist-info/LICENSE
+Filename: jcal-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: jcal-0.1.0.dist-info/WHEEL
+Filename: jcal-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: jcal-0.1.0.dist-info/METADATA
+Filename: jcal-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: jcal-0.1.0.dist-info/RECORD
+Filename: jcal-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `jcal-0.1.0.dist-info/LICENSE` & `jcal-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `jcal-0.1.0.dist-info/METADATA` & `jcal-0.2.0.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: jcal
-Version: 0.1.0
+Version: 0.2.0
 Summary: `jcal` is a package for Japanese holiday.
 Home-page: https://github.com/SaitoTsutomu/jcal
 License: Apache-2.0
 Author: Saito Tsutomu
 Author-email: tsutomu7@hotmail.co.jp
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 1 - Planning
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development
 Description-Content-Type: text/markdown
 
 # jcal
 
 `jcal` is a package for Japanese holiday at 2019-2021.
```

