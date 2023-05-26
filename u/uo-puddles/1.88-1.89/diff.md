# Comparing `tmp/uo_puddles-1.88.tar.gz` & `tmp/uo_puddles-1.89.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uo_puddles-1.88.tar", last modified: Fri Apr 21 22:32:05 2023, max compression
+gzip compressed data, was "uo_puddles-1.89.tar", last modified: Fri May 26 21:02:16 2023, max compression
```

## Comparing `uo_puddles-1.88.tar` & `uo_puddles-1.89.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:32:05.991790 uo_puddles-1.88/
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-04-21 22:31:51.000000 uo_puddles-1.88/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-21 22:32:05.991790 uo_puddles-1.88/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-21 22:31:51.000000 uo_puddles-1.88/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 22:31:51.000000 uo_puddles-1.88/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 22:32:05.991790 uo_puddles-1.88/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      748 2023-04-21 22:31:51.000000 uo_puddles-1.88/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:32:05.991790 uo_puddles-1.88/uo_puddles/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/cis423.py
--rw-r--r--   0 runner    (1001) docker     (123)    26237 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/good_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/good_ai_22.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/gremcat_df.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-04-21 22:31:51.000000 uo_puddles-1.88/uo_puddles/gremcat_oo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 22:32:05.991790 uo_puddles-1.88/uo_puddles.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-21 22:32:05.000000 uo_puddles-1.88/uo_puddles.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-21 22:32:05.000000 uo_puddles-1.88/uo_puddles.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 22:32:05.000000 uo_puddles-1.88/uo_puddles.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-21 22:32:05.000000 uo_puddles-1.88/uo_puddles.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:02:16.582081 uo_puddles-1.89/
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-26 21:02:07.000000 uo_puddles-1.89/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-26 21:02:16.582081 uo_puddles-1.89/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-26 21:02:07.000000 uo_puddles-1.89/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 21:02:07.000000 uo_puddles-1.89/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 21:02:16.582081 uo_puddles-1.89/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      748 2023-05-26 21:02:07.000000 uo_puddles-1.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:02:16.582081 uo_puddles-1.89/uo_puddles/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19518 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/cis423.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26336 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/good_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24737 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/good_ai_22.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/gremcat_df.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-26 21:02:07.000000 uo_puddles-1.89/uo_puddles/gremcat_oo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 21:02:16.582081 uo_puddles-1.89/uo_puddles.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-26 21:02:16.000000 uo_puddles-1.89/uo_puddles.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-26 21:02:16.000000 uo_puddles-1.89/uo_puddles.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 21:02:16.000000 uo_puddles-1.89/uo_puddles.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-26 21:02:16.000000 uo_puddles-1.89/uo_puddles.egg-info/top_level.txt
```

### Comparing `uo_puddles-1.88/LICENSE.txt` & `uo_puddles-1.89/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.88/setup.py` & `uo_puddles-1.89/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="uo_puddles",
-    version="1.88",    #also change pypi_version variable at top of library
+    version="1.89",    #also change pypi_version variable at top of library
     author="Stephen Fickas",
     author_email="stephenfickas@gmail.com",
     description="for cis423 class",
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `uo_puddles-1.88/uo_puddles/cis423.py` & `uo_puddles-1.89/uo_puddles/cis423.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.88/uo_puddles/good_ai.py` & `uo_puddles-1.89/uo_puddles/good_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -438,27 +438,28 @@
 from tensorflow.keras import Sequential
 from tensorflow.keras.layers import Dense, Activation, Dropout
 import tensorflow as tf
 from tensorflow import keras
 
 import matplotlib.pyplot as plt
 
-def up_neural_net(train_table, test_table, architecture):
+def up_neural_net(train_table, test_table, architecture, target):
   assert isinstance(train_table, pd.core.frame.DataFrame), f'Puddles says: expecting train_table to be table but instead got a {type(train_table)}!'
   assert isinstance(test_table, pd.core.frame.DataFrame), f'Puddles says: expecting test_table to be table but instead got a {type(test_table)}!'
   assert isinstance(architecture, list) or isinstance(architecture, tuple), f'architecture is a list or tuple, the number of nodes per layer. Instead got {type(architecture)}'
   assert architecture, f'architecture cannot be the empty list'
   assert all([isinstance(x,int) and x>0 for x in architecture]), f'Puddles says: architecture must contain integers greater than 0'
+  assert target in set(train_table.columns)
+  assert target in set(test_table.columns)
 
 
   np.random.seed(seed=1234)
   tf.random.set_seed(1234)
 
   columns = up_list_column_names(train_table)
-  target = columns[-1]
   new_train = train_table.drop(columns=target).to_numpy()
   labels = np.array(up_get_column(train_table, target))
   new_test = test_table.drop(columns=target).to_numpy()
   n = len(columns)-1
 
   metrics=tf.keras.metrics.BinaryAccuracy(
     name='binary_accuracy', dtype=None, threshold=0.5
@@ -490,34 +491,35 @@
     layer_units = layer
     model.add(Dense(units=layer_units, activation=layer_act, activity_regularizer=l2_regu, kernel_initializer=initializer))
     model.add(Dropout(layer_dropout))
     
   #now output layer
   model.add(Dense(units=1, activation='sigmoid'))
 
-  model.compile(loss=loss,
-              optimizer=keras.optimizers.Adam(learning_rate=learning_rate),
-              metrics=[metrics])
+  model.compile(optimizer=keras.optimizers.Adam(learning_rate=learning_rate),
+              metrics=[metrics],
+              loss=loss,
+               )
   
   batch = 20
   epochs = 100
   training = model.fit(x=new_train,
                           y=labels,
                           batch_size=batch,
                           epochs=epochs,
                           verbose=0,
                           callbacks=[early_stop_cb])
   print(f'Finished training with {len(training.history["loss"])} epochs ...')
-
+  '''
   plt.plot(training.history['binary_accuracy'])
   plt.title('model accuracy')
   plt.ylabel('accuracy')
   plt.xlabel('epoch')
   plt.show()
-
+  '''
   np_predictions = model.predict(new_test)
 
   predictions = [[1-p[0], p[0]] for p in np_predictions]
   print('Finished testing ...')
   return predictions
 
 def up_lower_string_list(string_list):
```

### Comparing `uo_puddles-1.88/uo_puddles/good_ai_22.py` & `uo_puddles-1.89/uo_puddles/good_ai_22.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.88/uo_puddles/gremcat_df.py` & `uo_puddles-1.89/uo_puddles/gremcat_df.py`

 * *Files identical despite different names*

### Comparing `uo_puddles-1.88/uo_puddles/gremcat_oo.py` & `uo_puddles-1.89/uo_puddles/gremcat_oo.py`

 * *Files identical despite different names*

