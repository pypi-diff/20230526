# Comparing `tmp/flowchain-0.0.2.tar.gz` & `tmp/flowchain-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchain-0.0.2.tar", last modified: Fri May 26 15:33:35 2023, max compression
+gzip compressed data, was "flowchain-0.0.3.tar", last modified: Fri May 26 15:47:11 2023, max compression
```

## Comparing `flowchain-0.0.2.tar` & `flowchain-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:33:35.372752 flowchain-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 15:33:21.000000 flowchain-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 15:33:35.372752 flowchain-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-26 15:33:21.000000 flowchain-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:33:35.372752 flowchain-0.0.2/flowchain/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 15:33:21.000000 flowchain-0.0.2/flowchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-26 15:33:21.000000 flowchain-0.0.2/flowchain/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:33:35.372752 flowchain-0.0.2/flowchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 15:33:35.000000 flowchain-0.0.2/flowchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 15:33:35.000000 flowchain-0.0.2/flowchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:33:35.000000 flowchain-0.0.2/flowchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:33:35.000000 flowchain-0.0.2/flowchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:33:35.372752 flowchain-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 15:33:21.000000 flowchain-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:47:11.041035 flowchain-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 15:46:59.000000 flowchain-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 15:47:11.041035 flowchain-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-26 15:46:59.000000 flowchain-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:47:11.037035 flowchain-0.0.3/flowchain/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 15:46:59.000000 flowchain-0.0.3/flowchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-05-26 15:46:59.000000 flowchain-0.0.3/flowchain/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:47:11.041035 flowchain-0.0.3/flowchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 15:47:11.000000 flowchain-0.0.3/flowchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 15:47:11.000000 flowchain-0.0.3/flowchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:47:11.000000 flowchain-0.0.3/flowchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:47:11.000000 flowchain-0.0.3/flowchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:47:11.041035 flowchain-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 15:46:59.000000 flowchain-0.0.3/setup.py
```

### Comparing `flowchain-0.0.2/LICENSE` & `flowchain-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.2/PKG-INFO` & `flowchain-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Flowchain - Method Chaining for TensorFlow
 Home-page: https://github.com/OrigamiDream/flowchain
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,method chaining,extension
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flowchain-0.0.2/flowchain/chain.py` & `flowchain-0.0.3/flowchain/chain.py`

 * *Files 12% similar despite different names*

```diff
@@ -91,19 +91,7 @@
 
 
 def enable_tensor_chaining(mappings=None):
     register_tensor_chaining(tf.Variable, mappings)
     register_tensor_chaining(tf.Tensor, mappings)
     register_tensor_chaining(tf.RaggedTensor, mappings)
     register_tensor_chaining(tf.SparseTensor, mappings)
-
-    try:
-        from keras.engine.keras_tensor import KerasTensor
-        register_tensor_chaining(KerasTensor, mappings)
-    except ImportError:
-        pass
-
-    try:
-        from keras.src.engine.keras_tensor import KerasTensor
-        register_tensor_chaining(KerasTensor, mappings)
-    except ImportError:
-        pass
```

### Comparing `flowchain-0.0.2/flowchain.egg-info/PKG-INFO` & `flowchain-0.0.3/flowchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchain
-Version: 0.0.2
+Version: 0.0.3
 Summary: Flowchain - Method Chaining for TensorFlow
 Home-page: https://github.com/OrigamiDream/flowchain
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,method chaining,extension
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flowchain-0.0.2/setup.py` & `flowchain-0.0.3/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flowchain',
     packages=find_packages(exclude=[]),
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     description='Flowchain - Method Chaining for TensorFlow',
     author='OrigamiDream',
     author_email='hello@origamidream.me',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/OrigamiDream/flowchain',
```

