# Comparing `tmp/jsonpatchplus-0.1.0.tar.gz` & `tmp/jsonpatchplus-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonpatchplus-0.1.0.tar", last modified: Wed May 24 03:21:01 2023, max compression
+gzip compressed data, was "jsonpatchplus-0.1.1.tar", last modified: Fri May 26 02:41:02 2023, max compression
```

## Comparing `jsonpatchplus-0.1.0.tar` & `jsonpatchplus-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 elm        (501) staff       (20)        0 2023-05-24 03:21:01.866681 jsonpatchplus-0.1.0/
--rw-r--r--   0 elm        (501) staff       (20)     1068 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/LICENSE
--rw-r--r--   0 elm        (501) staff       (20)     1512 2023-05-24 03:21:01.866273 jsonpatchplus-0.1.0/PKG-INFO
--rw-r--r--   0 elm        (501) staff       (20)       13 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/README.md
--rw-r--r--   0 elm        (501) staff       (20)      582 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/pyproject.toml
--rw-r--r--   0 elm        (501) staff       (20)       38 2023-05-24 03:21:01.866819 jsonpatchplus-0.1.0/setup.cfg
-drwxr-xr-x   0 elm        (501) staff       (20)        0 2023-05-24 03:21:01.840151 jsonpatchplus-0.1.0/src/
-drwxr-xr-x   0 elm        (501) staff       (20)        0 2023-05-24 03:21:01.844140 jsonpatchplus-0.1.0/src/jsonpatchplus/
--rw-r--r--   0 elm        (501) staff       (20)      102 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/src/jsonpatchplus/__init__.py
--rw-r--r--   0 elm        (501) staff       (20)     4202 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/src/jsonpatchplus/core.py
--rw-r--r--   0 elm        (501) staff       (20)     1155 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/src/jsonpatchplus/ctypes.py
--rw-r--r--   0 elm        (501) staff       (20)      276 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/src/jsonpatchplus/exceptions.py
-drwxr-xr-x   0 elm        (501) staff       (20)        0 2023-05-24 03:21:01.865651 jsonpatchplus-0.1.0/src/jsonpatchplus/loaders/
--rw-r--r--   0 elm        (501) staff       (20)      163 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/src/jsonpatchplus/loaders/__init__.py
--rw-r--r--   0 elm        (501) staff       (20)      795 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/src/jsonpatchplus/loaders/jsonpatch.py
--rw-r--r--   0 elm        (501) staff       (20)     2863 2023-05-24 03:19:06.000000 jsonpatchplus-0.1.0/src/jsonpatchplus/loaders/jsonpatchplus.py
-drwxr-xr-x   0 elm        (501) staff       (20)        0 2023-05-24 03:21:01.864044 jsonpatchplus-0.1.0/src/jsonpatchplus.egg-info/
--rw-r--r--   0 elm        (501) staff       (20)     1512 2023-05-24 03:21:01.000000 jsonpatchplus-0.1.0/src/jsonpatchplus.egg-info/PKG-INFO
--rw-r--r--   0 elm        (501) staff       (20)      472 2023-05-24 03:21:01.000000 jsonpatchplus-0.1.0/src/jsonpatchplus.egg-info/SOURCES.txt
--rw-r--r--   0 elm        (501) staff       (20)        1 2023-05-24 03:21:01.000000 jsonpatchplus-0.1.0/src/jsonpatchplus.egg-info/dependency_links.txt
--rw-r--r--   0 elm        (501) staff       (20)       49 2023-05-24 03:21:01.000000 jsonpatchplus-0.1.0/src/jsonpatchplus.egg-info/requires.txt
--rw-r--r--   0 elm        (501) staff       (20)       14 2023-05-24 03:21:01.000000 jsonpatchplus-0.1.0/src/jsonpatchplus.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.340405 jsonpatchplus-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 02:41:02.340405 jsonpatchplus-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 02:41:02.340405 jsonpatchplus-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.336405 jsonpatchplus-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.336405 jsonpatchplus-0.1.1/src/jsonpatchplus/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4202 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.340405 jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/jsonpatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-05-26 02:40:52.000000 jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/jsonpatchplus.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 02:41:02.336405 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 02:41:02.000000 jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/top_level.txt
```

### Comparing `jsonpatchplus-0.1.0/LICENSE` & `jsonpatchplus-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonpatchplus-0.1.0/PKG-INFO` & `jsonpatchplus-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonpatchplus
-Version: 0.1.0
+Version: 0.1.1
 Summary: JsonPatch+
 Author-email: Elmer Nocon <elmernocon@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Elmer Nocon
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `jsonpatchplus-0.1.0/pyproject.toml` & `jsonpatchplus-0.1.1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 
 [project]
 name = "jsonpatchplus"
 description = "JsonPatch+"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
+    "jsonpatch",
+    "jsonpointer",
     "PyYAML",
 ]
 license = {file = "LICENSE"}
 authors = [
     {name = "Elmer Nocon", email = "elmernocon@gmail.com"},
 ]
 dynamic = [
```

### Comparing `jsonpatchplus-0.1.0/src/jsonpatchplus/core.py` & `jsonpatchplus-0.1.1/src/jsonpatchplus/core.py`

 * *Files identical despite different names*

### Comparing `jsonpatchplus-0.1.0/src/jsonpatchplus/ctypes.py` & `jsonpatchplus-0.1.1/src/jsonpatchplus/ctypes.py`

 * *Files identical despite different names*

### Comparing `jsonpatchplus-0.1.0/src/jsonpatchplus/loaders/jsonpatch.py` & `jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/jsonpatch.py`

 * *Files identical despite different names*

### Comparing `jsonpatchplus-0.1.0/src/jsonpatchplus/loaders/jsonpatchplus.py` & `jsonpatchplus-0.1.1/src/jsonpatchplus/loaders/jsonpatchplus.py`

 * *Files identical despite different names*

### Comparing `jsonpatchplus-0.1.0/src/jsonpatchplus.egg-info/PKG-INFO` & `jsonpatchplus-0.1.1/src/jsonpatchplus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonpatchplus
-Version: 0.1.0
+Version: 0.1.1
 Summary: JsonPatch+
 Author-email: Elmer Nocon <elmernocon@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Elmer Nocon
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

