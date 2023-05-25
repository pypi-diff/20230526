# Comparing `tmp/mdforest-1.5.1.tar.gz` & `tmp/mdforest-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdforest-1.5.1.tar", last modified: Thu May 25 04:32:15 2023, max compression
+gzip compressed data, was "mdforest-1.5.2.tar", last modified: Thu May 25 22:29:31 2023, max compression
```

## Comparing `mdforest-1.5.1.tar` & `mdforest-1.5.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:32:15.508379 mdforest-1.5.1/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.5.1/LICENSE
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-25 04:32:15.507379 mdforest-1.5.1/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2592 2023-05-20 13:55:14.000000 mdforest-1.5.1/README.rst
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:32:15.505379 mdforest-1.5.1/mdforest/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1135 2023-05-25 04:25:35.000000 mdforest-1.5.1/mdforest/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3255 2023-05-25 04:00:23.000000 mdforest-1.5.1/mdforest/mdforest.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:32:15.507379 mdforest-1.5.1/mdforest/tree/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 02:13:23.000000 mdforest-1.5.1/mdforest/tree/__init__.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-25 03:54:31.000000 mdforest-1.5.1/mdforest/tree/types.py
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-19 02:13:23.000000 mdforest-1.5.1/mdforest/treebuild.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:32:15.506379 mdforest-1.5.1/mdforest.egg-info/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-25 04:32:15.000000 mdforest-1.5.1/mdforest.egg-info/PKG-INFO
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-25 04:32:15.000000 mdforest-1.5.1/mdforest.egg-info/SOURCES.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-25 04:32:15.000000 mdforest-1.5.1/mdforest.egg-info/dependency_links.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-25 04:32:15.000000 mdforest-1.5.1/mdforest.egg-info/requires.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-25 04:32:15.000000 mdforest-1.5.1/mdforest.egg-info/top_level.txt
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.5.1/pyproject.toml
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-25 04:32:15.508379 mdforest-1.5.1/setup.cfg
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      918 2023-05-25 04:16:10.000000 mdforest-1.5.1/setup.py
-drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 04:32:15.507379 mdforest-1.5.1/tests/
--rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-19 02:13:23.000000 mdforest-1.5.1/tests/test_mdtree.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 22:29:31.794952 mdforest-1.5.2/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)    11358 2023-05-11 02:15:26.000000 mdforest-1.5.2/LICENSE
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-25 22:29:31.794952 mdforest-1.5.2/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     2592 2023-05-20 13:55:14.000000 mdforest-1.5.2/README.rst
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 22:29:31.792952 mdforest-1.5.2/mdforest/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1241 2023-05-25 22:28:28.000000 mdforest-1.5.2/mdforest/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3255 2023-05-25 04:00:23.000000 mdforest-1.5.2/mdforest/mdforest.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 22:29:31.793952 mdforest-1.5.2/mdforest/tree/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-19 02:13:23.000000 mdforest-1.5.2/mdforest/tree/__init__.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3378 2023-05-25 03:54:31.000000 mdforest-1.5.2/mdforest/tree/types.py
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     6325 2023-05-19 02:13:23.000000 mdforest-1.5.2/mdforest/treebuild.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 22:29:31.793952 mdforest-1.5.2/mdforest.egg-info/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     3016 2023-05-25 22:29:31.000000 mdforest-1.5.2/mdforest.egg-info/PKG-INFO
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      335 2023-05-25 22:29:31.000000 mdforest-1.5.2/mdforest.egg-info/SOURCES.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        1 2023-05-25 22:29:31.000000 mdforest-1.5.2/mdforest.egg-info/dependency_links.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       43 2023-05-25 22:29:31.000000 mdforest-1.5.2/mdforest.egg-info/requires.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        9 2023-05-25 22:29:31.000000 mdforest-1.5.2/mdforest.egg-info/top_level.txt
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-11 02:27:02.000000 mdforest-1.5.2/pyproject.toml
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)       38 2023-05-25 22:29:31.794952 mdforest-1.5.2/setup.cfg
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)      918 2023-05-25 22:28:53.000000 mdforest-1.5.2/setup.py
+drwxr-xr-x   0 kjmoraes  (1000) kjmoraes  (1000)        0 2023-05-25 22:29:31.793952 mdforest-1.5.2/tests/
+-rw-r--r--   0 kjmoraes  (1000) kjmoraes  (1000)     1196 2023-05-19 02:13:23.000000 mdforest-1.5.2/tests/test_mdtree.py
```

### Comparing `mdforest-1.5.1/LICENSE` & `mdforest-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.1/PKG-INFO` & `mdforest-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.5.1
+Version: 1.5.2
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.1.zip
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.2.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 mdforest - Markdown Forest
 ==========================
```

### Comparing `mdforest-1.5.1/README.rst` & `mdforest-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.1/mdforest/__init__.py` & `mdforest-1.5.2/mdforest/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,9 +29,12 @@
     
     # Remove bold and italics formatting
     markdown_text = re.sub(r'\*\*(.*?)\*\*', r'\1', markdown_text)
     markdown_text = re.sub(r'__(.*?)__', r'\1', markdown_text)
     markdown_text = re.sub(r'\*(.*?)\*', r'\1', markdown_text)
     markdown_text = re.sub(r'_(.*?)_', r'\1', markdown_text)
     
+    # Remove empty lines
+    markdown_text = re.sub(r'^\s*$', '', markdown_text, flags=re.MULTILINE)
+    
     return markdown_text
```

### Comparing `mdforest-1.5.1/mdforest/mdforest.py` & `mdforest-1.5.2/mdforest/mdforest.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.1/mdforest/tree/types.py` & `mdforest-1.5.2/mdforest/tree/types.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.1/mdforest/treebuild.py` & `mdforest-1.5.2/mdforest/treebuild.py`

 * *Files identical despite different names*

### Comparing `mdforest-1.5.1/mdforest.egg-info/PKG-INFO` & `mdforest-1.5.2/mdforest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mdforest
-Version: 1.5.1
+Version: 1.5.2
 Summary: A package to convert between Markdown and a forest data structure for efficient processing.
 Home-page: http://github.com/kj3moraes/mdforest
 Author: Keane Moraes
 Author-email: lordvader3002@gmail.com
 License: Apache 2.0
-Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.1.zip
+Download-URL: https://github.com/kj3moraes/mdforest/archive/1.5.2.zip
 Platform: UNKNOWN
 Classifier: Topic :: Utilities
 License-File: LICENSE
 
 mdforest - Markdown Forest
 ==========================
```

### Comparing `mdforest-1.5.1/setup.py` & `mdforest-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 from setuptools.command.test import test as TestCommand
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 LONG_DESCRIPTION = (this_directory / "README.rst").read_text()
 
-VERSION = '1.5.1'
+VERSION = '1.5.2'
 DESCRIPTION = 'A package to convert between Markdown and a forest data structure for efficient processing.'
 
 setup(
     name = "mdforest",
     version = VERSION,
     author = "Keane Moraes",
     author_email = 'lordvader3002@gmail.com',
```

### Comparing `mdforest-1.5.1/tests/test_mdtree.py` & `mdforest-1.5.2/tests/test_mdtree.py`

 * *Files identical despite different names*

