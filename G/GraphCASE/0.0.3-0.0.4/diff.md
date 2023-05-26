# Comparing `tmp/GraphCASE-0.0.3.tar.gz` & `tmp/GraphCASE-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "GraphCASE-0.0.3.tar", last modified: Tue Oct 11 17:43:29 2022, max compression
+gzip compressed data, was "GraphCASE-0.0.4.tar", last modified: Fri May 26 07:15:42 2023, max compression
```

## Comparing `GraphCASE-0.0.3.tar` & `GraphCASE-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2022-10-11 17:43:29.854167 GraphCASE-0.0.3/
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2022-10-11 17:43:29.852062 GraphCASE-0.0.3/GAE/
--rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.3/GAE/__init__.py
--rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.3/GAE/dataFeeder.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11494 2022-09-19 17:34:14.000000 GraphCASE-0.0.3/GAE/data_feeder_graphframes.py
--rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13494 2022-09-19 17:34:14.000000 GraphCASE-0.0.3/GAE/data_feeder_nx.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    15494 2022-09-26 09:18:51.000000 GraphCASE-0.0.3/GAE/graph_case_controller.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     2585 2022-09-26 09:14:26.000000 GraphCASE-0.0.3/GAE/graph_case_tools.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7511 2022-09-23 08:42:42.000000 GraphCASE-0.0.3/GAE/graph_reconstructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)    10903 2022-09-26 06:58:27.000000 GraphCASE-0.0.3/GAE/input_layer_constructor.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     8464 2022-09-19 17:34:14.000000 GraphCASE-0.0.3/GAE/model.py
--rw-r--r--   0 tonpoppe   (501) staff       (20)     6660 2022-09-19 17:34:14.000000 GraphCASE-0.0.3/GAE/transformation_layer.py
-drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2022-10-11 17:43:29.853434 GraphCASE-0.0.3/GraphCASE.egg-info/
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2022-10-11 17:43:28.000000 GraphCASE-0.0.3/GraphCASE.egg-info/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)      401 2022-10-11 17:43:29.000000 GraphCASE-0.0.3/GraphCASE.egg-info/SOURCES.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2022-10-11 17:43:29.000000 GraphCASE-0.0.3/GraphCASE.egg-info/dependency_links.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2022-10-11 17:43:29.000000 GraphCASE-0.0.3/GraphCASE.egg-info/top_level.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.3/LICENSE.txt
--rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2022-10-11 17:43:29.853853 GraphCASE-0.0.3/PKG-INFO
--rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.3/README.md
--rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2022-10-11 17:43:29.854277 GraphCASE-0.0.3/setup.cfg
--rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2022-10-11 17:43:25.000000 GraphCASE-0.0.3/setup.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-05-26 07:15:42.102336 GraphCASE-0.0.4/
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-05-26 07:15:42.099966 GraphCASE-0.0.4/GAE/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        0 2020-07-29 20:02:56.000000 GraphCASE-0.0.4/GAE/__init__.py
+-rw-rw-rw-   0 tonpoppe   (501) staff       (20)     6564 2020-07-21 05:00:15.000000 GraphCASE-0.0.4/GAE/dataFeeder.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    11493 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/data_feeder_graphframes.py
+-rwxr-xr-x   0 tonpoppe   (501) staff       (20)    13402 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/data_feeder_nx.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    15634 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/graph_case_controller.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     2585 2022-09-26 09:14:26.000000 GraphCASE-0.0.4/GAE/graph_case_tools.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     7511 2022-09-23 08:42:42.000000 GraphCASE-0.0.4/GAE/graph_reconstructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    13470 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/input_layer_constructor.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     8746 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/model.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    12802 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/position_manager.py
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     6979 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/GAE/transformation_layer.py
+drwxr-xr-x   0 tonpoppe   (501) staff       (20)        0 2023-05-26 07:15:42.101554 GraphCASE-0.0.4/GraphCASE.egg-info/
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-05-26 07:15:41.000000 GraphCASE-0.0.4/GraphCASE.egg-info/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      425 2023-05-26 07:15:42.000000 GraphCASE-0.0.4/GraphCASE.egg-info/SOURCES.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        1 2023-05-26 07:15:41.000000 GraphCASE-0.0.4/GraphCASE.egg-info/dependency_links.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)        4 2023-05-26 07:15:41.000000 GraphCASE-0.0.4/GraphCASE.egg-info/top_level.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)    35149 2020-07-19 21:06:49.000000 GraphCASE-0.0.4/LICENSE.txt
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      296 2023-05-26 07:15:42.101979 GraphCASE-0.0.4/PKG-INFO
+-rw-r--r--   0 tonpoppe   (501) staff       (20)     7404 2022-09-19 17:31:14.000000 GraphCASE-0.0.4/README.md
+-rw-r--r--   0 tonpoppe   (501) staff       (20)       38 2023-05-26 07:15:42.102454 GraphCASE-0.0.4/setup.cfg
+-rw-r--r--   0 tonpoppe   (501) staff       (20)      322 2023-05-26 07:12:59.000000 GraphCASE-0.0.4/setup.py
```

### Comparing `GraphCASE-0.0.3/GAE/dataFeeder.py` & `GraphCASE-0.0.4/GAE/dataFeeder.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.3/GAE/data_feeder_graphframes.py` & `GraphCASE-0.0.4/GAE/data_feeder_graphframes.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
         # determine node number of the dummy node
         if self.dummy_id is None:
             self.dummy_id = self.node_df.count()  # count starts with zero
 
         edge = (edge
             .withColumn(
-                'edge_features', 
+                'edge_features',
                 F.when(F.col(counterparty).isNull(), None)
                     .otherwise(F.array(self.edge_labels))
                 )
             )
 
         w = Window.partitionBy('id').orderBy(-F.col('weight')).rowsBetween(0, self.neighb_size-1)
         w2 = Window.partitionBy('id').orderBy(-F.col('weight'))
```

### Comparing `GraphCASE-0.0.3/GAE/data_feeder_nx.py` & `GraphCASE-0.0.4/GAE/data_feeder_nx.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,24 +2,21 @@
 # -*- coding: utf-8 -*-
 """
 Created on Fri Jul 26 10:22:45 2019
 
 @author: tonpoppe
 """
 
-import os
 import random
 import tensorflow as tf
-from tensorflow import keras
 import networkx as nx
 import datetime
-from multiprocessing.pool import ThreadPool
 import numpy as np
-from pathlib import Path
-import csv
+from tensorflow import keras
+
 
 class DataFeederNx:
     """
     This class reads a directed network object and covert this to
     the samples for training the GraphCase algorithm.
     Note that the first label with index 0 is used as edge weight.
     No multiple edge labels are currently supported.
```

### Comparing `GraphCASE-0.0.3/GAE/graph_case_controller.py` & `GraphCASE-0.0.4/GAE/graph_case_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import pickle
 from datetime import datetime
 import numpy as np
 import tensorflow as tf
 from GAE.model import GraphAutoEncoderModel
 from GAE.input_layer_constructor import InputLayerConstructor
 from GAE.graph_reconstructor import GraphReconstructor
-from GAE.transformation_layer import DecTransLayer, EncTransLayer, Hub0_encoder, Hub0_decoder
+from GAE.transformation_layer import DecTransLayer, EncTransLayer, Hub0_encoder, Hub0Decoder
 from GAE.data_feeder_nx import DataFeederNx
 tf.compat.v1.logging.set_verbosity(tf.compat.v1.logging.ERROR)
 class GraphAutoEncoder:
     """
     This class implement the graphCase algorithm. Refer for more details
     to the corresponding documentation.
 
@@ -47,15 +47,16 @@
                  weight_label='weight',
                  encoder_labels=None,
                  act=tf.nn.sigmoid,
                  useBN=False,
                  val_fraction=0.3,
                  model_config=None,
                  dropout=False,
-                 data_feeder_cls=DataFeederNx
+                 data_feeder_cls=DataFeederNx,
+                 pos_enc_cls=None
                  ):
         self.learning_rate = learning_rate
         self.dims = dims
         self.hub0_feature_with_neighb_dim = hub0_feature_with_neighb_dim
         self.batch_size = batch_size
         self.support_size = support_size
         self.verbose = verbose
@@ -63,37 +64,38 @@
         self.act = act
         self.weight_label = weight_label
         self.encoder_labels = encoder_labels
         self.useBN = useBN
         self.dropout = dropout
         self.val_fraction = val_fraction
         self.data_feeder_cls = data_feeder_cls
+        self.pos_enc_cls = pos_enc_cls
         if graph is not None:
             self.__consistency_checks()
-            self.sampler = self.__init_sampler(graph, val_fraction)
+            self.sampler = self.__init_sampler(graph, val_fraction, pos_enc_cls)
             self.model = self.__init_model()
         if model_config is not None:
             custom_objects = {
                 "DecTransLayer": DecTransLayer,
                 "EncTransLayer": EncTransLayer,
                 "Hub0_encoder": Hub0_encoder,
-                " Hub0_decoder": Hub0_decoder
+                "Hub0_decoder": Hub0Decoder
             }
             with tf.keras.utils.custom_object_scope(custom_objects):
                 self.model = GraphAutoEncoderModel.from_config(model_config)
 
-    def __init_sampler(self, graph, val_fraction):
+    def __init_sampler(self, graph, val_fraction, pos_enc_cls):
         """
         Initialises the datafeeder
         """
         return InputLayerConstructor(
             graph, support_size=self.support_size, val_fraction=val_fraction,
             batch_size=self.batch_size, verbose=self.verbose, seed=self.seed,
             weight_label=self.weight_label, encoder_labels=self.encoder_labels,
-            data_feeder_cls=self.data_feeder_cls
+            data_feeder_cls=self.data_feeder_cls, pos_enc_cls=pos_enc_cls
         )
 
     def __init_model(self):
         """
         Initialises the model
         """
         model = GraphAutoEncoderModel(
@@ -128,15 +130,15 @@
             A 2d numpy array with one embedding per row.
         """
         self.verbose = verbose
         if verbose:
             print("calculating all embeddings")
 
         if graph is not None:
-            self.sampler = self.__init_sampler(graph, self.val_fraction)
+            self.sampler = self.__init_sampler(graph, self.val_fraction, self.pos_enc_cls)
 
         embedding = None
         counter = 0
         for i in self.sampler.init_incr_batch(nodes):
             counter += 1
             try:
                 embed = self.model.calculate_embedding(i)
```

### Comparing `GraphCASE-0.0.3/GAE/graph_case_tools.py` & `GraphCASE-0.0.4/GAE/graph_case_tools.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.3/GAE/graph_reconstructor.py` & `GraphCASE-0.0.4/GAE/graph_reconstructor.py`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.3/GAE/model.py` & `GraphCASE-0.0.4/GAE/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 @author: tonpoppe
 """
 
 import os
 import tensorflow as tf
 import numpy as np
-from GAE.transformation_layer import DecTransLayer, EncTransLayer, Hub0_encoder, Hub0_decoder
+from GAE.transformation_layer import DecTransLayer, EncTransLayer, Hub0_encoder, Hub0Decoder
 from tensorflow.keras.layers import Dense, BatchNormalization, Dropout, Lambda
 from tensorflow.keras.initializers import GlorotUniform
 
 class GraphAutoEncoderModel(tf.keras.Model):
     """
     Directed graph implementation of GraphCase
 
@@ -64,21 +64,28 @@
         if self.hub0_feature_with_neighb_dim is None:
             # return identity layer when no dimension is set
             return Lambda(lambda x:x)
         return Hub0_encoder(
             self.hub0_feature_with_neighb_dim, self.act, self.seed)
 
     def create_hub0_decoder(self):
+        """Creates the decoder for the last layer. This laer take the embedding
+        as input and return the feature values of the root node Xn
+        and the input for the next layer to decoder Z
+
+        Returns:
+            _type_: Custom tensor keras layer
+        """
         # return identity layer when no dimension is set
         if self.hub0_feature_with_neighb_dim is None:
             return Lambda(lambda x:x)
         dense_size = EncTransLayer.get_output_dim(
             len(self.dims)+1, self.support_size, self.dims, self.feature_dim)
         dense_size = dense_size + self.number_of_node_labels
-        return Hub0_decoder(
+        return Hub0Decoder(
                 dense_size, self.act, self.number_of_node_labels, self.seed)
 
     def get_config(self):
         # config = super(GraphAutoEncoderModel, self).get_config()
         config = {
             "dims": self.dims,
             "support_size": self.support_size,
```

### Comparing `GraphCASE-0.0.3/GAE/transformation_layer.py` & `GraphCASE-0.0.4/GAE/transformation_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,14 @@
         return config
     
 class Hub0_encoder(tf.keras.layers.Layer):
     """
     Combines the features of the target node with the embedding of the target node and calculates
     a new embedding containing both the own features and neighbourhood.
     """
-
     def __init__(self, dim, act, seed=0, **kwargs):
         super(Hub0_encoder, self).__init__(**kwargs)
         self.dim = dim
         self.act = act
         self.seed = seed
         self.dense_layer = Dense(dim, activation=act, kernel_initializer=GlorotUniform(seed=seed))
 
@@ -150,17 +149,24 @@
         config.update({
             "dim": self.dim, 
             "act": self.act, 
             "seed": self.seed
             })
         return config
 
-class Hub0_decoder(tf.keras.layers.Layer):
+class Hub0Decoder(tf.keras.layers.Layer):
+    """Custom tensor keras layer class that extract the root node label Xn
+    and the input for the decorder of Z. Input in this layer is the 
+    embedding.
+
+    Args:
+        tf (_type_): _description_
+    """
     def __init__(self, embedding_dim, act, node_dims, seed=0, **kwargs):
-        super(Hub0_decoder, self).__init__(**kwargs)
+        super(Hub0Decoder, self).__init__(**kwargs)
         self.embedding_dim = embedding_dim
         self.act = act
         self.node_dims = node_dims
         self.seed = seed
         self.dense_layer = Dense(embedding_dim, activation=act, kernel_initializer=GlorotUniform(seed=seed))
 
     def call(self, inputs, training=False):
@@ -173,15 +179,20 @@
         """
         combined = self.dense_layer(inputs[0], training=training)
         feat_out = combined[...,:self.node_dims]
         trans_layer = combined[...,self.node_dims:]
         return (trans_layer, feat_out)
 
     def get_config(self):
-        config = super(Hub0_decoder, self).get_config()
+        """method for getting config to store
+
+        Returns:
+            _type_: _description_
+        """
+        config = super(Hub0Decoder, self).get_config()
         config.update({
             "embedding_dim": self.embedding_dim, 
             "act": self.act, 
             "node_dims": self.node_dims,
             "seed": self.seed
             })
         return config
```

### Comparing `GraphCASE-0.0.3/LICENSE.txt` & `GraphCASE-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `GraphCASE-0.0.3/README.md` & `GraphCASE-0.0.4/README.md`

 * *Files identical despite different names*

