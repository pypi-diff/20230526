# Comparing `tmp/pref_voting-0.3.1.tar.gz` & `tmp/pref_voting-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.3.1.tar", max compression
+gzip compressed data, was "pref_voting-0.3.2.tar", max compression
```

## Comparing `pref_voting-0.3.1.tar` & `pref_voting-0.3.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.3.1/LICENSE
--rw-r--r--   0        0        0     3198 2023-05-26 14:32:56.499334 pref_voting-0.3.1/README.md
--rw-r--r--   0        0        0       22 2023-05-26 16:46:47.206085 pref_voting-0.3.1/pref_voting/__init__.py
--rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.3.1/pref_voting/analysis.py
--rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.3.1/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.3.1/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.3.1/pref_voting/axioms.py
--rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.3.1/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.3.1/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.3.1/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.3.1/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0     4664 2023-05-26 14:20:44.876014 pref_voting-0.3.1/pref_voting/generate_utility_profiles.py
--rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.3.1/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.3.1/pref_voting/helper.py
--rw-r--r--   0        0        0    73193 2023-05-25 12:07:00.027553 pref_voting-0.3.1/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.3.1/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    59902 2023-05-26 16:43:02.649354 pref_voting-0.3.1/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.3.1/pref_voting/other_methods.py
--rw-r--r--   0        0        0    27160 2023-05-24 21:44:14.545976 pref_voting-0.3.1/pref_voting/profiles.py
--rw-r--r--   0        0        0    23817 2023-05-26 10:29:19.112624 pref_voting-0.3.1/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.3.1/pref_voting/rankings.py
--rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.3.1/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.3.1/pref_voting/utility_methods.py
--rw-r--r--   0        0        0    13967 2023-05-26 12:07:03.892154 pref_voting-0.3.1/pref_voting/utility_profiles.py
--rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.3.1/pref_voting/variable_voter_axioms.py
--rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.3.1/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.3.1/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    50074 2023-05-25 15:22:53.891568 pref_voting-0.3.1/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      689 2023-05-26 16:46:47.204961 pref_voting-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4151 1970-01-01 00:00:00.000000 pref_voting-0.3.1/setup.py
--rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 pref_voting-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3200 2023-05-26 16:48:07.750821 pref_voting-0.3.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-26 17:48:30.275420 pref_voting-0.3.2/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.3.2/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.3.2/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.3.2/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.3.2/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.3.2/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.3.2/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.3.2/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.3.2/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     4664 2023-05-26 14:20:44.876014 pref_voting-0.3.2/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.3.2/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.3.2/pref_voting/helper.py
+-rw-r--r--   0        0        0    73193 2023-05-25 12:07:00.027553 pref_voting-0.3.2/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.3.2/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    59218 2023-05-26 17:44:51.542166 pref_voting-0.3.2/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.3.2/pref_voting/other_methods.py
+-rw-r--r--   0        0        0    28609 2023-05-26 17:29:58.194223 pref_voting-0.3.2/pref_voting/profiles.py
+-rw-r--r--   0        0        0    25273 2023-05-26 17:38:33.040884 pref_voting-0.3.2/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.3.2/pref_voting/rankings.py
+-rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.3.2/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.3.2/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    13967 2023-05-26 12:07:03.892154 pref_voting-0.3.2/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.3.2/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.3.2/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.3.2/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    51549 2023-05-26 17:29:52.723637 pref_voting-0.3.2/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      689 2023-05-26 17:48:30.274441 pref_voting-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4153 1970-01-01 00:00:00.000000 pref_voting-0.3.2/setup.py
+-rw-r--r--   0        0        0     4268 1970-01-01 00:00:00.000000 pref_voting-0.3.2/PKG-INFO
```

### Comparing `pref_voting-0.3.1/LICENSE` & `pref_voting-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/README.md` & `pref_voting-0.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 - v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 - v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
 - v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
-- v0.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
+- v0.3.1 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.3.1/pref_voting/analysis.py` & `pref_voting-0.3.2/pref_voting/analysis.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/axiom.py` & `pref_voting-0.3.2/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/c1_methods.py` & `pref_voting-0.3.2/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/combined_methods.py` & `pref_voting-0.3.2/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/dominance_axioms.py` & `pref_voting-0.3.2/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/generate_profiles.py` & `pref_voting-0.3.2/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/generate_utility_profiles.py` & `pref_voting-0.3.2/pref_voting/generate_utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.3.2/pref_voting/generate_weighted_majority_graphs.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/helper.py` & `pref_voting-0.3.2/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/iterative_methods.py` & `pref_voting-0.3.2/pref_voting/iterative_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/maj_graph_ex1.png` & `pref_voting-0.3.2/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/margin_based_methods.py` & `pref_voting-0.3.2/pref_voting/margin_based_methods.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,27 +383,17 @@
         from pref_voting.margin_based_methods import split_cycle
         
         mg = MarginGraph([0, 1, 2, 3], [(0, 2, 3), (1, 0, 5), (2, 1, 5), (2, 3, 1), (3, 0, 3), (3, 1, 1)])
         
         split_cycle.display(mg)
     """
     
-    candidates = edata.candidates if curr_cands is None else curr_cands  
+    strength_matrix, cand_to_cindex = edata.strength_matrix(curr_cands = curr_cands, strength_function=strength_function)
 
-    if curr_cands is not None: 
-        cindices = [cidx for cidx, c in enumerate(curr_cands)]
-        cindex_to_cand = lambda cidx: curr_cands[cidx]
-        cand_to_cindex = lambda c: cindices[curr_cands.index(c)]
-        strength_function = edata.margin if strength_function is None else strength_function
-        strength_matrix = np.array([[strength_function(cindex_to_cand(a_idx), cindex_to_cand(b_idx)) for b_idx in cindices] for a_idx in cindices])
-    else:  
-        cindices = edata.cindices
-        cindex_to_cand = edata.cindex_to_cand
-        cand_to_cindex = edata.cand_to_cindex
-        strength_matrix = np.array(edata.margin_matrix) if strength_function is None else np.array([[strength_function(cindex_to_cand(a_idx), cindex_to_cand(b_idx)) for b_idx in cindices] for a_idx in cindices])
+    candidates = edata.candidates if curr_cands is None else curr_cands  
 
     strength_function = edata.margin if strength_function is None else strength_function 
 
     potential_winners = set(candidates)
 
     for a in candidates:
         for b in candidates:
```

### Comparing `pref_voting-0.3.1/pref_voting/other_methods.py` & `pref_voting-0.3.2/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/profiles.py` & `pref_voting-0.3.2/pref_voting/profiles.py`

 * *Files 6% similar despite different names*

```diff
@@ -265,14 +265,33 @@
 
     def is_tied(self, c1, c2):
         """Returns True if ``c1`` tied with ``c2``.  That is, the same number of voters rank ``c1`` over ``c2`` as ``c2`` over ``c1``. 
         """ 
 
         return _margin(self._tally, c1, c2) == 0
 
+    def strength_matrix(self, curr_cands = None, strength_function = None): 
+        """
+        Return the strength matrix of the profile.  The strength matrix is a matrix where the entry in row :math:`i` and column :math:`j` is the number of voters that rank the candidate with index :math:`i` over the candidate with index :math:`j`.  If ``curr_cands`` is provided, then the strength matrix is restricted to the candidates in ``curr_cands``.  If ``strength_function`` is provided, then the strength matrix is computed using the strength function."""
+
+        if curr_cands is not None: 
+            cindices = [cidx for cidx, _ in enumerate(curr_cands)]
+            cindex_to_cand = lambda cidx: curr_cands[cidx]
+            cand_to_cindex = lambda c: cindices[curr_cands.index(c)]
+            strength_function = self.margin if strength_function is None else strength_function
+            strength_matrix = np.array([[strength_function(cindex_to_cand(a_idx), cindex_to_cand(b_idx)) for b_idx in cindices] for a_idx in cindices])
+        else:  
+            cindices = self.cindices
+            cindex_to_cand = self.cindex_to_cand
+            cand_to_cindex = self.cand_to_cindex
+            strength_matrix = np.array(self.margin_matrix) if strength_function is None else np.array([[strength_function(cindex_to_cand(a_idx), cindex_to_cand(b_idx)) for b_idx in cindices] for a_idx in cindices])
+
+        return strength_matrix, cand_to_cindex
+
+
     def cycles(self): 
         """Return a list of the cycles in the profile."""
 
         return self.margin_graph().cycles()
 
     def num_rank(self, c, level): 
         """The number of voters that rank candidate ``c`` at position ``level``
```

### Comparing `pref_voting-0.3.1/pref_voting/profiles_with_ties.py` & `pref_voting-0.3.2/pref_voting/profiles_with_ties.py`

 * *Files 6% similar despite different names*

```diff
@@ -198,14 +198,32 @@
             return 1
 
     def majority_prefers(self, c1, c2):
         """Returns True if ``c1`` is majority preferred to ``c2``."""
 
         return self.margin(c1, c2) > 0
 
+    def strength_matrix(self, curr_cands = None, strength_function = None): 
+        """
+        Return the strength matrix of the profile.  The strength matrix is a matrix where the entry in row :math:`i` and column :math:`j` is the number of voters that rank the candidate with index :math:`i` over the candidate with index :math:`j`.  If ``curr_cands`` is provided, then the strength matrix is restricted to the candidates in ``curr_cands``.  If ``strength_function`` is provided, then the strength matrix is computed using the strength function."""
+        
+        if curr_cands is not None: 
+            cindices = [cidx for cidx, _ in enumerate(curr_cands)]
+            cindex_to_cand = lambda cidx: curr_cands[cidx]
+            cand_to_cindex = lambda c: cindices[curr_cands.index(c)]
+            strength_function = self.margin if strength_function is None else strength_function
+            strength_matrix = np.array([[strength_function(cindex_to_cand(a_idx), cindex_to_cand(b_idx)) for b_idx in cindices] for a_idx in cindices])
+        else:  
+            cindices = self.cindices
+            cindex_to_cand = self.cindex_to_cand
+            cand_to_cindex = self.cand_to_cindex
+            strength_matrix = np.array(self.margin_matrix) if strength_function is None else np.array([[strength_function(cindex_to_cand(a_idx), cindex_to_cand(b_idx)) for b_idx in cindices] for a_idx in cindices])
+
+        return strength_matrix, cand_to_cindex
+
     def condorcet_winner(self, curr_cands=None):
         """Returns the Condorcet winner in the profile restricted to ``curr_cands`` if one exists, otherwise return None.
 
         The **Condorcet winner** is the candidate that is majority preferred to every other candidate.
         """
         curr_cands = curr_cands if curr_cands is not None else self.candidates
```

### Comparing `pref_voting-0.3.1/pref_voting/rankings.py` & `pref_voting-0.3.2/pref_voting/rankings.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/scoring_methods.py` & `pref_voting-0.3.2/pref_voting/scoring_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/utility_methods.py` & `pref_voting-0.3.2/pref_voting/utility_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/utility_profiles.py` & `pref_voting-0.3.2/pref_voting/utility_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/variable_voter_axioms.py` & `pref_voting-0.3.2/pref_voting/variable_voter_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/voting_method.py` & `pref_voting-0.3.2/pref_voting/voting_method.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.3.1/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.3.2/pref_voting/weighted_majority_graphs.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 import networkx as nx
 from tabulate import tabulate
 import matplotlib.pyplot as plt
 import string
 from itertools import combinations
+import numpy as np
 
 class MajorityGraph(object):
     """A majority graph is an asymmetric directed graph.  The nodes are the candidates and an edge from candidate :math:`c` to :math:`d` means that :math:`c` is majority preferred to :math:`d`.
 
     :param candidates: List of the candidates.  To be used as nodes in the majority graph.
     :type candidates: list[int] or  list[str]
     :param edges: List of the pairs of candidates describing the edges in the majority graph.   If :math:`(c,d)` is in the list of edges, then there is an edge from :math:`c` to :math:`d`.
@@ -472,14 +473,32 @@
             self.margin_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)] = margin
             self.margin_matrix[self.cand_to_cindex(c2)][self.cand_to_cindex(c1)] = -1 * margin
 
     def margin(self, c1, c2):
         """Returns the margin of ``c1`` over ``c2``."""
         return self.margin_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)]
 
+    def strength_matrix(self, curr_cands = None, strength_function = None): 
+        """
+        Return the strength matrix of the profile.  The strength matrix is a matrix where the entry in row :math:`i` and column :math:`j` is the number of voters that rank the candidate with index :math:`i` over the candidate with index :math:`j`.  If ``curr_cands`` is provided, then the strength matrix is restricted to the candidates in ``curr_cands``.  If ``strength_function`` is provided, then the strength matrix is computed using the strength function."""
+        
+        if curr_cands is not None: 
+            cindices = [cidx for cidx, _ in enumerate(curr_cands)]
+            cindex_to_cand = lambda cidx: curr_cands[cidx]
+            cand_to_cindex = lambda c: cindices[curr_cands.index(c)]
+            strength_function = self.margin if strength_function is None else strength_function
+            strength_matrix = np.array([[strength_function(cindex_to_cand(a_idx), cindex_to_cand(b_idx)) for b_idx in cindices] for a_idx in cindices])
+        else:  
+            cindices = self.cindices
+            cindex_to_cand = self.cindex_to_cand
+            cand_to_cindex = self.cand_to_cindex
+            strength_matrix = np.array(self.margin_matrix) if strength_function is None else np.array([[strength_function(cindex_to_cand(a_idx), cindex_to_cand(b_idx)) for b_idx in cindices] for a_idx in cindices])
+
+        return strength_matrix, cand_to_cindex
+
     @property
     def edges(self):
         """Returns a list of the weighted edges in the margin graph."""
 
         return [(c1, c2, self.margin(c1, c2)) for c1, c2 in self.mg.edges]
 
     def remove_candidates(self, cands_to_ignore):
```

### Comparing `pref_voting-0.3.1/pyproject.toml` & `pref_voting-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.3.1"
+version = "0.3.2"
 description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
```

### Comparing `pref_voting-0.3.1/setup.py` & `pref_voting-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.3.1',
+    'version': '0.3.2',
     'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3.1 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.3.1/PKG-INFO` & `pref_voting-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.3.1
+Version: 0.3.2
 Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -84,15 +84,15 @@
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
 - v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
 - v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
 - v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
-- v0.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
+- v0.3.1 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

