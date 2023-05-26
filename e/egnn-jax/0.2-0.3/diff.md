# Comparing `tmp/egnn_jax-0.2.tar.gz` & `tmp/egnn_jax-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "egnn_jax-0.2.tar", last modified: Fri Mar 31 18:11:52 2023, max compression
+gzip compressed data, was "egnn_jax-0.3.tar", last modified: Fri May 26 14:18:01 2023, max compression
```

## Comparing `egnn_jax-0.2.tar` & `egnn_jax-0.3.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:11:52.090698 egnn_jax-0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-03-31 18:11:41.000000 egnn_jax-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-31 18:11:52.090698 egnn_jax-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-03-31 18:11:41.000000 egnn_jax-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:11:52.090698 egnn_jax-0.2/egnn_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-31 18:11:41.000000 egnn_jax-0.2/egnn_jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-03-31 18:11:41.000000 egnn_jax-0.2/egnn_jax/egnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-03-31 18:11:41.000000 egnn_jax-0.2/egnn_jax/variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-31 18:11:52.090698 egnn_jax-0.2/egnn_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-03-31 18:11:52.000000 egnn_jax-0.2/egnn_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-03-31 18:11:52.000000 egnn_jax-0.2/egnn_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-31 18:11:52.000000 egnn_jax-0.2/egnn_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-31 18:11:52.000000 egnn_jax-0.2/egnn_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-31 18:11:52.000000 egnn_jax-0.2/egnn_jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-03-31 18:11:41.000000 egnn_jax-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-03-31 18:11:52.094698 egnn_jax-0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-03-31 18:11:41.000000 egnn_jax-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:01.577509 egnn_jax-0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-26 14:17:52.000000 egnn_jax-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-26 14:18:01.577509 egnn_jax-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-05-26 14:17:52.000000 egnn_jax-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:01.573509 egnn_jax-0.3/egnn_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 14:17:52.000000 egnn_jax-0.3/egnn_jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8414 2023-05-26 14:17:52.000000 egnn_jax-0.3/egnn_jax/egnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-26 14:17:52.000000 egnn_jax-0.3/egnn_jax/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-26 14:17:52.000000 egnn_jax-0.3/egnn_jax/variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 14:18:01.577509 egnn_jax-0.3/egnn_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-05-26 14:18:01.000000 egnn_jax-0.3/egnn_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-26 14:18:01.000000 egnn_jax-0.3/egnn_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 14:18:01.000000 egnn_jax-0.3/egnn_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-26 14:18:01.000000 egnn_jax-0.3/egnn_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 14:18:01.000000 egnn_jax-0.3/egnn_jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-26 14:17:52.000000 egnn_jax-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 14:18:01.577509 egnn_jax-0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 14:17:52.000000 egnn_jax-0.3/setup.py
```

### Comparing `egnn_jax-0.2/LICENSE` & `egnn_jax-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `egnn_jax-0.2/PKG-INFO` & `egnn_jax-0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,53 @@
-Metadata-Version: 2.1
-Name: egnn_jax
-Version: 0.2
-Summary: E(3) GNN in jax
-Author: Gianluca Galletti
-Author-email: g.galletti@tum.de
-Classifier: Programming Language :: Python :: 3.8
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # E(n) Equivariant GNN in jax
 Reimplementation of [EGNN](https://arxiv.org/abs/2102.09844) in jax. Original work by Victor Garcia Satorras, Emiel Hogeboom and Max Welling.
 
 ## Installation
 ```
 python -m pip install egnn-jax
 ```
 
 Or clone this repository and build locally
 ```
+git clone https://github.com/gerkone/egnn-jax
+cd painn-jax
 python -m pip install -e .
 ```
-
 ### GPU support
 Upgrade `jax` to the gpu version
 ```
-pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade "jax[cuda]==0.4.10" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Validation
 N-body (charged) is included for validation from the original paper. Times are  __model only__ on batches of 100 graphs, in (global) single precision.
 |                  |  MSE  | Inference [ms]* |
 |------------------|-------|-----------------|
 | torch (original) | .0071 |      8.27       |
-| jax (ours)       | .011  |      0.94       |
+| jax (ours)       | .0093 |      0.94       |
 
 \* remeasured (Quadro RTX 4000)
 
 ### Validation install
 
 The N-Body experiments are only included in the github repo, so it needs to be cloned first.
 ```
 git clone https://github.com/gerkone/egnn-jax
 ```
 
 They are adapted from the original implementation, so additionally `torch` and `torch_geometric` are needed (cpu versions are enough).
 ```
-pip3 install torch==1.12.1 --extra-index-url https://download.pytorch.org/whl/cpu
 python -m pip install -r nbody/requirements.txt
 ```
 
 ### Valdation usage
 The charged N-body dataset has to be locally generated in the directory [/nbody/data](/nbody/data).
 ```
-python3 -u generate_dataset.py --num-train=3000
+python -u generate_dataset.py --num-train 3000 --seed 43 --sufix small
 ```
-Then, the model can be trained and evaluated (from the repo root) with
+Then, the model can be trained and evaluated with
 ```
-python main.py --epochs=500 --batch-size=100 --lr=1e-4 --weight-decay=1e-8
+python validate.py --epochs=1000 --batch-size=100 --lr=1e-4 --weight-decay=1e-12
 ```
 
 ## Acknowledgements
 This implementation heavily borrows from the [original pytorch code](https://github.com/vgsatorras/egnn).
```

### Comparing `egnn_jax-0.2/egnn_jax/egnn.py` & `egnn_jax-0.3/egnn_jax/egnn.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,81 +2,100 @@
 
 import haiku as hk
 import jax
 import jax.numpy as jnp
 import jraph
 from jax.tree_util import Partial
 
+from egnn_jax.utils import LinearXav, MLPXav
+
 
 class EGNNLayer(hk.Module):
-    """EGNN layer."""
+    """EGNN layer.
+
+    Args:
+        layer_num: layer number
+        hidden_size: hidden size
+        output_size: output size
+        blocks: number of blocks in the node and edge MLPs
+        act_fn: activation function
+        pos_aggregate_fn: position aggregation function
+        msg_aggregate_fn: message aggregation function
+        residual: whether to use residual connections
+        attention: whether to use attention
+        normalize: whether to normalize the coordinates
+        tanh: whether to use tanh in the position update
+        dt: position update step size
+        eps: small number to avoid division by zero
+    """
 
     def __init__(
         self,
         layer_num: int,
         hidden_size: int,
         output_size: int,
         blocks: int = 1,
         act_fn: Callable = jax.nn.silu,
         pos_aggregate_fn: Optional[Callable] = jraph.segment_sum,
         msg_aggregate_fn: Optional[Callable] = jraph.segment_sum,
         residual: bool = True,
         attention: bool = False,
         normalize: bool = False,
         tanh: bool = False,
+        dt: float = 0.001,
         eps: float = 1e-8,
     ):
         super().__init__(f"layer_{layer_num}")
 
         # message network
-        self._edge_mlp = hk.nets.MLP(
+        self._edge_mlp = MLPXav(
             [hidden_size] * blocks + [hidden_size],
             activation=act_fn,
             activate_final=True,
         )
 
         # update network
-        self._node_mlp = hk.nets.MLP(
+        self._node_mlp = MLPXav(
             [hidden_size] * blocks + [output_size],
             activation=act_fn,
             activate_final=False,
         )
 
         # position update network
-        net = [hk.Linear(hidden_size)] * blocks
+        net = [LinearXav(hidden_size)] * blocks
         # NOTE: from https://github.com/vgsatorras/egnn/blob/main/models/gcl.py#L254
-        a = 0.001 * jnp.sqrt(6 / hidden_size)
+        a = dt * jnp.sqrt(6 / hidden_size)
         net += [
             act_fn,
-            hk.Linear(1, with_bias=False, w_init=hk.initializers.TruncatedNormal(a)),
+            LinearXav(1, with_bias=False, w_init=hk.initializers.UniformScaling(a)),
         ]
         if tanh:
             net.append(jax.nn.tanh)
-        self._pos_mlp = hk.Sequential(net)
+        self._pos_correction_mlp = hk.Sequential(net)
 
         # attention
         self._attention_mlp = None
         if attention:
             self._attention_mlp = hk.Sequential(
-                [hk.Linear(hidden_size), jax.nn.sigmoid]
+                [LinearXav(hidden_size), jax.nn.sigmoid]
             )
 
         self.pos_aggregate_fn = pos_aggregate_fn
         self.msg_aggregate_fn = msg_aggregate_fn
         self._residual = residual
         self._normalize = normalize
         self._eps = eps
 
     def _pos_update(
         self,
         pos: jnp.ndarray,
         graph: jraph.GraphsTuple,
         coord_diff: jnp.ndarray,
     ) -> jnp.ndarray:
-        trans = coord_diff * self._pos_mlp(graph.edges)
+        trans = coord_diff * self._pos_correction_mlp(graph.edges)
         # NOTE: was in the original code
         trans = jnp.clip(trans, -100, 100)
         return self.pos_aggregate_fn(trans, graph.senders, num_segments=pos.shape[0])
 
     def _message(
         self,
         radial: jnp.ndarray,
@@ -179,16 +198,15 @@
             hidden_size: Number of hidden features
             output_size: Number of features for 'h' at the output
             act_fn: Non-linearity
             num_layers: Number of layer for the EGNN
             residual: Use residual connections, we recommend not changing this one
             attention: Whether using attention or not
             normalize: Normalizes the coordinates messages such that:
-                instead of: x^{l+1}_i = x^{l}_i + \sum(x_i - x_j)\phi_x(m_{ij})
-                use:        x^{l+1}_i = x^{l}_i + \sum(x_i - x_j)\phi_x(m_{ij})\|x_i - x_j\|
+                x^{l+1}_i = x^{l}_i + \sum(x_i - x_j)\phi_x(m_{ij})\|x_i - x_j\|
                 It may help in the stability or generalization. Not used in the paper.
             tanh: Sets a tanh activation function at the output of \phi_x(m_{ij}). It
                 bounds the output of \phi_x(m_{ij}) which definitely improves in
                 stability but it may decrease in accuracy. Not used in the paper.
         """
         super().__init__()
 
@@ -217,24 +235,24 @@
             edge_attribute: Edge attribute (optional)
             node_attribute: Node attribute (optional)
 
         Returns:
             Tuple of updated node features and positions
         """
         # input node embedding
-        h = hk.Linear(self._hidden_size, name="embedding")(graph.nodes)
+        h = LinearXav(self._hidden_size, name="embedding")(graph.nodes)
         graph = graph._replace(nodes=h)
         # message passing
         for n in range(self._num_layers):
             graph, pos = EGNNLayer(
                 layer_num=n,
                 hidden_size=self._hidden_size,
                 output_size=self._hidden_size,
                 act_fn=self._act_fn,
                 residual=self._residual,
                 attention=self._attention,
                 normalize=self._normalize,
                 tanh=self._tanh,
             )(graph, pos, edge_attribute=edge_attribute, node_attribute=node_attribute)
         # node readout
-        h = hk.Linear(self._output_size, name="readout")(graph.nodes)
+        h = LinearXav(self._output_size, name="readout")(graph.nodes)
         return h, pos
```

### Comparing `egnn_jax-0.2/egnn_jax.egg-info/PKG-INFO` & `egnn_jax-0.3/egnn_jax.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: egnn-jax
-Version: 0.2
+Version: 0.3
 Summary: E(3) GNN in jax
 Author: Gianluca Galletti
 Author-email: g.galletti@tum.de
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -15,50 +15,50 @@
 ## Installation
 ```
 python -m pip install egnn-jax
 ```
 
 Or clone this repository and build locally
 ```
+git clone https://github.com/gerkone/egnn-jax
+cd painn-jax
 python -m pip install -e .
 ```
-
 ### GPU support
 Upgrade `jax` to the gpu version
 ```
-pip install --upgrade "jax[cuda]==0.4.8" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
+pip install --upgrade "jax[cuda]==0.4.10" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
 ```
 
 ## Validation
 N-body (charged) is included for validation from the original paper. Times are  __model only__ on batches of 100 graphs, in (global) single precision.
 |                  |  MSE  | Inference [ms]* |
 |------------------|-------|-----------------|
 | torch (original) | .0071 |      8.27       |
-| jax (ours)       | .011  |      0.94       |
+| jax (ours)       | .0093 |      0.94       |
 
 \* remeasured (Quadro RTX 4000)
 
 ### Validation install
 
 The N-Body experiments are only included in the github repo, so it needs to be cloned first.
 ```
 git clone https://github.com/gerkone/egnn-jax
 ```
 
 They are adapted from the original implementation, so additionally `torch` and `torch_geometric` are needed (cpu versions are enough).
 ```
-pip3 install torch==1.12.1 --extra-index-url https://download.pytorch.org/whl/cpu
 python -m pip install -r nbody/requirements.txt
 ```
 
 ### Valdation usage
 The charged N-body dataset has to be locally generated in the directory [/nbody/data](/nbody/data).
 ```
-python3 -u generate_dataset.py --num-train=3000
+python -u generate_dataset.py --num-train 3000 --seed 43 --sufix small
 ```
-Then, the model can be trained and evaluated (from the repo root) with
+Then, the model can be trained and evaluated with
 ```
-python main.py --epochs=500 --batch-size=100 --lr=1e-4 --weight-decay=1e-8
+python validate.py --epochs=1000 --batch-size=100 --lr=1e-4 --weight-decay=1e-12
 ```
 
 ## Acknowledgements
 This implementation heavily borrows from the [original pytorch code](https://github.com/vgsatorras/egnn).
```

