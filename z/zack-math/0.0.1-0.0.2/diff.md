# Comparing `tmp/zack_math-0.0.1.tar.gz` & `tmp/zack_math-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zack_math-0.0.1.tar", max compression
+gzip compressed data, was "zack_math-0.0.2.tar", max compression
```

## Comparing `zack_math-0.0.1.tar` & `zack_math-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,6 @@
--rw-r--r--   0        0        0     1096 2023-05-26 11:52:20.701309 zack_math-0.0.1/LICENSE
--rw-r--r--   0        0        0       52 2023-05-26 11:51:28.055200 zack_math-0.0.1/README.md
--rw-r--r--   0        0        0      460 2023-05-26 12:13:35.994801 zack_math-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       45 2023-05-26 11:56:39.081395 zack_math-0.0.1/zack_math/__init__.py
--rw-r--r--   0        0        0      140 2023-05-26 11:56:07.401248 zack_math-0.0.1/zack_math/index.py
--rw-r--r--   0        0        0      403 2023-05-26 12:33:21.728402 zack_math-0.0.1/zack_math/zack_math.egg-info/PKG-INFO
--rw-r--r--   0        0        0        0 2023-05-26 12:31:14.395853 zack_math-0.0.1/zack_math/zack_math.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2023-05-26 12:33:21.728520 zack_math-0.0.1/zack_math/zack_math.egg-info/dependency_links.txt
--rw-r--r--   0        0        0       20 2023-05-26 12:33:21.728646 zack_math-0.0.1/zack_math/zack_math.egg-info/top_level.txt
--rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 zack_math-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-05-26 19:14:05.655409 zack_math-0.0.2/LICENSE
+-rw-r--r--   0        0        0       52 2023-05-26 19:14:05.655409 zack_math-0.0.2/README.md
+-rw-r--r--   0        0        0      460 2023-05-26 19:14:05.655409 zack_math-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       23 2023-05-26 19:14:05.655409 zack_math-0.0.2/zack_math/__init__.py
+-rw-r--r--   0        0        0      140 2023-05-26 19:14:05.655409 zack_math-0.0.2/zack_math/operators.py
+-rw-r--r--   0        0        0      756 1970-01-01 00:00:00.000000 zack_math-0.0.2/PKG-INFO
```

### Comparing `zack_math-0.0.1/LICENSE` & `zack_math-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `zack_math-0.0.1/PKG-INFO` & `zack_math-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zack-math
-Version: 0.0.1
+Version: 0.0.2
 Summary: a test project
 Home-page: https://github.com/kevinypfan/zack_math
 License: MIT
 Keywords: math,zack,zack_math
 Author: zackfan
 Author-email: zackfan@fugle.tw
 Requires-Python: >=3.7,<4.0
```

