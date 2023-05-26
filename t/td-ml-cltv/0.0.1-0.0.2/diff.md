# Comparing `tmp/td_ml_cltv-0.0.1.tar.gz` & `tmp/td_ml_cltv-0.0.2.tar.gz`

## Comparing `td_ml_cltv-0.0.1.tar` & `td_ml_cltv-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.1/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.1/src/td_ml_cltv/__init__.py
--rw-r--r--   0        0        0    12650 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.1/src/td_ml_cltv/cltv_helpers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.1/LICENSE
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.1/README.md
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.2/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.2/src/td_ml_cltv/__init__.py
+-rw-r--r--   0        0        0    12650 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.2/src/td_ml_cltv/cltv_helpers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.2/LICENSE
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.2/README.md
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 td_ml_cltv-0.0.2/PKG-INFO
```

### Comparing `td_ml_cltv-0.0.1/.DS_Store` & `td_ml_cltv-0.0.2/.DS_Store`

 * *Files identical despite different names*

### Comparing `td_ml_cltv-0.0.1/src/td_ml_cltv/cltv_helpers.py` & `td_ml_cltv-0.0.2/src/td_ml_cltv/cltv_helpers.py`

 * *Files identical despite different names*

### Comparing `td_ml_cltv-0.0.1/pyproject.toml` & `td_ml_cltv-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "td_ml_cltv"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Yish Lim", email="yish.lim@treasure-data.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

