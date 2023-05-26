# Comparing `tmp/eodc_sdk-2023.5.0rc0.tar.gz` & `tmp/eodc_sdk-2023.5.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eodc_sdk-2023.5.0rc0.tar", max compression
+gzip compressed data, was "eodc_sdk-2023.5.0rc1.tar", max compression
```

## Comparing `eodc_sdk-2023.5.0rc0.tar` & `eodc_sdk-2023.5.0rc1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       62 2023-05-26 06:49:03.468621 eodc_sdk-2023.5.0rc0/README.md
--rw-r--r--   0        0        0       30 2023-05-26 07:14:42.738460 eodc_sdk-2023.5.0rc0/eodc/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 06:49:03.468621 eodc_sdk-2023.5.0rc0/eodc/client.py
--rw-r--r--   0        0        0      125 2023-05-26 06:49:03.468621 eodc_sdk-2023.5.0rc0/eodc/config.py
--rw-r--r--   0        0        0        0 2023-05-26 06:49:03.468621 eodc_sdk-2023.5.0rc0/eodc/dask_clusters.py
--rw-r--r--   0        0        0      108 2023-05-26 06:49:03.468621 eodc_sdk-2023.5.0rc0/eodc/processors.py
--rw-r--r--   0        0        0     1074 2023-05-26 07:14:33.068462 eodc_sdk-2023.5.0rc0/pyproject.toml
--rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 eodc_sdk-2023.5.0rc0/PKG-INFO
+-rw-r--r--   0        0        0       62 2023-05-26 07:44:53.024237 eodc_sdk-2023.5.0rc1/README.md
+-rw-r--r--   0        0        0       30 2023-05-26 07:44:53.024237 eodc_sdk-2023.5.0rc1/eodc/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 07:44:53.024237 eodc_sdk-2023.5.0rc1/eodc/client.py
+-rw-r--r--   0        0        0      125 2023-05-26 07:44:53.024237 eodc_sdk-2023.5.0rc1/eodc/config.py
+-rw-r--r--   0        0        0        0 2023-05-26 07:44:53.024237 eodc_sdk-2023.5.0rc1/eodc/dask_clusters.py
+-rw-r--r--   0        0        0      108 2023-05-26 07:44:53.024237 eodc_sdk-2023.5.0rc1/eodc/processors.py
+-rw-r--r--   0        0        0     1074 2023-05-26 07:44:53.024237 eodc_sdk-2023.5.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     1296 1970-01-01 00:00:00.000000 eodc_sdk-2023.5.0rc1/PKG-INFO
```

### Comparing `eodc_sdk-2023.5.0rc0/pyproject.toml` & `eodc_sdk-2023.5.0rc1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eodc-sdk"
-version = "2023.5.0-rc.0"
+version = "2023.5.0-rc.1"
 description = "Python SDK for interacting with EODC services."
 authors = ["Lukas Weidenholzer <lukas.weidenholzer@eodc.eu>"]
 maintainers = ["EODC Staff <support@eodc.eu>"]
 readme = "README.md"
 repository = "https://github.com/eodcgmbh/eodc-sdk"
 classifiers = [
     "Development Status :: 1 - Planning",
```

### Comparing `eodc_sdk-2023.5.0rc0/PKG-INFO` & `eodc_sdk-2023.5.0rc1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eodc-sdk
-Version: 2023.5.0rc0
+Version: 2023.5.0rc1
 Summary: Python SDK for interacting with EODC services.
 Home-page: https://github.com/eodcgmbh/eodc-sdk
 Author: Lukas Weidenholzer
 Author-email: lukas.weidenholzer@eodc.eu
 Maintainer: EODC Staff
 Maintainer-email: support@eodc.eu
 Requires-Python: >=3.8,<3.12
```

