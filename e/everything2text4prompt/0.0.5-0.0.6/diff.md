# Comparing `tmp/everything2text4prompt-0.0.5.tar.gz` & `tmp/everything2text4prompt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everything2text4prompt-0.0.5.tar", last modified: Sun May 21 07:30:26 2023, max compression
+gzip compressed data, was "everything2text4prompt-0.0.6.tar", last modified: Fri May 26 15:45:44 2023, max compression
```

## Comparing `everything2text4prompt-0.0.5.tar` & `everything2text4prompt-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 07:30:26.014077 everything2text4prompt-0.0.5/
--rw-rw-rw-   0        0        0     1089 2023-05-18 13:27:55.000000 everything2text4prompt-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1052 2023-05-21 07:30:26.013080 everything2text4prompt-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      658 2023-05-18 13:34:54.000000 everything2text4prompt-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 07:30:25.995128 everything2text4prompt-0.0.5/everything2text4prompt/
--rw-rw-rw-   0        0        0       87 2023-05-21 07:29:32.000000 everything2text4prompt-0.0.5/everything2text4prompt/__init__.py
--rw-rw-rw-   0        0        0     4947 2023-05-21 07:26:08.000000 everything2text4prompt-0.0.5/everything2text4prompt/everything2text4prompt.py
-drwxrwxrwx   0        0        0        0 2023-05-21 07:30:26.010088 everything2text4prompt-0.0.5/everything2text4prompt/playground/
--rw-rw-rw-   0        0        0      754 2023-05-19 14:34:30.000000 everything2text4prompt-0.0.5/everything2text4prompt/playground/test_split_mp3.py
--rw-rw-rw-   0        0        0      340 2023-05-19 15:00:50.000000 everything2text4prompt-0.0.5/everything2text4prompt/playground/test_whisper.py
--rw-rw-rw-   0        0        0     1281 2023-05-19 14:58:14.000000 everything2text4prompt-0.0.5/everything2text4prompt/util.py
-drwxrwxrwx   0        0        0        0 2023-05-21 07:30:26.006098 everything2text4prompt-0.0.5/everything2text4prompt.egg-info/
--rw-rw-rw-   0        0        0     1052 2023-05-21 07:30:25.000000 everything2text4prompt-0.0.5/everything2text4prompt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      472 2023-05-21 07:30:25.000000 everything2text4prompt-0.0.5/everything2text4prompt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 07:30:25.000000 everything2text4prompt-0.0.5/everything2text4prompt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-05-21 07:30:25.000000 everything2text4prompt-0.0.5/everything2text4prompt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2023-05-21 07:30:25.000000 everything2text4prompt-0.0.5/everything2text4prompt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 07:30:26.014077 everything2text4prompt-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      768 2023-05-21 07:27:42.000000 everything2text4prompt-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:45:44.059115 everything2text4prompt-0.0.6/
+-rw-rw-rw-   0        0        0     1089 2023-05-18 13:27:55.000000 everything2text4prompt-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1052 2023-05-26 15:45:44.058129 everything2text4prompt-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      658 2023-05-18 13:34:54.000000 everything2text4prompt-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 15:45:44.040166 everything2text4prompt-0.0.6/everything2text4prompt/
+-rw-rw-rw-   0        0        0      125 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/__init__.py
+-rw-rw-rw-   0        0        0     2372 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/everything2text4prompt.py
+-rw-rw-rw-   0        0        0      369 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/pdf_util.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:45:44.055154 everything2text4prompt-0.0.6/everything2text4prompt/playground/
+-rw-rw-rw-   0        0        0      754 2023-05-19 14:34:30.000000 everything2text4prompt-0.0.6/everything2text4prompt/playground/test_split_mp3.py
+-rw-rw-rw-   0        0        0      340 2023-05-19 15:00:50.000000 everything2text4prompt-0.0.6/everything2text4prompt/playground/test_whisper.py
+-rw-rw-rw-   0        0        0     1062 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/podcast_util.py
+-rw-rw-rw-   0        0        0     2075 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/util.py
+-rw-rw-rw-   0        0        0     2235 2023-05-26 15:42:05.000000 everything2text4prompt-0.0.6/everything2text4prompt/youtube_util.py
+drwxrwxrwx   0        0        0        0 2023-05-26 15:45:44.051166 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/
+-rw-rw-rw-   0        0        0     1052 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      585 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-05-26 15:45:43.000000 everything2text4prompt-0.0.6/everything2text4prompt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 15:45:44.059115 everything2text4prompt-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      768 2023-05-26 15:44:54.000000 everything2text4prompt-0.0.6/setup.py
```

### Comparing `everything2text4prompt-0.0.5/LICENSE` & `everything2text4prompt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.5/PKG-INFO` & `everything2text4prompt-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everything2text4prompt
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert many medium into text, and the text format is specialized for prompt input
 Home-page: https://github.com/michaelthwan/everything2text4prompt
 Author: michaethwan
 Author-email: michaelthwan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `everything2text4prompt-0.0.5/README.md` & `everything2text4prompt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.5/everything2text4prompt/playground/test_split_mp3.py` & `everything2text4prompt-0.0.6/everything2text4prompt/playground/test_split_mp3.py`

 * *Files identical despite different names*

### Comparing `everything2text4prompt-0.0.5/everything2text4prompt.egg-info/PKG-INFO` & `everything2text4prompt-0.0.6/everything2text4prompt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: everything2text4prompt
-Version: 0.0.5
+Version: 0.0.6
 Summary: Convert many medium into text, and the text format is specialized for prompt input
 Home-page: https://github.com/michaelthwan/everything2text4prompt
 Author: michaethwan
 Author-email: michaelthwan@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `everything2text4prompt-0.0.5/setup.py` & `everything2text4prompt-0.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="everything2text4prompt",
-    version="0.0.5",
+    version="0.0.6",
     description="Convert many medium into text, and the text format is specialized for prompt input",
     # package_dir={'': 'everything2text4prompt'},
     packages=find_packages(),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/michaelthwan/everything2text4prompt",
     author="michaethwan",
```

