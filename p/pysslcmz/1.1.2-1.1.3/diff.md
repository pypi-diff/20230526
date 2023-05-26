# Comparing `tmp/pysslcmz-1.1.2.tar.gz` & `tmp/pysslcmz-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysslcmz-1.1.2.tar", max compression
+gzip compressed data, was "pysslcmz-1.1.3.tar", max compression
```

## Comparing `pysslcmz-1.1.2.tar` & `pysslcmz-1.1.3.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rwxr-xr-x   0        0        0     1073 2022-08-31 05:36:44.407090 pysslcmz-1.1.2/LICENSE
--rwxr-xr-x   0        0        0     1879 2022-08-31 06:46:03.426859 pysslcmz-1.1.2/README.md
--rwxr-xr-x   0        0        0      689 2022-08-31 06:43:06.915435 pysslcmz-1.1.2/pyproject.toml
--rwxr-xr-x   0        0        0       22 2022-08-31 06:24:12.115885 pysslcmz-1.1.2/pysslcmz/__init__.py
--rwxr-xr-x   0        0        0      136 2022-08-31 05:56:35.700962 pysslcmz-1.1.2/pysslcmz/_constants.py
--rwxr-xr-x   0        0        0     7185 2022-08-31 06:42:48.660977 pysslcmz-1.1.2/pysslcmz/payment.py
--rw-r--r--   0        0        0     2538 2022-08-31 06:46:41.202135 pysslcmz-1.1.2/setup.py
--rw-r--r--   0        0        0     2624 2022-08-31 06:46:41.202315 pysslcmz-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-26 21:49:30.668813 pysslcmz-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1879 2023-05-26 21:49:30.668813 pysslcmz-1.1.3/README.md
+-rw-r--r--   0        0        0      705 2023-05-26 21:49:30.668813 pysslcmz-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-05-26 21:49:30.668813 pysslcmz-1.1.3/pysslcmz/__init__.py
+-rw-r--r--   0        0        0      136 2023-05-26 21:49:30.668813 pysslcmz-1.1.3/pysslcmz/_constants.py
+-rw-r--r--   0        0        0     7185 2023-05-26 21:49:30.668813 pysslcmz-1.1.3/pysslcmz/payment.py
+-rw-r--r--   0        0        0     2689 1970-01-01 00:00:00.000000 pysslcmz-1.1.3/PKG-INFO
```

### Comparing `pysslcmz-1.1.2/LICENSE` & `pysslcmz-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pysslcmz-1.1.2/README.md` & `pysslcmz-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pysslcmz-1.1.2/pyproject.toml` & `pysslcmz-1.1.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "pysslcmz"
-version = "1.1.2"
-description = "Implements SSLCOMMERZ payment gateway in python based web apps."
+version = "1.1.3"
+description = "Implements SSLCOMMERZ payment gateway in python based web apps (python 3.8+)."
 authors = ["Piecoders IT Solutions <piecodersit@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/piecoders/pyssl"
 repository = "https://github.com/piecoders/pyssl"
 keywords = ["SSLCommerz", "sslcommerz", "SSLCOMMERZ", "bkash", "nagod", "upai", "rocket"]
 classifiers = [
@@ -15,12 +15,12 @@
     "LICENSE",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 
 [tool.poetry.dev-dependencies]
-pytest = "^5.2"
+pytest = "^5.4.3"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pysslcmz-1.1.2/pysslcmz/payment.py` & `pysslcmz-1.1.3/pysslcmz/payment.py`

 * *Files identical despite different names*

### Comparing `pysslcmz-1.1.2/PKG-INFO` & `pysslcmz-1.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pysslcmz
-Version: 1.1.2
-Summary: Implements SSLCOMMERZ payment gateway in python based web apps.
+Version: 1.1.3
+Summary: Implements SSLCOMMERZ payment gateway in python based web apps (python 3.8+).
 Home-page: https://github.com/piecoders/pyssl
 License: MIT
 Keywords: SSLCommerz,sslcommerz,SSLCOMMERZ,bkash,nagod,upai,rocket
 Author: Piecoders IT Solutions
 Author-email: piecodersit@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/piecoders/pyssl
 Description-Content-Type: text/markdown
 
 # SSLCOMMERZ Payment Gateway implementation in Python
 Provides a python module to implement payment gateway in python based web apps.
 
 ## Installation
```

