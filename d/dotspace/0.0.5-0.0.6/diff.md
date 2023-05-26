# Comparing `tmp/dotspace-0.0.5.tar.gz` & `tmp/dotspace-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotspace-0.0.5.tar", last modified: Fri May 26 17:09:17 2023, max compression
+gzip compressed data, was "dotspace-0.0.6.tar", last modified: Fri May 26 17:20:25 2023, max compression
```

## Comparing `dotspace-0.0.5.tar` & `dotspace-0.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:09:17.877991 dotspace-0.0.5/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-26 16:21:36.000000 dotspace-0.0.5/LICENSE
--rw-r--r--   0 mfsteele   (502) staff       (20)       87 2023-05-26 16:21:36.000000 dotspace-0.0.5/MANIFEST.in
--rw-r--r--   0 mfsteele   (502) staff       (20)     1754 2023-05-26 17:09:17.877851 dotspace-0.0.5/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)       41 2023-05-26 16:21:36.000000 dotspace-0.0.5/README.md
--rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-26 17:09:12.000000 dotspace-0.0.5/pyproject.toml
--rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-26 17:09:17.878039 dotspace-0.0.5/setup.cfg
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:09:17.872807 dotspace-0.0.5/src/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:09:17.874007 dotspace-0.0.5/src/dotspace/
--rw-r--r--   0 mfsteele   (502) staff       (20)       56 2023-05-26 17:09:12.000000 dotspace-0.0.5/src/dotspace/__init__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)       74 2023-05-26 16:21:36.000000 dotspace-0.0.5/src/dotspace/__main__.py
--rw-r--r--   0 mfsteele   (502) staff       (20)      252 2023-05-26 16:54:17.000000 dotspace-0.0.5/src/dotspace/dots.py
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:09:17.872929 dotspace-0.0.5/src/dotspace/inc/
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:09:17.875102 dotspace-0.0.5/src/dotspace/inc/json/
--rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 dotspace-0.0.5/src/dotspace/inc/json/dict_tracy.json
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:09:17.874971 dotspace-0.0.5/src/dotspace.egg-info/
--rw-r--r--   0 mfsteele   (502) staff       (20)     1754 2023-05-26 17:09:17.000000 dotspace-0.0.5/src/dotspace.egg-info/PKG-INFO
--rw-r--r--   0 mfsteele   (502) staff       (20)      385 2023-05-26 17:09:17.000000 dotspace-0.0.5/src/dotspace.egg-info/SOURCES.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-26 17:09:17.000000 dotspace-0.0.5/src/dotspace.egg-info/dependency_links.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       52 2023-05-26 17:09:17.000000 dotspace-0.0.5/src/dotspace.egg-info/entry_points.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-26 17:09:17.000000 dotspace-0.0.5/src/dotspace.egg-info/requires.txt
--rw-r--r--   0 mfsteele   (502) staff       (20)        9 2023-05-26 17:09:17.000000 dotspace-0.0.5/src/dotspace.egg-info/top_level.txt
-drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:09:17.877671 dotspace-0.0.5/tests/
--rw-r--r--   0 mfsteele   (502) staff       (20)        0 2023-05-26 16:47:50.000000 dotspace-0.0.5/tests/test.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:20:25.321124 dotspace-0.0.6/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1063 2023-05-26 16:21:36.000000 dotspace-0.0.6/LICENSE
+-rw-r--r--   0 mfsteele   (502) staff       (20)       87 2023-05-26 16:21:36.000000 dotspace-0.0.6/MANIFEST.in
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1754 2023-05-26 17:20:25.320990 dotspace-0.0.6/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)       41 2023-05-26 16:21:36.000000 dotspace-0.0.6/README.md
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1139 2023-05-26 17:20:20.000000 dotspace-0.0.6/pyproject.toml
+-rw-r--r--   0 mfsteele   (502) staff       (20)       38 2023-05-26 17:20:25.321170 dotspace-0.0.6/setup.cfg
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:20:25.316242 dotspace-0.0.6/src/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:20:25.317480 dotspace-0.0.6/src/dotspace/
+-rw-r--r--   0 mfsteele   (502) staff       (20)       56 2023-05-26 17:20:20.000000 dotspace-0.0.6/src/dotspace/__init__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)       74 2023-05-26 16:21:36.000000 dotspace-0.0.6/src/dotspace/__main__.py
+-rw-r--r--   0 mfsteele   (502) staff       (20)      254 2023-05-26 17:12:53.000000 dotspace-0.0.6/src/dotspace/dots.py
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:20:25.316366 dotspace-0.0.6/src/dotspace/inc/
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:20:25.318546 dotspace-0.0.6/src/dotspace/inc/json/
+-rw-r--r--   0 mfsteele   (502) staff       (20)  1606047 2023-05-23 19:17:04.000000 dotspace-0.0.6/src/dotspace/inc/json/dict_tracy.json
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:20:25.318416 dotspace-0.0.6/src/dotspace.egg-info/
+-rw-r--r--   0 mfsteele   (502) staff       (20)     1754 2023-05-26 17:20:25.000000 dotspace-0.0.6/src/dotspace.egg-info/PKG-INFO
+-rw-r--r--   0 mfsteele   (502) staff       (20)      385 2023-05-26 17:20:25.000000 dotspace-0.0.6/src/dotspace.egg-info/SOURCES.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        1 2023-05-26 17:20:25.000000 dotspace-0.0.6/src/dotspace.egg-info/dependency_links.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       52 2023-05-26 17:20:25.000000 dotspace-0.0.6/src/dotspace.egg-info/entry_points.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)       64 2023-05-26 17:20:25.000000 dotspace-0.0.6/src/dotspace.egg-info/requires.txt
+-rw-r--r--   0 mfsteele   (502) staff       (20)        9 2023-05-26 17:20:25.000000 dotspace-0.0.6/src/dotspace.egg-info/top_level.txt
+drwxr-xr-x   0 mfsteele   (502) staff       (20)        0 2023-05-26 17:20:25.320781 dotspace-0.0.6/tests/
+-rw-r--r--   0 mfsteele   (502) staff       (20)      216 2023-05-26 17:19:53.000000 dotspace-0.0.6/tests/test.py
```

### Comparing `dotspace-0.0.5/LICENSE` & `dotspace-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dotspace-0.0.5/PKG-INFO` & `dotspace-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotspace
-Version: 0.0.5
+Version: 0.0.6
 Summary: Access Nested Data with Dots
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dotspace-0.0.5/pyproject.toml` & `dotspace-0.0.6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dotspace"
-version = "0.0.5"
+version = "0.0.6"
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
-current_version = "0.0.5"
+current_version = "0.0.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `dotspace-0.0.5/src/dotspace/inc/json/dict_tracy.json` & `dotspace-0.0.6/src/dotspace/inc/json/dict_tracy.json`

 * *Files identical despite different names*

### Comparing `dotspace-0.0.5/src/dotspace.egg-info/PKG-INFO` & `dotspace-0.0.6/src/dotspace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotspace
-Version: 0.0.5
+Version: 0.0.6
 Summary: Access Nested Data with Dots
 Author-email: Mike Steele <mike@mikesteele.us>
 License: MIT License
         
         Copyright (c) 2023 soulrx
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

