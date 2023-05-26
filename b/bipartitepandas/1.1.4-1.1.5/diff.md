# Comparing `tmp/bipartitepandas-1.1.4.tar.gz` & `tmp/bipartitepandas-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bipartitepandas-1.1.4.tar", last modified: Sun Jan  8 21:44:07 2023, max compression
+gzip compressed data, was "bipartitepandas-1.1.5.tar", last modified: Fri May 26 18:48:02 2023, max compression
```

## Comparing `bipartitepandas-1.1.4.tar` & `bipartitepandas-1.1.5.tar`

### file list

```diff
@@ -1,34 +1,45 @@
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-01-08 21:44:07.346359 bipartitepandas-1.1.4/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1058 2022-07-24 19:52:06.000000 bipartitepandas-1.1.4/LICENSE
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2794 2023-01-08 21:44:07.346452 bipartitepandas-1.1.4/PKG-INFO
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2201 2023-01-08 21:39:31.000000 bipartitepandas-1.1.4/README.rst
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-01-08 21:44:07.344485 bipartitepandas-1.1.4/bipartitepandas/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      818 2022-09-02 23:11:52.000000 bipartitepandas-1.1.4/bipartitepandas/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    85764 2023-01-08 21:33:14.000000 bipartitepandas-1.1.4/bipartitepandas/bipartitebase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    32553 2022-09-03 22:00:33.000000 bipartitepandas-1.1.4/bipartitepandas/bipartitedataframe.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3582 2022-07-24 19:52:06.000000 bipartitepandas-1.1.4/bipartitepandas/bipartiteeventstudy.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    57942 2022-09-02 23:16:34.000000 bipartitepandas-1.1.4/bipartitepandas/bipartiteeventstudybase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3500 2023-01-08 21:22:33.000000 bipartitepandas-1.1.4/bipartitepandas/bipartiteeventstudycollapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3818 2022-09-02 23:16:52.000000 bipartitepandas-1.1.4/bipartitepandas/bipartiteextendedeventstudy.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    50571 2023-01-08 21:22:25.000000 bipartitepandas-1.1.4/bipartitepandas/bipartiteextendedeventstudybase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3758 2023-01-08 21:22:35.000000 bipartitepandas-1.1.4/bipartitepandas/bipartiteextendedeventstudycollapsed.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    27554 2022-09-02 23:16:54.000000 bipartitepandas-1.1.4/bipartitepandas/bipartitelong.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    72365 2023-01-08 21:22:26.000000 bipartitepandas-1.1.4/bipartitepandas/bipartitelongbase.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34407 2023-01-08 21:22:37.000000 bipartitepandas-1.1.4/bipartitepandas/bipartitelongcollapsed.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-01-08 21:44:07.345913 bipartitepandas-1.1.4/bipartitepandas/grouping/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.4/bipartitepandas/grouping/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3162 2022-07-24 19:52:06.000000 bipartitepandas-1.1.4/bipartitepandas/grouping/grouping.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-01-08 21:44:07.346216 bipartitepandas-1.1.4/bipartitepandas/measures/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.4/bipartitepandas/measures/__init__.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8462 2022-07-24 19:52:06.000000 bipartitepandas-1.1.4/bipartitepandas/measures/measures.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8604 2022-09-02 23:16:50.000000 bipartitepandas-1.1.4/bipartitepandas/simbipartite.py
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)    13173 2022-09-02 23:16:51.000000 bipartitepandas-1.1.4/bipartitepandas/util.py
-drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-01-08 21:44:07.345580 bipartitepandas-1.1.4/bipartitepandas.egg-info/
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2794 2023-01-08 21:44:07.000000 bipartitepandas-1.1.4/bipartitepandas.egg-info/PKG-INFO
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      945 2023-01-08 21:44:07.000000 bipartitepandas-1.1.4/bipartitepandas.egg-info/SOURCES.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)        1 2023-01-08 21:44:07.000000 bipartitepandas-1.1.4/bipartitepandas.egg-info/dependency_links.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       82 2023-01-08 21:44:07.000000 bipartitepandas-1.1.4/bipartitepandas.egg-info/requires.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)       16 2023-01-08 21:44:07.000000 bipartitepandas-1.1.4/bipartitepandas.egg-info/top_level.txt
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      103 2022-08-28 19:50:50.000000 bipartitepandas-1.1.4/pyproject.toml
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      763 2023-01-08 21:44:07.346857 bipartitepandas-1.1.4/setup.cfg
--rw-r--r--   0 adamoppenheimer   (501) staff       (20)      162 2023-01-08 21:43:24.000000 bipartitepandas-1.1.4/setup.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.650304 bipartitepandas-1.1.5/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1058 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/LICENSE
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2794 2023-05-26 18:48:02.650394 bipartitepandas-1.1.5/PKG-INFO
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2201 2023-01-08 21:39:31.000000 bipartitepandas-1.1.5/README.rst
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.647316 bipartitepandas-1.1.5/bipartitepandas/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      818 2022-09-02 23:11:52.000000 bipartitepandas-1.1.5/bipartitepandas/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86380 2023-05-26 18:39:16.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitebase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    32553 2022-09-03 22:00:33.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitedataframe.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3582 2023-05-26 18:35:42.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudy.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    58472 2023-05-26 18:17:43.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudybase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3500 2023-01-08 21:22:33.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudycollapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3818 2022-09-02 23:16:52.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudy.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    50571 2023-01-08 21:22:25.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudybase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3758 2023-01-08 21:22:35.000000 bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudycollapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    27925 2023-05-26 18:38:14.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitelong.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    75272 2023-05-26 18:15:28.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitelongbase.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34407 2023-01-08 21:22:37.000000 bipartitepandas-1.1.5/bipartitepandas/bipartitelongcollapsed.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.648379 bipartitepandas-1.1.5/bipartitepandas/grouping/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/bipartitepandas/grouping/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     3162 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/bipartitepandas/grouping/grouping.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.648664 bipartitepandas-1.1.5/bipartitepandas/measures/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       25 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/bipartitepandas/measures/__init__.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8462 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/bipartitepandas/measures/measures.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     8604 2022-09-02 23:16:50.000000 bipartitepandas-1.1.5/bipartitepandas/simbipartite.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    13173 2022-09-02 23:16:51.000000 bipartitepandas-1.1.5/bipartitepandas/util.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.648099 bipartitepandas-1.1.5/bipartitepandas.egg-info/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2794 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/PKG-INFO
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     1201 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/SOURCES.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)        1 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/dependency_links.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       82 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/requires.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)       16 2023-05-26 18:48:02.000000 bipartitepandas-1.1.5/bipartitepandas.egg-info/top_level.txt
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      103 2022-08-28 19:50:50.000000 bipartitepandas-1.1.5/pyproject.toml
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      763 2023-05-26 18:48:02.650776 bipartitepandas-1.1.5/setup.cfg
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)      162 2023-01-08 21:43:24.000000 bipartitepandas-1.1.5/setup.py
+drwxr-xr-x   0 adamoppenheimer   (501) staff       (20)        0 2023-05-26 18:48:02.650175 bipartitepandas-1.1.5/tests/
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2900 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    86879 2022-09-02 23:16:33.000000 bipartitepandas-1.1.5/tests/test_bpd_base.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    17659 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_clustering.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    34290 2023-05-26 18:42:55.000000 bipartitepandas-1.1.5/tests/test_bpd_connectedness.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    16145 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_custom.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2253 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_df.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4536 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_es.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     4978 2022-07-24 19:52:06.000000 bipartitepandas-1.1.5/tests/test_bpd_es_collapsed.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)    14606 2022-09-02 23:16:46.000000 bipartitepandas-1.1.5/tests/test_bpd_long.py
+-rw-r--r--   0 adamoppenheimer   (501) staff       (20)     2954 2022-08-06 18:51:15.000000 bipartitepandas-1.1.5/tests/test_bpd_long_collapsed.py
```

### Comparing `bipartitepandas-1.1.4/LICENSE` & `bipartitepandas-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/PKG-INFO` & `bipartitepandas-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipartitepandas
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python tools for bipartite labor data
 Home-page: https://github.com/tlamadon/bipartitepandas/
 Author: Thibaut Lamadon
 Author-email: thibaut.lamadon@gmail.com
 Project-URL: Documentation, https://tlamadon.github.io/bipartitepandas/
 Project-URL: GitHub, https://github.com/tlamadon/bipartitepandas/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bipartitepandas-1.1.4/README.rst` & `bipartitepandas-1.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/__init__.py` & `bipartitepandas-1.1.5/bipartitepandas/__init__.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartitebase.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartitebase.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 
             return frame
         return recollapse_loop_inner_inner
     return recollapse_loop_inner
 
 # Define default parameter dictionaries
 clean_params = ParamsDict({
-    'connectedness': (None, 'set', ['connected', 'strongly_connected', 'leave_out_observation', 'leave_out_spell', 'leave_out_match', 'leave_out_worker', 'leave_out_firm', None],
+    'connectedness': (None, 'set', ['connected', 'strongly_connected', 'leave_out_observation', 'leave_out_spell', 'leave_out_match', 'leave_out_worker', 'leave_out_firm', 'strongly_leave_out_observation', 'strongly_leave_out_spell', 'strongly_leave_out_match', 'strongly_leave_out_worker', None],
         '''
-            (default=None) When computing largest connected set of firms: if 'connected', keep observations in the largest connected set of firms; if 'strongly_connected', keep observations in the largest strongly connected set of firms; if 'leave_out_observation', keep observations in the largest leave-one-observation-out connected set; if 'leave_out_spell', keep observations in the largest leave-one-spell-out connected set; if 'leave_out_match', keep observations in the largest leave-one-match-out connected set; if 'leave_out_worker', keep observations in the largest leave-one-worker-out connected set; if 'leave_out_firm', keep observations in the largest leave-one-firm-out connected set; if None, keep all observations.
+            (default=None) When computing largest connected set of firms: if 'connected', keep observations in the largest connected set of firms; if 'strongly_connected', keep observations in the largest strongly connected set of firms; if 'leave_out_x', keep observations in the largest leave-one-x-out connected set; if 'strongly_leave_out_x', keep observations in the largest strongly connected set that is also leave-one-x-out connected (NOT leave-one-x-out strongly connected); if None, keep all observations.
         ''', None),
     'collapse_at_connectedness_measure': (False, 'type', bool,
         '''
             (default=False) If True, computing leave-out-spell connected set will collapse data at the spell level, and computing leave-out-match connected set will collapse data at the match level.
         ''', None),
     'component_size_variable': ('firms', 'set', ['len', 'length', 'firms', 'workers', 'stayers', 'movers', 'firms_plus_workers', 'firms_plus_stayers', 'firms_plus_movers', 'len_stayers', 'length_stayers', 'len_movers', 'length_movers', 'stays', 'moves'],
         '''
@@ -1178,15 +1178,15 @@
                 raise ValueError(error_msg)
 
     def _connected_components(self, connectedness='connected', component_size_variable='firms', drop_single_stayers=False, drop_returns_to_stays=False, is_sorted=False, copy=True):
         '''
         Update data to include only the largest component connected by movers.
 
         Arguments:
-            connectedness (str or None): if 'connected', keep observations in the largest connected set of firms; if 'strongly_connected', keep observations in the largest strongly connected set of firms; if 'leave_out_observation', keep observations in the largest leave-one-observation-out connected set; if 'leave_out_spell', keep observations in the largest leave-one-spell-out connected set; if 'leave_out_match', keep observations in the largest leave-one-match-out connected set; if 'leave_out_worker', keep observations in the largest leave-one-worker-out connected set; if 'leave_out_firm', keep observations in the largest leave-one-firm-out connected set; if None, keep all observations
+            connectedness (str or None): if 'connected', keep observations in the largest connected set of firms; if 'strongly_connected', keep observations in the largest strongly connected set of firms; if 'leave_out_x', keep observations in the largest leave-one-x-out connected set; if 'strongly_leave_out_x', keep observations in the largest strongly connected set that is also leave-one-x-out connected (NOT leave-one-x-out strongly connected); if None, keep all observations
             component_size_variable (str): how to determine largest connected component. Options are 'len'/'length' (length of frames), 'firms' (number of unique firms), 'workers' (number of unique workers), 'stayers' (number of unique stayers), 'movers' (number of unique movers), 'firms_plus_workers' (number of unique firms + number of unique workers), 'firms_plus_stayers' (number of unique firms + number of unique stayers), 'firms_plus_movers' (number of unique firms + number of unique movers), 'len_stayers'/'length_stayers' (number of stayer observations), 'len_movers'/'length_movers' (number of mover observations), 'stays' (number of stay observations), and 'moves' (number of move observations).
             drop_single_stayers (bool): if True, drop stayers who have <= 1 observation weight (check number of observations if data is unweighted)
             drop_returns_to_stays (bool): if True, when recollapsing collapsed data, drop observations that need to be recollapsed instead of collapsing (this is for computational efficiency when re-collapsing data for leave-one-out connected components, where intermediate observations can be dropped, causing a worker who returns to a firm to become a stayer)
             is_sorted (bool): if False, dataframe will be sorted by i (and t, if included). Returned dataframe is not guaranteed to be sorted if original dataframe is not sorted. Sorting may alter original dataframe if copy is set to False. Set is_sorted to True if dataframe is already sorted.
             copy (bool): if False, avoid copy
 
         Returns:
@@ -1231,25 +1231,28 @@
                         frame_largest_cc = frame_cc
             frame = frame_largest_cc
             try:
                 # Remove comp_size attribute
                 del frame.comp_size
             except AttributeError:
                 pass
-        elif connectedness in ['leave_out_observation', 'leave_out_spell', 'leave_out_match']:
+        elif connectedness in ['leave_out_observation', 'leave_out_spell', 'leave_out_match', 'strongly_leave_out_observation', 'strongly_leave_out_spell', 'strongly_leave_out_match']:
+            # Extract information about group and strong/weak connectedness
+            strongly_connected, leave_out_group = (connectedness.split('_')[0] == 'strongly'), connectedness.split('_')[-1]
             # Compute all connected components of firms (each entry is a connected component)
-            cc_list = G.components(mode='weak')
+            cc_list = G.components(mode={False: 'weak', True: 'strong'}[strongly_connected])
             # Keep largest leave-one-(observation/spell/match)-out component
-            leave_out_group = connectedness.split('_')[-1]
-            frame = frame._leave_out_observation_spell_match(cc_list=cc_list, max_j=max_j, leave_out_group=leave_out_group, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, is_sorted=is_sorted, copy=False)
-        elif connectedness == 'leave_out_worker':
+            frame = frame._leave_out_observation_spell_match(cc_list=cc_list, max_j=max_j, leave_out_group=leave_out_group, strongly_connected=strongly_connected, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, is_sorted=is_sorted, copy=False)
+        elif connectedness in ['leave_out_worker', 'strongly_leave_out_worker']:
+            # Extract information about strong/weak connectedness
+            strongly_connected = (connectedness.split('_')[0] == 'strongly')
             # Compute all connected components of firms (each entry is a connected component)
-            cc_list = G.components(mode='weak')
+            cc_list = G.components(mode={False: 'weak', True: 'strong'}[strongly_connected])
             # Keep largest leave-one-worker-out set of firms
-            frame = frame._leave_out_worker(cc_list=cc_list, max_j=max_j, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, is_sorted=is_sorted, copy=False)
+            frame = frame._leave_out_worker(cc_list=cc_list, max_j=max_j, strongly_connected=strongly_connected, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, is_sorted=is_sorted, copy=False)
         elif connectedness == 'leave_out_firm':
             # Compute all biconnected components of firms (each entry is a biconnected component)
             bcc_list = sorted(G.biconnected_components(), reverse=True, key=len)
             # Iterate over connected components to find the largest
             largest_bcc = bcc_list[0]
             frame_largest_bcc = frame.keep_ids('j', largest_bcc, is_sorted=is_sorted, copy=False)
             if component_size_variable != 'firms':
@@ -1262,15 +1265,15 @@
             frame = frame_largest_bcc
             try:
                 # Remove comp_size attribute
                 del frame.comp_size
             except AttributeError:
                 pass
         else:
-            raise NotImplementedError(f"Connectedness measure {connectedness!r} is invalid: it must be one of None, 'connected', 'strongly_connected', 'leave_out_observation', 'leave_out_spell', 'leave_out_match', 'leave_out_worker', or 'leave_out_firm'.")
+            raise NotImplementedError(f"Connectedness measure {connectedness!r} is invalid: it must be one of None, 'connected', 'strongly_connected', 'leave_out_observation', 'leave_out_spell', 'leave_out_match', 'leave_out_worker', 'strongly_leave_out_observation', 'strongly_leave_out_spell', 'strongly_leave_out_match', or 'leave_out_firm'.")
 
         if drop_single_stayers:
             # Drop stayers who have <= 1 observation weight
             worker_m = frame.get_worker_m(is_sorted=True)
             if frame._col_included('w'):
                 stayers_weight = frame.loc[~worker_m, ['i', 'w']].groupby('i', sort=False)['w'].transform('sum').to_numpy()
             else:
@@ -1291,15 +1294,15 @@
         return frame
 
     def _construct_graph(self, connectedness='connected', is_sorted=False, copy=True):
         '''
         Construct igraph graph linking firms by movers.
 
         Arguments:
-            connectedness (str): if 'connected', keep observations in the largest connected set of firms; if 'strongly_connected', keep observations in the largest strongly connected set of firms; if 'leave_out_observation', keep observations in the largest leave-one-observation-out connected set; if 'leave_out_spell', keep observations in the largest leave-one-spell-out connected set; if 'leave_out_match', keep observations in the largest leave-one-match-out connected set; if 'leave_out_worker', keep observations in the largest leave-one-worker-out connected set; if 'leave_out_firm', keep observations in the largest leave-one-firm-out connected set; if None, keep all observations
+            connectedness (str): if 'connected', keep observations in the largest connected set of firms; if 'strongly_connected', keep observations in the largest strongly connected set of firms; if 'leave_out_x', keep observations in the largest leave-one-x-out connected set; if 'strongly_leave_out_x', keep observations in the largest strongly connected set that is also leave-one-x-out connected (NOT leave-one-x-out strongly connected); if None, keep all observations
             is_sorted (bool): If False, dataframe will be sorted by i (and t, if included). Sorting may alter original dataframe if copy is set to False. Set is_sorted to True if dataframe is already sorted.
             copy (bool): if False, avoid copy
 
         Returns:
             (igraph Graph): graph
             (int): maximum firm id
         '''
@@ -1307,24 +1310,32 @@
         linkages_fn_dict = {
             'connected': self._construct_firm_linkages,
             'strongly_connected': self._construct_firm_linkages,
             'leave_out_observation': self._construct_firm_worker_linkages,
             'leave_out_spell': self._construct_firm_worker_linkages,
             'leave_out_match': self._construct_firm_worker_linkages,
             'leave_out_worker': self._construct_firm_worker_linkages,
-            'leave_out_firm': self._construct_firm_double_linkages
+            'leave_out_firm': self._construct_firm_double_linkages,
+            'strongly_leave_out_observation': self._construct_firm_linkages,
+            'strongly_leave_out_spell': self._construct_firm_linkages,
+            'strongly_leave_out_match': self._construct_firm_linkages,
+            'strongly_leave_out_worker': self._construct_firm_linkages
         }
         directed_dict = {
             'connected': False,
             'strongly_connected': True,
             'leave_out_observation': False,
             'leave_out_spell': False,
             'leave_out_match': False,
             'leave_out_worker': False,
-            'leave_out_firm': False
+            'leave_out_firm': False,
+            'strongly_leave_out_observation': True,
+            'strongly_leave_out_spell': True,
+            'strongly_leave_out_match': True,
+            'strongly_leave_out_worker': True
 
         }
         linkages, max_j = linkages_fn_dict[connectedness](is_sorted=is_sorted, copy=copy)
         # n_firms = self.loc[(self.loc[:, 'm'] > 0).to_numpy(), :].n_firms()
         return Graph(edges=linkages, directed=directed_dict[connectedness]), max_j # n=n_firms
 
     def sort_cols(self, copy=True):
```

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartitedataframe.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartitedataframe.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartiteeventstudy.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudy.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartiteeventstudybase.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudybase.py`

 * *Files 2% similar despite different names*

```diff
@@ -441,66 +441,68 @@
         Returns:
             data (Pandas DataFrame): data prepared for clustering
             weights (NumPy Array or None): if weighted=True, gives NumPy array of firm weights for clustering; otherwise, is None
             jids (NumPy Array): firm ids of firms in subset of data used to cluster
         '''
         return self.to_long(is_sorted=is_sorted, copy=copy)._prep_cluster(stayers_movers=stayers_movers, t=t, weighted=weighted, is_sorted=True, copy=False)
 
-    def _leave_out_observation_spell_match(self, cc_list, max_j, leave_out_group, component_size_variable='firms', drop_returns_to_stays=False, frame_largest_cc=None, is_sorted=False, copy=True, first_loop=True):
+    def _leave_out_observation_spell_match(self, cc_list, max_j, leave_out_group, strongly_connected=False, component_size_variable='firms', drop_returns_to_stays=False, frame_largest_cc=None, is_sorted=False, copy=True, first_loop=True):
         '''
         Extract largest leave-one-(observation/spell/match)-out connected component.
 
         Arguments:
             cc_list (list of lists): each entry is a connected component
             max_j (int): maximum j in graph
             leave_out_group (str): which type of leave-one-out connected component to compute (options are 'observation', 'spell', or 'match')
+            strongly_connected (bool): if True, compute the largest strongly connected set that is also leave-one-(observation/spell/match)-out connected (NOT leave-one-(observation/spell/match)-out strongly connected)
             component_size_variable (str): how to determine largest leave-one-(observation/spell/match)-out connected component. Options are 'len'/'length' (length of frames), 'firms' (number of unique firms), 'workers' (number of unique workers), 'stayers' (number of unique stayers), 'movers' (number of unique movers), 'firms_plus_workers' (number of unique firms + number of unique workers), 'firms_plus_stayers' (number of unique firms + number of unique stayers), 'firms_plus_movers' (number of unique firms + number of unique movers), 'len_stayers'/'length_stayers' (number of stayer observations), 'len_movers'/'length_movers' (number of mover observations), 'stays' (number of stay observations), and 'moves' (number of move observations).
             drop_returns_to_stays (bool): if True, when recollapsing collapsed data, drop observations that need to be recollapsed instead of collapsing (this is for computational efficiency when re-collapsing data for leave-one-(observation/spell/match)-out connected components, where intermediate observations can be dropped, causing a worker who returns to a firm to become a stayer)
             frame_largest_cc (BipartiteLongBase): dataframe of baseline largest leave-one-(observation/spell/match)-out connected component
             is_sorted (bool): if False, dataframe will be sorted by i (and t, if included). Returned dataframe will be sorted. Sorting may alter original dataframe if copy is set to False. Set is_sorted to True if dataframe is already sorted.
             copy (bool): if False, avoid copy
             first_loop (bool): if True, this is the first loop of the method
 
         Returns:
             (BipartiteEventStudyBase): dataframe of largest leave-one-(observation/spell/match)-out connected component
         '''
         # Keep track of columns that aren't supposed to convert to long, but we allow to convert because this is during data cleaning
         no_split_cols = [col for col, long_es_split in self.col_long_es_dict.items() if long_es_split is None]
 
         # Compute leave-one-(observation/spell/match)-out connected components
-        frame = self.to_long(drop_no_split_columns=False, is_sorted=is_sorted, copy=copy)._leave_out_observation_spell_match(cc_list=cc_list, max_j=max_j, leave_out_group=leave_out_group, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=first_loop).to_eventstudy(is_sorted=True, copy=False)
+        frame = self.to_long(drop_no_split_columns=False, is_sorted=is_sorted, copy=copy)._leave_out_observation_spell_match(cc_list=cc_list, max_j=max_j, leave_out_group=leave_out_group, strongly_connected=strongly_connected, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=first_loop).to_eventstudy(is_sorted=True, copy=False)
 
         # Update col_long_es_dict for columns that aren't supposed to convert to long
         for col in no_split_cols:
             frame.col_long_es_dict[col] = None
 
         return frame
 
-    def _leave_out_worker(self, cc_list, max_j, component_size_variable='firms', drop_returns_to_stays=False, frame_largest_cc=None, is_sorted=False, copy=True, first_loop=True):
+    def _leave_out_worker(self, cc_list, max_j, strongly_connected=False, component_size_variable='firms', drop_returns_to_stays=False, frame_largest_cc=None, is_sorted=False, copy=True, first_loop=True):
         '''
         Extract largest leave-one-worker-out connected component.
 
         Arguments:
             cc_list (list of lists): each entry is a connected component
             max_j (int): maximum j in graph
+            strongly_connected (bool): if True, compute the largest strongly connected set that is also leave-one-worker-out connected (NOT leave-one-worker-out strongly connected)
             component_size_variable (str): how to determine largest leave-one-worker-out connected component. Options are 'len'/'length' (length of frame), 'firms' (number of unique firms), 'workers' (number of unique workers), 'stayers' (number of unique stayers), and 'movers' (number of unique movers)
             drop_returns_to_stays (bool): if True, when recollapsing collapsed data, drop observations that need to be recollapsed instead of collapsing (this is for computational efficiency when re-collapsing data for leave-one-out connected components, where intermediate observations can be dropped, causing a worker who returns to a firm to become a stayer)
             frame_largest_cc (BipartiteLongBase): dataframe of baseline largest leave-one-worker-out connected component
             is_sorted (bool): if False, dataframe will be sorted by i (and t, if included). Returned dataframe will be sorted. Sorting may alter original dataframe if copy is set to False. Set is_sorted to True if dataframe is already sorted.
             copy (bool): if False, avoid copy
             first_loop (bool): if True, this is the first loop of the method
 
         Returns:
             (BipartiteEventStudyBase): dataframe of largest leave-one-worker-out connected component
         '''
         # Keep track of columns that aren't supposed to convert to long, but we allow to convert because this is during data cleaning
         no_split_cols = [col for col, long_es_split in self.col_long_es_dict.items() if long_es_split is None]
 
         # Compute leave-one-worker-out connected components
-        frame = self.to_long(drop_no_split_columns=False, is_sorted=is_sorted, copy=copy)._leave_out_worker(cc_list=cc_list, max_j=max_j, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=first_loop).to_eventstudy(is_sorted=True, copy=False)
+        frame = self.to_long(drop_no_split_columns=False, is_sorted=is_sorted, copy=copy)._leave_out_worker(cc_list=cc_list, max_j=max_j, strongly_connected=strongly_connected, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=first_loop).to_eventstudy(is_sorted=True, copy=False)
 
         # Update col_long_es_dict for columns that aren't supposed to convert to long
         for col in no_split_cols:
             frame.col_long_es_dict[col] = None
 
         return frame
```

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartiteeventstudycollapsed.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartiteeventstudycollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartiteextendedeventstudy.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudy.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartiteextendedeventstudybase.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudybase.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartiteextendedeventstudycollapsed.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartiteextendedeventstudycollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartitelong.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartitelong.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,30 +88,36 @@
             params = params.copy()
 
         self.log('beginning BipartiteLong data cleaning', level='info')
 
         connectedness = params['connectedness']
         collapse_connectedness = params['collapse_at_connectedness_measure']
         # If will have to collapse the data after cleaning
-        collapse = (collapse_connectedness and connectedness in ['leave_out_spell', 'leave_out_match'])
+        collapse = (collapse_connectedness and connectedness in ['leave_out_spell', 'leave_out_match', 'strongly_leave_out_spell', 'strongly_leave_out_match'])
         if collapse:
             params['connectedness'] = None
 
         ## Initial cleaning ##
         frame = super().clean(params)
 
         if collapse:
             ## Collapse then compute largest connected set ##
             # Update parameters
             level_dict = {
                 'leave_out_spell': 'spell',
-                'leave_out_match': 'match'
+                'leave_out_match': 'match',
+                'strongly_leave_out_spell': 'spell',
+                'strongly_leave_out_match': 'match'
             }
             # NOTE: leave-out-observation is equivalent to leave-out-(spell/match) if the data is collapsed at the (spell/match) level, but the code is faster
-            params['connectedness'] = 'leave_out_observation'
+            strongly_connected = (connectedness.split('_')[0] == 'strongly')
+            if strongly_connected:
+                params['connectedness'] = 'strongly_leave_out_observation'
+            else:
+                params['connectedness'] = 'leave_out_observation'
             params['drop_returns'] = False
             params['is_sorted'] = True
             params['copy'] = False
             params['force'] = False
 
             # Collapse
             frame = frame.collapse(level=level_dict[connectedness], is_sorted=True, copy=False)
```

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartitelongbase.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartitelongbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -683,35 +683,43 @@
         bridges_workers = set([bridge[0] - (max_j + 1) for bridge in bridges])
         bridges_firms = set([bridge[1] for bridge in bridges])
 
         # Return articulation matches
         # return self.loc[pd.Series(map(tuple, self.loc[:, ['i', 'j']].to_numpy())).reindex_like(self, copy=False).isin(bridges), :].index.to_numpy() # FIXME this doesn't work
         return self.loc[self.loc[:, 'i'].isin(bridges_workers) & self.loc[:, 'j'].isin(bridges_firms), :].index.to_numpy()
 
-    def _leave_out_observation_spell_match(self, cc_list, max_j, leave_out_group, component_size_variable='firms', drop_returns_to_stays=False, frame_largest_cc=None, is_sorted=False, copy=True, first_loop=True):
+    def _leave_out_observation_spell_match(self, cc_list, max_j, leave_out_group, strongly_connected=False, component_size_variable='firms', drop_returns_to_stays=False, frame_largest_cc=None, is_sorted=False, copy=True, first_loop=True):
         '''
         Extract largest leave-one-(observation/spell/match)-out connected component.
 
         Arguments:
             cc_list (list of lists): each entry is a connected component
             max_j (int): maximum j in graph
             leave_out_group (str): which type of leave-one-out connected component to compute (options are 'observation', 'spell', or 'match')
+            strongly_connected (bool): if True, compute the largest strongly connected set that is also leave-one-(observation/spell/match)-out connected (NOT leave-one-(observation/spell/match)-out strongly connected)
             component_size_variable (str): how to determine largest leave-one-(observation/spell/match)-out connected component. Options are 'len'/'length' (length of frames), 'firms' (number of unique firms), 'workers' (number of unique workers), 'stayers' (number of unique stayers), 'movers' (number of unique movers), 'firms_plus_workers' (number of unique firms + number of unique workers), 'firms_plus_stayers' (number of unique firms + number of unique stayers), 'firms_plus_movers' (number of unique firms + number of unique movers), 'len_stayers'/'length_stayers' (number of stayer observations), 'len_movers'/'length_movers' (number of mover observations), 'stays' (number of stay observations), and 'moves' (number of move observations).
             drop_returns_to_stays (bool): if True, when recollapsing collapsed data, drop observations that need to be recollapsed instead of collapsing (this is for computational efficiency when re-collapsing data for leave-one-(observation/spell/match)-out connected components, where intermediate observations can be dropped, causing a worker who returns to a firm to become a stayer)
             frame_largest_cc (BipartiteLongBase): dataframe of baseline largest leave-one-(observation/spell/match)-out connected component
             is_sorted (bool): if False, dataframe will be sorted by i (and t, if included). Returned dataframe will be sorted. Sorting may alter original dataframe if copy is set to False. Set is_sorted to True if dataframe is already sorted.
             copy (bool): if False, avoid copy
             first_loop (bool): if True, this is the first loop of the method
 
         Returns:
             (BipartiteLongBase): dataframe of largest leave-one-(observation/spell/match)-out connected component
         '''
         # Sort and copy
         frame_init = self.sort_rows(is_sorted=is_sorted, copy=copy)
 
+        # Name of connectedness
+        connectedness_name_short = f'leave_out_{leave_out_group}'
+        if strongly_connected:
+            connectedness_name_full = f'strongly_{connectedness_name_short}'
+        else:
+            connectedness_name_full = connectedness_name_short
+
         for cc in sorted(cc_list, reverse=True, key=len):
             cc = np.array(cc)
             cc_j = cc[cc <= max_j]
             if frame_largest_cc is not None:
                 # Can check if frame_cc is already smaller than frame_largest_cc before any computations
                 skip = False
                 if component_size_variable == 'firms':
@@ -738,25 +746,35 @@
                 # If frame_cc is already smaller than frame_largest_cc
                 skip = bpd.util.compare_frames(frame_largest_cc, frame_cc, size_variable=component_size_variable, operator='geq', save_to_frame1=True, is_sorted=True)
 
                 if skip:
                     continue
 
             # Remove firms with only 1 mover observation (can have 1 mover with multiple observations)
+            if strongly_connected:
+                prev_len = len(frame_cc)
             frame_cc = frame_cc.min_moves_frame(2, drop_returns_to_stays, is_sorted=True, copy=False)
+            if strongly_connected and (len(frame_cc) != prev_len):
+                # Dropping firms with 1 mover observation can change the strongly connected components, so recompute strongly connected components
+                G2, max_j2 = frame_cc._construct_graph(connectedness_name_full, is_sorted=True, copy=False)
+                cc_list_2 = G2.components(mode='strong')
+                del G2
+                if len(cc_list_2) > 1:
+                    # Recursion step (only necessary if dropping firms with 1 mover observations disconnects the set of firms)
+                    frame_cc = frame_cc._leave_out_observation_spell_match(cc_list=cc_list_2, max_j=max_j2, leave_out_group=leave_out_group, strongly_connected=strongly_connected, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=False)
 
             if frame_largest_cc is not None:
                 # If frame_cc is already smaller than frame_largest_cc
                 skip = bpd.util.compare_frames(frame_largest_cc, frame_cc, size_variable=component_size_variable, operator='geq', save_to_frame1=True, is_sorted=True)
 
                 if skip:
                     continue
 
             # Construct graph
-            G2, max_j2 = frame_cc._construct_graph(f'leave_out_{leave_out_group}', is_sorted=True, copy=False)
+            G2, max_j2 = frame_cc._construct_graph(connectedness_name_short, is_sorted=True, copy=False)
 
             # Extract articulation rows
             articulation_fn_dict = {
                 'observation': frame_cc._get_articulation_observations,
                 'spell': frame_cc._get_articulation_spells,
                 'match': frame_cc._get_articulation_matches
             }
@@ -766,20 +784,20 @@
                 'match': {'G': G2, 'max_j': max_j2}
             }
             articulation_rows = articulation_fn_dict[leave_out_group](**articulation_params_dict[leave_out_group])
             del articulation_fn_dict, articulation_params_dict
 
             if len(articulation_rows) > 0:
                 # If new frame is not leave-one-(observation/spell/match)-out connected, recompute connected components after dropping articulation rows (but note that articulation rows should be kept in the final dataframe) (NOTE: this does not require a copy)
-                G2, max_j3 = frame_cc.drop_rows(articulation_rows, drop_returns_to_stays, is_sorted=True, reset_index=False, copy=False)._construct_graph(f'leave_out_{leave_out_group}', is_sorted=True, copy=False)
-                cc_list_2 = G2.components(mode='weak')
+                G2, max_j3 = frame_cc.drop_rows(articulation_rows, drop_returns_to_stays, is_sorted=True, reset_index=False, copy=False)._construct_graph(connectedness_name_full, is_sorted=True, copy=False)
+                cc_list_2 = G2.components(mode={False: 'weak', True: 'strong'}[strongly_connected])
                 del G2, articulation_rows
                 if len(cc_list_2) > 1:
                     # Recursion step (only necessary if dropping articulation workers disconnects the set of firms)
-                    frame_cc = frame_cc._leave_out_observation_spell_match(cc_list=cc_list_2, max_j=max_j3, leave_out_group=leave_out_group, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=False)
+                    frame_cc = frame_cc._leave_out_observation_spell_match(cc_list=cc_list_2, max_j=max_j3, leave_out_group=leave_out_group, strongly_connected=strongly_connected, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=False)
                 del cc_list_2
             else:
                 del G2, articulation_rows
 
             if frame_largest_cc is None:
                 # If in the first round
                 replace = True
@@ -798,21 +816,22 @@
                 del frame_largest_cc.comp_size
             except AttributeError:
                 pass
 
         # Return largest leave-one-(observation/spell/match)-out component
         return frame_largest_cc
 
-    def _leave_out_worker(self, cc_list, max_j, component_size_variable='firms', drop_returns_to_stays=False, frame_largest_cc=None, is_sorted=False, copy=True, first_loop=True):
+    def _leave_out_worker(self, cc_list, max_j, strongly_connected=False, component_size_variable='firms', drop_returns_to_stays=False, frame_largest_cc=None, is_sorted=False, copy=True, first_loop=True):
         '''
         Extract largest leave-one-worker-out connected component.
 
         Arguments:
             cc_list (list of lists): each entry is a connected component
             max_j (int): maximum j in graph
+            strongly_connected (bool): if True, compute the largest strongly connected set that is also leave-one-worker-out connected (NOT leave-one-worker-out strongly connected)
             component_size_variable (str): how to determine largest leave-one-worker-out connected component. Options are 'len'/'length' (length of frames), 'firms' (number of unique firms), 'workers' (number of unique workers), 'stayers' (number of unique stayers), 'movers' (number of unique movers), 'firms_plus_workers' (number of unique firms + number of unique workers), 'firms_plus_stayers' (number of unique firms + number of unique stayers), 'firms_plus_movers' (number of unique firms + number of unique movers), 'len_stayers'/'length_stayers' (number of stayer observations), 'len_movers'/'length_movers' (number of mover observations), 'stays' (number of stay observations), and 'moves' (number of move observations).
             drop_returns_to_stays (bool): if True, when recollapsing collapsed data, drop observations that need to be recollapsed instead of collapsing (this is for computational efficiency when re-collapsing data for leave-one-out connected components, where intermediate observations can be dropped, causing a worker who returns to a firm to become a stayer)
             frame_largest_cc (BipartiteLongBase): dataframe of baseline largest leave-one-worker-out connected component
             is_sorted (bool): if False, dataframe will be sorted by i (and t, if included). Returned dataframe will be sorted. Sorting may alter original dataframe if copy is set to False. Set is_sorted to True if dataframe is already sorted.
             copy (bool): if False, avoid copy
             first_loop (bool): if True, this is the first loop of the method
 
@@ -852,15 +871,25 @@
                 # If frame_cc is already smaller than frame_largest_cc
                 skip = bpd.util.compare_frames(frame_largest_cc, frame_cc, size_variable=component_size_variable, operator='geq', save_to_frame1=True, is_sorted=True)
 
                 if skip:
                     continue
 
             # Remove firms with only 1 mover observation (can have 1 mover with multiple observations)
+            if strongly_connected:
+                prev_len = len(frame_cc)
             frame_cc = frame_cc.min_moves_frame(2, drop_returns_to_stays, is_sorted=True, copy=False)
+            if strongly_connected and (len(frame_cc) != prev_len):
+                # Dropping firms with 1 mover observation can change the strongly connected components, so recompute strongly connected components
+                G2, max_j2 = frame_cc._construct_graph('strongly_leave_out_worker', is_sorted=True, copy=False)
+                cc_list_2 = G2.components(mode='strong')
+                del G2
+                if len(cc_list_2) > 1:
+                    # Recursion step (only necessary if dropping firms with 1 mover observations disconnects the set of firms)
+                    frame_cc = frame_cc._leave_out_worker(cc_list=cc_list_2, max_j=max_j2, strongly_connected=strongly_connected, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=False)
 
             if frame_largest_cc is not None:
                 # If frame_cc is already smaller than frame_largest_cc
                 skip = bpd.util.compare_frames(frame_largest_cc, frame_cc, size_variable=component_size_variable, operator='geq', save_to_frame1=True, is_sorted=True)
 
                 if skip:
                     continue
@@ -872,20 +901,20 @@
             articulation_ids = np.array(G2.articulation_points())
             articulation_workers = articulation_ids[articulation_ids > max_j2]
             articulation_workers -= (max_j2 + 1)
             del articulation_ids
 
             if len(articulation_workers) > 0:
                 # If new frame is not leave-one-worker-out connected, recompute connected components after dropping articulation workers (but note that articulation workers should be kept in the final dataframe) (NOTE: this does not require a copy)
-                G2, max_j3 = frame_cc.drop_ids('i', articulation_workers, drop_returns_to_stays, is_sorted=True, reset_index=False, copy=False)._construct_graph('leave_out_worker', is_sorted=True, copy=False)
-                cc_list_2 = G2.components(mode='weak')
+                G2, max_j3 = frame_cc.drop_ids('i', articulation_workers, drop_returns_to_stays, is_sorted=True, reset_index=False, copy=False)._construct_graph({False: 'leave_out_worker', True: 'strongly_leave_out_worker'}[strongly_connected], is_sorted=True, copy=False)
+                cc_list_2 = G2.components(mode={False: 'weak', True: 'strong'}[strongly_connected])
                 del G2, articulation_workers
                 if len(cc_list_2) > 1:
                     # Recursion step (only necessary if dropping articulation workers disconnects the set of firms)
-                    frame_cc = frame_cc._leave_out_worker(cc_list=cc_list_2, max_j=max_j3, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=False)
+                    frame_cc = frame_cc._leave_out_worker(cc_list=cc_list_2, max_j=max_j3, strongly_connected=strongly_connected, component_size_variable=component_size_variable, drop_returns_to_stays=drop_returns_to_stays, frame_largest_cc=frame_largest_cc, is_sorted=True, copy=False, first_loop=False)
                 del cc_list_2
             else:
                 del G2, articulation_workers
 
             if frame_largest_cc is None:
                 # If in the first round
                 replace = True
```

### Comparing `bipartitepandas-1.1.4/bipartitepandas/bipartitelongcollapsed.py` & `bipartitepandas-1.1.5/bipartitepandas/bipartitelongcollapsed.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/grouping/grouping.py` & `bipartitepandas-1.1.5/bipartitepandas/grouping/grouping.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/measures/measures.py` & `bipartitepandas-1.1.5/bipartitepandas/measures/measures.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/simbipartite.py` & `bipartitepandas-1.1.5/bipartitepandas/simbipartite.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas/util.py` & `bipartitepandas-1.1.5/bipartitepandas/util.py`

 * *Files identical despite different names*

### Comparing `bipartitepandas-1.1.4/bipartitepandas.egg-info/PKG-INFO` & `bipartitepandas-1.1.5/bipartitepandas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bipartitepandas
-Version: 1.1.4
+Version: 1.1.5
 Summary: Python tools for bipartite labor data
 Home-page: https://github.com/tlamadon/bipartitepandas/
 Author: Thibaut Lamadon
 Author-email: thibaut.lamadon@gmail.com
 Project-URL: Documentation, https://tlamadon.github.io/bipartitepandas/
 Project-URL: GitHub, https://github.com/tlamadon/bipartitepandas/
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bipartitepandas-1.1.4/setup.cfg` & `bipartitepandas-1.1.5/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = bipartitepandas
-version = 1.1.4
+version = 1.1.5
 author = Thibaut Lamadon
 author_email = thibaut.lamadon@gmail.com
 description = Python tools for bipartite labor data
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/tlamadon/bipartitepandas/
 project_urls =
```

