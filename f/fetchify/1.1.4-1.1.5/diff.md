# Comparing `tmp/fetchify-1.1.4.tar.gz` & `tmp/fetchify-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fetchify-1.1.4.tar", last modified: Fri May 26 07:09:23 2023, max compression
+gzip compressed data, was "fetchify-1.1.5.tar", last modified: Fri May 26 07:17:40 2023, max compression
```

## Comparing `fetchify-1.1.4.tar` & `fetchify-1.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 07:09:23.045259 fetchify-1.1.4/
--rw-rw-rw-   0        0        0      594 2023-05-26 07:09:22.604017 fetchify-1.1.4/PKG-INFO
--rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.1.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 07:09:22.602509 fetchify-1.1.4/fetchify.egg-info/
--rw-rw-rw-   0        0        0      594 2023-05-26 07:09:22.000000 fetchify-1.1.4/fetchify.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      204 2023-05-26 07:09:22.000000 fetchify-1.1.4/fetchify.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 07:09:22.000000 fetchify-1.1.4/fetchify.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 07:09:22.000000 fetchify-1.1.4/fetchify.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-26 07:09:22.000000 fetchify-1.1.4/fetchify.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      825 2023-05-26 07:05:59.000000 fetchify-1.1.4/fetchify.py
--rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.1.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-26 07:09:23.045939 fetchify-1.1.4/setup.cfg
--rw-rw-rw-   0        0        0      904 2023-05-26 07:09:04.000000 fetchify-1.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 07:17:40.100513 fetchify-1.1.5/
+-rw-rw-rw-   0        0        0      594 2023-05-26 07:17:40.097527 fetchify-1.1.5/PKG-INFO
+-rw-rw-rw-   0        0        0        9 2023-05-19 11:17:31.000000 fetchify-1.1.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 07:17:40.091543 fetchify-1.1.5/fetchify.egg-info/
+-rw-rw-rw-   0        0        0      594 2023-05-26 07:17:39.000000 fetchify-1.1.5/fetchify.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      204 2023-05-26 07:17:39.000000 fetchify-1.1.5/fetchify.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 07:17:39.000000 fetchify-1.1.5/fetchify.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 07:17:39.000000 fetchify-1.1.5/fetchify.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-26 07:17:39.000000 fetchify-1.1.5/fetchify.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      826 2023-05-26 07:16:47.000000 fetchify-1.1.5/fetchify.py
+-rw-rw-rw-   0        0        0       86 2023-05-18 06:16:12.000000 fetchify-1.1.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-26 07:17:40.101523 fetchify-1.1.5/setup.cfg
+-rw-rw-rw-   0        0        0      904 2023-05-26 07:17:08.000000 fetchify-1.1.5/setup.py
```

### Comparing `fetchify-1.1.4/PKG-INFO` & `fetchify-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.4
+Version: 1.1.5
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.4/fetchify.egg-info/PKG-INFO` & `fetchify-1.1.5/fetchify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fetchify
-Version: 1.1.4
+Version: 1.1.5
 Summary: Library to access Code Files from Cloud
 Home-page: https://techinfoak.wixsite.com/tech-info
 Author: Anupam Kanoongo
 Author-email: programmer.tiak@gmail.com
 License: MIT
 Project-URL: Our Website, https://techinfoak.wixsite.com/tech-info
 Project-URL: Our YT Handle, https://youtube.com/@techinfoak
```

### Comparing `fetchify-1.1.4/fetchify.py` & `fetchify-1.1.5/fetchify.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """This a library that mean't to access files from github repo without opening it again and again"""
 
 import requests
 url = {
-    "py" : "https://raw.githubusercontent.com/Anupam1707/Python_Programmes/main/"
+    "py" : "https://raw.githubusercontent.com/Anupam1707/Python_Programmes/main/",
     "we" : "https://raw.githubusercontent.com/Anupam1707/weather-app-py/main/",
     "aiu" : "https://raw.githubusercontent.com/Anupam1707/ai/main/",
     "ds" : "https://raw.githubusercontent.com/Anupam1707/datasense/main/",
     "spy" : "https://raw.githubusercontent.com/Anupam1707/SecuriPy/main/"
 }
 
 def fetch(filename, code, image = False):
```

### Comparing `fetchify-1.1.4/setup.py` & `fetchify-1.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="fetchify",
-    version="1.1.4",
+    version="1.1.5",
     author="Anupam Kanoongo",
     author_email="programmer.tiak@gmail.com",
     description="Library to access Code Files from Cloud",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://techinfoak.wixsite.com/tech-info",
     project_urls={
```

