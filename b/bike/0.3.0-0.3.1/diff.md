# Comparing `tmp/bike-0.3.0.tar.gz` & `tmp/bike-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bike-0.3.0.tar", max compression
+gzip compressed data, was "bike-0.3.1.tar", max compression
```

## Comparing `bike-0.3.0.tar` & `bike-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.0/LICENSE
--rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.0/README.md
--rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.0/bike/__init__.py
--rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.0/bike/controllers.py
--rw-r--r--   0        0        0     2780 2023-05-20 11:23:00.413966 bike-0.3.0/bike/fields.py
--rw-r--r--   0        0        0     8299 2023-05-21 10:46:27.744577 bike-0.3.0/bike/models.py
--rw-r--r--   0        0        0      534 2023-05-21 11:51:10.827971 bike-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 09:53:26.052501 bike-0.3.1/LICENSE
+-rw-r--r--   0        0        0     2773 2023-05-21 11:06:50.768748 bike-0.3.1/README.md
+-rw-r--r--   0        0        0      183 2023-05-04 09:53:26.052501 bike-0.3.1/bike/__init__.py
+-rw-r--r--   0        0        0     1063 2023-05-08 10:10:28.086731 bike-0.3.1/bike/controllers.py
+-rw-r--r--   0        0        0     2780 2023-05-20 11:23:00.413966 bike-0.3.1/bike/fields.py
+-rw-r--r--   0        0        0     8299 2023-05-21 10:46:27.744577 bike-0.3.1/bike/models.py
+-rw-r--r--   0        0        0      495 2023-05-26 09:59:14.492885 bike-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     3335 1970-01-01 00:00:00.000000 bike-0.3.1/PKG-INFO
```

### Comparing `bike-0.3.0/LICENSE` & `bike-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bike-0.3.0/README.md` & `bike-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `bike-0.3.0/bike/controllers.py` & `bike-0.3.1/bike/controllers.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.0/bike/fields.py` & `bike-0.3.1/bike/fields.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.0/bike/models.py` & `bike-0.3.1/bike/models.py`

 * *Files identical despite different names*

### Comparing `bike-0.3.0/PKG-INFO` & `bike-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bike
-Version: 0.3.0
+Version: 0.3.1
 Summary: A lightweight model validator for modern projects.
 Home-page: https://github.com/manasseslima/bike
 License: MIT
 Author: Manasses Lima
 Author-email: manasseslima@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

