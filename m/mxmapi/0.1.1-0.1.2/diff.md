# Comparing `tmp/mxmapi-0.1.1.tar.gz` & `tmp/mxmapi-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mxmapi-0.1.1.tar", last modified: Fri May 26 19:57:08 2023, max compression
+gzip compressed data, was "mxmapi-0.1.2.tar", last modified: Fri May 26 20:23:26 2023, max compression
```

## Comparing `mxmapi-0.1.1.tar` & `mxmapi-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 19:57:08.328940 mxmapi-0.1.1/
--rw-rw-rw-   0        0        0     1089 2023-05-25 23:10:02.000000 mxmapi-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      933 2023-05-26 19:57:08.315937 mxmapi-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      550 2023-05-25 23:02:27.000000 mxmapi-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 19:57:08.264410 mxmapi-0.1.1/mxmapi/
--rw-rw-rw-   0        0        0       57 2023-05-26 19:54:09.000000 mxmapi-0.1.1/mxmapi/__init__.py
--rw-rw-rw-   0        0        0    23306 2023-05-26 08:34:00.000000 mxmapi-0.1.1/mxmapi/client.py
--rw-rw-rw-   0        0        0     1025 2023-05-25 19:50:31.000000 mxmapi-0.1.1/mxmapi/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-05-26 19:57:08.310938 mxmapi-0.1.1/mxmapi.egg-info/
--rw-rw-rw-   0        0        0      933 2023-05-26 19:57:08.000000 mxmapi-0.1.1/mxmapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-26 19:57:08.000000 mxmapi-0.1.1/mxmapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 19:57:08.000000 mxmapi-0.1.1/mxmapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-05-26 19:57:08.000000 mxmapi-0.1.1/mxmapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-26 19:57:08.000000 mxmapi-0.1.1/mxmapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 19:57:08.329941 mxmapi-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      946 2023-05-26 19:57:01.000000 mxmapi-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:23:26.333095 mxmapi-0.1.2/
+-rw-rw-rw-   0        0        0     1089 2023-05-25 23:10:02.000000 mxmapi-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      933 2023-05-26 20:23:26.292865 mxmapi-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      550 2023-05-25 23:02:27.000000 mxmapi-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-05-26 20:23:26.233978 mxmapi-0.1.2/mxmapi/
+-rw-rw-rw-   0        0        0       57 2023-05-26 19:54:09.000000 mxmapi-0.1.2/mxmapi/__init__.py
+-rw-rw-rw-   0        0        0    23306 2023-05-26 08:34:00.000000 mxmapi-0.1.2/mxmapi/client.py
+-rw-rw-rw-   0        0        0     1013 2023-05-26 20:21:51.000000 mxmapi-0.1.2/mxmapi/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-05-26 20:23:26.286339 mxmapi-0.1.2/mxmapi.egg-info/
+-rw-rw-rw-   0        0        0      933 2023-05-26 20:23:26.000000 mxmapi-0.1.2/mxmapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2023-05-26 20:23:26.000000 mxmapi-0.1.2/mxmapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-26 20:23:26.000000 mxmapi-0.1.2/mxmapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-26 20:23:26.000000 mxmapi-0.1.2/mxmapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-26 20:23:26.000000 mxmapi-0.1.2/mxmapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-26 20:23:26.334097 mxmapi-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0      946 2023-05-26 20:22:34.000000 mxmapi-0.1.2/setup.py
```

### Comparing `mxmapi-0.1.1/LICENSE` & `mxmapi-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mxmapi-0.1.1/PKG-INFO` & `mxmapi-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxmapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Python library for the Musixmatch Web API
 Home-page: https://mxmapi.readthedocs.io/
 Author: Adel Hashem
 Author-email: adel.mohamed.9998@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AdelHashem/mxmapi
 Description-Content-Type: text/markdown
```

### Comparing `mxmapi-0.1.1/README.md` & `mxmapi-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `mxmapi-0.1.1/mxmapi/client.py` & `mxmapi-0.1.2/mxmapi/client.py`

 * *Files identical despite different names*

### Comparing `mxmapi-0.1.1/mxmapi/exceptions.py` & `mxmapi-0.1.2/mxmapi/exceptions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 class MXMException(Exception):
 
     codes = {
         400: "The request had bad syntax or was inherently impossible to be satisfied.",
         401: "Authentication failed, probably because of invalid/missing API key.",
         402: "The usage limit has been reached, either you exceeded per day requests limits or your balance is insufficient.",
         403: "You are not authorized to perform this operation.",
-        404: "You are not authorized to perform this operation.",
+        404: "The requested resource was not found.",
         405: "The requested method was not found.",
         500: "Ops. Something were wrong.",
         503: "Our system is a bit busy at the moment and your request can't be satisfied."
     }
 
 
     def __init__(self,status_code, message):
```

### Comparing `mxmapi-0.1.1/mxmapi.egg-info/PKG-INFO` & `mxmapi-0.1.2/mxmapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mxmapi
-Version: 0.1.1
+Version: 0.1.2
 Summary: A simple Python library for the Musixmatch Web API
 Home-page: https://mxmapi.readthedocs.io/
 Author: Adel Hashem
 Author-email: adel.mohamed.9998@gmail.com
 License: MIT
 Project-URL: Source, https://github.com/AdelHashem/mxmapi
 Description-Content-Type: text/markdown
```

### Comparing `mxmapi-0.1.1/setup.py` & `mxmapi-0.1.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 # Get the long description from the README file
 with open(path.join(HERE, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name="mxmapi",
-    version="0.1.1",
+    version="0.1.2",
     description="A simple Python library for the Musixmatch Web API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://mxmapi.readthedocs.io/",
     author="Adel Hashem",
     author_email="adel.mohamed.9998@gmail.com",
     license="MIT",
```

