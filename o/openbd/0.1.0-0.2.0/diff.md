# Comparing `tmp/openbd-0.1.0-py3-none-any.whl.zip` & `tmp/openbd-0.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7440 bytes, number of entries: 7
+Zip file size: 7439 bytes, number of entries: 7
 -rw-r--r--  2.0 unx     3673 b- defN 80-Jan-01 00:00 openbd/__init__.py
 -rw-r--r--  2.0 unx       27 b- defN 80-Jan-01 00:00 openbd/__main__.py
-?rw-r--r--  2.0 unx       38 b- defN 16-Jan-01 00:00 openbd-0.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 openbd-0.1.0.dist-info/LICENSE
-?rw-r--r--  2.0 unx       88 b- defN 16-Jan-01 00:00 openbd-0.1.0.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1389 b- defN 16-Jan-01 00:00 openbd-0.1.0.dist-info/METADATA
-?rw-r--r--  2.0 unx      533 b- defN 16-Jan-01 00:00 openbd-0.1.0.dist-info/RECORD
-7 files, 16505 bytes uncompressed, 6500 bytes compressed:  60.6%
+-rw-r--r--  2.0 unx    10757 b- defN 80-Jan-01 00:00 openbd-0.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1389 b- defN 80-Jan-01 00:00 openbd-0.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 openbd-0.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       38 b- defN 80-Jan-01 00:00 openbd-0.2.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      533 b- defN 16-Jan-01 00:00 openbd-0.2.0.dist-info/RECORD
+7 files, 16505 bytes uncompressed, 6499 bytes compressed:  60.6%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: openbd/__init__.py
 Comment: 
 
 Filename: openbd/__main__.py
 Comment: 
 
-Filename: openbd-0.1.0.dist-info/entry_points.txt
+Filename: openbd-0.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: openbd-0.1.0.dist-info/LICENSE
+Filename: openbd-0.2.0.dist-info/METADATA
 Comment: 
 
-Filename: openbd-0.1.0.dist-info/WHEEL
+Filename: openbd-0.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: openbd-0.1.0.dist-info/METADATA
+Filename: openbd-0.2.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: openbd-0.1.0.dist-info/RECORD
+Filename: openbd-0.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `openbd-0.1.0.dist-info/LICENSE` & `openbd-0.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `openbd-0.1.0.dist-info/METADATA` & `openbd-0.2.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: openbd
-Version: 0.1.0
+Version: 0.2.0
 Summary: `openbd` is a package for openBD( https://openbd.jp/ ).
 Home-page: https://github.com/SaitoTsutomu/openbd
 License: Apache-2.0
 Author: SaitoTsutomu
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
 
 # openbd
 
 `openbd` is a package for openBD( https://openbd.jp/ ).
```

## Comparing `openbd-0.1.0.dist-info/RECORD` & `openbd-0.2.0.dist-info/RECORD`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 openbd/__init__.py,sha256=idlp9dV5P9atT_VTgTi5T-scN6ry-vsvgre6Irgg_UQ,3673
 openbd/__main__.py,sha256=ubt6XyZvcHwdjCQ90B_U4MeP-3YJduz5GWUC9yOgkrg,27
-openbd-0.1.0.dist-info/entry_points.txt,sha256=FUiDzgOotueC_Pzx0jPpC83NubgTMa1NglUINqSFBNU,38
-openbd-0.1.0.dist-info/LICENSE,sha256=P4wG11QaWXFTeHpKANPvc83droyjtsKJwzCAbzqFscA,10757
-openbd-0.1.0.dist-info/WHEEL,sha256=gSF7fibx4crkLz_A-IKR6kcuq0jJ64KNCkG8_bcaEao,88
-openbd-0.1.0.dist-info/METADATA,sha256=ZUrrF2tOvgmnigLR_U7e9DdXNLHG0_B7W2qizVeg4ns,1389
-openbd-0.1.0.dist-info/RECORD,,
+openbd-0.2.0.dist-info/LICENSE,sha256=P4wG11QaWXFTeHpKANPvc83droyjtsKJwzCAbzqFscA,10757
+openbd-0.2.0.dist-info/METADATA,sha256=t5nn7Yd_h7vgWbPF32dtySvsOCMyMes8ui61JburG08,1389
+openbd-0.2.0.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+openbd-0.2.0.dist-info/entry_points.txt,sha256=FUiDzgOotueC_Pzx0jPpC83NubgTMa1NglUINqSFBNU,38
+openbd-0.2.0.dist-info/RECORD,,
```

