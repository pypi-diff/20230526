# Comparing `tmp/odoo13_addons_oca_edi-13.0.20230223.0-py3-none-any.whl.zip` & `tmp/odoo13_addons_oca_edi-13.0.20230525.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1596 bytes, number of entries: 4
--rw-r--r--  2.0 unx     2279 b- defN 23-Feb-24 04:27 odoo13_addons_oca_edi-13.0.20230223.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Feb-24 04:27 odoo13_addons_oca_edi-13.0.20230223.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Feb-24 04:27 odoo13_addons_oca_edi-13.0.20230223.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      393 b- defN 23-Feb-24 04:27 odoo13_addons_oca_edi-13.0.20230223.0.dist-info/RECORD
-4 files, 2765 bytes uncompressed, 822 bytes compressed:  70.3%
+Zip file size: 1611 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     2330 b- defN 23-May-26 03:19 odoo13_addons_oca_edi-13.0.20230525.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-26 03:19 odoo13_addons_oca_edi-13.0.20230525.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-26 03:19 odoo13_addons_oca_edi-13.0.20230525.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      393 b- defN 23-May-26 03:19 odoo13_addons_oca_edi-13.0.20230525.0.dist-info/RECORD
+4 files, 2816 bytes uncompressed, 837 bytes compressed:  70.3%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo13_addons_oca_edi-13.0.20230223.0.dist-info/METADATA
+Filename: odoo13_addons_oca_edi-13.0.20230525.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo13_addons_oca_edi-13.0.20230223.0.dist-info/WHEEL
+Filename: odoo13_addons_oca_edi-13.0.20230525.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo13_addons_oca_edi-13.0.20230223.0.dist-info/top_level.txt
+Filename: odoo13_addons_oca_edi-13.0.20230525.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo13_addons_oca_edi-13.0.20230223.0.dist-info/RECORD
+Filename: odoo13_addons_oca_edi-13.0.20230525.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo13_addons_oca_edi-13.0.20230223.0.dist-info/METADATA` & `odoo13_addons_oca_edi-13.0.20230525.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo13-addons-oca-edi
-Version: 13.0.20230223.0
+Version: 13.0.20230525.0
 Summary: Meta package for oca-edi Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 13.0
@@ -21,14 +21,15 @@
 Requires-Dist: odoo13-addon-base-edi
 Requires-Dist: odoo13-addon-base-facturx
 Requires-Dist: odoo13-addon-base-ubl
 Requires-Dist: odoo13-addon-base-ubl-payment
 Requires-Dist: odoo13-addon-edi
 Requires-Dist: odoo13-addon-edi-account
 Requires-Dist: odoo13-addon-edi-backend-partner
+Requires-Dist: odoo13-addon-edi-bank-statement-oca
 Requires-Dist: odoo13-addon-edi-exchange-template
 Requires-Dist: odoo13-addon-edi-purchase-oca
 Requires-Dist: odoo13-addon-edi-stock-oca
 Requires-Dist: odoo13-addon-edi-storage
 Requires-Dist: odoo13-addon-edi-voxel
 Requires-Dist: odoo13-addon-edi-voxel-account-invoice
 Requires-Dist: odoo13-addon-edi-voxel-sale-order-import
```

