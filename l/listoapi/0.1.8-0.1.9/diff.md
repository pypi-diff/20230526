# Comparing `tmp/listoapi-0.1.8.tar.gz` & `tmp/listoapi-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\listoapi-0.1.8.tar", last modified: Mon Jul 30 16:16:08 2018, max compression
+gzip compressed data, was "dist\listoapi-0.1.9.tar", last modified: Mon Jul 30 22:20:47 2018, max compression
```

## Comparing `listoapi-0.1.8.tar` & `listoapi-0.1.9.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2018-07-30 16:16:08.000000 listoapi-0.1.8/
-drwxrwxrwx   0        0        0        0 2018-07-30 16:16:08.000000 listoapi-0.1.8/listoapi/
--rw-rw-rw-   0        0        0     4198 2018-07-30 16:14:30.000000 listoapi-0.1.8/listoapi/api.py
--rw-rw-rw-   0        0        0      372 2018-07-27 15:05:14.000000 listoapi-0.1.8/listoapi/banks.py
--rw-rw-rw-   0        0        0     1075 2018-07-24 15:46:17.000000 listoapi-0.1.8/listoapi/cfdi_payments.py
--rw-rw-rw-   0        0        0     2652 2018-07-24 15:46:17.000000 listoapi-0.1.8/listoapi/documents.py
--rw-rw-rw-   0        0        0     1337 2018-07-24 15:46:17.000000 listoapi-0.1.8/listoapi/expenses.py
--rw-rw-rw-   0        0        0     7813 2018-07-25 22:23:44.000000 listoapi-0.1.8/listoapi/invoices.py
--rw-rw-rw-   0        0        0     5514 2018-07-24 15:46:17.000000 listoapi-0.1.8/listoapi/invoicing.py
--rw-rw-rw-   0        0        0     2079 2018-07-24 15:46:17.000000 listoapi-0.1.8/listoapi/items.py
--rw-rw-rw-   0        0        0     2171 2018-07-24 15:46:17.000000 listoapi-0.1.8/listoapi/setup.py
--rw-rw-rw-   0        0        0     1027 2018-07-25 14:57:45.000000 listoapi-0.1.8/listoapi/__init__.py
-drwxrwxrwx   0        0        0        0 2018-07-30 16:16:08.000000 listoapi-0.1.8/listoapi.egg-info/
--rw-rw-rw-   0        0        0        1 2018-07-30 16:16:07.000000 listoapi-0.1.8/listoapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0     2578 2018-07-30 16:16:07.000000 listoapi-0.1.8/listoapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       35 2018-07-30 16:16:07.000000 listoapi-0.1.8/listoapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0      381 2018-07-30 16:16:07.000000 listoapi-0.1.8/listoapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        9 2018-07-30 16:16:07.000000 listoapi-0.1.8/listoapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2578 2018-07-30 16:16:08.000000 listoapi-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     1297 2018-07-24 16:57:53.000000 listoapi-0.1.8/README.rst
--rw-rw-rw-   0        0        0       42 2018-07-30 16:16:08.000000 listoapi-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      949 2018-07-30 16:15:13.000000 listoapi-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2018-07-30 22:20:47.000000 listoapi-0.1.9/
+drwxrwxrwx   0        0        0        0 2018-07-30 22:20:47.000000 listoapi-0.1.9/listoapi/
+-rw-rw-rw-   0        0        0     4198 2018-07-30 16:14:30.000000 listoapi-0.1.9/listoapi/api.py
+-rw-rw-rw-   0        0        0      372 2018-07-27 15:05:14.000000 listoapi-0.1.9/listoapi/banks.py
+-rw-rw-rw-   0        0        0     1075 2018-07-24 15:46:17.000000 listoapi-0.1.9/listoapi/cfdi_payments.py
+-rw-rw-rw-   0        0        0     2652 2018-07-24 15:46:17.000000 listoapi-0.1.9/listoapi/documents.py
+-rw-rw-rw-   0        0        0     1337 2018-07-24 15:46:17.000000 listoapi-0.1.9/listoapi/expenses.py
+-rw-rw-rw-   0        0        0     7813 2018-07-25 22:23:44.000000 listoapi-0.1.9/listoapi/invoices.py
+-rw-rw-rw-   0        0        0     5514 2018-07-24 15:46:17.000000 listoapi-0.1.9/listoapi/invoicing.py
+-rw-rw-rw-   0        0        0     2079 2018-07-24 15:46:17.000000 listoapi-0.1.9/listoapi/items.py
+-rwxrwxrwx   0        0        0  1802436 2018-07-24 15:46:17.000000 listoapi-0.1.9/listoapi/openssl.exe
+-rw-rw-rw-   0        0        0     2171 2018-07-24 15:46:17.000000 listoapi-0.1.9/listoapi/setup.py
+-rw-rw-rw-   0        0        0     1027 2018-07-25 14:57:45.000000 listoapi-0.1.9/listoapi/__init__.py
+drwxrwxrwx   0        0        0        0 2018-07-30 22:20:47.000000 listoapi-0.1.9/listoapi.egg-info/
+-rw-rw-rw-   0        0        0        1 2018-07-30 22:20:45.000000 listoapi-0.1.9/listoapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0     2578 2018-07-30 22:20:45.000000 listoapi-0.1.9/listoapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0       35 2018-07-30 22:20:45.000000 listoapi-0.1.9/listoapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0      414 2018-07-30 22:20:46.000000 listoapi-0.1.9/listoapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        9 2018-07-30 22:20:45.000000 listoapi-0.1.9/listoapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       28 2018-07-30 22:18:43.000000 listoapi-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2578 2018-07-30 22:20:47.000000 listoapi-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1297 2018-07-24 16:57:53.000000 listoapi-0.1.9/README.rst
+-rw-rw-rw-   0        0        0       42 2018-07-30 22:20:47.000000 listoapi-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      982 2018-07-30 22:20:14.000000 listoapi-0.1.9/setup.py
```

### Comparing `listoapi-0.1.8/listoapi/api.py` & `listoapi-0.1.9/listoapi/api.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi/cfdi_payments.py` & `listoapi-0.1.9/listoapi/cfdi_payments.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi/documents.py` & `listoapi-0.1.9/listoapi/documents.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi/expenses.py` & `listoapi-0.1.9/listoapi/expenses.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi/invoices.py` & `listoapi-0.1.9/listoapi/invoices.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi/invoicing.py` & `listoapi-0.1.9/listoapi/invoicing.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi/items.py` & `listoapi-0.1.9/listoapi/items.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi/setup.py` & `listoapi-0.1.9/listoapi/setup.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi/__init__.py` & `listoapi-0.1.9/listoapi/__init__.py`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/listoapi.egg-info/PKG-INFO` & `listoapi-0.1.9/listoapi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: listoapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Listo SDK module for web API integration
 Home-page: https://github.com/listomx/bridges-common
 Author: Hugo Villegas <hugo.villegas@listo.mx>
 Author-email: hugo.villegas@listo.mx
 License: UNKNOWN
 Description: Listo SDK module for web API integration
         ===============================================
```

### Comparing `listoapi-0.1.8/PKG-INFO` & `listoapi-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: listoapi
-Version: 0.1.8
+Version: 0.1.9
 Summary: Listo SDK module for web API integration
 Home-page: https://github.com/listomx/bridges-common
 Author: Hugo Villegas <hugo.villegas@listo.mx>
 Author-email: hugo.villegas@listo.mx
 License: UNKNOWN
 Description: Listo SDK module for web API integration
         ===============================================
```

### Comparing `listoapi-0.1.8/README.rst` & `listoapi-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `listoapi-0.1.8/setup.py` & `listoapi-0.1.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import setuptools
 
 with open("README.rst", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="listoapi",
-    version="0.1.8",
+    version="0.1.9",
     author="Hugo Villegas <hugo.villegas@listo.mx>",
     author_email="hugo.villegas@listo.mx",
     keywords='api listo listoapi sdk integration python',
     description="Listo SDK module for web API integration",
     long_description=long_description,
     url="https://github.com/listomx/bridges-common",
     packages=setuptools.find_packages(),
+    include_package_data = True,
     install_requires=[
         "requests>=2.19.1",
         "pyopenssl==17.5.0",
     ],
     classifiers=(
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
```

