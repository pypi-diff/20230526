# Comparing `tmp/connex-0.1.4.tar.gz` & `tmp/connex-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connex-0.1.4.tar", last modified: Sat Jul  9 17:00:41 2022, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `connex-0.1.4.tar` & `connex-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,13 @@
-drwxr-xr-x   0 leonardgleyzer   (501) staff       (20)        0 2022-07-09 17:00:41.573961 connex-0.1.4/
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)    11356 2022-06-12 20:49:13.000000 connex-0.1.4/LICENSE
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     4613 2022-07-09 17:00:41.573618 connex-0.1.4/PKG-INFO
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     3594 2022-07-09 16:42:50.000000 connex-0.1.4/README.md
-drwxr-xr-x   0 leonardgleyzer   (501) staff       (20)        0 2022-07-09 17:00:41.569751 connex-0.1.4/connex/
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)      207 2022-07-09 16:25:51.000000 connex-0.1.4/connex/__init__.py
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     1632 2022-06-11 22:06:14.000000 connex-0.1.4/connex/custom_types.py
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)    15612 2022-07-09 16:55:17.000000 connex-0.1.4/connex/network.py
-drwxr-xr-x   0 leonardgleyzer   (501) staff       (20)        0 2022-07-09 17:00:41.573155 connex-0.1.4/connex/nn/
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)       45 2022-06-10 01:08:26.000000 connex-0.1.4/connex/nn/__init__.py
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     2862 2022-07-04 00:22:44.000000 connex-0.1.4/connex/nn/mcmlp.py
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     2476 2022-07-04 00:22:32.000000 connex-0.1.4/connex/nn/mlp.py
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)    19844 2022-07-04 00:17:21.000000 connex-0.1.4/connex/plasticity.py
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     4073 2022-07-09 16:10:05.000000 connex-0.1.4/connex/test.py
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     1290 2022-07-09 16:46:55.000000 connex-0.1.4/connex/utils.py
-drwxr-xr-x   0 leonardgleyzer   (501) staff       (20)        0 2022-07-09 17:00:41.572245 connex-0.1.4/connex.egg-info/
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     4613 2022-07-09 17:00:40.000000 connex-0.1.4/connex.egg-info/PKG-INFO
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)      374 2022-07-09 17:00:41.000000 connex-0.1.4/connex.egg-info/SOURCES.txt
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)        1 2022-07-09 17:00:41.000000 connex-0.1.4/connex.egg-info/dependency_links.txt
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)        1 2022-06-13 21:39:08.000000 connex-0.1.4/connex.egg-info/not-zip-safe
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)       53 2022-07-09 17:00:41.000000 connex-0.1.4/connex.egg-info/requires.txt
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)        7 2022-07-09 17:00:41.000000 connex-0.1.4/connex.egg-info/top_level.txt
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)       38 2022-07-09 17:00:41.574064 connex-0.1.4/setup.cfg
--rw-r--r--   0 leonardgleyzer   (501) staff       (20)     1826 2022-07-09 16:29:19.000000 connex-0.1.4/setup.py
+-rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 connex-0.2.0/connex/__init__.py
+-rw-r--r--   0        0        0    35120 2020-02-02 00:00:00.000000 connex-0.2.0/connex/_network.py
+-rw-r--r--   0        0        0    44763 2020-02-02 00:00:00.000000 connex-0.2.0/connex/_plasticity.py
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 connex-0.2.0/connex/_utils.py
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 connex-0.2.0/connex/nn/__init__.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 connex-0.2.0/connex/nn/_dense_mlp.py
+-rw-r--r--   0        0        0     2526 2020-02-02 00:00:00.000000 connex-0.2.0/connex/nn/_mlp.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 connex-0.2.0/connex/nn/_utils.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 connex-0.2.0/.gitignore
+-rw-r--r--   0        0        0    11356 2020-02-02 00:00:00.000000 connex-0.2.0/LICENSE
+-rw-r--r--   0        0        0     3766 2020-02-02 00:00:00.000000 connex-0.2.0/README.md
+-rw-r--r--   0        0        0     1119 2020-02-02 00:00:00.000000 connex-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    17767 2020-02-02 00:00:00.000000 connex-0.2.0/PKG-INFO
```

### Comparing `connex-0.1.4/LICENSE` & `connex-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connex-0.1.4/PKG-INFO` & `connex-0.2.0/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,37 @@
-Metadata-Version: 2.1
-Name: connex
-Version: 0.1.4
-Summary: Making neural networks more neural.
-Home-page: https://github.com/leonard-gleyzer/connex
-Author: Leonard Gleyzer
-Author-email: leonard_gleyzer@brown.edu
-Maintainer: Leonard Gleyzer
-Maintainer-email: leonard_gleyzer@brown.edu
-License: Apache-2.0
-Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Intended Audience :: Information Technology
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Requires-Python: ~=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <h1 align='center'>Connex</h1>
 
+Connex is a [JAX](https://github.com/google/jax) library built on [Equinox](https://github.com/patrick-kidger/equinox) that allows for fine-grained, dynamic control of neural network topology. With Connex, you can
 
-Connex is a small [JAX](https://github.com/google/jax) library built on [Equinox](https://github.com/patrick-kidger/equinox) whose aim is to incorporate artificial analogues of biological neural network attributes into deep learning research and architecture design. Currently, this includes:
-
-- **Complex Connectivity**: Turn any directed acyclic graph (DAG) into a trainable neural network.
-- **Plasticity**: Add and remove both connections and neurons at the individual level.
-- **Firing Modulation**: Set and modify dropout probabilities for all neurons individually.
+- Turn any directed acyclic graph (DAG) into a trainable neural network.
+- Add and remove both connections and neurons at the individual level.
+- Set and modify dropout probabilities for all neurons individually.
+- Easily toggle techniques such as normalization, adaptive activations, and self-attention.
+- Export a trained network to a NetworkX weighted digraph for network analysis.
 
 ## Installation
 
 ```bash
 pip install connex
 ```
 
-## Documentation
-
-Available at [https://leonard-gleyzer.github.io/connex/](https://leonard-gleyzer.github.io/connex/).
-
 ## Usage
 
-As a small example, let's create a trainable neural network from the following DAG 
+As a tiny pedagogical example, let's create a trainable neural network from the following DAG
 
-![dag](https://www.mdpi.com/algorithms/algorithms-13-00256/article_deploy/html/images/algorithms-13-00256-g001.png)
+![dag](docs/imgs/dag.png)
 
-with input neuron 0 and output neurons 3 and 11 (in that order), with a ReLU activation function for the hidden neurons:
+with input neuron 0 and output neurons 3 and 11 (in that order) and ReLU activation for the hidden neurons:
 
 ```python
 import connex as cnx
 import jax.nn as jnn
 
-# Specify number of neurons
-num_neurons = 12
 
-# Build the adjacency dict
+# Create the graph data
 adjacency_dict = {
     0: [1, 2, 3],
     1: [4],
     2: [4, 5],
     4: [6],
     5: [7],
     6: [8, 9],
@@ -74,70 +43,83 @@
 
 # Specify the input and output neurons
 input_neurons = [0]
 output_neurons = [3, 11]
 
 # Create the network
 network = cnx.NeuralNetwork(
-    num_neurons,
-    adjacency_dict, 
+    adjacency_dict,
     input_neurons, 
     output_neurons,
     jnn.relu
 )
 ```
 
 That's it! A `connex.NeuralNetwork` is a subclass of `equinox.Module`, so it can be trained in the same fashion:
 
 ```python
 import equinox as eqx
 import jax
 import jax.numpy as jnp
+import jax.random as jr
 import optax
 
 # Initialize the optimizer
 optim = optax.adam(1e-3)
 opt_state = optim.init(eqx.filter(network, eqx.is_array))
 
 # Define the loss function
 @eqx.filter_value_and_grad
-def loss_fn(model, x, y):
-    preds = jax.vmap(model)(x)
+def loss_fn(model, x, y, keys):
+    preds = jax.vmap(model)(x, keys)
     return jnp.mean((preds - y) ** 2)
 
 # Define a single training step
 @eqx.filter_jit
-def step(model, opt_state, x, y):
-    loss, grads = loss_fn(model, x, y)
+def step(model, opt_state, x, y, keys):
+    loss, grads = loss_fn(model, x, y, keys)
     updates, opt_state = optim.update(grads, opt_state, model)
     model = eqx.apply_updates(model, updates)
     return model, opt_state, loss
 
 # Toy data
 x = jnp.expand_dims(jnp.linspace(0, 2 * jnp.pi, 250), 1)
 y = jnp.hstack((jnp.cos(x), jnp.sin(x)))
 
 # Training loop
-n_epochs = 1000
-for _ in range(n_epochs):
-    network, opt_state, loss = step(network, opt_state, x, y)
+n_epochs = 500
+key = jr.PRNGKey(0)
+for epoch in range(n_epochs):
+    *keys, key = jr.split(key, x.shape[0] + 1)
+    keys = jnp.array(keys)
+    network, opt_state, loss = step(network, opt_state, x, y, keys)
+    print(f"Epoch: {epoch + 1}   Loss: {loss}")
 ```
 
 Now suppose we wish to add connections 1 &rarr; 6 and 2 &rarr; 11, remove neuron 9, and set the dropout probability of all hidden neurons to 0.1:
 
 ```python
 # Add connections
 network = cnx.add_connections(network, [(1, 6), (2, 11)])
 
 # Remove neuron
-network, _ = cnx.remove_neurons(network, [9])
+network = cnx.remove_neurons(network, [9])
 
 # Set dropout probability
 network.set_dropout_p(0.1)
 ```
 
 That's all there is to it.  The new connections have been initialized with untrained parameters, and the neurons in the original network that have not been removed (along with their respective incoming and outgoing connections) have retained their trained parameters. Furthermore, since a `connex.NeuralNetwork` is an `equinox.Module`, it can seamlessly be used as a submodule inside other Equinox Modules.
 
 For more information about manipulating connectivity structure and the `NeuralNetwork` base class, please see the API section of the documentation. For examples of subclassing `NeuralNetwork`, please see `connex.nn`.
 
-Feedback is greatly appeciated!
+## Citation
 
+```bibtex
+@software{gleyzer2023connex,
+  author = {Leonard Gleyzer},
+  title = {{C}onnex: Fine-grained Control over Neural Network Topology in {JAX}},
+  url = {http://github.com/leonard-gleyzer/connex},
+  version = {0.2.0},
+  year = {2023},
+}
+```
```

### Comparing `connex-0.1.4/connex/nn/mcmlp.py` & `connex-0.2.0/connex/nn/_mlp.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,74 +1,69 @@
 from typing import Callable, Optional
 
-import jax.numpy as jnp
 import jax.nn as jnn
 import jax.random as jr
+import numpy as np
 
-from .. import NeuralNetwork
-from ..utils import _identity
+from .._network import NeuralNetwork
+from ._utils import _identity
 
 
-class MCMLP(NeuralNetwork):
+class MLP(NeuralNetwork):
     """
-    A "Maximally-Connected Multi-Layer Perceptron". Like a standard MLP, but
-    every neuron is connected to every other neuron in all later layers, rather
-    than only the next layer.
+    A standard Multi-Layer Perceptron with constant layer width.
     """
 
     def __init__(
         self,
         input_size: int,
         output_size: int,
         width: int,
         depth: int,
         hidden_activation: Callable = jnn.silu,
-        output_activation_elem: Callable = _identity,
-        output_activation_group: Callable = _identity,
+        output_transformation: Callable = _identity,
         *,
         key: Optional[jr.PRNGKey] = None,
         **kwargs,
     ):
         """**Arguments**:
 
-        - `input_size`: The number of neurons in the input layer.
-        - `output_size`: The number of neurons in the output layer.
-        - `width`: The number of neurons in each hidden layer.
-        - `depth`: The number of hidden layers.
-        - `hidden_activation`: The activation function applied element-wise to the 
-            hidden (i.e. non-input, non-output) neurons. It can itself be a 
-            trainable equinox Module.
-        - `output_activation_elem`: The activation function applied element-wise to 
-            the  output neurons. It can itself be a trainable `equinox.Module`.
-        - `output_activation_group`: The activation function applied to the output 
-            neurons as a whole after applying `output_activation_elem` element-wise, 
-            e.g. `jax.nn.softmax`. It can itself be a trainable `equinox.Module`.
-            the  output neurons. It can itself be a trainable equinox Module.
-        - `key`: The `PRNGKey` used to initialize parameters. Optional, keyword-only 
-            argument. Defaults to `jax.random.PRNGKey(0)`.
+         - `input_size`: The number of neurons in the input layer.
+         - `output_size`: The number of neurons in the output layer.
+         - `width`: The number of neurons in each hidden layer.
+         - `depth`: The number of hidden layers.
+         - `hidden_activation`: The activation function applied element-wise to
+            the hidden (i.e. non-input, non-output) neurons. It can itself be a
+            trainable `equinox Module`.
+        - `output_transformation`: The transformation applied group-wise to the
+            output neurons, e.g. `jax.nn.softmax`. It can itself be a trainable
+            `equinox.Module`.
+         - `key`: The `PRNGKey` used to initialize parameters. Optional, keyword-only
+             argument. Defaults to `jax.random.PRNGKey(0)`.
         """
         key = key if key is not None else jr.PRNGKey(0)
         num_neurons = width * depth + input_size + output_size
-        input_neurons = jnp.arange(input_size)
+        input_neurons = np.arange(input_size, dtype=int)
         output_neurons_start = num_neurons - output_size
-        output_neurons = jnp.arange(output_size) + output_neurons_start
+        output_neurons = np.arange(output_size, dtype=int) + output_neurons_start
         adjacency_dict = {}
         layer_sizes = [input_size] + ([width] * depth) + [output_size]
         neuron = 0
-        for layer_size in layer_sizes[:-1]:
-            row_idx = range(neuron, neuron + layer_size)
-            col_idx = range(neuron + layer_size, num_neurons)
+        for layer_size in range(len(layer_sizes) - 1):
+            in_size, out_size = layer_sizes[layer_size], layer_sizes[layer_size + 1]
+            row_idx = range(neuron, neuron + in_size)
+            col_idx = range(neuron + in_size, neuron + in_size + out_size)
             for r in row_idx:
                 adjacency_dict[r] = list(col_idx)
-            neuron += layer_size
+            neuron += in_size
+        topo_sort = list(range(num_neurons))
 
         super().__init__(
-            num_neurons,
             adjacency_dict,
             input_neurons,
             output_neurons,
             hidden_activation,
-            output_activation_elem,
-            output_activation_group,
+            output_transformation,
+            topo_sort=topo_sort,
             key=key,
-            **kwargs
-        )
+            **kwargs,
+        )
```

