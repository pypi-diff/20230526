# Comparing `tmp/sas7bdat_converter_cli-0.2.0.tar.gz` & `tmp/sas7bdat_converter_cli-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sas7bdat_converter_cli-0.2.0.tar", max compression
+gzip compressed data, was "sas7bdat_converter_cli-1.0.0.tar", max compression
```

## Comparing `sas7bdat_converter_cli-0.2.0.tar` & `sas7bdat_converter_cli-1.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1080 2023-05-25 12:46:19.743144 sas7bdat_converter_cli-0.2.0/LICENSE
--rw-r--r--   0        0        0     2675 2023-05-25 12:46:19.743144 sas7bdat_converter_cli-0.2.0/README.md
--rw-r--r--   0        0        0     2180 2023-05-25 12:46:19.743144 sas7bdat_converter_cli-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-25 12:46:19.743144 sas7bdat_converter_cli-0.2.0/sas7bdat_converter_cli/__init__.py
--rw-r--r--   0        0        0      102 2023-05-25 12:46:19.743144 sas7bdat_converter_cli-0.2.0/sas7bdat_converter_cli/__main__.py
--rw-r--r--   0        0        0     7567 2023-05-25 12:46:19.743144 sas7bdat_converter_cli-0.2.0/sas7bdat_converter_cli/main.py
--rw-r--r--   0        0        0        0 2023-05-25 12:46:19.743144 sas7bdat_converter_cli-0.2.0/sas7bdat_converter_cli/py.typed
--rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 sas7bdat_converter_cli-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-26 00:04:33.790166 sas7bdat_converter_cli-1.0.0/LICENSE
+-rw-r--r--   0        0        0     2675 2023-05-26 00:04:33.790166 sas7bdat_converter_cli-1.0.0/README.md
+-rw-r--r--   0        0        0     2180 2023-05-26 00:04:33.790166 sas7bdat_converter_cli-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-26 00:04:33.790166 sas7bdat_converter_cli-1.0.0/sas7bdat_converter_cli/__init__.py
+-rw-r--r--   0        0        0      102 2023-05-26 00:04:33.790166 sas7bdat_converter_cli-1.0.0/sas7bdat_converter_cli/__main__.py
+-rw-r--r--   0        0        0     9627 2023-05-26 00:04:33.790166 sas7bdat_converter_cli-1.0.0/sas7bdat_converter_cli/main.py
+-rw-r--r--   0        0        0        0 2023-05-26 00:04:33.790166 sas7bdat_converter_cli-1.0.0/sas7bdat_converter_cli/py.typed
+-rw-r--r--   0        0        0     3780 1970-01-01 00:00:00.000000 sas7bdat_converter_cli-1.0.0/PKG-INFO
```

### Comparing `sas7bdat_converter_cli-0.2.0/LICENSE` & `sas7bdat_converter_cli-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sas7bdat_converter_cli-0.2.0/README.md` & `sas7bdat_converter_cli-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `sas7bdat_converter_cli-0.2.0/pyproject.toml` & `sas7bdat_converter_cli-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sas7bdat-converter-cli"
-version = "0.2.0"
+version = "1.0.0"
 description = "CLI to convert sas7bdat and xport files into other formats"
 authors = ["Paul Sanders <paul@pbsdatasolutions.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/pbs-data-solutions/sas7bdat-converter-cli"
 homepage = "https://github.com/pbs-data-solutions/sas7bdat-converter-cli"
 documentation = "https://github.com/pbs-data-solutions/sas7bdat-converter-cli"
```

### Comparing `sas7bdat_converter_cli-0.2.0/PKG-INFO` & `sas7bdat_converter_cli-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sas7bdat-converter-cli
-Version: 0.2.0
+Version: 1.0.0
 Summary: CLI to convert sas7bdat and xport files into other formats
 Home-page: https://github.com/pbs-data-solutions/sas7bdat-converter-cli
 License: MIT
 Keywords: sas,sas7bdat,converter,xpt,XPort
 Author: Paul Sanders
 Author-email: paul@pbsdatasolutions.com
 Requires-Python: >=3.8,<4.0
```

