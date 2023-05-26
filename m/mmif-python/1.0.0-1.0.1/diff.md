# Comparing `tmp/mmif-python-1.0.0.tar.gz` & `tmp/mmif-python-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmif-python-1.0.0.tar", last modified: Fri May 26 01:14:33 2023, max compression
+gzip compressed data, was "mmif-python-1.0.1.tar", last modified: Fri May 26 13:34:57 2023, max compression
```

## Comparing `mmif-python-1.0.0.tar` & `mmif-python-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.534109 mmif-python-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-26 01:13:53.000000 mmif-python-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 01:13:53.000000 mmif-python-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 01:14:33.534109 mmif-python-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 01:13:53.000000 mmif-python-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 01:13:53.000000 mmif-python-1.0.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.530109 mmif-python-1.0.0/mmif/
--rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.530109 mmif-python-1.0.0/mmif/res/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:32.000000 mmif-python-1.0.0/mmif/res/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/res/clams.vocabulary.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 01:14:32.000000 mmif-python-1.0.0/mmif/res/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/res/mmif.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.530109 mmif-python-1.0.0/mmif/serialize/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/mmif.py
--rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-26 01:13:53.000000 mmif-python-1.0.0/mmif/serialize/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.530109 mmif-python-1.0.0/mmif/ver/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 01:14:32.000000 mmif-python-1.0.0/mmif/ver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 01:14:32.000000 mmif-python-1.0.0/mmif/ver/do-not-edit.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.534109 mmif-python-1.0.0/mmif/vocabulary/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/annotation_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/base_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/do-not-edit.txt
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif/vocabulary/document_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:14:33.534109 mmif-python-1.0.0/mmif_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 01:14:33.000000 mmif-python-1.0.0/mmif_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 01:13:53.000000 mmif-python-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:14:33.534109 mmif-python-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-05-26 01:13:53.000000 mmif-python-1.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.949401 mmif-python-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-05-26 13:34:05.000000 mmif-python-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-26 13:34:05.000000 mmif-python-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 13:34:57.949401 mmif-python-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-26 13:34:05.000000 mmif-python-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-26 13:34:05.000000 mmif-python-1.0.1/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.945401 mmif-python-1.0.1/mmif/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.945401 mmif-python-1.0.1/mmif/res/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/res/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8317 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/res/clams.vocabulary.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/res/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/res/mmif.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.945401 mmif-python-1.0.1/mmif/serialize/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14150 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20102 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/mmif.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18712 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16164 2023-05-26 13:34:05.000000 mmif-python-1.0.1/mmif/serialize/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.945401 mmif-python-1.0.1/mmif/ver/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/ver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/ver/do-not-edit.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.949401 mmif-python-1.0.1/mmif/vocabulary/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/annotation_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7075 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/base_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/do-not-edit.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif/vocabulary/document_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 13:34:57.949401 mmif-python-1.0.1/mmif_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 13:34:57.000000 mmif-python-1.0.1/mmif_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 13:34:05.000000 mmif-python-1.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 13:34:57.949401 mmif-python-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)    12446 2023-05-26 13:34:05.000000 mmif-python-1.0.1/setup.py
```

### Comparing `mmif-python-1.0.0/LICENSE` & `mmif-python-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.0/PKG-INFO` & `mmif-python-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.0/mmif/res/clams.vocabulary.yaml` & `mmif-python-1.0.1/mmif/res/clams.vocabulary.yaml`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.0/mmif/res/mmif.json` & `mmif-python-1.0.1/mmif/res/mmif.json`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.0/mmif/serialize/annotation.py` & `mmif-python-1.0.1/mmif/serialize/annotation.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.0/mmif/serialize/mmif.py` & `mmif-python-1.0.1/mmif/serialize/mmif.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.0/mmif/serialize/model.py` & `mmif-python-1.0.1/mmif/serialize/model.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.0/mmif/serialize/view.py` & `mmif-python-1.0.1/mmif/serialize/view.py`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.0/mmif/vocabulary/annotation_types.py` & `mmif-python-1.0.1/mmif/vocabulary/annotation_types.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Spec version 0.5.0
+# Spec version 1.0.0
 # This file is auto-generated by setup.py
 
 from .base_types import AnnotationTypesBase
 
 
 class AnnotationTypes(AnnotationTypesBase):
     """
     This class contains the CLAMS annotation types 
-    defined in the spec version 0.5.0 as class variables. 
+    defined in the spec version 1.0.0 as class variables. 
     """
     Annotation = AnnotationTypesBase('http://mmif.clams.ai/vocabulary/Annotation/v2')
     Region = AnnotationTypesBase('http://mmif.clams.ai/vocabulary/Region/v1')
     TimePoint = AnnotationTypesBase('http://mmif.clams.ai/vocabulary/TimePoint/v1')
     Interval = AnnotationTypesBase('http://mmif.clams.ai/vocabulary/Interval/v1')
     Span = AnnotationTypesBase('http://mmif.clams.ai/vocabulary/Span/v1')
     TimeFrame = AnnotationTypesBase('http://mmif.clams.ai/vocabulary/TimeFrame/v1')
```

### Comparing `mmif-python-1.0.0/mmif/vocabulary/base_types.py` & `mmif-python-1.0.1/mmif/vocabulary/base_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,11 +192,11 @@
     """
     ...
 
 
 class ThingType(ThingTypesBase):
     """
     This class contains the topmost CLAMS thing type 
-    defined in the spec version 0.5.0 as a class variable. 
+    defined in the spec version 1.0.0 as a class variable. 
     """
     Thing = ClamsTypesBase('http://mmif.clams.ai/vocabulary/Thing/v1')
     typevers = {'Thing': 'v1'}
```

### Comparing `mmif-python-1.0.0/mmif/vocabulary/document_types.py` & `mmif-python-1.0.1/mmif/vocabulary/document_types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# Spec version 0.5.0
+# Spec version 1.0.0
 # This file is auto-generated by setup.py
 
 from .base_types import DocumentTypesBase
 
 
 class DocumentTypes(DocumentTypesBase):
     """
     This class contains the CLAMS document types 
-    defined in the spec version 0.5.0 as class variables. 
+    defined in the spec version 1.0.0 as class variables. 
     """
     Document = DocumentTypesBase('http://mmif.clams.ai/vocabulary/Document/v1')
     VideoDocument = DocumentTypesBase('http://mmif.clams.ai/vocabulary/VideoDocument/v1')
     AudioDocument = DocumentTypesBase('http://mmif.clams.ai/vocabulary/AudioDocument/v1')
     ImageDocument = DocumentTypesBase('http://mmif.clams.ai/vocabulary/ImageDocument/v1')
     TextDocument = DocumentTypesBase('http://mmif.clams.ai/vocabulary/TextDocument/v1')
     typevers = {'Document': 'v1', 'VideoDocument': 'v1', 'AudioDocument': 'v1', 'ImageDocument': 'v1', 'TextDocument': 'v1'}
```

### Comparing `mmif-python-1.0.0/mmif_python.egg-info/PKG-INFO` & `mmif-python-1.0.1/mmif_python.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmif-python
-Version: 1.0.0
+Version: 1.0.1
 Summary: Python implementation of MultiMedia Interchange Format specification. (https://mmif.clams.ai)
 Home-page: https://mmif.clams.ai
 Author: Brandeis Lab for Linguistics and Computation
 Author-email: admin@clams.ai
 License: UNKNOWN
 Description: ## MultiMedia Interchange Format
         [MMIF](https://mmif.clams.ai) is a JSON(-LD)-based data format designed for transferring annotation data between computational analysis applications in [CLAMS project](https://clams.ai).
```

### Comparing `mmif-python-1.0.0/mmif_python.egg-info/SOURCES.txt` & `mmif-python-1.0.1/mmif_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mmif-python-1.0.0/setup.py` & `mmif-python-1.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,19 +158,25 @@
         enum_contents = generate_vocab_enum(spec_version, type_ver_list, mod_name)
         write_res_file(vocabulary_dir, mod_name+'.py', enum_contents)
 
     return vocabulary_dir
 
 
 def get_latest_mmif_gittag():
-    # vmaj, vmin, vpat = version.split('.')[0:3]
-    res = request.urlopen('https://api.github.com/repos/clamsproject/mmif/git/refs/tags')
-    body = json.loads(res.read())
-    tags = [os.path.basename(tag['ref']) for tag in body]
+    cur_p = 1
+    body = [None]
+    tags = []
+    while len(body) > 0:
+        # for when we have more than 30 (default pagination size) tags
+        res = request.urlopen(f'https://api.github.com/repos/clamsproject/mmif/tags?per_page=100&page={cur_p}')
+        body = json.loads(res.read())
+        tags.extend([tag['name'] for tag in body])
+        cur_p += 1
     # sort and return highest version
+    print(tags)
     mmif_ver_format = lambda x: re.match(r'\d+\.\d+\.\d$', x)
     return sorted([tag for tag in tags if mmif_ver_format(tag)])[-1]
 
 
 def get_spec_file_at_gitref(tag, filepath: str) -> bytes:
     filepath = filepath.format(version=tag)
     if LOCALMMIF is not None:
```

