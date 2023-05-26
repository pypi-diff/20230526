# Comparing `tmp/shlep-1.2.0.tar.gz` & `tmp/shlep-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shlep-1.2.0.tar", last modified: Fri May 26 06:55:16 2023, max compression
+gzip compressed data, was "shlep-1.2.1.tar", last modified: Fri May 26 15:31:58 2023, max compression
```

## Comparing `shlep-1.2.0.tar` & `shlep-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.2.0/LICENSE
--rw-r--r--   0        0        0     2221 2023-05-26 04:43:52.285127 shlep-1.2.0/README.md
--rw-r--r--   0        0        0      454 2023-05-26 06:55:16.675943 shlep-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.2.0/shlep/__init__.py
--rw-r--r--   0        0        0     3886 2023-05-26 06:54:57.004075 shlep-1.2.0/shlep/main.py
--rw-r--r--   0        0        0     2502 1970-01-01 00:00:00.000000 shlep-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-05-21 19:33:44.704545 shlep-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2164 2023-05-26 15:31:27.296172 shlep-1.2.1/README.md
+-rw-r--r--   0        0        0      454 2023-05-26 15:31:58.200276 shlep-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       32 2023-05-26 04:01:45.741927 shlep-1.2.1/shlep/__init__.py
+-rw-r--r--   0        0        0     3886 2023-05-26 06:54:57.004075 shlep-1.2.1/shlep/main.py
+-rw-r--r--   0        0        0     2445 1970-01-01 00:00:00.000000 shlep-1.2.1/PKG-INFO
```

### Comparing `shlep-1.2.0/LICENSE` & `shlep-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `shlep-1.2.0/README.md` & `shlep-1.2.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # shlep
 
-<img src="static/ai.png" alt="mascot" style="width: 400px; height: auto;">   
+![ai](static/ai.png)
 
 `shlep` lets you package your directory's content in a format that can be easily passed to ChatGPT. This is especially
 useful when using the code interpreter plugin!
 
 It automatically excludes files that match what's in your `.gitignore` file, as well as any additional exclude patterns you provide.
 
 ## Installation
```

### Comparing `shlep-1.2.0/shlep/main.py` & `shlep-1.2.1/shlep/main.py`

 * *Files identical despite different names*

### Comparing `shlep-1.2.0/PKG-INFO` & `shlep-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: shlep
-Version: 1.2.0
+Version: 1.2.1
 Summary: gather directory contents into a single file
 Author-Email: Stephan Fitzpatrick <knowsuchagency@gmail.com>
 License: Apache-2.0
 Requires-Python: >=3.10
 Requires-Dist: pathspec>=0.11.1
 Description-Content-Type: text/markdown
 
 # shlep
 
-<img src="static/ai.png" alt="mascot" style="width: 400px; height: auto;">   
+![ai](static/ai.png)
 
 `shlep` lets you package your directory's content in a format that can be easily passed to ChatGPT. This is especially
 useful when using the code interpreter plugin!
 
 It automatically excludes files that match what's in your `.gitignore` file, as well as any additional exclude patterns you provide.
 
 ## Installation
```

