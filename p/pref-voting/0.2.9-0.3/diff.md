# Comparing `tmp/pref_voting-0.2.9.tar.gz` & `tmp/pref_voting-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pref_voting-0.2.9.tar", max compression
+gzip compressed data, was "pref_voting-0.3.tar", max compression
```

## Comparing `pref_voting-0.2.9.tar` & `pref_voting-0.3.tar`

### file list

```diff
@@ -1,27 +1,31 @@
--rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.2.9/LICENSE
--rw-r--r--   0        0        0     2843 2023-05-16 22:54:30.865590 pref_voting-0.2.9/README.md
--rw-r--r--   0        0        0       22 2023-05-16 22:54:28.075986 pref_voting-0.2.9/pref_voting/__init__.py
--rw-r--r--   0        0        0     9631 2023-05-10 11:35:26.690819 pref_voting-0.2.9/pref_voting/analysis.py
--rw-r--r--   0        0        0     1226 2023-05-10 11:42:24.592401 pref_voting-0.2.9/pref_voting/axiom.py
--rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.2.9/pref_voting/axiom_helpers.py
--rw-r--r--   0        0        0       43 2023-04-27 22:57:52.337540 pref_voting-0.2.9/pref_voting/axioms.py
--rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.2.9/pref_voting/c1_methods.py
--rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.2.9/pref_voting/combined_methods.py
--rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.2.9/pref_voting/dominance_axioms.py
--rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.2.9/pref_voting/generate_profiles.py
--rw-r--r--   0        0        0    10484 2023-01-11 11:10:14.000000 pref_voting-0.2.9/pref_voting/generate_weighted_majority_graphs.py
--rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.2.9/pref_voting/helper.py
--rw-r--r--   0        0        0    73229 2023-05-10 11:16:21.455329 pref_voting-0.2.9/pref_voting/iterative_methods.py
--rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.2.9/pref_voting/maj_graph_ex1.png
--rw-r--r--   0        0        0    59105 2023-05-16 22:53:18.787316 pref_voting-0.2.9/pref_voting/margin_based_methods.py
--rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.2.9/pref_voting/other_methods.py
--rw-r--r--   0        0        0     9526 2023-05-10 11:24:57.793416 pref_voting-0.2.9/pref_voting/pr_voting_methods.py
--rw-r--r--   0        0        0    26954 2023-05-15 22:14:59.029784 pref_voting-0.2.9/pref_voting/profiles.py
--rw-r--r--   0        0        0    34203 2023-04-27 22:31:21.483788 pref_voting-0.2.9/pref_voting/profiles_with_ties.py
--rw-r--r--   0        0        0    11064 2023-05-05 16:30:25.075183 pref_voting-0.2.9/pref_voting/scoring_methods.py
--rw-r--r--   0        0        0     5381 2023-02-15 15:31:23.315651 pref_voting-0.2.9/pref_voting/voting_method.py
--rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.2.9/pref_voting/voting_methods.py
--rw-r--r--   0        0        0    49214 2023-05-16 18:00:25.171109 pref_voting-0.2.9/pref_voting/weighted_majority_graphs.py
--rw-r--r--   0        0        0      715 2023-05-16 22:54:29.631117 pref_voting-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     3819 1970-01-01 00:00:00.000000 pref_voting-0.2.9/setup.py
--rw-r--r--   0        0        0     3937 1970-01-01 00:00:00.000000 pref_voting-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1068 2022-07-08 15:47:57.000000 pref_voting-0.3/LICENSE
+-rw-r--r--   0        0        0     3198 2023-05-26 14:32:56.499334 pref_voting-0.3/README.md
+-rw-r--r--   0        0        0       20 2023-05-26 14:33:27.955784 pref_voting-0.3/pref_voting/__init__.py
+-rw-r--r--   0        0        0     9632 2023-05-24 13:13:44.583927 pref_voting-0.3/pref_voting/analysis.py
+-rw-r--r--   0        0        0     1226 2023-05-24 13:13:43.582814 pref_voting-0.3/pref_voting/axiom.py
+-rw-r--r--   0        0        0      360 2023-05-10 11:16:28.091090 pref_voting-0.3/pref_voting/axiom_helpers.py
+-rw-r--r--   0        0        0       91 2023-05-25 14:07:56.083200 pref_voting-0.3/pref_voting/axioms.py
+-rw-r--r--   0        0        0    23065 2023-05-10 11:22:02.837497 pref_voting-0.3/pref_voting/c1_methods.py
+-rw-r--r--   0        0        0     8564 2023-02-15 17:29:01.299008 pref_voting-0.3/pref_voting/combined_methods.py
+-rw-r--r--   0        0        0    11517 2023-05-10 11:58:43.699679 pref_voting-0.3/pref_voting/dominance_axioms.py
+-rw-r--r--   0        0        0    20643 2023-05-10 11:16:22.353419 pref_voting-0.3/pref_voting/generate_profiles.py
+-rw-r--r--   0        0        0     4664 2023-05-26 14:20:44.876014 pref_voting-0.3/pref_voting/generate_utility_profiles.py
+-rw-r--r--   0        0        0    10486 2023-05-24 13:13:45.272860 pref_voting-0.3/pref_voting/generate_weighted_majority_graphs.py
+-rw-r--r--   0        0        0     1806 2022-08-08 19:08:16.000000 pref_voting-0.3/pref_voting/helper.py
+-rw-r--r--   0        0        0    73193 2023-05-25 12:07:00.027553 pref_voting-0.3/pref_voting/iterative_methods.py
+-rw-r--r--   0        0        0    20246 2022-07-12 12:12:35.000000 pref_voting-0.3/pref_voting/maj_graph_ex1.png
+-rw-r--r--   0        0        0    59345 2023-05-25 15:31:46.387817 pref_voting-0.3/pref_voting/margin_based_methods.py
+-rw-r--r--   0        0        0    25681 2023-05-10 11:20:32.560828 pref_voting-0.3/pref_voting/other_methods.py
+-rw-r--r--   0        0        0    27160 2023-05-24 21:44:14.545976 pref_voting-0.3/pref_voting/profiles.py
+-rw-r--r--   0        0        0    23817 2023-05-26 10:29:19.112624 pref_voting-0.3/pref_voting/profiles_with_ties.py
+-rw-r--r--   0        0        0    12468 2023-05-26 10:23:18.532269 pref_voting-0.3/pref_voting/rankings.py
+-rw-r--r--   0        0        0    11066 2023-05-26 12:19:11.420399 pref_voting-0.3/pref_voting/scoring_methods.py
+-rw-r--r--   0        0        0     6661 2023-05-26 14:18:34.309764 pref_voting-0.3/pref_voting/utility_methods.py
+-rw-r--r--   0        0        0    13967 2023-05-26 12:07:03.892154 pref_voting-0.3/pref_voting/utility_profiles.py
+-rw-r--r--   0        0        0     8393 2023-05-26 10:50:34.876976 pref_voting-0.3/pref_voting/variable_voter_axioms.py
+-rw-r--r--   0        0        0     5395 2023-05-26 10:54:32.445716 pref_voting-0.3/pref_voting/voting_method.py
+-rw-r--r--   0        0        0      253 2022-07-31 21:02:46.000000 pref_voting-0.3/pref_voting/voting_methods.py
+-rw-r--r--   0        0        0    50074 2023-05-25 15:22:53.891568 pref_voting-0.3/pref_voting/weighted_majority_graphs.py
+-rw-r--r--   0        0        0      687 2023-05-26 14:33:27.954241 pref_voting-0.3/pyproject.toml
+-rw-r--r--   0        0        0     4149 1970-01-01 00:00:00.000000 pref_voting-0.3/setup.py
+-rw-r--r--   0        0        0     4264 1970-01-01 00:00:00.000000 pref_voting-0.3/PKG-INFO
```

### Comparing `pref_voting-0.2.9/LICENSE` & `pref_voting-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/README.md` & `pref_voting-0.3/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -56,15 +56,18 @@
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
-- v0.2.9 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
+- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
+- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
+- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
+- v0.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

### Comparing `pref_voting-0.2.9/pref_voting/analysis.py` & `pref_voting-0.3/pref_voting/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         vms (list(functions)): A list of voting methods,
         numbers_of_candidates (list(int), default = [3, 4, 5]): The numbers of candidates to check.
         numbers_of_voters (list(int), default = [5, 25, 50, 100]): The numbers of voters to check.
         all_unique_winners (bool, default = False): If True, only return profiles in which each voting method has a unique winner.
         show_profiles (bool, default=True): If True, show profiles with different winning sets for the voting methods when discovered.
         show_margin_graphs (bool, default=True): If True, show margin graphs of the profiles with different winning sets for the voting methods when discovered.
         show_winning_sets (bool, default=True): If True, show the different winning sets for the voting methods when discovered.
-        show_rankings_counts (bool, default=True): If True, show the rankins and counts of the profiles with different winning sets for the voting methods.
+        show_rankings_counts (bool, default=True): If True, show the rankings and counts of the profiles with different winning sets for the voting methods.
         return_multiple_profiles (bool, default=True): If True, return all profiles that are found.
         probmod (str, default="IC"): The probability model to be passed to the ``generate_profile`` method
         num_trials (int, default=10000): The number of profiles to check for different winning sets.
 
     """
     profiles = list()
     for num_cands in numbers_of_candidates:
```

### Comparing `pref_voting-0.2.9/pref_voting/axiom.py` & `pref_voting-0.3/pref_voting/axiom.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/pref_voting/c1_methods.py` & `pref_voting-0.3/pref_voting/c1_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/pref_voting/combined_methods.py` & `pref_voting-0.3/pref_voting/combined_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/pref_voting/dominance_axioms.py` & `pref_voting-0.3/pref_voting/dominance_axioms.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/pref_voting/generate_profiles.py` & `pref_voting-0.3/pref_voting/generate_profiles.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/pref_voting/generate_weighted_majority_graphs.py` & `pref_voting-0.3/pref_voting/generate_weighted_majority_graphs.py`

 * *Files 0% similar despite different names*

```diff
@@ -247,15 +247,15 @@
     a ceot as a ``MaringGraph`` where the margins represent the linear order of the edges.  
     
     Args:
         num_cands (int): the number of candidates
         parity (str, optional): The parity of the margins, either 'even' or 'odd'.
 
     Returns:
-        A generator of ``MarginGraph`` for ``num_candidats``
+        A generator of ``MarginGraph`` for ``num_candidates``
         
     .. warning:: It is only feasible to run this function for up to 5 candidates.    
 
     """
     
     assert parity in ["odd", "even"], "parity must be either 'odd' or 'even'"
     
@@ -286,15 +286,15 @@
     Enumerate all representatives from isomorphism classes of margin graphs with weights drawn from ``weight_domain``. 
     
     Args:
         num_cands (int): the number of candidates
         weight_domain (List[int]): The list of weights in the margin graph.
         
     Returns:
-        A generator of ``MarginGraph`` for ``num_candidats``
+        A generator of ``MarginGraph`` for ``num_candidates``
         
 
     .. warning:: It is only feasible to run this function for up to 5 candidates.    
 
     """
     
     weight_domain = sorted(weight_domain)
```

### Comparing `pref_voting-0.2.9/pref_voting/helper.py` & `pref_voting-0.3/pref_voting/helper.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/pref_voting/iterative_methods.py` & `pref_voting-0.3/pref_voting/iterative_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     
     Implementations of iterative voting methods.
 '''
 
 from pref_voting.voting_method import  *
 from pref_voting.voting_method import _num_rank_last, _num_rank_first
 from pref_voting.profiles import  _borda_score, _find_updated_profile
-from pref_voting.margin_based_methods import split_cycle_faster
+from pref_voting.margin_based_methods import split_cycle
 
 import copy
 from itertools import permutations, product
 import numpy as np
 
 @vm(name = "Instant Runoff")
 def instant_runoff(profile, curr_cands = None):
@@ -216,15 +216,15 @@
     
     rs, rcounts = profile.rankings_counts # get all the ranking data
         
     winners = [c for c in candidates 
                if _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
 
     if len(winners) == 0:
-        # run Instant Runoff with tie-breaker for each permulation of candidates
+        # run Instant Runoff with tie-breaker for each permutation of candidates
         for tb in permutations(candidates):
             winners += instant_runoff_tb(profile, curr_cands = curr_cands, tie_breaker = tb) 
     return sorted(list(set(winners)))
 
 
 # Create some aliases for instant runoff
 instant_runoff_put.set_name("Hare PUT")
@@ -311,15 +311,15 @@
             winners = [c for c in candidates 
                        if not isin(cands_to_ignore,c) and _num_rank_first(rs, rcounts, cands_to_ignore, c) >= strict_maj_size]
      
     return sorted(winners), elims_list
 
 
 @vm(name="Instant Runoff")
-def instant_runoff_for_truncated_linear_orders(profile, curr_cands = None, threshold = None, hide_warnings = False): 
+def instant_runoff_for_truncated_linear_orders(profile, curr_cands = None, threshold = None, hide_warnings = True): 
     """
     Instant Runoff for Truncated Linear Orders.  Iteratively remove the candidates with the fewest number of first place votes, until there is a candidate with more than the threshold number of first-place votes. 
     If a threshold is not set, then it is strictly more than half of the non-empty ballots. 
     
     Args:
         profile (ProfileWithTies): An anonymous profile with no ties in the ballots (note that ProfileWithTies allows for truncated linear orders).
         threshold (int, float, optional): The threshold needed to win the election.  If it is not set, then it is strictly more than half of the remaining ballots.
@@ -975,15 +975,15 @@
 
     candidates = profile.candidates if curr_cands is None else curr_cands    
     cw = profile.condorcet_winner(curr_cands=curr_cands)
     
     winners = list() if cw is None else [cw]
 
     if len(winners) == 0:
-        # run Coombs with tie-breaker for each permulation of candidates
+        # run Coombs with tie-breaker for each permutation of candidates
         for tb in permutations(candidates):
             winners += baldwin_tb(profile, curr_cands = curr_cands, tie_breaker = tb) 
 
     return sorted(list(set(winners)))
 
 
 def baldwin_with_explanation(profile, curr_cands = None):
@@ -1476,29 +1476,29 @@
 
     :Example: 
 
     .. exec_code:: 
 
         from pref_voting.profiles import Profile
         from pref_voting.iterative_methods import iterated_split_cycle
-        from pref_voting.margin_based_methods import split_cycle_faster
+        from pref_voting.margin_based_methods import split_cycle
         
         prof = Profile([[2, 0, 3, 1], [2, 3, 0, 1], [3, 1, 2, 0], [2, 1, 3, 0], [3, 0, 1, 2], [1, 2, 3, 0]], [1, 1, 1, 1, 1, 2])
 
         prof.display()
-        split_cycle_faster.display(prof)
+        split_cycle.display(prof)
         iterated_split_cycle.display(prof)
     
     """    
     prev_sc_winners = edata.candidates if curr_cands is None else curr_cands
-    sc_winners = split_cycle_faster(edata, curr_cands = curr_cands, strength_function = strength_function)
+    sc_winners = split_cycle(edata, curr_cands = curr_cands, strength_function = strength_function)
     
     while len(sc_winners) != 1 and sc_winners != prev_sc_winners: 
         prev_sc_winners = sc_winners
-        sc_winners = split_cycle_faster(edata, curr_cands = sc_winners, strength_function = strength_function)
+        sc_winners = split_cycle(edata, curr_cands = sc_winners, strength_function = strength_function)
         
     return sorted(sc_winners)
 
 @vm(name = "Benham")
 def benham(profile, curr_cands = None):
     """
     As long as the profile has no Condorcet winner, eliminate the candidate with the lowest plurality score. Then elect the Condorcet winner of the restricted profile. 
@@ -1623,15 +1623,15 @@
     cands_to_ignore = np.empty(0) if curr_cands is None else np.array([c for c in profile.candidates if c not in curr_cands])
     
     cw = profile.condorcet_winner(curr_cands = [c for c in profile.candidates if not isin(cands_to_ignore, c)])
     
     winners = [cw] if cw is not None else list()
         
     if len(winners) == 0:
-        # run Instant Runoff with tie-breaker for each permulation of candidates
+        # run Instant Runoff with tie-breaker for each permutation of candidates
         for tb in permutations(candidates):
             winners += instant_runoff_tb(profile, curr_cands = curr_cands, tie_breaker = tb) 
     return sorted(list(set(winners)))
     
 iterated_vms = [
     instant_runoff,
     instant_runoff_tb,
```

### Comparing `pref_voting-0.2.9/pref_voting/maj_graph_ex1.png` & `pref_voting-0.3/pref_voting/maj_graph_ex1.png`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/pref_voting/margin_based_methods.py` & `pref_voting-0.3/pref_voting/margin_based_methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,17 +7,15 @@
     Implementations of voting methods that work on both profiles and margin graphs.
 '''
 
 from pref_voting.voting_method import  *
 from pref_voting.helper import get_mg
 import math
 from itertools import product, permutations, combinations, chain
-
 import networkx as nx
-import matplotlib.pyplot as plt
 
 
 @vm(name = "Minimax")
 def minimax(edata, curr_cands = None, strength_function = None):   
     """
     The Minimax winners are the candidates with the smallest maximum pairwise defeat.  That is, for each candidate :math:`a` find the biggest margin of a candidate :math:`b` over :math:`a`, then elect the candidate(s) with the smallest such loss. Also known as the Simpson-Kramer Rule.
     
@@ -149,15 +147,15 @@
         strength_function (function, optional): The strength function to be used to calculate the strength of a path.   The default is the margin method of ``edata``.   This only matters when the ballots are not linear orders. 
 
     Returns: 
         A sorted list of candidates. 
 
     .. seealso::
 
-        :meth:`pref_voting.margin_based_methods.beat_path_faster`, :meth:`pref_voting.margin_based_methods.beat_path_defeat`
+        :meth:`pref_voting.margin_based_methods.beat_path_Floyd_Warshall`, :meth:`pref_voting.margin_based_methods.beat_path_defeat`
 
 
     :Example: 
 
     .. plot::  margin_graphs_examples/mg_ex_bp_rp.py
         :context: reset  
         :include-source: True
@@ -201,16 +199,16 @@
     for c in candidates: 
         if all([beat_paths_weights[c][c2] >= beat_paths_weights[c2][c] for c2 in candidates  if c2 != c]):
             winners.append(c)
     return sorted(list(winners))
 
 
 @vm(name="Beat Path")
-def beat_path_faster(edata, curr_cands = None, strength_function = None):   
-    """An implementation of Beat Path using a variation of the Floyd Warshall-Algorithm
+def beat_path_Floyd_Warshall(edata, curr_cands = None, strength_function = None):   
+    """An implementation of Beat Path using a variation of the Floyd-Warshall Algorithm
     See https://en.wikipedia.org/wiki/Schulze_method#Implementation)
  
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         strength_function (function, optional): The strength function to be used to calculate the strength of a path.   The default is the margin method of ``edata``.   This only matters when the ballots are not linear orders. 
 
@@ -227,30 +225,30 @@
     .. plot::  margin_graphs_examples/mg_ex_bp_rp.py
         :context: reset  
         :include-source: True
 
 
     .. code-block:: 
 
-        from pref_voting.margin_based_methods import beat_path_faster
+        from pref_voting.margin_based_methods import beat_path_Floyd_Warshall
 
         beat_path.display(mg)
-        beat_path_faster.display(mg)
+        beat_path_Floyd_Warshall.display(mg)
 
 
     .. exec_code:: 
         :hide_code:
 
         from pref_voting.weighted_majority_graphs import MarginGraph
-        from pref_voting.margin_based_methods import beat_path, beat_path_faster
+        from pref_voting.margin_based_methods import beat_path, beat_path_Floyd_Warshall
         
         mg = MarginGraph([0, 1, 2, 3], [(0, 2, 3), (1, 0, 5), (2, 1, 5), (2, 3, 1), (3, 0, 3), (3, 1, 1)])
 
         beat_path.display(mg)
-        beat_path_faster.display(mg)
+        beat_path_Floyd_Warshall.display(mg)
 
     """
 
     candidates = edata.candidates if curr_cands is None else curr_cands    
     strength_function = edata.margin if strength_function is None else strength_function
         
     s_matrix = [[-np.inf for _ in candidates] for _ in candidates]
@@ -282,72 +280,91 @@
         strength_function (function, optional): The strength function to be used to calculate the strength of a path.   The default is the margin method of ``edata``.   This only matters when the ballots are not linear orders. 
 
     Returns: 
         A networkx DiGraph representing the Beat Path defeat relation. 
 
     .. seealso::
 
-        :meth:`pref_voting.margin_based_methods.beat_path`, :meth:`pref_voting.margin_based_methods.beat_path_faster`
+        :meth:`pref_voting.margin_based_methods.beat_path`, :meth:`pref_voting.margin_based_methods.beat_path_Floyd_Warshall`
 
     :Example: 
 
     .. plot::  margin_graphs_examples/mg_ex_bp_defeat.py
         :context: reset  
         :include-source: True
 
     """
 
-    defeat = nx.DiGraph()
-    
     candidates = edata.candidates if curr_cands is None else curr_cands    
     strength_function = edata.margin if strength_function is None else strength_function
-    
-    mg = get_mg(edata, curr_cands = curr_cands)
-    
-    beat_paths_weights = {c: {c2:0 for c2 in candidates if c2 != c} for c in candidates}
-    for c in candidates: 
-        for other_c in beat_paths_weights[c].keys():
-            all_paths = list(nx.all_simple_paths(mg, c, other_c))
-            if len(all_paths) > 0:
-                beat_paths_weights[c][other_c] = max([min([strength_function(p[i], p[i+1]) for i in range(0,len(p)-1)]) for p in all_paths])
         
-    defeat.add_nodes_from(candidates)
-    edges = list()
-    for c1 in candidates: 
-        for c2 in candidates: 
-            if c1 != c2: 
-                if beat_paths_weights[c1][c2] > beat_paths_weights[c2][c1]: 
-                    edges.append((c1, c2))
+    s_matrix = [[-np.inf for _ in candidates] for _ in candidates]
+    for c1_idx, c1 in enumerate(candidates):
+        for c2_idx, c2 in enumerate(candidates):
+            if (edata.majority_prefers(c1, c2) or c1 == c2):
+                s_matrix[c1_idx][c2_idx] = strength_function(c1, c2) 
+    strength = list(map(lambda i : list(map(lambda j : j , i)) , s_matrix))
+    for i_idx, i in enumerate(candidates):         
+        for j_idx, j in enumerate(candidates): 
+            if i!= j:
+                for k_idx, k in enumerate(candidates): 
+                    if i!= k and j != k:
+                        strength[j_idx][k_idx] = max(strength[j_idx][k_idx], min(strength[j_idx][i_idx],strength[i_idx][k_idx]))
 
-    defeat.add_edges_from(edges)
-    return defeat
+    defeat_graph = nx.DiGraph()
+    defeat_graph.add_nodes_from(candidates)
     
+    for i_idx, i in enumerate(candidates): 
+        for j_idx, j in enumerate(candidates):
+            if i!=j:
+                if strength[j_idx][i_idx] > strength[i_idx][j_idx]:
+                    defeat_graph.add_weighted_edges_from([(j,i,s_matrix[j_idx][i_idx])])
+
+    return defeat_graph
+    
+def has_strong_path(A, source, target, k):
+    """Given a square matrix A, return True if there is a path from source to target in the associated directed graph     where each edge has a weight greater than or equal to k, and False otherwise."""
+    
+    n = A.shape[0] # assume A is a square matrix
+    visited = np.zeros(n, dtype=bool)
+
+    def dfs(node):
+        if node == target:
+            return True
+        visited[node] = True
+        for neighbor, weight in enumerate(A[node, :]):
+            if weight >= k and not visited[neighbor]:
+                if dfs(neighbor):
+                    return True
+        return False
+
+    return dfs(source)
+
 @vm(name="Split Cycle")
 def split_cycle(edata, curr_cands = None, strength_function = None):
+
     """A **majority cycle** is a sequence :math:`x_1, \ldots ,x_n` of distinct candidates with :math:`x_1=x_n` such that for :math:`1 \leq k \leq n-1`,  :math:`x_k` is majority preferred to :math:`x_{k+1}`.  The Split Cycle winners are determined as follows:  
     
-    1. In each cycle, identify the head-to-head win(s) with the smallest margin of victory in that cycle.
-    2. After completing step 1 for all cycles, discard the identified wins. All remaining wins count as defeats of the losing candidates.
-
-    The candidates that are undefeated are the Split Cycle winners. 
+    If candidate x has a positive margin over y and (x,y) is not the weakest edge in a cycle, then x defeats y. Equivalently, if x has a positive margin over y and there is no path from y back to x of strength at least the margin of x over y, then x defeats y. 
+    
+    The candidates that are undefeated are the Split Cycle winners.
 
     See https://github.com/epacuit/splitcycle and the paper https://arxiv.org/abs/2004.02350 for more information. 
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
         strength_function (function, optional): The strength function to be used to calculate the strength of a path.   The default is the margin method of ``edata``.   This only matters when the ballots are not linear orders. 
 
     Returns: 
         A sorted list of candidates. 
 
     .. seealso::
 
-        :meth:`pref_voting.margin_based_methods.split_cycle_faster`, :meth:`pref_voting.margin_based_methods.split_cycle_defeat`
-
+        :meth:`pref_voting.margin_based_methods.split_cycle_Floyd_Warshall`, :meth:`pref_voting.margin_based_methods.split_cycle_defeat`
 
     :Example: 
 
     .. plot::  margin_graphs_examples/mg_ex_bp_rp.py
         :context: reset  
         :include-source: True
 
@@ -364,60 +381,35 @@
 
         from pref_voting.weighted_majority_graphs import MarginGraph
         from pref_voting.margin_based_methods import split_cycle
         
         mg = MarginGraph([0, 1, 2, 3], [(0, 2, 3), (1, 0, 5), (2, 1, 5), (2, 3, 1), (3, 0, 3), (3, 1, 1)])
         
         split_cycle.display(mg)
-
-
     """
+    
+    candidates = edata.candidates if curr_cands is None else curr_cands  
+
+    strength_matrix = np.array(edata.margin_matrix) if strength_function is None else np.array([[strength_function(edata.cindex_to_cand(a_idx),edata.cindex_to_cand(b_idx)) for b_idx in edata.cindices] for a_idx in edata.cindices])
 
-    candidates = edata.candidates if curr_cands is None else curr_cands    
     strength_function = edata.margin if strength_function is None else strength_function 
-    
-    # create the majority graph
-    mg = get_mg(edata, curr_cands = curr_cands) 
-    
-    # find the cycle number for each candidate
-    cycle_number = {cs:0 for cs in permutations(candidates,2)}
-    for cycle in nx.simple_cycles(mg): # for each cycle in the margin graph
-        
-        # get all the margins (i.e., the weights) of the edges in the cycle
-        strengths = list() 
-        for idx,c1 in enumerate(cycle): 
-            next_idx = idx + 1 if (idx + 1) < len(cycle) else 0
-            c2 = cycle[next_idx]
-            strengths.append(strength_function(c1, c2))
-            
-        split_number = min(strengths) # the split number of the cycle is the minimal margin
-        
-        for c1,c2 in cycle_number.keys():
-            c1_index = cycle.index(c1) if c1 in cycle else -1
-            c2_index = cycle.index(c2) if c2 in cycle else -1
-
-            # only need to check cycles with an edge from c1 to c2
-            if (c1_index != -1 and c2_index != -1) and ((c2_index == c1_index + 1) or (c1_index == len(cycle)-1 and c2_index == 0)):
-                cycle_number[(c1,c2)] = split_number if split_number > cycle_number[(c1,c2)] else cycle_number[(c1,c2)]        
-    
-    # construct the defeat relation, where a defeats b if margin(a,b) > cycle_number(a,b) (see Lemma 3.13)
-    defeat = nx.DiGraph()
-    defeat.add_nodes_from(candidates)
-    defeat.add_edges_from([(c1,c2)  
-           for c1 in candidates 
-           for c2 in candidates if c1 != c2 if edata.majority_prefers(c1, c2) and strength_function(c1,c2) > cycle_number[(c1,c2)]])
-   
-    # the winners are candidates not defeated by any other candidate
-    winners = maximal_elements(defeat)
-    
-    return sorted(list(set(winners)))
+
+    potential_winners = set(edata.candidates)
+
+    for a in candidates:
+        for b in candidates:
+            if strength_function(b,a) > 0 and not has_strong_path(strength_matrix, edata.cand_to_cindex(a), edata.cand_to_cindex(b), strength_function(b,a)):
+                potential_winners.discard(a)
+                break
+
+    return sorted(potential_winners)
 
 
 @vm(name="Split Cycle")
-def split_cycle_faster(edata, curr_cands = None, strength_function = None):   
+def split_cycle_Floyd_Warshall(edata, curr_cands = None, strength_function = None):   
     """An implementation of Split Cycle based on the Floyd-Warshall Algorithm. 
 
     See https://github.com/epacuit/splitcycle and the paper https://arxiv.org/abs/2004.02350 for more information. 
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
@@ -436,30 +428,30 @@
     .. plot::  margin_graphs_examples/mg_ex_bp_rp.py
         :context: reset  
         :include-source: True
 
 
     .. code-block:: 
 
-        from pref_voting.margin_based_methods import split_cycle, split_cycle_faster
+        from pref_voting.margin_based_methods import split_cycle, split_cycle_Floyd_Warshall
 
         split_cycle.display(mg)
-        split_cycle_faster.display(mg)
+        split_cycle_Floyd_Warshall.display(mg)
 
 
     .. exec_code:: 
         :hide_code:
 
         from pref_voting.weighted_majority_graphs import MarginGraph
-        from pref_voting.margin_based_methods import split_cycle, split_cycle_faster
+        from pref_voting.margin_based_methods import split_cycle, split_cycle_Floyd_Warshall
         
         mg = MarginGraph([0, 1, 2, 3], [(0, 2, 3), (1, 0, 5), (2, 1, 5), (2, 3, 1), (3, 0, 3), (3, 1, 1)])
         
         split_cycle.display(mg)
-        split_cycle_faster.display(mg)
+        split_cycle_Floyd_Warshall.display(mg)
 
 
     """
 
     candidates = edata.candidates if curr_cands is None else curr_cands    
     strength_function = edata.margin if strength_function is None else strength_function 
  
@@ -486,73 +478,71 @@
         for j_idx, j in enumerate(candidates):
             if i != j:
                 if s_matrix[j_idx][i_idx] > strength[i_idx][j_idx]: # the main difference with Beat Path
                     winners[i] = False
     return sorted([c for c in candidates if winners[c]])
 
 
-def split_cycle_defeat(edata, curr_cands = None):
+def split_cycle_defeat(edata, curr_cands = None, strength_function = None):   
     """
     Returns the Split Cycle defeat relation. 
 
     See https://arxiv.org/abs/2008.08451 for an extended discussion of this notion of defeat in an election. 
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
         curr_cands (List[int], optional): If set, then find the winners for the profile restricted to the candidates in ``curr_cands``
-        strength_function (function, optional): The strength function to be used to calculate the strength of a path.   The default is the margin method of ``edata``.   This only matters when the ballots are not linear orders. 
 
     Returns: 
-        A networkx DiGraph representing the Beat Path defeat relation. 
+        A networkx DiGraph representing the Split Cycle defeat relation. 
 
     .. seealso::
 
-        :meth:`pref_voting.margin_based_methods.split_cycle`, :meth:`pref_voting.margin_based_methods.split_cycle_faster`
+        :meth:`pref_voting.margin_based_methods.split_cycle`, :meth:`pref_voting.margin_based_methods.split_cycle_Floyd_Warshall`
 
     :Example: 
 
     .. plot::  margin_graphs_examples/mg_ex_sc_defeat.py
         :context: reset  
         :include-source: True
 
     """
+
+    candidates = edata.candidates if curr_cands is None else curr_cands    
+    strength_function = edata.margin if strength_function is None else strength_function 
+ 
+    weak_condorcet_winners = {c:True for c in candidates}
+    s_matrix = [[-np.inf for _ in candidates] for _ in candidates]
     
-    candidates = edata.candidates if curr_cands is None else curr_cands
-    
-    # create the margin graph
-    mg = get_mg(edata, curr_cands = curr_cands)
+    # initialize the s_matrix
+    for c1_idx, c1 in enumerate(candidates):
+        for c2_idx, c2 in enumerate(candidates):
+            if (edata.majority_prefers(c1, c2) or c1 == c2):
+                s_matrix[c1_idx][c2_idx] = strength_function(c1, c2) 
+                weak_condorcet_winners[c2] = weak_condorcet_winners[c2] and (c1 == c2) # weak Condorcet winners are Split Cycle winners
     
-    # find the cycle number for each candidate
-    cycle_number = {cs:0 for cs in permutations(candidates,2)}
-    for cycle in nx.simple_cycles(mg): # for each cycle in the margin graph
-
-        # get all the margins (i.e., the weights) of the edges in the cycle
-        margins = list() 
-        for idx,c1 in enumerate(cycle): 
-            next_idx = idx + 1 if (idx + 1) < len(cycle) else 0
-            c2 = cycle[next_idx]
-            margins.append(edata.margin(c1, c2))
-            
-        split_number = min(margins) # the split number of the cycle is the minimal margin
-        for c1,c2 in cycle_number.keys():
-            c1_index = cycle.index(c1) if c1 in cycle else -1
-            c2_index = cycle.index(c2) if c2 in cycle else -1
-
-            # only need to check cycles with an edge from c1 to c2
-            if (c1_index != -1 and c2_index != -1) and ((c2_index == c1_index + 1) or (c1_index == len(cycle)-1 and c2_index == 0)):
-                cycle_number[(c1,c2)] = split_number if split_number > cycle_number[(c1,c2)] else cycle_number[(c1,c2)]        
-
-    # construct the defeat relation, where a defeats b if margin(a,b) > cycle_number(a,b) (see Lemma 3.13)
-    defeat = nx.DiGraph()
-    defeat.add_nodes_from(candidates)
-    defeat.add_weighted_edges_from([(c1,c2, edata.margin(c1, c2))  
-           for c1 in candidates 
-           for c2 in candidates if c1 != c2 if edata.margin(c1,c2) > cycle_number[(c1,c2)]])
+    strength = list(map(lambda i : list(map(lambda j : j , i)) , s_matrix))
+    for i_idx, i in enumerate(candidates): 
+        for j_idx, j in enumerate(candidates):
+            if i!= j:
+                if not weak_condorcet_winners[j]: # weak Condorcet winners are Split Cycle winners
+                    for k_idx, k in enumerate(candidates): 
+                        if i != k and j != k:
+                            strength[j_idx][k_idx] = max(strength[j_idx][k_idx], min(strength[j_idx][i_idx],strength[i_idx][k_idx]))
+ 
+    defeat_graph = nx.DiGraph()
+    defeat_graph.add_nodes_from(candidates)
 
-    return defeat
+    for i_idx, i in enumerate(candidates):
+        for j_idx, j in enumerate(candidates):
+            if i != j:
+                if s_matrix[j_idx][i_idx] > strength[i_idx][j_idx]: # the main difference with Beat Path
+                    defeat_graph.add_weighted_edges_from([(j,i,s_matrix[j_idx][i_idx])])
+                
+    return defeat_graph
 
 
 
 # flatten a 2d list - turn a 2d list into a single list of items
 flatten = lambda l: [item for sublist in l for item in sublist]
 
 def does_create_cycle(g, edge):
@@ -1087,60 +1077,52 @@
                         if does_create_cycle(river_defeat, e):
                             river_defeat.remove_edge(e[0], e[1])
                 winners.append(maximal_elements(river_defeat)[0])
     return sorted(list(set(winners)))
 
 # Simple Stable Voting 
 def _simple_stable_voting(edata, 
-                          curr_cands = None, 
-                          mem_sv_winners = {}, 
-                          strength_function = None,
-                          sorted_matches = None): 
+                          curr_cands, 
+                          strength_function,
+                          mem_sv_winners, 
+                          sorted_matches):
     '''
     Determine the Simple Stable Voting winners while keeping track 
     of the winners in any subprofiles checked during computation. 
     '''
     
-    # curr_cands is the set of candidates who have not been removed
-    curr_cands = edata.candidates if curr_cands is None else curr_cands
-    strength_function = edata.margin if strength_function is None else strength_function  
-    
     sv_winners = list()
-
-    if sorted_matches is None:
-        matches = [(a, b, strength_function(a, b)) for a in curr_cands for b in curr_cands if a != b]
-        sorted_matches = sorted(matches, reverse=True, key=lambda m_w_weight: m_w_weight[2])
         
     if len(curr_cands) == 1: 
         mem_sv_winners[tuple(curr_cands)] = curr_cands
         return curr_cands, mem_sv_winners
     
-    max_margin_witnessing_win = -math.inf
+    margin_witnessing_win = -math.inf
 
     for a, b, s in sorted_matches:
-        if s < max_margin_witnessing_win: 
+        if s < margin_witnessing_win: 
             break
         if a not in sv_winners: 
             cands_minus_b = [c for c in curr_cands if c != b]
             cands_minus_b_key = tuple(sorted(cands_minus_b))
             if cands_minus_b_key not in mem_sv_winners.keys(): 
                 ws, mem_sv_winners = _simple_stable_voting(edata, 
                                                            curr_cands = cands_minus_b,
-                                                           mem_sv_winners = mem_sv_winners,
-                                                           strength_function = strength_function, 
+                                                           strength_function = strength_function,
+                                                           mem_sv_winners = mem_sv_winners, 
                                                            sorted_matches = [(a, c, s) for a, c, s in sorted_matches if c != b and a != b])
                 mem_sv_winners[cands_minus_b_key] = ws
             else: 
                 ws = mem_sv_winners[cands_minus_b_key]
             if a in ws:
                 sv_winners.append(a)
-                max_margin_witnessing_win = s
-    return sv_winners, mem_sv_winners
+                margin_witnessing_win = s
 
-          
+    return sv_winners, mem_sv_winners
+    
 @vm(name = "Simple Stable Voting")
 def simple_stable_voting(edata, curr_cands = None, strength_function = None): 
     """Implementation of  Simple Stable Voting from https://arxiv.org/abs/2108.00542. 
 
     Simple Stable Voting is a recursive voting method defined as follows: 
 
     1.  If there is only one candidate in the profile, then that candidate is the winner. 
@@ -1168,20 +1150,25 @@
 
         mg = MarginGraph([0, 1, 2, 3], [(0, 3, 8), (1, 0, 10), (2, 0, 4), (2, 1, 8), (3, 1, 8)])
 
         simple_stable_voting.display(mg)
 
     """
     
+    curr_cands = edata.candidates if curr_cands is None else curr_cands
+    strength_function = edata.margin if strength_function is None else strength_function  
+
+    matches = [(a, b, strength_function(a, b)) for a in curr_cands for b in curr_cands if a != b]
+    sorted_matches = sorted(matches, reverse=True, key=lambda m_w_weight: m_w_weight[2])
+    
     return sorted(_simple_stable_voting(edata, 
                                         curr_cands = curr_cands, 
+                                        strength_function = strength_function,
                                         mem_sv_winners = {}, 
-                                        strength_function = strength_function)[0],
-                                        sorted_matches = None)
-
+                                        sorted_matches = sorted_matches)[0])
 
 @vm(name = "Simple Stable Voting")
 def simple_stable_voting_faster(edata, curr_cands = None, strength_function = None): 
     """Simple Stable Voting is Condorcet consistent.   It is faster to skip executing the recursive algorithm when there is a Condorcet winnerFirst check if there is a Condorcet winner.  If so, return the Condorcet winner, otherwise find the Simple Stable Voting winner using _simple_stable_voting
 
     Args:
         edata (Profile, ProfileWithTies, MarginGraph): Any election data that has a `margin` method. 
@@ -1210,66 +1197,65 @@
 
     """
     
     cw = edata.condorcet_winner(curr_cands = None)
     if cw is not None: 
         return [cw]
     else: 
+        curr_cands = edata.candidates if curr_cands is None else curr_cands
+        strength_function = edata.margin if strength_function is None else strength_function  
+
+        matches = [(a, b, strength_function(a, b)) for a in curr_cands for b in curr_cands if a != b]
+        sorted_matches = sorted(matches, reverse=True, key=lambda m_w_weight: m_w_weight[2])
+    
         return sorted(_simple_stable_voting(edata, 
                                             curr_cands = curr_cands, 
+                                            strength_function = strength_function,
                                             mem_sv_winners = {}, 
-                                            strength_function = strength_function)[0],
-                                            sorted_matches = None)
+                                            sorted_matches = sorted_matches)[0])
 
     
 def _stable_voting(edata, 
-                   curr_cands = None,
-                   mem_sv_winners = {}, 
-                   strength_function = None, 
-                   sorted_matches = None): 
+                   curr_cands,
+                   strength_function,
+                   mem_sv_winners,
+                   sorted_matches): 
     '''
     Determine the Stable Voting winners for the profile while keeping track of the winners in any subprofiles checked during computation. 
     '''
     
-    # curr_cands is the set of candidates who have not been removed
-    curr_cands = edata.candidates if curr_cands is None else curr_cands
-    strength_function = edata.margin if strength_function is None else strength_function  
-    
     sv_winners = list()
     
-    undefeated_candidates = split_cycle_faster(edata, curr_cands = curr_cands)
+    undefeated_candidates = split_cycle(edata, curr_cands = curr_cands)
 
-    if sorted_matches is None:
-        matches = [(a, b, strength_function(a, b)) for a in curr_cands for b in curr_cands if a != b]
-        sorted_matches = sorted(matches, reverse=True, key=lambda m_w_weight: m_w_weight[2])
-        
     if len(curr_cands) == 1: 
         mem_sv_winners[tuple(curr_cands)] = curr_cands
         return curr_cands, mem_sv_winners
     
-    max_margin_witnessing_win = -math.inf
+    margin_witnessing_win = -math.inf
 
     for a, b, s in sorted_matches:
-        if s < max_margin_witnessing_win: 
+        if s < margin_witnessing_win: 
             break
         if a in undefeated_candidates and a not in sv_winners: 
             cands_minus_b = [c for c in curr_cands if c != b]
             cands_minus_b_key = tuple(sorted(cands_minus_b))
             if cands_minus_b_key not in mem_sv_winners.keys(): 
                 ws, mem_sv_winners = _stable_voting(edata,
                                                     curr_cands = cands_minus_b,
+                                                    strength_function = strength_function,
                                                     mem_sv_winners = mem_sv_winners,
-                                                    strength_function = strength_function, 
                                                     sorted_matches = [(a, c, s) for a, c, s in sorted_matches if c != b and a != b])
                 mem_sv_winners[cands_minus_b_key] = ws
             else: 
                 ws = mem_sv_winners[cands_minus_b_key]
             if a in ws:
                 sv_winners.append(a)
-                max_margin_witnessing_win = s
+                margin_witnessing_win = s
+                
     return sv_winners, mem_sv_winners
         
 @vm(name = "Stable Voting")
 def stable_voting(edata, curr_cands = None, strength_function = None): 
     """Implementation of  Stable Voting from https://arxiv.org/abs/2108.00542. 
 
     Stable Voting is a recursive voting method defined as follows: 
@@ -1298,20 +1284,26 @@
         from pref_voting.margin_based_methods import stable_voting
 
         mg = MarginGraph([0, 1, 2, 3], [(0, 3, 8), (1, 0, 10), (2, 0, 4), (2, 1, 8), (3, 1, 8)])
 
         stable_voting.display(mg)
 
     """
+
+    curr_cands = edata.candidates if curr_cands is None else curr_cands
+    strength_function = edata.margin if strength_function is None else strength_function  
+
+    matches = [(a, b, strength_function(a, b)) for a in curr_cands for b in curr_cands if a != b]
+    sorted_matches = sorted(matches, reverse=True, key=lambda m_w_weight: m_w_weight[2])
+
     return sorted(_stable_voting(edata, 
                                  curr_cands = curr_cands, 
+                                 strength_function = strength_function,
                                  mem_sv_winners = {}, 
-                                 strength_function = strength_function)[0],
-                                 sorted_matches = None)
-
+                                 sorted_matches = sorted_matches)[0])
 
 @vm(name = "Stable Voting")
 def stable_voting_faster(edata, curr_cands = None, strength_function = None): 
     """
     Stable Voting is Condorcet consistent.   It is faster to skip executing the recursive algorithm when there is a Condorcet winner.  
 
     Args:
@@ -1341,28 +1333,33 @@
 
 
     """
     cw = edata.condorcet_winner(curr_cands = curr_cands)
     if cw is not None: 
         return [cw]
     else: 
-        return sorted(_stable_voting(edata, 
-                                     curr_cands = curr_cands, 
-                                     mem_sv_winners = {}, 
-                                     strength_function = strength_function)[0],
-                                     sorted_matches = None) 
+        curr_cands = edata.candidates if curr_cands is None else curr_cands
+        strength_function = edata.margin if strength_function is None else strength_function  
 
+        matches = [(a, b, strength_function(a, b)) for a in curr_cands for b in curr_cands if a != b]
+        sorted_matches = sorted(matches, reverse=True, key=lambda m_w_weight: m_w_weight[2])
+
+        return sorted(_stable_voting(edata, 
+                                    curr_cands = curr_cands, 
+                                    strength_function = strength_function,
+                                    mem_sv_winners = {}, 
+                                    sorted_matches = sorted_matches)[0])
 
 
 mg_vms = [
     minimax, 
     split_cycle,
-    split_cycle_faster,
+    split_cycle_Floyd_Warshall,
     beat_path,
-    beat_path_faster,
+    beat_path_Floyd_Warshall,
     #ranked_pairs,
     #ranked_pairs_with_test,
     ranked_pairs_zt,
     ranked_pairs_tb,
     #river,
     #river_with_test, 
     simple_stable_voting,
@@ -1371,21 +1368,21 @@
     stable_voting_faster,
 ]
 
 
 mg_vms_all = [
     minimax, 
     split_cycle,
-    split_cycle_faster,
+    split_cycle_Floyd_Warshall,
     beat_path,
-    beat_path_faster,
+    beat_path_Floyd_Warshall,
     ranked_pairs,
     ranked_pairs_with_test,
     ranked_pairs_zt,
     ranked_pairs_tb,
     river,
     river_with_test, 
     simple_stable_voting,
     simple_stable_voting_faster,
     stable_voting,
     stable_voting_faster,
-]
+]
```

### Comparing `pref_voting-0.2.9/pref_voting/other_methods.py` & `pref_voting-0.3/pref_voting/other_methods.py`

 * *Files identical despite different names*

### Comparing `pref_voting-0.2.9/pref_voting/profiles.py` & `pref_voting-0.3/pref_voting/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,14 +172,19 @@
         """constructor method"""
         
         self.num_cands = len(rankings[0]) if len(rankings) > 0 else 0 
         """The number of candidates"""
 
         self.candidates = list(range(0, self.num_cands)) 
         
+        # needed for uniformity with ProfileWithTies and MarginGraph
+        self.cindices = self.candidates
+        self.cand_to_cindex = lambda c: c
+        self.cindex_to_cand = lambda i: i
+
         # linear ordering of the candidates for each voter
         self._rankings = np.array(rankings)   
         
         # for number of each ranking
         self._rcounts = np.array([1]*len(rankings)) if rcounts is None else np.array(rcounts) 
         
         # for each voter, the rankings of each candidate
@@ -424,14 +429,15 @@
 
     def majority_graph(self): 
         """Returns the majority graph of the profile.  See :class:`.MarginGraph`.  
         """
     
         return MajorityGraph.from_profile(self)
 
+    @property
     def margin_matrix(self):
         """Returns the margin matrix of the profile: A matrix where the :math:`i, j` entry is the margin of candidate :math:`i` over candidate :math:`j`.    
         """
 
         return [[self.margin(c1,c2) for c2 in self.candidates] for c1 in self.candidates]
     
     def is_uniquely_weighted(self): 
@@ -539,15 +545,15 @@
         
         return latex_str
 
     def display_margin_matrix(self): 
         """Display the margin matrix using tabulate.
         """
         
-        print(tabulate(self.margin_matrix(), tablefmt="grid"))   
+        print(tabulate(self.margin_matrix, tablefmt="grid"))   
 
     def display_margin_graph(self, cmap=None, curr_cands = None):
         """ 
         Display the margin graph of the profile (restricted to ``curr_cands``) using the ``cmap``.  See :class:`.MarginGraph`. 
         """
 
         cmap = cmap if cmap is not None else self.cmap
```

### Comparing `pref_voting-0.2.9/pref_voting/profiles_with_ties.py` & `pref_voting-0.3/pref_voting/profiles_with_ties.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,358 +8,33 @@
     Functions to reason about profiles of (truncated) strict weak orders.
 """
 
 from math import ceil
 import copy
 import numpy as np
 from tabulate import tabulate
+from pref_voting.profiles import Profile
+from pref_voting.rankings import Ranking
 from pref_voting.weighted_majority_graphs import (
     MajorityGraph,
     MarginGraph,
     SupportGraph,
 )
 
-class Ranking(object):
-    """A ranking of a set of candidates.
-
-    A ranking is a map from candidates to ranks (integers).  There is no assumption that all candidates in an election are ranked.
-
-    :param rmap: Dictionary in which the keys are the candidates and the values are the ranks.
-    :type rmap: dict[int or str: int]
-    :param cmap: Dictionary mapping candidates (keys of the ``rmap``) to candidate names (strings).  If not provied, each candidate  is mapped to itself.
-    :type cmap: dict[int: str], optional
-
-    :Example:
-
-    The following code creates three rankings:
-
-    1. ``rank1`` is the ranking where 0 is ranked first, 2 is ranked in second-place, and 1 is ranked last.
-    2. ``rank2`` is the ranking where 0 and 1 are tied for first place, and 2 is ranked last.
-    3. ``rank3`` is the ranking where 0 is ranked first, and 2 is ranked in last place.
-
-    .. code-block:: python
-
-            rank1 = Ranking({0:1, 1:3, 2:2})
-            rank2 = Ranking({0:1, 1:1, 2:2})
-            rank3 = Ranking({0:1, 2:3})
-
-    .. important::
-        The numerical value of the ranks do not mean anything.  They are only used to make ordinal comparisons.  For instance, each of the following represents the same ranking:
-        0 is ranked  first, 2 is ranked second, and 1 is ranked in last place.
-
-        .. code-block:: python
-
-            rank1 = Ranking({0:1, 1:3, 2:2})
-            rank2 = Ranking({0:1, 1:10, 2:3})
-            rank3 = Ranking({0:10, 1:100, 2:30})
-
-    """
-
-    def __init__(self, rmap, cmap=None):
-        """constructer method"""
-
-        self.rmap = rmap
-        self.cmap = cmap if cmap is not None else {c: str(c) for c in rmap.keys()}
-
-    @property
-    def ranks(self):
-        """Returns a sorted list of the ranks."""
-        return sorted(set(self.rmap.values()))
-
-    @property
-    def cands(self):
-        """Returns a sorted list of the candidates that are ranked."""
-        return sorted(list(self.rmap.keys()))
-
-    def cands_at_rank(self, r):
-        """Returns a list of the candidates that are assigned the rank ``r``."""
-        return [c for c in self.rmap.keys() if self.rmap[c] == r]
-
-    def is_ranked(self, c):
-        """Returns True if the candidate ``c`` is ranked."""
-
-        return c in self.rmap.keys()
-
-    def strict_pref(self, c1, c2):
-        """Returns True if ``c1`` is strictly preferred to ``c2``.
-
-        The return value is True when both ``c1`` and ``c2`` are ranked and the rank of ``c1`` is strictly smaller than the rank of ``c2``.
-        """
-
-        return (self.is_ranked(c1) and self.is_ranked(c2)) and self.rmap[
-            c1
-        ] < self.rmap[c2]
-
-    def extended_strict_pref(self, c1, c2):
-        """Returns True when either ``c1`` is ranked and ``c2`` is not ranked or the rank of ``c1`` is strictly smaller than the rank of ``c2``."""
-
-        return (self.is_ranked(c1) and not self.is_ranked(c2)) or (
-            (self.is_ranked(c1) and self.is_ranked(c2))
-            and self.rmap[c1] < self.rmap[c2]
-        )
-
-    def indiff(self, c1, c2):
-        """Returns True if ``c1`` and ``c2`` are tied.
-
-        The return value is True when  both ``c1`` and  ``c2`` are  ranked and the rank of ``c1`` equals the rank of ``c2``.
-
-        """
-
-        return (
-            self.is_ranked(c1) and self.is_ranked(c2) and self.rmap[c1] == self.rmap[c2]
-        )
-
-    def extended_indiff(self, c1, c2):
-        """Returns True  when either both ``c1`` and  ``c2`` are not ranked or the rank of ``c1`` equals the rank of ``c2``."""
-
-        return (not self.is_ranked(c1) and not self.is_ranked(c2)) or (
-            self.is_ranked(c1) and self.is_ranked(c2) and self.rmap[c1] == self.rmap[c2]
-        )
-
-    def weak_pref(self, c1, c2):
-        """Returns True if ``c1`` is weakly preferred to ``c2``.
-
-        The return value is True if either ``c1`` is tied with ``c2`` or ``c1`` is strictly preferred to ``c2``.
-        """
-
-        return self.strict_pref(c1, c2) or self.indiff(c1, c2)
-
-    def extended_weak_pref(self, c1, c2):
-        """Returns True when either ``c1`` and ``c2`` are in the relation of extended indifference or ``c1`` is extended strictly preferred to ``c2``."""
-
-        return self.extended_strict_pref(c1, c2) or self.extended_indiff(c1, c2)
-
-    def remove_cand(self, a):
-        """Returns a Ranking with the candidate ``a`` removed."""
-
-        new_rmap = {c: self.rmap[c] for c in self.rmap.keys() if c != a}
-        new_cmap = {c: self.cmap[c] for c in self.cmap.keys() if c != a}
-        return Ranking(new_rmap, cmap=new_cmap)
-
-    def first(self, cs=None):
-        """Returns the list of candidates from ``cs`` that have the highest ranking.   If ``cs`` is None, then use all the ranked candidates."""
-
-        _ranks = list(self.rmap.values()) if cs is None else [self.rmap[c] for c in cs if c in self.rmap.keys()]
-        _cands = list(self.rmap.keys()) if cs is None else cs
-        min_rank = min(_ranks) if len(_ranks) > 0 else None
-        return sorted([c for c in _cands if c in self.rmap.keys() and self.rmap[c] == min_rank])
-
-    def last(self, cs=None):
-        """Returns the list of candidates from ``cs`` that have the worst ranking.   If ``cs`` is None, then use all the ranked candidates."""
-
-        _ranks = list(self.rmap.values()) if cs is None else [self.rmap[c] for c in cs if c in self.rmap.keys()]
-        _cands = list(self.rmap.keys()) if cs is None else cs
-        max_rank = max(_ranks)
-        return sorted([c for c in _cands if c in self.rmap.keys() and self.rmap[c] == max_rank])
-
-    def is_empty(self): 
-        """Return True when the ranking is empty."""
-        return len(self.rmap.keys()) == 0
-        
-    def has_tie(self): 
-        """Return True when the ranking has a tie."""
-        return len(list(set(self.rmap.values()))) != len(list(self.rmap.values()))
-
-    def is_linear(self, num_cands):
-        """Return True when the ranking is a linear order of ``num_cands`` candidates. 
-        """
-
-        return not self.has_tie() and len(self.rmap.keys()) == num_cands
-
-    def is_truncated_linear(self, num_cands): 
-        """Return True when the ranking is a truncated linear order, so it is linear but ranks fewer than ``num_cands`` candidates. 
-        """
-        return  not self.has_tie() and len(self.rmap.keys()) < num_cands
-    
-    def has_skipped_rank(self): 
-        """Returns True when a rank is skipped."""
-        return len(self.ranks) != 0 and len(list(set(self.rmap.values()))) != max(list(self.rmap.values()))
-
-    def has_overvote(self): 
-        """
-        Return True if the voter submitted an overvote (a ranking with a tie). 
-        """
-        return self.has_tie()
-    
-
-    def truncate_overvote(self):
-        """
-        Truncate the ranking at an overvote.  
-        """ 
-        
-        new_rmap = dict()
-
-        for r in self.ranks:
-            cands_at_rank = self.cands_at_rank(r)
-            if len(cands_at_rank) == 1:
-                new_rmap[cands_at_rank[0]] = r
-            elif len(cands_at_rank) > 1: 
-                break
-
-        self.rmap = new_rmap
-
-    def normalize_ranks(self):
-        """Change the ranks so that they start with 1, and the next rank is the next integer after the previous rank.
-
-        :Example:
-
-        .. exec_code:: python
-
-            from pref_voting.profiles_with_ties import Ranking
-            r = Ranking({0:1, 1:3, 2:2})
-            print(r.rmap)
-            r.normalize_ranks()
-            print("After normalizing: ", r.rmap)
-
-            r = Ranking({0:1, 1:10, 2:3})
-            print(r.rmap)
-            r.normalize_ranks()
-            print("After normalizing: ", r.rmap)
-
-            r = Ranking({0:-100, 1:123, 2:0})
-            print(r.rmap)
-            r.normalize_ranks()
-            print("After normalizing: ", r.rmap)
-
-            r = Ranking({0:10, 1:10, 2:100})
-            print(r.rmap)
-            r.normalize_ranks()
-            print("After normalizing: ", r.rmap)
-
-        """
-        self.rmap = {c: self.ranks.index(r) + 1 for c, r in self.rmap.items()}
-
-    ## set preferences
-    def AAdom(self, c1s, c2s, use_extended_preferences=False):
-        """
-        Returns True if every candidate in ``c1s`` is weakly preferred to every candidate in ``c2s``. If ``use_extended_preferences`` is True, then use the extended weak preference.
-        """
-
-        weak_pref = (
-            self.extended_weak_pref if use_extended_preferences else self.weak_pref
-        )
-
-        return all([all([weak_pref(c1, c2) for c2 in c2s]) for c1 in c1s])
-
-    def strong_dom(self, c1s, c2s, use_extended_preferences=False):
-        """
-        Returns True if ``AAdom(c1s, c2s)`` and there is some candidate in ``c1s`` that is strictly preferred to every candidate in ``c2s``. If ``use_extended_preferences`` is True, then use the extended  preferences.
-        """
-
-        strict_pref = (
-            self.extended_strict_pref if use_extended_preferences else self.strict_pref
-        )
-
-        return self.AAdom(
-            c1s, c2s, use_extended_preferences=use_extended_preferences
-        ) and any([all([strict_pref(c1, c2) for c2 in c2s]) for c1 in c1s])
-
-    def weak_dom(self, c1s, c2s, use_extended_preferences=False):
-        """
-        Returns True if ``AAdom(c1s, c2s)`` and there is some candidate in ``c1s`` that is strictly preferred to some candidate in ``c2s``. If ``use_extended_preferences`` is True, then use the extended  preferences.
-        """
-
-        strict_pref = (
-            self.extended_strict_pref if use_extended_preferences else self.strict_pref
-        )
-
-        return self.AAdom(
-            c1s, c2s, use_extended_preferences=use_extended_preferences
-        ) and any([any([strict_pref(c1, c2) for c2 in c2s]) for c1 in c1s])
-
-    def display(self, cmap = None): 
-        """
-        Display the ranking vertically as a column of a table. 
-        
-        :Example:
-
-        .. exec_code:: python
-
-            from pref_voting.profiles_with_ties import Ranking
-            r = Ranking({0:2, 1:1, 2:3})
-            print(r)
-            r.display()
-            print()
-
-            r = Ranking({0:1, 1:1, 2:3})
-            print(r)
-            r.display()
-
-            print()
-            r = Ranking({0:1,  2:3})
-            print(r)
-            r.display()
-
-        """
-        cmap = cmap if cmap is not None else self.cmap
-        _r = copy.deepcopy(self)
-        _r.normalize_ranks()
-        print(
-            tabulate([[" ".join([
-                str(self.cmap[c])
-                for c in _r.cands_at_rank(rank)])] 
-                      for rank in _r.ranks],
-                     tablefmt="pretty")
-        )
-     
-    def __str__(self):
-        """
-        Display the ranking as a string.
-        """
-        r_str = ""
-
-        for r in self.ranks:
-            cands_at_rank = self.cands_at_rank(r)
-            if len(cands_at_rank) == 1:
-                r_str += str(self.cmap[cands_at_rank[0]]) + " "
-            else:
-                r_str += "( " + " ".join(map(lambda c: str(self.cmap[c]) + " ", cands_at_rank)) + ") "
-        return r_str
-
-    def __eq__(self, other): 
-        
-        """
-        Returns True if the rankings are the same.  
-        
-        :Example:
-
-        .. exec_code:: python
-
-            from pref_voting.profiles_with_ties import Ranking
-
-            r = Ranking({1:2, 2:3})            
-            r2 = Ranking({1:1, 2:2})
-            r3 = Ranking({1:1})
-
-            print(r == r2) # True
-            print(r == r3) # False
-        
-        """
-        
-        self_ranks = self.ranks
-        other_ranks = other.ranks
-        
-        if len(self_ranks) != len(other_ranks): 
-            return False
-
-        for self_rank, other_rank in zip(self_ranks, other_ranks): 
-            if set(self.cands_at_rank(self_rank)) != set(other.cands_at_rank(other_rank)): 
-                return False
-        return True
 
 class ProfileWithTies(object):
     """An anonymous profile of (truncated) strict weak orders of :math:`n` candidates. 
 
     :param rankings: List of rankings in the profile, where a ranking is either a :class:`Ranking` object or a dictionary.
     :type rankings: list[dict[int or str: int]] or list[Ranking]
-    :param rcounts: List of the number of voters associated with each ranking.  Should be the same length as rankings.   If not provided, it is assumed that 1 voters submitted each element of ``rankings``.
+    :param rcounts: List of the number of voters associated with each ranking.  Should be the same length as rankings.  If not provided, it is assumed that 1 voters submitted each element of ``rankings``.
     :type rcounts: list[int], optional
-    :param candidates: List of candidates in the profile.  If not provied, this is the list that is ranked by at least on voter.
+    :param candidates: List of candidates in the profile.  If not provided, this is the list that is ranked by at least on voter.
     :type candidates: list[int] or list[str], optional
-    :param cmap: Dictionary mapping candidates (integers) to candidate names (strings).  If not provied, each candidate name is mapped to itself.
+    :param cmap: Dictionary mapping candidates (integers) to candidate names (strings).  If not provided, each candidate name is mapped to itself.
     :type cmap: dict[int: str], optional
 
     :Example:
 
     The following code creates a profile in which
     2 voters submitted the ranking 0 ranked first, 1 ranked second, and 2 ranked third; 3 voters submitted the ranking 1 and 2 are tied for first place and 0 is ranked second; and 1 voter submitted the ranking in which 2 is ranked first and 0 is ranked second:
 
@@ -370,39 +45,50 @@
 
     def __init__(self, rankings, rcounts=None, candidates=None, cmap=None):
         """constructor method"""
 
         assert rcounts is None or len(rankings) == len(
             rcounts
         ), "The number of rankings much be the same as the number of rcounts"
+        
 
+        get_cands = lambda r: list(r.keys()) if type(r) == dict else r.cands
         self.candidates = (
             sorted(candidates)
             if candidates is not None
-            else sorted(list(set([c for r in rankings for c in r.keys()])))
+            else sorted(list(set([c for r in rankings for c in get_cands(r)])))
         )
         """The candidates in the profile. """
 
         self.num_cands = len(self.candidates)
         """The number of candidates in the profile."""
 
-        self.ranks = list(range(1, self.num_cands + 1))
-
         self.cmap = cmap if cmap is not None else {c: c for c in self.candidates}
         """The candidate map is a dictionary associating a candidate with the name used when displaying a candidate."""
-        
+
         self.rankings = [
             Ranking(r, cmap=self.cmap)
             if type(r) == dict
             else Ranking(r.rmap, cmap=self.cmap)
             for r in rankings
         ]
         """The list of rankings in the Profile (each ranking is a :class:`Ranking` object). 
         """
 
+        self.ranks = list(range(1, self.num_cands + 1))
+        """The ranks that are possible in the profile. """
+
+        self.cindices = list(range(self.num_cands))
+        self._cand_to_cindex = {c: i for i, c in enumerate(self.candidates)}
+        self.cand_to_cindex = lambda c: self._cand_to_cindex[c]
+        self._cindex_to_cand = {i: c for i, c in enumerate(self.candidates)}
+        self.cindex_to_cand = lambda i: self._cindex_to_cand[i]
+        """Maps candidates to their index in the list of candidates and vice versa. """
+
+    
         self.rcounts = [1] * len(rankings) if rcounts is None else list(rcounts)
 
         self.num_voters = np.sum(self.rcounts)
         """The number of voters in the profile. """
 
         self.using_extended_strict_preference = False
         """A flag indicating whether the profile is using extended strict preferences when calculating supports, margins, etc."""
@@ -466,18 +152,26 @@
 
     def support(self, c1, c2, use_extended_preferences=False):
         """Returns the support of candidate ``c1`` over candidate ``c2``, where the support is the number of voters that rank ``c1`` strictly above ``c2``."""
 
         return self._supports[c1][c2]
 
     def margin(self, c1, c2):
-        """Returns the margin of candidate ``c1`` over candidate ``c2``, where the maring is the number of voters that rank ``c1`` strictly above ``c2`` minus the number of voters that rank ``c2`` strictly above ``c1``."""
+        """Returns the margin of candidate ``c1`` over candidate ``c2``, where the margin is the number of voters that rank ``c1`` strictly above ``c2`` minus the number of voters that rank ``c2`` strictly above ``c1``."""
 
         return self._supports[c1][c2] - self._supports[c2][c1]
 
+    @property
+    def margin_matrix(self):
+        """Returns the margin matrix of the profile, where the entry at row ``i`` and column ``j`` is the margin of candidate ``i`` over candidate ``j``."""
+
+        return np.array(
+            [[self.margin(self.cindex_to_cand(c1_idx), self.cindex_to_cand(c2_idx)) for c2_idx in self.cindices] for c1_idx in self.cindices]
+        )
+    
     def is_tied(self, c1, c2): 
         """Returns True if ``c1`` and ``c2`` are tied (i.e., the margin of ``c1`` over ``c2`` is 0)."""
 
         return self.margin(c1, c2) == 0
 
     def dominators(self, cand, curr_cands=None):
         """Returns the list of candidates that are majority preferred to ``cand`` in the profile restricted to the candidates in ``curr_cands``."""
@@ -684,14 +378,24 @@
                     found_it = True
             if not found_it: 
                 ranks.append(new_ranking)
                 rcounts.append(1)
 
         return ProfileWithTies([r.rmap for r in ranks], rcounts=rcounts, cmap=self.cmap)
 
+    def to_linear_profile(self):
+        """Return a linear profile from the profile with ties. """
+        
+        rankings, rcounts = self.rankings_counts
+        new_rankings = [r.to_linear() for r in rankings]
+        if any([r is None or len(r) != len(self.candidates) for r in new_rankings]): 
+            print("Error: Cannot convert to linear profile.")
+            return None
+        return Profile(new_rankings, rcounts=rcounts, cmap=self.cmap)
+
     def unique_rankings(self): 
         """Return to the list of unique rankings in the profile. 
         """
         
         return (list(set([str(r) for r in self.rankings])))
                 
     def margin_graph(self):
@@ -702,15 +406,15 @@
         .. exec_code:: python
 
                 from pref_voting.profiles_with_ties import ProfileWithTies
                 prof = ProfileWithTies([{0: 1, 1: 2, 2: 3}, {1:1, 2:1, 0:2}, {2:1, 0:2}], [2, 3, 1])
 
                 mg = prof.margin_graph()
                 print(mg.edges)
-                print(mg.m_matrix)
+                print(mg.margin_matrix)
         """
 
         return MarginGraph.from_profile(self)
 
     def support_graph(self):
         """Returns the support graph of the profile.  See :class:`.SupportGraph`.
```

### Comparing `pref_voting-0.2.9/pref_voting/scoring_methods.py` & `pref_voting-0.3/pref_voting/scoring_methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 '''
     File: scoring_rules.py
     Author: Eric Pacuit (epacuit@umd.edu)
     Date: January 6, 2022
     
-    Implemenation of scoring rules. 
+    Implementations of scoring rules. 
 '''
 from pref_voting.voting_method import  *
 from pref_voting.voting_method import _num_rank_last 
 from pref_voting.profiles import _find_updated_profile, _num_rank
 
 @vm(name = "Plurality")
 def plurality(profile, curr_cands = None):
```

### Comparing `pref_voting-0.2.9/pref_voting/voting_method.py` & `pref_voting-0.3/pref_voting/voting_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 '''
     File: voting_methods.py
     Author: Eric Pacuit (epacuit@umd.edu)
     Date: November 6, 2021
     Update: January 15, 2023
     
-    The VotingMethod class and helper functions for voting methdods
+    The VotingMethod class and helper functions for voting methods
 '''
 
 import functools
 import numpy as np
-# from numba import jit # Remove until numba supports python3.11
+# from numba import jit # Remove until numba supports python 3.11
 import random
 
 class VotingMethod(object): 
     """
     A class to add functionality to voting methods. 
 
     Args:
@@ -52,15 +52,15 @@
         Display the winning set of candidates.
         """
  
         cmap = cmap if cmap is not None else edata.cmap
 
         ws = self.__call__(edata, curr_cands = curr_cands, **kwargs)
 
-        if ws is None:  # some voting methods, such as Ranked Pairs, may return None if it is taking long to compute the winner.
+        if ws is None:  # some voting methods, such as ``ranked_pairs_with_test``, may return None if it is taking long to compute the winner.
             print(f"{self.name} winning set is not available")
         else: 
             w_str = f"{self.name} winner is " if len(ws) == 1 else f"{self.name} winners are "
             print(w_str + "{" + ", ".join([str(cmap[c]) for c in ws]) + "}")
         
     def set_name(self, new_name):
         """Set the name of the voting method."""
```

### Comparing `pref_voting-0.2.9/pref_voting/weighted_majority_graphs.py` & `pref_voting-0.3/pref_voting/weighted_majority_graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -41,31 +41,39 @@
         mg = nx.DiGraph()
         mg.add_nodes_from(candidates)
         mg.add_edges_from(edges)
         self.mg = mg
         """A networkx DiGraph object representing the majority graph."""
 
         self.cmap = cmap if cmap is not None else {c: str(c) for c in candidates}
-        self.cindx = {c: cidx for cidx, c in enumerate(candidates)}
+        
         self.candidates = list(candidates)
         """The list of candidates."""
+        
+        self.num_cands = len(self.candidates)
+        """The number of candidates."""
 
-        self.cindices = range(len(candidates))
+        self.cindices = list(range(self.num_cands))
+        self._cand_to_cindex = {c: i for i, c in enumerate(self.candidates)}
+        self.cand_to_cindex = lambda c: self._cand_to_cindex[c]
+        self._cindex_to_cand = {i: c for i, c in enumerate(self.candidates)}
+        self.cindex_to_cand = lambda i: self._cindex_to_cand[i]
+        """A dictionary mapping each candidate to its index in the list of candidates and vice versa."""
 
         self.maj_matrix = [[False for c2 in self.cindices] for c1 in self.cindices]
         """A matrix of Boolean values representing the majority graph."""
 
-        for c1 in self.cindices:
-            for c2 in self.cindices:
-                if mg.has_edge(c1, c2):
-                    self.maj_matrix[c1][c2] = True
-                    self.maj_matrix[c2][c1] = False
-                elif mg.has_edge(c2, c1):
-                    self.maj_matrix[c2][c1] = True
-                    self.maj_matrix[c1][c2] = False
+        for c1_idx in self.cindices:
+            for c2_idx in self.cindices:
+                if mg.has_edge(self.cindex_to_cand(c1_idx), self.cindex_to_cand(c2_idx)):
+                    self.maj_matrix[c1_idx][c2_idx] = True
+                    self.maj_matrix[c2_idx][c1_idx] = False
+                elif mg.has_edge(self.cindex_to_cand(c2_idx), self.cindex_to_cand(c1_idx)):
+                    self.maj_matrix[c2_idx][c1_idx] = True
+                    self.maj_matrix[c1_idx][c2_idx] = False
 
     def margin(self, c1, c2):
         raise NotImplemented
 
     def support(self, c1, c2):
         raise NotImplemented
 
@@ -453,24 +461,24 @@
     """
 
     def __init__(self, candidates, w_edges, cmap=None):
         """constructor method"""
 
         super().__init__(candidates, [(e[0], e[1]) for e in w_edges], cmap=cmap)
 
-        self.m_matrix = [[0 for c2 in self.cindices] for c1 in self.cindices]
+        self.margin_matrix = [[0 for c2 in self.cindices] for c1 in self.cindices]
         """The margin matrix, where the :math:`(i, j)`-entry is the number of voters who rank candidate with index :math:`i` above the candidate with index :math:`j` minus the number of voters  who rank candidate with index :math:`j` above the candidate with index :math:`i`. """
 
         for c1, c2, margin in w_edges:
-            self.m_matrix[self.cindx[c1]][self.cindx[c2]] = margin
-            self.m_matrix[self.cindx[c2]][self.cindx[c1]] = -1 * margin
+            self.margin_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)] = margin
+            self.margin_matrix[self.cand_to_cindex(c2)][self.cand_to_cindex(c1)] = -1 * margin
 
     def margin(self, c1, c2):
         """Returns the margin of ``c1`` over ``c2``."""
-        return self.m_matrix[self.cindx[c1]][self.cindx[c2]]
+        return self.margin_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)]
 
     @property
     def edges(self):
         """Returns a list of the weighted edges in the margin graph."""
 
         return [(c1, c2, self.margin(c1, c2)) for c1, c2 in self.mg.edges]
 
@@ -500,19 +508,19 @@
 
         new_cmap = {c: cname for c, cname in self.cmap.items() if c in new_cands}
 
         return MarginGraph(new_cands, new_edges, cmap=new_cmap)
 
     def majority_prefers(self, c1, c2):
         """Returns True if the margin of ``c1`` over ``c2`` is positive."""
-        return self.m_matrix[self.cindx[c1]][self.cindx[c2]] > 0
+        return self.margin_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)] > 0
 
     def is_tied(self, c1, c2):
         """Returns True if the margin ``c1`` over ``c2`` is zero."""
-        return self.m_matrix[self.cindx[c1]][self.cindx[c2]] == 0
+        return self.margin_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)] == 0
 
     def is_uniquely_weighted(self):
         """Returns True if all the margins between distinct candidates are unique and there is no 0 margin between distinct candidates."""
         has_zero_margins = any(
             [
                 self.margin(c1, c2) == 0
                 for c1 in self.candidates
@@ -837,20 +845,20 @@
         .. exec_code::
 
             from pref_voting.profiles import Profile
             from pref_voting.weighted_majority_graphs import MarginGraph
             prof = Profile([[0,1,2], [1,2,0], [2,0,1]], [2, 1, 2])
             mg = MarginGraph.from_profile(prof)
             print(mg.edges)
-            print(mg.m_matrix)
+            print(mg.margin_matrix)
 
             # it is better to use the Profile method
             mg = prof.margin_graph()
             print(mg.edges)
-            print(mg.m_matrix)
+            print(mg.margin_matrix)
 
         """
 
         cmap = profile.cmap if cmap is None else cmap
         return cls(
             profile.candidates,
             [
@@ -901,53 +909,53 @@
             cmap=cmap,
         )
 
         self.s_matrix = [[0 for c2 in self.cindices] for c1 in self.cindices]
         """The support matrix, where the   :math:`(i, j)`-entry is the number of voters who rank candidate with index :math:`i` above the candidate with index :math:`j`. """
 
         for c1, c2, support in w_edges:
-            self.s_matrix[self.cindx[c1]][self.cindx[c2]] = support[0]
-            self.s_matrix[self.cindx[c2]][self.cindx[c1]] = support[1]
+            self.s_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)] = support[0]
+            self.s_matrix[self.cand_to_cindex(c2)][self.cand_to_cindex(c1)] = support[1]
 
     @property
     def edges(self):
         """Returns a list of the weighted edges in the margin graph."""
 
         return [
             (c1, c2, (self.support(c1, c2), self.support(c2, c1)))
             for c1, c2 in self.mg.edges
         ]
 
     def margin(self, c1, c2):
         """Returns the margin of ``c1`` over ``c2``."""
 
         return (
-            self.s_matrix[self.cindx[c1]][self.cindx[c2]]
-            - self.s_matrix[self.cindx[c2]][self.cindx[c1]]
+            self.s_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)]
+            - self.s_matrix[self.cand_to_cindex(c2)][self.cand_to_cindex(c1)]
         )
 
     def support(self, c1, c2):
         """Returns the support of ``c1`` over ``c2``."""
 
-        return self.s_matrix[self.cindx[c1]][self.cindx[c2]]
+        return self.s_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)]
 
     def majority_prefers(self, c1, c2):
         """Returns True if ``c1`` is majority preferred to ``c2``."""
 
         return (
-            self.s_matrix[self.cindx[c1]][self.cindx[c2]]
-            > self.s_matrix[self.cindx[c2]][self.cindx[c1]]
+            self.s_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)]
+            > self.s_matrix[self.cand_to_cindex(c2)][self.cand_to_cindex(c1)]
         )
 
     def is_tied(self, c1, c2):
         """Returns True if ``c1`` is tied with  ``c2``."""
 
         return (
-            self.s_matrix[self.cindx[c1]][self.cindx[c2]]
-            == self.s_matrix[self.cindx[c2]][self.cindx[c1]]
+            self.s_matrix[self.cand_to_cindex(c1)][self.cand_to_cindex(c2)]
+            == self.s_matrix[self.cand_to_cindex(c2)][self.cand_to_cindex(c1)]
         )
 
     def remove_candidates(self, cands_to_ignore):
         """Remove all candidates from ``cands_to_ignore`` from the Majority Graph.
 
         :param cands_to_ignore: list of candidates to remove from the profile
         :type cands_to_ignore: list[int]
```

### Comparing `pref_voting-0.2.9/pyproject.toml` & `pref_voting-0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,16 +3,16 @@
     "setuptools>=42",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 name = "pref_voting"
-version = "0.2.9"
-description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods."
+version = "0.3"
+description = "pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods."
 authors = ["Eric Pacuit <epacuit@umd.edu>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/voting-tools/pref_voting"
 repository = "https://github.com/voting-tools/pref_voting"
 
 [tool.poetry.dependencies]
```

### Comparing `pref_voting-0.2.9/setup.py` & `pref_voting-0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,17 @@
  'networkx>=3.0,<4.0',
  'random2>=1.0.1,<2.0.0',
  'scipy>=1.0.0,<2.0.0',
  'tabulate>=0.9.0,<0.10.0']
 
 setup_kwargs = {
     'name': 'pref-voting',
-    'version': '0.2.9',
-    'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.',
-    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.9 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
+    'version': '0.3',
+    'description': 'pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.',
+    'long_description': 'pref_voting\n==========\n\n## Installation\n\nWith pip package manager:\n\n```bash\npip install pref_voting\n```\n## Documentation\n\nOnline documentation is available at [https://pref_voting.readthedocs.io](https://pref_voting.readthedocs.io).\n\n## Profiles and Voting Methods\n\nA profile (of linear orders over the candidates) is created by initializing a Profile class object.  This needs a list of rankings (each ranking is a tuple of numbers), the number of candidates, and a list giving the number of each ranking in the profile:\n\n```python\nfrom pref_voting.profiles import Profile\n\nrankings = [(0, 1, 2, 3), (2, 3, 1, 0), (3, 1, 2, 0), (1, 2, 0, 3), (1, 3, 2, 0)]\nrcounts = [5, 3, 2, 4, 3]\n\nprof = Profile(rankings, rcounts=rcounts)\n```\n\nThe function generate_profile is used to generate a profile for a given number of candidates and voters:  \n```python\nfrom pref_voting.generate_profiles import generate_profile\n\n# generate a profile using the Impartial Culture probability model\nprof = generate_profile(3, 4) # prof is a Profile object\n\n# generate a profile using the Impartial Anonymous Culture probability model\nprof = generate_profile(3, 4, probmod = "IAC") # prof is a Profile object \n```\n\n```python\nfrom pref_voting.profiles import Profile\nfrom pref_voting.voting_methods import *\n\nprof = Profile(rankings, num_cands, rcounts=rcounts)\nprint(f"{split_cycle.name} winners:  {split_cycle(prof)}")\nsplit_cycle.display(prof)\n\n```\n\n## Versions\n\n- v0.1.10 (2022-08-09): **Initial release** \n- v0.1.13 (2022-11-05): Minor updates and bug fixes \n- v0.1.14 (2022-12-19): Add plurality_scores to ProfileWithTies; add generate ceots function; bug fixes \n- v0.1.23 (2022-12-27): Add instant_runoff_for_truncated_linear_orders and functions to truncate overvotes in a ProfileWithTies, add smith_irv_put, document analysis functions\n- v0.1.25 (2023-1-11): Add condorcet_irv, condorcet_irv_put; Update documentation; add axioms.py; add display and equality to Ranking class; fix enumerate ceots functions\n- v0.1.27 (2023-2-07): Add Borda for ProfileWithTies\n- v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies\n- v0.2.1 (2023-2-15): Bug fixes\n- v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation\n- v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.\n- v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.\n- v0.2.8 (2023-5-16): Add description function to Majority Graphs.\n- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.\n- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.\n- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies\n- v0.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.\n\n## Questions?\n\nFeel free to [send me an email](https://pacuit.org/) if you have questions about the project.\n\n## License\n\n[MIT](https://github.com/jontingvold/pyrankvote/blob/master/LICENSE.txt)\n',
     'author': 'Eric Pacuit',
     'author_email': 'epacuit@umd.edu',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/voting-tools/pref_voting',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pref_voting-0.2.9/PKG-INFO` & `pref_voting-0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pref-voting
-Version: 0.2.9
-Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of a variety of preferential voting methods.
+Version: 0.3
+Summary: pref_voting is a Python packaging that contains tools to reason about election profiles and margin graphs, and implementations of voting methods.
 Home-page: https://github.com/voting-tools/pref_voting
 License: MIT
 Author: Eric Pacuit
 Author-email: epacuit@umd.edu
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -81,15 +81,18 @@
 - v0.1.27 (2023-2-07): Add Borda for ProfileWithTies
 - v0.2 (2023-2-15): Add Benham, add anonymize to Profile method, comment out numba to make compatible with Python 3.11, add add_unranked_candidates to ProfileWithTies
 - v0.2.1 (2023-2-15): Bug fixes
 - v0.2.3 (2023-4-2): Add plurality_with_runoff_with_explanation
 - v0.2.4 (2023-4-9): Update generate_truncated_profile so that it implements the IC probability model.
 - v0.2.6 (2023-5-10): Add axiom class, dominance axioms, and axiom_violations_data.
 - v0.2.8 (2023-5-16): Add description function to Majority Graphs.
-- v0.2.9 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
+- v0.2.11 (2023-5-16): Update implementation of Simple Stable Voting and Stable Voting.
+- v0.2.13 (2023-5-24): Improve implementation of split_cycle; Breaking changes: split_cycle_faster renamed split_cycle_Floyd_Warshall and beat_path_faster renamed beat_path_Floyd_Warshall.
+- v0.2.17 (2023-5-25): Add to_linear_profile to ProfileWithTies
+- v0.3 (2023-5-26): Add implementations of UtilityProfile and a number of different utility methods.
 
 ## Questions?
 
 Feel free to [send me an email](https://pacuit.org/) if you have questions about the project.
 
 ## License
```

