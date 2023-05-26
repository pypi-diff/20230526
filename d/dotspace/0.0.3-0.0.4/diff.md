# Comparing `tmp/dotspace-0.0.3.tar.gz` & `tmp/dotspace-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotspace-0.0.3.tar", last modified: Fri May 26 16:42:19 2023, max compression
+gzip compressed data, was "dotspace-0.0.4.tar", last modified: Fri May 26 16:54:56 2023, max compression
```

## Comparing `dotspace-0.0.3.tar` & `dotspace-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:42:19.920454 dotspace-0.0.3/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-26 16:21:36.000000 dotspace-0.0.3/LICENSE
--rw-r--r--   0 mfsteele   (502) staff       (20)       87 2023-05-26 16:21:36.000000 dotspace-0.0.3/MANIFEST.in
--rw-r--r--   0 mfsteele   (502) staff       (20)     1754 2023-05-26 16:42:19.920296 dotspace-0.0.3/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)       41 2023-05-26 16:21:36.000000 dotspace-0.0.3/README.md
--rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-26 16:42:14.000000 dotspace-0.0.3/pyproject.toml
--rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-26 16:42:19.920528 dotspace-0.0.3/setup.cfg
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:42:19.914128 dotspace-0.0.3/src/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:42:19.915380 dotspace-0.0.3/src/dotspace/
--rw-r--r--   0 mfsteele   (502) staff       (20)       26 2023-05-26 16:42:14.000000 dotspace-0.0.3/src/dotspace/__init__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)       74 2023-05-26 16:21:36.000000 dotspace-0.0.3/src/dotspace/__main__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)      256 2023-05-26 16:41:24.000000 dotspace-0.0.3/src/dotspace/dotspace.py
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:42:19.914251 dotspace-0.0.3/src/dotspace/inc/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:42:19.916628 dotspace-0.0.3/src/dotspace/inc/json/
--rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 dotspace-0.0.3/src/dotspace/inc/json/dict_tracy.json
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:42:19.916480 dotspace-0.0.3/src/dotspace.egg-info/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1754 2023-05-26 16:42:19.000000 dotspace-0.0.3/src/dotspace.egg-info/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)      375 2023-05-26 16:42:19.000000 dotspace-0.0.3/src/dotspace.egg-info/SOURCES.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-26 16:42:19.000000 dotspace-0.0.3/src/dotspace.egg-info/dependency_links.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       52 2023-05-26 16:42:19.000000 dotspace-0.0.3/src/dotspace.egg-info/entry_points.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-26 16:42:19.000000 dotspace-0.0.3/src/dotspace.egg-info/requires.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        9 2023-05-26 16:42:19.000000 dotspace-0.0.3/src/dotspace.egg-info/top_level.txt
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:54:56.977231 dotspace-0.0.4/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-26 16:21:36.000000 dotspace-0.0.4/LICENSE
+-rw-r--r--   0 mfsteele   (502) staff       (20)       87 2023-05-26 16:21:36.000000 dotspace-0.0.4/MANIFEST.in
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1754 2023-05-26 16:54:56.977073 dotspace-0.0.4/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)       41 2023-05-26 16:21:36.000000 dotspace-0.0.4/README.md
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-26 16:54:51.000000 dotspace-0.0.4/pyproject.toml
+-rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-26 16:54:56.977276 dotspace-0.0.4/setup.cfg
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:54:56.972051 dotspace-0.0.4/src/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:54:56.973331 dotspace-0.0.4/src/dotspace/
+-rw-r--r--   0 mfsteele   (502) staff       (20)       26 2023-05-26 16:54:51.000000 dotspace-0.0.4/src/dotspace/__init__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)       74 2023-05-26 16:21:36.000000 dotspace-0.0.4/src/dotspace/__main__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)      252 2023-05-26 16:54:17.000000 dotspace-0.0.4/src/dotspace/dots.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:54:56.972174 dotspace-0.0.4/src/dotspace/inc/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:54:56.974394 dotspace-0.0.4/src/dotspace/inc/json/
+-rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 dotspace-0.0.4/src/dotspace/inc/json/dict_tracy.json
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:54:56.974267 dotspace-0.0.4/src/dotspace.egg-info/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1754 2023-05-26 16:54:56.000000 dotspace-0.0.4/src/dotspace.egg-info/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)      385 2023-05-26 16:54:56.000000 dotspace-0.0.4/src/dotspace.egg-info/SOURCES.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-26 16:54:56.000000 dotspace-0.0.4/src/dotspace.egg-info/dependency_links.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       52 2023-05-26 16:54:56.000000 dotspace-0.0.4/src/dotspace.egg-info/entry_points.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-26 16:54:56.000000 dotspace-0.0.4/src/dotspace.egg-info/requires.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        9 2023-05-26 16:54:56.000000 dotspace-0.0.4/src/dotspace.egg-info/top_level.txt
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:54:56.976869 dotspace-0.0.4/tests/
+-rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:47:50.000000 dotspace-0.0.4/tests/test.py
```

### Comparing `dotspace-0.0.3/LICENSE` & `dotspace-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dotspace-0.0.3/PKG-INFO` & `dotspace-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotspace
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access Nested Data with Dots
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dotspace-0.0.3/pyproject.toml` & `dotspace-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dotspace"
-version = "0.0.3"
+version = "0.0.4"
 description = "Access Nested Data with Dots"
 readme = "README.md"
 authors = [{ name = "Mike Steele", email = "mike@mikesteele.us" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -29,15 +29,15 @@
 [project.urls]
 Homepage = "https://github.com/soulrx/dotspace"
 
 [project.scripts]
 dotspace = "dotspace.__main__:main"
 
 [tool.bumpver]
-current_version = "0.0.3"
+current_version = "0.0.4"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `dotspace-0.0.3/src/dotspace/inc/json/dict_tracy.json` & `dotspace-0.0.4/src/dotspace/inc/json/dict_tracy.json`

 * *Files identical despite different names*

### Comparing `dotspace-0.0.3/src/dotspace.egg-info/PKG-INFO` & `dotspace-0.0.4/src/dotspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotspace
-Version: 0.0.3
+Version: 0.0.4
 Summary: Access Nested Data with Dots
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

