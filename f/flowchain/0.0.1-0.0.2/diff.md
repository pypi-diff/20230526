# Comparing `tmp/flowchain-0.0.1.tar.gz` & `tmp/flowchain-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchain-0.0.1.tar", last modified: Fri May 26 14:56:41 2023, max compression
+gzip compressed data, was "flowchain-0.0.2.tar", last modified: Fri May 26 15:33:35 2023, max compression
```

## Comparing `flowchain-0.0.1.tar` & `flowchain-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:41.796295 flowchain-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 14:56:30.000000 flowchain-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 14:56:41.796295 flowchain-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-26 14:56:30.000000 flowchain-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:41.792295 flowchain-0.0.1/flowchain/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 14:56:30.000000 flowchain-0.0.1/flowchain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-05-26 14:56:30.000000 flowchain-0.0.1/flowchain/chain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:56:41.796295 flowchain-0.0.1/flowchain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 14:56:41.000000 flowchain-0.0.1/flowchain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-26 14:56:41.000000 flowchain-0.0.1/flowchain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:56:41.000000 flowchain-0.0.1/flowchain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 14:56:41.000000 flowchain-0.0.1/flowchain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 14:56:41.000000 flowchain-0.0.1/flowchain.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 14:56:41.796295 flowchain-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-26 14:56:30.000000 flowchain-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:33:35.372752 flowchain-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 15:33:21.000000 flowchain-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 15:33:35.372752 flowchain-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-26 15:33:21.000000 flowchain-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:33:35.372752 flowchain-0.0.2/flowchain/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-26 15:33:21.000000 flowchain-0.0.2/flowchain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-26 15:33:21.000000 flowchain-0.0.2/flowchain/chain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:33:35.372752 flowchain-0.0.2/flowchain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-26 15:33:35.000000 flowchain-0.0.2/flowchain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-26 15:33:35.000000 flowchain-0.0.2/flowchain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:33:35.000000 flowchain-0.0.2/flowchain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 15:33:35.000000 flowchain-0.0.2/flowchain.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 15:33:35.372752 flowchain-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 15:33:21.000000 flowchain-0.0.2/setup.py
```

### Comparing `flowchain-0.0.1/LICENSE` & `flowchain-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchain-0.0.1/PKG-INFO` & `flowchain-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchain
-Version: 0.0.1
+Version: 0.0.2
 Summary: Flowchain - Method Chaining for TensorFlow
 Home-page: https://github.com/OrigamiDream/flowchain
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,method chaining,extension
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flowchain-0.0.1/flowchain/chain.py` & `flowchain-0.0.2/flowchain/chain.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import inspect
 import tensorflow as tf
 
 from inspect import getmembers, isfunction
 from typing import Any, Optional, List, Callable, Tuple, Union
-from tensorflow.python.framework.ops import Tensor
-from keras.engine.keras_tensor import KerasTensor
 
 _TENSOR_FN_CACHE = dict()
 _DEFAULT_MODULE_WHITELIST = [
     ('tensorflow.python.ops.array_ops', ['!concat', '!fill', '!meshgrid', '!ones', '!zeros', '!stack']),
     ('tensorflow.python.ops.gen_array_ops', ['!tile']),
     'tensorflow.python.ops.gen_math_ops',
     'tensorflow.python.ops.gen_nn_ops',
@@ -68,29 +66,44 @@
         signature = inspect.signature(func)
         if len(signature.parameters) == 0:
             continue
         funcs[name] = _tf_func_wrap(func)
     return funcs
 
 
-def enable_tensor_chaining(mappings=None):
+def register_tensor_chaining(obj, mappings=None):
+    global _TENSOR_FN_CACHE
+
     if mappings is None:
         mappings = _DEFAULT_OBJECT_MAPPINGS
 
-    def _register_tensor_chaining(obj):
-        global _TENSOR_FN_CACHE
+    key = str(obj)
+    if key in _TENSOR_FN_CACHE:
+        return False
+    func_map = dict()
+    for orig, whitelist in mappings:
+        func_map.update(_retrieve_tf_func(orig, whitelist))
+    for tf_name, tf_func in func_map.items():
+        if hasattr(obj, tf_name) or 'type' == tf_name:
+            continue
+        setattr(obj, tf_name, tf_func)
+    _TENSOR_FN_CACHE[key] = func_map
+    return True
 
-        key = str(obj)
-        if key in _TENSOR_FN_CACHE:
-            return False
-        func_map = dict()
-        for orig, whitelist in mappings:
-            func_map.update(_retrieve_tf_func(orig, whitelist))
-        for tf_name, tf_func in func_map.items():
-            if hasattr(obj, tf_name) or 'type' == tf_name:
-                continue
-            setattr(obj, tf_name, tf_func)
-        _TENSOR_FN_CACHE[key] = func_map
-        return True
 
-    _register_tensor_chaining(Tensor)
-    _register_tensor_chaining(KerasTensor)
+def enable_tensor_chaining(mappings=None):
+    register_tensor_chaining(tf.Variable, mappings)
+    register_tensor_chaining(tf.Tensor, mappings)
+    register_tensor_chaining(tf.RaggedTensor, mappings)
+    register_tensor_chaining(tf.SparseTensor, mappings)
+
+    try:
+        from keras.engine.keras_tensor import KerasTensor
+        register_tensor_chaining(KerasTensor, mappings)
+    except ImportError:
+        pass
+
+    try:
+        from keras.src.engine.keras_tensor import KerasTensor
+        register_tensor_chaining(KerasTensor, mappings)
+    except ImportError:
+        pass
```

### Comparing `flowchain-0.0.1/flowchain.egg-info/PKG-INFO` & `flowchain-0.0.2/flowchain.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchain
-Version: 0.0.1
+Version: 0.0.2
 Summary: Flowchain - Method Chaining for TensorFlow
 Home-page: https://github.com/OrigamiDream/flowchain
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,method chaining,extension
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flowchain-0.0.1/setup.py` & `flowchain-0.0.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flowchain',
     packages=find_packages(exclude=[]),
-    version='0.0.1',
+    version='0.0.2',
     license='MIT',
     description='Flowchain - Method Chaining for TensorFlow',
     author='OrigamiDream',
     author_email='hello@origamidream.me',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/OrigamiDream/flowchain',
     python_requires='>=3.8.0',
     extra_require={
         'gpu': ['tensorflow>=2.4'],
         'cpu': ['tensorflow-cpu>=2.4']
     },
-    install_requires=[
-        'packaging'
-    ],
+    install_requires=[],
     keywords=[
         'machine learning',
         'deep learning',
         'tensorflow',
         'method chaining',
         'extension'
     ],
```

