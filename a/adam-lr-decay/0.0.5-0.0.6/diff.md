# Comparing `tmp/adam-lr-decay-0.0.5.tar.gz` & `tmp/adam-lr-decay-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adam-lr-decay-0.0.5.tar", last modified: Wed Mar 29 05:03:16 2023, max compression
+gzip compressed data, was "adam-lr-decay-0.0.6.tar", last modified: Fri May 26 18:46:58 2023, max compression
```

## Comparing `adam-lr-decay-0.0.5.tar` & `adam-lr-decay-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:03:16.372162 adam-lr-decay-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-29 05:03:06.000000 adam-lr-decay-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-29 05:03:16.372162 adam-lr-decay-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-03-29 05:03:06.000000 adam-lr-decay-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:03:16.372162 adam-lr-decay-0.0.5/adam_lr_decay/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-03-29 05:03:06.000000 adam-lr-decay-0.0.5/adam_lr_decay/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5672 2023-03-29 05:03:06.000000 adam-lr-decay-0.0.5/adam_lr_decay/adam_lr_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-29 05:03:16.372162 adam-lr-decay-0.0.5/adam_lr_decay.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-03-29 05:03:16.000000 adam-lr-decay-0.0.5/adam_lr_decay.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-03-29 05:03:16.000000 adam-lr-decay-0.0.5/adam_lr_decay.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-29 05:03:16.000000 adam-lr-decay-0.0.5/adam_lr_decay.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-03-29 05:03:16.000000 adam-lr-decay-0.0.5/adam_lr_decay.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-29 05:03:16.000000 adam-lr-decay-0.0.5/adam_lr_decay.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-29 05:03:16.372162 adam-lr-decay-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-03-29 05:03:06.000000 adam-lr-decay-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:46:58.957147 adam-lr-decay-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 18:46:47.000000 adam-lr-decay-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-26 18:46:58.957147 adam-lr-decay-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-05-26 18:46:47.000000 adam-lr-decay-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:46:58.953147 adam-lr-decay-0.0.6/adam_lr_decay/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 18:46:47.000000 adam-lr-decay-0.0.6/adam_lr_decay/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5697 2023-05-26 18:46:47.000000 adam-lr-decay-0.0.6/adam_lr_decay/adam_lr_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:46:58.957147 adam-lr-decay-0.0.6/adam_lr_decay.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-26 18:46:58.000000 adam-lr-decay-0.0.6/adam_lr_decay.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-26 18:46:58.000000 adam-lr-decay-0.0.6/adam_lr_decay.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:46:58.000000 adam-lr-decay-0.0.6/adam_lr_decay.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-26 18:46:58.000000 adam-lr-decay-0.0.6/adam_lr_decay.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 18:46:58.000000 adam-lr-decay-0.0.6/adam_lr_decay.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:46:58.957147 adam-lr-decay-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 18:46:47.000000 adam-lr-decay-0.0.6/setup.py
```

### Comparing `adam-lr-decay-0.0.5/LICENSE` & `adam-lr-decay-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `adam-lr-decay-0.0.5/PKG-INFO` & `adam-lr-decay-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-lr-decay
-Version: 0.0.5
+Version: 0.0.6
 Summary: Adam Layer-wise LR Decay
 Home-page: https://github.com/OrigamiDream/adam-lr-decay
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,optimizers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adam-lr-decay-0.0.5/README.md` & `adam-lr-decay-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `adam-lr-decay-0.0.5/adam_lr_decay/adam_lr_decay.py` & `adam-lr-decay-0.0.6/adam_lr_decay/adam_lr_decay.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import re
+from flowchain import enable_tensor_chaining
 from typing import Union
 
 try:
     import tensorflow as tf
     from tensorflow.keras import optimizers
 except ImportError as e:
     raise ImportError('You must install `tensorflow>=2.11` or `tensorflow-cpu>=2.11`: {}'.format(e))
@@ -10,14 +11,16 @@
 from packaging import version
 
 if version.parse(tf.__version__) < version.parse('2.11.0'):
     raise version.InvalidVersion(
         'The tensorflow must be greater than or equal to 2.11, but current version is `{}`'.format(tf.__version__)
     )
 
+enable_tensor_chaining()
+
 
 class AdamLRDecay(optimizers.Adam):
     def __init__(self,
                  learning_rate: Union[float, tf.Tensor, optimizers.schedules.LearningRateSchedule] = 0.001,
                  beta_1=0.9,
                  beta_2=0.999,
                  epsilon=1e-7,
@@ -75,68 +78,68 @@
                 return rate
         for name, rate in mapped_layerwise_lr_decay_names.items():
             if re.search(name, variable.name) is not None:
                 return rate
         return None
 
     def _calculate_learning_rate(self, variable):
-        lr = tf.cast(self.learning_rate, variable.dtype)
+        lr = self.learning_rate.cast(variable.dtype)
         decay_rate = self._use_layerwise_lr_decay(variable)
         if decay_rate is not None:
-            decay_rate = tf.cast(decay_rate, variable.dtype)
+            decay_rate = decay_rate.cast(variable.dtype)
             return lr * (1. - decay_rate)
         return lr
 
     def update_step(self, gradient, variable):
         """Update step given gradient and the associated model variable."""
         lr = self._calculate_learning_rate(variable)
-        local_step = tf.cast(self.iterations + 1, variable.dtype)
-        beta_1_power = tf.pow(tf.cast(self.beta_1, variable.dtype), local_step)
-        beta_2_power = tf.pow(tf.cast(self.beta_2, variable.dtype), local_step)
+        local_step = (self.iterations + 1).cast(variable.dtype)
+        beta_1_power = self.beta_1.cast(variable.dtype) ** local_step
+        beta_2_power = self.beta_2.cast(variable.dtype) ** local_step
 
         var_key = self._var_key(variable)
         m = self._momentums[self._index_dict[var_key]]
         v = self._velocities[self._index_dict[var_key]]
 
-        alpha = lr * tf.sqrt(1 - beta_2_power) / (1 - beta_1_power)
+        alpha = lr * (1 - beta_2_power).sqrt() / (1 - beta_1_power)
 
         if isinstance(gradient, tf.IndexedSlices):
             # Sparse gradients.
             m.assign_add(-m * (1 - self.beta_1))
             m.scatter_add(
                 tf.IndexedSlices(
                     gradient.values * (1 - self.beta_1), gradient.indices
                 )
             )
             v.assign_add(-v * (1 - self.beta_2))
             v.scatter_add(
                 tf.IndexedSlices(
-                    tf.square(gradient.values) * (1 - self.beta_2),
+                    gradient.values.square() * (1 - self.beta_2),
                     gradient.indices,
-                    )
+                )
             )
             if self.amsgrad:
                 v_hat = self._velocity_hats[self._index_dict[var_key]]
                 v_hat.assign(tf.maximum(v_hat, v))
                 v = v_hat
-            variable.assign_sub((m * alpha) / (tf.sqrt(v) + self.epsilon))
+            variable.assign_sub((m * alpha) / (v.sqrt() + self.epsilon))
         else:
             # Dense gradients.
             m.assign_add((gradient - m) * (1 - self.beta_1))
-            v.assign_add((tf.square(gradient) - v) * (1 - self.beta_2))
+            v.assign_add((gradient.square() - v) * (1 - self.beta_2))
             if self.amsgrad:
                 v_hat = self._velocity_hats[self._index_dict[var_key]]
                 v_hat.assign(tf.maximum(v_hat, v))
                 v = v_hat
-            variable.assign_sub((m * alpha) / (tf.sqrt(v) + self.epsilon))
+            variable.assign_sub((m * alpha) / (v.sqrt() + self.epsilon))
 
     def _apply_weight_decay(self, variables):
         if self.weight_decay is None:
             return
         for variable in variables:
             if self._use_weight_decay(variable):
                 lr = self._calculate_learning_rate(variable)
-                wd = tf.cast(self.weight_decay, variable.dtype)
+                wd = self.weight_decay.cast(variable.dtype)
                 variable.assign_sub(variable * wd * lr)
 
     def get_config(self):
         return super().get_config()
```

### Comparing `adam-lr-decay-0.0.5/adam_lr_decay.egg-info/PKG-INFO` & `adam-lr-decay-0.0.6/adam_lr_decay.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adam-lr-decay
-Version: 0.0.5
+Version: 0.0.6
 Summary: Adam Layer-wise LR Decay
 Home-page: https://github.com/OrigamiDream/adam-lr-decay
 Author: OrigamiDream
 Author-email: hello@origamidream.me
 License: MIT
 Keywords: machine learning,deep learning,tensorflow,optimizers
 Classifier: Development Status :: 4 - Beta
```

### Comparing `adam-lr-decay-0.0.5/setup.py` & `adam-lr-decay-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name='adam-lr-decay',
     packages=find_packages(exclude=[]),
-    version='0.0.5',
+    version='0.0.6',
     license='MIT',
     description='Adam Layer-wise LR Decay',
     author='OrigamiDream',
     author_email='hello@origamidream.me',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/OrigamiDream/adam-lr-decay',
     python_requires='>=3.8.0',
     extras_require={
         'gpu': ['tensorflow>=2.11'],
         'cpu': ['tensorflow-cpu>=2.11']
     },
     install_requires=[
-        'packaging'
+        'packaging',
+        'flowchain>=0.0.4'
     ],
     keywords=[
         'machine learning',
         'deep learning',
         'tensorflow',
         'optimizers',
     ],
```

