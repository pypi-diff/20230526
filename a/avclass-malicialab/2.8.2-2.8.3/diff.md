# Comparing `tmp/avclass-malicialab-2.8.2.tar.gz` & `tmp/avclass-malicialab-2.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avclass-malicialab-2.8.2.tar", last modified: Fri May  5 15:20:07 2023, max compression
+gzip compressed data, was "avclass-malicialab-2.8.3.tar", last modified: Fri May 26 13:04:36 2023, max compression
```

## Comparing `avclass-malicialab-2.8.2.tar` & `avclass-malicialab-2.8.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-05 15:20:07.197136 avclass-malicialab-2.8.2/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.2/LICENSE
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.2/MANIFEST.in
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-05-05 15:20:07.197136 avclass-malicialab-2.8.2/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.2/README.md
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-05 15:20:07.197136 avclass-malicialab-2.8.2/avclass/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.2/avclass/__init__.py
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    20596 2023-05-05 15:16:06.000000 avclass-malicialab-2.8.2/avclass/common.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-05 15:20:07.197136 avclass-malicialab-2.8.2/avclass/data/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.2/avclass/data/andropup.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.2/avclass/data/default.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    56429 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.2/avclass/data/default.tagging
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    41254 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.2/avclass/data/default.taxonomy
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.2/avclass/evaluate.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23606 2023-02-27 10:51:54.000000 avclass-malicialab-2.8.2/avclass/labeler.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.2/avclass/misp.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.2/avclass/normalize.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.2/avclass/update.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-05 15:20:07.197136 avclass-malicialab-2.8.2/avclass_malicialab.egg-info/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-05-05 15:20:07.000000 avclass-malicialab-2.8.2/avclass_malicialab.egg-info/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-05-05 15:20:07.000000 avclass-malicialab-2.8.2/avclass_malicialab.egg-info/SOURCES.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-05-05 15:20:07.000000 avclass-malicialab-2.8.2/avclass_malicialab.egg-info/dependency_links.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-05-05 15:20:07.000000 avclass-malicialab-2.8.2/avclass_malicialab.egg-info/entry_points.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-05-05 15:20:07.000000 avclass-malicialab-2.8.2/avclass_malicialab.egg-info/top_level.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-05-05 15:18:55.000000 avclass-malicialab-2.8.2/pyproject.toml
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-05-05 15:20:07.197136 avclass-malicialab-2.8.2/setup.cfg
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.3/LICENSE
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.3/MANIFEST.in
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.3/README.md
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/avclass/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.3/avclass/__init__.py
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    20596 2023-05-05 15:16:06.000000 avclass-malicialab-2.8.3/avclass/common.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/avclass/data/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.3/avclass/data/andropup.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.3/avclass/data/default.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    56429 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.3/avclass/data/default.tagging
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    41254 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.3/avclass/data/default.taxonomy
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.3/avclass/evaluate.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23609 2023-05-26 13:02:48.000000 avclass-malicialab-2.8.3/avclass/labeler.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.3/avclass/misp.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.3/avclass/normalize.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.3/avclass/update.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/entry_points.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-05-26 13:04:36.000000 avclass-malicialab-2.8.3/avclass_malicialab.egg-info/top_level.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-05-26 13:03:02.000000 avclass-malicialab-2.8.3/pyproject.toml
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-05-26 13:04:36.697236 avclass-malicialab-2.8.3/setup.cfg
```

### Comparing `avclass-malicialab-2.8.2/LICENSE` & `avclass-malicialab-2.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/PKG-INFO` & `avclass-malicialab-2.8.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.2
+Version: 2.8.3
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.2/README.md` & `avclass-malicialab-2.8.3/README.md`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass/common.py` & `avclass-malicialab-2.8.3/avclass/common.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass/data/andropup.expansion` & `avclass-malicialab-2.8.3/avclass/data/andropup.expansion`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass/data/default.tagging` & `avclass-malicialab-2.8.3/avclass/data/default.tagging`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass/data/default.taxonomy` & `avclass-malicialab-2.8.3/avclass/data/default.taxonomy`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass/evaluate.py` & `avclass-malicialab-2.8.3/avclass/evaluate.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass/labeler.py` & `avclass-malicialab-2.8.3/avclass/labeler.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
     else:
         log.info('[-] Using default expansion tags in %s' % DEFAULT_EXP_PATH)
 
     if args.av:
         log.info("[-] Using AV engines in %s" % args.av)
 
     # Build list of input files
-    files = set(args.f) if args.f is not None else {}
+    files = set(args.f) if args.f is not None else set()
     if args.d:
         for d in args.d:
             if os.path.isdir:
                 for f in os.listdir(d):
                     filepath = os.path.join(d, f)
                     if os.path.isfile(filepath):
                         files.add(filepath)
```

### Comparing `avclass-malicialab-2.8.2/avclass/misp.py` & `avclass-malicialab-2.8.3/avclass/misp.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass/normalize.py` & `avclass-malicialab-2.8.3/avclass/normalize.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass/update.py` & `avclass-malicialab-2.8.3/avclass/update.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.2/avclass_malicialab.egg-info/PKG-INFO` & `avclass-malicialab-2.8.3/avclass_malicialab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.2
+Version: 2.8.3
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.2/pyproject.toml` & `avclass-malicialab-2.8.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avclass-malicialab"
-version = "2.8.2"
+version = "2.8.3"
 description = "AVClass is a Python package and command line tool to tag / label malware samples."
 readme = "README.md"
 authors = [{ name = "MaliciaLab" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

