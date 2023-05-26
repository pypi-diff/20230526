# Comparing `tmp/hcai-nova-server-nightly-0.1.7.dev202305251001.tar.gz` & `tmp/hcai-nova-server-nightly-0.1.7.dev202305261329.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hcai-nova-server-nightly-0.1.7.dev202305251001.tar", last modified: Thu May 25 10:01:32 2023, max compression
+gzip compressed data, was "hcai-nova-server-nightly-0.1.7.dev202305261329.tar", last modified: Fri May 26 13:29:02 2023, max compression
```

## Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001.tar` & `hcai-nova-server-nightly-0.1.7.dev202305261329.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:32.353884 hcai-nova-server-nightly-0.1.7.dev202305251001/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 10:01:32.353884 hcai-nova-server-nightly-0.1.7.dev202305251001/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:32.349884 hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-25 10:01:32.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-25 10:01:32.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 10:01:32.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-25 10:01:32.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-25 10:01:32.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-25 10:01:32.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:32.349884 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/app.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:32.349884 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/cancel.py
--rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/explain.py
--rw-r--r--   0 runner    (1001) docker     (122)     9863 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/extract.py
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/log.py
--rw-r--r--   0 runner    (1001) docker     (122)     7040 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/predict.py
--rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/status.py
--rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/train.py
--rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:32.349884 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/templates/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:32.353884 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/dataset_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    12139 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/explain_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/import_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/key_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/status_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/thread_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 10:01:32.353884 hcai-nova-server-nightly-0.1.7.dev202305251001/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-05-25 10:01:21.000000 hcai-nova-server-nightly-0.1.7.dev202305251001/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 13:29:02.760899 hcai-nova-server-nightly-0.1.7.dev202305261329/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-26 13:29:02.760899 hcai-nova-server-nightly-0.1.7.dev202305261329/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      374 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 13:29:02.756899 hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     1369 2023-05-26 13:29:02.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      955 2023-05-26 13:29:02.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 13:29:02.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-26 13:29:02.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-05-26 13:29:02.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       12 2023-05-26 13:29:02.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 13:29:02.756899 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2597 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/app.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 13:29:02.760899 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1051 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13652 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/explain.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9863 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/extract.py
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/log.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7185 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/predict.py
+-rw-r--r--   0 runner    (1001) docker     (122)      756 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/status.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6075 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/train.py
+-rw-r--r--   0 runner    (1001) docker     (122)      351 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 13:29:02.760899 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 13:29:02.760899 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2254 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/dataset_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13768 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1785 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/explain_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1233 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/import_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      983 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/key_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1375 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2159 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/status_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/thread_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)      103 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 13:29:02.760899 hcai-nova-server-nightly-0.1.7.dev202305261329/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2562 2023-05-26 13:28:53.000000 hcai-nova-server-nightly-0.1.7.dev202305261329/setup.py
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/PKG-INFO` & `hcai-nova-server-nightly-0.1.7.dev202305261329/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.7.dev202305251001
+Version: 0.1.7.dev202305261329
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/PKG-INFO` & `hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hcai-nova-server-nightly
-Version: 0.1.7.dev202305251001
+Version: 0.1.7.dev202305261329
 Summary: !Alpha Version! - This repository contains code to setup a computational backend server for the nova annotation tool. You can use this backend to train models of your choosing or create explanations for existing models.
 Home-page: https://github.com/pypa/sampleproject
 Author: Dominik Schiller
 Author-email: dominik.schiller@uni-a.de
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/hcai_nova_server_nightly.egg-info/SOURCES.txt` & `hcai-nova-server-nightly-0.1.7.dev202305261329/hcai_nova_server_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/app.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/app.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/cancel.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/cancel.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/explain.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/explain.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/extract.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/extract.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/log.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/log.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/predict.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/predict.py`

 * *Files 7% similar despite different names*

```diff
@@ -130,17 +130,22 @@
         annos = predictor.to_anno(data)
         logger.info("...done")
 
         logger.info("Saving predictions to database...")
 
         # TODO: Refactor to not use request form in upload
         request_form_copy = copy.copy(request_form)
+        request_form_copy['scheme'] = 'activelistening'
+
         assert len(ss_ds_iter.sessions) == 1
         request_form_copy['sessions'] = ss_ds_iter.sessions[0]
-        db_utils.write_annotation_to_db(request_form_copy, annos, logger)
+        request_form_copy['roles'] = ss_ds_iter.roles[0]
+
+        for anno in annos:
+            db_utils.write_annotation_to_db(request_form_copy, anno, logger)
         logger.info("...done")
 
     logger.info("Prediction completed!")
     status_utils.update_status(key, status_utils.JobStatus.FINISHED)
 
     # model_script.ds_iter = ds_iter
     # model_script.request_form["sessions"] = session
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/status.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/status.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/route/train.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/route/train.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/dataset_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/dataset_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/db_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/db_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import sys
 import bson
 import copy
 import warnings
 import numpy as np
 
 from hcai_datasets.hcai_nova_dynamic.nova_db_handler import NovaDBHandler
-from hcai_datasets.hcai_nova_dynamic.utils import nova_data_utils
-
+from nova_utils.ssi_utils.ssi_anno_utils import Anno, SchemeType
 MAX_MONGO_DB_DOC_SIZE = 16777216
 database = None
 scheme = None
 session = None
 annotator = None
 roles = None
 
@@ -60,49 +59,116 @@
         is_valid=is_valid,
         sr=sr,
         dimlabels=dimlables,
         overwrite=True,
     )
 
 
-def write_annotation_to_db(request_form, results: dict, logger):
-    global database, scheme, session, annotator, roles
-    check_format(results, logger)
+def write_annotation_to_db(request_form, anno: Anno, logger):
+    #global database, scheme, session, annotator, roles
+    #check_format(results, logger)
 
     # TODO check if we really need to establish a new connection to the database
+    # DB Config
     db_config_dict = {
         "ip": request_form["server"].split(":")[0],
         "port": int(request_form["server"].split(":")[1]),
         "user": request_form["username"],
         "password": request_form["password"],
     }
 
+    # Database specific options
     db_handler = NovaDBHandler(db_config_dict=db_config_dict)
     database = request_form["database"]
-    scheme = request_form["scheme"]
     session = request_form["sessions"]
-    annotator = request_form["annotator"]
-    roles = request_form["roles"]
 
-    if request_form["schemeType"] == "DISCRETE":
-        write_discrete_to_db(request_form, results, db_handler, logger)
-    elif request_form["schemeType"] == "FREE":
-        write_freeform_to_db(request_form, results, db_handler, logger)
-    elif request_form["schemeType"] == "CONTINUOUS":
-        write_continuous_to_db(request_form, results, db_handler, logger)
-    elif request_form["schemeType"] == "POINT":
-        pass  # todo
-    elif (
-        request_form["schemeType"] == "DISCRETE_POLYGON"
-        or request_form["schemeType"] == "POLYGON"
-    ):
-        write_polygons_to_db(request_form, results, db_handler, logger)
+    # Format data correctly
+    scheme_dtype_names = anno.scheme.get_dtype()['names']
+    anno_data = [
+        dict(zip(scheme_dtype_names, ad))
+        for ad
+        in anno.data
+    ]
+
+
+    db_handler.set_annos(
+        database=database,
+        session=session,
+        scheme=anno.scheme.name,
+        annotator=anno.annotator,
+        role=anno.role,
+        annos=anno_data,
+    )
+
+    # if request_form["schemeType"] == "DISCRETE":
+    #     write_discrete_to_db(request_form, anno, db_handler, logger)
+    # elif request_form["schemeType"] == "FREE":
+    #     write_freeform_to_db(request_form, anno, db_handler, logger)
+    # elif request_form["schemeType"] == "CONTINUOUS":
+    #     write_continuous_to_db(request_form, anno, db_handler, logger)
+    # else:
+    #     raise NotImplementedError()
+    # elif request_form["schemeType"] == "POINT":
+    #     pass  # todo
+    # elif (
+    #     request_form["schemeType"] == "DISCRETE_POLYGON"
+    #     or request_form["schemeType"] == "POLYGON"
+    # ):
+    #     write_polygons_to_db(request_form, anno, db_handler, logger)
 
 
-def write_freeform_to_db(request_form, results: dict, db_handler, logger):
+def write_freeform_to_db(request_form, anno: Anno, db_handler, logger):
+    """
+    Args:
+        request_form ():
+        results (dict): {
+            'from_to' : {
+                <role>.<stream>: {
+                    'name': <text>, 'conf': <confidence>
+                }
+            }
+        }
+        db_handler ():
+        logger ():
+
+    """
+
+    annotations = {}
+
+
+    for frame, results in results.items():
+        frame_info = frame.split("_")
+        frame_from = float(frame_info[-2])
+        frame_to = float(frame_info[-1])
+        for stream_id, anno in results.items():
+
+            conf = anno["conf"]
+            name = anno["name"]
+
+            if stream_id not in annotations.keys():
+                annotations[stream_id] = []
+
+            annotations[stream_id].append(
+                {"from": frame_from, "to": frame_to, "conf": conf, "name": name}
+            )
+
+    for anno_id, anno in annotations.items():
+        # TODO does not work with flattened roles
+        role, stream = anno_id.split(".")
+
+        db_handler.set_annos(
+            database=database,
+            scheme=scheme,
+            session=session,
+            annotator=annotator,
+            role=role,
+            annos=anno,
+        )
+
+def write_discrete_to_db(request_form, results: dict, db_handler, logger):
     """
     Args:
         request_form ():
         results (dict): {
             'from_to' : {
                 <role>.<stream>: {
                     'name': <text>, 'conf': <confidence>
@@ -123,21 +189,21 @@
     for frame, results in results.items():
         frame_info = frame.split("_")
         frame_from = float(frame_info[-2])
         frame_to = float(frame_info[-1])
         for stream_id, anno in results.items():
 
             conf = anno["conf"]
-            name = anno["name"]
+            id = anno["id"]
 
             if stream_id not in annotations.keys():
                 annotations[stream_id] = []
 
             annotations[stream_id].append(
-                {"from": frame_from, "to": frame_to, "conf": conf, "name": name}
+                {"from": frame_from, "to": frame_to, "conf": conf, "id": id}
             )
 
     for anno_id, anno in annotations.items():
         # TODO does not work with flattened roles
         role, stream = anno_id.split(".")
 
         db_handler.set_annos(
@@ -146,14 +212,15 @@
             session=session,
             annotator=annotator,
             role=role,
             annos=anno,
         )
 
 
+'''
 def write_discrete_to_db(request_form, results: dict, db_handler, logger):
     # TODO: We only take one role into account in this case. Fix
     # role = roles.split(';')[0]
     role = results["roles"]
     frame_size = nova_data_utils.parse_time_string_to_ms(request_form["frameSize"])
     mongo_scheme = db_handler.get_mongo_scheme(scheme, database)
     annos = []
@@ -199,15 +266,15 @@
         database=database,
         scheme=scheme,
         session=session,
         annotator=annotator,
         role=role,
         annos=annos,
     )
-
+    '''
 
 def write_continuous_to_db(request_form, results: dict, db_handler, logger):
     role = results["roles"]
     # role = roles.split(';')[0]
     annos = []
 
     if request_form["startTime"] != "0":
```

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/explain_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/explain_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/import_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/import_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/key_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/key_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/log_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/log_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/status_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/status_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/nova_server/utils/thread_utils.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/nova_server/utils/thread_utils.py`

 * *Files identical despite different names*

### Comparing `hcai-nova-server-nightly-0.1.7.dev202305251001/setup.py` & `hcai-nova-server-nightly-0.1.7.dev202305261329/setup.py`

 * *Files identical despite different names*

