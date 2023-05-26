# Comparing `tmp/MEGABYTE-pytorch-0.0.8.tar.gz` & `tmp/MEGABYTE-pytorch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MEGABYTE-pytorch-0.0.8.tar", last modified: Fri May 26 16:46:05 2023, max compression
+gzip compressed data, was "MEGABYTE-pytorch-0.0.9.tar", last modified: Fri May 26 16:46:54 2023, max compression
```

## Comparing `MEGABYTE-pytorch-0.0.8.tar` & `MEGABYTE-pytorch-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:05.646130 MEGABYTE-pytorch-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 16:45:53.000000 MEGABYTE-pytorch-0.0.8/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:05.642130 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 16:45:53.000000 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-26 16:45:53.000000 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    12346 2023-05-26 16:45:53.000000 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch/megabyte.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:05.642130 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 16:46:05.000000 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-26 16:46:05.000000 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:46:05.000000 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 16:46:05.000000 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:46:05.000000 MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 16:46:05.646130 MEGABYTE-pytorch-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-26 16:45:53.000000 MEGABYTE-pytorch-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:46:05.646130 MEGABYTE-pytorch-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-26 16:45:53.000000 MEGABYTE-pytorch-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/megabyte.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 16:46:54.000000 MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3512 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 16:46:54.771808 MEGABYTE-pytorch-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-26 16:46:43.000000 MEGABYTE-pytorch-0.0.9/setup.py
```

### Comparing `MEGABYTE-pytorch-0.0.8/LICENSE` & `MEGABYTE-pytorch-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch/attend.py` & `MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch/megabyte.py` & `MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch/megabyte.py`

 * *Files 1% similar despite different names*

```diff
@@ -258,15 +258,15 @@
                 attn_dropout = attn_dropout,
                 ff_dropout = ff_dropout,
                 ff_mult = ff_mult,
                 rel_pos_bias = rel_pos_bias,
                 flash_attn = flash_attn
             ))
 
-            proj = nn.Linear(h_dim, next_h_dim) if exists(next_h_dim) else nn.Identity()
+            proj = nn.Linear(h_dim, next_h_dim) if exists(next_h_dim) and next_h_dim != dim else nn.Identity()
             self.to_next_transformer_projections.append(proj)
 
         self.to_logits = nn.Linear(fine_dim, num_tokens)
         self.pad_id = pad_id
 
     def generate(self, prime = None, filter_thres = 0.9, temperature = 1., default_batch_size = 1):
         total_seq_len = reduce_mult(self.max_seq_len)
```

### Comparing `MEGABYTE-pytorch-0.0.8/MEGABYTE_pytorch.egg-info/PKG-INFO` & `MEGABYTE-pytorch-0.0.9/MEGABYTE_pytorch.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.8/PKG-INFO` & `MEGABYTE-pytorch-0.0.9/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MEGABYTE-pytorch
-Version: 0.0.8
+Version: 0.0.9
 Summary: MEGABYTE - Pytorch
 Home-page: https://github.com/lucidrains/MEGABYTE-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,attention mechanism,transformers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `MEGABYTE-pytorch-0.0.8/README.md` & `MEGABYTE-pytorch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `MEGABYTE-pytorch-0.0.8/setup.py` & `MEGABYTE-pytorch-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'MEGABYTE-pytorch',
   packages = find_packages(),
-  version = '0.0.8',
+  version = '0.0.9',
   license='MIT',
   description = 'MEGABYTE - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/MEGABYTE-pytorch',
   keywords = [
```

