# Comparing `tmp/torch_utilities-1.0.4.tar.gz` & `tmp/torch_utilities-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_utilities-1.0.4.tar", last modified: Tue May  9 23:05:44 2023, max compression
+gzip compressed data, was "torch_utilities-1.0.5.tar", last modified: Fri May 26 13:02:45 2023, max compression
```

## Comparing `torch_utilities-1.0.4.tar` & `torch_utilities-1.0.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-09 23:05:44.705839 torch_utilities-1.0.4/
--rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/LICENSE
--rw-rw-r--   0 deema     (1000) deema     (1000)     5072 2023-05-09 23:05:44.705839 torch_utilities-1.0.4/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     4735 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/README.md
--rw-rw-r--   0 deema     (1000) deema     (1000)       80 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/pyproject.toml
--rw-rw-r--   0 deema     (1000) deema     (1000)      837 2023-05-09 23:05:44.709839 torch_utilities-1.0.4/setup.cfg
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-09 23:05:44.701839 torch_utilities-1.0.4/tests/
--rw-rw-r--   0 deema     (1000) deema     (1000)      196 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3514 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/generate_test_data.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    11107 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     2179 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6096 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     5870 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     2045 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_features.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     1228 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     9425 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_model_trainer.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    37668 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3980 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/tests/test_pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-09 23:05:44.705839 torch_utilities-1.0.4/torch_utilities/
--rw-rw-r--   0 deema     (1000) deema     (1000)      410 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/__init__.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    17154 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/audio.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     6376 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/augmentation.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     9044 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/common.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    13587 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/data_loading.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     4079 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/features.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     7047 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/io.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     1867 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/losses.py
--rw-rw-r--   0 deema     (1000) deema     (1000)     3695 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/metrics.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    29213 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/model_trainer.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    45377 2023-05-09 22:59:52.000000 torch_utilities-1.0.4/torch_utilities/modules.py
--rw-rw-r--   0 deema     (1000) deema     (1000)    10451 2023-05-09 22:58:46.000000 torch_utilities-1.0.4/torch_utilities/pytorch.py
-drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-09 23:05:44.705839 torch_utilities-1.0.4/torch_utilities.egg-info/
--rw-rw-r--   0 deema     (1000) deema     (1000)     5072 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/PKG-INFO
--rw-rw-r--   0 deema     (1000) deema     (1000)     1163 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/SOURCES.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)        1 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/dependency_links.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      147 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/entry_points.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)      154 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/requires.txt
--rw-rw-r--   0 deema     (1000) deema     (1000)       22 2023-05-09 23:05:44.000000 torch_utilities-1.0.4/torch_utilities.egg-info/top_level.txt
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-26 13:02:45.468980 torch_utilities-1.0.5/
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1074 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/LICENSE
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5072 2023-05-26 13:02:45.468980 torch_utilities-1.0.5/PKG-INFO
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4735 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/README.md
+-rw-rw-r--   0 deema     (1000) deema     (1000)       80 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/pyproject.toml
+-rw-rw-r--   0 deema     (1000) deema     (1000)      837 2023-05-26 13:02:45.468980 torch_utilities-1.0.5/setup.cfg
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-26 13:02:45.464980 torch_utilities-1.0.5/tests/
+-rw-rw-r--   0 deema     (1000) deema     (1000)      196 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/__init__.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3514 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/generate_test_data.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    11107 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_audio.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     2179 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_augmentation.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     6096 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_common.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5870 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_data_loading.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     2045 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_features.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4081 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_io.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1228 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_metrics.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     9425 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_model_trainer.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    37668 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_modules.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3980 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/tests/test_pytorch.py
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-26 13:02:45.464980 torch_utilities-1.0.5/torch_utilities/
+-rw-rw-r--   0 deema     (1000) deema     (1000)      410 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/__init__.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    17154 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/audio.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     6376 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/augmentation.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     9044 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/common.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    13587 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/data_loading.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     4079 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/features.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     7047 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/io.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1867 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/losses.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)     3695 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/metrics.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    29213 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/model_trainer.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    45377 2023-05-26 12:58:15.000000 torch_utilities-1.0.5/torch_utilities/modules.py
+-rw-rw-r--   0 deema     (1000) deema     (1000)    10451 2023-05-09 22:58:46.000000 torch_utilities-1.0.5/torch_utilities/pytorch.py
+drwxrwxr-x   0 deema     (1000) deema     (1000)        0 2023-05-26 13:02:45.468980 torch_utilities-1.0.5/torch_utilities.egg-info/
+-rw-rw-r--   0 deema     (1000) deema     (1000)     5072 2023-05-26 13:02:45.000000 torch_utilities-1.0.5/torch_utilities.egg-info/PKG-INFO
+-rw-rw-r--   0 deema     (1000) deema     (1000)     1163 2023-05-26 13:02:45.000000 torch_utilities-1.0.5/torch_utilities.egg-info/SOURCES.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)        1 2023-05-26 13:02:45.000000 torch_utilities-1.0.5/torch_utilities.egg-info/dependency_links.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)      147 2023-05-26 13:02:45.000000 torch_utilities-1.0.5/torch_utilities.egg-info/entry_points.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)      154 2023-05-26 13:02:45.000000 torch_utilities-1.0.5/torch_utilities.egg-info/requires.txt
+-rw-rw-r--   0 deema     (1000) deema     (1000)       22 2023-05-26 13:02:45.000000 torch_utilities-1.0.5/torch_utilities.egg-info/top_level.txt
```

### Comparing `torch_utilities-1.0.4/LICENSE` & `torch_utilities-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/PKG-INFO` & `torch_utilities-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_utilities
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `torch_utilities-1.0.4/README.md` & `torch_utilities-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/setup.cfg` & `torch_utilities-1.0.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = torch_utilities
-version = 1.0.4
+version = 1.0.5
 author = Federico Di Marzo
 author_email = federicodimarzo@protonmail.com
 description = Simplifying audio and deep learning with PyTorch.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/FedericoDiMarzo/torch_utilities
```

### Comparing `torch_utilities-1.0.4/tests/generate_test_data.py` & `torch_utilities-1.0.5/tests/generate_test_data.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_audio.py` & `torch_utilities-1.0.5/tests/test_audio.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_augmentation.py` & `torch_utilities-1.0.5/tests/test_augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_common.py` & `torch_utilities-1.0.5/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_data_loading.py` & `torch_utilities-1.0.5/tests/test_data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_features.py` & `torch_utilities-1.0.5/tests/test_features.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_io.py` & `torch_utilities-1.0.5/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_metrics.py` & `torch_utilities-1.0.5/tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_model_trainer.py` & `torch_utilities-1.0.5/tests/test_model_trainer.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_modules.py` & `torch_utilities-1.0.5/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/tests/test_pytorch.py` & `torch_utilities-1.0.5/tests/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/audio.py` & `torch_utilities-1.0.5/torch_utilities/audio.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/augmentation.py` & `torch_utilities-1.0.5/torch_utilities/augmentation.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/common.py` & `torch_utilities-1.0.5/torch_utilities/common.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/data_loading.py` & `torch_utilities-1.0.5/torch_utilities/data_loading.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/features.py` & `torch_utilities-1.0.5/torch_utilities/features.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/io.py` & `torch_utilities-1.0.5/torch_utilities/io.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/losses.py` & `torch_utilities-1.0.5/torch_utilities/losses.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/metrics.py` & `torch_utilities-1.0.5/torch_utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/model_trainer.py` & `torch_utilities-1.0.5/torch_utilities/model_trainer.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities/modules.py` & `torch_utilities-1.0.5/torch_utilities/modules.py`

 * *Files 0% similar despite different names*

```diff
@@ -682,15 +682,15 @@
         pad_f = dilation_f * (kernel_size_f - 1) + 1 - self.stride_f
         half_pad_f = pad_f // 2
         if self.padding_f is not None:
             pad = nn.Identity()  # manual padding
         elif pad_f % 2 == 0:
             pad = nn.ConstantPad2d((half_pad_f, half_pad_f, 0, 0), 0)
         else:
-            pad = nn.ConstantPad2d((half_pad_f, half_pad_f + 1, 0, 0), 0)
+            pad = nn.ConstantPad2d((half_pad_f + 1, half_pad_f, 0, 0), 0)
         return pad
 
 
 class CausalSubConv2d(Module):
     def __init__(
         self,
         in_channels: int,
```

### Comparing `torch_utilities-1.0.4/torch_utilities/pytorch.py` & `torch_utilities-1.0.5/torch_utilities/pytorch.py`

 * *Files identical despite different names*

### Comparing `torch_utilities-1.0.4/torch_utilities.egg-info/PKG-INFO` & `torch_utilities-1.0.5/torch_utilities.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-utilities
-Version: 1.0.4
+Version: 1.0.5
 Summary: Simplifying audio and deep learning with PyTorch.
 Home-page: https://github.com/FedericoDiMarzo/torch_utilities
 Author: Federico Di Marzo
 Author-email: federicodimarzo@protonmail.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `torch_utilities-1.0.4/torch_utilities.egg-info/SOURCES.txt` & `torch_utilities-1.0.5/torch_utilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

