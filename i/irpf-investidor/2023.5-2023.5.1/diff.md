# Comparing `tmp/irpf_investidor-2023.5.tar.gz` & `tmp/irpf_investidor-2023.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irpf_investidor-2023.5.tar", max compression
+gzip compressed data, was "irpf_investidor-2023.5.1.tar", max compression
```

## Comparing `irpf_investidor-2023.5.tar` & `irpf_investidor-2023.5.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1056 2023-05-01 05:03:11.920374 irpf_investidor-2023.5/LICENSE
--rw-r--r--   0        0        0     4628 2023-05-01 05:03:29.228535 irpf_investidor-2023.5/README.md
--rw-r--r--   0        0        0     1888 2023-05-01 05:03:29.228535 irpf_investidor-2023.5/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/__init__.py
--rw-r--r--   0        0        0     1449 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/__main__.py
--rw-r--r--   0        0        0    26239 2023-05-01 05:03:29.228535 irpf_investidor-2023.5/src/irpf_investidor/b3.py
--rw-r--r--   0        0        0     1272 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/formatting.py
--rw-r--r--   0        0        0     1002 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/prompt.py
--rw-r--r--   0        0        0        0 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/py.typed
--rw-r--r--   0        0        0     9200 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/report_reader.py
--rw-r--r--   0        0        0     1477 2023-05-01 05:03:11.924375 irpf_investidor-2023.5/src/irpf_investidor/responses.py
--rw-r--r--   0        0        0     5514 1970-01-01 00:00:00.000000 irpf_investidor-2023.5/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-26 04:39:21.013419 irpf_investidor-2023.5.1/LICENSE
+-rw-r--r--   0        0        0     4628 2023-05-26 04:39:21.013419 irpf_investidor-2023.5.1/README.md
+-rw-r--r--   0        0        0     1890 2023-05-26 04:39:37.209560 irpf_investidor-2023.5.1/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-26 04:39:21.013419 irpf_investidor-2023.5.1/src/irpf_investidor/__init__.py
+-rw-r--r--   0        0        0     1449 2023-05-26 04:39:21.013419 irpf_investidor-2023.5.1/src/irpf_investidor/__main__.py
+-rw-r--r--   0        0        0    26239 2023-05-26 04:39:21.017418 irpf_investidor-2023.5.1/src/irpf_investidor/b3.py
+-rw-r--r--   0        0        0     1272 2023-05-26 04:39:21.017418 irpf_investidor-2023.5.1/src/irpf_investidor/formatting.py
+-rw-r--r--   0        0        0     1002 2023-05-26 04:39:21.017418 irpf_investidor-2023.5.1/src/irpf_investidor/prompt.py
+-rw-r--r--   0        0        0        0 2023-05-26 04:39:21.017418 irpf_investidor-2023.5.1/src/irpf_investidor/py.typed
+-rw-r--r--   0        0        0     9200 2023-05-26 04:39:37.209560 irpf_investidor-2023.5.1/src/irpf_investidor/report_reader.py
+-rw-r--r--   0        0        0     1477 2023-05-26 04:39:21.017418 irpf_investidor-2023.5.1/src/irpf_investidor/responses.py
+-rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 irpf_investidor-2023.5.1/PKG-INFO
```

### Comparing `irpf_investidor-2023.5/LICENSE` & `irpf_investidor-2023.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `irpf_investidor-2023.5/README.md` & `irpf_investidor-2023.5.1/README.md`

 * *Files identical despite different names*

### Comparing `irpf_investidor-2023.5/pyproject.toml` & `irpf_investidor-2023.5.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "irpf-investidor"
-version = "2023.5"
+version = "2023.5.1"
 description = "IRPF Investidor"
 authors = ["staticdev <staticdev-support@proton.me>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/staticdev/irpf-investidor"
 repository = "https://github.com/staticdev/irpf-investidor"
 documentation = "https://irpf-investidor.readthedocs.io"
```

### Comparing `irpf_investidor-2023.5/src/irpf_investidor/__main__.py` & `irpf_investidor-2023.5.1/src/irpf_investidor/__main__.py`

 * *Files identical despite different names*

### Comparing `irpf_investidor-2023.5/src/irpf_investidor/b3.py` & `irpf_investidor-2023.5.1/src/irpf_investidor/b3.py`

 * *Files identical despite different names*

### Comparing `irpf_investidor-2023.5/src/irpf_investidor/formatting.py` & `irpf_investidor-2023.5.1/src/irpf_investidor/formatting.py`

 * *Files identical despite different names*

### Comparing `irpf_investidor-2023.5/src/irpf_investidor/prompt.py` & `irpf_investidor-2023.5.1/src/irpf_investidor/prompt.py`

 * *Files identical despite different names*

### Comparing `irpf_investidor-2023.5/src/irpf_investidor/report_reader.py` & `irpf_investidor-2023.5.1/src/irpf_investidor/report_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 IRPF_INVESTIMENT_CODES = {
     "ETF": "74 (ETF)",
     "FII": "73 (FII)",
     "STOCKS": "31 (Ações)",
     "NOT_FOUND": "Não encontrado",
 }
 FIRST_IMPLEMENTED_YEAR = 2019
-LAST_IMPLEMENTED_YEAR = 2021
+LAST_IMPLEMENTED_YEAR = 2022
 
 
 def get_xls_filename() -> str:
     """Return first xls filename in current folder or Downloads folder."""
     filenames = glob.glob("InfoCEI*.xls")
     if filenames:
         return filenames[0]
```

### Comparing `irpf_investidor-2023.5/src/irpf_investidor/responses.py` & `irpf_investidor-2023.5.1/src/irpf_investidor/responses.py`

 * *Files identical despite different names*

### Comparing `irpf_investidor-2023.5/PKG-INFO` & `irpf_investidor-2023.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irpf-investidor
-Version: 2023.5
+Version: 2023.5.1
 Summary: IRPF Investidor
 Home-page: https://github.com/staticdev/irpf-investidor
 License: MIT
 Author: staticdev
 Author-email: staticdev-support@proton.me
 Requires-Python: >=3.10
 Classifier: Development Status :: 5 - Production/Stable
```

