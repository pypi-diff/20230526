# Comparing `tmp/hashkern-0.3.2.tar.gz` & `tmp/hashkern-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashkern-0.3.2.tar", last modified: Thu May 25 21:54:00 2023, max compression
+gzip compressed data, was "hashkern-0.3.3.tar", last modified: Thu May 25 21:59:40 2023, max compression
```

## Comparing `hashkern-0.3.2.tar` & `hashkern-0.3.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:54:00.077934 hashkern-0.3.2/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    11344 2023-01-13 23:42:17.000000 hashkern-0.3.2/LICENSE
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14841 2023-05-25 21:54:00.077934 hashkern-0.3.2/PKG-INFO
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14107 2023-05-25 21:38:34.000000 hashkern-0.3.2/README.md
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       38 2023-05-25 21:54:00.077934 hashkern-0.3.2/setup.cfg
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     1231 2023-05-25 21:49:20.000000 hashkern-0.3.2/setup.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:54:00.073933 hashkern-0.3.2/src/
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:54:00.073933 hashkern-0.3.2/src/hash/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      239 2023-05-10 20:44:27.000000 hashkern-0.3.2/src/hash/__init__.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:54:00.073933 hashkern-0.3.2/src/hash/cli/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       23 2023-01-14 12:45:56.000000 hashkern-0.3.2/src/hash/cli/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5912 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/cli/main.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7189 2023-01-13 23:42:17.000000 hashkern-0.3.2/src/hash/dag.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     2148 2023-05-14 21:16:53.000000 hashkern-0.3.2/src/hash/errors.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:54:00.073933 hashkern-0.3.2/src/hash/kern/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      148 2023-05-25 21:49:40.000000 hashkern-0.3.2/src/hash/kern/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    10412 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/kern/action.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7361 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/kern/execute.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      931 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/kern/hash.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3196 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/kern/main.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    16126 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/kern/planner.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     4181 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/kern/secrets.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    19277 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/kern/state.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5952 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/kern/templates.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3461 2023-01-13 23:42:17.000000 hashkern-0.3.2/src/hash/logs.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:54:00.077934 hashkern-0.3.2/src/hash/resources/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       69 2023-05-14 22:02:35.000000 hashkern-0.3.2/src/hash/resources/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    97796 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/resources/base.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    22702 2023-05-15 21:31:58.000000 hashkern-0.3.2/src/hash/resources/targets.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:54:00.077934 hashkern-0.3.2/src/hash/store/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       59 2023-01-13 23:42:17.000000 hashkern-0.3.2/src/hash/store/__init__.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    28132 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/store/base.py
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    12523 2023-05-25 21:36:32.000000 hashkern-0.3.2/src/hash/utils.py
-drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:54:00.077934 hashkern-0.3.2/src/hashkern.egg-info/
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14841 2023-05-25 21:54:00.000000 hashkern-0.3.2/src/hashkern.egg-info/PKG-INFO
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      738 2023-05-25 21:54:00.000000 hashkern-0.3.2/src/hashkern.egg-info/SOURCES.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        1 2023-05-25 21:54:00.000000 hashkern-0.3.2/src/hashkern.egg-info/dependency_links.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       39 2023-05-25 21:54:00.000000 hashkern-0.3.2/src/hashkern.egg-info/entry_points.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      213 2023-05-25 21:54:00.000000 hashkern-0.3.2/src/hashkern.egg-info/requires.txt
--rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        5 2023-05-25 21:54:00.000000 hashkern-0.3.2/src/hashkern.egg-info/top_level.txt
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    11344 2023-01-13 23:42:17.000000 hashkern-0.3.3/LICENSE
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14841 2023-05-25 21:59:40.606595 hashkern-0.3.3/PKG-INFO
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14107 2023-05-25 21:38:34.000000 hashkern-0.3.3/README.md
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       38 2023-05-25 21:59:40.606595 hashkern-0.3.3/setup.cfg
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     1231 2023-05-25 21:59:10.000000 hashkern-0.3.3/setup.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.602595 hashkern-0.3.3/src/
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      296 2023-05-25 21:58:21.000000 hashkern-0.3.3/src/hash/__init__.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/cli/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       23 2023-01-14 12:45:56.000000 hashkern-0.3.3/src/hash/cli/__init__.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5912 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/cli/main.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7189 2023-01-13 23:42:17.000000 hashkern-0.3.3/src/hash/dag.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     2148 2023-05-14 21:16:53.000000 hashkern-0.3.3/src/hash/errors.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/kern/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      148 2023-05-25 21:59:19.000000 hashkern-0.3.3/src/hash/kern/__init__.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    10412 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/action.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     7379 2023-05-25 21:58:08.000000 hashkern-0.3.3/src/hash/kern/execute.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      931 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/hash.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3196 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/main.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    16126 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/planner.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     4181 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/secrets.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    19277 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/state.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     5952 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/kern/templates.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)     3461 2023-01-13 23:42:17.000000 hashkern-0.3.3/src/hash/logs.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/resources/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       69 2023-05-14 22:02:35.000000 hashkern-0.3.3/src/hash/resources/__init__.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    97796 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/resources/base.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    22702 2023-05-15 21:31:58.000000 hashkern-0.3.3/src/hash/resources/targets.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hash/store/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       59 2023-01-13 23:42:17.000000 hashkern-0.3.3/src/hash/store/__init__.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    28132 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/store/base.py
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    12523 2023-05-25 21:36:32.000000 hashkern-0.3.3/src/hash/utils.py
+drwxrwxr-x   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        0 2023-05-25 21:59:40.606595 hashkern-0.3.3/src/hashkern.egg-info/
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)    14841 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/PKG-INFO
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      738 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/SOURCES.txt
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        1 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/dependency_links.txt
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)       39 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/entry_points.txt
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)      213 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/requires.txt
+-rw-rw-r--   0 mouhsenibrahim  (1000) mouhsenibrahim  (1000)        5 2023-05-25 21:59:40.000000 hashkern-0.3.3/src/hashkern.egg-info/top_level.txt
```

### Comparing `hashkern-0.3.2/LICENSE` & `hashkern-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/PKG-INFO` & `hashkern-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashkern
-Version: 0.3.2
+Version: 0.3.3
 Summary: A tool for managing resources in a mono repository
 Author: Mouhsen Ibrahim
 Author-email: mouhsen.ibrahim@gmail.com
 Project-URL: Documentation, https://hash-kern.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://gitlab.com/hash-platform/hashkern
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `hashkern-0.3.2/README.md` & `hashkern-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/setup.py` & `hashkern-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
         return f.read().splitlines()
 
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 setup(
     name="hashkern",
-    version="0.3.2",
+    version="0.3.3",
     author="Mouhsen Ibrahim",
     author_email="mouhsen.ibrahim@gmail.com",
     description="A tool for managing resources in a mono repository",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
```

### Comparing `hashkern-0.3.2/src/hash/cli/main.py` & `hashkern-0.3.3/src/hash/cli/main.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/dag.py` & `hashkern-0.3.3/src/hash/dag.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/errors.py` & `hashkern-0.3.3/src/hash/errors.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/kern/action.py` & `hashkern-0.3.3/src/hash/kern/action.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/kern/execute.py` & `hashkern-0.3.3/src/hash/kern/execute.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 from hash import errors
 from hash.kern.templates import Renderer
 from hash.dag import Graph
 from .action import Action
 
 import pluggy
-from pytest import hookimpl
+from hash import execute_hookimpl as hookimpl
 
 hookspec = pluggy.HookspecMarker("hash-executor")
 
 
 class ExecutorSpec:
     @hookspec
     def run(self, ac):
```

### Comparing `hashkern-0.3.2/src/hash/kern/hash.py` & `hashkern-0.3.3/src/hash/kern/hash.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/kern/main.py` & `hashkern-0.3.3/src/hash/kern/main.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/kern/planner.py` & `hashkern-0.3.3/src/hash/kern/planner.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/kern/secrets.py` & `hashkern-0.3.3/src/hash/kern/secrets.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/kern/state.py` & `hashkern-0.3.3/src/hash/kern/state.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/kern/templates.py` & `hashkern-0.3.3/src/hash/kern/templates.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/logs.py` & `hashkern-0.3.3/src/hash/logs.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/resources/base.py` & `hashkern-0.3.3/src/hash/resources/base.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/resources/targets.py` & `hashkern-0.3.3/src/hash/resources/targets.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/store/base.py` & `hashkern-0.3.3/src/hash/store/base.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hash/utils.py` & `hashkern-0.3.3/src/hash/utils.py`

 * *Files identical despite different names*

### Comparing `hashkern-0.3.2/src/hashkern.egg-info/PKG-INFO` & `hashkern-0.3.3/src/hashkern.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hashkern
-Version: 0.3.2
+Version: 0.3.3
 Summary: A tool for managing resources in a mono repository
 Author: Mouhsen Ibrahim
 Author-email: mouhsen.ibrahim@gmail.com
 Project-URL: Documentation, https://hash-kern.readthedocs.io/en/latest/index.html
 Project-URL: Source, https://gitlab.com/hash-platform/hashkern
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `hashkern-0.3.2/src/hashkern.egg-info/SOURCES.txt` & `hashkern-0.3.3/src/hashkern.egg-info/SOURCES.txt`

 * *Files identical despite different names*

