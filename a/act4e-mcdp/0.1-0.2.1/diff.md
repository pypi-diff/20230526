# Comparing `tmp/act4e_mcdp-0.1-py3-none-any.whl.zip` & `tmp/act4e_mcdp-0.2.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 6288 bytes, number of entries: 10
--rw-r--r--  2.0 unx      250 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
+Zip file size: 6322 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      273 b- defN 80-Jan-01 00:00 act4e_mcdp/__init__.py
 -rw-r--r--  2.0 unx     8426 b- defN 80-Jan-01 00:00 act4e_mcdp/loading.py
 -rw-r--r--  2.0 unx     3018 b- defN 80-Jan-01 00:00 act4e_mcdp/main.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 act4e_mcdp/py.typed
 -rw-r--r--  2.0 unx      729 b- defN 80-Jan-01 00:00 act4e_mcdp/solution_interface.py
 -rw-r--r--  2.0 unx     3239 b- defN 80-Jan-01 00:00 act4e_mcdp/structures.py
--rw-r--r--  2.0 unx      313 b- defN 80-Jan-01 00:00 act4e_mcdp-0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 act4e_mcdp-0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx      777 b- defN 16-Jan-01 00:00 act4e_mcdp-0.1.dist-info/RECORD
-10 files, 16898 bytes uncompressed, 4964 bytes compressed:  70.6%
+-rw-r--r--  2.0 unx      315 b- defN 80-Jan-01 00:00 act4e_mcdp-0.2.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 act4e_mcdp-0.2.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       58 b- defN 80-Jan-01 00:00 act4e_mcdp-0.2.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx      785 b- defN 16-Jan-01 00:00 act4e_mcdp-0.2.1.dist-info/RECORD
+10 files, 16931 bytes uncompressed, 4982 bytes compressed:  70.6%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: act4e_mcdp/solution_interface.py
 Comment: 
 
 Filename: act4e_mcdp/structures.py
 Comment: 
 
-Filename: act4e_mcdp-0.1.dist-info/METADATA
+Filename: act4e_mcdp-0.2.1.dist-info/METADATA
 Comment: 
 
-Filename: act4e_mcdp-0.1.dist-info/WHEEL
+Filename: act4e_mcdp-0.2.1.dist-info/WHEEL
 Comment: 
 
-Filename: act4e_mcdp-0.1.dist-info/entry_points.txt
+Filename: act4e_mcdp-0.2.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: act4e_mcdp-0.1.dist-info/RECORD
+Filename: act4e_mcdp-0.2.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## act4e_mcdp/__init__.py

```diff
@@ -3,11 +3,13 @@
 coloredlogs.install(level="DEBUG")
 
 from logging import getLogger, DEBUG
 
 logger = getLogger(__name__)
 logger.setLevel(DEBUG)
 
+__version__ = "0.2.1"
+
 from .loading import *
 from .structures import *
 from .main import *
 from .solution_interface import *
```

## Comparing `act4e_mcdp-0.1.dist-info/RECORD` & `act4e_mcdp-0.2.1.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-act4e_mcdp/__init__.py,sha256=n7aquIo9O9Khsz57KYKsSOiBJYhFBPQ-Gkt7dOufaZ0,250
+act4e_mcdp/__init__.py,sha256=nqM8O9zJsz0iu5fjloxjB6txzLavHTEeq85n4UvBD90,273
 act4e_mcdp/loading.py,sha256=dGRBzIsjeJEEAoW9dvJ8N1pa58CTLx-Wq2kGTS-aX4M,8426
 act4e_mcdp/main.py,sha256=P93v6jFVfeeD-CePlZa0yCdmm2KwRkK3asDeabv1Ezw,3018
 act4e_mcdp/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 act4e_mcdp/solution_interface.py,sha256=mwhfSGZlZSfufKdQn5qpho16dfOW4-tI1ZP0IVgqTRk,729
 act4e_mcdp/structures.py,sha256=n9kCF82W82eqqquWWv2txi2nTfy5FPDWRvh7T-FyXK0,3239
-act4e_mcdp-0.1.dist-info/METADATA,sha256=7VOZRClaY9MuwMTNGogjrmQ2pJplt8KQLRAOQ1Vql4w,313
-act4e_mcdp-0.1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
-act4e_mcdp-0.1.dist-info/entry_points.txt,sha256=cfj1OzFHMtFmK8Wl5Ulxkv9yficQNQ60fnULm1eq70w,58
-act4e_mcdp-0.1.dist-info/RECORD,,
+act4e_mcdp-0.2.1.dist-info/METADATA,sha256=qTqyvAF6aNG6oFufP1zChRQ6cHk54TeDmF2VpofnlIE,315
+act4e_mcdp-0.2.1.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+act4e_mcdp-0.2.1.dist-info/entry_points.txt,sha256=cfj1OzFHMtFmK8Wl5Ulxkv9yficQNQ60fnULm1eq70w,58
+act4e_mcdp-0.2.1.dist-info/RECORD,,
```

