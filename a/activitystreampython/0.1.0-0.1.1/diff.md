# Comparing `tmp/activitystreampython-0.1.0.tar.gz` & `tmp/activitystreampython-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activitystreampython-0.1.0.tar", max compression
+gzip compressed data, was "activitystreampython-0.1.1.tar", max compression
```

## Comparing `activitystreampython-0.1.0.tar` & `activitystreampython-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1068 2023-05-26 11:59:06.910357 activitystreampython-0.1.0/LICENSE
--rw-r--r--   0        0        0     2511 2023-05-26 12:33:51.991927 activitystreampython-0.1.0/README.md
--rw-r--r--   0        0        0     4972 2023-05-26 12:05:22.985037 activitystreampython-0.1.0/activitystreampython/activitystream.py
--rw-r--r--   0        0        0      601 2023-05-26 12:38:20.510964 activitystreampython-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 activitystreampython-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-26 11:59:06.910357 activitystreampython-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2531 2023-05-26 12:42:17.922443 activitystreampython-0.1.1/README.md
+-rw-r--r--   0        0        0     4972 2023-05-26 12:05:22.985037 activitystreampython-0.1.1/activitystreampython/activitystream.py
+-rw-r--r--   0        0        0      601 2023-05-26 12:42:34.945129 activitystreampython-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 activitystreampython-0.1.1/PKG-INFO
```

### Comparing `activitystreampython-0.1.0/LICENSE` & `activitystreampython-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.0/README.md` & `activitystreampython-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 To find out more about the Activity Stream Data Service API, [browse the Swagger documentation](https://api.activitystream.com/api/v1/swagger-ui/index.html).
 
 ## Usage
 
 ### Installation
 
-Coming soon...
+`pip install activitystreampython`
 
 ### Sample usage
 
 ```python
 from activitystreampython import ActivityStreamAPI
 from datetime import datetime, timezone, timedelta
```

### Comparing `activitystreampython-0.1.0/activitystreampython/activitystream.py` & `activitystreampython-0.1.1/activitystreampython/activitystream.py`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.0/pyproject.toml` & `activitystreampython-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "activitystreampython"
-version = "0.1.0"
+version = "0.1.1"
 description = "A convenience library to make retrieving data from the Activity Stream Data Service API easier"
 authors = ["Hugh Topping <hugh@crowdengage.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/crowdengage/activitystreampython/"
 repository = "https://github.com/crowdengage/activitystreampython/"
```

### Comparing `activitystreampython-0.1.0/PKG-INFO` & `activitystreampython-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activitystreampython
-Version: 0.1.0
+Version: 0.1.1
 Summary: A convenience library to make retrieving data from the Activity Stream Data Service API easier
 Home-page: https://github.com/crowdengage/activitystreampython/
 License: MIT
 Author: Hugh Topping
 Author-email: hugh@crowdengage.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -19,15 +19,15 @@
 
 To find out more about the Activity Stream Data Service API, [browse the Swagger documentation](https://api.activitystream.com/api/v1/swagger-ui/index.html).
 
 ## Usage
 
 ### Installation
 
-Coming soon...
+`pip install activitystreampython`
 
 ### Sample usage
 
 ```python
 from activitystreampython import ActivityStreamAPI
 from datetime import datetime, timezone, timedelta
```

