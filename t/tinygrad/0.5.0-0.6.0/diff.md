# Comparing `tmp/tinygrad-0.5.0.tar.gz` & `tmp/tinygrad-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tinygrad-0.5.0.tar", last modified: Tue Mar  7 02:21:43 2023, max compression
+gzip compressed data, was "tinygrad-0.6.0.tar", last modified: Fri May 26 01:03:26 2023, max compression
```

## Comparing `tinygrad-0.5.0.tar` & `tinygrad-0.6.0.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 02:21:43.928278 tinygrad-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-03-07 02:21:34.000000 tinygrad-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-03-07 02:21:43.928278 tinygrad-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8060 2023-03-07 02:21:34.000000 tinygrad-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-07 02:21:43.928278 tinygrad-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-03-07 02:21:34.000000 tinygrad-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 02:21:43.924278 tinygrad-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     3326 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_conv_shapetracker.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_gc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_jit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_net_speed.py
--rw-r--r--   0 runner    (1001) docker     (123)     4555 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_nn.py
--rw-r--r--   0 runner    (1001) docker     (123)    25487 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_optim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_randomness.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_specific_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     8364 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_speed_v_torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-03-07 02:21:34.000000 tinygrad-0.5.0/test/test_tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 02:21:43.924278 tinygrad-0.5.0/tinygrad/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 02:21:43.924278 tinygrad-0.5.0/tinygrad/codegen/
--rw-r--r--   0 runner    (1001) docker     (123)    10041 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/codegen/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    20643 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/codegen/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/codegen/llvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/jit.py
--rw-r--r--   0 runner    (1001) docker     (123)    14867 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5717 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/mlops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 02:21:43.924278 tinygrad-0.5.0/tinygrad/nn/
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/nn/optim.py
--rw-r--r--   0 runner    (1001) docker     (123)    11999 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 02:21:43.928278 tinygrad-0.5.0/tinygrad/runtime/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/runtime/ops_clang.py
--rw-r--r--   0 runner    (1001) docker     (123)     2575 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/runtime/ops_cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/runtime/ops_cuda.py
--rw-r--r--   0 runner    (1001) docker     (123)     4694 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/runtime/ops_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/runtime/ops_llvm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4628 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/runtime/ops_metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/runtime/ops_torch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 02:21:43.928278 tinygrad-0.5.0/tinygrad/shape/
--rw-r--r--   0 runner    (1001) docker     (123)    10570 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/shape/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/shape/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    24487 2023-03-07 02:21:34.000000 tinygrad-0.5.0/tinygrad/tensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-07 02:21:43.924278 tinygrad-0.5.0/tinygrad.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8557 2023-03-07 02:21:43.000000 tinygrad-0.5.0/tinygrad.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-07 02:21:43.000000 tinygrad-0.5.0/tinygrad.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-07 02:21:43.000000 tinygrad-0.5.0/tinygrad.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-03-07 02:21:43.000000 tinygrad-0.5.0/tinygrad.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-07 02:21:43.000000 tinygrad-0.5.0/tinygrad.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:03:26.838467 tinygrad-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-26 01:03:11.000000 tinygrad-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-26 01:03:26.838467 tinygrad-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8068 2023-05-26 01:03:11.000000 tinygrad-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 01:03:26.838467 tinygrad-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1415 2023-05-26 01:03:11.000000 tinygrad-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:03:26.834466 tinygrad-0.6.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_conv_shapetracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_custom_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_dtype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_gc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_net_speed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5213 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_nn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30247 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_randomness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_specific_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8848 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_speed_v_torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-05-26 01:03:11.000000 tinygrad-0.6.0/test/test_tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:03:26.834466 tinygrad-0.6.0/tinygrad/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:03:26.834466 tinygrad-0.6.0/tinygrad/codegen/
+-rw-r--r--   0 runner    (1001) docker     (123)    11674 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/codegen/cstyle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26652 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/codegen/linearizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6113 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/codegen/llvmir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3090 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/jit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18742 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8125 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/mlops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:03:26.834466 tinygrad-0.6.0/tinygrad/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4690 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/nn/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/nn/optim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:03:26.834466 tinygrad-0.6.0/tinygrad/runtime/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/runtime/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/runtime/ops_clang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/runtime/ops_cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2660 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/runtime/ops_cuda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5097 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/runtime/ops_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2675 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/runtime/ops_llvm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4531 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/runtime/ops_metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/runtime/ops_torch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:03:26.834466 tinygrad-0.6.0/tinygrad/shape/
+-rw-r--r--   0 runner    (1001) docker     (123)    13256 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/shape/shapetracker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/shape/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28131 2023-05-26 01:03:11.000000 tinygrad-0.6.0/tinygrad/tensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:03:26.834466 tinygrad-0.6.0/tinygrad.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8542 2023-05-26 01:03:26.000000 tinygrad-0.6.0/tinygrad.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-26 01:03:26.000000 tinygrad-0.6.0/tinygrad.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:03:26.000000 tinygrad-0.6.0/tinygrad.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-26 01:03:26.000000 tinygrad-0.6.0/tinygrad.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-26 01:03:26.000000 tinygrad-0.6.0/tinygrad.egg-info/top_level.txt
```

### Comparing `tinygrad-0.5.0/LICENSE` & `tinygrad-0.6.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright (c) 2020 George Hotz
+Copyright (c) 2023 George Hotz
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `tinygrad-0.5.0/PKG-INFO` & `tinygrad-0.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tinygrad
-Version: 0.5.0
-Summary: You like pytorch? You like micrograd? You love tinygrad! heart
+Version: 0.6.0
+Summary: You like pytorch? You like micrograd? You love tinygrad! <3
 Author: George Hotz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: gpu
 Provides-Extra: llvm
 Provides-Extra: cuda
 Provides-Extra: triton
 Provides-Extra: metal
 Provides-Extra: linting
 Provides-Extra: testing
 License-File: LICENSE
@@ -38,14 +37,17 @@
 We are working on support for the Apple Neural Engine and the Google TPU in the `accel/` folder. Eventually, [we will build custom hardware](https://geohot.github.io/blog/jekyll/update/2021/06/13/a-breakdown-of-ai-chip-companies.html) for tinygrad, and it will be blindingly fast. Now, it is slow.
 
 This project is maintained by [tiny corp](https://tinygrad.org/).
 
 ### Installation
 
 ```bash
+python3 -m pip install git+https://git@github.com/geohot/tinygrad.git
+
+# or
 git clone https://github.com/geohot/tinygrad.git
 cd tinygrad
 python3 -m pip install -e .
 ```
 
 ### Contributing
 
@@ -86,27 +88,27 @@
 ```
 
 ## Is tinygrad fast?
 
 Try a matmul. See how, despite the style, it is fused into one kernel with the power of laziness.
 
 ```python
-DEBUG=3 OPTLOCAL=1 GPU=1 python3 -c "from tinygrad.tensor import Tensor;
+DEBUG=3 OPTLOCAL=1 python3 -c "from tinygrad.tensor import Tensor;
 N = 1024; a, b = Tensor.randn(N, N), Tensor.randn(N, N);
 c = (a.reshape(N, 1, N) * b.permute(1,0).reshape(1, N, N)).sum(axis=2);
 print((c.numpy() - (a.numpy() @ b.numpy())).mean())"
 ```
 
 Change to `DEBUG=4` to see the generated code.
 
 ## Neural networks?
 
-It turns out, a decent autograd tensor library is 90% of what you need for neural networks. Add an optimizer (SGD, RMSprop, and Adam implemented) from tinygrad.nn.optim, write some boilerplate minibatching code, and you have all you need.
+It turns out, a decent autograd tensor library is 90% of what you need for neural networks. Add an optimizer (SGD, Adam, AdamW implemented) from tinygrad.nn.optim, write some boilerplate minibatching code, and you have all you need.
 
-### Neural network example (from test/test_mnist.py)
+### Neural network example (from test/models/test_mnist.py)
 
 ```python
 from tinygrad.tensor import Tensor
 import tinygrad.nn.optim as optim
 
 class TinyBobNet:
   def __init__(self):
@@ -160,33 +162,33 @@
 hlops are syntactic sugar around mlops. They support most things torch does.
 
 ### mlops
 
 mlops are mid level ops. They understand derivatives. They are very simple.
 
 ```
-Log, Exp                                       # unary ops
+Relu, Log, Exp                                 # unary ops
 Sum, Max                                       # reduce ops (with axis argument)
 Maximum, Add, Sub, Mul, Pow, Div, Equal        # binary ops (no broadcasting, use expand)
 Expand, Reshape, Permute, Pad, Shrink, Flip    # movement ops
 ```
 
 You no longer need to write mlops for a new accelerator
 
 ### Adding an accelerator (llops)
 
 The autodiff stuff is all in mlops now so you can focus on the raw operations
 
 ```
-Buffer                                                     # class of memory on this device
-unary_op  (NOOP, NEG, NOT, EXP, LOG)                       # A -> A
-reduce_op (SUM, MAX)                                       # A -> B (smaller size, B has 1 in shape)
-binary_op (ADD, SUB, MUL, DIV, POW, CMPEQ, MAX)            # A + A -> A (all the same size)
-movement_op (EXPAND, RESHAPE, PERMUTE, PAD, SHRINK, FLIP)  # A -> B (different size)
-fused_op [[optional]] (MULACC)                             # A * A -> B
+Buffer                                                       # class of memory on this device
+unary_op  (NOOP, EXP, LOG, CAST)                             # A -> A
+reduce_op (SUM, MAX)                                         # A -> B (smaller size, B has 1 in shape)
+binary_op (ADD, SUB, MUL, DIV, POW, CMPEQ, MAX)              # A + A -> A (all the same size)
+movement_op (EXPAND, RESHAPE, PERMUTE, PAD, SHRINK, STRIDE)  # A -> B (different size)
+fused_op [[optional]] (MULACC)                               # A * A -> B
 ```
 
 ## ImageNet inference
 
 Despite being tiny, tinygrad supports the full EfficientNet. Pass in a picture to discover what it is.
 
 ```bash
@@ -195,23 +197,21 @@
 
 Or, if you have a webcam and cv2 installed
 
 ```bash
 ipython3 examples/efficientnet.py webcam
 ```
 
-PROTIP: Set "GPU=1" environment variable if you want this to go faster.
-
-PROPROTIP: Set "DEBUG=1" environment variable if you want to see why it's slow.
+PROTIP: Set "DEBUG=1" environment variable if you want to see why it's slow.
 
 ### tinygrad supports Stable Diffusion!
 
 You might need to download the [weight](https://huggingface.co/CompVis/stable-diffusion-v-1-4-original/resolve/main/sd-v1-4.ckpt) of Stable Diffusion and put it into weights/
 
-Run `GPU=1 python3 examples/stable_diffusion.py`
+Run `python3 examples/stable_diffusion.py`
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/geohot/tinygrad/master/docs/stable_diffusion_by_tinygrad.jpg">
 </p>
 
 <p align="center">
 "a horse sized cat eating a bagel"
@@ -242,15 +242,15 @@
 * Nodes are Tensors
 * Black edge is a forward pass
 * Blue edge is a backward pass
 * Red edge is data the backward pass depends on
 * Purple edge is intermediates created in the forward
 
 ```bash
-GRAPH=1 python3 test/test_mnist.py TestMNIST.test_sgd_onestep
+GRAPH=1 python3 test/models/test_mnist.py TestMNIST.test_sgd_onestep
 # requires dot, outputs /tmp/net.svg
 ```
 
 ### Running tests
 
 For more examples on how to run the full test suite please refer to the [CI workflow](.github/workflows/test.yml).
```

### Comparing `tinygrad-0.5.0/README.md` & `tinygrad-0.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 We are working on support for the Apple Neural Engine and the Google TPU in the `accel/` folder. Eventually, [we will build custom hardware](https://geohot.github.io/blog/jekyll/update/2021/06/13/a-breakdown-of-ai-chip-companies.html) for tinygrad, and it will be blindingly fast. Now, it is slow.
 
 This project is maintained by [tiny corp](https://tinygrad.org/).
 
 ### Installation
 
 ```bash
+python3 -m pip install git+https://git@github.com/geohot/tinygrad.git
+
+# or
 git clone https://github.com/geohot/tinygrad.git
 cd tinygrad
 python3 -m pip install -e .
 ```
 
 ### Contributing
 
@@ -67,27 +70,27 @@
 ```
 
 ## Is tinygrad fast?
 
 Try a matmul. See how, despite the style, it is fused into one kernel with the power of laziness.
 
 ```python
-DEBUG=3 OPTLOCAL=1 GPU=1 python3 -c "from tinygrad.tensor import Tensor;
+DEBUG=3 OPTLOCAL=1 python3 -c "from tinygrad.tensor import Tensor;
 N = 1024; a, b = Tensor.randn(N, N), Tensor.randn(N, N);
 c = (a.reshape(N, 1, N) * b.permute(1,0).reshape(1, N, N)).sum(axis=2);
 print((c.numpy() - (a.numpy() @ b.numpy())).mean())"
 ```
 
 Change to `DEBUG=4` to see the generated code.
 
 ## Neural networks?
 
-It turns out, a decent autograd tensor library is 90% of what you need for neural networks. Add an optimizer (SGD, RMSprop, and Adam implemented) from tinygrad.nn.optim, write some boilerplate minibatching code, and you have all you need.
+It turns out, a decent autograd tensor library is 90% of what you need for neural networks. Add an optimizer (SGD, Adam, AdamW implemented) from tinygrad.nn.optim, write some boilerplate minibatching code, and you have all you need.
 
-### Neural network example (from test/test_mnist.py)
+### Neural network example (from test/models/test_mnist.py)
 
 ```python
 from tinygrad.tensor import Tensor
 import tinygrad.nn.optim as optim
 
 class TinyBobNet:
   def __init__(self):
@@ -141,33 +144,33 @@
 hlops are syntactic sugar around mlops. They support most things torch does.
 
 ### mlops
 
 mlops are mid level ops. They understand derivatives. They are very simple.
 
 ```
-Log, Exp                                       # unary ops
+Relu, Log, Exp                                 # unary ops
 Sum, Max                                       # reduce ops (with axis argument)
 Maximum, Add, Sub, Mul, Pow, Div, Equal        # binary ops (no broadcasting, use expand)
 Expand, Reshape, Permute, Pad, Shrink, Flip    # movement ops
 ```
 
 You no longer need to write mlops for a new accelerator
 
 ### Adding an accelerator (llops)
 
 The autodiff stuff is all in mlops now so you can focus on the raw operations
 
 ```
-Buffer                                                     # class of memory on this device
-unary_op  (NOOP, NEG, NOT, EXP, LOG)                       # A -> A
-reduce_op (SUM, MAX)                                       # A -> B (smaller size, B has 1 in shape)
-binary_op (ADD, SUB, MUL, DIV, POW, CMPEQ, MAX)            # A + A -> A (all the same size)
-movement_op (EXPAND, RESHAPE, PERMUTE, PAD, SHRINK, FLIP)  # A -> B (different size)
-fused_op [[optional]] (MULACC)                             # A * A -> B
+Buffer                                                       # class of memory on this device
+unary_op  (NOOP, EXP, LOG, CAST)                             # A -> A
+reduce_op (SUM, MAX)                                         # A -> B (smaller size, B has 1 in shape)
+binary_op (ADD, SUB, MUL, DIV, POW, CMPEQ, MAX)              # A + A -> A (all the same size)
+movement_op (EXPAND, RESHAPE, PERMUTE, PAD, SHRINK, STRIDE)  # A -> B (different size)
+fused_op [[optional]] (MULACC)                               # A * A -> B
 ```
 
 ## ImageNet inference
 
 Despite being tiny, tinygrad supports the full EfficientNet. Pass in a picture to discover what it is.
 
 ```bash
@@ -176,23 +179,21 @@
 
 Or, if you have a webcam and cv2 installed
 
 ```bash
 ipython3 examples/efficientnet.py webcam
 ```
 
-PROTIP: Set "GPU=1" environment variable if you want this to go faster.
-
-PROPROTIP: Set "DEBUG=1" environment variable if you want to see why it's slow.
+PROTIP: Set "DEBUG=1" environment variable if you want to see why it's slow.
 
 ### tinygrad supports Stable Diffusion!
 
 You might need to download the [weight](https://huggingface.co/CompVis/stable-diffusion-v-1-4-original/resolve/main/sd-v1-4.ckpt) of Stable Diffusion and put it into weights/
 
-Run `GPU=1 python3 examples/stable_diffusion.py`
+Run `python3 examples/stable_diffusion.py`
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/geohot/tinygrad/master/docs/stable_diffusion_by_tinygrad.jpg">
 </p>
 
 <p align="center">
 "a horse sized cat eating a bagel"
@@ -223,15 +224,15 @@
 * Nodes are Tensors
 * Black edge is a forward pass
 * Blue edge is a backward pass
 * Red edge is data the backward pass depends on
 * Purple edge is intermediates created in the forward
 
 ```bash
-GRAPH=1 python3 test/test_mnist.py TestMNIST.test_sgd_onestep
+GRAPH=1 python3 test/models/test_mnist.py TestMNIST.test_sgd_onestep
 # requires dot, outputs /tmp/net.svg
 ```
 
 ### Running tests
 
 For more examples on how to run the full test suite please refer to the [CI workflow](.github/workflows/test.yml).
```

### Comparing `tinygrad-0.5.0/setup.py` & `tinygrad-0.6.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,42 +4,41 @@
 from setuptools import setup
 
 directory = os.path.abspath(os.path.dirname(__file__))
 with open(os.path.join(directory, 'README.md'), encoding='utf-8') as f:
   long_description = f.read()
 
 setup(name='tinygrad',
-      version='0.5.0',
-      description='You like pytorch? You like micrograd? You love tinygrad! heart',
+      version='0.6.0',
+      description='You like pytorch? You like micrograd? You love tinygrad! <3',
       author='George Hotz',
       license='MIT',
       long_description=long_description,
       long_description_content_type='text/markdown',
       packages = ['tinygrad', 'tinygrad.codegen', 'tinygrad.nn', 'tinygrad.runtime', 'tinygrad.shape'],
       classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License"
       ],
-      install_requires=['numpy', 'requests', 'pillow', 'tqdm', 'networkx'],
+      install_requires=['numpy', 'requests', 'pillow', 'tqdm', 'networkx', 'pyopencl'],
       python_requires='>=3.8',
       extras_require={
-        'gpu': ["pyopencl"],
         'llvm': ["llvmlite"],
         'cuda': ["pycuda"],
         'triton': ["triton>=2.0.0.dev20221202"],
         'metal': ["pyobjc-framework-Metal", "pyobjc-framework-Cocoa", "pyobjc-framework-libdispatch"],
         'linting': [
             "flake8",
             "pylint",
             "mypy",
             "pre-commit",
         ],
         'testing': [
-            "torch~=1.13.0",
+            "torch",
             "pytest",
             "pytest-xdist",
-            "onnx~=1.13.0",
+            "onnx",
             "onnx2torch",
             "opencv-python",
         ],
       },
       include_package_data=True)
```

### Comparing `tinygrad-0.5.0/test/test_assign.py` & `tinygrad-0.6.0/test/test_assign.py`

 * *Files identical despite different names*

### Comparing `tinygrad-0.5.0/test/test_conv.py` & `tinygrad-0.6.0/test/test_conv.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,30 +34,30 @@
     b = Tensor(np.arange(C).astype(np.float32))
     ret = Tensor.conv2d(x,w,b).relu().conv2d(w,b)
 
     print(ret.numpy())
 
   def test_two_binops_no_rerun(self):
     Tensor.no_grad = True
-    x = Tensor.ones(1,12,128,256)
-    w = Tensor.ones(32,12,3,3)
+    x = Tensor.randn(1,12,128,256)
+    w = Tensor.randn(32,12,3,3)
     out = x.conv2d(w, stride=(2,2), padding=(1,1))
     r1, r2 = out.relu(), (out-1)
-    r1.numpy(), r2.numpy()
+    np.testing.assert_allclose(r1.numpy(), np.maximum(out.numpy(), 0))
+    np.testing.assert_allclose(r2.numpy(), out.numpy() - 1)
     Tensor.no_grad = False
-    # TODO: make this a real test
 
   def test_two_overlapping_binops_no_rerun(self):
     Tensor.no_grad = True
-    x = Tensor.ones(1,12,128,256)
-    w = Tensor.ones(32,12,3,3)
+    x = Tensor.randn(1,12,128,256)
+    w = Tensor.randn(32,12,3,3)
     out = x.conv2d(w, stride=(2,2), padding=(1,1))
     r1, r2 = out.relu(), out.elu()
-    r1.numpy(), r2.numpy()
-    # TODO: make this a real test
+    np.testing.assert_allclose(r1.numpy(), np.maximum(out.numpy(), 0))
+    np.testing.assert_allclose(r2.numpy(), np.where(out.numpy() > 0, out.numpy(), (np.exp(out.numpy()) - 1)), atol=1e-5)
     Tensor.no_grad = False
 
   def test_first_three(self):
     Tensor.no_grad = True
     x = Tensor.ones(1,12,128,256)
 
     w = Tensor.ones(32,12,3,3)
```

### Comparing `tinygrad-0.5.0/test/test_conv_shapetracker.py` & `tinygrad-0.6.0/test/test_conv_shapetracker.py`

 * *Files identical despite different names*

### Comparing `tinygrad-0.5.0/test/test_gc.py` & `tinygrad-0.6.0/test/test_gc.py`

 * *Files identical despite different names*

### Comparing `tinygrad-0.5.0/test/test_net_speed.py` & `tinygrad-0.6.0/test/test_net_speed.py`

 * *Files identical despite different names*

### Comparing `tinygrad-0.5.0/test/test_nn.py` & `tinygrad-0.6.0/test/test_nn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 import unittest
 import numpy as np
 from tinygrad.tensor import Tensor, Device
-from tinygrad.nn import BatchNorm2d, Conv2d, Linear, GroupNorm, LayerNorm
+from tinygrad.nn import BatchNorm2d, Conv2d, Linear, GroupNorm, LayerNorm, LayerNorm2d
 import torch
 
 class TestNN(unittest.TestCase):
 
   def test_batchnorm2d(self, training=False):
     sz = 4
 
@@ -72,15 +72,15 @@
     BS, T, in_dim, out_dim = 4, 2, 8, 16
     _test_linear(Tensor.randn(BS, in_dim))
     _test_linear(Tensor.randn(BS, T, in_dim)) # test with more dims
 
   def test_conv2d(self):
     BS, C1, H, W = 4, 16, 224, 224
     C2, K, S, P = 64, 7, 2, 1
-    
+
     # create in tinygrad
     layer = Conv2d(C1, C2, kernel_size=K, stride=S, padding=P)
 
     # create in torch
     with torch.no_grad():
       torch_layer = torch.nn.Conv2d(C1, C2, kernel_size=K, stride=S, padding=P).eval()
       torch_layer.weight[:] = torch.tensor(layer.weight.numpy(), dtype=torch.float32)
@@ -127,9 +127,28 @@
     # test
     x = Tensor.randn(N, C, H, W)
     z = layer(x)
     torch_x = torch.tensor(x.cpu().numpy())
     torch_z = torch_layer(torch_x)
     np.testing.assert_allclose(z.numpy(), torch_z.detach().numpy(), atol=5e-3, rtol=5e-3)
 
+  def test_layernorm_2d(self):
+    N, C, H, W = 20, 5, 10, 10
+
+    # create in tinygrad
+    layer = LayerNorm2d(C)
+
+    # create in torch
+    with torch.no_grad():
+      torch_layer = torch.nn.LayerNorm([C]).eval()
+      torch_layer.weight[:] = torch.tensor(layer.weight.numpy(), dtype=torch.float32)
+      torch_layer.bias[:] = torch.tensor(layer.bias.numpy(), dtype=torch.float32)
+
+    # test
+    x = Tensor.randn(N, C, H, W)
+    z = layer(x)
+    torch_x = torch.tensor(x.cpu().numpy())
+    torch_z = torch_layer(torch_x.permute(0,2,3,1)).permute(0,3,1,2)
+    np.testing.assert_allclose(z.numpy(), torch_z.detach().numpy(), atol=5e-3, rtol=5e-3)
+
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.5.0/test/test_ops.py` & `tinygrad-0.6.0/test/test_ops.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import torch
 import time
 import numpy as np
 import unittest
 from tinygrad.tensor import Tensor
 from tinygrad.helpers import getenv, IMAGE
+from tinygrad.lazy import Device
 
 FORWARD_ONLY = getenv("FORWARD_ONLY", 0)
+PRINT_TENSORS = getenv("PRINT_TENSORS", 0)
 def helper_test_op(shps, torch_fxn, tinygrad_fxn=None, atol=1e-6, rtol=1e-3, grad_atol=1e-4, grad_rtol=1e-3, forward_only=False, vals=None, a=-0.5, b=3):
   if tinygrad_fxn is None: tinygrad_fxn = torch_fxn
   torch.manual_seed(0)
   np.random.seed(0)
   if shps is None:
     ts = [torch.tensor(x, requires_grad=True) for x in vals]
   else:
@@ -22,30 +24,31 @@
   torch_fp = time.monotonic() - st
 
   st = time.monotonic()
   ret = tinygrad_fxn(*tst).realize()
   tinygrad_fp = time.monotonic() - st
 
   def compare(s, x,y,atol,rtol):
-    if y.shape != tuple(): assert x.shape == y.shape, f"shape mismatch {x.shape} != {y.shape}"
+    if PRINT_TENSORS: print(s, x, y)
+    if y.shape != tuple(): assert x.shape == y.shape, f"shape mismatch (tinygrad){x.shape} != (torch){y.shape}"
     try:
       np.testing.assert_allclose(x,y, atol=atol, rtol=rtol)
     except Exception:
       raise Exception(f"{s} failed shape {x.shape}")
 
   compare("forward pass", ret.numpy(), out.detach().numpy(), atol=atol, rtol=rtol)
 
   torch_fbp, tinygrad_fbp = np.nan, np.nan
   if not forward_only and not FORWARD_ONLY:
     st = time.monotonic()
-    out.square().mean().backward()
+    (out+1).square().mean().backward()
     torch_fbp = time.monotonic() - st
 
     st = time.monotonic()
-    ret.square().mean().backward()
+    (ret+1).square().mean().backward()
     for tt in tst: tt.grad.realize()
     tinygrad_fbp = time.monotonic() - st
 
     for i, (t, tt) in enumerate(zip(ts, tst)):
       compare(f"backward pass tensor {i}", tt.grad.numpy(), t.grad.detach().numpy(), atol=grad_atol, rtol=grad_rtol)
 
   print("\ntesting %40r   torch/tinygrad fp: %.2f / %.2f ms  bp: %.2f / %.2f ms " % (shps, torch_fp*1000, tinygrad_fp*1000, torch_fbp*1000, tinygrad_fbp*1000), end="")
@@ -63,15 +66,15 @@
   def _test_cmp(self, fxn, reverse=True):
     for shps in [[(3, 4, 5), (3, 4, 5)], [(3, 4, 5), (5,)], [(5,), (3, 4, 5)]]:
       helper_test_op(shps, fxn, fxn, forward_only=True)
     helper_test_op(None, fxn, fxn, forward_only=True, vals=[[0.,1,2], [2.,1,0]])
     helper_test_op(None, lambda x,y: fxn(x,2), lambda x,y: fxn(x,2), forward_only=True, vals=[[0.,1,2], [2.,1,0]])
     if reverse: helper_test_op(None, lambda x,y: fxn(2,y), lambda x,y: fxn(2,y), forward_only=True, vals=[[0.,1,2], [2.,1,0]])
 
-  def test_cmp_eq(self): self._test_cmp(lambda x,y: x.eq(y), reverse=False)
+  def test_cmp_eq(self): self._test_cmp(lambda x,y: x==y, reverse=False)
   def test_cmp_gt(self): self._test_cmp(lambda x,y: x>y)
   def test_cmp_ge(self): self._test_cmp(lambda x,y: x>=y)
   def test_cmp_lt(self): self._test_cmp(lambda x,y: x<y)
   def test_cmp_le(self): self._test_cmp(lambda x,y: x<=y)
 
   def test_cmp_eq_backwards(self):
     t1 = torch.ones(4, requires_grad=True)
@@ -87,26 +90,29 @@
     self.assertRaises(RuntimeError, (t1 < t2).sum().backward)
     tt1 = Tensor.ones(4, requires_grad=True)
     tt2 = Tensor.ones(4, requires_grad=True)
     self.assertRaises(RuntimeError, (tt1 < tt2).sum().backward)
 
   def test_maximum(self):
     helper_test_op([(45,65), (45,65)], torch.maximum, Tensor.maximum)
+    helper_test_op(None, torch.maximum, Tensor.maximum, vals=[[1., 0., 3., 4.], [1., 2., 3., 0.]])
   def test_minimum(self):
     helper_test_op([(45,65), (45,65)], torch.minimum, Tensor.minimum)
   def test_add(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x+y, Tensor.add)
   def test_add_simple(self):
     helper_test_op([(256), (256)], lambda x,y: x+y, Tensor.add, forward_only=True)
   def test_broadcasted_add(self):
     helper_test_op([(45,65), (45,1)], lambda x,y: x+y, lambda x,y: x+y)
   def test_broadcasted_add_2(self):
     helper_test_op([(45,65), (65,)], lambda x,y: x+y, lambda x,y: x+y)
   def test_sub(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x-y, Tensor.sub)
+  def test_neg(self):
+    helper_test_op([(45,65)], lambda x: -x)
   def test_mul(self):
     helper_test_op([(64,64), (64,64)], lambda x,y: x*y, Tensor.mul)
   def test_div(self):
     helper_test_op([(45,65), (45,65)], lambda x,y: x/y, Tensor.div)
   def test_div_const(self):
     helper_test_op([(45,65)], lambda x: x/255, lambda x: x/255)
     helper_test_op([(45,65)], lambda x: x/1, lambda x: x/1)
@@ -121,26 +127,43 @@
   def test_pow_const(self):
     helper_test_op([(45,65)], lambda x: x**1.0, lambda x: x**1.0)
     helper_test_op([(45,65)], lambda x: 1.0**x, lambda x: 1.0**x)
     helper_test_op([(45,65)], lambda x: x**2.0, lambda x: x**2.0)
     helper_test_op([(45,65)], lambda x: 2.0**x, lambda x: 2.0**x)
   def test_sqrt(self):
     helper_test_op([(45,65)], lambda x: x.sqrt(), Tensor.sqrt, a=0)
+  
+  def test_sin(self):
+    helper_test_op([(45,65)], lambda x: x.sin(), Tensor.sin, a=0)
+  def test_cos(self):
+    helper_test_op([(45,65)], lambda x: x.cos(), Tensor.cos, a=0)
+  def test_tan(self):
+    helper_test_op([(45,65)], lambda x: x.tan(), Tensor.tan, a=0)
+    
   def test_relu(self):
-    helper_test_op([(45,65)], lambda x: x.relu(), Tensor.relu)
+    helper_test_op([(64,64)], lambda x: x.relu(), Tensor.relu)
+  def test_relu_exact(self):
+    helper_test_op(None, lambda x: x.relu(), Tensor.relu, vals=[[-1.,0,1]])
+  def test_relu_maximum_exact(self):
+    helper_test_op(None, lambda x: torch.maximum(x, torch.zeros_like(x, requires_grad=False)), lambda x: Tensor.maximum(x, 0), vals=[[-1.,0,1]])
   def test_leakyrelu(self):
     helper_test_op([(45,65)], lambda x: torch.nn.functional.leaky_relu(x,0.01), Tensor.leakyrelu)
+  def test_celu(self):
+    for val in range(1, 5):
+      helper_test_op([(45,65)], lambda x: torch.nn.functional.celu(x,val), lambda x: x.celu(val))
   def test_abs(self):
     helper_test_op([(45,65)], lambda x: torch.abs(x), Tensor.abs)
   def test_log(self):
     helper_test_op([(45,65)], lambda x: torch.log(x), Tensor.log)
   def test_exp(self):
     helper_test_op([(45,65)], lambda x: torch.exp(x), Tensor.exp)
   def test_sign(self):
     helper_test_op([(45,65)], lambda x: torch.sign(x), Tensor.sign)
+  def test_softsign(self):
+    helper_test_op([(45,65)], lambda x: torch.nn.functional.softsign(x), Tensor.softsign)
   def test_sigmoid(self):
     helper_test_op([(45,65)], lambda x: x.sigmoid(), Tensor.sigmoid)
   def test_softplus(self):
     helper_test_op([(45,65)], lambda x: torch.nn.functional.softplus(x), Tensor.softplus, atol=1e-6, grad_atol=1e-6)
   @unittest.skip("not supported in older pytorch")
   def test_gelu(self):
     helper_test_op([(45,65)], lambda x: torch.nn.functional.gelu(x, approximate="tanh"), Tensor.gelu)
@@ -191,37 +214,55 @@
     helper_test_op([(45,3)], lambda x: x.max(), Tensor.max)
     helper_test_op([(45,3)], lambda x: x.max().mul(0.5), lambda x: Tensor.max(x).mul(0.5))
     helper_test_op(None, lambda x: x.max().mul(0.5), lambda x: Tensor.max(x).mul(0.5),
             vals=[
                 [[1.0,1.0,0.0,1.0]],
                 ])
     helper_test_op([(3,4,5,6)], lambda x: x.max(axis=1)[0], lambda x: Tensor.max(x, axis=1))
+  def test_mean(self):
+    helper_test_op([(3,4,5,6)], lambda x: x.mean())
   def test_mean_axis(self):
     helper_test_op([(3,4,5,6)], lambda x: x.mean(axis=(1,2)), lambda x: Tensor.mean(x, axis=(1,2)))
+  def test_std(self):
+    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, unbiased=False), lambda x: Tensor.std(x))
+  def test_std_axis(self):
+    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, unbiased=False, dim=0), lambda x: Tensor.std(x, axis=0))
+    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, unbiased=False, dim=2), lambda x: Tensor.std(x, axis=2))
+    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, unbiased=False, dim=[1, 2]), lambda x: Tensor.std(x, axis=[1, 2]))
+    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, unbiased=False, dim=None), lambda x: Tensor.std(x, axis=None))
+  def test_std_keepdim(self):
+    helper_test_op([(45, 65, 85)], lambda x: torch.std(x, keepdim=True), lambda x: Tensor.std(x, keepdim=True))
   def test_log_softmax(self):
     helper_test_op([(45,65)], lambda x: torch.nn.LogSoftmax(dim=1)(x), Tensor.log_softmax, atol=1e-7, grad_atol=1e-7)
   def test_log_softmax_other_axis(self):
     helper_test_op([(10,10,10)], lambda x: x.log_softmax(0), lambda x: x.log_softmax(0), atol=1e-7, grad_atol=1e-7)
     helper_test_op([(10,10,10)], lambda x: x.log_softmax(1), lambda x: x.log_softmax(1), atol=1e-7, grad_atol=1e-7)
     helper_test_op([(10,10,10)], lambda x: x.log_softmax(2), lambda x: x.log_softmax(2), atol=1e-7, grad_atol=1e-7)
   def test_tanh(self):
     helper_test_op([(45,65)], lambda x: x.tanh(), Tensor.tanh, atol=1e-6, grad_atol=1e-6)
+  def test_hardtanh(self):
+    for val in range(10, 30, 5):
+      helper_test_op([(45,65)], lambda x: torch.nn.functional.hardtanh(x,-val, val), lambda x: x.hardtanh(-val, val), atol=1e-6, grad_atol=1e-6)
   def test_topo_sort(self):
     helper_test_op([(45,65)], lambda x: (x+x)*x, lambda x: x.add(x).mul(x), atol=1e-6, grad_atol=1e-6)
 
   def test_scalar_mul(self):
     helper_test_op([(45,65)], lambda x: x*2, lambda x: x*2)
   def test_scalar_rmul(self):
     helper_test_op([(45,65)], lambda x: 2*x, lambda x: 2*x)
 
   def test_scalar_sub(self):
     helper_test_op([(45,65)], lambda x: x-2, lambda x: x-2)
   def test_scalar_rsub(self):
     helper_test_op([(45,65)], lambda x: 2-x, lambda x: 2-x)
 
+  def test_flip_eye_crash(self):
+    helper_test_op([], lambda: (torch.eye(10)@torch.eye(10).flip(0)),
+                       lambda: (Tensor.eye(10)@Tensor.eye(10).flip(0)), forward_only=True)
+
   def test_broadcast_full(self):
     for torch_op, tinygrad_op in [(torch.add, Tensor.add), (torch.sub, Tensor.sub), (torch.mul, Tensor.mul),
                                   (torch.div, Tensor.div), (torch.pow, Tensor.pow)]:
       for shapes in [((5,13,24,16), (5,1,24,1)), ((1,3,1,7,1), (2,1,5,1,8))]:
         with self.subTest(op=torch_op.__name__, shapes=shapes):
           helper_test_op(shapes, torch_op, tinygrad_op, a=-0.5 if tinygrad_op != Tensor.pow else 0.0)
 
@@ -251,28 +292,30 @@
   def test_slice_one_multi(self):
     helper_test_op([(10,10)], lambda x: x[1], lambda x: x[1])
 
   def test_pad2d(self):
     helper_test_op([(3,3,3,3)], lambda x: torch.nn.functional.pad(x, (1,2,3,4)), lambda x: x.pad2d(padding=(1,2,3,4)))
 
   def test_transpose(self):
-    helper_test_op([(3,3,3)], lambda x: x.transpose(1,2), lambda x: x.transpose(order=(0,2,1)))
-    helper_test_op([(3,3,3)], lambda x: x.transpose(0,2), lambda x: x.transpose(order=(2,1,0)))
-    helper_test_op([(1,2,3,4)], lambda x: x.movedim((3,0,2,1),(0,1,2,3)), lambda x: x.transpose(order=(3,0,2,1)))
-    helper_test_op([(3,4,5,6)], lambda x: x.movedim((3,2,1,0),(0,1,2,3)), lambda x: x.transpose(order=(3,2,1,0)))
+    helper_test_op([(3,3,3)], lambda x: x.transpose(1,2), lambda x: x.transpose(1,2))
+    helper_test_op([(3,3,3)], lambda x: x.transpose(0,2), lambda x: x.transpose(0,2))
+    helper_test_op([(1,2,3,4)], lambda x: x.movedim((3,0,2,1),(0,1,2,3)), lambda x: x.permute(order=(3,0,2,1)))
+    helper_test_op([(3,4,5,6)], lambda x: x.movedim((3,2,1,0),(0,1,2,3)), lambda x: x.permute(order=(3,2,1,0)))
 
   def test_reshape(self):
     helper_test_op([(4,3,6,6)], lambda x: torch.reshape(x, (-1,3,6,6)), lambda x: x.reshape(shape=(-1,3,6,6)))
     helper_test_op([(4,3,6,6)], lambda x: torch.reshape(x, (-1,1,6,6)), lambda x: x.reshape(shape=(-1,1,6,6)))
 
   def test_flip(self):
     helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (0,)), lambda x: x.flip(axis=(0,)))
     helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (0,1)), lambda x: x.flip(axis=(0,1)))
     helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (0,1,3)), lambda x: x.flip(axis=(0,1,3)))
     helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (3,)), lambda x: x.flip(axis=(3,)))
+    helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (0,1,3)).flip((0,)), lambda x: x.flip(axis=(0,1,3)).flip(0))
+    helper_test_op([(4,3,6,6)], lambda x: torch.flip(x, (3,)), lambda x: x.flip(axis=(-1,)))
 
   def test_unsqueeze(self):
     helper_test_op([(4,3,6,6)], lambda x: torch.unsqueeze(x, 0), lambda x: x.unsqueeze(dim=0))
     helper_test_op([(4,3,6,6)], lambda x: torch.unsqueeze(x, 4), lambda x: x.unsqueeze(dim=4))
     helper_test_op([(4,3,6,6)], lambda x: torch.unsqueeze(x, -1), lambda x: x.unsqueeze(dim=-1))
     helper_test_op([(4,3,6,6)], lambda x: torch.unsqueeze(x, -3), lambda x: x.unsqueeze(dim=-3))
 
@@ -290,23 +333,23 @@
   @unittest.skip("very slow")
   def test_sd_big_conv(self):
     # internal shape (1, 1, 512, 62, 62, 512, 3, 3) overflows a int
     helper_test_op([(1,256,64,64), (512,256,3,3)],
                     lambda x,w: torch.nn.functional.conv2d(x, w),
                     lambda x,w: x.conv2d(w), atol=1e-2)
 
-  @unittest.skip("not supported with IMAGE=1")
+  @unittest.skip("slow")
   def test_large_bs_conv(self):
     # large batch size can cause OpenCL image to exceed max image height on macOS
     # (or cause the conv kernel to overflow short sampling coords)
     helper_test_op([(4096,3,3,3), (1,3,3,3)],
                     lambda x,w: torch.nn.functional.conv2d(x, w),
                     lambda x,w: x.conv2d(w), atol=1e-4, rtol=1e-2)
 
-  @unittest.skip("not supported with IMAGE=1")
+  @unittest.skip("slow")
   def test_large_ic_conv(self):
     # large input channel count can cause OpenCL image to exceed max image width on macOS
     helper_test_op([(1,2048,3,3), (1,2048,3,3)],
                     lambda x,w: torch.nn.functional.conv2d(x, w),
                     lambda x,w: x.conv2d(w), atol=1e-4)
 
   def test_biased_conv2d(self):
@@ -316,14 +359,41 @@
       lambda x,w,b: Tensor.conv2d(x,w,b).relu().conv2d(w,b), atol=1e-4)
 
   def test_simple_conv2d(self):
     helper_test_op([(1,4,9,9), (4,4,3,3)],
       lambda x,w: torch.nn.functional.conv2d(x,w).relu(),
       lambda x,w: Tensor.conv2d(x,w).relu(), atol=1e-4, grad_rtol=1e-5)
 
+  @unittest.skipIf(IMAGE>0, "no conv3d on images")
+  def test_simple_conv3d(self):
+    helper_test_op([(1,4,9,9,9), (4,4,3,3,3)],
+      lambda x,w: torch.nn.functional.conv3d(x,w).relu(),
+      lambda x,w: Tensor.conv2d(x,w).relu(), atol=1e-4, grad_rtol=1e-5)
+
+  @unittest.skipIf(IMAGE>0, "no conv3d on images")
+  def test_padded_conv3d(self):
+    helper_test_op([(1,4,9,9,9), (4,4,3,3,3)],
+      lambda x,w: torch.nn.functional.conv3d(x,w,padding=1).relu(),
+      lambda x,w: Tensor.conv2d(x,w,padding=[1,1,1,1,1,1]).relu(), atol=1e-4, grad_rtol=1e-5)
+
+  def test_simple_conv2d_m4(self):
+    helper_test_op([(1,16,18,18), (16,16,3,3)],
+      lambda x,w: torch.nn.functional.conv2d(x,w).relu(),
+      lambda x,w: Tensor.conv2d(x,w).relu(), atol=1e-4, grad_rtol=1e-5)
+
+  def test_simple_conv2d_1x1(self):
+    helper_test_op([(1,4,9,9), (4,4,1,1)],
+      lambda x,w: torch.nn.functional.conv2d(x,w).relu(),
+      lambda x,w: Tensor.conv2d(x,w).relu(), atol=1e-4, grad_rtol=1e-5)
+
+  def test_simple_conv2d_1x1_m4(self):
+    helper_test_op([(1,16,32,32), (16,16,1,1)],
+      lambda x,w: torch.nn.functional.conv2d(x,w).relu(),
+      lambda x,w: Tensor.conv2d(x,w).relu(), atol=1e-4, grad_rtol=1e-5)
+
   def test_nested_conv2d(self):
     helper_test_op([(1,32,9,9), (32,32,3,3), (32,32,3,3)],
       lambda x,w1,w2: torch.nn.functional.conv2d(torch.nn.functional.conv2d(x,w1).relu(), w2).relu(),
       lambda x,w1,w2: x.conv2d(w1).relu().conv2d(w2).relu(), atol=1e-4, grad_rtol=1e-5)
 
   # expect reduce nodes == 3
   def test_simple_conv2d_nhwc(self):
@@ -362,24 +432,24 @@
   def test_simple_grouped_conv2d(self):
     bs = 1
     groups = 2
     rcout = 1
     cin = 2
     helper_test_op([(bs,groups*cin,1,1), (groups*rcout,cin,1,1)],
       lambda x,w: torch.nn.functional.conv2d(x,w,groups=groups).relu(),
-      lambda x,w: Tensor.conv2d(x,w,groups=groups).relu(), atol=1e-4, grad_rtol=1e-5, forward_only=IMAGE>=2)
+      lambda x,w: Tensor.conv2d(x,w,groups=groups).relu(), atol=1e-4, grad_rtol=1e-5)
 
   def test_medium_grouped_conv2d(self):
     bs = 1
     groups = 2
     rcout = 2
     cin = 2
     helper_test_op([(bs,groups*cin,1,1), (groups*rcout,cin,1,1)],
       lambda x,w: torch.nn.functional.conv2d(x,w,groups=groups).relu(),
-      lambda x,w: Tensor.conv2d(x,w,groups=groups).relu(), atol=1e-4, grad_rtol=1e-5, forward_only=IMAGE>=2)
+      lambda x,w: Tensor.conv2d(x,w,groups=groups).relu(), atol=1e-4, grad_rtol=1e-5)
 
   def test_depthwise_conv2d(self):
     bs = 1
     groups = 32
     rcout = 1
     cin = 1
     helper_test_op([(bs,groups*cin,32,32), (groups*rcout,cin,1,1)],
@@ -496,14 +566,15 @@
   def test_maxpool2d_bigger_stride(self):
     for stride in [(2,3), (3,2), 2, 3]:
       with self.subTest(stride=stride):
         helper_test_op([(32,2,110,28)],
           lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(2,2), stride=stride),
           lambda x: Tensor.max_pool2d(x, kernel_size=(2,2), stride=stride))
 
+  @unittest.skipIf(Device.DEFAULT == "CUDA", "CUDA fails on this")
   def test_maxpool2d_unit_stride(self):
     helper_test_op([(32,2,110,28)],
       lambda x: torch.nn.functional.max_pool2d(x, kernel_size=(5,5), stride=1),
       lambda x: Tensor.max_pool2d(x, kernel_size=(5,5), stride=1))
 
   def test_maxpool2d_smaller_stride(self):
     for stride in [(2,3), (3,2), 2, 3]:
@@ -529,16 +600,47 @@
     for dim in range(-1, 2):
       helper_test_op([(45,65), (45,65)], lambda x,y: torch.cat((x,y), dim), lambda x,y: x.cat(y, dim=dim))
 
   def test_multicat(self):
     for dim in range(-1, 2):
       helper_test_op([(45,65), (45,65), (45,65)], lambda x,y,z: torch.cat((x,y,z), dim), lambda x,y,z: x.cat(y, z, dim=dim))
 
+  def test_stack(self):
+    x = Tensor.randn(45, 65, 3)
+
+    for dim in range(-1, 3):
+      helper_test_op([(45, 65, 3), (45, 65, 3), (45, 65, 3)], lambda x, y, z: torch.stack((x, y, z), dim=dim), lambda x, y, z: Tensor.stack([x, y, z], dim=dim))
+
+    with self.assertRaises(IndexError):
+      Tensor.stack([x], dim=77)
+
+  def test_repeat(self):
+    x = Tensor.randn(45, 65, 3)
+    base_repeats = [2, 4, 3]
+
+    for reps in [[], [4], [2, 1], [3, 2, 2]]:
+      repeats = base_repeats + reps
+      helper_test_op([(45, 65, 3)], lambda x: x.repeat(*repeats), lambda x: x.repeat(repeats))
+
+    with self.assertRaises(AssertionError):
+      x.repeat((2, 4))
+
+    with self.assertRaises(AssertionError):
+      x.repeat((2, 0, 4))
+
+
   def test_clip(self):
     helper_test_op([(45,65)], lambda x: x.clip(-2.3, 1.2), lambda x: x.clip(-2.3, 1.2))
 
   def test_matvec(self):
     helper_test_op([(1,128), (128,128), (128,128)], lambda x,y,z: (x@y).relu()@z, atol=1e-4)
 
+  # this was the failure in llama early realizing freqs_cis
+  def test_double_slice(self):
+    helper_test_op([(4,4)], lambda x: x[:, 1:2][1:2])
+    helper_test_op([(4,4)], lambda x: x[1:3][1:2])
+    helper_test_op([(4,4)], lambda x: x[:, 1:2][0:1])
+    helper_test_op([(4,4)], lambda x: x[:, 1:2][:, 0:1])
+
 if __name__ == '__main__':
   np.random.seed(1337)
   unittest.main(verbosity=2)
```

### Comparing `tinygrad-0.5.0/test/test_randomness.py` & `tinygrad-0.6.0/test/test_randomness.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import math
 import unittest
 import numpy as np
+import torch
 from tinygrad.tensor import Tensor
 
 # https://gist.github.com/devries/11405101
 def ksprob(a):
   fac, total, termbf = 2.0, 0.0, 0.0
   a2 = -2.0 * a * a
   for j in range(1, 101):
@@ -33,43 +34,44 @@
     if dtemp > d:
       d = dtemp
   ne = float(n1 * n2) / float(n1 + n2)
   nesq = math.sqrt(ne)
   prob = ksprob((nesq + 0.12 + 0.11 / nesq) * d)
   return prob
 
-def equal_distribution(tinygrad_func, numpy_func, shape=(20, 23), alpha=0.05):
+def normal_test(func, shape=(20, 23), alpha=0.05):
+  x = func(*shape).cpu().numpy().flatten()
+  y = np.random.randn(*shape).flatten()
+  return kstest(x, y) >= alpha
+
+def equal_distribution(tiny_func, torch_func, numpy_func, shape=(20, 23), alpha=0.05):
   Tensor.manual_seed(1337)
+  torch.manual_seed(1337)
   np.random.seed(1337)
-  x = tinygrad_func(*shape).cpu().numpy().flatten()
+  x = tiny_func(*shape).cpu().numpy().flatten()
   y = numpy_func(shape).flatten()
-  p = kstest(x, y)
-  return p >= alpha
-
-def normal_test(func, shape=(20, 23), alpha=0.05):
-  y = lambda x: np.random.randn(*x)
-  p = equal_distribution(func, y, shape=shape, alpha=alpha)
-  return p >= alpha
+  z = torch_func(shape).numpy().flatten()
+  return kstest(x, y) >= alpha and kstest(x, z) >= alpha
 
 class TestRandomness(unittest.TestCase):
   def test_rand(self):
     self.assertFalse(normal_test(Tensor.rand))
-    self.assertTrue(equal_distribution(Tensor.rand, lambda x: np.random.rand(*x)))
+    self.assertTrue(equal_distribution(Tensor.rand, torch.rand, lambda x: np.random.rand(*x)))
 
   def test_randn(self):
     self.assertTrue(normal_test(Tensor.randn))
-    self.assertFalse(equal_distribution(Tensor.randn, lambda x: np.random.rand(*x)))
+    self.assertTrue(equal_distribution(Tensor.randn, torch.randn, lambda x: np.random.randn(*x)))
 
   def test_uniform(self):
     self.assertFalse(normal_test(Tensor.uniform))
-    self.assertTrue(equal_distribution(Tensor.uniform, lambda x: np.random.rand(*x) * 2 - 1))
+    self.assertTrue(equal_distribution(Tensor.uniform, lambda x: torch.nn.init.uniform_(torch.empty(x), a=-1, b=1), lambda x: np.random.rand(*x) * 2 - 1))
 
   def test_scaled_uniform(self):
     self.assertFalse(normal_test(Tensor.scaled_uniform))
-    self.assertTrue(equal_distribution(Tensor.scaled_uniform, lambda x: (np.random.rand(*x) * 2 - 1) / math.sqrt(math.prod(x))))
+    self.assertTrue(equal_distribution(Tensor.scaled_uniform, lambda x: torch.nn.init.uniform_(torch.empty(x), a=-1, b=1) / math.sqrt(math.prod(x)), lambda x: (np.random.rand(*x) * 2 - 1) / math.sqrt(math.prod(x))))
 
   def test_glorot_uniform(self):
     self.assertFalse(normal_test(Tensor.glorot_uniform))
-    self.assertTrue(equal_distribution(Tensor.glorot_uniform, lambda x: (np.random.rand(*x) * 2 - 1) * math.sqrt(6 / (x[0] + math.prod(x[1:])))))
+    self.assertTrue(equal_distribution(Tensor.glorot_uniform, lambda x: torch.nn.init.xavier_uniform_(torch.empty(x)), lambda x: (np.random.rand(*x) * 2 - 1) * math.sqrt(6 / (x[0] + math.prod(x[1:])))))
 
 if __name__ == "__main__":
   unittest.main()
```

### Comparing `tinygrad-0.5.0/test/test_specific_conv.py` & `tinygrad-0.6.0/test/test_specific_conv.py`

 * *Files identical despite different names*

### Comparing `tinygrad-0.5.0/test/test_speed_v_torch.py` & `tinygrad-0.6.0/test/test_speed_v_torch.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,23 +6,32 @@
 import unittest
 import torch
 torch.set_num_threads(1)
 import time
 import numpy as np
 np.set_printoptions(linewidth=160)
 from functools import partial
+from tinygrad.lazy import Device
 from tinygrad.ops import GlobalCounters
 from tinygrad.tensor import Tensor
 from tinygrad.nn import Conv2d
 from tinygrad.helpers import colored, getenv, DEBUG
 from tinygrad.jit import TinyJit
 
 IN_CHANS = [int(x) for x in getenv("IN_CHANS", "4,16,64").split(",")]
 
 torch_device = torch.device('mps' if getenv("MPS", 0) else ('cuda' if getenv("TORCHCUDA", 0) else 'cpu'))
+if str(torch_device) == "mps":
+  import torch.mps
+  sync = lambda: torch.mps.synchronize()
+elif str(torch_device) == "cuda":
+  import torch.cuda
+  sync = lambda: torch.cuda.synchronize()
+else:
+  sync = lambda: None
 
 def colorize_float(x):
   ret = f"{x:7.2f}x"
   if x < 0.75:
     return colored(ret, 'green')
   elif x > 1.5:
     return colored(ret, 'red')
@@ -31,32 +40,39 @@
 
 save_ops, save_mem = 0, 0
 CNT = 8
 def helper_test_speed(f1, *args):
   global save_ops, save_mem
   ets = []
   ret = None
-  for _ in range(CNT):
+  cache_defeat = np.zeros((2048,2048))
+  for i in range(CNT):
     del ret
-    args = [(x+1).realize() if isinstance(x, Tensor) else (None if x is None else (x+1)) for x in args]  # cache defeats
+
+    # operation cache defeats
+    args = [(x+1).realize() if isinstance(x, Tensor) else (None if x is None else (x+1)) for x in args]
 
     # force syncing
     [x.numpy() if isinstance(x, Tensor) or str(torch_device) == "cpu" else x.cpu().numpy() for x in args if x is not None]
 
+    # clear 32MB global memory cache (CPU and global memory only)
+    cache_defeat += 1
+
+    # manual pre sync
+    if isinstance(args[0], Tensor): Device[args[0].device].synchronize()
+    else: sync()
+
     GlobalCounters.global_ops = 0
     GlobalCounters.global_mem = 0
-    if DEBUG >= 4: print("benchmark start")
-    st = time.monotonic()
+    st = time.perf_counter()
     ret = f1(*args)
-    # not ideal, it's copying (sometimes). why is this so slow in tinygrad?
-    if isinstance(ret, Tensor) or str(torch_device) == "cpu": ret.numpy()
-    else: ret.cpu().numpy()
-    et = (time.monotonic() - st) * 1000
-    ets.append(et)
-    if DEBUG >= 4: print("benchmark stop")
+    if isinstance(ret, Tensor): Device[ret.device].synchronize()
+    else: sync()
+    et = (time.perf_counter() - st) * 1000
+    if i >= 1: ets.append(et)   # not the first run / one used for OPTLOCAL
     if GlobalCounters.global_ops:
       save_ops, save_mem = GlobalCounters.global_ops, GlobalCounters.global_mem
   return ret.cpu().numpy(), np.min(ets)
 
 def helper_test_generic_square(name, N, f1, f2, onearg=False):
   torch.manual_seed(0)
   torch_a = (torch.rand(N, N) - 0.5).to(torch_device)
@@ -72,25 +88,25 @@
   global prefix
   with torch.no_grad():
     val_torch, et_torch = helper_test_speed(f1, *f1_args)
   val_tinygrad, et_tinygrad = helper_test_speed(f2, *f2_args)
 
   desc = "faster" if et_torch > et_tinygrad else "slower"
   flops = save_ops*1e-6
-  mem = save_mem*4*1e-6
+  mem = save_mem*1e-6
   print(f"{prefix}{name:40s} {et_torch:7.2f} ms ({flops/et_torch:8.2f} GFLOPS {mem/et_torch:8.2f} GB/s) in torch, {et_tinygrad:7.2f} ms ({flops/et_tinygrad:8.2f} GFLOPS {mem/et_tinygrad:8.2f} GB/s) in tinygrad, {colorize_float(et_tinygrad/et_torch)} {desc} {flops:7.2f} MOPS {mem:7.2f} MB")
   prefix = " "
   np.testing.assert_allclose(val_tinygrad, val_torch, atol=1e-4, rtol=1e-3)
 
 class TestSpeed(unittest.TestCase):
   def setUp(self):
     global prefix
     prefix = " " if prefix is None else ""
     return super().setUp()
-  
+
   def test_sub(self):
     def f(a, b): return a-b
     helper_test_generic_square('sub', 4096, f, f)
 
   def test_pow(self):
     def f(a, b): return a.pow(b)
     helper_test_generic_square('pow', 2048, f, f)
@@ -112,15 +128,15 @@
 
   def test_permute(self):
     for N in [1024, 4096]:
       # this is a 64MB tensor, M1 L1 cache is 128kB
       # to fit easily in L1, rotations should be 128x128 chunks. 128x128 is also the AMX size
       def f(a, b): return a.permute(1,0).contiguous()
       helper_test_generic_square('permute', N, f, f, onearg=True)
-    
+
   def test_double_permute(self):
     N = 64
     torch.manual_seed(0)
     torch_a = (torch.rand(N, N, N, N) - 0.5).to(torch_device)
     tiny_a = Tensor(torch_a.cpu().numpy())
     def f(a): return a.permute(1,0,3,2).contiguous()
     helper_test_generic(f"double_permute {tiny_a.shape}", f, (torch_a,), TinyJit(lambda a: f(a).realize()), (tiny_a,))
@@ -156,22 +172,26 @@
 
   def test_add_sq(self):
     def f(a, b): return a*a + b*b
     helper_test_generic_square('add_sq', 4096, f, f)
 
   def test_gemm(self):
     def f(a, b): return a @ b
-    helper_test_generic_square('gemm', 512, f, f)
+    helper_test_generic_square('gemm', 1024, f, f)
+
+  def test_gemm_small(self):
+    def f(a, b): return a @ b
+    helper_test_generic_square('gemm', 256, f, f)
 
   def test_gemm_unrolled(self):
     N = 512
     def f1(a, b): return a@b.T
     def f2(a, b): return (a.reshape(N, 1, N).expand(N, N, N) * b.reshape(1, N, N).expand(N, N, N)).sum(axis=2)
     helper_test_generic_square('gemm_unrolled', N, f1, f2)
-  
+
   def test_gemm_unrolled_permute_l(self):
     N = 512
     def f1(a, b): return a.T@b.T
     def f2(a, b): return (a.permute(1,0).reshape(N, 1, N).expand(N, N, N) * b.reshape(1, N, N).expand(N, N, N)).sum(axis=2)
     helper_test_generic_square('gemm_unrolled_permute_l', N, f1, f2)
 
   def test_gemm_unrolled_permute_r(self):
```

### Comparing `tinygrad-0.5.0/test/test_tensor.py` & `tinygrad-0.6.0/test/test_tensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -145,14 +145,14 @@
     # coarse approx. since a "big" eps and the non-linearities of the model
     self.assertFalse(gradcheck(tiny_func, tiny_x, eps = 0.1))
 
   def test_random_fns_are_deterministic_with_seed(self):
     for random_fn in [Tensor.randn, Tensor.uniform, Tensor.scaled_uniform, Tensor.glorot_uniform]:
       with self.subTest(msg=f"Tensor.{random_fn.__name__}"):
         Tensor.manual_seed(1337)
-        a = random_fn(10,10)
+        a = random_fn(10,10).realize()
         Tensor.manual_seed(1337)
-        b = random_fn(10,10)
+        b = random_fn(10,10).realize()
         np.testing.assert_allclose(a.numpy(), b.numpy())
 
 if __name__ == '__main__':
   unittest.main()
```

### Comparing `tinygrad-0.5.0/tinygrad/graph.py` & `tinygrad-0.6.0/tinygrad/graph.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 import os, atexit, itertools
 try:
   import networkx as nx  # type: ignore
 except ImportError:
   nx = None # graph won't work
 from collections import defaultdict
 from typing import Dict, List, Optional
-from tinygrad.ops import DeviceBuffer, UnaryOps, BinaryOps, ReduceOps, MovementOps, LoadOps, FusedOps, Op, OpType, LazyOp, get_buffers, get_lazyops
-from tinygrad.helpers import getenv, DEBUG
+from tinygrad.ops import UnaryOps, BinaryOps, ReduceOps, MovementOps, LoadOps, FusedOps, Op, OpType, LazyOp, get_buffers, get_lazyops
+from tinygrad.lazy import LazyBuffer
+from tinygrad.helpers import getenv, DEBUG, GlobalCounters
+from tinygrad.runtime.lib import RawConst
 
 GRAPH, PRUNEGRAPH, GRAPHPATH = getenv("GRAPH", 0), getenv("PRUNEGRAPH", 0), getenv("GRAPHPATH", "/tmp/net")
 
 # **** debugging and graphing ****
 
 G = nx.DiGraph() if nx is not None else None
-cnts : Dict[OpType, int] = defaultdict(int)
+cnts: Dict[OpType, int] = defaultdict(int)
+if DEBUG >= 2:
+  def print_globalcounters():
+    if GlobalCounters.time_sum_s == 0: return
+    print(f"avg: {GlobalCounters.global_ops*1e-9/GlobalCounters.time_sum_s:8.2f} GFLOPS {GlobalCounters.global_mem*1e-9/GlobalCounters.time_sum_s:8.2f} GB/s",
+          f"{' '*10}total: {GlobalCounters.kernel_count:5d} kernels {GlobalCounters.global_ops*1e-9:8.2f} GOPS {GlobalCounters.global_mem*1e-9:8.2f} GB {GlobalCounters.time_sum_s*1e3:8.2f} ms")
+  atexit.register(print_globalcounters)
 if GRAPH:
   def save_graph_exit():
     for k,v in cnts.items(): print(k, v)
     if PRUNEGRAPH: prune_graph()
     print("saving", G)
     nx.drawing.nx_pydot.write_dot(G, f'{GRAPHPATH}.dot')
     # -Gnslimit=100 can make it finish, but you won't like results
@@ -28,44 +36,46 @@
 def nm(x):
   global node_count
   if not hasattr(x, 'node_id'):
     setattr(x, 'node_id', node_count)
     node_count += 1
   return x.node_id
 
-def get_sop(op : List[Op]):
+def get_sop(op: List[Op]):
   if len(op) <= 2: return '.'.join([str(y).split(".")[1] for y in op][::-1])
-  if len(op) <= 4: return '.'.join([str(y).split(".")[1][0:2] for y in op][::-1])
+  if len(op) <= 4: return '.'.join([str(y).split(".")[1][0:3] for y in op][::-1])
   return str(len(op))
 
-def log_op(ret : DeviceBuffer, ast : LazyOp, show_graph : Optional[bool] = None):
-  if show_graph is None: show_graph = GRAPH
+def str_dtype(dtyp):
+  ret = str(dtyp)[7:]
+  return "" if ret == 'float' else f"\n{ret}"
+
+def log_op(ret: LazyBuffer, ast: LazyOp, show_graph: Optional[bool] = None, phantom=False):
+  if show_graph is None: show_graph = bool(GRAPH)
   if not DEBUG and not show_graph: return
-  op : List[Op] = [x.op for x in get_lazyops(ast)]
-  inp : List[DeviceBuffer] = get_buffers(ast)
-  if len(inp) == 1 and inp[0] == ret:
-    if show_graph and nm(ret) in G.nodes: G.nodes[nm(ret)]['style'] += ', bold'
-    return   # don't log self loops
+  op: List[Op] = [x.op for x in get_lazyops(ast)]
+  inp: List[LazyBuffer] = [x for x in get_buffers(ast) if not isinstance(x.realized, RawConst) or GRAPH > 1]
   oporder = [LoadOps, FusedOps, ReduceOps, BinaryOps, UnaryOps, MovementOps]
   optype = type(sorted(op, key=lambda x: oporder.index(type(x)))[0])
   cnts[optype] += 1
-  if DEBUG >= 4: print(f"{op} : {', '.join([f'{x.shape}-<{nm(x)}>' for x in inp])} -> {ret.shape}-<{nm(ret)}>")
+  if DEBUG >= 6: print(f"{op} : {', '.join([f'{x.shape}-<{nm(x)}>' for x in inp])} -> {ret.shape}-<{nm(ret)}>")
   if show_graph:
     top_colors = {LoadOps: '#FFFF80', UnaryOps: "#c0c0c0", ReduceOps: "#8080ff", BinaryOps: "#c0c0c0", MovementOps: "#80ff80", FusedOps: "#ff8080"}
     dashed = (optype == LoadOps and hasattr(ret, "_backing")) or (hasattr(ret, "st") and not ret.st.contiguous)  # type: ignore
 
     for x in inp:
-      G.add_edge(nm(x), nm(ret), label=get_sop(op))
+      G.add_edge(nm(x), nm(ret), label=get_sop(op), color='#00000060' if phantom else 'black')
       if 'label' not in G.nodes[nm(x)]:
-        G.nodes[nm(x)]['label'] = str(x.shape)
+        G.nodes[nm(x)]['label'] = str(x.shape)+str_dtype(ret.dtype)
     if nm(ret) not in G.nodes: G.add_node(nm(ret))
 
-    G.nodes[nm(ret)]['label'] = str(set(x.shape for x in inp))+"\n"+str(ret.shape) if optype == ReduceOps else str(ret.shape)
-    G.nodes[nm(ret)]['fillcolor'] = (top_colors[optype] + ('80' if dashed else str())) if optype in top_colors else "#ffffff"
-    G.nodes[nm(ret)]['style'] = 'filled, dashed' if dashed else 'filled'
+    G.nodes[nm(ret)]['label'] = (str(set(x.shape for x in inp))+"\n"+str(ret.shape) if optype == ReduceOps else str(ret.shape))+str_dtype(ret.dtype)
+    G.nodes[nm(ret)]['fillcolor'] = (top_colors[optype] + ('60' if phantom else ('80' if dashed else str()))) if optype in top_colors else "#ffffff"
+    G.nodes[nm(ret)]['color'] = 'white' if phantom else 'black'
+    G.nodes[nm(ret)]['style'] = ('filled, dashed' if dashed else 'filled')
     G.nodes[nm(ret)]['prunable'] = optype in [LoadOps, MovementOps]
 
 # prune movementops and loadops
 def prune_graph():
   dead_nodes = []
   for n in G.nodes:
     if 'prunable' in G.nodes[n] and G.nodes[n]['prunable']:
```

### Comparing `tinygrad-0.5.0/tinygrad/image.py` & `tinygrad-0.6.0/tinygrad/nn/image.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,97 @@
-from tinygrad.helpers import IMAGE
+import numpy as np
+from tinygrad.helpers import prod, IMAGE, ImageDType, getenv, dtypes
 from tinygrad.lazy import get_single_root
 
-def image_conv2d_decorator(normal_conv):
-  if IMAGE == 0: return normal_conv
+FLOAT16 = getenv("FLOAT16", 0)
+base_image_type = (100, 2, "imageh", np.float16) if FLOAT16 else (100, 4, "imagef", np.float32)
 
-  def image_conv2d(self, weight, bias=None, groups=1, stride=1, dilation=1, padding=0):
-    (bs,_,iy,ix), (cout,cin,H,W) = self.shape, weight.shape
-    rcout = cout//groups
-    x, w = self, weight.reshape(groups, rcout, cin, H, W)
-
-    # hack for non multiples of 4 on cin
-    if cin % 4 != 0 and not (cin == 1 and groups%4 == 0):
-      x = x.reshape(bs, groups, cin, iy, ix)   # do this always?
-      added_input_channels = 4 - (cin % 4)
-      w = w.pad(tuple((0, added_input_channels) if i == 2 else (0, 0) for i in range(len(w.shape))))
-      x = x.pad(tuple((0, added_input_channels) if i == 2 else (0, 0) for i in range(len(x.shape))))
-      cin = cin + added_input_channels
-      x = x.reshape(bs, groups*cin, iy, ix)
-
-    # hack for non multiples of 4 on rcout
-    added_output_channels = 0
-    if rcout % 4 != 0 and not (rcout == 1 and groups%4 == 0):
-      added_output_channels = 4 - (rcout % 4)
-      rcout += added_output_channels
-      cout = groups * rcout
-      w = w.slice(tuple((0, rcout) if i == 1 else (0, w.shape[i]) for i in range(len(w.shape))))
-
-    # packed (note: flipping bs and iy would make the auto-padding work)
-    x = x.permute(0,2,3,1).reshape(bs * iy, ix * groups * cin//4, 4)
-    cin_last = iy == 1 and ix == 1
-    if cin == 1: w = w.reshape(cout//4,4,H*W).permute(0,2,1)
-    elif cin_last: w = w.reshape(cout//4,4,cin//4,4,H,W).permute(0,4,2,5,1,3).reshape(cout//4, H*cin//4*W*4, 4)
-    else: w = w.reshape(cout//4,4,cin//4,4,H,W).permute(0,4,2,5,3,1).reshape(cout//4, H*cin//4*W*4, 4)
-
-    # contiguous creates the image, and early realize static weights (TODO: test for the static weight)
-    x, w = x.contiguous(), w.contiguous()
-    if get_single_root(w.lazydata).realized: w.realize()
-
-    # expand out
-    rcin_hi, rcin_lo = cin//4 if cin >= 4 else 1, 4 if cin >= 4 else 1
-    cout_expand = [groups//4 if cin == 1 else groups, 4 if cin == 1 else 1, rcout//4 if rcout >= 4 else 1, 4 if rcout >= 4 else 1]
-    x = x.reshape(bs, iy, ix, groups, rcin_hi, rcin_lo)
-    if cin_last: w = w.reshape(cout//4, H, rcin_hi, W, 4, rcin_lo)
-    else: w = w.reshape(cout//4, H, rcin_hi, W, rcin_lo, 4).permute(0,1,2,3,5,4)
-
-    # padding
-    padding_ = [padding]*4 if isinstance(padding, int) else (padding if len(padding) == 4 else [padding[1], padding[1], padding[0], padding[0]])
-    x = x.slice((None, (-padding_[2], x.shape[1]+padding_[3]), (-padding_[0], x.shape[2]+padding_[1]), None, None, None))
-
-    # prepare input
-    x = x.permute(0,3,4,5,1,2)._pool((H, W), stride, dilation) # -> (bs, groups, rcin_hi, rcin_lo, oy, ox, H, W)
-    oy, ox = x.shape[4:6]
-    x = x.permute(0,4,5,1,2,3,6,7).reshape(bs, oy, ox, *cout_expand[0:2], 1, 1, rcin_hi, rcin_lo, H, W)
-    x = x.expand(bs, oy, ox, *cout_expand, rcin_hi, rcin_lo, H, W)
-
-    # prepare weights
-    w = w.permute(0,4,2,5,1,3)
-    w = w.reshape((1, 1, 1, *cout_expand, rcin_hi, rcin_lo, H, W))
-
-    # the conv!
-    ret = (x*w).sum((-4, -3, -2, -1)).reshape(bs*oy, ox*cout//4, 4)
-    if IMAGE >= 3: ret = ret.contiguous()
-
-    # undo hack for non multiples of 4 on C.rcout
-    if added_output_channels != 0:
-      ret = ret.reshape(bs, oy, ox, groups, rcout)[:, :, :, :, :-added_output_channels]
-      rcout -= added_output_channels
-      cout = groups * rcout
-
-    # NCHW output
-    ret = ret.reshape(bs, oy, ox, cout).permute(0,3,1,2)
-    return ret if bias is None else ret.add(bias.reshape(1, -1, 1, 1))
-  return image_conv2d
+def image_dot(self, w):
+  # NOTE: we use a 1x1 conv2d to do the matmul. mxk @ kxn = (1,k,m,1).conv2d(n,k,1,1)
+  bs, groups = prod(self.shape[0:-2]), prod(w.shape[0:-2])
+  cin, cout = w.shape[-2], w.shape[-1]
+  out_shape_t = self.shape[0:-2] + (cout,-1)
+  if len(self.shape) > 1:
+    order = tuple(range(len(self.shape)-2)) + (len(self.shape)-1, len(self.shape)-2)
+  else:
+    order, out_shape_t = (0,), (cout, )
+  worder = tuple(range(len(w.shape)-2)) + (len(w.shape)-1, len(w.shape)-2)
+
+  # NOTE: with NHWC we can remove the transposes
+  # bs x groups*cin x H x W
+  cx = self.permute(order=order).reshape(shape=(bs//groups, groups*cin, -1, 1))
+  # groups*cout x cin x H, W
+  cw = w.permute(order=worder).reshape(shape=(groups*cout, cin, 1, 1))
+  return cx.conv2d(cw, groups=groups).reshape(shape=out_shape_t).permute(order=order)
+
+def image_conv2d(self, weight, bias=None, groups=1, stride=1, dilation=1, padding=0):
+  (bs,_,iy,ix), (cout,cin,H,W) = self.shape, weight.shape
+  rcout = cout//groups
+  x, w = self, weight.reshape(groups, rcout, cin, H, W)
+
+  # hack for non multiples of 4 on cin
+  if cin % 4 != 0 and not (cin == 1 and groups%4 == 0):
+    x = x.reshape(bs, groups, cin, iy, ix)   # do this always?
+    added_input_channels = 4 - (cin % 4)
+    w = w.pad(tuple((0, added_input_channels) if i == 2 else (0, 0) for i in range(len(w.shape))))
+    x = x.pad(tuple((0, added_input_channels) if i == 2 else (0, 0) for i in range(len(x.shape))))
+    cin = cin + added_input_channels
+    x = x.reshape(bs, groups*cin, iy, ix)
+
+  # hack for non multiples of 4 on rcout
+  added_output_channels = 0
+  if rcout % 4 != 0 and not (rcout == 1 and groups%4 == 0):
+    added_output_channels = 4 - (rcout % 4)
+    rcout += added_output_channels
+    cout = groups * rcout
+    w = w.slice(tuple((0, rcout) if i == 1 else (0, w.shape[i]) for i in range(len(w.shape))))
+
+  # packed (note: flipping bs and iy would make the auto-padding work)
+  x = x.permute(0,2,3,1).reshape(bs * iy, ix * groups * cin//4, 4)
+  cin_last = iy == 1 and ix == 1
+  if cin == 1: w = w.reshape(cout//4,4,H*W).permute(0,2,1)
+  elif cin_last: w = w.reshape(cout//4,4,cin//4,4,H,W).permute(0,4,2,5,1,3).reshape(cout//4, H*cin//4*W*4, 4)
+  else: w = w.reshape(cout//4,4,cin//4,4,H,W).permute(0,4,2,5,3,1).reshape(cout//4, H*cin//4*W*4, 4)
+
+  # contiguous creates the image, and early realize static weights (TODO: test for the static weight)
+  if IMAGE >= 2: x,w = x.cast(ImageDType(*base_image_type, shape=x.shape)), w.cast(ImageDType(*base_image_type, shape=w.shape))
+  x, w = x.contiguous(), w.contiguous()
+  if get_single_root(w.lazydata).realized: w.realize()
+
+  # expand out
+  rcin_hi, rcin_lo = cin//4 if cin >= 4 else 1, 4 if cin >= 4 else 1
+  cout_expand = [groups//4 if cin == 1 else groups, 4 if cin == 1 else 1, rcout//4 if rcout >= 4 else 1, 4 if rcout >= 4 else 1]
+  x = x.reshape(bs, iy, ix, groups, rcin_hi, rcin_lo)
+  if cin_last: w = w.reshape(cout//4, H, rcin_hi, W, 4, rcin_lo)
+  else: w = w.reshape(cout//4, H, rcin_hi, W, rcin_lo, 4).permute(0,1,2,3,5,4)
+
+  # padding
+  padding_ = [padding]*4 if isinstance(padding, int) else (padding if len(padding) == 4 else [padding[1], padding[1], padding[0], padding[0]])
+  x = x.slice((None, (-padding_[2], x.shape[1]+padding_[3]), (-padding_[0], x.shape[2]+padding_[1]), None, None, None))
+
+  # prepare input
+  x = x.permute(0,3,4,5,1,2)._pool((H, W), stride, dilation) # -> (bs, groups, rcin_hi, rcin_lo, oy, ox, H, W)
+  oy, ox = x.shape[4:6]
+  x = x.permute(0,4,5,1,2,3,6,7).reshape(bs, oy, ox, *cout_expand[0:2], 1, 1, rcin_hi, rcin_lo, H, W)
+  x = x.expand(bs, oy, ox, *cout_expand, rcin_hi, rcin_lo, H, W)
+
+  # prepare weights
+  w = w.permute(0,4,2,5,1,3)
+  w = w.reshape((1, 1, 1, *cout_expand, rcin_hi, rcin_lo, H, W)).expand(x.shape)
+
+  # the conv! (+ the bias)
+  ret = (x*w).cast(dtypes.float32).sum((-4, -3, -2, -1))
+
+  # reshape to image and cast back to image
+  ret = ret.reshape(bs*oy, ox*cout//4, 4)
+  if IMAGE >= 2: ret = ret.cast(ImageDType(*base_image_type, shape=ret.shape))
+  if IMAGE >= 3: ret = ret.contiguous()
+
+  # undo hack for non multiples of 4 on C.rcout
+  if added_output_channels != 0:
+    ret = ret.reshape(bs, oy, ox, groups, rcout)[:, :, :, :, :-added_output_channels]
+    rcout -= added_output_channels
+    cout = groups * rcout
+
+  # NCHW output
+  ret = ret.reshape(bs, oy, ox, cout).permute(0,3,1,2)
+  return ret if bias is None else ret.add(bias.reshape(1, -1, 1, 1))
```

### Comparing `tinygrad-0.5.0/tinygrad/jit.py` & `tinygrad-0.6.0/tinygrad/jit.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,46 +1,51 @@
 from typing import Callable, List, Tuple, Any, Dict, cast, Union
-import itertools
-from tinygrad.helpers import DEBUG, colored
+import functools, itertools
+from tinygrad.helpers import DEBUG, DType
 
 from tinygrad.lazy import Device
 from tinygrad.tensor import Tensor
-from tinygrad.ops import GlobalCounters, CompiledBuffer, RawBuffer
+from tinygrad.ops import GlobalCounters, RawBuffer
 
 class TinyJit:
   def __init__(self, fxn:Callable):
-    self.fxn : Callable = fxn
-    self.cnt : int = 0
-    self.jit_cache : List[Tuple[Callable, Any]] = []  # TODO: Any should be List[RawBuffer], but this fails
-    self.ret : Any = None
-    self.input_replace : Dict[Tuple[int, int], Union[int, str]]= {}
+    self.fxn: Callable = fxn
+    self.cnt: int = 0
+    self.jit_cache: List[Tuple[Callable, Any]] = []  # TODO: Any should be List[RawBuffer], but this fails
+    self.ret: Any = None
+    self.input_replace: Dict[Tuple[int, int], Tuple[Union[int, str], int, DType]]= {}   # (kernel_number, buffer_number) -> (input_name, expected_size, expected_type)
+
+  # add support for instance methods
+  def __get__(self, obj, objtype): return functools.partial(self.__call__, obj)
 
   def __call__(self, *args, **kwargs) -> Any:
     if Device.DEFAULT not in ["GPU", "CLANG", "METAL", "CUDA"]: return self.fxn(*args, **kwargs)  # only jit on the GPU codegen
     # NOTE: this cast is needed since although we know realize will create a ".realized" DeviceBuffer, the type checker doesn't
-    input_rawbuffers : Dict[Union[int, str], RawBuffer] = {cast(Union[int, str], k):cast(CompiledBuffer, v.realize().lazydata.realized).raw() for k,v in itertools.chain(enumerate(args), kwargs.items()) if isinstance(v, Tensor)}
+    input_rawbuffers: Dict[Union[int, str], RawBuffer] = {cast(Union[int, str], k):cast(RawBuffer, v.realize().lazydata.realized) for k,v in itertools.chain(enumerate(args), kwargs.items()) if isinstance(v, Tensor)}
     assert len(input_rawbuffers) != 0, "no inputs to JIT"
+    assert len(set(input_rawbuffers.values())) == len(input_rawbuffers), "duplicate inputs to JIT"
     if self.cnt >= 2:
-      for (j,i),idx in self.input_replace.items(): self.jit_cache[j][1][i] = input_rawbuffers[idx]
-      if DEBUG >= 2: print(colored("TOK", 'magenta').split("TOK")[0], end="")
-      for prg, args in self.jit_cache: prg(args)
-      if DEBUG >= 2: print(colored("TOK", 'magenta').split("TOK")[1], end="")
-      for (j,i),idx in self.input_replace.items(): self.jit_cache[j][1][i] = None
+      for (j,i),(input_name, expected_size, expected_type) in self.input_replace.items():
+        assert input_rawbuffers[input_name].size == expected_size and input_rawbuffers[input_name].dtype == expected_type, f"size or type mismatch in JIT, {input_rawbuffers[input_name]} != <{expected_size}, {expected_type}>"
+        self.jit_cache[j][1][i] = input_rawbuffers[input_name]
+      for prg, args in self.jit_cache: prg(args, jit=True)
+      for (j,i) in self.input_replace.keys(): self.jit_cache[j][1][i] = None
     elif self.cnt == 1:
       GlobalCounters.cache = []
       self.ret = self.fxn(*args, **kwargs)
       self.jit_cache = GlobalCounters.cache
       GlobalCounters.cache = None
       assert len(self.jit_cache) != 0, "didn't JIT anything!"
       if DEBUG >= 1: print(f"JIT captured {len(self.jit_cache)} kernels with {len(input_rawbuffers)} inputs")
 
       # get the inputs for replacement
       for j,(prg,args) in enumerate(self.jit_cache):  # pylint: disable=E1133
         for i,a in enumerate(args):
           if a in input_rawbuffers.values():
-            self.input_replace[(j,i)] = [k for k,v in input_rawbuffers.items() if v == a][0]
-      assert set(self.input_replace.values()) == set(input_rawbuffers.keys()), "some input tensors not found"
-      for (j,i),idx in self.input_replace.items(): self.jit_cache[j][1][i] = None
+            self.input_replace[(j,i)] = [(k, v.size, v.dtype) for k,v in input_rawbuffers.items() if v == a][0]
+        #if prg.local_size is None: prg.local_size = prg.optimize_local_size(args, preserve_output=True)  # the JIT can optimize local
+      assert set([x[0] for x in self.input_replace.values()]) == set(input_rawbuffers.keys()), "some input tensors not found"
+      for (j,i) in self.input_replace.keys(): self.jit_cache[j][1][i] = None
     elif self.cnt == 0:
       self.ret = self.fxn(*args, **kwargs)
     self.cnt += 1
     return self.ret
```

### Comparing `tinygrad-0.5.0/tinygrad/lazy.py` & `tinygrad-0.6.0/tinygrad/lazy.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,67 +1,53 @@
 from __future__ import annotations
-from typing import Optional, Tuple, Union, List, Dict, Any, ClassVar, Type
-import os, sys, weakref, importlib, inspect, functools
+from typing import Optional, Tuple, Union, List, Dict, Any, cast
+import sys, weakref, importlib, inspect, functools, pathlib
 from weakref import WeakValueDictionary
-from tinygrad.helpers import prod, getenv
-from tinygrad.shape import ShapeTracker, get_contraction
-from tinygrad.ops import DeviceBuffer, UnaryOps, BinaryOps, ReduceOps, MovementOps, LoadOps, OpType, LazyOp, get_buffers, get_lazyops, map_buffers
-from tinygrad.graph import log_op
+from tinygrad.helpers import prod, getenv, DType, dtypes, LazyNumpyArray, flatten, ImageDType
+from tinygrad.shape.shapetracker import ShapeTracker, get_contraction
+from tinygrad.ops import Compiled, Interpreted, UnaryOps, BinaryOps, ReduceOps, MovementOps, LoadOps, OpType, LazyOp, get_lazyops, get_buffers, map_buffers
+from tinygrad.runtime.lib import RawConst, RawBuffer
 
 # lazy can recurse a lot
 sys.setrecursionlimit(10000)
 
 OPT = getenv("OPT", 2)
 LAZY = getenv("LAZY", 1)
 
-def get_buffer(name, base='tinygrad.runtime'):
-  try:
-    return [cls for cname, cls in inspect.getmembers(importlib.import_module(f'{base}.ops_{name}'), inspect.isclass) if (cname.lower() == name + "buffer")][0]
-  except Exception as e:  # NOTE: this can't be put on one line due to mypy issue
-    print(name, "backend not available", e, file=sys.stderr)
-
-class _Device:
-  def __init__(self) -> None:
-    self._buffers : Dict[str, Type[DeviceBuffer]] = {x.upper():get_buffer(x) for x in
-      [os.path.splitext(x)[0][len("ops_"):] for x in sorted(os.listdir(os.path.join(os.path.dirname(os.path.realpath(__file__)), "runtime"))) if x.startswith("ops_")] if x is not None}
-    self.DEFAULT : str = "CPU"
-    for name in self._buffers:
-      if getenv(name) == 1: self.DEFAULT = name  # note: DEFAULT can be a Device that can't be imported. better than silent use of a different device
-      if self._buffers[name] is not None: self.__setattr__(name, name)
-Device = _Device()
-
 # TODO: movement ops that only change shape are really nops. treat them as such
-REMOVE_MOVEMENT_NOPS, MERGE_UNARY_OPS, MERGE_ELEMENTWISE_INTO_REDUCE, SHUFFLE_MOVEMENT_OPS = OPT>=1, OPT>=1, OPT>=1, OPT>=1
-MERGE_ELEMENTWISE_OPS, MERGE_ONE_REDUCE_INTO_ELEMENTWISE = OPT>=2, OPT>=2
+REMOVE_MOVEMENT_NOPS, MERGE_ELEMENTWISE_INTO_REDUCE, SHUFFLE_MOVEMENT_OPS, MERGE_ELEMENTWISE_OPS = OPT>=1, OPT>=1, OPT>=1, OPT>=1
+MERGE_ONE_REDUCE_INTO_ELEMENTWISE, SHUFFLE_PAD_OPS = OPT>=2, OPT>=2   # shuffle pad ops is fine now since we only push to merge binops
 PUSH_PERMUTES, PUSH_CONTIGUOUS = OPT>=3, OPT>=3
 
 # **** realize functions ****
 def _ast_reduceops(self:LazyBuffer) -> LazyOp:
   # TODO: this can also corealize a binary op after the reduce, not just before
   src = self.op.src[0]
   if MERGE_ELEMENTWISE_INTO_REDUCE and src.realized is None and src.optype == BinaryOps and len(src.children) <= 1:
     src = src.op
   return LazyOp(self.op.op, (src,), self.op.arg)
 
 # this supports late merging an upstream Reduce op and even an Elementwise op above that
 def _ast_binaryops(self:LazyBuffer) -> LazyOp:
-  real_srcs : Dict[LazyBuffer, Union[None, LazyOp, LazyBuffer]] = {x:None for x in get_buffers(self.op)}
+  real_srcs: Dict[LazyBuffer, Union[None, LazyOp, LazyBuffer]] = {x:None for x in get_buffers(self.op)}
   # NOTE: contiguous does not always mean the same size with SHRINK. this is still mergeable but requires more thought how
-  psrcs : List[Tuple[LazyBuffer, LazyBuffer]] = [(k,x) for k,x in zip(real_srcs.keys(), map(get_movementroot_contiguous, real_srcs.keys())) if x.optype == ReduceOps and x.realized is None and prod(k.shape) == prod(x.shape) and len(x.children) <= 1 and len(k.children) <= 1]
-  intermediate_shape : Tuple[int, ...] = self.shape
+  # TODO: this can also support late fusion of BinaryOps, required for test_fold_conv_sgd
+  psrcs: List[Tuple[LazyBuffer, LazyBuffer]] = [(k,x) for k,x in zip(real_srcs.keys(), map(get_movementroot_contiguous, real_srcs.keys())) if x.optype == ReduceOps and x.realized is None and prod(k.shape) == prod(x.shape) and len(x.children) <= 1 and len(k.children) <= 1]
+  intermediate_shape: Tuple[int, ...] = self.shape
   if len(psrcs) == 1 and MERGE_ONE_REDUCE_INTO_ELEMENTWISE:
-    if psrcs[0][1].optype == ReduceOps:
-      top = _ast_reduceops(psrcs[0][1])
-    real_srcs[psrcs[0][0]] = top
+    psrc = psrcs[0] # NOTE: right now we can't handle multiple, as we'd have to check for loop
+    if psrc[1].optype == ReduceOps:
+      top = _ast_reduceops(psrc[1])
+    real_srcs[psrc[0]] = top
     real_srcs.update({x:x for x in get_buffers(top)})  # the reduce op buffers are not modified
 
     # if the ReduceOp is followed by a reshape, we push this reshape before all the ElementwiseOp inputs
-    if psrcs[0][0].shape != psrcs[0][1].shape:
-      intermediate_shape = psrcs[0][1].shape
-      assert psrcs[0][0].shape == self.shape, f"shape mismatch {psrcs[0][0].shape} != {self.shape}"
+    if psrc[0].shape != psrc[1].shape:
+      intermediate_shape = psrc[1].shape
+      assert psrc[0].shape == self.shape, f"shape mismatch {psrc[0].shape} != {self.shape}"
 
   # reshape all the late ops into the output shape
   # NOTE: these RESHAPEs will return self if they don't change the shape
   for x in real_srcs.keys():
     if real_srcs[x] is None: real_srcs[x] = x.movement_op(MovementOps.RESHAPE, intermediate_shape)
   ast = map_buffers(real_srcs, self.op)
   return LazyOp(MovementOps.RESHAPE, (ast, ), self.shape) if intermediate_shape != self.shape else ast
@@ -69,180 +55,248 @@
 # **** lazy operations ****
 
 def get_weakop(op:LazyOp) -> LazyOp: return LazyOp(op.op, tuple(get_weakop(x) if isinstance(x, LazyOp) else weakref.ref(x) for x in op.src), op.arg)
 def get_single_root(root:LazyBuffer) -> LazyBuffer: return get_single_root(root.op.src[0]) if getattr(root, 'op', None) and len(root.op.src) == 1 else root
 def get_movementroot(root:LazyBuffer, allow_contiguous=False) -> LazyBuffer: return get_movementroot(root.op.src[0], allow_contiguous) if root.realized is None and (root.optype == MovementOps or (root.op.op == LoadOps.CONTIGUOUS and allow_contiguous and root.op.src[0].st.contiguous)) else root
 def get_movementroot_contiguous(x:LazyBuffer) -> LazyBuffer: return get_movementroot_contiguous(x.op.src[0]) if x.realized is None and x.op.op == LoadOps.CONTIGUOUS else (get_movementroot(x, True) if x.optype == MovementOps and x.st.contiguous else x)
 
-def replace_with_movement_op(y:Union[LazyOp, LazyBuffer], op:MovementOps, arg:Tuple[Any, ...]) -> LazyBuffer:
-  if isinstance(y, LazyBuffer): return y.movement_op(op, arg)
+def replace_with_movement_ops(y:Union[LazyOp, LazyBuffer], ops:List[Tuple[MovementOps, Tuple[Any, ...]]]) -> LazyBuffer:
+  if isinstance(y, LazyBuffer):
+    for op, arg in ops: y = y.movement_op(op, arg)
+    return y
   assert y.op in BinaryOps or y.op in UnaryOps
-  return elementwise_op(y.op, *[replace_with_movement_op(z, op, arg) for z in y.src])   # type: ignore
+  return elementwise_op(y.op, *[replace_with_movement_ops(z, ops) for z in y.src], arg=y.arg)   # type: ignore
+
+lazycache: WeakValueDictionary[Tuple[str, DType, OpType, LazyOp], LazyBuffer] = WeakValueDictionary()
+def create_lazybuffer(device:str, shape:Union[ShapeTracker, Tuple[int, ...]], optype:OpType, op:LazyOp, dtype:DType):
+  st = shape if isinstance(shape, ShapeTracker) else ShapeTracker(tuple(shape))
+
+  # fromcpu aren't cached
+  if optype == LoadOps and op.op == LoadOps.FROMCPU: return LazyBuffer(device, st, optype, op, dtype)
+
+  #print("create_lazybuffer", device, shape, optype, op, dtype)
+
+  # NOTE: shape should be deterministic. annoying to cache with the ShapeTracker
+  # get_weakop makes all the LazyBuffers in the op have a weakref
+  wop = (device, dtype, optype, get_weakop(op))
+
+  if wop not in lazycache: lazycache[wop] = ret = LazyBuffer(device, st, optype, op, dtype)
+  else: ret = lazycache[wop]
+  return ret
 
-def support_weakref(x): return x
-@support_weakref  # needed for mypyc, this prevents LazyBuffer from becoming a native class
 class LazyBuffer:
   __deletable__ = ('op',)
-  lazycache : ClassVar[WeakValueDictionary[Tuple[str, OpType, LazyOp], LazyBuffer]] = WeakValueDictionary()
-  def __new__(cls, device:str, shape:Union[ShapeTracker, Tuple[int, ...]], optype:OpType, op:LazyOp):
-    # fromcpu aren't cached
-    if optype == LoadOps and op.op == LoadOps.FROMCPU:
-      return super().__new__(cls)
-    wop = (device, optype, get_weakop(op))   # NOTE: shape should be deterministic. annoying to cache with the ShapeTracker
-    # NOTE: we need "ret" to prevent the new buffer from being immediately deleted
-    if wop not in LazyBuffer.lazycache: LazyBuffer.lazycache[wop] = ret = super().__new__(cls)
-    else: ret = LazyBuffer.lazycache[wop]
-    return ret
-
-  def __init__(self, device:str, shape:Union[ShapeTracker, Tuple[int, ...]], optype:OpType, op:LazyOp):
-    if hasattr(self, 'device'):
-      return  # cache hit, we return and don't reinit
-    self.st = shape if isinstance(shape, ShapeTracker) else ShapeTracker(tuple(shape))
-    self.shape, self.optype, self.op = self.st.shape, optype, op
-    self.realized : Optional[DeviceBuffer] = None
-    self.output_buffer : Optional[DeviceBuffer] = None
-    self.device, self.dbuffer = device, Device._buffers[device]
+  def __init__(self, device:str, st:ShapeTracker, optype:OpType, op:LazyOp, dtype:DType):
+    self.st = st  # NOTE: this is not a copy! this should be a "read-only" ShapeTracker
+    self.device, self.shape, self.optype, self.dtype = device, self.st.shape, optype, dtype
+    self.op: LazyOp = op
+    self.realized: Optional[RawBuffer] = None
+    self.output_buffer: Optional[RawBuffer] = None   # TODO: do we really need this? or can we just use realized
     # TODO: does children have to be a ref count instead of a set? can a Buffer be a double child?
-    self.children : weakref.WeakSet[LazyBuffer] = weakref.WeakSet()
+    self.children: weakref.WeakSet[LazyBuffer] = weakref.WeakSet()
     # NOTE: op should be read only after construction of LazyBuffer
     for x in get_buffers(op): x.children.add(self)
     if not LAZY: self.realize()
 
-  def __repr__(self): return f"<LB {self.shape} op:{self.op.op if self.realized is None else 'realized'}>"
+    # log phantom ops to the graph
+    from tinygrad.graph import log_op, GRAPH
+    if GRAPH >= 3: log_op(self, self.op, phantom=True)
+
+  def __repr__(self): return f"<LB {self.shape} {self.dtype} op:{self.op.op if self.realized is None else self.realized} st:{self.st}>"
+  def _device_extra_args(self) -> Dict[str, int]: return {"device": int(self.device.split(":")[1])} if ":" in self.device else {}
 
-  # this produces a device buffer
-  def realize(self:LazyBuffer, required_device=None) -> DeviceBuffer:
-    assert required_device is None or required_device == self.device
+  def realize(self:LazyBuffer) -> LazyBuffer:
     if self.realized is None:
       # get real ops first
       if self.op.op == LoadOps.FROMCPU:
-        self.realized = Device._buffers[self.device].fromCPU(self.op.arg)
-        ast = LazyOp(self.op.op, tuple())
+        if prod(self.op.arg.shape) == 1 and hasattr(Device[self.device].codegen, 'supports_constant_folding'):
+          self.realized = RawConst(1, dtypes.from_np(self.op.arg.dtype), self.op.arg().flatten()[0])
+        else:
+          self.realized = Device[self.device].buffer.fromCPU(self.op.arg(), **self._device_extra_args())
       elif self.op.op == LoadOps.CONTIGUOUS:
-        real_src = self.op.src[0].realize(self.device)
-        self.realized = real_src.contiguous()
-        ast = LazyOp(self.op.op, (real_src, ))
-      elif self.optype == MovementOps:
-        src = self.op.src[0]
-
-        # fuse RESHAPE and ReduceOps
-        if src.realized is None and src.optype == ReduceOps and self.op.op == MovementOps.RESHAPE and len(src.children) <= 1:
-          # it's okay to add a RESHAPE to the ast here
-          ast = LazyOp(MovementOps.RESHAPE, (_ast_reduceops(src), ), self.op.arg)
+        realized = self.op.src[0].realize().realized
+        if self.op.src[0].st.contiguous and not isinstance(realized, RawConst) and realized.size == prod(self.shape):
+          # no need to run an AST, this is already contiguous
+          self.realized = realized
         else:
-          # movement ops aren't an AST, just run them
-          real_src = src.realize(self.device)
-          self.realized = real_src.movement_op(self.op.op, self.op.arg)
-          ast = LazyOp(self.op.op, (real_src, ))
-      elif self.optype == ReduceOps: ast = _ast_reduceops(self)
-      elif self.optype == BinaryOps: ast = _ast_binaryops(self)
-
-      # no need to keep the op after realization
-      del self.op
+          # TODO: remove UnaryOps.NOOP, replace with LoadOps.CONTIGUOUS. confusing with Compiled though
+          self.op = LazyOp(UnaryOps.NOOP, self.op.src)
+      elif self.op.op == LoadOps.CUSTOM:
+        # this needs to immediately realize
+        self.realized = self.op.arg(self, *[x.realize() for x in self.op.src])
+      # these can be late folded and change the op to go further back in the graph
+      elif self.optype == ReduceOps: self.op = _ast_reduceops(self)
+      elif self.optype == BinaryOps: self.op = _ast_binaryops(self)  # ISSUE: this can include a reshape
 
       # run the ast if we still have to, and log the op
       if self.realized is None:
-        ast = map_buffers({x:x.realize(self.device) for x in get_buffers(ast)}, ast)
-        self.realized = self.dbuffer.exec_ast(ast, output_buffer=self.output_buffer)
-      log_op(self.realized, ast)
-
-    assert self.realized.shape == self.shape, f"shape mismatch on realize {self.realized.shape} vs {self.shape}"
-    assert isinstance(self.realized, Device._buffers[self.device])
-    return self.realized
+        for x in get_buffers(self.op): x.realize()
+
+        # HACK: image shape can be wrong, hot cast it back to a normal float
+        if self.optype != MovementOps and isinstance(self.dtype, ImageDType) and (prod(self.shape) != prod(self.dtype.shape) or not any(self.shape[x]%4 == 0 for x in self.st.unit_stride_axes())):
+          if self.op.op == MovementOps.RESHAPE:
+            # put CAST before the final RESHAPE
+            self.op = LazyOp(MovementOps.RESHAPE, (LazyOp(UnaryOps.CAST, self.op.src, dtypes.float32),), self.op.arg)
+          else:
+            self.op = LazyOp(UnaryOps.CAST, (self.op,), dtypes.float32)
+          self.dtype = dtypes.float32
+
+        self.realized = Device[self.device].exec_ast(self.op, output=self, **self._device_extra_args())
+
+      assert isinstance(self.realized, (RawConst, Device[self.device].buffer)), f"device mismatch on realized got {type(self.realized)} expected {self.device}"
+      # HACK: allow hot casting of images
+      assert self.realized.dtype == self.dtype or self.dtype.name.startswith("image"), f"dtype mismatch on realize got {self.realized.dtype} expected {self.dtype}"
+      self.dtype = self.realized.dtype
+
+      # log to the graph
+      from tinygrad.graph import log_op, GRAPH
+      if not isinstance(self.realized, RawConst) or GRAPH >= 2: log_op(self, self.op)
+
+      # no need to keep the op after realization
+      del self.op
+    return self
 
+  # NOTE: we have to make a copy of the numpy array here in case the user changes it. expose this? LazyNumpyArray doesn't have this problem
   @staticmethod
-  def fromCPU(x, device) -> LazyBuffer: return LazyBuffer(device, x.shape, LoadOps, LazyOp(LoadOps.FROMCPU, tuple(), x.copy()))
-  def toCPU(self): return self.realize().toCPU()
+  def fromCPU(x:LazyNumpyArray, device) -> LazyBuffer:
+    return create_lazybuffer(device, x.shape, LoadOps, LazyOp(LoadOps.FROMCPU, tuple(), x), dtypes.from_np(x.dtype))
 
+  # create a constant with the shape and dtype of self
+  def const_like(self, val) -> LazyBuffer:
+    return create_lazybuffer(self.device, (1,), LoadOps, LazyOp(LoadOps.FROMCPU, tuple(), LazyNumpyArray([val], (1,), self.dtype.np)), self.dtype) \
+      .movement_op(MovementOps.RESHAPE, (1,)*len(self.shape)).movement_op(MovementOps.EXPAND, self.shape)
+
+  # NOTE: we also have to copy the numpy array on the way out...otherwise the underlying Tensor could be freed and use after free. improve this?
+  def toCPU(self):
+    realized = self.cast(dtypes.from_np(self.dtype.np)).contiguous().realize().realized
+    ret = cast(RawBuffer, realized).toCPU().reshape(self.shape)
+    return ret
+
+  def cast(self:LazyBuffer, arg:DType) -> LazyBuffer: return elementwise_op(UnaryOps.CAST, self, arg=arg) if self.dtype != arg else self
   def unary_op(self:LazyBuffer, op:UnaryOps) -> LazyBuffer: return elementwise_op(op, self)
   def binary_op(self:LazyBuffer, op:BinaryOps, y:LazyBuffer) -> LazyBuffer: return elementwise_op(op, self, y)
-  def contiguous(self:LazyBuffer) -> LazyBuffer: return LazyBuffer(self.device, self.shape, LoadOps, LazyOp(LoadOps.CONTIGUOUS, (self,)))
+  def contiguous(self:LazyBuffer) -> LazyBuffer:
+    if self.realized is None and self.op.op == LoadOps.CONTIGUOUS: return self  # two CONTIGUOUS in a row is one
+    return create_lazybuffer(self.device, self.shape, LoadOps, LazyOp(LoadOps.CONTIGUOUS, (self,)), self.dtype)
 
   def reduce_op(self:LazyBuffer, op:ReduceOps, new_shape:Tuple[int, ...]) -> LazyBuffer:
     if self.shape == tuple(new_shape): return self
-    reduce = list(enumerate(zip(self.shape, new_shape)))
-    # move the reduce axes to the end
-    x = self.movement_op(MovementOps.PERMUTE, tuple([i for i,(s,n) in reduce if s == n] + [i for i,(s,n) in reduce if s != n]))
-    new_tmp_shape = tuple([n for _,(s,n) in reduce if s == n] + [n for _,(s,n) in reduce if s != n])
-    # NOTE: this reshape can only move around 1s
-    return LazyBuffer(x.device, new_tmp_shape, ReduceOps, LazyOp(op, (x,), new_tmp_shape)).movement_op(MovementOps.RESHAPE, new_shape)
+    srcs = _push_movement_ops((self,)) if SHUFFLE_MOVEMENT_OPS else (self,)
+    return create_lazybuffer(self.device, new_shape, ReduceOps, LazyOp(op, tuple(srcs), new_shape), self.dtype)
 
+  # shrink -> stride -> permute -> reshape -> pad -> expand
   def movement_op(self:LazyBuffer, op:MovementOps, arg:Tuple[Any, ...]) -> LazyBuffer:
     # very instant nop
     if op == MovementOps.RESHAPE and self.shape == arg: return self
 
     # TODO: look into why that copy is needed
     local_st = ShapeTracker(self.shape).movement_op(op, arg)
 
     # instant nops
     if local_st.contiguous and self.shape == local_st.shape: return self
 
     # two ops in a row is one op. merge them if unresolved
     if self.realized is None and self.op.op == op:
       # TODO: why is deleting self from children needed? shouldn't GC do it?
       self.op.src[0].children.discard(self)
-      if op in [MovementOps.RESHAPE, MovementOps.EXPAND, MovementOps.SHRINK]: return self.op.src[0].movement_op(op, arg)
+      if op in [MovementOps.RESHAPE, MovementOps.EXPAND]: return self.op.src[0].movement_op(op, arg)
+      if op == MovementOps.SHRINK: return self.op.src[0].movement_op(op, tuple((b1+b2, b1+e2) for (b1,e1),(b2,e2) in zip(self.op.arg, arg)))
       if op == MovementOps.PERMUTE: return self.op.src[0].movement_op(op, tuple(self.op.arg[i] for i in arg))
       if op == MovementOps.PAD: return self.op.src[0].movement_op(op, tuple((b1+b2, e1+e2) for (b1,e1),(b2,e2) in zip(self.op.arg, arg)))
-      if op == MovementOps.FLIP: return self.op.src[0].movement_op(op, tuple(i for i in arg+self.op.arg if not (i in arg and i in self.op.arg)))
+      if op == MovementOps.STRIDE: return self.op.src[0].movement_op(op, tuple(i*j for i,j in zip(arg, self.op.arg)))
 
     # push permutes before reduce ops
     if op == MovementOps.PERMUTE and PUSH_PERMUTES and self.realized is None and self.optype == ReduceOps:
       # reduceops have one buffer input, permute it
       narg = tuple(self.op.arg[arg[i]] for i in range(len(arg)))
       src, rop = self.op.src[0], self.op.op
       src.children.discard(self)
       del self  # TODO: why doesn't this delete remove it from the children
       return src.movement_op(op, arg).reduce_op(rop, narg)
 
     # some permutes are actually just reshapes
     if op == MovementOps.PERMUTE and local_st.contiguous: return self.movement_op(MovementOps.RESHAPE, tuple(self.shape[i] for i in arg))
 
-    # move permutes before expands
-    if op == MovementOps.PERMUTE and PUSH_PERMUTES and self.realized is None and self.op.op == MovementOps.EXPAND:
+    # move permutes before expands (always, this is safe)
+    if op == MovementOps.PERMUTE and self.realized is None and self.op.op == MovementOps.EXPAND:
       self.op.src[0].children.discard(self)
       return self.op.src[0].movement_op(MovementOps.PERMUTE, arg).movement_op(MovementOps.EXPAND, tuple(self.op.arg[a] for a in arg))
 
     # move permutes before reshapes if we can
     if op == MovementOps.PERMUTE and PUSH_PERMUTES and self.realized is None and self.op.op == MovementOps.RESHAPE and isinstance(self.op.src[0], LazyBuffer):
       if shape_idx_groups := get_contraction(self.op.src[0].shape, self.shape):
-        new_arg : List[int] = functools.reduce(lambda r, x: r + shape_idx_groups[x], arg, [])
         self.op.src[0].children.discard(self)   # this changes nothing?
-        return self.op.src[0].movement_op(MovementOps.PERMUTE, tuple(new_arg)) \
+        return self.op.src[0].movement_op(MovementOps.PERMUTE, tuple(flatten(shape_idx_groups[i] for i in arg))) \
           .movement_op(MovementOps.RESHAPE, ShapeTracker(self.st).movement_op(op, arg).shape)
 
     # if this MovementOp is being applied to a BinaryOp, apply the MovementOp to all the BinaryOp inputs instead. NOTE: UnaryOps is never an OpType
-    if SHUFFLE_MOVEMENT_OPS and self.optype == BinaryOps and self.realized is None and len(self.children) == 0 and op != MovementOps.EXPAND and (op != MovementOps.PAD or all(x.op != BinaryOps.DIV for x in get_lazyops(self.op))):
-      return replace_with_movement_op(self.op, op, arg)
+    if SHUFFLE_MOVEMENT_OPS and self.optype == BinaryOps and self.realized is None and (op in [MovementOps.SHRINK, MovementOps.STRIDE, MovementOps.PERMUTE] or (op == MovementOps.RESHAPE and self.op.op in UnaryOps)) and len(self.children) == 0: # and op != MovementOps.EXPAND and (op != MovementOps.PAD or (SHUFFLE_PAD_OPS and all(x.op != BinaryOps.DIV for x in get_lazyops(self.op)))):
+      return replace_with_movement_ops(self.op, [(op, arg)])
 
     # create the buffer
-    ret = LazyBuffer(self.device, ShapeTracker(self.st).movement_op(op, arg), MovementOps, LazyOp(op, (self,), arg))
+    ret = create_lazybuffer(self.device, ShapeTracker(self.st).movement_op(op, arg), MovementOps, LazyOp(op, (self,), arg), self.dtype)
 
     # if the ShapeTracker becomes contiguous, replace the whole thing with a reshape (or nothing if shapes match)
     # NOTE: if ret is in the cache, it can already be realized
     if REMOVE_MOVEMENT_NOPS and ret.realized is None and self.realized is None and ret.st.contiguous:
       # MovementOps aren't stacked any more, they each have one parent, find the root
       root = get_movementroot(self)
       if root.st.contiguous and root != self and prod(ret.st.shape) == prod(root.shape):
         return root.movement_op(MovementOps.RESHAPE, ret.st.shape)
 
     return ret
 
-def elementwise_op(op:Union[UnaryOps, BinaryOps], *srcs:LazyBuffer) -> LazyBuffer:
-  out_device, out_shape = srcs[0].device, srcs[0].shape
+def _push_movement_ops(srcs:Tuple[LazyBuffer, ...]) -> Tuple[LazyBuffer, ...]:
+  new_srcs = []
+  for x in srcs:
+    mops: List[Tuple[MovementOps, Tuple[Any, ...]]] = []
+    bx = x
+    # backwalk all the movement ops. don't push PAD or EXPAND
+    while bx.realized is None and bx.optype == MovementOps and bx.op.op != MovementOps.EXPAND and (bx.op.op != MovementOps.PAD or SHUFFLE_PAD_OPS) and len(bx.children) <= 1:
+      assert isinstance(bx.op.op, MovementOps)
+      mops.append((bx.op.op, bx.op.arg))
+      bx = bx.op.src[0]
+    # NOTE: can't push pads with a div
+    if bx.realized is None and bx.optype == BinaryOps and len(bx.children) <= 1 and len(mops) and (all(x[0] != MovementOps.PAD for x in mops) or all(x.op != BinaryOps.DIV for x in get_lazyops(bx.op))):
+      new_srcs.append(replace_with_movement_ops(bx.op, mops[::-1]))
+    else:
+      new_srcs.append(x)
+  return tuple(new_srcs)
+
+def elementwise_op(op:Union[UnaryOps, BinaryOps], *srcs:LazyBuffer, arg:Optional[Any]=None) -> LazyBuffer:
+  # if we are separated from other binary ops by movement ops, we push those movement ops above those binaryops
+  if SHUFFLE_MOVEMENT_OPS: srcs = _push_movement_ops(srcs)
+
+  # get outputs now
+  out_device, out_shape, out_dtype = srcs[0].device, srcs[0].shape, max(x.dtype for x in srcs) if op != UnaryOps.CAST else cast(DType, arg)
 
   # push all contiguous to the end of BinaryOps. kernels 198 -> 196
   if PUSH_CONTIGUOUS and any(x.realized is None and x.op.op == LoadOps.CONTIGUOUS and len(x.op.src[0].children) <= 1 for x in srcs):
     new_srcs = []
     for x in srcs:
       if x.realized is None and x.op.op == LoadOps.CONTIGUOUS and len(x.op.src[0].children) <= 1:
         x.op.src[0].children.discard(x)
         new_srcs.append(x.op.src[0])
       else:
         new_srcs.append(x)
-    return elementwise_op(op, *new_srcs).contiguous()
+    return elementwise_op(op, *new_srcs, arg=arg).contiguous()
 
-  if MERGE_ELEMENTWISE_OPS or (MERGE_UNARY_OPS and len(set(srcs)) == 1):
+  if MERGE_ELEMENTWISE_OPS:
     # remove the buffers from any (childless) BinaryOps that feed into this
     srcs = tuple(x.op if x.optype == BinaryOps and len(x.children) == 0 and x.realized is None else x for x in srcs)  # type: ignore
 
-  return LazyBuffer(out_device, out_shape, BinaryOps, LazyOp(op, srcs))
+  return create_lazybuffer(out_device, out_shape, BinaryOps, LazyOp(op, srcs, arg), out_dtype)
+
+class _Device:
+  def __init__(self) -> None:
+    self._buffers: List[str] = [x.stem[len("ops_"):].upper() for x in (pathlib.Path(__file__).parent/"runtime").iterdir() if x.stem.startswith("ops_")]
+    self.DEFAULT: str = functools.reduce(lambda val, ele: ele if getenv(ele) == 1 else val, self._buffers, self._default_device())
+  def __getitem__(self, x:str) -> Union[Interpreted, Compiled]: return self._get_device(x.split(":")[0].upper())
+  @functools.lru_cache(maxsize=None)  # this class is a singleton, pylint: disable=method-cache-max-size-none
+  def _get_device(self, x:str) -> Union[Interpreted, Compiled]: return [cls for cname, cls in inspect.getmembers(importlib.import_module(f'tinygrad.runtime.ops_{x.lower()}')) if (cname.lower() == x.lower() + "buffer") and x in self._buffers][0]
+  def _default_device(self) -> str:
+    for device in ["METAL", "CUDA", "GPU"]:
+      try:
+        if self[device]: return device
+      except Exception: pass
+    return "CPU"
+Device = _Device()
```

### Comparing `tinygrad-0.5.0/tinygrad/nn/__init__.py` & `tinygrad-0.6.0/tinygrad/nn/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,85 +1,83 @@
 from typing import Optional, Union, Tuple
 from tinygrad.tensor import Tensor
 
 class BatchNorm2d:
   def __init__(self, sz, eps=1e-5, affine=True, track_running_stats=True, momentum=0.1):
-    assert affine, "BatchNorm2d is only supported with affine"
     self.eps, self.track_running_stats, self.momentum = eps, track_running_stats, momentum
 
-    self.weight, self.bias = Tensor.ones(sz), Tensor.zeros(sz)
+    if affine: self.weight, self.bias = Tensor.ones(sz), Tensor.zeros(sz)
+    else: self.weight, self.bias = None, None
 
     self.running_mean, self.running_var = Tensor.zeros(sz, requires_grad=False), Tensor.ones(sz, requires_grad=False)
     self.num_batches_tracked = Tensor.zeros(1, requires_grad=False)
 
   def __call__(self, x:Tensor):
     if Tensor.training:
       # This requires two full memory accesses to x
       # https://github.com/pytorch/pytorch/blob/c618dc13d2aa23625cb0d7ada694137532a4fa33/aten/src/ATen/native/cuda/Normalization.cuh
       # There's "online" algorithms that fix this, like https://en.wikipedia.org/wiki/Algorithms_for_calculating_variance#Welford's_Online_algorithm
-      x_detached = x.detach()
-      batch_mean = x_detached.mean(axis=(0,2,3))
-      y = (x_detached - batch_mean.reshape(shape=[1, -1, 1, 1]))
+      batch_mean = x.mean(axis=(0,2,3))
+      y = (x - batch_mean.reshape(shape=[1, -1, 1, 1]))
       batch_var = (y*y).mean(axis=(0,2,3))
       batch_invstd = batch_var.add(self.eps).pow(-0.5)
-      self.batch_invstd = None
 
       # NOTE: wow, this is done all throughout training in most PyTorch models
       if self.track_running_stats:
-        self.running_mean.assign((1 - self.momentum) * self.running_mean + self.momentum * batch_mean)
-        self.running_var.assign((1 - self.momentum) * self.running_var + self.momentum * batch_var)
+        self.running_mean.assign((1 - self.momentum) * self.running_mean + self.momentum * batch_mean.detach())
+        self.running_var.assign((1 - self.momentum) * self.running_var + self.momentum * batch_var.detach())
         self.num_batches_tracked += 1
     else:
-      batch_mean, batch_var = self.running_mean, self.running_var
-      # NOTE: this can be precomputed for static inference. if you manually update running_var, you have to reset this
-      if not hasattr(self, "batch_invstd") or not self.batch_invstd:
-        self.batch_invstd = batch_var.add(self.eps).pow(-0.5)
-      batch_invstd = self.batch_invstd
+      batch_mean = self.running_mean
+      # NOTE: this can be precomputed for static inference. we expand it here so it fuses
+      batch_invstd = self.running_var.reshape(1, -1, 1, 1).expand(x.shape).add(self.eps).rsqrt()
 
     return x.batchnorm(self.weight, self.bias, batch_mean, batch_invstd)
 
 # TODO: is this good weight init?
 class Conv2d:
-  def __init__(self, in_channels, out_channels, kernel_size, stride=1, padding=0, bias=True):
-    self.kernel_size = (kernel_size, kernel_size) if isinstance(kernel_size, int) else (kernel_size[0], kernel_size[1])
-    self.stride = (stride, stride) if isinstance(stride, int) else (stride[0], stride[1])
-    self.padding = (padding, ) * 4 if isinstance(padding, int) else ((padding[0], padding[0], padding[1], padding[1]) if len(padding) == 2 else padding)
-    # TODO: why is this realize needed? shouldn't it realize on the first run?
-    self.weight = Tensor.glorot_uniform(out_channels, in_channels, self.kernel_size[0], self.kernel_size[1]).realize()
-    self.bias = Tensor.zeros(out_channels).contiguous().realize() if bias else None
+  def __init__(self, in_channels, out_channels, kernel_size, stride=1, padding=0, dilation=1, groups=1, bias=True):
+    self.kernel_size = (kernel_size, kernel_size) if isinstance(kernel_size, int) else tuple(kernel_size)
+    self.stride, self.padding, self.dilation, self.groups = stride, padding, dilation, groups
+    self.weight = Tensor.glorot_uniform(out_channels, in_channels//groups, *self.kernel_size)
+    self.bias = Tensor.zeros(out_channels) if bias else None
 
   def __call__(self, x):
-    return x.conv2d(self.weight, self.bias, padding=self.padding, stride=self.stride)
+    return x.conv2d(self.weight, self.bias, padding=self.padding, stride=self.stride, dilation=self.dilation, groups=self.groups)
 
 class Linear:
   def __init__(self, in_features, out_features, bias=True):
-    self.weight = Tensor.glorot_uniform(out_features, in_features).realize()
-    self.bias = Tensor.zeros(out_features).contiguous().realize() if bias else None
+    self.weight = Tensor.glorot_uniform(out_features, in_features)
+    self.bias = Tensor.zeros(out_features) if bias else None
 
   def __call__(self, x):
     return x.linear(self.weight.transpose(), self.bias)
 
 class GroupNorm:
   def __init__(self, num_groups:int, num_channels:int, eps:float=1e-5, affine:bool=True):
     self.num_groups, self.num_channels, self.eps = num_groups, num_channels, eps
-    self.weight : Optional[Tensor] = Tensor.ones(num_channels) if affine else None
-    self.bias : Optional[Tensor] = Tensor.zeros(num_channels) if affine else None
+    self.weight: Optional[Tensor] = Tensor.ones(num_channels) if affine else None
+    self.bias: Optional[Tensor] = Tensor.zeros(num_channels) if affine else None
 
   def __call__(self, x:Tensor):
     # reshape for layernorm to work as group norm
     # subtract mean and divide stddev
     x = x.reshape(x.shape[0], self.num_groups, -1).layernorm(eps=self.eps).reshape(x.shape)
 
     if self.weight is None or self.bias is None: return x
     # elementwise_affine on channels
-    return x * self.weight.reshape(1, -1, 1, 1) + self.bias.reshape(1, -1, 1, 1)
+    return x * self.weight.reshape(1, -1, *[1 for _ in range(len(x.shape)-2)]) + self.bias.reshape(1, -1, *[1 for _ in range(len(x.shape)-2)])
 
 class LayerNorm:
   def __init__(self, normalized_shape:Union[int, Tuple[int, ...]], eps:float=1e-5, elementwise_affine:bool=True):
-    normalized_shape = (normalized_shape,) if isinstance(normalized_shape, int) else tuple(normalized_shape)
-    self.axis, self.eps, self.elementwise_affine = tuple(-1-i for i in range(len(normalized_shape))), eps, elementwise_affine
-    self.weight, self.bias = (Tensor.ones(*normalized_shape), Tensor.zeros(*normalized_shape)) if elementwise_affine else (None, None)
+    self.normalized_shape = (normalized_shape,) if isinstance(normalized_shape, int) else tuple(normalized_shape)
+    self.axis, self.eps, self.elementwise_affine = tuple(-1-i for i in range(len(self.normalized_shape))), eps, elementwise_affine
+    self.weight, self.bias = (Tensor.ones(*self.normalized_shape), Tensor.zeros(*self.normalized_shape)) if elementwise_affine else (None, None)
 
   def __call__(self, x:Tensor):
+    assert self.normalized_shape == x.shape[-len(self.normalized_shape):], f"last dimensions of {x.shape} must match {self.normalized_shape}"
     x = x.layernorm(eps=self.eps, axis=self.axis)
     if not self.elementwise_affine: return x
     return x * self.weight + self.bias
+
+class LayerNorm2d(LayerNorm):
+  def __call__(self, x): return super().__call__(x.permute(0, 2, 3, 1)).permute(0, 3, 1, 2)
```

### Comparing `tinygrad-0.5.0/tinygrad/nn/optim.py` & `tinygrad-0.6.0/tinygrad/nn/optim.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,87 +1,71 @@
 # sorted in order of increasing complexity
-from typing import List
+from typing import List, Dict
 from tinygrad.tensor import Tensor
 
 class Optimizer:
-  def __init__(self, params : List[Tensor]):
+  def __init__(self, params: List[Tensor]):
     # if it's None, but being put into an optimizer, set it to True
     for x in params:
       if x.requires_grad is None: x.requires_grad = True
 
-    self.params : List[Tensor] = [x for x in params if x.requires_grad]
-    self.buffers : List[Tensor] = [x for x in params if not x.requires_grad]   # buffers are still realized
-
-  # TODO: this probably shouldn't change the gradients, just the ones used by the optimizer
-  def clipnorm(self, amount=1):
-    for param in self.params:
-      assert param.grad is not None
-      # clipnorm is the L2 norm, not value: is this right?
-      param.grad.assign(param.grad.clip(-(amount**2), (amount**2)))
+    self.params: List[Tensor] = [x for x in params if x.requires_grad]
+    self.buffers: List[Tensor] = [x for x in params if not x.requires_grad]   # buffers are still realized
 
   def zero_grad(self):
     for param in self.params: param.grad = None
 
   def realize(self, extra=None):
     # TODO: corealize
+    # NOTE: in extra is too late for most of the params due to issues with assign
     for p in extra + self.params + self.buffers if extra is not None else self.params + self.buffers:
       p.realize()
 
 class SGD(Optimizer):
-  def __init__(self, params : List[Tensor], lr=0.001, momentum=0, nesterov=False):
+  def __init__(self, params: List[Tensor], lr=0.001, momentum=0, nesterov=False):
     super().__init__(params)
     self.lr, self.momentum, self.nesterov = lr, momentum, nesterov
-    self.b = [Tensor.zeros(*t.shape, device=params[0].device, requires_grad=False) for t in self.params] if self.momentum else []
+    self.b = [Tensor.zeros(*t.shape, device=t.device, requires_grad=False) for t in self.params] if self.momentum else []
 
   # https://pytorch.org/docs/stable/generated/torch.optim.SGD.html
   def step(self) -> None:
     for i, t in enumerate(self.params):
       assert t.grad is not None
-      g = t.grad
+      g = t.grad.realize()
       if self.momentum:
-        self.b[i].assign(self.momentum * self.b[i] + g)
+        self.b[i].assign(self.momentum * self.b[i] + g).realize()  # NOTE: self.b[i] is zero on the first run, no if required
         g = (g + self.momentum * self.b[i]) if self.nesterov else self.b[i]
       t.assign(t.detach() - g * self.lr)
     self.realize(self.b)
 
-class RMSprop(Optimizer):
-  def __init__(self, params : List[Tensor], lr=0.001, decay=0.9, eps=1e-8):
-    super().__init__(params)
-    self.lr, self.decay, self.eps = lr, decay, eps
-
-    self.v = [Tensor.zeros(*t.shape, device=params[0].device, requires_grad=False) for t in self.params]
-
-  def step(self) -> None:
-    for i, t in enumerate(self.params):
-      assert t.grad is not None
-      self.v[i].assign(self.decay * self.v[i] + (1.0 - self.decay) * (t.grad * t.grad))
-      t.assign(t.detach() - (t.grad * self.lr).div(self.v[i].sqrt() + self.eps))
-    self.realize(self.v)
-
-class Adam(Optimizer):
-  def __init__(self, params : List[Tensor], lr=0.001, b1=0.9, b2=0.999, eps=1e-8):
+class AdamW(Optimizer):
+  def __init__(self, params: List[Tensor], lr=0.001, b1=0.9, b2=0.999, eps=1e-8, wd=0.01):
     super().__init__(params)
     # NOTE: self.t is a tensor so Adam can be jitted
-    self.lr, self.b1, self.b2, self.eps, self.t = lr, b1, b2, eps, Tensor([0], requires_grad=False).realize()
+    self.lr, self.b1, self.b2, self.eps, self.wd, self.t = lr, b1, b2, eps, wd, Tensor([0], requires_grad=False).realize()
 
-    self.m = [Tensor.zeros(*t.shape, device=params[0].device, requires_grad=False) for t in self.params]
-    self.v = [Tensor.zeros(*t.shape, device=params[0].device, requires_grad=False) for t in self.params]
+    self.m = [Tensor.zeros(*t.shape, device=t.device, requires_grad=False) for t in self.params]
+    self.v = [Tensor.zeros(*t.shape, device=t.device, requires_grad=False) for t in self.params]
 
   def step(self) -> None:
-    self.t = self.t + 1
+    self.t.assign(self.t + 1).realize()
     a = self.lr * ((1.0 - self.b2**self.t)**0.5) / (1.0 - self.b1**self.t)
     for i, t in enumerate(self.params):
       assert t.grad is not None
-      self.m[i].assign(self.b1 * self.m[i] + (1.0 - self.b1) * t.grad)
-      self.v[i].assign(self.b2 * self.v[i] + (1.0 - self.b2) * (t.grad * t.grad))
-      t.assign(t.detach() - a * self.m[i].div(self.v[i].sqrt() + self.eps))
+      g = t.grad.realize()
+      self.m[i].assign(self.b1 * self.m[i] + (1.0 - self.b1) * g).realize()
+      self.v[i].assign(self.b2 * self.v[i] + (1.0 - self.b2) * (g * g)).realize()
+      t.assign(t.detach() - a * self.m[i].div(self.v[i].sqrt() + self.eps) - self.lr * self.wd * t.detach())
     self.realize([self.t] + self.m + self.v)
 
-def get_parameters(obj) -> List[Tensor]:
-  parameters : List[Tensor] = []
-  if isinstance(obj, Tensor):
-    parameters.append(obj)
-  elif isinstance(obj, (list, tuple)):
-    for x in obj: parameters.extend(get_parameters(x))
-  elif hasattr(obj, '__dict__'):
-    for v in obj.__dict__.values(): parameters.extend(get_parameters(v))
-  return parameters
+def Adam(params: List[Tensor], lr=0.001, b1=0.9, b2=0.999, eps=1e-8): return AdamW(params, lr, b1, b2, eps, 0.0)
+
+def get_state_dict(obj, prefix:str='') -> Dict[str, Tensor]:
+  if isinstance(obj, Tensor): return {prefix.strip('.'):obj}
+  if hasattr(obj, '__dict__'): return get_state_dict(obj.__dict__, prefix)
+  state_dict = {}
+  if isinstance(obj, (list, tuple)):
+    for i,x in enumerate(obj): state_dict.update(get_state_dict(x, f"{prefix}{str(i)}."))
+  elif isinstance(obj, dict):
+    for k,v in obj.items(): state_dict.update(get_state_dict(v, f"{prefix}{str(k)}."))
+  return state_dict
+def get_parameters(obj) -> List[Tensor]: return list(get_state_dict(obj).values())
```

### Comparing `tinygrad-0.5.0/tinygrad/runtime/ops_clang.py` & `tinygrad-0.6.0/tinygrad/runtime/ops_clang.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,33 +1,27 @@
 import os, time, ctypes, hashlib, subprocess, platform
-import numpy as np
-from collections import defaultdict
-from typing import Final, Dict
-from tinygrad.ops import CompiledBuffer, RawBufferCopyIn
-from tinygrad.codegen.gpu import GPUCodegen, GPULanguage
-
-class RawMallocBuffer(RawBufferCopyIn):
-  def __init__(self, size): self._buf = (ctypes.c_float * (size//4))()
-  def copyin(self, x:np.ndarray): ctypes.memmove(self._buf, x.ctypes.data, x.size*4)
-  def toCPU(self): return np.ctypeslib.as_array(self._buf)
+from tinygrad.ops import Compiled
+from tinygrad.runtime.lib import RawMallocBuffer
+from tinygrad.codegen.cstyle import CStyleCodegen, CStyleLanguage
 
 class ClangProgram:
-  kernel_cnt : Final[Dict[str, int]] = defaultdict(int)
   def __init__(self, name:str, prg:str):
-    prg = "#include <math.h>\n#define max(x,y) ((x>y)?x:y)\n" + prg
+    prg = "#include <math.h>\n#define max(x,y) ((x>y)?x:y)\n#define half __fp16\n" + prg
     # TODO: is there a way to not write this to disk?
     fn = f"/tmp/clang_{hashlib.md5(prg.encode('utf-8')).hexdigest()}.{'dylib' if platform.system() == 'Darwin' else 'so'}"
+    # NOTE: --rtlib=compiler-rt fixes float16 on Linux, it defines __gnu_h2f_ieee and __gnu_f2h_ieee
     if not os.path.exists(fn):
-      subprocess.check_output(['clang', '-shared', '-O2', '-Wall','-Werror', '-lm', '-fPIC', '-x', 'c', '-', '-o', fn+".tmp"], input=prg.encode('utf-8'))
+      subprocess.check_output(['clang', '-shared', '-O2', '-Wall','-Werror', '-lm', '--rtlib=compiler-rt', '-fPIC', '-x', 'c', '-', '-o', fn+".tmp"], input=prg.encode('utf-8'))
       os.rename(fn+".tmp", fn)
     self.lib = ctypes.CDLL(fn)
     self.fxn = self.lib[name]
-  def __call__(self, *args, wait=False):
+
+  def __call__(self, global_size, local_size, *args, wait=False):
     if wait: st = time.monotonic()
-    self.fxn(*[x._buf for x in args[2:]])
+    self.fxn(*[x._buf for x in args])
     if wait: return time.monotonic()-st
 
-class ClangCodegen(GPUCodegen):
-  lang = GPULanguage(buffer_suffix="restrict")
+class ClangCodegen(CStyleCodegen):
+  lang = CStyleLanguage(buffer_suffix=" restrict")
+  supports_float4: bool = False
 
-class ClangBuffer(CompiledBuffer):
-  raw_buffer_type, codegen_type, runtime_type = RawMallocBuffer, ClangCodegen, ClangProgram
+ClangBuffer = Compiled(RawMallocBuffer, ClangCodegen, ClangProgram)
```

### Comparing `tinygrad-0.5.0/tinygrad/runtime/ops_cpu.py` & `tinygrad-0.6.0/tinygrad/runtime/ops_cpu.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import numpy as np
 import operator
-from typing import ClassVar, Callable, Dict, Tuple
-from tinygrad.ops import UnaryOps, BinaryOps, MovementOps, ReduceOps, FusedOps, InterpretedBuffer, Op
+from typing import Callable, Dict, Tuple
+from tinygrad.helpers import dtypes
+from tinygrad.ops import UnaryOps, BinaryOps, MovementOps, ReduceOps, FusedOps, Op, Interpreted
+from tinygrad.runtime.lib import RawBuffer
 
 def shape_to_axis(old_shape:Tuple[int, ...], new_shape:Tuple[int, ...]) -> Tuple[int, ...]:
   assert len(old_shape) == len(new_shape), "reduce shapes must have same dimensions"
   return tuple(i for i,(a,b) in enumerate(zip(old_shape, new_shape)) if a != b)
 
-base_fxn_for_op : Dict[Op, Callable] = {
-  UnaryOps.NEG: lambda x: -x, UnaryOps.NOT: lambda x: (1.0 - x),
+base_fxn_for_op: Dict[Op, Callable] = {
   BinaryOps.ADD: operator.add, BinaryOps.SUB: operator.sub, BinaryOps.MUL: operator.mul, BinaryOps.DIV: operator.truediv, BinaryOps.POW: operator.pow,
   ReduceOps.SUM: lambda x, new_shape: x.sum(shape_to_axis(x.shape, new_shape), keepdims=True) if tuple(x.shape) != tuple(new_shape) else x[:],
   ReduceOps.MAX: lambda x, new_shape: (x.amax if hasattr(x, 'amax') else x.max)(shape_to_axis(x.shape, new_shape), keepdims=True) if tuple(x.shape) != tuple(new_shape) else x[:],
-  MovementOps.SHRINK: lambda x, arg: x[tuple(slice(p[0], p[1], None) for p in arg)],
+  MovementOps.RESHAPE: lambda x, arg: x.reshape(arg), MovementOps.SHRINK: lambda x, arg: x[tuple(slice(p[0], p[1], None) for p in arg)],
 }
 
 def einsum_mulacc(einsum, get_strides, expand):
   def einscripts(x): return ''.join(["abcdefghijklmnopqrstuvwxyz"[i] for i in x])
   def axes_slice(strides): return [i for i in range(len(strides)) if strides[i] != 0], tuple(slice(None) if strides[i] != 0 else 0 for i in range(len(strides)))
   def mulacc(a, b, new_shape):
     (a_axes, a_slices), (b_axes, b_slices) = axes_slice(get_strides(a)), axes_slice(get_strides(b))
     out = [i for i in range(len(new_shape)) if a.shape[i] == new_shape[i] and (i in a_axes or i in b_axes)]
     ret = einsum(f"{einscripts(a_axes)}, {einscripts(b_axes)} -> {einscripts(out)}", a[a_slices], b[b_slices])
     return expand(ret.reshape([(1 if i not in a_axes and i not in b_axes else s) for i,s in enumerate(new_shape)]), new_shape)
   return mulacc
 
-numpy_fxn_for_op : Dict[Op, Callable] = {**base_fxn_for_op, **{
-  UnaryOps.NOOP: np.ascontiguousarray, UnaryOps.EXP: np.exp, UnaryOps.LOG: np.log,
+numpy_fxn_for_op: Dict[Op, Callable] = {**base_fxn_for_op, **{
+  UnaryOps.NOOP: lambda x: np.require(x, requirements='C'), UnaryOps.EXP: np.exp, UnaryOps.LOG: np.log, UnaryOps.CAST: lambda x,y: x.astype(y.np), UnaryOps.SIN: np.sin,
   BinaryOps.MAX: np.maximum, BinaryOps.CMPEQ: lambda x,y: (x==y).astype(np.float32),
-  MovementOps.FLIP: np.flip, MovementOps.PERMUTE: lambda x, order: x.transpose(order),
-  MovementOps.PAD: np.pad, MovementOps.EXPAND: np.broadcast_to,
-  FusedOps.MULACC: einsum_mulacc(lambda s,a,b: np.einsum(s, a.copy(), b.copy()), lambda x: x.strides, np.broadcast_to)
+  MovementOps.PERMUTE: lambda x, order: x.transpose(order), MovementOps.PAD: np.pad, MovementOps.EXPAND: np.broadcast_to,
+  MovementOps.STRIDE: lambda x, arg: x[tuple(slice(None, None, i) for i in arg)],
+  FusedOps.MULACC: einsum_mulacc(lambda s,a,b: np.einsum(s, a.copy(), b.copy()), lambda x: x.strides, np.broadcast_to),
 }}
 
-class CPUBuffer(InterpretedBuffer):
-  fxn_for_op : ClassVar = numpy_fxn_for_op
-
-  @staticmethod
-  def fromCPU(x): return CPUBuffer(x)
+class RawNumpyBuffer(RawBuffer):
+  def __init__(self, buf:np.ndarray): super().__init__(buf.size, dtypes.from_np(buf.dtype), buf)
+  @classmethod
+  def fromCPU(cls, x): return cls(x)
   def toCPU(self): return self._buf
+CPUBuffer = Interpreted(RawNumpyBuffer, numpy_fxn_for_op)
```

### Comparing `tinygrad-0.5.0/tinygrad/runtime/ops_cuda.py` & `tinygrad-0.6.0/tinygrad/runtime/ops_cuda.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,31 @@
+import subprocess
 from typing import Optional
 import numpy as np
 import pycuda.autoprimaryctx # type: ignore # pylint: disable=unused-import # noqa: F401
 import pycuda.driver as cuda # type: ignore
 from pycuda.compiler import compile as cuda_compile # type: ignore
 from tinygrad.helpers import DEBUG
-from tinygrad.ops import CompiledBuffer, RawBufferCopyInOut
-from tinygrad.codegen.gpu import GPUCodegen, GPULanguage
+from tinygrad.ops import Compiled
+from tinygrad.runtime.lib import RawBufferCopyInOut
+from tinygrad.codegen.cstyle import CStyleCodegen, CStyleLanguage
 
 class RawCUDABuffer(RawBufferCopyInOut):
-  def __init__(self, size): self.size, self._cl = size, cuda.mem_alloc(size)
-  def copyin(self, x:np.ndarray, stream:Optional[cuda.Stream]=None): cuda.memcpy_htod_async(self._cl, x, stream)
-  def copyout(self, x:np.ndarray): cuda.memcpy_dtoh(x, self._cl)
+  def __init__(self, size, dtype): super().__init__(size, dtype, cuda.mem_alloc(size * dtype.itemsize))
+  def _copyin(self, x:np.ndarray, stream:Optional[cuda.Stream]=None): cuda.memcpy_htod_async(self._buf, x, stream)
+  def _copyout(self, x:np.ndarray): cuda.memcpy_dtoh(x, self._buf)
 
 class CUDAProgram:
   def __init__(self, name:str, prg:str, binary=False):
     try:
+      if DEBUG >= 6:
+        with open("/tmp/cubin", "wb") as f:
+          f.write(cuda_compile(prg, target="cubin", no_extern_c=True))
+        sass = subprocess.check_output(['nvdisasm', '/tmp/cubin']).decode('utf-8')
+        print(sass)
       if not binary: prg = cuda_compile(prg, target="ptx", no_extern_c=True).decode('utf-8')
     except cuda.CompileError as e:
       if DEBUG >= 3: print("FAILED TO BUILD", prg)
       raise e
     if DEBUG >= 5: print(prg)
     # TODO: name is wrong, so we get it from the ptx using hacks
     self.prg = cuda.module_from_buffer(prg.encode('utf-8')).get_function(prg.split(".visible .entry ")[1].split("(")[0])
@@ -27,21 +34,21 @@
     local_size = (local_size + [1] * (3 - len(local_size))) if local_size is not None else (1,1,1)
     global_size = global_size + [1] * (3 - len(global_size))
     assert all(x%y == 0 for x,y in zip(global_size, local_size)), f"local:{local_size} must divide global:{global_size}"
     global_size = [x//y for x,y in zip(global_size, local_size)]
     if wait:
       start, end = cuda.Event(), cuda.Event()
       start.record()
-    self.prg(*[x._cl for x in args], block=tuple(local_size), grid=tuple(global_size))
+    self.prg(*[x._buf for x in args], block=tuple(local_size), grid=tuple(global_size))
     if wait:
       end.record()
       end.synchronize()
       return start.time_till(end)*1e-3
 
-class CUDACodegen(GPUCodegen):
-  lang = GPULanguage(
+class CUDACodegen(CStyleCodegen):
+  lang = CStyleLanguage(
     kernel_prefix = "__global__", smem_prefix = "__shared__ ", barrier = "__syncthreads();", float4 = "make_float4",
+    half_prekernel = "#include <cuda_fp16.h>",
     gid = [f'blockDim.{chr(120+i)}*blockIdx.{chr(120+i)}+threadIdx.{chr(120+i)}' for i in range(3)],
     lid = [f'threadIdx.{chr(120+i)}' for i in range(3)])
 
-class CUDABuffer(CompiledBuffer):
-  raw_buffer_type, codegen_type, runtime_type = RawCUDABuffer, CUDACodegen, CUDAProgram
+CUDABuffer = Compiled(RawCUDABuffer, CUDACodegen, CUDAProgram, cuda.Context.synchronize)
```

### Comparing `tinygrad-0.5.0/tinygrad/runtime/ops_llvm.py` & `tinygrad-0.6.0/tinygrad/runtime/ops_llvm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import time, hashlib, ctypes
 from typing import ClassVar
-from tinygrad.ops import CompiledBuffer
-from tinygrad.runtime.ops_clang import RawMallocBuffer
+from tinygrad.ops import Compiled
 from tinygrad.helpers import getenv, DEBUG
 from ctypes import CFUNCTYPE
-from tinygrad.codegen.llvm import LLVMCodegen
+from tinygrad.codegen.llvmir import LLVMIRCodegen
+from tinygrad.runtime.lib import RawMallocBuffer
 
 import llvmlite.binding as llvm  # type: ignore
 
 class LLVM:
-  target_machine : ClassVar[llvm.targets.TargetMachine] = None
-  engine : ClassVar[llvm.executionengine.ExecutionEngine] = None
-  optimizer : ClassVar[llvm.passmanagers.ModulePassManager] = None
+  target_machine: ClassVar[llvm.targets.TargetMachine] = None
+  engine: ClassVar[llvm.executionengine.ExecutionEngine] = None
+  optimizer: ClassVar[llvm.passmanagers.ModulePassManager] = None
 
   def __init__(self):
     if LLVM.engine is not None: return
     llvm.initialize()
     llvm.initialize_native_target()
     llvm.initialize_native_asmprinter()
     llvm.initialize_native_asmparser()
@@ -53,14 +53,13 @@
     LLVM.engine.add_module(self.mod)
     LLVM.engine.finalize_object()
     self.fxn = LLVM.engine.get_function_address(name)
 
   def __del__(self): LLVM.engine.remove_module(self.mod)
 
   def __call__(self, unused_global_size, unused_local_size, *bufs, wait=False):
-    cfunc = CFUNCTYPE(ctypes.c_int, *[ctypes.POINTER(ctypes.c_float) for _ in bufs])(self.fxn)
+    cfunc = CFUNCTYPE(ctypes.c_int, *[ctypes.c_void_p for _ in bufs])(self.fxn)
     if wait: st = time.monotonic()
     cfunc(*[x._buf for x in bufs])
     if wait: return time.monotonic()-st
 
-class LLVMBuffer(CompiledBuffer):
-  raw_buffer_type, codegen_type, runtime_type = RawMallocBuffer, LLVMCodegen, LLVMProgram
+LLVMBuffer = Compiled(RawMallocBuffer, LLVMIRCodegen, LLVMProgram)
```

### Comparing `tinygrad-0.5.0/tinygrad/runtime/ops_metal.py` & `tinygrad-0.6.0/tinygrad/runtime/ops_metal.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 # pip3 install pyobjc-framework-Metal pyobjc-framework-Cocoa pyobjc-framework-libdispatch
-import os, subprocess, pathlib, functools
+import os, subprocess, pathlib
 import Metal, Cocoa, libdispatch # type: ignore
-import numpy as np
 from typing import List, Any
-from tinygrad.codegen.gpu import GPUCodegen, GPULanguage
-from tinygrad.helpers import prod, getenv, DEBUG
-from tinygrad.ops import CompiledBuffer, RawBufferCopyIn
+from tinygrad.codegen.cstyle import CStyleCodegen, CStyleLanguage
+from tinygrad.helpers import prod, getenv, DEBUG, DType
+from tinygrad.ops import Compiled
+from tinygrad.runtime.lib import RawBufferMapped
 
 METAL_XCODE = getenv("METAL_XCODE")
 
 class _METAL:
-  mtl_buffers_in_flight : List[Any] = []
-  @functools.cached_property
-  def device(self):
-    return Metal.MTLCreateSystemDefaultDevice()
-  @functools.cached_property
-  def mtl_queue(self):
-    return METAL.device.newCommandQueue()
+  def __init__(self):
+    self.mtl_buffers_in_flight: List[Any] = []
+    self.device = Metal.MTLCreateSystemDefaultDevice()
+    self.mtl_queue = self.device.newCommandQueue()
+  # TODO: is there a better way to do this?
+  def synchronize(self):
+    for cbuf in self.mtl_buffers_in_flight: cbuf.waitUntilCompleted()
+    self.mtl_buffers_in_flight.clear()
 METAL = _METAL()
 
-class RawMetalBuffer(RawBufferCopyIn):
-  def __init__(self, size): self.size, self._cl = size, METAL.device.newBufferWithLength_options_(size, Metal.MTLResourceStorageModeShared)
-  def __del__(self): self._cl.release()
-  def _as_np(self): return np.frombuffer(self._cl.contents().as_buffer(self._cl.length()), dtype=np.float32)
-  def copyin(self, x:np.ndarray): np.copyto(self._as_np(), x.reshape(-1).data)
-  def toCPU(self) -> np.ndarray:
-    for cbuf in METAL.mtl_buffers_in_flight: cbuf.waitUntilCompleted()
-    METAL.mtl_buffers_in_flight = []
-    return self._as_np()  # no copy!
+class RawMetalBuffer(RawBufferMapped):
+  def __init__(self, size:int, dtype:DType): super().__init__(size, dtype, METAL.device.newBufferWithLength_options_(size*dtype.itemsize, Metal.MTLResourceStorageModeShared))
+  def __del__(self):
+    self._buf.release()
+    super().__del__()
+  def _buffer(self):
+    METAL.synchronize()
+    return self._buf.contents().as_buffer(self._buf.length())
 
 def unwrap(x):
   ret, err = x
   assert err is None, str(err)
   return ret
 
 class MetalProgram:
@@ -62,26 +62,25 @@
     if local_size is None: local_size = [32]
     local_size += [1] * (3-len(local_size))
 
     assert prod(local_size) <= self.pipeline_state.maxTotalThreadsPerThreadgroup(), f"local size {local_size} bigger than {self.pipeline_state.maxTotalThreadsPerThreadgroup()} with exec width {self.pipeline_state.threadExecutionWidth()} memory length {self.pipeline_state.staticThreadgroupMemoryLength()}"
     command_buffer = METAL.mtl_queue.commandBuffer()
     encoder = command_buffer.computeCommandEncoder()
     encoder.setComputePipelineState_(self.pipeline_state)
-    for i,a in enumerate(bufs): encoder.setBuffer_offset_atIndex_(a._cl, 0, i)
+    for i,a in enumerate(bufs): encoder.setBuffer_offset_atIndex_(a._buf, 0, i)
     encoder.dispatchThreads_threadsPerThreadgroup_(Metal.MTLSize(*global_size), Metal.MTLSize(*local_size))
     encoder.endEncoding()
     command_buffer.commit()
     if wait:
       command_buffer.waitUntilCompleted()
       return command_buffer.GPUEndTime() - command_buffer.GPUStartTime()
     else:
       METAL.mtl_buffers_in_flight.append(command_buffer)
 
-class MetalCodegen(GPUCodegen):
-  lang = GPULanguage(
+class MetalCodegen(CStyleCodegen):
+  lang = CStyleLanguage(
     kernel_prefix = "#include <metal_stdlib>\nusing namespace metal;\nkernel", buffer_prefix = "device ", smem_prefix = "threadgroup ",
     barrier = "threadgroup_barrier(mem_flags::mem_threadgroup);", float4 = "float4",
     gid = [f"gid.{chr(120+i)}" for i in range(3)], lid = [f"lid.{chr(120+i)}" for i in range(3)],
     extra_args = ['uint3 gid [[thread_position_in_grid]]', 'uint3 lid [[thread_position_in_threadgroup]]'])
 
-class MetalBuffer(CompiledBuffer):
-  raw_buffer_type, codegen_type, runtime_type = RawMetalBuffer, MetalCodegen, MetalProgram
+MetalBuffer = Compiled(RawMetalBuffer, MetalCodegen, MetalProgram, METAL.synchronize)
```

### Comparing `tinygrad-0.5.0/tinygrad/shape/symbolic.py` & `tinygrad-0.6.0/tinygrad/shape/symbolic.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,56 +2,63 @@
 import math, itertools, functools
 from typing import List, Dict, Callable, Type, Union
 from tinygrad.helpers import partition, all_same
 
 # NOTE: Python has different behavior for negative mod and floor div than c
 # symbolic matches the Python behavior, but the code output is agnostic, and will never have negative numbers in div or mod
 
-def create_node(typ:Type[Node], *args):
-  ret = typ(*args)
-  assert ret.min <= ret.max, f"min greater than max! {ret.min} {ret.max} when creating {typ} {args}"
-  if ret.min == ret.max: return NumNode(ret.min)
-  return ret
-
 class Node:
   b: int
   min: int
   max: int
   def render(self, ops=None, ctx=None) -> str:
     if ops is None: ops = render_python
-    assert isinstance(self, NumNode) or self.min != self.max
+    assert isinstance(self, (Variable, NumNode)) or self.min != self.max
     return ops[type(self)](self, ops, ctx)
   @functools.cached_property
   def key(self) -> str: return self.render(ctx="DEBUG")
   def __repr__(self): return "<"+self.key+">"
   def __eq__(self, other:object) -> bool:
     if not isinstance(other, Node): return NotImplemented
     return self.key == other.key
   def __neg__(self): return self*-1
   def __add__(self, b:Union[Node, int]): return Variable.sum([self, b if isinstance(b, Node) else Variable.num(b)])
   def __sub__(self, b:Union[Node, int]): return self+-b
-  def __ge__(self, b:int): return create_node(GeNode, self, b)
-  def __lt__(self, b:int): return create_node(LtNode, self, b)
+  def __ge__(self, b:int): return create_opnode(GeNode, self, b)
+  def __lt__(self, b:int): return create_opnode(LtNode, self, b)
   def __mul__(self, b:int):
     if b == 0: return NumNode(0)
     elif b == 1: return self
+
+    # this is a hack to make div work with boolean nodes. TODO: make generic
+    if isinstance(self, GeNode): return (self.a*b) >= (self.b*b)
+    if isinstance(self, LtNode): return (self.a*b) < (self.b*b)
+    if isinstance(self, AndNode): return Variable.ands([x*b for x in self.nodes])
+
     if isinstance(self, MulNode): return self.a*(self.b*b) # two muls is one mul
     if isinstance(self, SumNode): return Variable.sum([x*b for x in self.nodes]) # distribute mul into sum
-    return create_node(MulNode, self, b)
+    return create_opnode(MulNode, self, b)
 
   # *** complex ops ***
 
-  def __floordiv__(self, b:int):
+  def __floordiv__(self, b:int, factoring_allowed=True):
     assert b != 0
     if b < 0: return (self//-b)*-1
     if b == 1: return self
+
+    # this is a hack to make div work with boolean nodes. TODO: make generic
+    if isinstance(self, GeNode): return (self.a//b) >= (self.b//b)
+    if isinstance(self, LtNode): return (self.a//b) < (self.b//b)
+    if isinstance(self, AndNode): return Variable.ands([x//b for x in self.nodes])
+
+    if isinstance(self, ModNode) and self.b % b == 0: return (self.a//b) % (self.b//b) # put the div inside mod
     if isinstance(self, DivNode): return self.a//(self.b*b) # two divs is one div
     if isinstance(self, MulNode) and self.b % b == 0: return self.a*(self.b//b)
-    if isinstance(self, MulNode) and b % self.b == 0: return self.a//(b//self.b)
-    if isinstance(self, SumNode):
+    if isinstance(self, MulNode) and b % self.b == 0 and self.b > 0: return self.a//(b//self.b) # NOTE: mod negative isn't handled right
+    if isinstance(self, SumNode) and factoring_allowed:
       factors, tmp_nofactor = partition(self.nodes, lambda x: (isinstance(x, (MulNode, NumNode))) and x.b%b == 0)
       nofactor = []
       # ugh, i doubt this is universally right
       for x in tmp_nofactor:
         if isinstance(x, NumNode):
           if (x.b%b) != x.b:
             factors.append(Variable.num(x.b - (x.b%b)))  # python does floor division
@@ -67,18 +74,20 @@
           nofactor_term = Variable.sum(nofactor)//b
         return Variable.sum([(x.a * (x.b//b)) if isinstance(x, MulNode) else Variable.num(x.b//b) for x in factors] + [nofactor_term])
       else:
         muls = [x.b for x in nofactor if isinstance(x, MulNode)]
         for m in muls:
           if m > 1 and b%m == 0:
             return (self//m)//(b//m)
+    # the numerator of div is not allowed to be negative
     if self.min < 0:
       offset = self.min//b
-      return (self+offset*b)//b - offset
-    return create_node(DivNode, self, b)
+      # factor out an "offset" to make the numerator positive. don't allowing factoring again
+      return (self + -offset*b).__floordiv__(b, factoring_allowed=False) + offset
+    return create_opnode(DivNode, self, b)
 
   def __mod__(self, b:int):
     assert b > 0
     if b == 1: return NumNode(0)
     if isinstance(self, SumNode):
       new_nodes = []
       for x in self.nodes:
@@ -87,16 +96,16 @@
         else: new_nodes.append(x)
       a = Variable.sum(new_nodes)
     elif isinstance(self, MulNode):
       a = self.a * (self.b%b)
     else:
       a = self
     if a.min >= 0 and a.max < b: return a
-    if a.min < 0: return (a + ((a.min//b)*b)) % b
-    return create_node(ModNode, a, b)
+    if a.min < 0: return (a - ((a.min//b)*b)) % b
+    return create_opnode(ModNode, a, b)
 
   @staticmethod
   def num(num:int) -> Node: return NumNode(num)
 
   @staticmethod
   def sum(nodes:List[Node]) -> Node:
     # expand any sums inside one sum
@@ -106,31 +115,32 @@
       return Variable.sum(nodes)
 
     # combine any numbers inside a sum
     nodes, num_nodes = partition(nodes, lambda x: not isinstance(x, NumNode))
     nodes.append(NumNode(sum([x.b for x in num_nodes])))
 
     # combine any MulNodes that factorize (big hack sticking the MulNode(x, 1) on things)
+    # TODO: this is slow!
     nodes, mul_nodes = partition(nodes, lambda x: not isinstance(x, MulNode))
     mul_nodes += [MulNode(x, 1) for x in nodes]
     mul_nodes = sorted(mul_nodes, key=lambda x: x.a.render()) # group by equality (ugh, uses render!)
     new_nodes = [k * sum(x.b for x in g) for k, g in itertools.groupby(mul_nodes, key=lambda x: x.a)]
     nodes = [x if not isinstance(x, MulNode) or x.b != 1 else x.a for x in new_nodes]
 
     # filter 0s
     nodes = [x for x in nodes if x.min != 0 or x.max != 0]
-    return create_node(SumNode, nodes) if len(nodes) > 1 else (nodes[0] if len(nodes) == 1 else NumNode(0))
+    return create_rednode(SumNode, nodes) if len(nodes) > 1 else (nodes[0] if len(nodes) == 1 else NumNode(0))
 
   @staticmethod
   def ands(nodes:List[Node]) -> Node:
     if any((x.min == 0 and x.max == 0) for x in nodes): return NumNode(0)
 
     # filter 1s
     nodes = [x for x in nodes if x.min != x.max]
-    return create_node(AndNode, nodes) if len(nodes) > 1 else (nodes[0] if len(nodes) == 1 else NumNode(1))
+    return create_rednode(AndNode, nodes) if len(nodes) > 1 else (nodes[0] if len(nodes) == 1 else NumNode(1))
 
 # 4 basic node types
 
 class Variable(Node):
   def __new__(cls, expr:str, nmin:int, nmax:int):
     assert nmin >= 0 and nmin <= nmax
     if nmin == nmax: return NumNode(nmin)
@@ -139,53 +149,57 @@
   def __init__(self, expr:str, nmin:int, nmax:int):
     self.expr, self.min, self.max = expr, nmin, nmax
 
 class NumNode(Node):
   def __init__(self, num:int):
     self.b, self.min, self.max = num, num, num
 
+def create_node(ret:Node):
+  assert ret.min <= ret.max, f"min greater than max! {ret.min} {ret.max} when creating {type(ret)} {ret}"
+  if ret.min == ret.max: return NumNode(ret.min)
+  return ret
+
 class OpNode(Node):
-  def __init__(self, a:Node, b:int):
-    self.a, self.b = a, b
-    self.min, self.max = self.minmax(a,b)
-  minmax = staticmethod(lambda a,b: (1//0, 1//0))
+  def __init__(self, a:Node, b:int): self.a, self.b = a, b
 
-class RedNode(Node):
-  def __init__(self, nodes:List[Node]):
-    self.nodes = nodes
-    self.min, self.max = self.minmax(nodes)
-  minmax = staticmethod(lambda nodes: (1//0, 1//0))
-
-# operation nodes
-
-class GeNode(OpNode): minmax = staticmethod(lambda a,b: (int(a.min >= b), int(a.max >= b)))
-class LtNode(OpNode): minmax = staticmethod(lambda a,b: (int(a.max < b), int(a.min < b)))
-class MulNode(OpNode): minmax = staticmethod(lambda a,b: (a.min*b, a.max*b) if b >= 0 else (a.max*b, a.min*b))
-class DivNode(OpNode):
-  @staticmethod
-  def minmax(a, b):
+class GeNode(OpNode): pass
+class LtNode(OpNode): pass
+class MulNode(OpNode): pass
+class DivNode(OpNode): pass
+class ModNode(OpNode): pass
+
+def create_opnode(typ:Type[OpNode], a:Node, b:int):
+  ret = typ(a, b)
+  if typ == GeNode: ret.min, ret.max = int(a.min >= b), int(a.max >= b)
+  elif typ == LtNode: ret.min, ret.max = int(a.max < b), int(a.min < b)
+  elif typ == MulNode: ret.min, ret.max = (a.min*b, a.max*b) if b >= 0 else (a.max*b, a.min*b)
+  elif typ == DivNode:
     assert a.min >= 0
-    return a.min//b, a.max//b
-
-class ModNode(OpNode):
-  @staticmethod
-  def minmax(a, b):
+    ret.min, ret.max = a.min//b, a.max//b
+  elif typ == ModNode:
     assert a.min >= 0
-    if a.max - a.min >= b or (a.min != a.max and a.min%b >= a.max%b): return (0, b-1)
-    return a.min%b, a.max%b
+    ret.min, ret.max = (0, b-1) if a.max - a.min >= b or (a.min != a.max and a.min%b >= a.max%b) else (a.min%b, a.max%b)
+  return create_node(ret)
+
+class RedNode(Node):
+  def __init__(self, nodes:List[Node]): self.nodes = nodes
 
-# reduce nodes
+class SumNode(RedNode): pass
+class AndNode(RedNode): pass
 
-class SumNode(RedNode): minmax = staticmethod(lambda nodes: (sum([x.min for x in nodes]), sum([x.max for x in nodes])))
-class AndNode(RedNode): minmax = staticmethod(lambda nodes: (min([x.min for x in nodes]), max([x.max for x in nodes])))
+def create_rednode(typ:Type[RedNode], nodes:List[Node]):
+  ret = typ(nodes)
+  if typ == SumNode: ret.min, ret.max = (sum([x.min for x in nodes]), sum([x.max for x in nodes]))
+  elif typ == AndNode: ret.min, ret.max = (min([x.min for x in nodes]), max([x.max for x in nodes]))
+  return create_node(ret)
 
-render_python : Dict[Type, Callable] = {
-  Variable: lambda self,ops,ctx: f"{self.expr}<{self.min},{self.max}>" if ctx == "DEBUG" else f"{self.expr}",
+render_python: Dict[Type, Callable] = {
+  Variable: lambda self,ops,ctx: f"{self.expr}[{self.min}-{self.max}]" if ctx == "DEBUG" else f"{self.expr}",
   NumNode: lambda self,ops,ctx: f"{self.b}",
   MulNode: lambda self,ops,ctx: f"({self.a.render(ops,ctx)}*{self.b})",
   DivNode: lambda self,ops,ctx: f"({self.a.render(ops,ctx)}//{self.b})",
   ModNode: lambda self,ops,ctx: f"({self.a.render(ops,ctx)}%{self.b})",
   GeNode: lambda self,ops,ctx: f"({self.a.render(ops,ctx)}>={self.b})",
   LtNode: lambda self,ops,ctx: f"({self.a.render(ops,ctx)}<{self.b})",
   SumNode: lambda self,ops,ctx: f"({'+'.join(sorted([x.render(ops,ctx) for x in self.nodes]))})",
-  AndNode: lambda self,ops,ctx: f"({'&&'.join(sorted([x.render(ops,ctx) for x in self.nodes]))})"
+  AndNode: lambda self,ops,ctx: f"({' and '.join(sorted([x.render(ops,ctx) for x in self.nodes]))})"
 }
```

### Comparing `tinygrad-0.5.0/tinygrad/tensor.py` & `tinygrad-0.6.0/tinygrad/tensor.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 # inspired by https://github.com/karpathy/micrograd/blob/master/micrograd/engine.py
 from __future__ import annotations
 import math, functools, itertools
 import numpy as np
 from typing import List, Tuple, Callable, Optional, ClassVar, Type, Union, Sequence
-from tinygrad.helpers import prod, argfix, make_pair, getenv, DEBUG, flatten
+from tinygrad.helpers import prod, argfix, make_pair, getenv, IMAGE, DEBUG, flatten, DType, dtypes, LazyNumpyArray
 from tinygrad.lazy import Device, LazyBuffer
-from tinygrad.image import image_conv2d_decorator
 
 # An instantiation of the Function is the Context
 class Function:
   def __init__(self, device:str, *tensors:Tensor):
     self.device, self.parents = device, tensors
     self.needs_input_grad = [t.requires_grad for t in self.parents]
     self.requires_grad = True if any(self.needs_input_grad) else (None if any(x is None for x in self.needs_input_grad) else False)
@@ -26,64 +25,77 @@
 
 import tinygrad.mlops as mlops
 
 # **** start with two base classes, Tensor and Function ****
 
 class Tensor:
   __deletable__ = ('_ctx',)
-  training : ClassVar[bool] = False
-  no_grad : ClassVar[bool] = False
+  training: ClassVar[bool] = False
+  no_grad: ClassVar[bool] = False
+  default_type: ClassVar[DType] = dtypes.float32
 
-  def __init__(self, data, device=Device.DEFAULT, requires_grad:Optional[bool]=None):
+  def __init__(self, data:Union[list, LazyBuffer, LazyNumpyArray, np.ndarray], device=Device.DEFAULT, dtype:Optional[DType]=None, requires_grad:Optional[bool]=None):
+    device = device.upper().replace(":0", "")  # canonicalize device
     if isinstance(data, list):
-      data = np.array(data, dtype=np.float32)
+      data = np.array(data, dtype=(dtype if dtype is not None else Tensor.default_type).np)
     elif isinstance(data, LazyBuffer) and data.device != device:
       # TODO: this has to realize, it shouldn't have to
       data = data.realize().toCPU()
 
-    if isinstance(data, np.ndarray):
+    # all ndarrays are lazy now
+    if isinstance(data, np.ndarray): data = LazyNumpyArray(data, data.shape, data.dtype)
+
+    # by here, it's either LazyNumpyArray or LazyBuffer
+    # TODO: it should all be LazyBuffer I think
+    if isinstance(data, LazyNumpyArray):
       data = data if data.shape else data.reshape((1,))
-      self.lazydata = LazyBuffer.fromCPU(data.astype(np.float32), device)
+      lazydata = LazyBuffer.fromCPU(data.astype(dtype.np) if dtype is not None else data, device)
     elif isinstance(data, LazyBuffer):
-      self.lazydata = data
+      assert dtype is None or dtype == data.dtype, "dtype doesn't match, and casting isn't supported"
+      lazydata = data
     else:
       raise RuntimeError(f"can't create Tensor from {data}")
 
+    # this is set once we are here
+    self.lazydata: LazyBuffer = lazydata
+
     # tensors have gradients, buffers do not
-    self.grad : Optional[Tensor] = None
+    self.grad: Optional[Tensor] = None
 
     # NOTE: this can be in three states. False and None: no gradient, True: gradient
     # None (the default) will be updated to True if it's put in an optimizer
-    self.requires_grad : Optional[bool] = requires_grad
+    self.requires_grad: Optional[bool] = requires_grad
 
     # internal variables used for autograd graph construction
-    self._ctx : Optional[Function] = None
+    self._ctx: Optional[Function] = None
 
   def __repr__(self):
-    return f"<Tensor {self.lazydata if self.lazydata.realized is None else self.lazydata.realized!r} with grad {(self.grad.lazydata if self.grad else None)!r}>"
+    return f"<Tensor {self.lazydata if self.lazydata.realized is None else self.lazydata.realized!r} on {self.device} with grad {(self.grad.lazydata if self.grad else None)!r}>"
+
+  # Python has a non moving GC, so this should be okay
+  def __hash__(self): return id(self)
 
   @property
-  def shape(self) -> Tuple[int, ...]: return self.lazydata.shape
+  def device(self) -> str: return self.lazydata.device
 
-  # dtype handling was very broken. it's always float32 now
   @property
-  def dtype(self) -> type: return np.float32
+  def shape(self) -> Tuple[int, ...]: return self.lazydata.shape
 
   @property
-  def device(self) -> str: return self.lazydata.device
+  def dtype(self) -> DType: return self.lazydata.dtype
 
   # ***** data handlers ****
 
   def realize(self) -> Tensor:
     self.lazydata.realize()
     return self
 
   def assign(self, x) -> Tensor:
     if not isinstance(x, Tensor): x = Tensor(x)
-    assert self.shape == x.shape
+    assert self.shape == x.shape, f"assign shape mismatch {self.shape} != {x.shape}"
     assert not x.requires_grad  # self requires_grad is okay?
     if DEBUG >= 4: print(f"assign {self.lazydata} <- {x.lazydata}")
     if self.lazydata.realized is not None and not getenv("DISALLOW_ASSIGN"): x.lazydata.output_buffer = self.lazydata.realized
     self.lazydata = x.lazydata
     return self
 
   def detach(self): return Tensor(self.lazydata, device=self.device, requires_grad=False)
@@ -123,24 +135,24 @@
   # TODO: requires cumsum to remove numpy
   @staticmethod
   def arange(stop, start=0, step=1, **kwargs): return Tensor(np.arange(start=start, stop=stop, step=step, dtype=np.float32), **kwargs)
 
   # ***** (numpy) rng helper functions *****
   # TODO: move randomness generation out of numpy
 
-  _rng : ClassVar[np.random.Generator] = np.random.default_rng()
+  _rng: ClassVar[np.random.Generator] = np.random.default_rng()
   @staticmethod
   def manual_seed(seed=None): Tensor._rng = np.random.default_rng(seed=seed)
 
   @staticmethod
-  def rand(*shape, **kwargs) -> Tensor: return Tensor(Tensor._rng.random(size=shape, dtype=np.float32), **kwargs)
+  def rand(*shape, **kwargs) -> Tensor: return Tensor(LazyNumpyArray(lambda lna: Tensor._rng.random(size=lna.shape, dtype=lna.dtype), shape, np.float32), **kwargs)
 
   # TODO: replace with a transformation from uniform -> gaussian
   @staticmethod
-  def randn(*shape, **kwargs) -> Tensor: return Tensor(Tensor._rng.standard_normal(size=shape, dtype=np.float32), **kwargs)
+  def randn(*shape, **kwargs) -> Tensor: return Tensor(LazyNumpyArray(lambda lna: Tensor._rng.standard_normal(size=lna.shape, dtype=lna.dtype), shape, np.float32), **kwargs)
 
   # ***** rng hlops *****
 
   @staticmethod
   def uniform(*shape, **kwargs) -> Tensor: return Tensor.rand(*shape, **kwargs) * 2 - 1
 
   @staticmethod
@@ -161,40 +173,41 @@
         nodes.append(node)
       return nodes
     return _deepwalk(self, set(), [])
 
   def backward(self):
     assert self.shape == (1,)
 
-    # fill in the first grad with one
+    # fill in the first grad with one. don't use Tensor.ones because we don't need contiguous
     # this is "implicit gradient creation"
-    self.grad = Tensor.ones(*self.shape, device=self.device, requires_grad=False)
+    self.grad = Tensor([1], device=self.device, requires_grad=False)
 
     for t0 in reversed(self.deepwalk()):
       if not any(x.requires_grad for x in t0._ctx.parents):
+        del t0._ctx  # TODO: does it help to delete this here ever?
         continue
       assert (t0.grad is not None)
       grads = t0._ctx.backward(t0.grad.lazydata)
       grads = [Tensor(g, device=self.device, requires_grad=False) if g is not None else None
         for g in ([grads] if len(t0._ctx.parents) == 1 else grads)]
       for t, g in zip(t0._ctx.parents, grads):
         if g is not None and t.requires_grad:
-          assert g.shape == t.shape, f"grad shape must match tensor shape in {self._ctx!r}, {g.shape!r} != {t.shape!r}"
+          assert g.shape == t.shape, f"grad shape must match tensor shape, {g.shape!r} != {t.shape!r}"
           t.grad = g if t.grad is None else (t.grad + g)
       del t0._ctx
 
   # ***** movement mlops *****
 
   def reshape(self, shape, *args) -> Tensor:
     new_shape = argfix(shape, *args)
     assert len(new_shape) > 0 and all(x != 0 for x in new_shape), f"zeros not allowed in shape {new_shape}"
     return mlops.Reshape.apply(self, shape=tuple(-prod(self.shape) // prod(new_shape) if s == -1 else s for s in new_shape))
   def expand(self, shape, *args) -> Tensor: return mlops.Expand.apply(self, shape=tuple(x if x != -1 else s for s,x in zip(self.shape, argfix(shape, *args))))
   def permute(self, order, *args) -> Tensor: return mlops.Permute.apply(self, order=argfix(order, *args))
-  def flip(self, axis, *args) -> Tensor: return mlops.Flip.apply(self, axis=argfix(axis, *args))
+  def flip(self, axis, *args) -> Tensor: return mlops.Flip.apply(self, axis=[x if x >= 0 else x+len(self.shape) for x in argfix(axis, *args)])
   def pad(self, arg:Tuple[Tuple[int, int], ...]) -> Tensor: return mlops.Pad.apply(self, arg=arg) if any(x != (0,0) for x in arg) else self
   def shrink(self, arg:Tuple[Tuple[int, int], ...]) -> Tensor: return mlops.Shrink.apply(self, arg=arg) if any(x != (0,s) for x,s in zip(arg, self.shape)) else self
 
   # ***** movement hlops *****
 
   # NOTE: using slice is discouraged and things should migrate to pad and shrink
   def slice(self, arg:Sequence[Optional[Tuple[int, int]]]) -> Tensor:
@@ -206,26 +219,26 @@
   # - Negative indices are taken relative to the end of the sequence, so X[-2] returns the 2nd-to-last element
   # - A slice i:j returns the elements with indices in [i, j)
   #   - If omitted, i and j will default to 0 and N, respectively, where N is the length of the sequence
   #   - Negative values for i and j are taken relative to the end of the sequence
   #   - Both i and j will be clamped to the range (-N, N], where N in the length of the sequence
   # - Indexing with np.newaxis or None on a given axis will add a new dimension of size one before that axis
   # - Empty slices are not allowed
-  # - Strides other than 1 are not allowedå
+  # - Strides other than 1 are not allowed
   def __getitem__(self, val):
     def slcfix(i, sz, default): return default if i is None else max(0, min(sz, sz+i if i < 0 else i))  # Fix negative idxs, clamp to [0,N]
     new_slice, new_shape = [], []
     val = [val] if not isinstance(val, (list, tuple)) else val
     assert sum(s is not None for s in val) <= len(self.shape)
     assert all(s.step is None or s.step == 1 for s in val if isinstance(s, slice))
     for i,(sz,s) in enumerate(zip(self.shape, [v for v in val if v is not None])):  # Slicing only depends on ints + slices
       if isinstance(s, int) and not (-sz <= s < sz):
         raise IndexError(f"index {s} is out of bounds for dimension {i} with size {sz}")
       new_slice.append((s%sz, s%sz+1) if isinstance(s, int) else (slcfix(s.start, sz, 0), slcfix(s.stop, sz, sz)))
-    for s,sz in zip(val, [self.shape[i-1] for i in itertools.accumulate([s is not None for s in val])]):  # Shape depends on slices + positions of Nones
+    for s,sz in zip(val, [self.shape[i-1] for i in itertools.accumulate([int(s is not None) for s in val])]):  # Shape depends on slices + positions of Nones
       if not isinstance(s, int):
         new_shape.append(1 if s is None else slcfix(s.stop, sz, sz) - slcfix(s.start, sz, 0))
     new_shape += [self.shape[i] for i in range(len(new_slice), len(self.shape))]
     new_slice += [(0,self.shape[i]) for i in range(len(new_slice), len(self.shape))]
     return self.slice(new_slice).reshape(new_shape if len(new_shape) else (1,))
 
   def cat(self, *args, dim=0):
@@ -235,48 +248,75 @@
     catargs = [self] + list(args)
     shape_cumsum = [0, *itertools.accumulate([y.shape[dim] for y in catargs])]
     slc = [[(0, s) for s in self.shape] for _ in catargs]
     for s,k in zip(slc, shape_cumsum):
       s[dim] = (-k, shape_cumsum[-1]-k)
     return functools.reduce(Tensor.__add__, [arg.slice(s) for arg,s in zip(catargs, slc)])
 
+  @staticmethod
+  def stack(tensors, dim=0):
+    first = tensors[0].unsqueeze(dim)
+    unsqueezed_tensors = [tensor.unsqueeze(dim) for tensor in tensors[1:]]
+    # checks for shapes and number of dimensions delegated to cat
+    return first.cat(*unsqueezed_tensors, dim=dim)
+
+  def repeat(self, repeats):
+    ndim = len(self.shape)
+    base_shape = self.shape
+    if len(repeats) > ndim:
+      base_shape = (1,) * (len(repeats) - ndim) + base_shape
+    new_shape = [x for i in range(len(base_shape)) for x in [1, base_shape[i]]]
+    expand_shape = [x for r,s in zip(repeats, base_shape) for x in [r,s]]
+    final_shape = [r*s for r,s in zip(repeats, base_shape)]
+    return self.reshape(new_shape).expand(expand_shape).reshape(final_shape)
+
   # TODO: make this nicer with syntactic sugar in slice
   def chunk(self, num, dim):
     slice_params = [[(0, s) for s in self.shape] for _ in range(num)]
     for i,k in enumerate(range(0, self.shape[dim], self.shape[dim]//num)):
       slice_params[i][dim] = (k, min(self.shape[dim], k+self.shape[dim]//num))
     return [self.slice(p) for p in slice_params]
 
   def unsqueeze(self, dim):
     if dim < 0: dim = len(self.shape) + dim + 1
     return self.reshape(self.shape[:dim] + (1,) + self.shape[dim:])
 
   # (padding_left, padding_right, padding_top, padding_bottom)
-  def pad2d(self, padding:Tuple[int, ...]): return self.slice(((0,self.shape[0]), (0,self.shape[1]), (-padding[2],self.shape[2]+padding[3]), (-padding[0],self.shape[3]+padding[1])))
-  # TODO: this is totally not transpose
-  def transpose(self, order=(1,0)) -> Tensor: return self.permute(order=order)
+  def pad2d(self, padding:Union[List[int], Tuple[int, ...]]):
+    slc = [(-p0, s+p1) for p0,p1,s in zip(padding[::2], padding[1::2], self.shape[::-1])][::-1]
+    return self.slice([(0,s) for s in self.shape[:-(len(padding)//2)]] + slc)
+
+  @property
+  def T(self) -> Tensor: return self.transpose()
+  def transpose(self, ax1=1, ax2=0) -> Tensor:
+    order = list(range(len(self.shape)))
+    order[ax1], order[ax2] = order[ax2], order[ax1]
+    return self.permute(order)
   def flatten(self, start_dim=0): return self.reshape(shape=tuple(list(self.shape[0:start_dim]) + [-1]))
 
   # ***** reduce ops *****
 
   def _reduce(self, fxn:Type[Function], axis:Optional[Union[int, Tuple[int, ...]]]=None, keepdim=False):
-    axis_ : List[int] = list(range(len(self.shape))) if axis is None else ([axis] if isinstance(axis, int) else list(axis))
+    axis_: List[int] = list(range(len(self.shape))) if axis is None else ([axis] if isinstance(axis, int) else list(axis))
     axis_ = [x if x >= 0 else x+len(self.shape) for x in axis_]
     shape = [self.shape[i] for i in range(len(self.shape)) if i not in axis_]
     ret = fxn.apply(self, new_shape=tuple(1 if i in axis_ else self.shape[i] for i in range(len(self.shape))))
     return ret if keepdim else ret.reshape(shape=[1] if shape == [] else shape)
 
   def sum(self, axis=None, keepdim=False): return self._reduce(mlops.Sum, axis, keepdim)
   def max(self, axis=None, keepdim=False): return self._reduce(mlops.Max, axis, keepdim)
   def min(self, axis=None, keepdim=False): return -((-self).max(axis=axis, keepdim=keepdim))
 
   def mean(self, axis=None, keepdim=False):
     out = self.sum(axis=axis, keepdim=keepdim)
     return out * (prod(out.shape)/prod(self.shape))
-
+  # TODO: implement unbiased True option for torch bessel's correction (subtracting 1 from divisor causes 0.01 error)
+  def std(self, axis=None, keepdim=False):
+    square_sum = ((self - self.mean(axis=axis, keepdim=True)).square()).sum(axis=axis, keepdim=keepdim)
+    return (square_sum * (prod(square_sum.shape)/prod(self.shape))).sqrt()
   def _softmax(self, axis):
     m = self - self.max(axis=axis, keepdim=True)
     e = m.exp()
     return m, e, e.sum(axis=axis, keepdim=True)
 
   def softmax(self, axis=-1):
     _, e, ss = self._softmax(axis)
@@ -284,124 +324,127 @@
 
   def log_softmax(self, axis=-1):
     m, _, ss = self._softmax(axis)
     return m - ss.log()
 
   # ***** processing ops *****
 
-  def _pool(self, k_:Tuple[int, ...], stride:Union[Tuple[int, ...], int]=1, dilation:Union[Tuple[int, ...], int]=1) -> Tensor:
+  def _pool(self, k_:Tuple[int, ...], stride:Union[Tuple[int, ...], int]=1, dilation:Union[Tuple[int, ...], int]=1, _insert_dims=tuple()) -> Tensor:
     assert len(self.shape) >= len(k_), f"can't pool {self.shape} with {k_}"
     s_, d_ = make_pair(stride, len(k_)), make_pair(dilation, len(k_))
     assert len(k_) == len(s_) and len(k_) == len(d_), f"stride/dilation mismatch kernel:{k_} stride:{s_} dilation:{d_}"
     slc_prefix, prefix, i_ = [(0,x) for x in self.shape[0:-len(k_)]], self.shape[0:-len(k_)], self.shape[-len(k_):]
     if any(k > s for k,s in zip(k_, s_)) or any(d != 1 for d in d_):
       o_ = [(i - d * (k-1) - 1)//s + 1 for i,d,k,s in zip(i_, d_, k_, s_)]
       e_ = [math.ceil(k*(i+d) / i) for k,i,d in zip(k_, i_, d_)]  # expands such that we don't need padding
-      xup = self.reshape(*prefix, *flatten((1,i) for i in i_)).expand(*prefix, *flatten((e,i) for e,i in zip(e_, i_))).reshape(*prefix, *[e*i for e,i in zip(e_, i_)])
+      xup = self.reshape(*prefix, *([1]*len(_insert_dims)), *flatten((1,i) for i in i_)).expand(*prefix, *_insert_dims, *flatten((e,i) for e,i in zip(e_, i_))).reshape(*prefix, *_insert_dims, *[e*i for e,i in zip(e_, i_)])
+      # NOTE: _insert_dims is required because reduces can't be merged (yet)
+      prefix += _insert_dims
+      slc_prefix += [(0,x) for x in _insert_dims]
       # slide by dilation
       xup = xup.slice(slc_prefix + [(0,k*(i+d)) for k,i,d in zip(k_, i_, d_)])
       xup = xup.reshape(*prefix, *flatten((k,i+d) for k,i,d in zip(k_, i_, d_)))
       xup = xup.slice(slc_prefix + flatten(((0,k), (0,o*s)) for k,o,s in zip(k_, o_, s_)))
       # handle stride, and permute to move reduce to the end
       xup = xup.reshape(*prefix, *flatten((k,o,s) for k,o,s in zip(k_, o_, s_)))
       xup = xup.slice(slc_prefix + flatten(((0,k), (0,o), (0,1)) for k,o in zip(k_, o_)))
       xup = xup.reshape(*prefix, *flatten((k,o) for k,o in zip(k_, o_)))
       return xup.permute(*range(len(prefix)), *[len(prefix)+i*2+1 for i in range(len(k_))], *[len(prefix)+i*2 for i in range(len(k_))])
     else:
       # TODO: once the shapetracker can optimize well, remove this alternative implementation. or not if the CPU implementation doesn't use ShapeTracker
       o_ = [(i+(s-k))//s for i,s,k in zip(i_, s_, k_)]
       xup = self.slice(slc_prefix + [(0,o*s) for o,s in zip(o_, s_)])
-      xup = xup.reshape(*prefix, *flatten(((o, s) for o,s in zip(o_, s_))))
+      xup = xup.reshape(*prefix, *([1]*len(_insert_dims)), *flatten(((o, s) for o,s in zip(o_, s_))))
+      if len(_insert_dims):
+        xup = xup.expand(*prefix, *_insert_dims, *flatten(((o, s) for o,s in zip(o_, s_))))
+        prefix += _insert_dims
+        slc_prefix += [(0,x) for x in _insert_dims]
       xup = xup.slice(slc_prefix + flatten(((0,o), (0,k)) for o,k in zip(o_, k_)))
       return xup.permute(*range(len(prefix)), *[len(prefix)+i*2 for i in range(len(k_))], *[len(prefix)+i*2+1 for i in range(len(k_))])
 
   # NOTE: these work for more than 2D
   def avg_pool2d(self, kernel_size=(2,2), stride=None): return self._pool(make_pair(kernel_size), stride if stride is not None else kernel_size).mean(axis=tuple(range(0-len(make_pair(kernel_size)), 0)))
   def max_pool2d(self, kernel_size=(2,2), stride=None): return self._pool(make_pair(kernel_size), stride if stride is not None else kernel_size).max(axis=tuple(range(0-len(make_pair(kernel_size)), 0)))
 
-  @image_conv2d_decorator
   def conv2d(self, weight:Tensor, bias:Optional[Tensor]=None, groups=1, stride=1, dilation=1, padding=0) -> Tensor:
-    (bs,cin_,_,_), (cout,cin,H,W) = self.shape, weight.shape
-    assert cin*groups == cin_, f"Input Tensor shape {self.shape} does not match the shape of the weights {weight.shape}. ({cin*groups} vs. {cin_})"
-    padding_ = [padding]*4 if isinstance(padding, int) else (padding if len(padding) == 4 else [padding[1], padding[1], padding[0], padding[0]])
+    (bs,cin_), (cout,cin), HW = self.shape[:2], weight.shape[:2], weight.shape[2:]
+    assert groups*cin == cin_ and len(self.shape) == len(weight.shape), f"Input Tensor shape {self.shape} does not match the shape of the weights {weight.shape}. ({groups*cin} vs. {cin_})"
+    padding_ = [padding]*4 if isinstance(padding, int) else (padding if len(padding) >= 4 else [padding[1], padding[1], padding[0], padding[0]])
 
     # conv2d is a pooling op (with padding)
-    x = self.pad2d(padding_)._pool((H,W),stride, dilation)
-
-    oy, ox, rcout = x.shape[2], x.shape[3], cout//groups
-    # NOTE: we do this expand explicitly so the permute isn't pushed in the binop
-    x = x.reshape(bs, groups, 1, cin, oy, ox, H, W).expand(bs, groups, rcout, cin, oy, ox, H, W).permute(0,1,2,4,5,3,6,7)
-
-    # conv! broadcasted to (bs, groups, rcout, oy, ox, cin, H, W)
-    ret = (x * weight.reshape(1, groups, rcout, 1, 1, cin, H, W)).sum((-3, -2, -1)).reshape(bs, cout, oy, ox)
-    return ret if bias is None else ret.add(bias.reshape(1, -1, 1, 1))
+    x = self.pad2d(padding_)._pool(HW, stride, dilation)   # (bs, groups*cin, oy, ox, H, W)
+    rcout, oyx = cout//groups, x.shape[2:-len(HW)]
+    x = x.reshape(bs, groups, cin, 1, *oyx, *HW).expand(bs, groups, cin, rcout, *oyx, *HW).permute(0,1,3,*[4+i for i in range(len(oyx))],2,*[4+len(oyx)+i for i in range(len(HW))])
+
+    # expand the channels with the pool
+    # TODO: this reduces the number of kernels, but it's slower!
+    #x = self.pad2d(padding_)._pool((H,W), stride, dilation, _insert_dims=(cout//groups,))   # (bs, groups*cin, rcout, oy, ox, H, W)
+    #rcout, oy, ox = x.shape[2:5]
+    #x = x.reshape(bs, groups, cin, rcout, oy, ox, H, W).permute(0,1,3,4,5,2,6,7)
+
+    # conv! broadcasted to (bs, groups, rcout, *oyx, cin, *HW)
+    ret = (x * weight.reshape(1, groups, rcout, *[1 for _ in range(len(oyx))], cin, *HW)).sum([-1-i for i in range(1+len(oyx))], keepdim=True).reshape(bs, cout, *oyx)
+    return ret if bias is None else ret.add(bias.reshape(1, -1, *[1 for _ in range(len(HW))]))
 
   def dot(self, w:Tensor) -> Tensor:
-    # NOTE: we use a 1x1 conv2d to do the matmul. mxk @ kxn = (1,k,m,1).conv2d(n,k,1,1)
-    bs, groups = prod(self.shape[0:-2]), prod(w.shape[0:-2])
-    cin, cout = w.shape[-2], w.shape[-1]
-    out_shape_t = self.shape[0:-2] + (cout,-1)
-    if len(self.shape) > 1:
-      order = tuple(range(len(self.shape)-2)) + (len(self.shape)-1, len(self.shape)-2)
-    else:
-      order, out_shape_t = (0,), (cout, )
-    worder = tuple(range(len(w.shape)-2)) + (len(w.shape)-1, len(w.shape)-2)
-
-    # NOTE: with NHWC we can remove the transposes
-    # bs x groups*cin x H x W
-    cx = self.transpose(order=order).reshape(shape=(bs//groups, groups*cin, -1, 1))
-    # groups*cout x cin x H, W
-    cw = w.transpose(order=worder).reshape(shape=(groups*cout, cin, 1, 1))
-    return cx.conv2d(cw, groups=groups).reshape(shape=out_shape_t).transpose(order=order)
+    x = self.reshape(*self.shape[0:-1], 1, self.shape[-1])
+    w = w.reshape(*w.shape[0:-2], 1, w.shape[-2], w.shape[-1]).transpose(-1, -2)
+    return (x*w).sum(-1).reshape(*x.shape[0:-2], -1)
 
   # ***** mlops (unary) *****
 
   def contiguous(self): return mlops.Contiguous.apply(self)
   def log(self): return mlops.Log.apply(self)
   def exp(self): return mlops.Exp.apply(self)
-
+  def relu(self): return mlops.Relu.apply(self)
+  def sin(self): return mlops.Sin.apply(self)
+  def cos(self): return ((math.pi/2)-self).sin()
+  def tan(self): return self.sin() / self.cos()
   # ***** math functions (unary) *****
 
   def __neg__(self): return 0.0-self
   def sqrt(self): return self.pow(0.5)
+  def rsqrt(self): return self.pow(-0.5)
   def square(self): return self*self
   def clip(self, min_, max_): return ((self-min_).relu()+min_) - (self-max_).relu()
   def abs(self): return self.relu() + (-self).relu()
   def sign(self): return self / (self.abs() + 1e-10)
-  def relu(self): return self.maximum(0)
   def reciprocal(self): return 1.0/self
 
   # ***** activation functions (unary) *****
 
   def sigmoid(self): return (1.0 + (-self).exp()).reciprocal()
   def elu(self, alpha=1.0): return self.relu() - alpha*(1-self.exp()).relu()
+  def celu(self, alpha=1.0): return self.maximum(0) + (alpha * ((self / alpha).exp() - 1)).minimum(0)
   def swish(self): return self * self.sigmoid()
   def silu(self): return self.swish()   # The SiLU function is also known as the swish function.
   def relu6(self): return self.relu() - (self-6).relu()
   def hardswish(self): return self * (self+3).relu6() * (1/6)
   def tanh(self): return 2.0 * ((2.0 * self).sigmoid()) - 1.0
+  def hardtanh(self, min_val=-1, max_val=1): return self.clip(min_val, max_val)
   def gelu(self): return 0.5 * self * (1 + (self * 0.7978845608 * (1 + 0.044715 * self * self)).tanh())
   def quick_gelu(self): return self * (self * 1.702).sigmoid()
   def leakyrelu(self, neg_slope=0.01): return self.relu() - (-neg_slope*self).relu()
   def mish(self): return self * self.softplus().tanh()
   def softplus(self, beta=1): return (1/beta) * (1 + (self*beta).exp()).log()
+  def softsign(self): return self / (1 + self.abs())
 
   # ***** broadcasted binary mlops *****
 
   def _broadcasted(self, fxn:Type[Function], other:Union[Tensor, float], reverse:bool=False) -> Tensor:
     x,y = [Tensor([t], device=self.device, requires_grad=False) if not isinstance(t, Tensor) else t for t in ([other,self] if reverse else [self,other])]
     x,y = [t.reshape([1]*(max(len(x.shape), len(y.shape))-len(t.shape)) + list(t.shape)) for t in [x,y]]
     shape_ret = tuple(max(sx, sy) for sx,sy in zip(x.shape, y.shape))
     return fxn.apply(x.expand(shape_ret), y.expand(shape_ret))
 
   def add(self, x:Union[Tensor, float], reverse=False) -> Tensor: return self._broadcasted(mlops.Add, x, reverse) if isinstance(x, Tensor) or x != 0.0 else self
   def sub(self, x:Union[Tensor, float], reverse=False) -> Tensor: return self._broadcasted(mlops.Sub, x, reverse) if isinstance(x, Tensor) or x != 0.0 or reverse else self
   def mul(self, x:Union[Tensor, float], reverse=False) -> Tensor: return self._broadcasted(mlops.Mul, x, reverse) if isinstance(x, Tensor) or x != 1.0 else self
   def pow(self, x:Union[Tensor, float], reverse=False) -> Tensor: return self._broadcasted(mlops.Pow, x, reverse) if isinstance(x, Tensor) or x != 1.0 or reverse else self
-  def div(self, x:Union[Tensor, float], reverse=False) -> Tensor: return self._broadcasted(mlops.Div, x, reverse) if isinstance(x, Tensor) or x != 1.0 or reverse else self
+  def div(self, x:Union[Tensor, float], reverse=False) -> Tensor: return self._broadcasted(mlops.Div, x, reverse) if isinstance(x, Tensor) or reverse else self.mul(1/x)
   def matmul(self, x:Tensor, reverse=False) -> Tensor: return x.dot(self) if reverse else self.dot(x)
 
   def maximum(self, x:Union[Tensor, float]) -> Tensor: return self._broadcasted(mlops.Maximum, x)
   def minimum(self, x:Union[Tensor, float]) -> Tensor: return -((-self).maximum(-x))
   def eq(self, x) -> Tensor: return self._broadcasted(mlops.Equal, x, False)
 
   # ***** binary op wrappers (18 wasted lines to make the typechecker happy) *****
@@ -428,33 +471,49 @@
   def __itruediv__(self, x) -> Tensor: return self.assign(self.div(x))
   def __imatmul__(self, x) -> Tensor: return self.assign(self.matmul(x))
 
   def __ge__(self, x) -> Tensor: return self.maximum(x).eq(self)
   def __le__(self, x) -> Tensor: return self.maximum(x).eq(x)
   def __lt__(self, x) -> Tensor: return 1.0-(self>=x)
   def __gt__(self, x) -> Tensor: return 1.0-(self<=x)
+  def __eq__(self, x) -> Tensor: return self.eq(x)  # type: ignore # mypy things this should be a bool
 
   # ***** functional nn ops *****
 
   def linear(self, weight:Tensor, bias:Optional[Tensor]=None):
     x = self.mul(weight) if len(weight.shape) == 1 else self.dot(weight)
     return x.add(bias) if bias is not None else x
 
   def sequential(self, ll:List[Callable[[Tensor], Tensor]]): return functools.reduce(lambda x,f: f(x), ll, self)
 
   def layernorm(self, axis=-1, eps:float=1e-5) -> Tensor:
-    y = (self - self.mean(axis=axis, keepdim=True))
-    return y.div((y*y).mean(axis=axis, keepdim=True).add(eps).sqrt())
+    y = (self - self.mean(axis, keepdim=True))
+    return y.mul((y*y).mean(axis, keepdim=True).add(eps).rsqrt())
 
-  def batchnorm(self, weight:Tensor, bias:Tensor, mean:Tensor, invstd:Tensor) -> Tensor:
-    x = (self - mean.reshape(shape=[1, -1, 1, 1])) * weight.reshape(shape=[1, -1, 1, 1])
-    return x.mul(invstd.reshape(shape=[1, -1, 1, 1])) + bias.reshape(shape=[1, -1, 1, 1])
+  def batchnorm(self, weight:Optional[Tensor], bias:Optional[Tensor], mean:Tensor, invstd:Tensor) -> Tensor:
+    x = (self - mean.reshape(shape=[1, -1, 1, 1]))
+    if weight: x = x * weight.reshape(shape=[1, -1, 1, 1])
+    ret = x.mul(invstd.reshape(shape=[1, -1, 1, 1]) if len(invstd.shape) == 1 else invstd)
+    return (ret + bias.reshape(shape=[1, -1, 1, 1])) if bias else ret
 
   def dropout(self, p=0.5) -> Tensor:
     if not Tensor.training: return self
-    _mask : np.ndarray = np.asarray(Tensor._rng.binomial(1, 1.0-p, size=self.shape), dtype=self.dtype)
+    # TODO: why is this going through numpy?
+    _mask: np.ndarray = np.asarray(Tensor._rng.binomial(1, 1.0-p, size=self.shape), dtype=np.float32)
     return self * Tensor(_mask, requires_grad=False, device=self.device) * (1/(1.0 - p))
 
+  # ***** cast ops *****
+
+  def cast(self, dtype:DType) -> Tensor: return mlops.Cast.apply(self, dtype=dtype) if self.dtype != dtype else self
+  def float(self) -> Tensor: return self.cast(dtypes.float32)
+  def half(self) -> Tensor: return self.cast(dtypes.float16)
+
 # register functions to move between devices
-for device in [device for device in Device._buffers.keys() if device[0] != "_"]:
+for device in Device._buffers:
   setattr(Tensor, f"{device.lower()}", functools.partialmethod(Tensor.to, device))
   setattr(Tensor, f"{device.lower()}_", functools.partialmethod(Tensor.to_, device))
+
+# if IMAGE>0 we install these replacement functions in Tensor (hack!)
+from tinygrad.nn.image import image_conv2d, image_dot
+if IMAGE:
+  setattr(Tensor, "conv2d", image_conv2d)
+  setattr(Tensor, "dot", image_dot)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tinygrad-0.5.0/tinygrad.egg-info/PKG-INFO` & `tinygrad-0.6.0/tinygrad.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: tinygrad
-Version: 0.5.0
-Summary: You like pytorch? You like micrograd? You love tinygrad! heart
+Version: 0.6.0
+Summary: You like pytorch? You like micrograd? You love tinygrad! <3
 Author: George Hotz
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: gpu
 Provides-Extra: llvm
 Provides-Extra: cuda
 Provides-Extra: triton
 Provides-Extra: metal
 Provides-Extra: linting
 Provides-Extra: testing
 License-File: LICENSE
@@ -38,14 +37,17 @@
 We are working on support for the Apple Neural Engine and the Google TPU in the `accel/` folder. Eventually, [we will build custom hardware](https://geohot.github.io/blog/jekyll/update/2021/06/13/a-breakdown-of-ai-chip-companies.html) for tinygrad, and it will be blindingly fast. Now, it is slow.
 
 This project is maintained by [tiny corp](https://tinygrad.org/).
 
 ### Installation
 
 ```bash
+python3 -m pip install git+https://git@github.com/geohot/tinygrad.git
+
+# or
 git clone https://github.com/geohot/tinygrad.git
 cd tinygrad
 python3 -m pip install -e .
 ```
 
 ### Contributing
 
@@ -86,27 +88,27 @@
 ```
 
 ## Is tinygrad fast?
 
 Try a matmul. See how, despite the style, it is fused into one kernel with the power of laziness.
 
 ```python
-DEBUG=3 OPTLOCAL=1 GPU=1 python3 -c "from tinygrad.tensor import Tensor;
+DEBUG=3 OPTLOCAL=1 python3 -c "from tinygrad.tensor import Tensor;
 N = 1024; a, b = Tensor.randn(N, N), Tensor.randn(N, N);
 c = (a.reshape(N, 1, N) * b.permute(1,0).reshape(1, N, N)).sum(axis=2);
 print((c.numpy() - (a.numpy() @ b.numpy())).mean())"
 ```
 
 Change to `DEBUG=4` to see the generated code.
 
 ## Neural networks?
 
-It turns out, a decent autograd tensor library is 90% of what you need for neural networks. Add an optimizer (SGD, RMSprop, and Adam implemented) from tinygrad.nn.optim, write some boilerplate minibatching code, and you have all you need.
+It turns out, a decent autograd tensor library is 90% of what you need for neural networks. Add an optimizer (SGD, Adam, AdamW implemented) from tinygrad.nn.optim, write some boilerplate minibatching code, and you have all you need.
 
-### Neural network example (from test/test_mnist.py)
+### Neural network example (from test/models/test_mnist.py)
 
 ```python
 from tinygrad.tensor import Tensor
 import tinygrad.nn.optim as optim
 
 class TinyBobNet:
   def __init__(self):
@@ -160,33 +162,33 @@
 hlops are syntactic sugar around mlops. They support most things torch does.
 
 ### mlops
 
 mlops are mid level ops. They understand derivatives. They are very simple.
 
 ```
-Log, Exp                                       # unary ops
+Relu, Log, Exp                                 # unary ops
 Sum, Max                                       # reduce ops (with axis argument)
 Maximum, Add, Sub, Mul, Pow, Div, Equal        # binary ops (no broadcasting, use expand)
 Expand, Reshape, Permute, Pad, Shrink, Flip    # movement ops
 ```
 
 You no longer need to write mlops for a new accelerator
 
 ### Adding an accelerator (llops)
 
 The autodiff stuff is all in mlops now so you can focus on the raw operations
 
 ```
-Buffer                                                     # class of memory on this device
-unary_op  (NOOP, NEG, NOT, EXP, LOG)                       # A -> A
-reduce_op (SUM, MAX)                                       # A -> B (smaller size, B has 1 in shape)
-binary_op (ADD, SUB, MUL, DIV, POW, CMPEQ, MAX)            # A + A -> A (all the same size)
-movement_op (EXPAND, RESHAPE, PERMUTE, PAD, SHRINK, FLIP)  # A -> B (different size)
-fused_op [[optional]] (MULACC)                             # A * A -> B
+Buffer                                                       # class of memory on this device
+unary_op  (NOOP, EXP, LOG, CAST)                             # A -> A
+reduce_op (SUM, MAX)                                         # A -> B (smaller size, B has 1 in shape)
+binary_op (ADD, SUB, MUL, DIV, POW, CMPEQ, MAX)              # A + A -> A (all the same size)
+movement_op (EXPAND, RESHAPE, PERMUTE, PAD, SHRINK, STRIDE)  # A -> B (different size)
+fused_op [[optional]] (MULACC)                               # A * A -> B
 ```
 
 ## ImageNet inference
 
 Despite being tiny, tinygrad supports the full EfficientNet. Pass in a picture to discover what it is.
 
 ```bash
@@ -195,23 +197,21 @@
 
 Or, if you have a webcam and cv2 installed
 
 ```bash
 ipython3 examples/efficientnet.py webcam
 ```
 
-PROTIP: Set "GPU=1" environment variable if you want this to go faster.
-
-PROPROTIP: Set "DEBUG=1" environment variable if you want to see why it's slow.
+PROTIP: Set "DEBUG=1" environment variable if you want to see why it's slow.
 
 ### tinygrad supports Stable Diffusion!
 
 You might need to download the [weight](https://huggingface.co/CompVis/stable-diffusion-v-1-4-original/resolve/main/sd-v1-4.ckpt) of Stable Diffusion and put it into weights/
 
-Run `GPU=1 python3 examples/stable_diffusion.py`
+Run `python3 examples/stable_diffusion.py`
 
 <p align="center">
   <img src="https://raw.githubusercontent.com/geohot/tinygrad/master/docs/stable_diffusion_by_tinygrad.jpg">
 </p>
 
 <p align="center">
 "a horse sized cat eating a bagel"
@@ -242,15 +242,15 @@
 * Nodes are Tensors
 * Black edge is a forward pass
 * Blue edge is a backward pass
 * Red edge is data the backward pass depends on
 * Purple edge is intermediates created in the forward
 
 ```bash
-GRAPH=1 python3 test/test_mnist.py TestMNIST.test_sgd_onestep
+GRAPH=1 python3 test/models/test_mnist.py TestMNIST.test_sgd_onestep
 # requires dot, outputs /tmp/net.svg
 ```
 
 ### Running tests
 
 For more examples on how to run the full test suite please refer to the [CI workflow](.github/workflows/test.yml).
```

### Comparing `tinygrad-0.5.0/tinygrad.egg-info/SOURCES.txt` & `tinygrad-0.6.0/tinygrad.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,46 @@
 LICENSE
 README.md
 setup.py
 test/test_assign.py
 test/test_conv.py
 test/test_conv_shapetracker.py
-test/test_example.py
+test/test_custom_function.py
+test/test_dtype.py
 test/test_gc.py
 test/test_jit.py
 test/test_net_speed.py
 test/test_nn.py
 test/test_ops.py
 test/test_optim.py
 test/test_randomness.py
 test/test_specific_conv.py
 test/test_speed_v_torch.py
 test/test_tensor.py
 tinygrad/graph.py
 tinygrad/helpers.py
-tinygrad/image.py
 tinygrad/jit.py
 tinygrad/lazy.py
 tinygrad/mlops.py
 tinygrad/ops.py
 tinygrad/tensor.py
 tinygrad.egg-info/PKG-INFO
 tinygrad.egg-info/SOURCES.txt
 tinygrad.egg-info/dependency_links.txt
 tinygrad.egg-info/requires.txt
 tinygrad.egg-info/top_level.txt
-tinygrad/codegen/ast.py
-tinygrad/codegen/gpu.py
-tinygrad/codegen/llvm.py
+tinygrad/codegen/cstyle.py
+tinygrad/codegen/linearizer.py
+tinygrad/codegen/llvmir.py
 tinygrad/nn/__init__.py
+tinygrad/nn/image.py
 tinygrad/nn/optim.py
+tinygrad/runtime/lib.py
 tinygrad/runtime/ops_clang.py
 tinygrad/runtime/ops_cpu.py
 tinygrad/runtime/ops_cuda.py
 tinygrad/runtime/ops_gpu.py
 tinygrad/runtime/ops_llvm.py
 tinygrad/runtime/ops_metal.py
 tinygrad/runtime/ops_torch.py
-tinygrad/shape/__init__.py
+tinygrad/shape/shapetracker.py
 tinygrad/shape/symbolic.py
```

