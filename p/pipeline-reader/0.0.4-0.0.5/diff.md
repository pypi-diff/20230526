# Comparing `tmp/pipeline-reader-0.0.4.tar.gz` & `tmp/pipeline-reader-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pipeline-reader-0.0.4.tar", last modified: Tue Feb  8 22:55:06 2022, max compression
+gzip compressed data, was "pipeline-reader-0.0.5.tar", last modified: Fri May 26 17:13:14 2023, max compression
```

## Comparing `pipeline-reader-0.0.4.tar` & `pipeline-reader-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,19 @@
-drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2022-02-08 22:55:06.100479 pipeline-reader-0.0.4/
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     7394 2022-02-08 22:55:06.100479 pipeline-reader-0.0.4/PKG-INFO
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     5249 2021-11-03 19:32:46.000000 pipeline-reader-0.0.4/README.md
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)       38 2022-02-08 22:55:06.100479 pipeline-reader-0.0.4/setup.cfg
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)      946 2021-07-26 22:17:06.000000 pipeline-reader-0.0.4/setup.py
-drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2022-02-08 22:55:06.100479 pipeline-reader-0.0.4/src/
-drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2022-02-08 22:55:06.100479 pipeline-reader-0.0.4/src/pipeline_reader/
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)      456 2021-11-03 16:53:22.000000 pipeline-reader-0.0.4/src/pipeline_reader/__init__.py
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     2802 2021-11-03 19:30:32.000000 pipeline-reader-0.0.4/src/pipeline_reader/objects.py
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)    15307 2022-02-08 22:53:44.000000 pipeline-reader-0.0.4/src/pipeline_reader/reader.py
-drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2022-02-08 22:55:06.100479 pipeline-reader-0.0.4/src/pipeline_reader.egg-info/
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     7394 2022-02-08 22:55:06.000000 pipeline-reader-0.0.4/src/pipeline_reader.egg-info/PKG-INFO
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)      283 2022-02-08 22:55:06.000000 pipeline-reader-0.0.4/src/pipeline_reader.egg-info/SOURCES.txt
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)        1 2022-02-08 22:55:06.000000 pipeline-reader-0.0.4/src/pipeline_reader.egg-info/dependency_links.txt
--rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)       16 2022-02-08 22:55:06.000000 pipeline-reader-0.0.4/src/pipeline_reader.egg-info/top_level.txt
+drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2023-05-26 17:13:14.090572 pipeline-reader-0.0.5/
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     1054 2023-05-26 17:06:57.000000 pipeline-reader-0.0.5/LICENSE
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     7394 2023-05-26 17:13:14.090572 pipeline-reader-0.0.5/PKG-INFO
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     5249 2023-05-26 17:06:57.000000 pipeline-reader-0.0.5/README.md
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)       38 2023-05-26 17:13:14.090572 pipeline-reader-0.0.5/setup.cfg
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     1083 2023-05-26 17:09:06.000000 pipeline-reader-0.0.5/setup.py
+drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2023-05-26 17:13:14.090572 pipeline-reader-0.0.5/src/
+drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2023-05-26 17:13:14.090572 pipeline-reader-0.0.5/src/pipeline_reader/
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)      456 2023-05-26 17:06:57.000000 pipeline-reader-0.0.5/src/pipeline_reader/__init__.py
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     2802 2023-05-26 17:06:57.000000 pipeline-reader-0.0.5/src/pipeline_reader/objects.py
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)    15286 2023-05-26 17:06:57.000000 pipeline-reader-0.0.5/src/pipeline_reader/reader.py
+drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2023-05-26 17:13:14.090572 pipeline-reader-0.0.5/src/pipeline_reader.egg-info/
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)     7394 2023-05-26 17:13:14.000000 pipeline-reader-0.0.5/src/pipeline_reader.egg-info/PKG-INFO
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)      347 2023-05-26 17:13:14.000000 pipeline-reader-0.0.5/src/pipeline_reader.egg-info/SOURCES.txt
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)        1 2023-05-26 17:13:14.000000 pipeline-reader-0.0.5/src/pipeline_reader.egg-info/dependency_links.txt
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)       15 2023-05-26 17:13:14.000000 pipeline-reader-0.0.5/src/pipeline_reader.egg-info/requires.txt
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)       16 2023-05-26 17:13:14.000000 pipeline-reader-0.0.5/src/pipeline_reader.egg-info/top_level.txt
+drwxr-xr-x   0 jcarter2010  (1000) jcarter2010  (1000)        0 2023-05-26 17:13:14.090572 pipeline-reader-0.0.5/tests/
+-rw-r--r--   0 jcarter2010  (1000) jcarter2010  (1000)      182 2023-05-26 17:06:57.000000 pipeline-reader-0.0.5/tests/test.py
```

### Comparing `pipeline-reader-0.0.4/PKG-INFO` & `pipeline-reader-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-reader
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for reading Jenkinsfile-like pipeline files
 Home-page: https://github.com/jfcarter2358/pipeline-reader
 Author: John Carter
 Author-email: jfcarter2358@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jfcarter2358/pipeline-reader/issues
 Description: # Pipeline Reader
```

### Comparing `pipeline-reader-0.0.4/README.md` & `pipeline-reader-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `pipeline-reader-0.0.4/src/pipeline_reader/objects.py` & `pipeline-reader-0.0.5/src/pipeline_reader/objects.py`

 * *Files identical despite different names*

### Comparing `pipeline-reader-0.0.4/src/pipeline_reader/reader.py` & `pipeline-reader-0.0.5/src/pipeline_reader/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -234,16 +234,16 @@
             obj.code += line[obj.indent:] + '\n'
             structure = cartils.helpers.set_from_key_list(structure, key + ["object"], obj)
     return structure['pipeline']['object']
 
 def load(f):
     return loads(f.read())
 
-def run(_pipeline, gs=None, ls=None, log_level='NONE'):
-    _logger = Logger(log_level)
+def run(_pipeline, gs=None, ls=None):
+    _logger = Logger("TRACE")
     if gs is None:
         gs = {}
     if ls is None:
         ls = {}
     _g = {**globals(), **gs}
     _l = {**locals(), **ls}
     _logger.TRACE(_pipeline)
@@ -307,8 +307,8 @@
                 exit(1)
         _stage_index += 1
     _logger.SUCCESS('Pipeline finished successfully')
 
 if __name__ == '__main__':
     with open('tests/test.pipeline') as f:
         p = load(f)
-    run(p)
+    run(p)
```

### Comparing `pipeline-reader-0.0.4/src/pipeline_reader.egg-info/PKG-INFO` & `pipeline-reader-0.0.5/src/pipeline_reader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pipeline-reader
-Version: 0.0.4
+Version: 0.0.5
 Summary: A package for reading Jenkinsfile-like pipeline files
 Home-page: https://github.com/jfcarter2358/pipeline-reader
 Author: John Carter
 Author-email: jfcarter2358@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/jfcarter2358/pipeline-reader/issues
 Description: # Pipeline Reader
```

