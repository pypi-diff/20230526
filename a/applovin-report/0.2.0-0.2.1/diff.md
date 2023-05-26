# Comparing `tmp/applovin_report-0.2.0.tar.gz` & `tmp/applovin_report-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "applovin_report-0.2.0.tar", max compression
+gzip compressed data, was "applovin_report-0.2.1.tar", max compression
```

## Comparing `applovin_report-0.2.0.tar` & `applovin_report-0.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-26 04:51:49.969633 applovin_report-0.2.0/LICENSE
--rw-r--r--   0        0        0      762 2023-05-26 04:51:49.969633 applovin_report-0.2.0/README.md
--rw-r--r--   0        0        0       94 2023-05-26 04:51:49.969633 applovin_report-0.2.0/applovin_report/__init__.py
--rw-r--r--   0        0        0     4773 2023-05-26 04:51:49.969633 applovin_report-0.2.0/applovin_report/revenue_reporting_api.py
--rw-r--r--   0        0        0     2589 2023-05-26 04:51:49.973633 applovin_report-0.2.0/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-26 04:51:49.973633 applovin_report-0.2.0/tests/__init__.py
--rw-r--r--   0        0        0     2065 2023-05-26 04:51:49.973633 applovin_report-0.2.0/tests/test_app.py
--rw-r--r--   0        0        0     2779 1970-01-01 00:00:00.000000 applovin_report-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-05-26 06:18:51.229395 applovin_report-0.2.1/LICENSE
+-rw-r--r--   0        0        0      762 2023-05-26 06:18:51.229395 applovin_report-0.2.1/README.md
+-rw-r--r--   0        0        0       94 2023-05-26 06:18:51.229395 applovin_report-0.2.1/applovin_report/__init__.py
+-rw-r--r--   0        0        0     4773 2023-05-26 06:18:51.229395 applovin_report-0.2.1/applovin_report/revenue_reporting_api.py
+-rw-r--r--   0        0        0     2589 2023-05-26 06:18:51.229395 applovin_report-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0       45 2023-05-26 06:18:51.233395 applovin_report-0.2.1/tests/__init__.py
+-rw-r--r--   0        0        0     2065 2023-05-26 06:18:51.233395 applovin_report-0.2.1/tests/test_app.py
+-rw-r--r--   0        0        0     2779 1970-01-01 00:00:00.000000 applovin_report-0.2.1/PKG-INFO
```

### Comparing `applovin_report-0.2.0/LICENSE` & `applovin_report-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `applovin_report-0.2.0/README.md` & `applovin_report-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `applovin_report-0.2.0/applovin_report/revenue_reporting_api.py` & `applovin_report-0.2.1/applovin_report/revenue_reporting_api.py`

 * *Files identical despite different names*

### Comparing `applovin_report-0.2.0/pyproject.toml` & `applovin_report-0.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "applovin_report"
-version = "0.2.0"
+version = "0.2.1"
 homepage = "https://github.com/ikamedawn/applovin_report"
 description = "Applovin Report APIs wrapper."
 authors = ["Dawn <minhpc@ikameglobal.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
     'Development Status :: 2 - Pre-Alpha',
```

### Comparing `applovin_report-0.2.0/tests/test_app.py` & `applovin_report-0.2.1/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `applovin_report-0.2.0/PKG-INFO` & `applovin_report-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: applovin-report
-Version: 0.2.0
+Version: 0.2.1
 Summary: Applovin Report APIs wrapper.
 Home-page: https://github.com/ikamedawn/applovin_report
 License: MIT
 Author: Dawn
 Author-email: minhpc@ikameglobal.com
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 2 - Pre-Alpha
```

