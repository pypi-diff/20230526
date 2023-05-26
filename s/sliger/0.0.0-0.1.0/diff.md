# Comparing `tmp/sliger-0.0.0.tar.gz` & `tmp/sliger-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sliger-0.0.0.tar", max compression
+gzip compressed data, was "sliger-0.1.0.tar", max compression
```

## Comparing `sliger-0.0.0.tar` & `sliger-0.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     4659 2023-05-26 09:25:35.586126 sliger-0.0.0/README.md
--rw-r--r--   0        0        0      555 2023-05-26 09:30:54.051700 sliger-0.0.0/pyproject.toml
--rw-r--r--   0        0        0    15063 2023-05-26 09:26:11.591289 sliger-0.0.0/sliger/__init__.py
--rw-r--r--   0        0        0     5441 1970-01-01 00:00:00.000000 sliger-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4659 2023-05-26 09:25:35.586126 sliger-0.1.0/README.md
+-rw-r--r--   0        0        0      594 2023-05-26 11:42:17.175137 sliger-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0    15063 2023-05-26 09:26:11.591289 sliger-0.1.0/sliger/__init__.py
+-rw-r--r--   0        0        0     5480 1970-01-01 00:00:00.000000 sliger-0.1.0/PKG-INFO
```

### Comparing `sliger-0.0.0/README.md` & `sliger-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `sliger-0.0.0/pyproject.toml` & `sliger-0.1.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "sliger"
-version = "0.0.0"
-description = "Slide of the Tiger"
-authors = ["Giulio Picollo <gipiccol@cisco.com>"]
+version = "0.1.0"
+description = "Slide the power of Python (and Jinja2) into Google Slides"
+authors = ["Giulio Piccolo <gipiccol@cisco.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = "^0.9.0"
 google = "^3.0.0"
```

### Comparing `sliger-0.0.0/sliger/__init__.py` & `sliger-0.1.0/sliger/__init__.py`

 * *Files identical despite different names*

### Comparing `sliger-0.0.0/PKG-INFO` & `sliger-0.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: sliger
-Version: 0.0.0
-Summary: Slide of the Tiger
+Version: 0.1.0
+Summary: Slide the power of Python (and Jinja2) into Google Slides
 License: Apache 2.0
-Author: Giulio Picollo
+Author: Giulio Piccolo
 Author-email: gipiccol@cisco.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google (>=3.0.0,<4.0.0)
```

#### html2text {}

```diff
@@ -1,18 +1,19 @@
-Metadata-Version: 2.1 Name: sliger Version: 0.0.0 Summary: Slide of the Tiger
-License: Apache 2.0 Author: Giulio Picollo Author-email: gipiccol@cisco.com
-Requires-Python: >=3.10,<4.0 Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: google (>=3.0.0,<4.0.0) Requires-Dist: google-api-python-client
-(>=2.87.0,<3.0.0) Requires-Dist: google-auth (==2.19.0) Requires-Dist: google-
-auth-httplib2 (>=0.1.0,<0.2.0) Requires-Dist: google-auth-oauthlib
-(>=1.0.0,<2.0.0) Requires-Dist: jinja2 (>=3.1.2,<4.0.0) Requires-Dist: toml
-(>=0.10.2,<0.11.0) Requires-Dist: typer (>=0.9.0,<0.10.0) Description-Content-
-Type: text/markdown # `sliger`
+Metadata-Version: 2.1 Name: sliger Version: 0.1.0 Summary: Slide the power of
+Python (and Jinja2) into Google Slides License: Apache 2.0 Author: Giulio
+Piccolo Author-email: gipiccol@cisco.com Requires-Python: >=3.10,<4.0
+Classifier: License :: Other/Proprietary License Classifier: Programming
+Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Requires-Dist: google
+(>=3.0.0,<4.0.0) Requires-Dist: google-api-python-client (>=2.87.0,<3.0.0)
+Requires-Dist: google-auth (==2.19.0) Requires-Dist: google-auth-httplib2
+(>=0.1.0,<0.2.0) Requires-Dist: google-auth-oauthlib (>=1.0.0,<2.0.0) Requires-
+Dist: jinja2 (>=3.1.2,<4.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Requires-
+Dist: typer (>=0.9.0,<0.10.0) Description-Content-Type: text/markdown #
+`sliger`
  [https://raw.githubusercontent.com/slidoapp/sliger/main/static/images/sliger-
    black.png] Slide of the tiger Slide the power of Python (and Jinja2) into
                                  Google Slides
  ![PyPI](https://img.shields.io/pypi/v/sliger) ![License: Apache 2.0](https://
   img.shields.io/badge/License-Apache_2.0-green.svg) [https://img.shields.io/
    badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336] [https://
 img.shields.io/badge/code%20style-black-000000.svg] [![Scc Count Badge](https:/
```

