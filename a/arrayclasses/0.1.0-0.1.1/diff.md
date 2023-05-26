# Comparing `tmp/arrayclasses-0.1.0.tar.gz` & `tmp/arrayclasses-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrayclasses-0.1.0.tar", max compression
+gzip compressed data, was "arrayclasses-0.1.1.tar", max compression
```

## Comparing `arrayclasses-0.1.0.tar` & `arrayclasses-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      406 2023-05-26 18:21:10.162650 arrayclasses-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      121 2023-05-26 18:28:15.092746 arrayclasses-0.1.0/src/arrayclasses/__init__.py
--rw-r--r--   0        0        0     3295 2023-05-26 18:31:27.283474 arrayclasses-0.1.0/src/arrayclasses/wrapper.py
--rw-r--r--   0        0        0      730 2023-05-26 18:42:14.595666 arrayclasses-0.1.0/setup.py
--rw-r--r--   0        0        0      476 2023-05-26 18:42:14.595898 arrayclasses-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-26 18:48:49.288191 arrayclasses-0.1.1/LICENSE
+-rw-r--r--   0        0        0      731 2023-05-26 18:39:05.635839 arrayclasses-0.1.1/README.md
+-rw-r--r--   0        0        0      667 2023-05-26 18:45:09.172843 arrayclasses-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-05-26 18:28:15.092746 arrayclasses-0.1.1/src/arrayclasses/__init__.py
+-rw-r--r--   0        0        0     3295 2023-05-26 18:31:27.283474 arrayclasses-0.1.1/src/arrayclasses/wrapper.py
+-rw-r--r--   0        0        0     1533 2023-05-26 18:49:19.350574 arrayclasses-0.1.1/setup.py
+-rw-r--r--   0        0        0     1405 2023-05-26 18:49:19.350813 arrayclasses-0.1.1/PKG-INFO
```

### Comparing `arrayclasses-0.1.0/src/arrayclasses/wrapper.py` & `arrayclasses-0.1.1/src/arrayclasses/wrapper.py`

 * *Files identical despite different names*

