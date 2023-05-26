# Comparing `tmp/autogluon.features-0.7.1b20230525.tar.gz` & `tmp/autogluon.features-0.7.1b20230526.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.features-0.7.1b20230525.tar", last modified: Thu May 25 09:04:07 2023, max compression
+gzip compressed data, was "autogluon.features-0.7.1b20230526.tar", last modified: Fri May 26 09:03:57 2023, max compression
```

## Comparing `autogluon.features-0.7.1b20230525.tar` & `autogluon.features-0.7.1b20230526.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:07.037207 autogluon.features-0.7.1b20230525/
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-05-25 09:04:07.037207 autogluon.features-0.7.1b20230525/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 09:04:07.037207 autogluon.features-0.7.1b20230525/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:07.029207 autogluon.features-0.7.1b20230525/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:07.029207 autogluon.features-0.7.1b20230525/src/autogluon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:07.033207 autogluon.features-0.7.1b20230525/src/autogluon/features/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/binning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:07.037207 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    44073 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/abstract.py
--rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/astype.py
--rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/auto_ml_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/binned.py
--rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/bulk.py
--rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/category.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/drop_duplicates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/drop_unique.py
--rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/fillna.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/isnan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/label_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/memory_minimize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/one_hot_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     8876 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/rename.py
--rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/text_ngram.py
--rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/generators/text_special.py
--rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-25 09:03:38.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/vectorizers.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-25 09:04:06.000000 autogluon.features-0.7.1b20230525/src/autogluon/features/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 09:04:07.033207 autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-05-25 09:04:06.000000 autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-25 09:04:07.000000 autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:04:06.000000 autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:04:06.000000 autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-25 09:04:06.000000 autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-25 09:04:06.000000 autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 09:04:06.000000 autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:57.927641 autogluon.features-0.7.1b20230526/
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-05-26 09:03:57.927641 autogluon.features-0.7.1b20230526/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 09:03:57.927641 autogluon.features-0.7.1b20230526/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:57.923642 autogluon.features-0.7.1b20230526/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:57.923642 autogluon.features-0.7.1b20230526/src/autogluon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:57.923642 autogluon.features-0.7.1b20230526/src/autogluon/features/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/binning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:57.927641 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44073 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13301 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/astype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8056 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/auto_ml_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2367 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/binned.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13727 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/bulk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9713 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7312 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/drop_duplicates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/drop_unique.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1407 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3055 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/fillna.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/isnan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/label_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/memory_minimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/one_hot_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/rename.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15724 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/text_ngram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7411 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/generators/text_special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2085 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-05-26 09:03:32.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/vectorizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-26 09:03:57.000000 autogluon.features-0.7.1b20230526/src/autogluon/features/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:03:57.923642 autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12549 2023-05-26 09:03:57.000000 autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1497 2023-05-26 09:03:57.000000 autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:03:57.000000 autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:03:57.000000 autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-26 09:03:57.000000 autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 09:03:57.000000 autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:03:57.000000 autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/zip-safe
```

### Comparing `autogluon.features-0.7.1b20230525/PKG-INFO` & `autogluon.features-0.7.1b20230526/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.features
-Version: 0.7.1b20230525
+Version: 0.7.1b20230526
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.features-0.7.1b20230525/setup.py` & `autogluon.features-0.7.1b20230526/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/binning.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/binning.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/__init__.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/abstract.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/abstract.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/astype.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/astype.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/auto_ml_pipeline.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/auto_ml_pipeline.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/binned.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/binned.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/bulk.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/bulk.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/category.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/category.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/datetime.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/datetime.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/drop_duplicates.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/drop_duplicates.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from typing import Union
 from collections import defaultdict
 
+import numpy as np
 from pandas import DataFrame
 
 from autogluon.common.features.types import R_INT, R_FLOAT, R_CATEGORY, R_BOOL
 
 from .abstract import AbstractFeatureGenerator
 
 logger = logging.getLogger(__name__)
@@ -14,28 +15,28 @@
 # TODO: Not necessary to exist after fitting, can just update outer context feature_out/feature_in and then delete this
 class DropDuplicatesFeatureGenerator(AbstractFeatureGenerator):
     """
     Drops features which are exact duplicates of other features, leaving only one instance of the data.
 
     Parameters
     ----------
-    sample_size_init : int, default 1000
+    sample_size_init : int, default 500
         The number of rows to sample when doing an initial filter of duplicate feature candidates.
         Usually, the majority of features can be filtered out using this smaller amount of rows which greatly speeds up the computation of the final check.
         If None or greater than the number of rows, no initial filter will occur. This may increase the time to fit immensely for large datasets.
-    sample_size_final : int, default 20000
+    sample_size_final : int, default 2000
         The number of rows to sample when doing the final filter to determine duplicate features.
         This theoretically can lead to features that are very nearly duplicates but not exact duplicates being removed,
         but should be near impossible in practice.
         If None or greater than the number of rows, will perform exact duplicate detection (most expensive).
-        It is recommend to keep this value below 100000 to maintain reasonable fit times.
+        It is recommended to keep this value below 100000 to maintain reasonable fit times.
     **kwargs :
         Refer to :class:`AbstractFeatureGenerator` documentation for details on valid key word arguments.
     """
-    def __init__(self, sample_size_init=1000, sample_size_final=20000, **kwargs):
+    def __init__(self, sample_size_init=500, sample_size_final=2000, **kwargs):
         super().__init__(**kwargs)
         self.sample_size_init = sample_size_init
         self.sample_size_final = sample_size_final
 
     def _fit_transform(self, X: DataFrame, **kwargs) -> (DataFrame, dict):
         if self.sample_size_init is not None and len(X) > self.sample_size_init:
             features_to_check = self._drop_duplicate_features(X, self.feature_metadata_in, keep=False, sample_size=self.sample_size_init)
@@ -124,14 +125,16 @@
             # Only need to check features that have same amount of unique values.
             features_to_check = features_unique_count_dict[feature_unique_count]
             if len(features_to_check) <= 1:
                 continue
             mapping_features_val_dict_cur = {feature: mapping_features_val_dict[feature] for feature in features_to_check}
             # Converts ['a', 'd', 'f', 'a'] to [0, 1, 2, 0]
             # Converts [5, 'a', np.nan, 5] to [0, 1, 2, 0], these would be considered duplicates since they carry the same information.
-            X_cur = X[features_to_check].replace(mapping_features_val_dict_cur)
+
+            # Have to convert to object dtype because category dtype for unknown reasons will refuse to replace NaNs.
+            X_cur = X[features_to_check].astype('object').replace(mapping_features_val_dict_cur).astype(np.int64)
             features_to_remove += cls._drop_duplicate_features_numeric(X=X_cur, keep=keep)
 
         return features_to_remove
 
     def _more_tags(self):
         return {'feature_interactions': False}
```

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/drop_unique.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/drop_unique.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/dummy.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/dummy.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/fillna.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/fillna.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/identity.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/identity.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/isnan.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/isnan.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/label_encoder.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/label_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/memory_minimize.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/memory_minimize.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/one_hot_encoder.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/one_hot_encoder.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/pipeline.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/pipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,21 +21,22 @@
     """
     PipelineFeatureGenerator is an implementation of BulkFeatureGenerator with various smart defaults and edge case handling functionality to enable
     robust data handling.
     It is recommended that users base any custom feature generators meant for end-to-end data transformation from PipelineFeatureGenerator.
         Reference AutoMLPipelineFeatureGenerator for an example of extending PipelineFeatureGenerator.
     It is not recommended that PipelineFeatureGenerator be used as a generator within any other generator's pre or post generators.
     """
-    def __init__(self, pre_generators=None, post_generators=None, pre_drop_useless=True, pre_enforce_types=True, reset_index=True, verbosity=3, **kwargs):
+    def __init__(self, pre_generators=None, post_generators=None, pre_drop_useless=True, pre_enforce_types=True, reset_index=True, post_drop_duplicates=True, verbosity=3, **kwargs):
         if pre_generators is None:
             pre_generators = [FillNaFeatureGenerator(inplace=True)]
         if post_generators is None:
             post_generators = [DropUniqueFeatureGenerator()]
 
-        super().__init__(pre_generators=pre_generators, post_generators=post_generators, pre_drop_useless=pre_drop_useless, pre_enforce_types=pre_enforce_types,
+        super().__init__(pre_generators=pre_generators, post_generators=post_generators,
+                         post_drop_duplicates=post_drop_duplicates, pre_drop_useless=pre_drop_useless, pre_enforce_types=pre_enforce_types,
                          reset_index=reset_index, verbosity=verbosity, **kwargs)
 
         # FeatureMetadata object based on the original input features real dtypes
         # (will contain dtypes such as 'int16' and 'float32' instead of 'int' and 'float').
         self._feature_metadata_in_real: FeatureMetadata = None
 
         self._is_dummy = False  # If True, returns a single dummy feature as output. Occurs if fit with no useful features.
```

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/rename.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/rename.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/text_ngram.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/text_ngram.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/generators/text_special.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/generators/text_special.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/utils.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/utils.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon/features/vectorizers.py` & `autogluon.features-0.7.1b20230526/src/autogluon/features/vectorizers.py`

 * *Files identical despite different names*

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/PKG-INFO` & `autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.features
-Version: 0.7.1b20230525
+Version: 0.7.1b20230526
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.features-0.7.1b20230525/src/autogluon.features.egg-info/SOURCES.txt` & `autogluon.features-0.7.1b20230526/src/autogluon.features.egg-info/SOURCES.txt`

 * *Files identical despite different names*

