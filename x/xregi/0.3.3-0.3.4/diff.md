# Comparing `tmp/xregi-0.3.3-py3-none-any.whl.zip` & `tmp/xregi-0.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 53065 bytes, number of entries: 29
+Zip file size: 53068 bytes, number of entries: 29
 -rw-rw-r--  2.0 unx      217 b- defN 23-May-26 15:44 xregi/__init__.py
 -rw-rw-r--  2.0 unx     1502 b- defN 23-May-26 15:44 xregi/__main__.py
 -rw-rw-r--  2.0 unx     1231 b- defN 23-May-26 15:44 xregi/args.py
 -rw-rw-r--  2.0 unx     1795 b- defN 23-May-26 15:44 xregi/config.py
 -rw-rw-r--  2.0 unx    12557 b- defN 23-May-26 15:44 xregi/landmark_container.py
 -rw-rw-r--  2.0 unx     9906 b- defN 23-May-26 15:44 xregi/landmark_detector.py
 -rw-rw-r--  2.0 unx     3848 b- defN 23-May-26 15:44 xregi/registration_2d_3d.py
@@ -19,13 +19,13 @@
 -rw-rw-r--  2.0 unx     6217 b- defN 23-May-08 23:35 xregi/synthex/test_ensemble.py
 -rw-rw-r--  2.0 unx    11437 b- defN 23-May-26 15:44 xregi/synthex/util.py
 -rw-rw-r--  2.0 unx        0 b- defN 23-May-26 15:44 xregi/synthex/TransUNet/__init__.py
 -rw-rw-r--  2.0 unx    29577 b- defN 23-May-26 15:44 xregi/synthex/TransUNet/transunet.py
 -rw-rw-r--  2.0 unx     4297 b- defN 23-May-26 15:44 xregi/synthex/TransUNet/vit_seg_configs.py
 -rw-rw-r--  2.0 unx    17634 b- defN 23-May-26 15:44 xregi/synthex/TransUNet/vit_seg_modeling.py
 -rw-rw-r--  2.0 unx     6250 b- defN 23-May-26 15:44 xregi/synthex/TransUNet/vit_seg_modeling_resnet_skip.py
--rw-rw-r--  2.0 unx     1070 b- defN 23-May-26 19:52 xregi-0.3.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     4273 b- defN 23-May-26 19:52 xregi-0.3.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-26 19:52 xregi-0.3.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx        6 b- defN 23-May-26 19:52 xregi-0.3.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     2376 b- defN 23-May-26 19:52 xregi-0.3.3.dist-info/RECORD
-29 files, 209522 bytes uncompressed, 49277 bytes compressed:  76.5%
+-rw-rw-r--  2.0 unx     1070 b- defN 23-May-26 19:59 xregi-0.3.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     4278 b- defN 23-May-26 19:59 xregi-0.3.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-26 19:59 xregi-0.3.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx        6 b- defN 23-May-26 19:59 xregi-0.3.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     2376 b- defN 23-May-26 19:59 xregi-0.3.4.dist-info/RECORD
+29 files, 209527 bytes uncompressed, 49280 bytes compressed:  76.5%
```

## zipnote {}

```diff
@@ -66,23 +66,23 @@
 
 Filename: xregi/synthex/TransUNet/vit_seg_modeling.py
 Comment: 
 
 Filename: xregi/synthex/TransUNet/vit_seg_modeling_resnet_skip.py
 Comment: 
 
-Filename: xregi-0.3.3.dist-info/LICENSE
+Filename: xregi-0.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: xregi-0.3.3.dist-info/METADATA
+Filename: xregi-0.3.4.dist-info/METADATA
 Comment: 
 
-Filename: xregi-0.3.3.dist-info/WHEEL
+Filename: xregi-0.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: xregi-0.3.3.dist-info/top_level.txt
+Filename: xregi-0.3.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xregi-0.3.3.dist-info/RECORD
+Filename: xregi-0.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `xregi-0.3.3.dist-info/LICENSE` & `xregi-0.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `xregi-0.3.3.dist-info/METADATA` & `xregi-0.3.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: xregi
-Version: 0.3.3
+Version: 0.3.4
 Summary: A package for automatic 2D/3D registration of X-ray and CT images
 Home-page: https://github.com/shez12/xregi
 Download-URL: 
 Author: Jiaming Zhang
 Author-email: jzhan282@jhu.edu
 License: MIT
-Description-Content-Type: markdown
+Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: h5py (>=3.7.0)
 Requires-Dist: imgaug (>=0.4.0)
 Requires-Dist: matplotlib (>=3.5.2)
 Requires-Dist: ml-collections (>=0.1.1)
 Requires-Dist: numpy (>=1.24.2)
 Requires-Dist: opencv-python (>=4.6.0.66)
```

### html2text {}

```diff
@@ -1,17 +1,18 @@
-Metadata-Version: 2.1 Name: xregi Version: 0.3.3 Summary: A package for
+Metadata-Version: 2.1 Name: xregi Version: 0.3.4 Summary: A package for
 automatic 2D/3D registration of X-ray and CT images Home-page: https://
 github.com/shez12/xregi Download-URL: Author: Jiaming Zhang Author-email:
-jzhan282@jhu.edu License: MIT Description-Content-Type: markdown License-File:
-LICENSE Requires-Dist: h5py (>=3.7.0) Requires-Dist: imgaug (>=0.4.0) Requires-
-Dist: matplotlib (>=3.5.2) Requires-Dist: ml-collections (>=0.1.1) Requires-
-Dist: numpy (>=1.24.2) Requires-Dist: opencv-python (>=4.6.0.66) Requires-Dist:
-pandas (>=1.4.3) Requires-Dist: Pillow (>=9.3.0) Requires-Dist: pydicom
-(>=2.3.0) Requires-Dist: scipy (>=1.9.0) Requires-Dist: seaborn (>=0.12.2)
-Requires-Dist: torch (>=1.12.0) Requires-Dist: torchvision (>=0.13.0)
+jzhan282@jhu.edu License: MIT Description-Content-Type: text/markdown License-
+File: LICENSE Requires-Dist: h5py (>=3.7.0) Requires-Dist: imgaug (>=0.4.0)
+Requires-Dist: matplotlib (>=3.5.2) Requires-Dist: ml-collections (>=0.1.1)
+Requires-Dist: numpy (>=1.24.2) Requires-Dist: opencv-python (>=4.6.0.66)
+Requires-Dist: pandas (>=1.4.3) Requires-Dist: Pillow (>=9.3.0) Requires-Dist:
+pydicom (>=2.3.0) Requires-Dist: scipy (>=1.9.0) Requires-Dist: seaborn
+(>=0.12.2) Requires-Dist: torch (>=1.12.0) Requires-Dist: torchvision
+(>=0.13.0)
                                  [xregi logo]
      [Tutorial_in_Colab] [https://img.shields.io/badge/Made%20with-Python-
         1f425f.svg] [https://badge.fury.io/py/xregi.svg] [License:_MIT]
 This is a python package for registering x-ray images and CT scans. It is based
 on the [xReg](https://github.com/rg2/xreg), a C++ library for medical image
 registration, and [synthex](https://github.com/arcadelab/SyntheX), a python
 package for synthetic x-ray imaging. ## Third-party libraries Before you start,
```

## Comparing `xregi-0.3.3.dist-info/RECORD` & `xregi-0.3.4.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -18,12 +18,12 @@
 xregi/synthex/test_ensemble.py,sha256=4R-tWuR_s_ClpyFY8zMNiZqEj7gSBCZZe_WyvPTLZaQ,6217
 xregi/synthex/util.py,sha256=d6_PJdlAcV73KEoV6WWMSIAE3_D45dewyaCDqG6Sq3s,11437
 xregi/synthex/TransUNet/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 xregi/synthex/TransUNet/transunet.py,sha256=bX2-1GfVD1-hwqpbDZb7bs-ZNji72CHwyYlOVMPeXOA,29577
 xregi/synthex/TransUNet/vit_seg_configs.py,sha256=ZhY53sEFRbIDjZWiQUt26pVSYHYTiJyrLCXvPsG8RTw,4297
 xregi/synthex/TransUNet/vit_seg_modeling.py,sha256=q4Vcfa23r3GhrAmtuk11x0qYZ_iUgMZeuau2RGHz-j8,17634
 xregi/synthex/TransUNet/vit_seg_modeling_resnet_skip.py,sha256=u2artZjji-J9c4OZzS6Z_iGEQAEEUhX0F_5gaBLfPuU,6250
-xregi-0.3.3.dist-info/LICENSE,sha256=pRjedJyE-HxSQfgARQPRAePZ26xRUjBS_JXQqBJPvSo,1070
-xregi-0.3.3.dist-info/METADATA,sha256=9TgEGW3SUIy4lUB2jhqPmF1UQrncvyfakFl1MdAgrFk,4273
-xregi-0.3.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-xregi-0.3.3.dist-info/top_level.txt,sha256=dpIwGdSiJ2zG9qouq-IP7ik-23coM9Si2al3x3ObsO0,6
-xregi-0.3.3.dist-info/RECORD,,
+xregi-0.3.4.dist-info/LICENSE,sha256=pRjedJyE-HxSQfgARQPRAePZ26xRUjBS_JXQqBJPvSo,1070
+xregi-0.3.4.dist-info/METADATA,sha256=sZD36Y7e7gHQQxPkilhG1ZN3MPzPqSRuY_a9GCLciyA,4278
+xregi-0.3.4.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+xregi-0.3.4.dist-info/top_level.txt,sha256=dpIwGdSiJ2zG9qouq-IP7ik-23coM9Si2al3x3ObsO0,6
+xregi-0.3.4.dist-info/RECORD,,
```

