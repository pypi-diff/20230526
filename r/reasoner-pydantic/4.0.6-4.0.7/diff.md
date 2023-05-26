# Comparing `tmp/reasoner-pydantic-4.0.6.tar.gz` & `tmp/reasoner-pydantic-4.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reasoner-pydantic-4.0.6.tar", last modified: Thu May 25 14:35:27 2023, max compression
+gzip compressed data, was "reasoner-pydantic-4.0.7.tar", last modified: Fri May 26 19:32:42 2023, max compression
```

## Comparing `reasoner-pydantic-4.0.6.tar` & `reasoner-pydantic-4.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:27.026882 reasoner-pydantic-4.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-25 14:35:27.026882 reasoner-pydantic-4.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:27.022882 reasoner-pydantic-4.0.6/reasoner_pydantic/
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/auxgraphs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/kgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/metakg.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/qgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/shared.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/reasoner_pydantic/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 14:35:27.026882 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 14:35:27.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-25 14:35:26.000000 reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 14:35:27.026882 reasoner-pydantic-4.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-25 14:35:21.000000 reasoner-pydantic-4.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/reasoner_pydantic/
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/auxgraphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4440 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/kgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7085 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/metakg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/qgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5692 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/shared.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/reasoner_pydantic/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 19:32:42.000000 reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 19:32:42.383168 reasoner-pydantic-4.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-05-26 19:32:39.000000 reasoner-pydantic-4.0.7/setup.py
```

### Comparing `reasoner-pydantic-4.0.6/PKG-INFO` & `reasoner-pydantic-4.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.6
+Version: 4.0.7
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.6/README.md` & `reasoner-pydantic-4.0.7/README.md`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/__init__.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/__init__.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/auxgraphs.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/auxgraphs.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/base_model.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/base_model.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/kgraph.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/kgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/message.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/message.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/metakg.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/metakg.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/qgraph.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/qgraph.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/results.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/results.py`

 * *Files 5% similar despite different names*

```diff
@@ -177,21 +177,22 @@
 
     class Config:
         title = "results"
         extra = "allow"
 
     def add(self, result):
         results = self.__root__
-        for old_result in results:
-            if result == old_result:
-                results.remove(result)
-                old_result.update(result)
-                results.add(old_result)
-                return
-        results.add(result)
+        if result in results:
+            # this is slow for larger results
+            for original_result in results:
+                if result == original_result:
+                    original_result.update(result)
+                    return
+        else:
+            results.add(result)
 
     def __len__(self):
         return len(self.__root__)
 
     def __iter__(self):
         return self.__root__.__iter__()
```

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/shared.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/shared.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/utils.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/utils.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic/workflow.py` & `reasoner-pydantic-4.0.7/reasoner_pydantic/workflow.py`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/PKG-INFO` & `reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reasoner-pydantic
-Version: 4.0.6
+Version: 4.0.7
 Summary: Pydantic models for the Reasoner API data formats
 Home-page: https://github.com/TranslatorSRI/reasoner-pydantic
 Author: Kenneth Morton
 Author-email: kenny@covar.com
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `reasoner-pydantic-4.0.6/reasoner_pydantic.egg-info/SOURCES.txt` & `reasoner-pydantic-4.0.7/reasoner_pydantic.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `reasoner-pydantic-4.0.6/setup.py` & `reasoner-pydantic-4.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="reasoner-pydantic",
-    version="4.0.6",
+    version="4.0.7",
     author="Kenneth Morton",
     author_email="kenny@covar.com",
     url="https://github.com/TranslatorSRI/reasoner-pydantic",
     description="Pydantic models for the Reasoner API data formats",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=["reasoner_pydantic"],
```

