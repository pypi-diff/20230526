# Comparing `tmp/proteinflow-1.3.4.tar.gz` & `tmp/proteinflow-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteinflow-1.3.4.tar", last modified: Mon May 22 16:51:19 2023, max compression
+gzip compressed data, was "proteinflow-1.3.5.tar", last modified: Fri May 26 11:32:45 2023, max compression
```

## Comparing `proteinflow-1.3.4.tar` & `proteinflow-1.3.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.497694 proteinflow-1.3.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-22 16:51:07.000000 proteinflow-1.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-22 16:51:19.497694 proteinflow-1.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-05-22 16:51:07.000000 proteinflow-1.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.493694 proteinflow-1.3.4/proteinflow/
--rw-r--r--   0 runner    (1001) docker     (123)   100565 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.493694 proteinflow-1.3.4/proteinflow/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/scripts/proteinflow_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.497694 proteinflow-1.3.4/proteinflow/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/async_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/biotite_sse.py
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/build_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/cluster_and_partition.py
--rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/filter_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/mmcif_fix.py
--rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/process_pdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-22 16:51:07.000000 proteinflow-1.3.4/proteinflow/utils/split_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.493694 proteinflow-1.3.4/proteinflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-22 16:51:19.000000 proteinflow-1.3.4/proteinflow.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-22 16:51:07.000000 proteinflow-1.3.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-22 16:51:19.497694 proteinflow-1.3.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 16:51:19.497694 proteinflow-1.3.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-22 16:51:08.000000 proteinflow-1.3.4/tests/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-22 16:51:08.000000 proteinflow-1.3.4/tests/test_generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-22 16:51:08.000000 proteinflow-1.3.4/tests/test_sabdab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-26 11:32:30.000000 proteinflow-1.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-26 11:32:45.960125 proteinflow-1.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10922 2023-05-26 11:32:30.000000 proteinflow-1.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.956125 proteinflow-1.3.5/proteinflow/
+-rw-r--r--   0 runner    (1001) docker     (123)   100459 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/proteinflow/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/scripts/proteinflow_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/proteinflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/async_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/biotite_sse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/build_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41081 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/cluster_and_partition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3254 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/filter_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/mmcif_fix.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16980 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/process_pdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6594 2023-05-26 11:32:30.000000 proteinflow-1.3.5/proteinflow/utils/split_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/proteinflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-26 11:32:45.000000 proteinflow-1.3.5/proteinflow.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-05-26 11:32:30.000000 proteinflow-1.3.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:32:45.960125 proteinflow-1.3.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:32:45.960125 proteinflow-1.3.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-26 11:32:30.000000 proteinflow-1.3.5/tests/test_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-26 11:32:30.000000 proteinflow-1.3.5/tests/test_generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2063 2023-05-26 11:32:30.000000 proteinflow-1.3.5/tests/test_sabdab.py
```

### Comparing `proteinflow-1.3.4/LICENSE` & `proteinflow-1.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/PKG-INFO` & `proteinflow-1.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.4
+Version: 1.3.5
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.4 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.5 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-1.3.4/README.md` & `proteinflow-1.3.5/README.md`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/__init__.py` & `proteinflow-1.3.5/proteinflow/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -699,14 +699,15 @@
         self,
         mask_residues=True,
         lower_limit=15,
         upper_limit=100,
         mask_frac=None,
         mask_whole_chains=False,
         force_binding_sites_frac=0.15,
+        mask_all_cdrs=False,
     ):
         """
         Parameters
         ----------
         batch : dict
             a batch generated by `ProteinDataset` and `PadCollate`
         lower_limit : int, default 15
@@ -716,14 +717,16 @@
         mask_frac : float, optional
             if given, the `lower_limit` and `upper_limit` are ignored and the number of residues to mask is `mask_frac` times the length of the chain
         mask_whole_chains : bool, default False
             if `True`, `upper_limit`, `force_binding_sites` and `lower_limit` are ignored and the whole chain is masked instead
         force_binding_sites_frac : float, default 0.15
             if > 0, in the fraction of cases where a chain from a polymer is sampled, the center of the masked region will be
             forced to be in a binding site
+        mask_all_cdrs : bool, default False
+            if `True`, all CDRs are masked
 
         Returns
         -------
         chain_M : torch.Tensor
             a `(B, L)` shaped binary tensor where 1 denotes the part that needs to be predicted and
             0 is everything else
         """
@@ -731,14 +734,15 @@
         super().__init__()
         self.mask_residues = mask_residues
         self.lower_limit = lower_limit
         self.upper_limit = upper_limit
         self.mask_frac = mask_frac
         self.mask_whole_chains = mask_whole_chains
         self.force_binding_sites_frac = force_binding_sites_frac
+        self.mask_all_cdrs = mask_all_cdrs
 
     def _get_masked_sequence(
         self,
         batch,
     ):
         """
         Get the mask for the residues that need to be predicted
@@ -751,37 +755,29 @@
         If `force_binding_sites_frac` > 0 and `mask_whole_chains` is `False`, in the fraction of cases where a chain
         from a polymer is sampled, the center of the masked region will be forced to be in a binding site.
 
         Parameters
         ----------
         batch : dict
             a batch generated by `ProteinDataset` and `PadCollate`
-        lower_limit : int, default 15
-            the minimum number of residues to mask
-        upper_limit : int, default 100
-            the maximum number of residues to mask
-        mask_frac : float, optional
-            if given, the `lower_limit` and `upper_limit` are ignored and the number of residues to mask is `mask_frac` times the length of the chain
-        mask_whole_chains : bool, default False
-            if `True`, `upper_limit`, `force_binding_sites` and `lower_limit` are ignored and the whole chain is masked instead
-        force_binding_sites_frac : float, default 0.15
-            if > 0, in the fraction of cases where a chain from a polymer is sampled, the center of the masked region will be
-            forced to be in a binding site
 
         Returns
         -------
         chain_M : torch.Tensor
             a `(B, L)` shaped binary tensor where 1 denotes the part that needs to be predicted and
             0 is everything else
         """
         
         if "cdr" in batch and "cdr_id" in batch:
             chain_M = torch.zeros_like(batch["cdr"])
             for i, cdr_arr in enumerate(batch["cdr"]):
-                chain_M[i] = cdr_arr == batch["cdr_id"][i]
+                if self.mask_all_cdrs:
+                    chain_M[i] = cdr_arr != CDR["-"]
+                else:
+                    chain_M[i] = cdr_arr == batch["cdr_id"][i]
         else:
             chain_M = torch.zeros(batch["S"].shape)
             for i, coords in enumerate(batch["X"]):
                 chain_index = batch["chain_id"][i]
                 chain_bool = batch["chain_encoding_all"][i] == chain_index
 
                 if self.mask_whole_chains:
@@ -2267,14 +2263,15 @@
         upper_limit=100,
         mask_residues=True,
         mask_whole_chains=False,
         mask_frac=None,
         collate_func=_PadCollate,
         force_binding_sites_frac=0,
         shuffle_batches=True,
+        mask_all_cdrs=False,
         *args,
         **kwargs,
     ):
         """
         Parameters
         ----------
         dataset : ProteinDataset
@@ -2290,27 +2287,30 @@
         force_binding_sites_frac : float, default 0
             if > 0, in the fraction of cases where a chain from a polymer is sampled, the center of the masked region will be
             forced to be in a binding site
         shuffle_clusters : bool, default True
             if `True`, a new representative is randomly selected for each cluster at each epoch (if `clustering_dict_path` is given)
         shuffle_batches : bool, default True
             if `True`, the batches are shuffled at each epoch
+        mask_all_cdrs : bool, default False
+            if `True`, all CDRs are masked instead of just the sampled one
         collate_func : callable, optional
             a function that takes a list of samples and returns a batch and inherits from _PadCollate
         """
 
         super().__init__(
             dataset,
             collate_fn=collate_func(
                 mask_residues=mask_residues,
                 mask_whole_chains=mask_whole_chains,
                 mask_frac=mask_frac,
                 lower_limit=lower_limit,
                 upper_limit=upper_limit,
                 force_binding_sites_frac=force_binding_sites_frac,
+                mask_all_cdrs=mask_all_cdrs,
             ),
             shuffle=shuffle_batches,
             *args,
             **kwargs,
         )
 
     @staticmethod
@@ -2331,14 +2331,15 @@
         upper_limit=100,
         mask_residues=True,
         mask_whole_chains=False,
         mask_frac=None,
         force_binding_sites_frac=0,
         shuffle_clusters=True,
         shuffle_batches=True,
+        mask_all_cdrs=False,
         *args,
         **kwargs,
     ) -> None:
         """
         Creates a `ProteinLoader` instance with a `ProteinDataset` from the given arguments
 
         Parameters
@@ -2378,14 +2379,16 @@
         force_binding_sites_frac : float, default 0
             if > 0, in the fraction of cases where a chain from a polymer is sampled, the center of the masked region will be
             forced to be in a binding site
         shuffle_clusters : bool, default True
             if `True`, a new representative is randomly selected for each cluster at each epoch (if `clustering_dict_path` is given)
         shuffle_batches : bool, default True
             if `True`, the batches are shuffled at each epoch
+        mask_all_cdrs : bool, default False
+            if `True`, all CDRs are masked instead of just the sampled one
         """
 
         dataset = ProteinDataset(
             dataset_folder=dataset_folder,
             features_folder=features_folder,
             clustering_dict_path=clustering_dict_path,
             max_length=max_length,
@@ -2404,14 +2407,15 @@
             lower_limit=lower_limit,
             upper_limit=upper_limit,
             mask_residues=mask_residues,
             mask_whole_chains=mask_whole_chains,
             mask_frac=mask_frac,
             force_binding_sites_frac=force_binding_sites_frac,
             shuffle_batches=shuffle_batches,
+            mask_all_cdrs=mask_all_cdrs,
             *args,
             **kwargs,
         )
 
 
 def sidechain_order():
     """
```

### Comparing `proteinflow-1.3.4/proteinflow/scripts/proteinflow_cli.py` & `proteinflow-1.3.5/proteinflow/scripts/proteinflow_cli.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/utils/async_download.py` & `proteinflow-1.3.5/proteinflow/utils/async_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/utils/biotite_sse.py` & `proteinflow-1.3.5/proteinflow/utils/biotite_sse.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/utils/build_pdb.py` & `proteinflow-1.3.5/proteinflow/utils/build_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/utils/cluster_and_partition.py` & `proteinflow-1.3.5/proteinflow/utils/cluster_and_partition.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/utils/filter_database.py` & `proteinflow-1.3.5/proteinflow/utils/filter_database.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/utils/mmcif_fix.py` & `proteinflow-1.3.5/proteinflow/utils/mmcif_fix.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/utils/process_pdb.py` & `proteinflow-1.3.5/proteinflow/utils/process_pdb.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow/utils/split_dataset.py` & `proteinflow-1.3.5/proteinflow/utils/split_dataset.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/proteinflow.egg-info/PKG-INFO` & `proteinflow-1.3.5/proteinflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteinflow
-Version: 1.3.4
+Version: 1.3.5
 Summary: Versatile pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova <liza@adaptyvbio.com>, Arthur Valentin <arthur@adaptyvbio.com>
 License: BSD-3-Clause
 Keywords: bioinformatics,dataset,protein,PDB,deep learning
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: proteinflow Version: 1.3.4 Summary: Versatile
+Metadata-Version: 2.1 Name: proteinflow Version: 1.3.5 Summary: Versatile
 pipeline for processing protein structure data for deep learning applications.
 Author-email: Liza Kozlova
 adaptyvbio.com>, Arthur Valentin
 adaptyvbio.com> License: BSD-3-Clause Keywords:
 bioinformatics,dataset,protein,PDB,deep learning Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE
   ProteinFlow - A data processing pipeline for all your protein design needs
```

### Comparing `proteinflow-1.3.4/proteinflow.egg-info/SOURCES.txt` & `proteinflow-1.3.5/proteinflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/pyproject.toml` & `proteinflow-1.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "proteinflow"
-version = "1.3.4"
+version = "1.3.5"
 authors = [
     {name = "Liza Kozlova", email = "liza@adaptyvbio.com"},
     {name = "Arthur Valentin", email = "arthur@adaptyvbio.com"}
 ]
 description = "Versatile pipeline for processing protein structure data for deep learning applications."
 readme = "README.md"
 requires-python = ">=3.8"
@@ -33,8 +33,8 @@
 ]
 keywords = ["bioinformatics", "dataset", "protein", "PDB", "deep learning"]
 
 [project.scripts]
 proteinflow = "proteinflow.scripts.proteinflow_cli:cli"
 
 [tool.setuptools.packages]
-find = {}
+find = {}
```

### Comparing `proteinflow-1.3.4/tests/test_download.py` & `proteinflow-1.3.5/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/tests/test_generate.py` & `proteinflow-1.3.5/tests/test_generate.py`

 * *Files identical despite different names*

### Comparing `proteinflow-1.3.4/tests/test_sabdab.py` & `proteinflow-1.3.5/tests/test_sabdab.py`

 * *Files identical despite different names*

