# Comparing `tmp/PyScalapack-0.3.5-py3-none-any.whl.zip` & `tmp/PyScalapack-0.3.6-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6302 bytes, number of entries: 5
--rw-r--r--  2.0 unx    14724 b- defN 23-Apr-01 11:57 PyScalapack/__init__.py
--rw-r--r--  2.0 unx     3818 b- defN 23-Apr-01 11:57 PyScalapack-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Apr-01 11:57 PyScalapack-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-Apr-01 11:57 PyScalapack-0.3.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      395 b- defN 23-Apr-01 11:57 PyScalapack-0.3.5.dist-info/RECORD
-5 files, 19041 bytes uncompressed, 5566 bytes compressed:  70.8%
+Zip file size: 6285 bytes, number of entries: 5
+-rw-r--r--  2.0 unx    14724 b- defN 23-May-26 16:06 PyScalapack/__init__.py
+-rw-r--r--  2.0 unx     3798 b- defN 23-May-26 16:06 PyScalapack-0.3.6.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 16:06 PyScalapack-0.3.6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-26 16:06 PyScalapack-0.3.6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      395 b- defN 23-May-26 16:06 PyScalapack-0.3.6.dist-info/RECORD
+5 files, 19021 bytes uncompressed, 5549 bytes compressed:  70.8%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: PyScalapack/__init__.py
 Comment: 
 
-Filename: PyScalapack-0.3.5.dist-info/METADATA
+Filename: PyScalapack-0.3.6.dist-info/METADATA
 Comment: 
 
-Filename: PyScalapack-0.3.5.dist-info/WHEEL
+Filename: PyScalapack-0.3.6.dist-info/WHEEL
 Comment: 
 
-Filename: PyScalapack-0.3.5.dist-info/top_level.txt
+Filename: PyScalapack-0.3.6.dist-info/top_level.txt
 Comment: 
 
-Filename: PyScalapack-0.3.5.dist-info/RECORD
+Filename: PyScalapack-0.3.6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `PyScalapack-0.3.5.dist-info/METADATA` & `PyScalapack-0.3.6.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: PyScalapack
-Version: 0.3.5
+Version: 0.3.6
 Summary: python wrapper for scalapack
 Home-page: https://github.com/USTC-TNS/TAT/tree/TAT/PyScalapack
 Author: Hao Zhang
 Author-email: zh970205@mail.ustc.edu.cn
 License: GPLv3
-Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 
 
 # PyScalapack
 
@@ -137,9 +136,7 @@
     
     print(scalapack.pdgemm)
     print(scalapack.pgemm["D"])
 
     <function Scalapack._fortran_function.<locals>.result at 0x7f0a0a35dbd0>
     <function Scalapack._fortran_function.<locals>.result at 0x7f0a0a35dbd0>
 
-
-
```

