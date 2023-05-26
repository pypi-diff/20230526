# Comparing `tmp/shlep-1.2.3.tar.gz` & `tmp/shlep-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-1.2.3.tar", last modified: Fri May 26 15:54:28 2023, max compression
+gzip compressed data, was "shlep-1.3.0.tar", last modified: Fri May 26 15:55:35 2023, max compression
```

## Comparing `shlep-1.2.3.tar` & `shlep-1.3.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.2.3/LICENSE
--rw-r--r--   0        0        0     2348 2023-05-26 15:54:07.624515 shlep-1.2.3/README.md
--rw-r--r--   0        0        0      454 2023-05-26 15:54:28.407888 shlep-1.2.3/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.2.3/shlep/__init__.py
--rw-r--r--   0        0        0     3941 2023-05-26 15:45:24.441652 shlep-1.2.3/shlep/main.py
--rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 shlep-1.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.3.0/LICENSE
+-rw-r--r--   0        0        0     2348 2023-05-26 15:54:07.624515 shlep-1.3.0/README.md
+-rw-r--r--   0        0        0      454 2023-05-26 15:55:35.501531 shlep-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.3.0/shlep/__init__.py
+-rw-r--r--   0        0        0     3941 2023-05-26 15:45:24.441652 shlep-1.3.0/shlep/main.py
+-rw-r--r--   0        0        0     2629 1970-01-01 00:00:00.000000 shlep-1.3.0/PKG-INFO
```

### Comparing `shlep-1.2.3/LICENSE` & `shlep-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-1.2.3/README.md` & `shlep-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `shlep-1.2.3/shlep/main.py` & `shlep-1.3.0/shlep/main.py`

 * *Files identical despite different names*

### Comparing `shlep-1.2.3/PKG-INFO` & `shlep-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 1.2.3
+Version: 1.3.0
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
```

