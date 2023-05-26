# Comparing `tmp/prfiesta-0.8.1b139.tar.gz` & `tmp/prfiesta-0.8.1b140.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.8.1b139.tar", max compression
+gzip compressed data, was "prfiesta-0.8.1b140.tar", max compression
```

## Comparing `prfiesta-0.8.1b139.tar` & `prfiesta-0.8.1b140.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-26 20:14:59.089743 prfiesta-0.8.1b139/LICENSE
--rw-r--r--   0        0        0     8016 2023-05-26 20:14:59.089743 prfiesta-0.8.1b139/README.md
--rw-r--r--   0        0        0      487 2023-05-26 20:14:59.097743 prfiesta-0.8.1b139/prfiesta/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-26 20:14:59.097743 prfiesta-0.8.1b139/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-26 20:14:59.097743 prfiesta-0.8.1b139/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-26 20:14:59.097743 prfiesta-0.8.1b139/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-26 20:14:59.097743 prfiesta-0.8.1b139/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-26 20:14:59.097743 prfiesta-0.8.1b139/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     4981 2023-05-26 20:14:59.101743 prfiesta-0.8.1b139/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-26 20:14:59.101743 prfiesta-0.8.1b139/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-26 20:14:59.101743 prfiesta-0.8.1b139/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-26 20:14:59.101743 prfiesta-0.8.1b139/prfiesta/spinner.py
--rw-r--r--   0        0        0     3199 2023-05-26 20:15:09.425891 prfiesta-0.8.1b139/pyproject.toml
--rw-r--r--   0        0        0     9377 1970-01-01 00:00:00.000000 prfiesta-0.8.1b139/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-26 20:20:18.733292 prfiesta-0.8.1b140/LICENSE
+-rw-r--r--   0        0        0     8016 2023-05-26 20:20:18.733292 prfiesta-0.8.1b140/README.md
+-rw-r--r--   0        0        0      487 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     4981 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-26 20:20:18.741292 prfiesta-0.8.1b140/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3199 2023-05-26 20:20:31.597472 prfiesta-0.8.1b140/pyproject.toml
+-rw-r--r--   0        0        0     9377 1970-01-01 00:00:00.000000 prfiesta-0.8.1b140/PKG-INFO
```

### Comparing `prfiesta-0.8.1b139/LICENSE` & `prfiesta-0.8.1b140/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b139/README.md` & `prfiesta-0.8.1b140/README.md`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b139/prfiesta/__main__.py` & `prfiesta-0.8.1b140/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b139/prfiesta/analysis/plot.py` & `prfiesta-0.8.1b140/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b139/prfiesta/analysis/view.py` & `prfiesta-0.8.1b140/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b139/prfiesta/collectors/github.py` & `prfiesta-0.8.1b140/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b139/prfiesta/environment.py` & `prfiesta-0.8.1b140/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b139/prfiesta/output.py` & `prfiesta-0.8.1b140/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.1b139/pyproject.toml` & `prfiesta-0.8.1b140/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.8.1b139"
+version = "0.8.1b140"
 description = "Collect and Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.8.1b139/PKG-INFO` & `prfiesta-0.8.1b140/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.8.1b139
+Version: 0.8.1b140
 Summary: Collect and Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
```

