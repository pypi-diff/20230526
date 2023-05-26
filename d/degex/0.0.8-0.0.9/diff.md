# Comparing `tmp/degex-0.0.8.tar.gz` & `tmp/degex-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "degex-0.0.8.tar", last modified: Wed Mar  8 20:23:52 2023, max compression
+gzip compressed data, was "degex-0.0.9.tar", last modified: Fri Mar 10 14:50:11 2023, max compression
```

## Comparing `degex-0.0.8.tar` & `degex-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 sumner     (501) staff       (20)        0 2023-03-08 20:23:52.367168 degex-0.0.8/
--rw-rw-r--   0 sumner     (501) staff       (20)    11337 2022-09-05 16:31:43.000000 degex-0.0.8/LICENSE
--rw-rw-r--   0 sumner     (501) staff       (20)      111 2022-09-05 16:31:43.000000 degex-0.0.8/MANIFEST.in
--rw-r--r--   0 sumner     (501) staff       (20)      785 2023-03-08 20:23:52.366864 degex-0.0.8/PKG-INFO
--rw-r--r--   0 sumner     (501) staff       (20)      109 2023-02-28 16:45:54.000000 degex-0.0.8/README.md
-drwxr-xr-x   0 sumner     (501) staff       (20)        0 2023-03-08 20:23:52.364016 degex-0.0.8/degex/
--rw-r--r--   0 sumner     (501) staff       (20)       22 2023-03-08 20:23:46.000000 degex-0.0.8/degex/__init__.py
--rw-r--r--   0 sumner     (501) staff       (20)    12924 2023-03-08 20:23:46.000000 degex-0.0.8/degex/_modidx.py
--rw-r--r--   0 sumner     (501) staff       (20)    19521 2023-03-08 20:21:47.000000 degex-0.0.8/degex/adata.py
--rw-r--r--   0 sumner     (501) staff       (20)    19455 2023-03-08 20:23:46.000000 degex-0.0.8/degex/branches.py
--rw-r--r--   0 sumner     (501) staff       (20)      570 2023-03-08 20:21:47.000000 degex-0.0.8/degex/core.py
--rw-r--r--   0 sumner     (501) staff       (20)     3347 2023-03-08 20:21:47.000000 degex-0.0.8/degex/plots.py
--rw-r--r--   0 sumner     (501) staff       (20)     4922 2023-03-08 20:21:47.000000 degex-0.0.8/degex/preprocessing.py
--rw-r--r--   0 sumner     (501) staff       (20)     5257 2023-03-08 20:21:47.000000 degex-0.0.8/degex/types.py
--rw-r--r--   0 sumner     (501) staff       (20)     2540 2023-03-08 20:21:47.000000 degex-0.0.8/degex/utils.py
-drwxr-xr-x   0 sumner     (501) staff       (20)        0 2023-03-08 20:23:52.366467 degex-0.0.8/degex.egg-info/
--rw-r--r--   0 sumner     (501) staff       (20)      785 2023-03-08 20:23:52.000000 degex-0.0.8/degex.egg-info/PKG-INFO
--rw-r--r--   0 sumner     (501) staff       (20)      405 2023-03-08 20:23:52.000000 degex-0.0.8/degex.egg-info/SOURCES.txt
--rw-r--r--   0 sumner     (501) staff       (20)        1 2023-03-08 20:23:52.000000 degex-0.0.8/degex.egg-info/dependency_links.txt
--rw-r--r--   0 sumner     (501) staff       (20)       32 2023-03-08 20:23:52.000000 degex-0.0.8/degex.egg-info/entry_points.txt
--rw-r--r--   0 sumner     (501) staff       (20)        1 2023-02-28 16:33:51.000000 degex-0.0.8/degex.egg-info/not-zip-safe
--rw-r--r--   0 sumner     (501) staff       (20)      225 2023-03-08 20:23:52.000000 degex-0.0.8/degex.egg-info/requires.txt
--rw-r--r--   0 sumner     (501) staff       (20)        6 2023-03-08 20:23:52.000000 degex-0.0.8/degex.egg-info/top_level.txt
--rw-r--r--   0 sumner     (501) staff       (20)     1130 2023-03-08 20:23:46.000000 degex-0.0.8/settings.ini
--rw-r--r--   0 sumner     (501) staff       (20)       38 2023-03-08 20:23:52.367273 degex-0.0.8/setup.cfg
--rw-rw-r--   0 sumner     (501) staff       (20)     2541 2022-09-05 16:31:43.000000 degex-0.0.8/setup.py
+drwxr-xr-x   0 sumner     (501) staff       (20)        0 2023-03-10 14:50:11.606797 degex-0.0.9/
+-rw-rw-r--   0 sumner     (501) staff       (20)    11337 2022-09-05 16:31:43.000000 degex-0.0.9/LICENSE
+-rw-rw-r--   0 sumner     (501) staff       (20)      111 2022-09-05 16:31:43.000000 degex-0.0.9/MANIFEST.in
+-rw-r--r--   0 sumner     (501) staff       (20)      967 2023-03-10 14:50:11.606417 degex-0.0.9/PKG-INFO
+-rw-r--r--   0 sumner     (501) staff       (20)      291 2023-03-10 14:50:02.000000 degex-0.0.9/README.md
+drwxr-xr-x   0 sumner     (501) staff       (20)        0 2023-03-10 14:50:11.599474 degex-0.0.9/degex/
+-rw-r--r--   0 sumner     (501) staff       (20)       22 2023-03-10 14:49:46.000000 degex-0.0.9/degex/__init__.py
+-rw-r--r--   0 sumner     (501) staff       (20)    13390 2023-03-10 14:49:46.000000 degex-0.0.9/degex/_modidx.py
+-rw-r--r--   0 sumner     (501) staff       (20)    19521 2023-03-10 14:49:46.000000 degex-0.0.9/degex/adata.py
+-rw-r--r--   0 sumner     (501) staff       (20)    21299 2023-03-10 14:49:46.000000 degex-0.0.9/degex/branches.py
+-rw-r--r--   0 sumner     (501) staff       (20)      570 2023-03-10 14:49:46.000000 degex-0.0.9/degex/core.py
+-rw-r--r--   0 sumner     (501) staff       (20)     3347 2023-03-10 14:49:46.000000 degex-0.0.9/degex/plots.py
+-rw-r--r--   0 sumner     (501) staff       (20)     4922 2023-03-10 14:49:46.000000 degex-0.0.9/degex/preprocessing.py
+-rw-r--r--   0 sumner     (501) staff       (20)     5257 2023-03-10 14:49:46.000000 degex-0.0.9/degex/types.py
+-rw-r--r--   0 sumner     (501) staff       (20)     2540 2023-03-10 14:49:46.000000 degex-0.0.9/degex/utils.py
+drwxr-xr-x   0 sumner     (501) staff       (20)        0 2023-03-10 14:50:11.605509 degex-0.0.9/degex.egg-info/
+-rw-r--r--   0 sumner     (501) staff       (20)      967 2023-03-10 14:50:11.000000 degex-0.0.9/degex.egg-info/PKG-INFO
+-rw-r--r--   0 sumner     (501) staff       (20)      405 2023-03-10 14:50:11.000000 degex-0.0.9/degex.egg-info/SOURCES.txt
+-rw-r--r--   0 sumner     (501) staff       (20)        1 2023-03-10 14:50:11.000000 degex-0.0.9/degex.egg-info/dependency_links.txt
+-rw-r--r--   0 sumner     (501) staff       (20)       32 2023-03-10 14:50:11.000000 degex-0.0.9/degex.egg-info/entry_points.txt
+-rw-r--r--   0 sumner     (501) staff       (20)        1 2023-02-28 16:33:51.000000 degex-0.0.9/degex.egg-info/not-zip-safe
+-rw-r--r--   0 sumner     (501) staff       (20)      225 2023-03-10 14:50:11.000000 degex-0.0.9/degex.egg-info/requires.txt
+-rw-r--r--   0 sumner     (501) staff       (20)        6 2023-03-10 14:50:11.000000 degex-0.0.9/degex.egg-info/top_level.txt
+-rw-r--r--   0 sumner     (501) staff       (20)     1130 2023-03-10 14:25:34.000000 degex-0.0.9/settings.ini
+-rw-r--r--   0 sumner     (501) staff       (20)       38 2023-03-10 14:50:11.606905 degex-0.0.9/setup.cfg
+-rw-rw-r--   0 sumner     (501) staff       (20)     2541 2022-09-05 16:31:43.000000 degex-0.0.9/setup.py
```

### Comparing `degex-0.0.8/LICENSE` & `degex-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `degex-0.0.8/PKG-INFO` & `degex-0.0.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.8
+Version: 0.0.9
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
@@ -17,7 +17,21 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 DEtect Gene EXpression (degex)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+## Install
+
+``` sh
+# create conda environment
+$ conda env create -f env.yml
+
+# update conda environment
+$ conda env update -n degex --file env.yml
+```
+
+``` sh
+pip install degex
+```
```

### Comparing `degex-0.0.8/degex/_modidx.py` & `degex-0.0.9/degex/_modidx.py`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,16 @@
                                                                                          'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.branch_classes': ( 'branches.html#branchpointpredictor.branch_classes',
                                                                                         'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.branch_points': ( 'branches.html#branchpointpredictor.branch_points',
                                                                                        'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.classes': ( 'branches.html#branchpointpredictor.classes',
                                                                                  'degex/branches.py'),
+                                'degex.branches.BranchPointPredictor.diff_op': ( 'branches.html#branchpointpredictor.diff_op',
+                                                                                 'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.diffuse_dirac_for_end_points': ( 'branches.html#branchpointpredictor.diffuse_dirac_for_end_points',
                                                                                                       'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.dmap': ( 'branches.html#branchpointpredictor.dmap',
                                                                               'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.fit': ('branches.html#branchpointpredictor.fit', 'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.is_landmarked': ( 'branches.html#branchpointpredictor.is_landmarked',
                                                                                        'degex/branches.py'),
@@ -76,14 +78,16 @@
                                                                                'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.nbrs_dim_est': ( 'branches.html#branchpointpredictor.nbrs_dim_est',
                                                                                       'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.nn_dist': ( 'branches.html#branchpointpredictor.nn_dist',
                                                                                  'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.nn_idxs': ( 'branches.html#branchpointpredictor.nn_idxs',
                                                                                  'degex/branches.py'),
+                                'degex.branches.BranchPointPredictor.optimal_t': ( 'branches.html#branchpointpredictor.optimal_t',
+                                                                                   'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.plot_branch_classes': ( 'branches.html#branchpointpredictor.plot_branch_classes',
                                                                                              'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.plot_branchs': ( 'branches.html#branchpointpredictor.plot_branchs',
                                                                                       'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.pmn': ('branches.html#branchpointpredictor.pmn', 'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.pnm': ('branches.html#branchpointpredictor.pnm', 'degex/branches.py'),
                                 'degex.branches.BranchPointPredictor.transform': ( 'branches.html#branchpointpredictor.transform',
```

### Comparing `degex-0.0.8/degex/adata.py` & `degex-0.0.9/degex/adata.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.8/degex/branches.py` & `degex-0.0.9/degex/branches.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,40 +17,191 @@
 import numpy as np
 import graphtools
 from sklearn.neighbors import NearestNeighbors
 from sklearn.base import BaseEstimator, TransformerMixin
 import scprep, scipy as sp, phate
 
 class BranchPointPredictor(BaseEstimator, TransformerMixin):
-    def __init__(self, phate_op):
+    def __init__(
+        self, 
+        phate_op: phate.PHATE, # a trained PHATE operator
+        extrema_percentile:float = 50, # percentile to mask when calculating extrema
+        diffusion_iterations:int=20 # number of iterations to diffuse
+    ):
+        
         self.phate_op = phate_op
-
-        self.diff_op = phate_op.diff_op
-        self.optimal_t = phate_op.optimal_t
-     
-            
+        self.extrema_percentile = extrema_percentile
+        self.diffusion_iterations = diffusion_iterations
+                      
     def fit(self, X, y=None):
         self.diffuse_dirac_for_end_points()
         self.assign_branches(X)
         self.plot_branchs(X)
         self.plot_branch_classes(X)
         return self
     
     def transform(self, X):
         return self.classes
-        return X
+    
+
+    # NOTE: these two properties are for convenience of the developer
+    # and they just expose the underlying PHATE operator values
+    @property
+    def diff_op(self):
+        try:
+            return self.phate_op.diff_op
+        except AttributeError:
+            return None
+
+    @property
+    def optimal_t(self):
+        try:
+            return self.phate_op.optimal_t
+        except AttributeError:
+            return None
+    
 
+    # NOTE: listing all properties up top for readability
     @property
     def dmap(self):
+        '''
+        Returns the diffusion map calculated from the diffusion operator
+        '''
         try:
             return self._dmap
         except AttributeError:        
             self._calc_dmap()            
             return self._dmap 
+
+    @property
+    def n_use(self):
+        '''
+        The number of eigenvectors in the diffusion map to use
+        for downstream analyses
+        '''
+        try:
+            return self._n_use
+        except AttributeError:        
+            self._calc_num_to_consider()            
+            return self._n_use 
+
+    @property
+    def most_distinct_points(self):
+        '''
+        The most distinct points **prior** to downstream analysis.
+        These are the extrema.
+        '''
+        try:
+            return self._most_distinct_points
+        except AttributeError:        
+            self._calc_extrema()          
+            return self._most_distinct_points
        
+    @property
+    def is_landmarked(self):
+        '''
+        Whether or not the graph in the PHATE operator is a Landmark Graph
+        which matters when reconstructing class labels
+        '''
+        return isinstance(self.phate_op.graph, graphtools.graphs.kNNLandmarkGraph)
+    
+    # NOTE: these two properties are for handling reconstruction from the landmark operator
+    # back to the original data space.
+    @property
+    def pmn(self):
+        try:
+            return self.phate_op.graph.transitions
+        except Exception:        
+            return None
+        
+    @property
+    def pnm(self):
+        try:
+            return self.phate_op.graph._data_transitions()
+        except Exception:        
+            return None
+        
+    @property
+    def n_rows(self):
+        return self.pmn.shape[0] if self.pmn is not None else self.diff_op.shape[0]
+    
+    @property
+    def nn_dist(self):
+        '''
+        Nearest Neighbor distance matrix calculated on diffusion operator
+        '''
+        try:
+            return self._nn_dist
+        except AttributeError:
+            self._knn_on_diff_op()
+            return self._nn_dist
+        
+    @property
+    def nn_idxs(self):
+        '''
+        Nearest Neighbor indicies calculated on diffusion operator
+        '''
+        try:
+            return self._nn_idxs
+        except AttributeError:
+            self._knn_on_diff_op()
+            return self._nn_idxs
+        
+    @property
+    def n_nbrs(self):
+        try:
+            return self._n_nbrs
+        except AttributeError:
+            self.max_likelihood_pointwise_dimensionality_est()
+            return self._n_nbrs
+    
+    @property
+    def nbrs_dim_est(self):
+        try:
+            return self._nbrs_dim_est
+        except AttributeError:
+            self.max_likelihood_pointwise_dimensionality_est()
+            return self._nbrs_dim_est
+    
+    @property
+    def most_distinct_points_adjusted(self):
+        try:
+            return self._most_distinct_points_adjusted
+        except AttributeError:
+            self.max_likelihood_pointwise_dimensionality_est()
+            return self._most_distinct_points_adjusted
+
+    @property
+    def classes(self):
+        '''
+        Branch class labels
+        '''
+        try:
+            return self._classes
+        except AttributeError:
+            self.diffuse_dirac_for_end_points()
+            return self._classes
+        
+    @property
+    def branch_classes(self):
+        try:
+            return self._branch_classes
+        except AttributeError:
+            self.assign_branches(self.phate_op.X)
+            return self._branch_classes
+
+    @property
+    def branch_points(self):
+        try:
+            return self._branch_points
+        except AttributeError:
+            self.diffuse_dirac_for_end_points()
+            return self._branch_points
+    
+    # NOTE: sets property dmap
     def _calc_dmap(self, t=None):
         if t is None:
             t = self.optimal_t
 
         evals, evecs = np.linalg.eig(self.diff_op)
                 
         # sort eigenvectors in descending order
@@ -62,23 +213,16 @@
         evals = np.power(evals, self.optimal_t)
         evecs = evecs.dot(np.diag(evals))
 
         self.evals = evals
         self.evecs = evecs
         self._dmap = evecs   
         return evecs
-    
-    @property
-    def n_use(self):
-        try:
-            return self._n_use
-        except AttributeError:        
-            self._calc_num_to_consider()            
-            return self._n_use 
-        
+
+    # NOTE: sets property n_use      
     def _calc_num_to_consider(self):
         dmap = self.dmap
         evals = self.evals
         
         # Number of eigenvectors (~ dimensions) to consider.
         dmap_diff = evals - np.roll(evals, 1)
         
@@ -86,35 +230,30 @@
         # Increase the number of eigenvectors until 
         while (dmap_diff[n_evecs + 1] > 2 * dmap_diff[n_evecs]):
             n_evecs += 1
         
         self._n_use = n_evecs
         return n_evecs
     
-    @property
-    def most_distinct_points(self):
-        try:
-            return self._most_distinct_points
-        except AttributeError:        
-            self._calc_extrema()          
-            return self._most_distinct_points 
-    
-
+    # NOTE: sets property most_distinct_points
     def _calc_extrema(self):
+        # NOTE: these functions are equivalent, but
+        # v2 is used in latest version on GitHub and
+        # although v1 looks cleaner
         return self.__calc_extrema_v2()
         return self.__calc_extrema_v1()
     
     def __calc_extrema_v1(self):
         dmap = self.dmap
 
         # Ignore first (trivial) eigenvector
         dmap = dmap[:, 1:].copy()
 
         # Mask lower 50% abs val
-        lower_half_abs = np.percentile(np.abs(dmap), 50)
+        lower_half_abs = np.percentile(np.abs(dmap), self.extrema_percentile)
         dmap[np.abs(dmap) < lower_half_abs] = 0
 
         max_idxs = dmap.argmax(axis=0)
         min_idxs = dmap.argmin(axis=0)
         extrema_idxs = np.unique(np.hstack((max_idxs, min_idxs)))
         self._most_distinct_points = extrema_idxs
         return extrema_idxs
@@ -140,15 +279,15 @@
         most_distinct_points = []
 
         # Always skip the first trivial eigenvector
         for i in np.arange(n_consider):
             cur_eigvec = np.copy(dmap[:,i+1])
             # Sometimes the eigvectors are skewed towards one side (much more possitive values than negative 
             # values and vice versa). This part ensures only the extrema on the more significant side is taken.            
-            lower_half_abs = np.percentile(np.abs(cur_eigvec), 50)
+            lower_half_abs = np.percentile(np.abs(cur_eigvec), self.extrema_percentile)
             cur_eigvec[np.abs(cur_eigvec) < lower_half_abs] = 0
 
             max_eig = np.argmax(cur_eigvec)
             min_eig = np.argmin(cur_eigvec)
 
             if cur_eigvec[max_eig] > 0 and max_eig not in most_distinct_points:
                 most_distinct_points.append(max_eig)
@@ -156,55 +295,15 @@
             if cur_eigvec[min_eig] < 0 and min_eig not in most_distinct_points:
                 most_distinct_points.append(min_eig)
 
         most_distinct_points = np.array(most_distinct_points)
         self._most_distinct_points = most_distinct_points
         return most_distinct_points        
 
-    @property
-    def is_landmarked(self):        
-        return isinstance(self.phate_op.graph, graphtools.graphs.kNNLandmarkGraph)
-    
-     
-    @property
-    def pmn(self):
-        try:
-            return self.phate_op.graph.transitions
-        except Exception:        
-            return None
-        
-    @property
-    def pnm(self):
-        try:
-            return self.phate_op.graph._data_transitions()
-        except Exception:        
-            return None
-        
-    
-    @property
-    def n_rows(self):
-        return self.pmn.shape[0] if self.pmn is not None else self.diff_op.shape[0]
-    
-    @property
-    def nn_dist(self):
-        try:
-            return self._nn_dist
-        except AttributeError:
-            self._knn_on_diff_op()
-            return self._nn_dist
-        
-    @property
-    def nn_idxs(self):
-        try:
-            return self._nn_idxs
-        except AttributeError:
-            self._knn_on_diff_op()
-            return self._nn_idxs
         
-    
     def _knn_on_diff_op(self):
         # NOTE: using KNN on diff_map is not invertable
         # i.e. need to revert landmark graph here!
         dmap = self.dmap
 
         #######################
         # INTRINSIC DIMENSION #
@@ -231,41 +330,15 @@
         nn_distances, nn_indices = nbrs.kneighbors(diff_map)
         nn_distances = nn_distances[:, 1:]
         nn_indices = nn_indices[:, 1:]
         self._nn_dist = nn_distances
         self._nn_idxs = nn_indices
         return nn_distances, nn_indices
 
-    @property
-    def n_nbrs(self):
-        try:
-            return self._n_nbrs
-        except AttributeError:
-            self.max_likelihood_pointwise_dimensionality_est()
-            return self._n_nbrs
-    
-    @property
-    def nbrs_dim_est(self):
-        try:
-            return self._nbrs_dim_est
-        except AttributeError:
-            self.max_likelihood_pointwise_dimensionality_est()
-            return self._nbrs_dim_est
-    
-    @property
-    def most_distinct_points_adjusted(self):
-        try:
-            return self._most_distinct_points_adjusted
-        except AttributeError:
-            self.max_likelihood_pointwise_dimensionality_est()
-            return self._most_distinct_points_adjusted
-    
     def max_likelihood_pointwise_dimensionality_est(self):
-        pnm = self.pnm
-        pmn = self.pmn
         n_rows = self.n_rows
         nn_dist = self.nn_dist
         nn_idxs = self.nn_idxs 
         most_distinct_points = np.copy(self.most_distinct_points)
 
         # Maximum Likelihood pointwise dimensionality estimation
         # Hill (1975), Levina and Bickel (2005)
@@ -289,29 +362,14 @@
         most_distinct_points = most_distinct_points[low_dim_est_mask]
 
         self._most_distinct_points_adjusted = most_distinct_points
         self._n_nbrs = n_nbrs
         self._nbrs_dim_est = nbrs_dim_est
         return n_nbrs, nbrs_dim_est
     
-    @property
-    def classes(self):
-        try:
-            return self._classes
-        except AttributeError:
-            self.diffuse_dirac_for_end_points()
-            return self._classes
-    @property
-    def branch_points(self):
-        try:
-            return self._branch_points
-        except AttributeError:
-            self.diffuse_dirac_for_end_points()
-            return self._branch_points
-    
     def diffuse_dirac_for_end_points(self):        
         n_nbrs = self.n_nbrs        
         nbrs_dim_est = self.nbrs_dim_est
         # NOTE: use adjusted distinct points from max_likelihood_pointwise_dimensionality_est
         most_distinct_points = self.most_distinct_points_adjusted
 
         ##################################
@@ -333,15 +391,15 @@
                 undo_diff = (pmn @ self.diff_op @ pnm)
                 diff_op_t = np.linalg.matrix_power(undo_diff, opt_t)
             else:
                 diff_op_t = np.linalg.matrix_power(self.diff_op, opt_t)            
 
             branch_point_dim_est_avg_cache = -float('inf')
 
-            for it in range(20):
+            for it in range(self.diffusion_iterations):
                 branch_from_end_point = diff_op_t[:, cur_end_point]
 
                 branch_max = np.max(branch_from_end_point)
                 branch_min = np.min(branch_from_end_point)
                 
                 branch_threshold = branch_min + (branch_max - branch_min) * 0.1
                 
@@ -395,37 +453,15 @@
         branch_points = np.delete(
             branch_points, 
             np.argwhere(np.isin(branch_points, points_to_exclude))
         )
         self._classes = classes
         self._branch_points = branch_points
         return branch_points
-    
-    def plot_branchs(self, emb):
-        most_distinct_points = self.most_distinct_points_adjusted
-        branch_points = self.branch_points
-        # Plot by class with end points and branch points
-        classes = self.classes        
-        ax = scprep.plot.scatter2d(emb, c=classes)
-        plot_numbers = np.repeat("", emb.shape[0])
-        plot_numbers[most_distinct_points] = np.arange(most_distinct_points.shape[0]) + 1
-        plot_numbers[branch_points] = "*"
-        bbox_props = dict(boxstyle="circle,pad=0.3", fc="w", ec="r", lw=2)
-        
-        for i, txt in enumerate(plot_numbers):
-            ax.annotate(txt, (emb[i][0], emb[i][1]), size=15, bbox=bbox_props)
 
-    @property
-    def branch_classes(self):
-        try:
-            return self._branch_classes
-        except AttributeError:
-            self.assign_branches(self.phate_op.X)
-            return self._branch_classes
-    
     def assign_branches(self, emb):
         ###################
         # ASSIGN BRANCHES #
         ###################
         dmap = self.dmap
         most_distinct_points = self.most_distinct_points_adjusted
 
@@ -448,14 +484,28 @@
         mdp_1 = np.argwhere(mdp_ranking==1)[:,1] + 1
         mdp_2 = np.argwhere(mdp_ranking==2)[:,1] + 1
         
         branch_classes = list(zip(mdp_1, mdp_2))
         branch_classes = [str(sorted(branch_class)) for branch_class in branch_classes]
         self._branch_classes = branch_classes 
 
+    def plot_branchs(self, emb):
+        most_distinct_points = self.most_distinct_points_adjusted
+        branch_points = self.branch_points
+        # Plot by class with end points and branch points
+        classes = self.classes        
+        ax = scprep.plot.scatter2d(emb, c=classes)
+        plot_numbers = np.repeat("", emb.shape[0])
+        plot_numbers[most_distinct_points] = np.arange(most_distinct_points.shape[0]) + 1
+        plot_numbers[branch_points] = "*"
+        bbox_props = dict(boxstyle="circle,pad=0.3", fc="w", ec="r", lw=2)
+        
+        for i, txt in enumerate(plot_numbers):
+            ax.annotate(txt, (emb[i][0], emb[i][1]), size=15, bbox=bbox_props)
+
     def plot_branch_classes(self, emb):
         branch_classes = self.branch_classes
         most_distinct_points = self.most_distinct_points_adjusted
 
         ax = scprep.plot.scatter2d(emb, c=branch_classes)
         
         plot_numbers = np.repeat("", emb.shape[0])
```

### Comparing `degex-0.0.8/degex/core.py` & `degex-0.0.9/degex/core.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.8/degex/plots.py` & `degex-0.0.9/degex/plots.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.8/degex/preprocessing.py` & `degex-0.0.9/degex/preprocessing.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.8/degex/types.py` & `degex-0.0.9/degex/types.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.8/degex/utils.py` & `degex-0.0.9/degex/utils.py`

 * *Files identical despite different names*

### Comparing `degex-0.0.8/degex.egg-info/PKG-INFO` & `degex-0.0.9/degex.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: degex
-Version: 0.0.8
+Version: 0.0.9
 Summary: Detect Gene Expression in Single-CEll data
 Home-page: https://github.com/dsm-72/degex
 Author: dsm-72
 Author-email: sumner.magruder@yale.edu
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python single cell detect gene expression spot marker genes
 Classifier: Development Status :: 4 - Beta
@@ -17,7 +17,21 @@
 Provides-Extra: dev
 License-File: LICENSE
 
 DEtect Gene EXpression (degex)
 ================
 
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
+
+## Install
+
+``` sh
+# create conda environment
+$ conda env create -f env.yml
+
+# update conda environment
+$ conda env update -n degex --file env.yml
+```
+
+``` sh
+pip install degex
+```
```

### Comparing `degex-0.0.8/settings.ini` & `degex-0.0.9/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [DEFAULT]
 repo = degex
 lib_name = degex
-version = 0.0.8
+version = 0.0.9
 min_python = 3.10
 license = apache2
 doc_path = _docs
 lib_path = degex
 nbs_path = nbs
 recursive = True
 tst_flags = notest
```

### Comparing `degex-0.0.8/setup.py` & `degex-0.0.9/setup.py`

 * *Files identical despite different names*

