# Comparing `tmp/BrainGB-1.0.3.tar.gz` & `tmp/BrainGB-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BrainGB-1.0.3.tar", last modified: Mon Mar 21 21:33:18 2022, max compression
+gzip compressed data, was "BrainGB-1.0.4.tar", last modified: Fri May 26 04:11:50 2023, max compression
```

## Comparing `BrainGB-1.0.3.tar` & `BrainGB-1.0.4.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2022-03-21 21:33:18.548492 BrainGB-1.0.3/
--rw-r--r--   0 daiyuanping   (503) staff       (20)     1084 2021-10-11 00:57:46.000000 BrainGB-1.0.3/LICENSE
--rw-r--r--   0 daiyuanping   (503) staff       (20)     2990 2022-03-21 21:33:18.548578 BrainGB-1.0.3/PKG-INFO
--rw-r--r--   0 daiyuanping   (503) staff       (20)     2470 2022-03-14 22:28:38.000000 BrainGB-1.0.3/README.md
--rw-r--r--   0 daiyuanping   (503) staff       (20)      103 2022-03-21 21:33:11.000000 BrainGB-1.0.3/pyproject.toml
--rw-r--r--   0 daiyuanping   (503) staff       (20)      809 2022-03-21 21:33:18.548888 BrainGB-1.0.3/setup.cfg
-drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2022-03-21 21:33:18.539790 BrainGB-1.0.3/src/
-drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2022-03-21 21:33:18.540901 BrainGB-1.0.3/src/BrainGB/
--rw-r--r--   0 daiyuanping   (503) staff       (20)        0 2022-03-21 20:59:22.000000 BrainGB-1.0.3/src/BrainGB/__init__.py
-drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2022-03-21 21:33:18.544405 BrainGB-1.0.3/src/BrainGB/dataset/
--rw-r--r--   0 daiyuanping   (503) staff       (20)       74 2022-02-18 15:00:24.000000 BrainGB-1.0.3/src/BrainGB/dataset/__init__.py
-drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2022-03-21 21:33:18.544860 BrainGB-1.0.3/src/BrainGB/dataset/abcd/
--rw-r--r--   0 daiyuanping   (503) staff       (20)        0 2022-02-20 20:05:31.000000 BrainGB-1.0.3/src/BrainGB/dataset/abcd/__init__.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     2812 2022-03-12 02:51:05.000000 BrainGB-1.0.3/src/BrainGB/dataset/abcd/load_abcd.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)      127 2022-02-18 15:02:18.000000 BrainGB-1.0.3/src/BrainGB/dataset/base_transform.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)      613 2022-02-18 01:46:40.000000 BrainGB-1.0.3/src/BrainGB/dataset/brain_data.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     4406 2022-03-12 02:51:05.000000 BrainGB-1.0.3/src/BrainGB/dataset/brain_dataset.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)      250 2022-02-17 15:38:16.000000 BrainGB-1.0.3/src/BrainGB/dataset/maskable_list.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     6455 2022-03-11 04:05:24.000000 BrainGB-1.0.3/src/BrainGB/dataset/transforms.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     2502 2022-02-17 15:38:16.000000 BrainGB-1.0.3/src/BrainGB/dataset/utils.py
-drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2022-03-21 21:33:18.547396 BrainGB-1.0.3/src/BrainGB/models/
--rw-r--r--   0 daiyuanping   (503) staff       (20)       92 2022-02-23 17:05:16.000000 BrainGB-1.0.3/src/BrainGB/models/__init__.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)      574 2022-03-14 21:40:41.000000 BrainGB-1.0.3/src/BrainGB/models/brainnn.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     6316 2022-03-14 21:28:34.000000 BrainGB-1.0.3/src/BrainGB/models/gat.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     5993 2022-03-14 21:28:34.000000 BrainGB-1.0.3/src/BrainGB/models/gcn.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     2915 2021-12-22 17:10:23.000000 BrainGB-1.0.3/src/BrainGB/models/losses.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)      843 2022-03-14 21:34:45.000000 BrainGB-1.0.3/src/BrainGB/models/mlp.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     2226 2022-01-20 23:22:17.000000 BrainGB-1.0.3/src/BrainGB/models/pna.py
-drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2022-03-21 21:33:18.548345 BrainGB-1.0.3/src/BrainGB/utils/
--rw-r--r--   0 daiyuanping   (503) staff       (20)      109 2022-03-07 04:09:16.000000 BrainGB-1.0.3/src/BrainGB/utils/__init__.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)      570 2022-02-18 03:12:50.000000 BrainGB-1.0.3/src/BrainGB/utils/bin_edges.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)      209 2022-02-18 15:24:40.000000 BrainGB-1.0.3/src/BrainGB/utils/get_y.py
--rw-r--r--   0 daiyuanping   (503) staff       (20)     1684 2022-03-07 04:09:16.000000 BrainGB-1.0.3/src/BrainGB/utils/mixup.py
-drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2022-03-21 21:33:18.541586 BrainGB-1.0.3/src/BrainGB.egg-info/
--rw-r--r--   0 daiyuanping   (503) staff       (20)     2990 2022-03-21 21:33:18.000000 BrainGB-1.0.3/src/BrainGB.egg-info/PKG-INFO
--rw-r--r--   0 daiyuanping   (503) staff       (20)      865 2022-03-21 21:33:18.000000 BrainGB-1.0.3/src/BrainGB.egg-info/SOURCES.txt
--rw-r--r--   0 daiyuanping   (503) staff       (20)        1 2022-03-21 21:33:18.000000 BrainGB-1.0.3/src/BrainGB.egg-info/dependency_links.txt
--rw-r--r--   0 daiyuanping   (503) staff       (20)      161 2022-03-21 21:33:18.000000 BrainGB-1.0.3/src/BrainGB.egg-info/requires.txt
--rw-r--r--   0 daiyuanping   (503) staff       (20)        8 2022-03-21 21:33:18.000000 BrainGB-1.0.3/src/BrainGB.egg-info/top_level.txt
+drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2023-05-26 04:11:50.812338 BrainGB-1.0.4/
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     1084 2021-10-11 00:57:46.000000 BrainGB-1.0.4/LICENSE
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     2954 2023-05-26 04:11:50.812406 BrainGB-1.0.4/PKG-INFO
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     2470 2022-03-14 22:28:38.000000 BrainGB-1.0.4/README.md
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      103 2022-03-21 21:33:11.000000 BrainGB-1.0.4/pyproject.toml
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      809 2023-05-26 04:11:50.812700 BrainGB-1.0.4/setup.cfg
+drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2023-05-26 04:11:50.804807 BrainGB-1.0.4/src/
+drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2023-05-26 04:11:50.805853 BrainGB-1.0.4/src/BrainGB/
+-rw-r--r--   0 daiyuanping   (503) staff       (20)        0 2022-03-21 20:59:22.000000 BrainGB-1.0.4/src/BrainGB/__init__.py
+drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2023-05-26 04:11:50.808466 BrainGB-1.0.4/src/BrainGB/dataset/
+-rw-r--r--   0 daiyuanping   (503) staff       (20)       74 2022-03-24 03:03:19.000000 BrainGB-1.0.4/src/BrainGB/dataset/__init__.py
+drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2023-05-26 04:11:50.809038 BrainGB-1.0.4/src/BrainGB/dataset/abcd/
+-rw-r--r--   0 daiyuanping   (503) staff       (20)        0 2022-02-20 20:05:31.000000 BrainGB-1.0.4/src/BrainGB/dataset/abcd/__init__.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     2842 2022-05-07 16:02:02.000000 BrainGB-1.0.4/src/BrainGB/dataset/abcd/load_abcd.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      127 2022-02-18 15:02:18.000000 BrainGB-1.0.4/src/BrainGB/dataset/base_transform.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      613 2022-02-18 01:46:40.000000 BrainGB-1.0.4/src/BrainGB/dataset/brain_data.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     4485 2022-05-07 16:07:23.000000 BrainGB-1.0.4/src/BrainGB/dataset/brain_dataset.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      250 2022-02-17 15:38:16.000000 BrainGB-1.0.4/src/BrainGB/dataset/maskable_list.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     6479 2022-08-06 14:49:08.000000 BrainGB-1.0.4/src/BrainGB/dataset/transforms.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     2494 2022-08-06 14:27:49.000000 BrainGB-1.0.4/src/BrainGB/dataset/utils.py
+drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2023-05-26 04:11:50.811232 BrainGB-1.0.4/src/BrainGB/models/
+-rw-r--r--   0 daiyuanping   (503) staff       (20)       92 2022-02-23 17:05:16.000000 BrainGB-1.0.4/src/BrainGB/models/__init__.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      574 2022-03-14 21:40:41.000000 BrainGB-1.0.4/src/BrainGB/models/brainnn.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     6247 2022-08-06 14:15:12.000000 BrainGB-1.0.4/src/BrainGB/models/gat.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     6042 2022-04-07 19:00:25.000000 BrainGB-1.0.4/src/BrainGB/models/gcn.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     2915 2021-12-22 17:10:23.000000 BrainGB-1.0.4/src/BrainGB/models/losses.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      843 2022-03-14 21:34:45.000000 BrainGB-1.0.4/src/BrainGB/models/mlp.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     2226 2022-01-20 23:22:17.000000 BrainGB-1.0.4/src/BrainGB/models/pna.py
+drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2023-05-26 04:11:50.812146 BrainGB-1.0.4/src/BrainGB/utils/
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      119 2022-05-07 16:02:02.000000 BrainGB-1.0.4/src/BrainGB/utils/__init__.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      570 2022-02-18 03:12:50.000000 BrainGB-1.0.4/src/BrainGB/utils/bin_edges.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      391 2022-05-07 16:07:23.000000 BrainGB-1.0.4/src/BrainGB/utils/get_y.py
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     1684 2022-03-07 04:09:16.000000 BrainGB-1.0.4/src/BrainGB/utils/mixup.py
+drwxr-xr-x   0 daiyuanping   (503) staff       (20)        0 2023-05-26 04:11:50.806531 BrainGB-1.0.4/src/BrainGB.egg-info/
+-rw-r--r--   0 daiyuanping   (503) staff       (20)     2954 2023-05-26 04:11:50.000000 BrainGB-1.0.4/src/BrainGB.egg-info/PKG-INFO
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      865 2023-05-26 04:11:50.000000 BrainGB-1.0.4/src/BrainGB.egg-info/SOURCES.txt
+-rw-r--r--   0 daiyuanping   (503) staff       (20)        1 2023-05-26 04:11:50.000000 BrainGB-1.0.4/src/BrainGB.egg-info/dependency_links.txt
+-rw-r--r--   0 daiyuanping   (503) staff       (20)      161 2023-05-26 04:11:50.000000 BrainGB-1.0.4/src/BrainGB.egg-info/requires.txt
+-rw-r--r--   0 daiyuanping   (503) staff       (20)        8 2023-05-26 04:11:50.000000 BrainGB-1.0.4/src/BrainGB.egg-info/top_level.txt
```

### Comparing `BrainGB-1.0.3/LICENSE` & `BrainGB-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/PKG-INFO` & `BrainGB-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: BrainGB
-Version: 1.0.3
+Version: 1.0.4
 Summary: Emory Brain Benchmark package
 Home-page: https://github.com/
 Author: Emory Brain Network
 Author-email: wdai26@emory.edu
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: BrainNet
 License-File: LICENSE
@@ -104,8 +102,7 @@
 
 - GCN
 - GAT
 
 # Contribution
 
 We welcome contributions to the package. Please feel free to open an issue or pull request. 
-
```

### Comparing `BrainGB-1.0.3/README.md` & `BrainGB-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/setup.cfg` & `BrainGB-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = BrainGB
-version = 1.0.3
+version = 1.0.4
 author = Emory Brain Network
 author_email = wdai26@emory.edu
 description = Emory Brain Benchmark package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/
 project_urls =
```

### Comparing `BrainGB-1.0.3/src/BrainGB/dataset/abcd/load_abcd.py` & `BrainGB-1.0.4/src/BrainGB/dataset/abcd/load_abcd.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,9 +63,10 @@
     return final_pearson, labels
 
 
 def load_data_abide(abide_path):
     data = np.load(abide_path + '/abide.npy', allow_pickle=True).item()
     final_pearson = data["corr"]
     labels = data["label"]
+    site = data['site']
 
-    return final_pearson, labels
+    return final_pearson, labels, site
```

### Comparing `BrainGB-1.0.3/src/BrainGB/dataset/brain_data.py` & `BrainGB-1.0.4/src/BrainGB/dataset/brain_data.py`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/src/BrainGB/dataset/brain_dataset.py` & `BrainGB-1.0.4/src/BrainGB/dataset/brain_dataset.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     def process(self):
         if self.name in ['ABCD', 'PNC', 'ABIDE']:
             if self.name == 'ABCD':
                 adj, y = load_data_abcd(self.raw_dir)
             elif self.name == 'PNC':
                 adj, y = load_data_pnc(self.raw_dir)
             elif self.name == 'ABIDE':
-                adj, y = load_data_abide(self.raw_dir)
+                adj, y, site = load_data_abide(self.raw_dir)
             y = torch.LongTensor(y)
             adj = torch.Tensor(adj)
             num_graphs = adj.shape[0]
             num_nodes = adj.shape[1]
         else:
             m = loadmat(osp.join(self.raw_dir, self.raw_file_names))
             if self.name == 'PPMI':
@@ -97,14 +97,16 @@
             y = torch.Tensor(m['label']).long().flatten()
             y[y == -1] = 0
 
         data_list = []
         for i in range(num_graphs):
             edge_index, edge_attr = dense_to_ind_val(adj[i])
             data = Data(num_nodes=num_nodes, y=y[i], edge_index=edge_index, edge_attr=edge_attr)
+            if self.name == 'ABIDE':
+                data.site = site[i]
             data_list.append(data)
 
         if self.pre_filter is not None:
             data_list = [data for data in data_list if self.pre_filter(data)]
 
         if self.pre_transform is not None:
             data_list = [self.pre_transform(data) for data in data_list]
```

### Comparing `BrainGB-1.0.3/src/BrainGB/dataset/transforms.py` & `BrainGB-1.0.4/src/BrainGB/dataset/transforms.py`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,16 @@
         """
         Returns node feature with degree bin transform.
         :param data: BrainData
         :return: torch.Tensor
         """
         adj = torch.sparse_coo_tensor(data.edge_index, data.edge_attr, [data.num_nodes, data.num_nodes])
         adj = adj.to_dense()
-        return torch.Tensor(binning(adj.sum(dim=1))).float()
+        data.x = torch.Tensor(binning(adj.sum(dim=1))).float()
+        return data
 
     def __str__(self):
         return 'Degree_Bin'
 
 
 class Adj(BaseTransform):
     def __call__(self, data: BrainData):
@@ -116,15 +117,15 @@
         :param data: BrainData
         :return: torch.Tensor
         """
         adj = torch.sparse_coo_tensor(data.edge_index, data.edge_attr, [data.num_nodes, data.num_nodes])
         adj = adj.to_dense()
         w, v = LA.eig(adj.numpy())
         # indices = np.argsort(w)[::-1]
-        v = v.transpose()
+        # v = v.transpose()
         data.x = torch.Tensor(v).float()
         return data
 
 
 class EigenNorm(BaseTransform):
     def __call__(self, data: BrainData):
         """
```

### Comparing `BrainGB-1.0.3/src/BrainGB/dataset/utils.py` & `BrainGB-1.0.4/src/BrainGB/dataset/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -73,14 +73,14 @@
             ]
 
     return x
 
 
 # for degree_bin node features
 def binning(a, n_bins=10):
-    n_graphs = a.shape[0]
-    n_nodes = a.shape[1]
+    # n_graphs = a.shape[0]
+    n_nodes = a.shape[0]
     _, bins = np.histogram(a, n_bins)
     binned = np.digitize(a, bins)
     binned = binned.reshape(-1, 1)
     enc = OneHotEncoder()
-    return enc.fit_transform(binned).toarray().reshape(n_graphs, n_nodes, -1).astype(np.float32)
+    return enc.fit_transform(binned).toarray().reshape(n_nodes, -1).astype(np.float32)
```

### Comparing `BrainGB-1.0.3/src/BrainGB/models/brainnn.py` & `BrainGB-1.0.4/src/BrainGB/models/brainnn.py`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/src/BrainGB/models/gat.py` & `BrainGB-1.0.4/src/BrainGB/models/gat.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,34 +9,33 @@
 from torch_geometric.nn.inits import glorot, zeros
 from torch_geometric.utils import softmax
 from torch import nn
 import torch_geometric
 
 
 class MPGATConv(GATConv):
-    def __init__(self, in_channels, out_channels, heads, gat_mp_type: str="attention_weighted"):
+    def __init__(self, in_channels, out_channels, heads, gat_mp_type: str = "attention_weighted"):
         super().__init__(in_channels, out_channels, heads)
 
         self.gat_mp_type = gat_mp_type
         input_dim = out_channels
         if gat_mp_type == "edge_node_concate":
-            input_dim = out_channels*2 + 1
+            input_dim = out_channels * 2 + 1
         elif gat_mp_type == "node_concate":
-            input_dim = out_channels*2
+            input_dim = out_channels * 2
         self.edge_lin = torch.nn.Linear(input_dim, out_channels)
 
-
     def message(self, x_i, x_j, alpha_j, alpha_i, edge_attr, index, ptr, size_i):
         alpha = alpha_j if alpha_i is None else alpha_j + alpha_i
         alpha = F.leaky_relu(alpha, self.negative_slope)
         alpha = softmax(alpha, index, ptr, size_i)
         self._alpha = alpha
         alpha = F.dropout(alpha, p=self.dropout, training=self.training)
 
-        attention_score = alpha.unsqueeze(-1)  
+        attention_score = alpha.unsqueeze(-1)
         edge_weights = torch.abs(edge_attr.view(-1, 1).unsqueeze(-1))
 
         if self.gat_mp_type == "attention_weighted":
             # (1) att: s^(l+1) = s^l * alpha
             msg = x_j * attention_score
             return msg
         elif self.gat_mp_type == "attention_edge_weighted":
@@ -45,15 +44,16 @@
             return msg
         elif self.gat_mp_type == "sum_attention_edge":
             # (3) m-att-1: s^(l+1) = s^l * (alpha + e), this one may not make sense cause it doesn't used attention score to control all
             msg = x_j * (attention_score + edge_weights)
             return msg
         elif self.gat_mp_type == "edge_node_concate":
             # (4) m-att-2: s^(l+1) = linear(concat(s^l, e) * alpha)
-            msg = torch.cat([x_i, x_j * attention_score, edge_attr.view(-1, 1).unsqueeze(-1).expand(-1, self.heads, -1)], dim=-1)
+            msg = torch.cat(
+                [x_i, x_j * attention_score, edge_attr.view(-1, 1).unsqueeze(-1).expand(-1, self.heads, -1)], dim=-1)
             msg = self.edge_lin(msg)
             return msg
         elif self.gat_mp_type == "node_concate":
             # (4) m-att-2: s^(l+1) = linear(concat(s^l, e) * alpha)
             msg = torch.cat([x_i, x_j * attention_score], dim=-1)
             msg = self.edge_lin(msg)
             return msg
@@ -82,46 +82,46 @@
         self.num_heads = num_heads
         self.num_layers = num_layers
         self.gat_mp_type = gat_mp_type
         self.dropout = dropout
 
         gat_input_dim = input_dim
 
-        for i in range(num_layers-1):
+        for i in range(num_layers - 1):
             conv = torch_geometric.nn.Sequential('x, edge_index, edge_attr', [
-                (MPGATConv(gat_input_dim, hidden_dim, heads=num_heads, dropout=dropout,
-                                 gat_mp_type=gat_mp_type),'x, edge_index, edge_attr -> x'),
-                nn.Linear(hidden_dim*num_heads, hidden_dim),
+                (MPGATConv(gat_input_dim, hidden_dim, heads=num_heads, gat_mp_type=gat_mp_type),
+                 'x, edge_index, edge_attr -> x'),
+                nn.Linear(hidden_dim * num_heads, hidden_dim),
                 nn.LeakyReLU(negative_slope=0.2),
                 nn.BatchNorm1d(hidden_dim)
             ])
             gat_input_dim = hidden_dim
             self.convs.append(conv)
 
         input_dim = 0
 
         if self.pooling == "concat":
             node_dim = 8
             conv = torch_geometric.nn.Sequential('x, edge_index, edge_attr', [
-                (MPGATConv(hidden_dim, hidden_dim, heads=num_heads, dropout=dropout,
-                                 gat_mp_type=gat_mp_type),'x, edge_index, edge_attr -> x'),
-                nn.Linear(hidden_dim*num_heads, 64),
+                (MPGATConv(hidden_dim, hidden_dim, heads=num_heads,
+                           gat_mp_type=gat_mp_type), 'x, edge_index, edge_attr -> x'),
+                nn.Linear(hidden_dim * num_heads, 64),
                 nn.LeakyReLU(negative_slope=0.2),
                 nn.Linear(64, node_dim),
                 nn.LeakyReLU(negative_slope=0.2),
                 nn.BatchNorm1d(node_dim)
             ])
-            input_dim = node_dim*num_nodes
+            input_dim = node_dim * num_nodes
 
         elif self.pooling == 'sum' or self.pooling == 'mean':
             node_dim = 256
             input_dim = node_dim
             conv = torch_geometric.nn.Sequential('x, edge_index, edge_attr', [
-                (MPGATConv(hidden_dim, hidden_dim, heads=num_heads, dropout=dropout,
-                                 gat_mp_type=gat_mp_type),'x, edge_index, edge_attr -> x'),
+                (MPGATConv(hidden_dim, hidden_dim, heads=num_heads, gat_mp_type=gat_mp_type),
+                 'x, edge_index, edge_attr -> x'),
                 nn.Linear(hidden_dim * num_heads, hidden_dim),
                 nn.LeakyReLU(negative_slope=0.2),
                 nn.BatchNorm1d(node_dim)
             ])
 
         self.convs.append(conv)
 
@@ -132,23 +132,21 @@
             nn.LeakyReLU(negative_slope=0.2),
             nn.Linear(32, num_classes)
         )
 
     def forward(self, x, edge_index, edge_attr, batch):
         z = x
         edge_attr = torch.abs(edge_attr)
-   
+
         for i, conv in enumerate(self.convs):
             # bz*nodes, hidden
             z = conv(z, edge_index, edge_attr)
 
         if self.pooling == "concat":
-            z = z.reshape((z.shape[0]//self.num_nodes, -1))
+            z = z.reshape((z.shape[0] // self.num_nodes, -1))
         elif self.pooling == 'sum':
-            z = global_add_pool(z,  batch)  # [N, F]
+            z = global_add_pool(z, batch)  # [N, F]
         elif self.pooling == 'mean':
             z = global_mean_pool(z, batch)  # [N, F]
 
         out = self.fcn(z)
         return out
-
-
```

### Comparing `BrainGB-1.0.3/src/BrainGB/models/gcn.py` & `BrainGB-1.0.4/src/BrainGB/models/gcn.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from torch_geometric.nn.inits import glorot, zeros
 from typing import Tuple
 from torch import Tensor
 from torch_geometric.nn import GCNConv
 from torch import nn
 import torch_geometric
 import math
+from torch_geometric.nn import SAGEConv, GATConv
 
 
 class MPGCNConv(GCNConv):
     def __init__(self, in_channels, out_channels, edge_emb_dim: int, gcn_mp_type: str, bucket_sz: float, 
                  normalize: bool = True, bias: bool = True):
         super(MPGCNConv, self).__init__(in_channels=in_channels, out_channels=out_channels, aggr='add')
```

### Comparing `BrainGB-1.0.3/src/BrainGB/models/losses.py` & `BrainGB-1.0.4/src/BrainGB/models/losses.py`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/src/BrainGB/models/mlp.py` & `BrainGB-1.0.4/src/BrainGB/models/mlp.py`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/src/BrainGB/models/pna.py` & `BrainGB-1.0.4/src/BrainGB/models/pna.py`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/src/BrainGB/utils/bin_edges.py` & `BrainGB-1.0.4/src/BrainGB/utils/bin_edges.py`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/src/BrainGB/utils/mixup.py` & `BrainGB-1.0.4/src/BrainGB/utils/mixup.py`

 * *Files identical despite different names*

### Comparing `BrainGB-1.0.3/src/BrainGB.egg-info/PKG-INFO` & `BrainGB-1.0.4/src/BrainGB.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 Metadata-Version: 2.1
 Name: BrainGB
-Version: 1.0.3
+Version: 1.0.4
 Summary: Emory Brain Benchmark package
 Home-page: https://github.com/
 Author: Emory Brain Network
 Author-email: wdai26@emory.edu
-License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: BrainNet
 License-File: LICENSE
@@ -104,8 +102,7 @@
 
 - GCN
 - GAT
 
 # Contribution
 
 We welcome contributions to the package. Please feel free to open an issue or pull request. 
-
```

### Comparing `BrainGB-1.0.3/src/BrainGB.egg-info/SOURCES.txt` & `BrainGB-1.0.4/src/BrainGB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

