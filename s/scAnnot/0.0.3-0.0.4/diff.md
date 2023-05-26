# Comparing `tmp/scAnnot-0.0.3.tar.gz` & `tmp/scAnnot-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scAnnot-0.0.3.tar", last modified: Wed May 10 13:15:38 2023, max compression
+gzip compressed data, was "scAnnot-0.0.4.tar", last modified: Fri May 26 03:27:20 2023, max compression
```

## Comparing `scAnnot-0.0.3.tar` & `scAnnot-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-10 13:15:38.000000 scAnnot-0.0.3/
--rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)    11337 2023-01-20 02:50:04.000000 scAnnot-0.0.3/LICENSE
--rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)      111 2023-01-20 02:50:04.000000 scAnnot-0.0.3/MANIFEST.in
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1666 2023-05-10 13:15:38.000000 scAnnot-0.0.3/PKG-INFO
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      890 2023-05-10 13:08:24.000000 scAnnot-0.0.3/README.md
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-10 13:15:38.000000 scAnnot-0.0.3/scAnnot/
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       22 2023-05-10 13:11:23.000000 scAnnot-0.0.3/scAnnot/__init__.py
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      369 2023-05-10 13:11:23.000000 scAnnot-0.0.3/scAnnot/_modidx.py
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     2880 2023-05-10 13:11:23.000000 scAnnot-0.0.3/scAnnot/core.py
-drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-10 13:15:38.000000 scAnnot-0.0.3/scAnnot.egg-info/
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1666 2023-05-10 13:15:35.000000 scAnnot-0.0.3/scAnnot.egg-info/PKG-INFO
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      324 2023-05-10 13:15:37.000000 scAnnot-0.0.3/scAnnot.egg-info/SOURCES.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-05-10 13:15:35.000000 scAnnot-0.0.3/scAnnot.egg-info/dependency_links.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       86 2023-05-10 13:15:35.000000 scAnnot-0.0.3/scAnnot.egg-info/entry_points.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-03-08 02:12:46.000000 scAnnot-0.0.3/scAnnot.egg-info/not-zip-safe
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       85 2023-05-10 13:15:35.000000 scAnnot-0.0.3/scAnnot.egg-info/requires.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        8 2023-05-10 13:15:35.000000 scAnnot-0.0.3/scAnnot.egg-info/top_level.txt
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1000 2023-05-10 13:03:56.000000 scAnnot-0.0.3/settings.ini
--rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       38 2023-05-10 13:15:38.000000 scAnnot-0.0.3/setup.cfg
--rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)     2560 2023-01-20 02:50:04.000000 scAnnot-0.0.3/setup.py
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-26 03:27:20.000000 scAnnot-0.0.4/
+-rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)    11337 2023-01-20 02:50:04.000000 scAnnot-0.0.4/LICENSE
+-rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)      111 2023-01-20 02:50:04.000000 scAnnot-0.0.4/MANIFEST.in
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1666 2023-05-26 03:27:20.000000 scAnnot-0.0.4/PKG-INFO
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      890 2023-05-10 13:08:24.000000 scAnnot-0.0.4/README.md
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-26 03:27:19.000000 scAnnot-0.0.4/scAnnot/
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       22 2023-05-26 03:23:53.000000 scAnnot-0.0.4/scAnnot/__init__.py
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      369 2023-05-26 03:23:54.000000 scAnnot-0.0.4/scAnnot/_modidx.py
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     3148 2023-05-26 03:23:53.000000 scAnnot-0.0.4/scAnnot/core.py
+drwxr-xr-x   0 huang_yin  (1166) miaozhichao  (1042)        0 2023-05-26 03:27:20.000000 scAnnot-0.0.4/scAnnot.egg-info/
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1666 2023-05-26 03:26:56.000000 scAnnot-0.0.4/scAnnot.egg-info/PKG-INFO
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)      324 2023-05-26 03:27:12.000000 scAnnot-0.0.4/scAnnot.egg-info/SOURCES.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-05-26 03:26:56.000000 scAnnot-0.0.4/scAnnot.egg-info/dependency_links.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       86 2023-05-26 03:26:57.000000 scAnnot-0.0.4/scAnnot.egg-info/entry_points.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        1 2023-03-08 02:12:46.000000 scAnnot-0.0.4/scAnnot.egg-info/not-zip-safe
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       85 2023-05-26 03:26:57.000000 scAnnot-0.0.4/scAnnot.egg-info/requires.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)        8 2023-05-26 03:26:58.000000 scAnnot-0.0.4/scAnnot.egg-info/top_level.txt
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)     1000 2023-05-26 03:22:04.000000 scAnnot-0.0.4/settings.ini
+-rw-r--r--   0 huang_yin  (1166) miaozhichao  (1042)       38 2023-05-26 03:27:20.000000 scAnnot-0.0.4/setup.cfg
+-rw-rw-r--   0 huang_yin  (1166) miaozhichao  (1042)     2560 2023-01-20 02:50:04.000000 scAnnot-0.0.4/setup.py
```

### Comparing `scAnnot-0.0.3/LICENSE` & `scAnnot-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `scAnnot-0.0.3/PKG-INFO` & `scAnnot-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scAnnot
-Version: 0.0.3
+Version: 0.0.4
 Summary: single cell annotation
 Home-page: https://github.com/changebio/scAnnot
 Author: Yin Huang
 Author-email: changebio@yeah.net
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `scAnnot-0.0.3/README.md` & `scAnnot-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `scAnnot-0.0.3/scAnnot/core.py` & `scAnnot-0.0.4/scAnnot/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,35 +10,40 @@
 from fastcore.script import *
 import warnings
 
 # %% ../nbs/00_core.ipynb 13
 @call_parse
 def scAnnot(h5:str, #the input h5ad file, must have row counts in X or layers
             output:str = None, # The path of output file. 1. None->output AnnData object with predicted labels, 2. a path end with h5ad->write out the AnnData. 3. a path end with csv-> write out the table of predicted labels. 
+            model_path='/home/huang_yin/projA/scBERT/model/twostep_2layer_subgenes/scanvi_3_epoch_model/',
+            ref_path='/home/huang_yin/projA/scBERT/model/reference_genes.h5ad',
             show:bool=False, #show umap plot. may not work in command line
+            latent:bool=False, #add scvi latent space to anndata
            ):
     warnings.filterwarnings("ignore")
     ad=sc.read(h5)
    
     if 'counts' not in ad.layers.keys():
         ad.layers['counts']=ad.X
     arr=ad.layers['counts'].data
     if not np.array_equal(arr, np.round(arr)):
         raise ValueError("Not all counts are integers")
     
     #concatenate query and ref
-    ref=sc.read('/home/huang_yin/projA/scBERT/model/reference_genes.h5ad')
-    ad=ad[:,ad.var.index.isin(ref.var.index)]
+    ref=sc.read(ref_path)
+    ref_var_idx=ref.var.index
+    ad=ad[:,ad.var.index.isin(ref_var_idx)]
     print(f'{ad.shape[1]} of genes are found in ref genes (total {ref.shape[1]}). The percentage is {ad.shape[1]/ref.shape[1]}')
     ad=ad.concatenate(ref,join='outer')[:-1] #remove ref cell
+    ad.var['inref']=ad.var.index.isin(ref_var_idx)
     if not ad.var.index.equals(ref.var.index):
         raise ValueError("The order of gene are not the same between query and reference")
     model=scvi.model.SCANVI.load_query_data(
             ad,
-            '/home/huang_yin/projA/scBERT/model/twostep_2layer_subgenes/scanvi_3_epoch_model/',
+            model_path,
             freeze_dropout = True,
             inplace_subset_query_vars = True,
         )
     
     ad.obs['predict_level1']=model.predict()
     
     if show:
@@ -56,16 +61,18 @@
         )
         ad.obs['predict_level2'][ad.obs.predict_level1==i]=model.predict()
     if show:
         latent.obs['predict_level1']=ad.obs['predict_level1'].tolist()
         latent.obs['predict_level2']=ad.obs['predict_level2'].tolist()
         sc.pp.neighbors(latent)
         sc.tl.umap(latent)
-        sc.pl.umap(latent,color=['predict_level1', 'predict_level2'],frameon=False)
+        sc.pl.umap(latent,color=['predict_level1', 'predict_level2'],frameon=False,ncols=1)
        
+    if latent:
+        ad.obsm['X_scvi']=latent.X
     if output is not None:
         if output.endswith('.csv'):
             ad.obs[['predict_level1','predict_level2']].to_csv(output)
             return
         if output.split('.')[-1] in ['h5ad','h5']:
             ad.write_h5ad(output)
             return
```

### Comparing `scAnnot-0.0.3/scAnnot.egg-info/PKG-INFO` & `scAnnot-0.0.4/scAnnot.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scAnnot
-Version: 0.0.3
+Version: 0.0.4
 Summary: single cell annotation
 Home-page: https://github.com/changebio/scAnnot
 Author: Yin Huang
 Author-email: changebio@yeah.net
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `scAnnot-0.0.3/settings.ini` & `scAnnot-0.0.4/settings.ini`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = scAnnot
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.4
 min_python = 3.7
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = scAnnot
 nbs_path = nbs
```

### Comparing `scAnnot-0.0.3/setup.py` & `scAnnot-0.0.4/setup.py`

 * *Files identical despite different names*

