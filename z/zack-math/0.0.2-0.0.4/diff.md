# Comparing `tmp/zack_math-0.0.2.tar.gz` & `tmp/zack_math-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zack_math-0.0.2.tar", max compression
+gzip compressed data, was "zack_math-0.0.4.tar", max compression
```

## Comparing `zack_math-0.0.2.tar` & `zack_math-0.0.4.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1096 2023-05-26 19:14:05.655409 zack_math-0.0.2/LICENSE
--rw-r--r--   0        0        0       52 2023-05-26 19:14:05.655409 zack_math-0.0.2/README.md
--rw-r--r--   0        0        0      460 2023-05-26 19:14:05.655409 zack_math-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       23 2023-05-26 19:14:05.655409 zack_math-0.0.2/zack_math/__init__.py
--rw-r--r--   0        0        0      140 2023-05-26 19:14:05.655409 zack_math-0.0.2/zack_math/operators.py
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 zack_math-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-26 19:23:45.617156 zack_math-0.0.4/LICENSE
+-rw-r--r--   0        0        0       52 2023-05-26 19:23:45.617156 zack_math-0.0.4/README.md
+-rw-r--r--   0        0        0      460 2023-05-26 19:23:45.617156 zack_math-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-26 19:23:45.617156 zack_math-0.0.4/zack_math/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-26 19:23:45.617156 zack_math-0.0.4/zack_math/operators.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 zack_math-0.0.4/PKG-INFO
```

### Comparing `zack_math-0.0.2/LICENSE` & `zack_math-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `zack_math-0.0.2/PKG-INFO` & `zack_math-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zack-math
-Version: 0.0.2
+Version: 0.0.4
 Summary: a test project
 Home-page: https://github.com/kevinypfan/zack_math
 License: MIT
 Keywords: math,zack,zack_math
 Author: zackfan
 Author-email: zackfan@fugle.tw
 Requires-Python: >=3.7,<4.0
```

