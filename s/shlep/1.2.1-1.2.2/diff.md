# Comparing `tmp/shlep-1.2.1.tar.gz` & `tmp/shlep-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-1.2.1.tar", last modified: Fri May 26 15:31:58 2023, max compression
+gzip compressed data, was "shlep-1.2.2.tar", last modified: Fri May 26 15:35:38 2023, max compression
```

## Comparing `shlep-1.2.1.tar` & `shlep-1.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.2.1/LICENSE
--rw-r--r--   0        0        0     2164 2023-05-26 15:31:27.296172 shlep-1.2.1/README.md
--rw-r--r--   0        0        0      454 2023-05-26 15:31:58.200276 shlep-1.2.1/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.2.1/shlep/__init__.py
--rw-r--r--   0        0        0     3886 2023-05-26 06:54:57.004075 shlep-1.2.1/shlep/main.py
--rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 shlep-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.2.2/LICENSE
+-rw-r--r--   0        0        0     2245 2023-05-26 15:35:29.532204 shlep-1.2.2/README.md
+-rw-r--r--   0        0        0      454 2023-05-26 15:35:38.099453 shlep-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.2.2/shlep/__init__.py
+-rw-r--r--   0        0        0     3886 2023-05-26 06:54:57.004075 shlep-1.2.2/shlep/main.py
+-rw-r--r--   0        0        0     2526 1970-01-01 00:00:00.000000 shlep-1.2.2/PKG-INFO
```

### Comparing `shlep-1.2.1/LICENSE` & `shlep-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-1.2.1/README.md` & `shlep-1.2.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # shlep
 
-![ai](static/ai.png)
+
+![ai](https://github.com/knowsuchagency/shlep/assets/11974795/ec862cfe-c1e3-45d8-9a75-92a240d2fb8d)
+
 
 `shlep` lets you package your directory's content in a format that can be easily passed to ChatGPT. This is especially
 useful when using the code interpreter plugin!
 
 It automatically excludes files that match what's in your `.gitignore` file, as well as any additional exclude patterns you provide.
 
 ## Installation
```

### Comparing `shlep-1.2.1/shlep/main.py` & `shlep-1.2.2/shlep/main.py`

 * *Files identical despite different names*

### Comparing `shlep-1.2.1/PKG-INFO` & `shlep-1.2.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 1.2.1
+Version: 1.2.2
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
 
 # shlep
 
-![ai](static/ai.png)
+
+![ai](https://github.com/knowsuchagency/shlep/assets/11974795/ec862cfe-c1e3-45d8-9a75-92a240d2fb8d)
+
 
 `shlep` lets you package your directory's content in a format that can be easily passed to ChatGPT. This is especially
 useful when using the code interpreter plugin!
 
 It automatically excludes files that match what's in your `.gitignore` file, as well as any additional exclude patterns you provide.
 
 ## Installation
```

