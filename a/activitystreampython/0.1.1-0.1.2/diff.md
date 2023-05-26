# Comparing `tmp/activitystreampython-0.1.1.tar.gz` & `tmp/activitystreampython-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "activitystreampython-0.1.1.tar", max compression
+gzip compressed data, was "activitystreampython-0.1.2.tar", max compression
```

## Comparing `activitystreampython-0.1.1.tar` & `activitystreampython-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,6 @@
--rw-r--r--   0        0        0     1068 2023-05-26 11:59:06.910357 activitystreampython-0.1.1/LICENSE
--rw-r--r--   0        0        0     2531 2023-05-26 12:42:17.922443 activitystreampython-0.1.1/README.md
--rw-r--r--   0        0        0     4972 2023-05-26 12:05:22.985037 activitystreampython-0.1.1/activitystreampython/activitystream.py
--rw-r--r--   0        0        0      601 2023-05-26 12:42:34.945129 activitystreampython-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 activitystreampython-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-05-26 11:59:06.910357 activitystreampython-0.1.2/LICENSE
+-rw-r--r--   0        0        0     2531 2023-05-26 12:42:17.922443 activitystreampython-0.1.2/README.md
+-rw-r--r--   0        0        0       45 2023-05-26 12:52:03.000967 activitystreampython-0.1.2/activitystreampython/__init__.py
+-rw-r--r--   0        0        0     4972 2023-05-26 12:05:22.985037 activitystreampython-0.1.2/activitystreampython/activitystream.py
+-rw-r--r--   0        0        0      601 2023-05-26 12:52:55.113985 activitystreampython-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3173 1970-01-01 00:00:00.000000 activitystreampython-0.1.2/PKG-INFO
```

### Comparing `activitystreampython-0.1.1/LICENSE` & `activitystreampython-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.1/README.md` & `activitystreampython-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.1/activitystreampython/activitystream.py` & `activitystreampython-0.1.2/activitystreampython/activitystream.py`

 * *Files identical despite different names*

### Comparing `activitystreampython-0.1.1/pyproject.toml` & `activitystreampython-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "activitystreampython"
-version = "0.1.1"
+version = "0.1.2"
 description = "A convenience library to make retrieving data from the Activity Stream Data Service API easier"
 authors = ["Hugh Topping <hugh@crowdengage.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/crowdengage/activitystreampython/"
 repository = "https://github.com/crowdengage/activitystreampython/"
```

### Comparing `activitystreampython-0.1.1/PKG-INFO` & `activitystreampython-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: activitystreampython
-Version: 0.1.1
+Version: 0.1.2
 Summary: A convenience library to make retrieving data from the Activity Stream Data Service API easier
 Home-page: https://github.com/crowdengage/activitystreampython/
 License: MIT
 Author: Hugh Topping
 Author-email: hugh@crowdengage.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

