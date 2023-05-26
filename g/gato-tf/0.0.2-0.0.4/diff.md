# Comparing `tmp/gato-tf-0.0.2.tar.gz` & `tmp/gato-tf-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gato-tf-0.0.2.tar", last modified: Thu Feb 16 15:24:52 2023, max compression
+gzip compressed data, was "gato-tf-0.0.4.tar", last modified: Fri May 26 18:27:10 2023, max compression
```

## Comparing `gato-tf-0.0.2.tar` & `gato-tf-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 seondongyoung   (501) staff       (20)        0 2023-02-16 15:24:52.116918 gato-tf-0.0.2/
--rw-r--r--   0 seondongyoung   (501) staff       (20)     1068 2022-06-24 10:52:07.000000 gato-tf-0.0.2/LICENSE
--rw-r--r--   0 seondongyoung   (501) staff       (20)      322 2023-02-16 15:24:52.116647 gato-tf-0.0.2/PKG-INFO
--rw-r--r--   0 seondongyoung   (501) staff       (20)     7818 2023-02-16 15:23:24.000000 gato-tf-0.0.2/README.md
-drwxr-xr-x   0 seondongyoung   (501) staff       (20)        0 2023-02-16 15:24:52.073171 gato-tf-0.0.2/gato/
--rw-r--r--   0 seondongyoung   (501) staff       (20)       64 2023-01-29 06:06:22.000000 gato-tf-0.0.2/gato/__init__.py
--rw-r--r--   0 seondongyoung   (501) staff       (20)     2954 2023-01-29 06:00:10.000000 gato-tf-0.0.2/gato/config.py
-drwxr-xr-x   0 seondongyoung   (501) staff       (20)        0 2023-02-16 15:24:52.109659 gato-tf-0.0.2/gato/models/
--rw-r--r--   0 seondongyoung   (501) staff       (20)     4890 2023-01-29 06:11:00.000000 gato-tf-0.0.2/gato/models/__init__.py
--rw-r--r--   0 seondongyoung   (501) staff       (20)    10880 2023-01-29 06:41:17.000000 gato-tf-0.0.2/gato/models/embedding.py
--rw-r--r--   0 seondongyoung   (501) staff       (20)     1634 2023-01-29 06:08:23.000000 gato-tf-0.0.2/gato/models/tokenizers.py
--rw-r--r--   0 seondongyoung   (501) staff       (20)     2837 2023-01-29 06:06:22.000000 gato-tf-0.0.2/gato/models/transformer.py
-drwxr-xr-x   0 seondongyoung   (501) staff       (20)        0 2023-02-16 15:24:52.116154 gato-tf-0.0.2/gato_tf.egg-info/
--rw-r--r--   0 seondongyoung   (501) staff       (20)      322 2023-02-16 15:24:52.000000 gato-tf-0.0.2/gato_tf.egg-info/PKG-INFO
--rw-r--r--   0 seondongyoung   (501) staff       (20)      314 2023-02-16 15:24:52.000000 gato-tf-0.0.2/gato_tf.egg-info/SOURCES.txt
--rw-r--r--   0 seondongyoung   (501) staff       (20)        1 2023-02-16 15:24:52.000000 gato-tf-0.0.2/gato_tf.egg-info/dependency_links.txt
--rw-r--r--   0 seondongyoung   (501) staff       (20)       17 2023-02-16 15:24:52.000000 gato-tf-0.0.2/gato_tf.egg-info/requires.txt
--rw-r--r--   0 seondongyoung   (501) staff       (20)        5 2023-02-16 15:24:52.000000 gato-tf-0.0.2/gato_tf.egg-info/top_level.txt
--rw-r--r--   0 seondongyoung   (501) staff       (20)       38 2023-02-16 15:24:52.117017 gato-tf-0.0.2/setup.cfg
--rw-r--r--   0 seondongyoung   (501) staff       (20)      486 2023-02-16 15:23:59.000000 gato-tf-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:10.823619 gato-tf-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-26 18:26:51.000000 gato-tf-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-26 18:27:10.823619 gato-tf-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-05-26 18:26:51.000000 gato-tf-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:10.819619 gato-tf-0.0.4/gato/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-26 18:26:51.000000 gato-tf-0.0.4/gato/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-26 18:26:51.000000 gato-tf-0.0.4/gato/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:10.819619 gato-tf-0.0.4/gato/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     4856 2023-05-26 18:26:51.000000 gato-tf-0.0.4/gato/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-05-26 18:26:51.000000 gato-tf-0.0.4/gato/models/embedding.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-26 18:26:51.000000 gato-tf-0.0.4/gato/models/tokenizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2837 2023-05-26 18:26:51.000000 gato-tf-0.0.4/gato/models/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:27:10.823619 gato-tf-0.0.4/gato_tf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8443 2023-05-26 18:27:10.000000 gato-tf-0.0.4/gato_tf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-05-26 18:27:10.000000 gato-tf-0.0.4/gato_tf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:27:10.000000 gato-tf-0.0.4/gato_tf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 18:27:10.000000 gato-tf-0.0.4/gato_tf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-26 18:27:10.000000 gato-tf-0.0.4/gato_tf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 18:27:10.823619 gato-tf-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-26 18:26:51.000000 gato-tf-0.0.4/setup.py
```

### Comparing `gato-tf-0.0.2/LICENSE` & `gato-tf-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `gato-tf-0.0.2/README.md` & `gato-tf-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `gato-tf-0.0.2/gato/config.py` & `gato-tf-0.0.4/gato/config.py`

 * *Files identical despite different names*

### Comparing `gato-tf-0.0.2/gato/models/__init__.py` & `gato-tf-0.0.4/gato/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,23 +32,23 @@
         # 0 - image
         # 1 - continuous
         # 2 - discrete (actions, texts)
         encoding = tf.one_hot(encoding, depth=3, dtype=tf.float32)
 
         ones = tf.ones((input_ids.shape[0], 1, self.config.layer_width), dtype=tf.float32)
         image_embed = self.image_embedding((input_ids, (row_pos, col_pos)), training=training)
-        image_embed *= tf.matmul(encoding[..., 0], ones, transpose_a=True)  # image patch masking
+        image_embed *= encoding[..., 0].transpose().matmul(ones)  # image patch masking
 
         # continuous value takes from first value of input_ids
         continuous_embed = self.continuous_encoding(input_ids[..., 0])
         continuous_embed = self.discrete_embedding(continuous_embed)
-        continuous_embed *= tf.matmul(encoding[..., 1], ones, transpose_a=True)  # continuous value masking
+        continuous_embed *= encoding[..., 1].transpose().matmul(ones)  # continuous value masking
 
         discrete_embed = self.discrete_embedding(input_ids[..., 0])
-        discrete_embed *= tf.matmul(encoding[..., 2], ones, transpose_a=True)  # discrete value masking
+        discrete_embed *= encoding[..., 2].transpose().matmul(ones)  # discrete value masking
 
         # Appendix C.3. Position Encodings > Local Observation Position Encodings
         # add local observation position encodings
         embed = image_embed + continuous_embed + discrete_embed
         embed += self.local_pos_encoding((obs_pos, obs_mask))
 
         hidden_states = self.transformer(embed)
@@ -97,14 +97,14 @@
         self.pos_encoding = PatchPositionEncoding(config, trainable=trainable, name='PatchPositionEncoding')
 
     def call(self, inputs, training=None, mask=None):
         input_ids, (row_pos, col_pos) = inputs
         patch_size = self.config.img_patch_size
         depth = self.config.input_dim // (patch_size * patch_size)
 
-        x = tf.reshape(input_ids, (-1, input_ids.shape[1], patch_size, patch_size, depth))
+        x = input_ids.reshape((-1, input_ids.shape[1], patch_size, patch_size, depth))
         x = self.residual_embedding(x)
         x = self.pos_encoding((x, (row_pos, col_pos)))
         return x
 
     def get_config(self):
         return super(PatchEmbedding, self).get_config()
```

### Comparing `gato-tf-0.0.2/gato/models/embedding.py` & `gato-tf-0.0.4/gato/models/embedding.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,40 +3,21 @@
 from tensorflow.keras import layers, models
 from gato import GatoConfig
 from typing import Dict, Any, Union
 
 
 def _randomized_positions(from_v, to_v):
     pos = tf.random.uniform(from_v.shape, minval=0, maxval=1, dtype=tf.float32)
-    pos = pos * tf.cast(to_v - from_v, dtype=tf.float32)
-    pos = tf.cast(pos, dtype=tf.int32)
-    return pos
+    pos = pos * (to_v - from_v).cast(tf.float32)
+    return pos.cast(tf.int32)
 
 
 def _rounded_mean_positions(from_v, to_v):
-    pos = tf.cast(from_v + to_v, tf.float32)
-    pos = pos / 2
-    pos = tf.round(pos)
-    return pos
-
-
-def _broadcast(row_pos, col_pos, row_ones, col_ones):
-    # broadcast (5,) to (20,) with column-axis
-    row_pos = tf.expand_dims(row_pos, 1)
-    row_pos = tf.matmul(row_pos, col_ones, transpose_b=True)
-    row_pos = tf.reshape(row_pos, (-1,))
-    row_pos = tf.stop_gradient(row_pos)
-
-    # broadcast (4,) to (20,) with row-axis
-    col_pos = tf.expand_dims(col_pos, 1)
-    col_pos = tf.matmul(row_ones, col_pos, transpose_b=True)
-    col_pos = tf.reshape(col_pos, (-1,))
-    col_pos = tf.stop_gradient(col_pos)
-
-    return row_pos, col_pos
+    pos = (from_v + to_v).cast(tf.float32) / 2.
+    return pos.round()
 
 
 class PatchPositionEncoding(layers.Layer):
 
     def __init__(self,
                  config: Union[GatoConfig, Dict[str, Any]],
                  trainable=True, name=None, *args, **kwargs):
@@ -53,15 +34,15 @@
         self.discretize_depth = self.config.discretize_depth
         self.patch_size = self.config.img_patch_size
 
         self.row_embedding = layers.Embedding(self.discretize_depth, self.embedding_dim, name='row_embedding')
         self.col_embedding = layers.Embedding(self.discretize_depth, self.embedding_dim, name='col_embedding')
 
     def _discretize(self, pos):
-        return tf.round(pos * self.discretize_depth)
+        return (pos * self.discretize_depth).round()
 
     def _discretize_interval(self, interval):
         pos_from, pos_to = interval
         return self._discretize(pos_from), self._discretize(pos_to)
 
     def call(self, inputs, *args, **kwargs):
         # Appendix C.3. Position Encodings; Figure 15 | Patch position encodings.
@@ -79,20 +60,17 @@
             row_pos = row_pos_from + _randomized_positions(row_pos_from, row_pos_to)
             col_pos = col_pos_from + _randomized_positions(col_pos_from, col_pos_to)
         else:
             # > During evaluation we deterministically take the (rounded) mean of the interval.
             row_pos = _rounded_mean_positions(row_pos_from, row_pos_to)
             col_pos = _rounded_mean_positions(col_pos_from, col_pos_to)
 
-        col_pos = tf.cast(col_pos, dtype=tf.int32)
-        row_pos = tf.cast(row_pos, dtype=tf.int32)
-
         # > Once row and column position encoding are retrieved from the embedding table,
         # > they are added onto the token embedding produced by the resnet embedding function.
-        return input_ids + self.row_embedding(row_pos) + self.col_embedding(col_pos)
+        return input_ids + self.row_embedding(row_pos.cast(tf.int32)) + self.col_embedding(col_pos.cast(tf.int32))
 
     def get_config(self):
         config = super(PatchPositionEncoding, self).get_config()
         config.update({
             'config': self.config.to_dict(),
         })
         return config
@@ -123,18 +101,18 @@
         # Supplementary Material B. Agent Data Tokenization Details; Figure 16
         # > This block uses the v2 ResNet architecture, GroupNorm (instead of LayerNorm) normalization,
         # > and GELU (instead RELU) activation functions.
         x = inputs
 
         residual = self.conv_proj(self.gn_proj(x))
 
-        x = tf.nn.gelu(self.gn1(x))
+        x = self.gn1(x).gelu()
         x = self.conv1(x)
 
-        x = tf.nn.gelu(self.gn2(x))
+        x = self.gn2(x).gelu()
         x = self.conv2(x)
 
         return x + residual
 
 
 class ResidualEmbedding(layers.Layer):
 
@@ -181,15 +159,15 @@
         # I don't think that transforming single 16x16 patch into feature map
         # with depth 768 at once does not give advantages coming from inductive bias.
         # This is currently discussing in issue #2
         for block in self.residual_units:
             x = block(x)
         if self.conv_proj is not None:
             x = self.conv_proj(x)
-        x = tf.reshape(x, shape=(-1, inputs.shape[1], self.config.layer_width))
+        x = x.reshape((-1, inputs.shape[1], self.config.layer_width))
         return x
 
     def get_config(self):
         config = super(ResidualEmbedding, self).get_config()
         config.update({
             'config': self.config.to_dict()
         })
@@ -218,16 +196,15 @@
         # > Note that no position encodings are added to action tokens.
 
         # So I added `obs_mask` to mask the action token into zeros.
         obs_pos, obs_mask = inputs
         embed = self.embedding(obs_pos)
 
         ones = tf.ones((embed.shape[0], 1, self.config.layer_width), dtype=tf.float32)
-        obs_mask = tf.cast(obs_mask, dtype=tf.float32)
-        obs_mask = tf.matmul(obs_mask, ones, transpose_a=True)
+        obs_mask = obs_mask.cast(tf.float32).transpose().matmul(ones)
         return embed * obs_mask
 
     def get_config(self):
         config = super(LocalPositionEncoding, self).get_config()
         config.update({
             'config': self.config.to_dict()
         })
```

### Comparing `gato-tf-0.0.2/gato/models/tokenizers.py` & `gato-tf-0.0.4/gato/models/tokenizers.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,29 +3,28 @@
 from gato import GatoConfig
 from tensorflow.keras import models
 from typing import Union, Dict, Any
 
 
 def mu_law_encode(x, mu=100, m=256):
     # Appendix B. Agent Data Tokenization Details
-    sign = tf.math.sign(x)
-    numerator = tf.math.log(tf.abs(x) * mu + 1.0)
+    numerator = tf.math.log(x.abs() * mu + 1.0)
     denominator = tf.math.log(m * mu + 1.0)
-    return (numerator / denominator) * sign
+    return (numerator / denominator) * x.sign()
 
 
 def tokenize_continuous_values(x, mu=100, m=256, bins=1024, shift=None):
     # Appendix B. Agent Data Tokenization Details
     # > Finally, they are discretized using bins of uniform width on the domain [-1, 1].
     c = mu_law_encode(x, mu, m)
 
     # > We use 1024 bins and shift the resulting integers
     # > so they are not overlapping with the ones used for text tokens.
     c = (c + 1) * (bins / 2)
-    c = tf.cast(c, tf.int32)
+    c = c.cast(tf.int32)
     if shift is not None:
         c += shift
     return c
 
 
 class ContinuousValueTokenizer(models.Model):
```

### Comparing `gato-tf-0.0.2/gato/models/transformer.py` & `gato-tf-0.0.4/gato/models/transformer.py`

 * *Files identical despite different names*

