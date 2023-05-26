# Comparing `tmp/sababa-0.0.3.tar.gz` & `tmp/sababa-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sababa-0.0.3.tar", last modified: Wed Dec 28 17:48:01 2022, max compression
+gzip compressed data, was "sababa-0.0.4.tar", last modified: Fri May 26 18:19:37 2023, max compression
```

## Comparing `sababa-0.0.3.tar` & `sababa-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:48:01.111163 sababa-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2022-12-28 17:47:49.000000 sababa-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2022-12-28 17:47:49.000000 sababa-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      984 2022-12-28 17:48:01.111163 sababa-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14760 2022-12-28 17:47:49.000000 sababa-0.0.3/README-original.md
--rw-r--r--   0 runner    (1001) docker     (123)       57 2022-12-28 17:47:49.000000 sababa-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2022-12-28 17:47:49.000000 sababa-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      109 2022-12-28 17:48:01.111163 sababa-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1759 2022-12-28 17:47:49.000000 sababa-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:48:01.111163 sababa-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:48:01.111163 sababa-0.0.3/src/sababa/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2022-12-28 17:47:49.000000 sababa-0.0.3/src/sababa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2022-12-28 17:47:49.000000 sababa-0.0.3/src/sababa/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:48:01.111163 sababa-0.0.3/src/sababa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      984 2022-12-28 17:48:01.000000 sababa-0.0.3/src/sababa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      318 2022-12-28 17:48:01.000000 sababa-0.0.3/src/sababa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-28 17:48:01.000000 sababa-0.0.3/src/sababa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2022-12-28 17:48:01.000000 sababa-0.0.3/src/sababa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2022-12-28 17:48:01.000000 sababa-0.0.3/src/sababa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-28 17:48:01.111163 sababa-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      224 2022-12-28 17:47:49.000000 sababa-0.0.3/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:37.088389 sababa-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-26 18:19:22.000000 sababa-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-26 18:19:22.000000 sababa-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-26 18:19:37.088389 sababa-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14760 2023-05-26 18:19:22.000000 sababa-0.0.4/README-original.md
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 18:19:22.000000 sababa-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 18:19:22.000000 sababa-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 18:19:37.088389 sababa-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-26 18:19:22.000000 sababa-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:37.084389 sababa-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:37.088389 sababa-0.0.4/src/sababa/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 18:19:22.000000 sababa-0.0.4/src/sababa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-26 18:19:22.000000 sababa-0.0.4/src/sababa/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:37.088389 sababa-0.0.4/src/sababa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-05-26 18:19:36.000000 sababa-0.0.4/src/sababa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 18:19:37.000000 sababa-0.0.4/src/sababa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:19:36.000000 sababa-0.0.4/src/sababa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 18:19:36.000000 sababa-0.0.4/src/sababa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-26 18:19:36.000000 sababa-0.0.4/src/sababa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:19:37.088389 sababa-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-26 18:19:22.000000 sababa-0.0.4/tests/test_module1.py
```

### Comparing `sababa-0.0.3/LICENSE` & `sababa-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sababa-0.0.3/PKG-INFO` & `sababa-0.0.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sababa
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sababa PyPI Package
 Home-page: https://github.com/sababacloud/sababa-python
 Author: sababa
 Author-email: python@sababa.cloud
 Project-URL: Documentation, https://github.com/sababacloud/sababa-python
 Project-URL: Bug Reports, https://github.com/sababacloud/sababa-python/issues
 Project-URL: Source Code, https://github.com/sababacloud/sababa-python
```

### Comparing `sababa-0.0.3/README-original.md` & `sababa-0.0.4/README-original.md`

 * *Files identical despite different names*

### Comparing `sababa-0.0.3/setup.py` & `sababa-0.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `sababa-0.0.3/src/sababa.egg-info/PKG-INFO` & `sababa-0.0.4/src/sababa.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sababa
-Version: 0.0.3
+Version: 0.0.4
 Summary: Sababa PyPI Package
 Home-page: https://github.com/sababacloud/sababa-python
 Author: sababa
 Author-email: python@sababa.cloud
 Project-URL: Documentation, https://github.com/sababacloud/sababa-python
 Project-URL: Bug Reports, https://github.com/sababacloud/sababa-python/issues
 Project-URL: Source Code, https://github.com/sababacloud/sababa-python
```

