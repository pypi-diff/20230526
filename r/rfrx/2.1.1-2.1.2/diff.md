# Comparing `tmp/rfrx-2.1.1.tar.gz` & `tmp/rfrx-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfrx-2.1.1.tar", max compression
+gzip compressed data, was "rfrx-2.1.2.tar", max compression
```

## Comparing `rfrx-2.1.1.tar` & `rfrx-2.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1303 2023-05-26 12:00:39.543793 rfrx-2.1.1/LICENSE
--rw-r--r--   0        0        0     1970 2023-05-26 12:00:39.543793 rfrx-2.1.1/README.md
--rw-r--r--   0        0        0     1003 2023-05-26 12:00:39.543793 rfrx-2.1.1/pyproject.toml
--rw-r--r--   0        0        0      139 2023-05-26 12:00:39.543793 rfrx-2.1.1/rfrx/__init__.py
--rw-r--r--   0        0        0     2475 2023-05-26 12:00:39.543793 rfrx-2.1.1/rfrx/protronik.py
--rw-r--r--   0        0        0     4542 2023-05-26 12:00:39.543793 rfrx-2.1.1/rfrx/sbus.py
--rw-r--r--   0        0        0     2740 1970-01-01 00:00:00.000000 rfrx-2.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1303 2023-05-26 12:02:19.043804 rfrx-2.1.2/LICENSE
+-rw-r--r--   0        0        0     1970 2023-05-26 12:02:19.043804 rfrx-2.1.2/README.md
+-rw-r--r--   0        0        0     1003 2023-05-26 12:02:19.043804 rfrx-2.1.2/pyproject.toml
+-rw-r--r--   0        0        0      139 2023-05-26 12:02:19.043804 rfrx-2.1.2/rfrx/__init__.py
+-rw-r--r--   0        0        0     2475 2023-05-26 12:02:19.043804 rfrx-2.1.2/rfrx/protronik.py
+-rw-r--r--   0        0        0     4542 2023-05-26 12:02:19.043804 rfrx-2.1.2/rfrx/sbus.py
+-rw-r--r--   0        0        0     2740 1970-01-01 00:00:00.000000 rfrx-2.1.2/PKG-INFO
```

### Comparing `rfrx-2.1.1/LICENSE` & `rfrx-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rfrx-2.1.1/README.md` & `rfrx-2.1.2/README.md`

 * *Files identical despite different names*

### Comparing `rfrx-2.1.1/pyproject.toml` & `rfrx-2.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 [tool.poetry]
 authors = ["Guilhem Saurel <guilhem.saurel@laas.fr>"]
 description = "Receive RF frames from SBUS and Pro-Tronik PTR-6A v2"
 homepage = "https://github.com/nim65s/rfrx"
 license = "BSD-2-Clause"
 name = "rfrx"
 readme = "README.md"
-version = "2.1.1"
+version = "2.1.2"
 
 [tool.poetry.dependencies]
 pyserial = "^3.5"
 python = "^3.7"
 
 [tool.poetry.group.dev]
 optional = true
```

### Comparing `rfrx-2.1.1/rfrx/protronik.py` & `rfrx-2.1.2/rfrx/protronik.py`

 * *Files identical despite different names*

### Comparing `rfrx-2.1.1/rfrx/sbus.py` & `rfrx-2.1.2/rfrx/sbus.py`

 * *Files identical despite different names*

### Comparing `rfrx-2.1.1/PKG-INFO` & `rfrx-2.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfrx
-Version: 2.1.1
+Version: 2.1.2
 Summary: Receive RF frames from SBUS and Pro-Tronik PTR-6A v2
 Home-page: https://github.com/nim65s/rfrx
 License: BSD-2-Clause
 Author: Guilhem Saurel
 Author-email: guilhem.saurel@laas.fr
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

