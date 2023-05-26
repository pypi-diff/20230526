# Comparing `tmp/activitystreampython-0.1.4.tar.gz` & `tmp/activitystreampython-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activitystreampython-0.1.4.tar", max compression
+gzip compressed data, was "activitystreampython-0.1.5.tar", max compression
```

## Comparing `activitystreampython-0.1.4.tar` & `activitystreampython-0.1.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-05-26 11:59:06.910357 activitystreampython-0.1.4/LICENSE
--rw-r--r--   0        0        0     2531 2023-05-26 12:42:17.922443 activitystreampython-0.1.4/README.md
--rw-r--r--   0        0        0       46 2023-05-26 13:03:57.815792 activitystreampython-0.1.4/activitystreampython/__init__.py
--rw-r--r--   0        0        0     4972 2023-05-26 12:05:22.985037 activitystreampython-0.1.4/activitystreampython/activitystream.py
--rw-r--r--   0        0        0      602 2023-05-26 13:14:28.571431 activitystreampython-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     3227 1970-01-01 00:00:00.000000 activitystreampython-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-26 11:59:06.910357 activitystreampython-0.1.5/LICENSE
+-rw-r--r--   0        0        0     2531 2023-05-26 12:42:17.922443 activitystreampython-0.1.5/README.md
+-rw-r--r--   0        0        0       46 2023-05-26 13:03:57.815792 activitystreampython-0.1.5/activitystreampython/__init__.py
+-rw-r--r--   0        0        0     4972 2023-05-26 12:05:22.985037 activitystreampython-0.1.5/activitystreampython/activitystream.py
+-rw-r--r--   0        0        0      609 2023-05-26 14:56:45.495577 activitystreampython-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     3246 1970-01-01 00:00:00.000000 activitystreampython-0.1.5/PKG-INFO
```

### Comparing `activitystreampython-0.1.4/LICENSE` & `activitystreampython-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.4/README.md` & `activitystreampython-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.4/activitystreampython/activitystream.py` & `activitystreampython-0.1.5/activitystreampython/activitystream.py`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.4/pyproject.toml` & `activitystreampython-0.1.5/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "activitystreampython"
-version = "0.1.4"
+version = "0.1.5"
 description = "A convenience library to make retrieving data from the Activity Stream Data Service API easier"
 authors = ["Hugh Topping <hugh@crowdengage.com>"]
-license = "MIT"
+license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/crowdengage/activitystreampython/"
 repository = "https://github.com/crowdengage/activitystreampython/"
 
 [tool.poetry.dependencies]
 python = "^3.9.5"
 requests = "^2.31.0"
```

### Comparing `activitystreampython-0.1.4/PKG-INFO` & `activitystreampython-0.1.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: activitystreampython
-Version: 0.1.4
+Version: 0.1.5
 Summary: A convenience library to make retrieving data from the Activity Stream Data Service API easier
 Home-page: https://github.com/crowdengage/activitystreampython/
-License: MIT
+License: Apache-2.0
 Author: Hugh Topping
 Author-email: hugh@crowdengage.com
 Requires-Python: >=3.9.5,<4.0.0
-Classifier: License :: OSI Approved :: MIT License
+Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Project-URL: Repository, https://github.com/crowdengage/activitystreampython/
 Description-Content-Type: text/markdown
```

