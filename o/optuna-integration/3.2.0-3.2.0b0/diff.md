# Comparing `tmp/optuna-integration-3.2.0.tar.gz` & `tmp/optuna-integration-3.2.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optuna-integration-3.2.0.tar", last modified: Fri May 26 07:45:54 2023, max compression
+gzip compressed data, was "optuna-integration-3.2.0b0.tar", last modified: Thu May 25 06:17:48 2023, max compression
```

## Comparing `optuna-integration-3.2.0.tar` & `optuna-integration-3.2.0b0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:45:54.445023 optuna-integration-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-26 07:45:54.445023 optuna-integration-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:45:54.445023 optuna-integration-3.2.0/optuna_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:45:54.445023 optuna-integration-3.2.0/optuna_integration/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/allennlp/_dump_best_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/allennlp/_environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/allennlp/_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/allennlp/_pruner.py
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/allennlp/_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/chainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/chainermn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/skorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/tfkeras.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/optuna_integration/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:45:54.445023 optuna-integration-3.2.0/optuna_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6090 2023-05-26 07:45:54.000000 optuna-integration-3.2.0/optuna_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-26 07:45:54.000000 optuna-integration-3.2.0/optuna_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 07:45:54.000000 optuna-integration-3.2.0/optuna_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-26 07:45:54.000000 optuna-integration-3.2.0/optuna_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-26 07:45:54.000000 optuna-integration-3.2.0/optuna_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-26 07:45:54.449023 optuna-integration-3.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 07:45:54.445023 optuna-integration-3.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/tests/test_catalyst.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/tests/test_chainer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/tests/test_chainermn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/tests/test_keras.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/tests/test_skorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/tests/test_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-26 07:45:37.000000 optuna-integration-3.2.0/tests/test_tfkeras.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.175664 optuna-integration-3.2.0b0/optuna_integration/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4081 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/optuna_integration/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_dump_best_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_pruner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/allennlp/_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4291 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11194 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/chainermn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/skorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/tfkeras.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/optuna_integration/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/optuna_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-25 06:17:48.000000 optuna-integration-3.2.0b0/optuna_integration.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 06:17:48.179664 optuna-integration-3.2.0b0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_catalyst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_chainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16494 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_chainermn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_keras.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_skorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-25 06:17:24.000000 optuna-integration-3.2.0b0/tests/test_tfkeras.py
```

### Comparing `optuna-integration-3.2.0/LICENSE` & `optuna-integration-3.2.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/PKG-INFO` & `optuna-integration-3.2.0b0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-integration
-Version: 3.2.0
+Version: 3.2.0b0
 Summary: Integration libraries of Optuna.
 License: MIT License
         
         Copyright (c) 2018 Preferred Networks, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `optuna-integration-3.2.0/README.md` & `optuna-integration-3.2.0b0/README.md`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/_imports.py` & `optuna-integration-3.2.0b0/optuna_integration/_imports.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/allennlp/_dump_best_config.py` & `optuna-integration-3.2.0b0/optuna_integration/allennlp/_dump_best_config.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/allennlp/_executor.py` & `optuna-integration-3.2.0b0/optuna_integration/allennlp/_executor.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/allennlp/_pruner.py` & `optuna-integration-3.2.0b0/optuna_integration/allennlp/_pruner.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/allennlp/_variables.py` & `optuna-integration-3.2.0b0/optuna_integration/allennlp/_variables.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/catalyst.py` & `optuna-integration-3.2.0b0/optuna_integration/catalyst.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/chainer.py` & `optuna-integration-3.2.0b0/optuna_integration/chainer.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/chainermn.py` & `optuna-integration-3.2.0b0/optuna_integration/chainermn.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/keras.py` & `optuna-integration-3.2.0b0/optuna_integration/keras.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/skorch.py` & `optuna-integration-3.2.0b0/optuna_integration/skorch.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/tensorflow.py` & `optuna-integration-3.2.0b0/optuna_integration/tensorflow.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration/tfkeras.py` & `optuna-integration-3.2.0b0/optuna_integration/tfkeras.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/optuna_integration.egg-info/PKG-INFO` & `optuna-integration-3.2.0b0/optuna_integration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: optuna-integration
-Version: 3.2.0
+Version: 3.2.0b0
 Summary: Integration libraries of Optuna.
 License: MIT License
         
         Copyright (c) 2018 Preferred Networks, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `optuna-integration-3.2.0/optuna_integration.egg-info/SOURCES.txt` & `optuna-integration-3.2.0b0/optuna_integration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/pyproject.toml` & `optuna-integration-3.2.0b0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/tests/test_chainer.py` & `optuna-integration-3.2.0b0/tests/test_chainer.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/tests/test_chainermn.py` & `optuna-integration-3.2.0b0/tests/test_chainermn.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/tests/test_keras.py` & `optuna-integration-3.2.0b0/tests/test_keras.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/tests/test_skorch.py` & `optuna-integration-3.2.0b0/tests/test_skorch.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/tests/test_tensorflow.py` & `optuna-integration-3.2.0b0/tests/test_tensorflow.py`

 * *Files identical despite different names*

### Comparing `optuna-integration-3.2.0/tests/test_tfkeras.py` & `optuna-integration-3.2.0b0/tests/test_tfkeras.py`

 * *Files identical despite different names*

