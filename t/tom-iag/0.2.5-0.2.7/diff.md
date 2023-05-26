# Comparing `tmp/tom_iag-0.2.5.tar.gz` & `tmp/tom_iag-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tom_iag-0.2.5.tar", max compression
+gzip compressed data, was "tom_iag-0.2.7.tar", max compression
```

## Comparing `tom_iag-0.2.5.tar` & `tom_iag-0.2.7.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1099 2023-02-14 12:51:38.030855 tom_iag-0.2.5/LICENSE
--rw-r--r--   0        0        0      169 2023-02-14 12:51:38.030855 tom_iag-0.2.5/README.md
--rw-r--r--   0        0        0      438 2023-02-14 12:51:38.030855 tom_iag-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-14 12:51:38.030855 tom_iag-0.2.5/tom_iag/__init__.py
--rw-r--r--   0        0        0    23504 2023-02-14 12:51:38.030855 tom_iag-0.2.5/tom_iag/iag.py
--rw-r--r--   0        0        0      764 1970-01-01 00:00:00.000000 tom_iag-0.2.5/setup.py
--rw-r--r--   0        0        0      836 1970-01-01 00:00:00.000000 tom_iag-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1099 2023-05-26 17:23:29.925434 tom_iag-0.2.7/LICENSE
+-rw-r--r--   0        0        0      169 2023-05-26 17:23:29.925434 tom_iag-0.2.7/README.md
+-rw-r--r--   0        0        0      438 2023-05-26 17:23:29.925434 tom_iag-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 17:23:29.925434 tom_iag-0.2.7/tom_iag/__init__.py
+-rw-r--r--   0        0        0    23504 2023-05-26 17:23:29.925434 tom_iag-0.2.7/tom_iag/iag.py
+-rw-r--r--   0        0        0      887 1970-01-01 00:00:00.000000 tom_iag-0.2.7/PKG-INFO
```

### Comparing `tom_iag-0.2.5/LICENSE` & `tom_iag-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tom_iag-0.2.5/tom_iag/iag.py` & `tom_iag-0.2.7/tom_iag/iag.py`

 * *Files identical despite different names*

### Comparing `tom_iag-0.2.5/PKG-INFO` & `tom_iag-0.2.7/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: tom-iag
-Version: 0.2.5
+Version: 0.2.7
 Summary: IAG telescopes facility module for the TOM Toolkit
 Home-page: https://github.com/thusser/tom_iag
 License: MIT
 Author: Tim-Oliver Husser
 Author-email: thusser@uni-goettingen.de
-Requires-Python: >=3.7,<3.11
+Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/thusser/tom_iag
 Description-Content-Type: text/markdown
 
 # TOM oservation facility interface for the IAG telescopes.
 
 ## Features
 This module adds support to the TOM Toolkit for the IAG telescopes (MONET/N, MONET/S IAG50cm).
```

