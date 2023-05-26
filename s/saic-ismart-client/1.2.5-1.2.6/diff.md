# Comparing `tmp/saic_ismart_client-1.2.5.tar.gz` & `tmp/saic_ismart_client-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saic_ismart_client-1.2.5.tar", last modified: Sun May 14 10:12:11 2023, max compression
+gzip compressed data, was "saic_ismart_client-1.2.6.tar", last modified: Fri May 26 13:28:34 2023, max compression
```

## Comparing `saic_ismart_client-1.2.5.tar` & `saic_ismart_client-1.2.6.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.647162 saic_ismart_client-1.2.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    21607 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/common_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/data_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/
--rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/Message.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/data_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    29707 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/src/saic_ismart_client/saic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.651162 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-14 10:12:11.000000 saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 10:12:11.655162 saic_ismart_client-1.2.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_Message_v1_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_Message_v2_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_Message_v3_0.py
--rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_abrp_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    16638 2023-05-14 10:11:58.000000 saic_ismart_client-1.2.5/tests/test_saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.079245 saic_ismart_client-1.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 13:28:22.000000 saic_ismart_client-1.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 13:28:22.000000 saic_ismart_client-1.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-26 13:28:34.079245 saic_ismart_client-1.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-26 13:28:22.000000 saic_ismart_client-1.2.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-26 13:28:22.000000 saic_ismart_client-1.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:28:34.079245 saic_ismart_client-1.2.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.071245 saic_ismart_client-1.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.075245 saic_ismart_client-1.2.6/src/saic_ismart_client/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.071245 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.075245 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-26 13:28:22.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.075245 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3609 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherHeader.asn1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.075245 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3230 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherHeader.asn1
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21291 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/common_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.075245 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v1_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v1_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v1_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15634 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v1_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.075245 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v2_1/
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v2_1/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v2_1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18407 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v2_1/data_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.075245 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v3_0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v3_0/Message.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v3_0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v3_0/data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29769 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/src/saic_ismart_client/saic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.075245 saic_ismart_client-1.2.6/src/saic_ismart_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-26 13:28:34.000000 saic_ismart_client-1.2.6/src/saic_ismart_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-26 13:28:34.000000 saic_ismart_client-1.2.6/src/saic_ismart_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:28:34.000000 saic_ismart_client-1.2.6/src/saic_ismart_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 13:28:34.000000 saic_ismart_client-1.2.6/src/saic_ismart_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 13:28:34.000000 saic_ismart_client-1.2.6/src/saic_ismart_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:28:34.079245 saic_ismart_client-1.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7936 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/tests/test_Message_v1_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/tests/test_Message_v2_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8581 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/tests/test_Message_v3_0.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4217 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/tests/test_abrp_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16753 2023-05-26 13:28:23.000000 saic_ismart_client-1.2.6/tests/test_saic_api.py
```

### Comparing `saic_ismart_client-1.2.5/LICENSE` & `saic_ismart_client-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/PKG-INFO` & `saic_ismart_client-1.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic_ismart_client
-Version: 1.2.5
+Version: 1.2.6
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.2.5/README.md` & `saic_ismart_client-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/pyproject.toml` & `saic_ismart_client-1.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "saic_ismart_client"
-version = "1.2.5"
+version = "1.2.6"
 authors = [
     { name = "Thomas Salm", email="saic-python-client@devtom.de"},
 ]
 dependencies = [
     "asn1tools >= 0.165.0",
     "requests >= 2.28.2",
     "urllib3 >= 1.26.14",
```

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v1_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v1_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v2_1/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v2_1/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v3_0/ApplicationData.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ASN.1_schema/v3_0/MP_DispatcherBody.asn1`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/abrp_api.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/common_model.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/common_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -419,25 +419,18 @@
         header_bytes = buffered_message_bytes.read(self.header_length)
         header.protocol_version = int(header_bytes[0])
         header.dispatcher_message_length = int(header_bytes[1])
         header.dispatcher_body_encoding = int(header_bytes[2])
 
         decoded_message.reserved = buffered_message_bytes.read(self.reserved_size)
 
-        if header.protocol_version == 32:
-            message_body = decoded_message.body
-            message_body.application_data_length = 0
-            message_body.result = -1
-            message_body.error_message = 'Skipping unknown protocol version 32'.encode()
-        else:
-            dispatcher_message_bytes = buffered_message_bytes.read(
-                header.dispatcher_message_length - self.header_length)
-            message_body_dict = self.asn1_tool_uper.decode('MPDispatcherBody', dispatcher_message_bytes)
-            message_body = decoded_message.body
-            message_body.init_from_dict(message_body_dict)
+        dispatcher_message_bytes = buffered_message_bytes.read(header.dispatcher_message_length - self.header_length)
+        message_body_dict = self.asn1_tool_uper.decode('MPDispatcherBody', dispatcher_message_bytes)
+        message_body = decoded_message.body
+        message_body.init_from_dict(message_body_dict)
 
         if message_body.application_data_length > 0:
             application_data_bytes = buffered_message_bytes.read(message_body.application_data_length)
             application_data_dict = self.asn1_tool_uper.decode(decoded_message.application_data.asn_type,
                                                                application_data_bytes)
             decoded_message.application_data.init_from_dict(application_data_dict)
         else:
```

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/Message.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v1_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v1_1/data_model.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v1_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/Message.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v2_1/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v2_1/data_model.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v2_1/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/Message.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v3_0/Message.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/ota_v3_0/data_model.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/ota_v3_0/data_model.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client/saic_api.py` & `saic_ismart_client-1.2.6/src/saic_ismart_client/saic_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -444,14 +444,15 @@
             vehicle_control_req.rvc_params.append(param)
 
         vehicle_control_cmd_req_msg = MessageV2(MessageBodyV2(), vehicle_control_req)
         application_id = '510'
         application_data_protocol_version = 25857
         self.message_V2_1_coder.initialize_message(self.uid, self.get_token(), vin_info.vin, application_id,
                                                    application_data_protocol_version, 1, vehicle_control_cmd_req_msg)
+        vehicle_control_cmd_req_msg.body.ack_required = False
         if event_id is not None:
             vehicle_control_cmd_req_msg.body.event_id = event_id
         self.publish_json_request(application_id, application_data_protocol_version,
                                   vehicle_control_cmd_req_msg.get_data())
         vehicle_control_cmd_req_msg_hex = self.message_V2_1_coder.encode_request(vehicle_control_cmd_req_msg)
         self.publish_raw_request(application_id, application_data_protocol_version, vehicle_control_cmd_req_msg_hex)
         vehicle_control_cmd_rsp_msg_hex = self.send_request(vehicle_control_cmd_req_msg_hex,
```

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/PKG-INFO` & `saic_ismart_client-1.2.6/src/saic_ismart_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saic-ismart-client
-Version: 1.2.5
+Version: 1.2.6
 Summary: SAIC client library (MG iSMART)
 Author-email: Thomas Salm <saic-python-client@devtom.de>
 Project-URL: Homepage, https://github.com/SAIC-iSmart-API/saic-python-client
 Project-URL: Bug Tracker, https://github.com/SAIC-iSmart-API/saic-python-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `saic_ismart_client-1.2.5/src/saic_ismart_client.egg-info/SOURCES.txt` & `saic_ismart_client-1.2.6/src/saic_ismart_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/tests/test_Message_v1_1.py` & `saic_ismart_client-1.2.6/tests/test_Message_v1_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/tests/test_Message_v2_1.py` & `saic_ismart_client-1.2.6/tests/test_Message_v2_1.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/tests/test_Message_v3_0.py` & `saic_ismart_client-1.2.6/tests/test_Message_v3_0.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/tests/test_abrp_api.py` & `saic_ismart_client-1.2.6/tests/test_abrp_api.py`

 * *Files identical despite different names*

### Comparing `saic_ismart_client-1.2.5/tests/test_saic_api.py` & `saic_ismart_client-1.2.6/tests/test_saic_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -242,14 +242,15 @@
     start_ac_rsp.basicVehicleStatus.veh_elec_rng_dsp = 125
     start_ac_rsp.basicVehicleStatus.rmt_htd_rr_wnd_st = 125
     start_ac_rsp.basicVehicleStatus.engine_status = 0
     start_ac_rsp.basicVehicleStatus.extended_data2 = 0  # is charging
     start_ac_rsp.basicVehicleStatus.fuel_range_elec = 32000
     start_ac_rsp_msg = MessageV2(MessageBodyV2(), start_ac_rsp)
     message_coder_v2_1.initialize_message(uid, token, vin_info.vin, '510', 25857, 1, start_ac_rsp_msg)
+    start_ac_rsp_msg.body.ack_required = False
     return message_coder_v2_1.encode_request(start_ac_rsp_msg)
 
 
 def mock_response(mocked_post, hex_value: str):
     def res():
         r = requests.Response()
         r.status_code = 200
@@ -309,7 +310,8 @@
     def test_start_ac(self, mocked_post):
         vin_info = create_vin_info(VIN)
         mock_response(mocked_post, mock_start_ac_rsp_msg(self.message_coder_v2_1, UID, TOKEN, vin_info))
 
         start_ac_rsp_msg = self.saic_api.start_ac(vin_info)
         app_data = cast(OtaRvcStatus25857, start_ac_rsp_msg.application_data)
         self.assertEqual(app_data.rvcReqType, b'\x06')
+        self.assertEqual(start_ac_rsp_msg.body.ack_required, False)
```

