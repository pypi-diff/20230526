# Comparing `tmp/abmap-0.1.3.tar.gz` & `tmp/abmap-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/net/scratch3/scratch3-3/chihoim/ablm/dist/.tmp-yrtrndem/abmap-0.1.3.tar", last modified: Mon May  8 21:08:26 2023, max compression
+gzip compressed data, was "/net/scratch3/scratch3-3/chihoim/ablm/dist/.tmp-p6kkklql/abmap-0.1.4.tar", last modified: Fri May 26 01:25:19 2023, max compression
```

## Comparing `abmap-0.1.3.tar` & `abmap-0.1.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 21:08:26.000000 abmap-0.1.3/
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1098 2023-02-28 02:48:26.000000 abmap-0.1.3/LICENSE.txt
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)       15 2023-02-28 02:50:10.000000 abmap-0.1.3/MANIFEST.in
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2656 2023-05-08 21:08:26.000000 abmap-0.1.3/PKG-INFO
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2174 2023-05-02 23:50:43.000000 abmap-0.1.3/README.md
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap/
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)      398 2023-05-02 23:51:18.000000 abmap-0.1.3/abmap/__init__.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1747 2023-04-28 00:51:56.000000 abmap-0.1.3/abmap/__main__.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)    10758 2023-04-28 00:51:56.000000 abmap-0.1.3/abmap/abmap_augment.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)      437 2023-03-02 06:59:12.000000 abmap-0.1.3/abmap/base_config.py
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap/commands/
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)       39 2023-03-02 05:58:52.000000 abmap-0.1.3/abmap/commands/__init__.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2395 2023-04-28 00:51:56.000000 abmap-0.1.3/abmap/commands/augment.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7504 2023-05-08 21:08:05.000000 abmap-0.1.3/abmap/commands/embed.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)    20348 2023-05-02 01:26:42.000000 abmap-0.1.3/abmap/commands/train.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    12204 2023-03-05 19:41:16.000000 abmap-0.1.3/abmap/dataloader.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)    12094 2023-03-02 06:10:26.000000 abmap-0.1.3/abmap/libraseq_preprocess.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    18789 2023-05-02 01:18:34.000000 abmap-0.1.3/abmap/model.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1531 2023-03-16 18:20:17.000000 abmap-0.1.3/abmap/mutate.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5626 2023-04-28 00:51:57.000000 abmap-0.1.3/abmap/plm_embed.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)    14912 2023-04-28 00:51:57.000000 abmap-0.1.3/abmap/sabdab_preprocess.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5700 2023-04-21 14:55:50.000000 abmap-0.1.3/abmap/utils.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)       18 2023-05-02 23:50:43.000000 abmap-0.1.3/abmap/version.py
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap.egg-info/
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)     2656 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap.egg-info/PKG-INFO
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      738 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap.egg-info/SOURCES.txt
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        1 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap.egg-info/dependency_links.txt
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       46 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap.egg-info/entry_points.txt
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      125 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap.egg-info/requires.txt
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       15 2023-05-08 21:08:25.000000 abmap-0.1.3/abmap.egg-info/top_level.txt
-drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-08 21:08:26.000000 abmap-0.1.3/analysis/
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        0 2023-02-24 06:16:30.000000 abmap-0.1.3/analysis/__init__.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    13874 2023-02-14 13:40:17.000000 abmap-0.1.3/analysis/briney_analysis.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     6033 2023-02-24 06:18:30.000000 abmap-0.1.3/analysis/covabdab_analyze.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    35361 2023-02-08 02:32:36.000000 abmap-0.1.3/analysis/desautels_analyze.py
--rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    37858 2023-02-08 02:32:36.000000 abmap-0.1.3/analysis/strucpred_analysis.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7143 2023-04-28 00:51:57.000000 abmap-0.1.3/analysis/thera_analysis.py
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)      436 2023-05-08 21:08:18.000000 abmap-0.1.3/pyproject.toml
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)       38 2023-05-08 21:08:26.000000 abmap-0.1.3/setup.cfg
--rw-r--r--   0 chihoim  (26113) chihoim  (26113)      986 2023-05-02 23:50:43.000000 abmap-0.1.3/setup.py
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-26 01:25:19.000000 abmap-0.1.4/
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1098 2023-02-28 02:48:26.000000 abmap-0.1.4/LICENSE.txt
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       15 2023-02-28 02:50:10.000000 abmap-0.1.4/MANIFEST.in
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2656 2023-05-26 01:25:19.000000 abmap-0.1.4/PKG-INFO
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2174 2023-05-02 23:50:43.000000 abmap-0.1.4/README.md
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap/
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      435 2023-05-26 01:23:16.000000 abmap-0.1.4/abmap/__init__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1747 2023-04-28 00:51:56.000000 abmap-0.1.4/abmap/__main__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    10803 2023-05-26 01:23:16.000000 abmap-0.1.4/abmap/abmap_augment.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      437 2023-03-02 06:59:12.000000 abmap-0.1.4/abmap/base_config.py
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap/commands/
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       39 2023-03-02 05:58:52.000000 abmap-0.1.4/abmap/commands/__init__.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     2395 2023-04-28 00:51:56.000000 abmap-0.1.4/abmap/commands/augment.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7596 2023-05-26 01:24:21.000000 abmap-0.1.4/abmap/commands/embed.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    20348 2023-05-02 01:26:42.000000 abmap-0.1.4/abmap/commands/train.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    12204 2023-03-05 19:41:16.000000 abmap-0.1.4/abmap/dataloader.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    12094 2023-03-02 06:10:26.000000 abmap-0.1.4/abmap/libraseq_preprocess.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    19902 2023-05-26 01:23:16.000000 abmap-0.1.4/abmap/model.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     1531 2023-03-16 18:20:17.000000 abmap-0.1.4/abmap/mutate.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5626 2023-04-28 00:51:57.000000 abmap-0.1.4/abmap/plm_embed.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)    14912 2023-04-28 00:51:57.000000 abmap-0.1.4/abmap/sabdab_preprocess.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     5947 2023-05-26 01:23:16.000000 abmap-0.1.4/abmap/utils.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       18 2023-05-02 23:50:43.000000 abmap-0.1.4/abmap/version.py
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap.egg-info/
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)     2656 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap.egg-info/PKG-INFO
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      738 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap.egg-info/SOURCES.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        1 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap.egg-info/dependency_links.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       46 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap.egg-info/entry_points.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)      125 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap.egg-info/requires.txt
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)       15 2023-05-26 01:25:19.000000 abmap-0.1.4/abmap.egg-info/top_level.txt
+drwxr-xr-x   0 chihoim  (26113) chihoim  (26113)        0 2023-05-26 01:25:19.000000 abmap-0.1.4/analysis/
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)        0 2023-02-24 06:16:30.000000 abmap-0.1.4/analysis/__init__.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    13874 2023-02-14 13:40:17.000000 abmap-0.1.4/analysis/briney_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     6033 2023-02-24 06:18:30.000000 abmap-0.1.4/analysis/covabdab_analyze.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    35361 2023-02-08 02:32:36.000000 abmap-0.1.4/analysis/desautels_analyze.py
+-rw-rw-r--   0 chihoim  (26113) chihoim  (26113)    37858 2023-02-08 02:32:36.000000 abmap-0.1.4/analysis/strucpred_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)     7143 2023-04-28 00:51:57.000000 abmap-0.1.4/analysis/thera_analysis.py
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      436 2023-05-26 01:25:07.000000 abmap-0.1.4/pyproject.toml
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)       38 2023-05-26 01:25:19.000000 abmap-0.1.4/setup.cfg
+-rw-r--r--   0 chihoim  (26113) chihoim  (26113)      986 2023-05-02 23:50:43.000000 abmap-0.1.4/setup.py
```

### Comparing `abmap-0.1.3/LICENSE.txt` & `abmap-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/PKG-INFO` & `abmap-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abmap
-Version: 0.1.3
+Version: 0.1.4
 Summary: AbMAP: Antibody Mutagenesis Augmented Processing
 Author: Chiho Im, Taylor Sorenson, Abhinav Gupta, Rohit Singh
 Author-email: Chiho Im <chihoim@mit.edu>, Rohit Singh <rohitsingh@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `abmap-0.1.3/README.md` & `abmap-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/__main__.py` & `abmap-0.1.4/abmap/__main__.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/abmap_augment.py` & `abmap-0.1.4/abmap/abmap_augment.py`

 * *Files 5% similar despite different names*

```diff
@@ -219,15 +219,15 @@
         kmut_matr_h = self.create_kmut_matrix(num_muts=k, embed_type=embed_type)
         cdr_embed = self.create_cdr_embedding(kmut_matr_h, sep = separator, mask = mask)
 
         return cdr_embed
             
 
 def augment_from_fasta(fastaPath, outputPath, chain_type, embed_type,
-                       num_mutations, separators, cdr_masks,
+                       num_mutations, separators=False, cdr_masks=True,
                        device=0, verbose=False):
     """
     Embed sequences with existing PLMs and augment with mutagenesis & CDR isolation
     
     :param fastaPath: Input sequence file (``.fasta`` format)
     :type fastaPath: str
     :param outputPath: Output embedding file (``.h5`` format)
@@ -236,15 +236,15 @@
     :type device: int
     :param verbose: Print embedding progress
     :type verbose: bool
     """
 
     reload_models_to_device(device, embed_type)
 
-    use_cuda = (device >= 0) and torch.cuda.is_available()
+    use_cuda = isinstance(device, int) and torch.cuda.is_available()
     if use_cuda:
         torch.cuda.set_device(device)
         if verbose:
             log(f"# Using CUDA device {device} - {torch.cuda.get_device_name(device)}")
     else:
         if verbose:
             log("# Using CPU")
@@ -262,15 +262,15 @@
     log("# Storing to {}...".format(outputPath))
     # with torch.no_grad(), h5py.File(outputPath, "a") as h5fi:
     try:
         for (name, seq) in tqdm(zip(names, seqs), total=len(names)):
             fname = os.path.join(outputPath, f'{name}.p')
             if not os.path.isfile(fname):
             # if name not in h5fi:
-                prot = ProteinEmbedding(seq, chain_type, embed_device=f'cuda:{device}', dev=device)
+                prot = ProteinEmbedding(seq, chain_type, embed_device=f'cuda:{device}' if use_cuda else device, dev=device)
                 if num_mutations > 0:
                     z = prot.create_cdr_specific_embedding(embed_type, num_mutations,
                                                                         separators, cdr_masks)
                 else:
                     z = prot.create_cdr_embedding_nomut(embed_type, separators, cdr_masks)
 
                 with open(fname, 'wb') as f:
```

### Comparing `abmap-0.1.3/abmap/commands/augment.py` & `abmap-0.1.4/abmap/commands/augment.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/commands/embed.py` & `abmap-0.1.4/abmap/commands/embed.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,23 +76,26 @@
     dev = torch.device(f'cuda:{device}' if torch.cuda.is_available() else "cpu")
     reload_models_to_device(device, plm_name)
 
     # load pre-trained model into device
     if plm_name == 'beplerberger':
         pretrained = AbMAPAttn(embed_dim=2200, mid_dim2=1024, mid_dim3=512, 
                                      proj_dim=252, num_enc_layers=1, num_heads=16).to(dev)
-    if plm_name == 'protbert':
+    elif plm_name == 'protbert':
         pretrained = AbMAPAttn(embed_dim=1024, mid_dim2=512, mid_dim3=256, 
                                      proj_dim=252, num_enc_layers=1, num_heads=16).to(dev)
-    if plm_name == 'esm1b':
+    elif plm_name in ['esm1b', 'esm2']:
         pretrained = AbMAPAttn(embed_dim=1280, mid_dim2=512, mid_dim3=256, 
                                      proj_dim=252, num_enc_layers=1, num_heads=16).to(dev)
-    if plm_name == 'tape':
+    elif plm_name == 'tape':
         pretrained = AbMAPAttn(embed_dim=768, mid_dim2=256, mid_dim3=128, 
                                      proj_dim=60, num_enc_layers=1, num_heads=8).to(dev)
+    else:
+        raise ValueError(f"No such PLM named {plm_name}")
+    
     checkpoint = torch.load(pretrained_path, map_location=dev)
     if 'model_state_dict' in checkpoint:
         pretrained.load_state_dict(checkpoint['model_state_dict'])
     else:
         pretrained.load_state_dict(checkpoint)
     pretrained.eval()
     print("Loaded the Pre-trained Model!")
```

### Comparing `abmap-0.1.3/abmap/commands/train.py` & `abmap-0.1.4/abmap/commands/train.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/dataloader.py` & `abmap-0.1.4/abmap/dataloader.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/libraseq_preprocess.py` & `abmap-0.1.4/abmap/libraseq_preprocess.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/model.py` & `abmap-0.1.4/abmap/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -385,17 +385,21 @@
     def forward(self, x):
         x = self.predictor(x)
         # x = F.relu(x)
         x = torch.exp(x)
         return torch.squeeze(x)
 
 
-class BrineyPredictorAttn(nn.Module):
+class PropertyPredictorAttn(nn.Module):
+    '''
+    For predicting properties. 
+    If you're interested in change in free energy (ddG), use ddGPredictor.
+    '''
     def __init__(self, input_dim = 512, mid_dim1 = 128, mid_dim2 = 32, mid_dim3 = 8):
-        super(BrineyPredictorAttn, self).__init__()
+        super(PropertyPredictorAttn, self).__init__()
 
         self.activation = nn.LeakyReLU()
 
         self.predictor = nn.Sequential(
                                nn.Linear(input_dim, mid_dim1),
                                self.activation,
                                nn.Linear(mid_dim1, mid_dim2),
@@ -423,23 +427,34 @@
         x = self.attention(x, x_mask)
         x = torch.squeeze(self.predictor(x), dim=-1)
         x = torch.logsumexp(x, dim=-1)
         x = torch.sigmoid(x)
         return x
 
 
+class BrineyPredictorAttn(PropertyPredictorAttn):
+    def __init__(self):
+        super(PropertyPredictorAttn, self).__init__()
+    
+    
 
 def init_weights(m):
     if isinstance(m, nn.Linear):
         torch.nn.init.xavier_uniform_(m.weight, gain=0.01)
 
-class DesautelsPredictor(nn.Module):
+
+
+class ddGPredictor(nn.Module):
+    '''
+    For predicting properties in which variants should be compared to a wildtype. 
+    For example, ddG is change in free energy, a difference between WT and a variant
+    '''
     def __init__(self, input_dim = 400, mid_dim = 64, embed_dim = 50, hidden_dim = 50, 
-                 output_dim = 5, dropout= 0.3, baseline = False, num_heads=16):
-        super(DesautelsPredictor, self).__init__()
+                 output_dim = 1, dropout= 0.3, baseline = False, num_heads=16):
+        super(ddGPredictor, self).__init__()
         self.activation = nn.LeakyReLU()
         num_enc_layers = 1
 
         self.predictor = nn.Sequential(
                             nn.Linear(input_dim, mid_dim),
                             self.activation,
                             nn.Dropout(p=dropout),
@@ -457,33 +472,48 @@
         # Xavier Uniform
         if baseline:
             self.attention_H.apply(init_weights)
             self.attention_L.apply(init_weights)
 
 
     def attention(self, x, chain_type):
+        # Choose correct model (H or L, corresponding to heavy or light chain)
         if chain_type == 'H':
             mha = self.attention_H
         else:
             mha = self.attention_L
 
         if x.shape[-1] > 6000:
             x = x[:,:,-2200:]
 
         output = mha(x)
 
+        # Mean pooling: Average over sequence dimension
         pooled_output = torch.mean(output, dim=1)
 
         return pooled_output
 
     def forward(self, h, wt_h, l, wt_l):
-
+        '''
+        ddG prediction takes the difference between a variant embedding 
+        and its wildtype embeddings, but for VH and VL
+        '''
         if torch.isnan(h).any() or torch.isnan(wt_h).any() or torch.isnan(l).any() or torch.isnan(wt_l).any():
             raise ValueError
 
         h, wt_h = self.attention(h, 'H'), self.attention(wt_h, 'H')
         l, wt_l = self.attention(l, 'L'), self.attention(wt_l, 'L')
 
         x = torch.cat([h, h - wt_h, l, l - wt_l], dim=-1)
 
         output = self.predictor(x)
         return output
+    
+    
+
+class DesautelsPredictor(nn.Module):
+    def __init__(self, input_dim = 400, mid_dim = 64, embed_dim = 50, hidden_dim = 50, 
+                 output_dim = 5, dropout= 0.3, baseline = False, num_heads=16):
+        # Inherit from ddG Predictor with 5 output dimensions
+        super(ddGPredictor, self).__init__(output_dim=output_dim)
+        
+
```

### Comparing `abmap-0.1.3/abmap/mutate.py` & `abmap-0.1.4/abmap/mutate.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/plm_embed.py` & `abmap-0.1.4/abmap/plm_embed.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/sabdab_preprocess.py` & `abmap-0.1.4/abmap/sabdab_preprocess.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/abmap/utils.py` & `abmap-0.1.4/abmap/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,15 +43,16 @@
         target = target.detach().cpu().numpy()
     rho, pval = spearmanr(pred, target)
     return rho
 
 
 
 def get_boolean_mask(sequence, chain_type, scheme, buffer_region, dev, fold=0,
-                     anarci_dir='../data/anarci_files'):
+                     anarci_dir='../data/anarci_files', verbose=False):
+    # TODO: add support for a batch of sequences (e.g. as fasta file or iterable)
     chothia_nums = {'H': [[26, 32], [52, 56], [96, 101]],
                     'L': [[26, 32], [50, 52], [91, 96]]}
 
     # chothia_nums2 = {'H': [[26, 32], [52, 56], [95, 102]],
     #                  'L': [[24, 34], [50, 56], [89, 97]]}
 
     chothia_nums2 = {'H': [[24, 34], [50, 58], [94, 103]],
@@ -77,29 +78,32 @@
 
     # change temp_path to a folder you'd like to save your ANARCI file to
     # temp_path = "/net/scratch3.mit.edu/scratch3-3/chihoim/misc/temp{}".format(fold)
 
     if not os.path.isdir(anarci_dir):
         os.makedirs(anarci_dir)
     
+    
+    
+    # Output ANARCI file for an individual sequence
     temp_name = os.path.join(anarci_dir, 'temp{}'.format(dev))
-    print(temp_name)
-    print(f'Sequence: {sequence}')
-    print(f'scheme: {scheme}')
-
     os.system('ANARCI -i {} --csv -o {} -s {}'.format(sequence, temp_name, scheme))
+    # NOTE - add verbose option?
+    # print(temp_name)
+    # print(f'Sequence: {sequence}')
+    # print(f'scheme: {scheme}')
     
     ### debug!
     # print("chain_type variable:", chain_type)
 
-    regions = all_regions[chain_type]
+    # Find filename of ANARCI output
     if chain_type == 'H':
-        file_name = glob.glob(anarci_dir+'/'+'*{}_H.csv'.format(dev))[0]
+        file_name = glob.glob(os.path.join(anarci_dir, f'*{dev}_H.csv'))[0]
     else:
-        file_name = glob.glob(anarci_dir+'/'+'*{}_KL.csv'.format(dev))[0]
+        file_name = glob.glob(os.path.join(anarci_dir, f'*{dev}_KL.csv'))[0]
 
     try:
         temp = pd.read_csv(file_name)
     except:
         print("Can't READ this file! file name is: {}".format(file_name))
         raise ValueError
     df = pd.DataFrame(temp)
@@ -116,14 +120,16 @@
     if int(seq_list[0]) > 34 or int(seq_list[-1]) < 89:
         print(sequence)
         print(seq_list)
         raise ValueError
 
     cdr_mask = torch.zeros(len(sequence))
 
+
+    regions = all_regions[chain_type]
     seqstart_idx = df.iloc[0]['seqstart_index']
     for r, (start_val, end_val) in enumerate(regions):
         start_pointer, end_pointer = start_val, end_val
 
         found = False
         while not found:
             if str(start_pointer) in seq_list:
```

### Comparing `abmap-0.1.3/abmap.egg-info/PKG-INFO` & `abmap-0.1.4/abmap.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abmap
-Version: 0.1.3
+Version: 0.1.4
 Summary: AbMAP: Antibody Mutagenesis Augmented Processing
 Author: Chiho Im, Taylor Sorenson, Abhinav Gupta, Rohit Singh
 Author-email: Chiho Im <chihoim@mit.edu>, Rohit Singh <rohitsingh@gmail.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `abmap-0.1.3/abmap.egg-info/SOURCES.txt` & `abmap-0.1.4/abmap.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/analysis/briney_analysis.py` & `abmap-0.1.4/analysis/briney_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/analysis/covabdab_analyze.py` & `abmap-0.1.4/analysis/covabdab_analyze.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/analysis/desautels_analyze.py` & `abmap-0.1.4/analysis/desautels_analyze.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/analysis/strucpred_analysis.py` & `abmap-0.1.4/analysis/strucpred_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/analysis/thera_analysis.py` & `abmap-0.1.4/analysis/thera_analysis.py`

 * *Files identical despite different names*

### Comparing `abmap-0.1.3/setup.py` & `abmap-0.1.4/setup.py`

 * *Files identical despite different names*

