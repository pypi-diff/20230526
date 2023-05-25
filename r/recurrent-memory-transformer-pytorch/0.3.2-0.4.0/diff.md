# Comparing `tmp/recurrent-memory-transformer-pytorch-0.3.2.tar.gz` & `tmp/recurrent-memory-transformer-pytorch-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recurrent-memory-transformer-pytorch-0.3.2.tar", last modified: Wed May  3 20:09:10 2023, max compression
+gzip compressed data, was "recurrent-memory-transformer-pytorch-0.4.0.tar", last modified: Thu May 25 22:35:36 2023, max compression
```

## Comparing `recurrent-memory-transformer-pytorch-0.3.2.tar` & `recurrent-memory-transformer-pytorch-0.4.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:09:10.516166 recurrent-memory-transformer-pytorch-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 20:09:10.516166 recurrent-memory-transformer-pytorch-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8121 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:09:10.512166 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/attend.py
--rw-r--r--   0 runner    (1001) docker     (123)    19184 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 20:09:10.516166 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 20:09:10.000000 recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 20:09:10.516166 recurrent-memory-transformer-pytorch-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 20:08:57.000000 recurrent-memory-transformer-pytorch-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/attend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-25 22:35:36.000000 recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 22:35:36.486204 recurrent-memory-transformer-pytorch-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-25 22:35:24.000000 recurrent-memory-transformer-pytorch-0.4.0/setup.py
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.2/LICENSE` & `recurrent-memory-transformer-pytorch-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.3.2/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.3.2
+Version: 0.4.0
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.2/README.md` & `recurrent-memory-transformer-pytorch-0.4.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -234,7 +234,17 @@
     author  = {Siyu Ding and Junyuan Shang and Shuohuan Wang and Yu Sun and Hao Tian and Hua Wu and Haifeng Wang},
     year    = {2021},
     eprint  = {2012.15688},
     archivePrefix = {arXiv},
     primaryClass = {cs.CL}
 }
 ```
+
+```bibtex
+@article{Xie2023ResiDualTW,
+  title     = {ResiDual: Transformer with Dual Residual Connections},
+  author    = {Shufang Xie and Huishuai Zhang and Junliang Guo and Xu Tan and Jiang Bian and Hany Hassan Awadalla and Arul Menezes and Tao Qin and Rui Yan},
+  journal   = {ArXiv},
+  year      = {2023},
+  volume    = {abs/2304.14802}
+}
+```
```

#### html2text {}

```diff
@@ -84,8 +84,12 @@
 Transformer Pretraining with Extra Normalization}, author = {Anonymous},
 booktitle = {Submitted to The Tenth International Conference on Learning
 Representations }, year = {2022}, url = {https://openreview.net/
 forum?id=GMYWzWztDx5}, note = {under review} } ``` ```bibtex @misc
 {ding2021erniedoc, title = {ERNIE-Doc: A Retrospective Long-Document Modeling
 Transformer}, author = {Siyu Ding and Junyuan Shang and Shuohuan Wang and Yu
 Sun and Hao Tian and Hua Wu and Haifeng Wang}, year = {2021}, eprint =
-{2012.15688}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ```
+{2012.15688}, archivePrefix = {arXiv}, primaryClass = {cs.CL} } ``` ```bibtex
+@article{Xie2023ResiDualTW, title = {ResiDual: Transformer with Dual Residual
+Connections}, author = {Shufang Xie and Huishuai Zhang and Junliang Guo and Xu
+Tan and Jiang Bian and Hany Hassan Awadalla and Arul Menezes and Tao Qin and
+Rui Yan}, journal = {ArXiv}, year = {2023}, volume = {abs/2304.14802} } ```
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/attend.py` & `recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/attend.py`

 * *Files identical despite different names*

### Comparing `recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py` & `recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch/recurrent_memory_transformer.py`

 * *Files 3% similar despite different names*

```diff
@@ -112,15 +112,14 @@
     def forward(self, x):
         x, gate = x.chunk(2, dim = -1)
         return x * F.gelu(gate)
 
 def FeedForward(dim, mult = 4):
     dim_inner = int(dim * mult * 2 / 3)
     return nn.Sequential(
-        RMSNorm(dim),
         Linear(dim, dim_inner * 2, bias = False),
         GEGLU(),
         RMSNorm(dim_inner),
         Linear(dim_inner, dim, bias = False)
     )
 
 # attention
@@ -143,31 +142,27 @@
 
         self.attend = Attend(
             causal = causal and not use_custom_causal_attn_mask,
             dropout = dropout,
             use_flash = use_flash_attn
         )
 
-        self.norm = RMSNorm(dim)
-
         self.to_q = Linear(dim, dim_inner)
         self.to_kv = Linear(dim, dim_inner * 2)
         self.to_out = Linear(dim_inner, dim)
 
     def forward(
         self,
         x,
         rotary_emb: Optional[Tuple[Tensor, Tensor]] = None,
         mask = None,
         xl_memories = None
     ):
         h = self.heads
 
-        x = self.norm(x)
-
         q = self.to_q(x)
         k, v = self.to_kv(x).chunk(2, dim = -1)
 
         q, k, v = map(lambda t: rearrange(t, 'b n (h d) -> b h n d', h = h), (q, k, v))
 
         next_xl_memories = torch.stack((k, v))
 
@@ -211,15 +206,14 @@
         rotary_pos_emb = False,
         token_shift = True,
         use_xl_memories = True,
         xl_mem_len = None,
         enhanced_xl_recurrence = False,     # add simple method for enhancing receptive field of xl memories, from ernie-doc paper
         emb_gradient_frac = 0.1,            # trick from cogview paper that leads to a bit more stability
         memory_not_causal = True,           # flash attention behaves a bit more optimally if causal mask is not explicitly passed in - but if the memories perform better without a causal mask, it is necessary to have this turned on
-        norm_write_memories = False,
     ):
         super().__init__()
         self.causal = causal
         self.seq_len = seq_len
 
         self.emb_gradient_frac = emb_gradient_frac
 
@@ -243,16 +237,14 @@
 
         self.read_memory_emb = nn.Parameter(torch.zeros(num_memory_tokens, dim))
         nn.init.normal_(self.read_memory_emb, std = 0.02)
 
         self.memory_tokens = nn.Parameter(torch.randn(num_memory_tokens, dim))
         nn.init.normal_(self.memory_tokens, std = 0.02)
 
-        self.write_memories_norm = RMSNorm(dim) if norm_write_memories else None
-
         # xl memories
 
         xl_mem_len = default(xl_mem_len, seq_len)
         assert xl_mem_len <= seq_len
         self.xl_mem_len = xl_mem_len
 
         self.use_xl_memories = use_xl_memories
@@ -268,21 +260,21 @@
                     dim = dim,
                     dim_head = dim_head,
                     causal = causal,
                     heads = heads,
                     use_flash_attn = use_flash_attn,
                     use_custom_causal_attn_mask = memory_not_causal
                 ),
-                FeedForward(dim = dim, mult = ff_mult)
+                RMSNorm(dim),
+                FeedForward(dim = dim, mult = ff_mult),
+                RMSNorm(dim)
             ]))
 
-        self.to_logits = nn.Sequential(
-            RMSNorm(dim),
-            nn.Linear(dim, num_tokens)
-        )
+        self.norm = RMSNorm(dim)
+        self.to_logits = nn.Linear(dim, num_tokens)
 
         self.ignore_index = ignore_index
 
         # whether to use custom attention mask if causal and memory should not be causal
 
         self.use_custom_causal_attn_mask = causal and memory_not_causal
 
@@ -388,37 +380,44 @@
         new_xl_memories = []
 
         if has_xl_memories and self.enhanced_xl_recurrence and len(xl_memories) > 1:  # simply shift all the xl memories down by one, so lower layer gets access to representations from layer above
             xl_memories = [*xl_memories[1:], xl_memories[0]]
 
         # attention and feedforward
 
-        for attn, ff in self.layers:
+        residual = x
+
+        for attn, attn_post_norm, ff, ff_post_norm in self.layers:
             attn_out, xl_memories = attn(shift_fn(x), mask = mask, xl_memories = next(xl_memories_iter, None), rotary_emb = rotary_emb)
             new_xl_memories.append(xl_memories)
 
-            x = x + attn_out
+            x = attn_post_norm(x + attn_out)
 
-            x = ff(shift_fn(x)) + x
+            residual = residual + attn_out
+
+            ff_out = ff(shift_fn(x))
+
+            x = ff_post_norm(x + ff_out)
+
+            residual = residual + ff_out
 
         # whether to return xl memories
 
         next_xl_memories = None
 
         if self.use_xl_memories:
             next_xl_memories = list(map(lambda t: torch.detach(t[..., -self.xl_mem_len:, :]), new_xl_memories))
 
-        # split out memories using unpack
+        # add final norm of residual, as in resiDual paper
 
-        read_memories, x, write_memories = unpack(x, ps, 'b * d')
+        x = x + self.norm(residual)
 
-        # whether to norm the write memories
+        # split out memories using unpack
 
-        if exists(self.write_memories_norm):
-            write_memories = self.write_memories_norm(write_memories)
+        read_memories, x, write_memories = unpack(x, ps, 'b * d')
 
         # to logits
 
         logits = self.to_logits(x)
 
         if not return_loss:
             return logits, write_memories, next_xl_memories
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.2/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO` & `recurrent-memory-transformer-pytorch-0.4.0/recurrent_memory_transformer_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: recurrent-memory-transformer-pytorch
-Version: 0.3.2
+Version: 0.4.0
 Summary: Recurrent Memory Transformer - Pytorch
 Home-page: https://github.com/lucidrains/recurrent-memory-transformer-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,recurrence,memory,long-context
 Classifier: Development Status :: 4 - Beta
```

### Comparing `recurrent-memory-transformer-pytorch-0.3.2/setup.py` & `recurrent-memory-transformer-pytorch-0.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'recurrent-memory-transformer-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.3.2',
+  version = '0.4.0',
   license='MIT',
   description = 'Recurrent Memory Transformer - Pytorch',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/recurrent-memory-transformer-pytorch',
   keywords = [
```

