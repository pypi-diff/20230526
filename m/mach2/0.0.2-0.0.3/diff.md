# Comparing `tmp/mach2-0.0.2.tar.gz` & `tmp/mach2-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mach2-0.0.2.tar", last modified: Sun May 21 09:38:38 2023, max compression
+gzip compressed data, was "mach2-0.0.3.tar", last modified: Fri May 26 03:02:51 2023, max compression
```

## Comparing `mach2-0.0.2.tar` & `mach2-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1581 2023-05-17 16:26:02.847064 mach2-0.0.2/LICENSE
--rw-r--r--   0        0        0     5012 2023-05-21 09:29:39.765450 mach2-0.0.2/README.md
--rw-r--r--   0        0        0      984 2023-05-21 09:38:38.315606 mach2-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       56 2023-05-15 12:06:57.622467 mach2-0.0.2/src/mach2/__init__.py
--rw-r--r--   0        0        0    13877 2023-05-15 22:46:48.571251 mach2-0.0.2/src/mach2/clonetree.py
--rw-r--r--   0        0        0    22493 2023-05-21 09:25:29.295937 mach2-0.0.2/src/mach2/mach.py
--rw-r--r--   0        0        0     3043 2023-05-15 22:25:01.101453 mach2-0.0.2/src/mach2/migrationgraph.py
--rw-r--r--   0        0        0     5131 2023-05-15 22:27:26.185860 mach2-0.0.2/src/mach2/solutionset.py
--rw-r--r--   0        0        0      296 2023-05-14 21:09:58.179420 mach2-0.0.2/src/mach2/utils.py
--rw-r--r--   0        0        0     7644 1970-01-01 00:00:00.000000 mach2-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1581 2023-05-17 16:26:02.847064 mach2-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5151 2023-05-26 01:55:52.377441 mach2-0.0.3/README.md
+-rw-r--r--   0        0        0      973 2023-05-26 03:02:51.995214 mach2-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       56 2023-05-24 15:15:54.897927 mach2-0.0.3/src/mach2/__init__.py
+-rw-r--r--   0        0        0    22478 2023-05-26 02:33:31.184198 mach2-0.0.3/src/mach2/mach.py
+-rw-r--r--   0        0        0     3217 2023-05-24 16:53:04.947933 mach2-0.0.3/src/mach2/migrationgraph.py
+-rw-r--r--   0        0        0    20120 2023-05-25 22:15:41.871331 mach2-0.0.3/src/mach2/phylogeny.py
+-rw-r--r--   0        0        0     5188 2023-05-24 16:53:04.947933 mach2-0.0.3/src/mach2/solutionset.py
+-rw-r--r--   0        0        0      304 2023-05-24 16:53:04.947933 mach2-0.0.3/src/mach2/utils.py
+-rw-r--r--   0        0        0     7764 1970-01-01 00:00:00.000000 mach2-0.0.3/PKG-INFO
```

### Comparing `mach2-0.0.2/LICENSE` & `mach2-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mach2-0.0.2/README.md` & `mach2-0.0.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # MACH2
 
 A mathematical framework for inferring migration histories of metastatic cancer from clone phylogeny and the location of extant clones.
 
 ## Table of contents
 
-1. Installation
-        - Prerequisite
-        - Install using `pip`
-2. Usage instruction
-        - I/O formats
-        - Input
-        - Output
-        - Usage
+1. [Installation](#installation)  
+        - [Prerequisite](#prerequisite)  
+        - [Install using `pip`](#install-using-pip)
+2. [Usage instruction](#usage-instruction)  
+        - [I/O formats](#i-o-formats)  
+        - [Input](#input)  
+        - [Output](#output)  
+        - [Usage](#usage)  
 
 ## 1. Installation
 
 ### Prerequisites
 
 - **Python** - `MACH2` requires Python 3.7 or newer.
 - **ILP solver** - `MACH2` requires an ILP solver installed to solve **PMH-TR**. Currently `MACH2` only supports `Gurobi optimizer`, but we are going to add support for more ILP solvers in the future. `MACH2` requires a valid Gurobi installation and license key. The location of Gurobi should be present in `LD_LIBRARY_PATH` (linux) and `DYLD_LIBRARY_PATH` (macOS) the license key should be saved in the environment variable `GRB_LICENSE_KEY`.
```

### Comparing `mach2-0.0.2/pyproject.toml` & `mach2-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "mach2"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "Mrinmoy Saha Roddur", email = "mroddur2@illinois.edu" },
 ]
 description = "Migration Analysis of Clonal History 2"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -22,19 +22,18 @@
     "Computational biology",
     "Bioinformatics",
     "Cancer",
     "Metastasis",
     "Phylogeny",
 ]
 dependencies = [
-    "numpy",
     "pandas",
     "pyomo",
     "networkx",
-    "gurobi",
+    "gurobipy",
 ]
 
 [project.license]
 file = "LICENSE"
 
 [project.optional-dependencies]
 jupyter = [
```

### Comparing `mach2-0.0.2/src/mach2/mach.py` & `mach2-0.0.3/src/mach2/mach.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 import pyomo.environ as pyo
 from pyomo.opt import SolverFactory
 import networkx as nx
 import os
 import argparse
 import time
 from collections import defaultdict
-from .clonetree import CloneTree, RefinedCloneTree
+from .phylogeny import Phylogeny, RefinedPhylogeny
 from .migrationgraph import MigrationGraph
 from .solutionset import SolutionSet
 from . import utils
 
 
 class MACH:
 
-    def __init__(self, clone_tree, primary_site = None, suboptimal_mode=False, seeding_site=False, specify_migration_comigration=None, possible_migration_list=None):
+    def __init__(self, phylogeny, primary_site = None, suboptimal_mode=False, seeding_site=False, specify_migration_comigration=None, possible_migration_list=None):
         if specify_migration_comigration is not None:
             suboptimal_mode = True
-        self.clone_tree = clone_tree
-        self.E = self.clone_tree.edges
-        self.V = [(i, 'node') for i in self.clone_tree.nodes]
-        self.L = [(i, 'node') for i in self.clone_tree.leaves]
-        self.Sigma = self.clone_tree.sites
+        self.phylogeny = phylogeny
+        self.E = self.phylogeny.edges
+        self.V = [(i, 'node') for i in self.phylogeny.nodes]
+        self.L = [(i, 'node') for i in self.phylogeny.leaves]
+        self.Sigma = self.phylogeny.locations
         self.suboptimal_mode = suboptimal_mode
         self.seeding_site = seeding_site
         self.specific_mig_comig = specify_migration_comigration
 
         self.m = pyo.ConcreteModel()
 
         self._add_vars()
         if suboptimal_mode:
             self._add_extra_vars_suboptimal()
         if seeding_site:
-            self._add_extra_vars_seeding_sites()
+            self._add_extra_vars_seeding_locations()
 
         if not seeding_site:
             self._add_optimization_function()
         else:
-            self._add_optimization_function_seeding_sites()
+            self._add_optimization_function_seeding_locations()
 
         self._add_leaf_constraints()
         self._add_root_constraints()
         self._add_constraints_for_p()
         self.add_polytomy_resolution_compatibility_constraints()
         self._add_original_edges_compatibility_constraints()
-        clone_tree.infer_paths()
         if suboptimal_mode:
             self.add_constraints_for_z_b_R_suboptimal()
             if seeding_site:
                 self.add_constraints_for_q_suboptimal()
         else:
             self.add_constraints_for_z()
             if seeding_site:
@@ -70,33 +69,33 @@
         self.m.r = pyo.Var(self.Sigma, domain=pyo.Binary)
         self.m.p = pyo.Var(self.Sigma, self.Sigma, self.E, domain=pyo.Binary)
 
     def _add_extra_vars_suboptimal(self):
         self.m.R = pyo.Var(self.Sigma, self.Sigma, self.L, domain=pyo.Binary)
         self.m.b = pyo.Var(self.Sigma, self.Sigma, self.L, domain=pyo.Binary)
 
-    def _add_extra_vars_seeding_sites(self):
+    def _add_extra_vars_seeding_locations(self):
         self.m.q = pyo.Var(self.Sigma, domain=pyo.Binary)
 
     def _add_optimization_function(self):
         self.m.obj = pyo.Objective(expr=sum(self.m.g[s, t, k] for s in self.Sigma for t in self.Sigma for k in self.E + self.V if s != t) +
                                    sum(self.m.z[s, t] for s in self.Sigma for t in self.Sigma if s != t))
 
-    def _add_optimization_function_seeding_sites(self):
+    def _add_optimization_function_seeding_locations(self):
         self.m.obj = pyo.Objective(expr=sum(self.m.g[s, t] for s in self.Sigma for t in self.Sigma if s != t) +
                                    sum(self.m.z[s, t] for s in self.Sigma for t in self.Sigma if s != t) +
                                    sum(self.m.q[s] for s in self.Sigma))
 
     def _add_leaf_constraints(self):
         self.m.leaf_constraints = pyo.ConstraintList()
         for i in self.L:
             self.m.leaf_constraints.add(
-                self.m.l[i, self.clone_tree.get_label(i[0])] == 1)
+                self.m.l[i, self.phylogeny.get_label(i[0])] == 1)
             self.m.leaf_constraints.add(sum(
-                self.m.l[i, s] for s in self.Sigma if s != self.clone_tree.get_label(i[0])) == 0)
+                self.m.l[i, s] for s in self.Sigma if s != self.phylogeny.get_label(i[0])) == 0)
             
     def _add_root_constraints(self):
         self.m.root_constraints = pyo.ConstraintList()
         self.m.root_constraints.add(sum(self.m.r[s] for s in self.Sigma) == 1)
 
     def _add_constraints_for_p(self):
         self.m.p_constraints = pyo.ConstraintList()
@@ -132,36 +131,36 @@
                     else:
                         self.m.polytomy_constraints_set_l.add(
                             self.m.g[s, t, i] == 0)
 
         for i in self.V:
             for s in self.Sigma:
                 sum1 = sum(self.m.g[t, s, i] for t in self.Sigma)
-                if i[0] != self.clone_tree.root:
-                    pii = self.clone_tree.get_parent_arc(i[0])
+                if i[0] != self.phylogeny.root:
+                    pii = self.phylogeny.get_parent_arc(i[0])
                     sum1 += sum(self.m.g[t, s, pii] for t in self.Sigma)
                 else:
                     sum1 += self.m.r[s]
                 self.m.polytomy_constraints_set_l.add(sum1 == self.m.l[i, s])
 
         for i in self.V:
-            delta_i = self.clone_tree.get_children_arcs(i[0])
+            delta_i = self.phylogeny.get_children_arcs(i[0])
             for s in self.Sigma:
                 for t in self.Sigma:
                     if s != t:
                         self.m.polytomy_constraints_set_l.add(self.m.g[s, t, i] <= sum(self.m.p[s, t, ij] for ij in delta_i))
 
         for i in self.V:
-            if i[0] != self.clone_tree.root:
-                pii = self.clone_tree.get_parent_arc(i[0])
-            delta_i = self.clone_tree.get_children_arcs(i[0])
+            if i[0] != self.phylogeny.root:
+                pii = self.phylogeny.get_parent_arc(i[0])
+            delta_i = self.phylogeny.get_children_arcs(i[0])
             for ij in delta_i:
                 for s in self.Sigma:
                     sum1 = 0
-                    if i[0] != self.clone_tree.root:
+                    if i[0] != self.phylogeny.root:
                         sum1 = sum(self.m.g[t,s,pii] for t in self.Sigma)
                     else:
                         sum1 = self.m.r[s]
                     sum2 = sum(self.m.p[s,t,ij]+self.m.g[s,t,ij] for t in self.Sigma)
                     self.m.polytomy_constraints_set_l.add(sum1 <= sum2)
 
         # self.m.polytomy_constraints_valid_structure = pyo.ConstraintList()
@@ -174,20 +173,20 @@
         # for s in self.Sigma:
         #     for ij in self.E:
         #         self.m.polytomy_constraints_valid_structure.add(
         #             sum(self.m.g[s, t, ij] + self.m.p[s, t, ij] for t in self.Sigma) <= 1)
 
         # for i in self.V:
         #     for s in self.Sigma:
-        #         if i[0] != self.clone_tree.root:
-        #             pii = self.clone_tree.get_parent_arc(i[0])
-        #         delta_i = self.clone_tree.get_children_arcs(i[0])
+        #         if i[0] != self.phylogeny.root:
+        #             pii = self.phylogeny.get_parent_arc(i[0])
+        #         delta_i = self.phylogeny.get_children_arcs(i[0])
         #         sum1 = 0
         #         for t in self.Sigma:
-        #             if i[0] != self.clone_tree.root:
+        #             if i[0] != self.phylogeny.root:
         #                 sum1 += self.m.g[t, s, pii]
         #             for ij in delta_i:
         #                 sum1 += self.m.g[s, t, ij]
         #         self.m.polytomy_constraints_valid_structure.add(
         #             sum1 >= self.m.l[i, s])
 
         for i in self.V:
@@ -195,15 +194,15 @@
                 sum1 = 0
                 sum2 = 0
                 for t in self.Sigma:
                     if s != t:
                         sum1 += self.m.g[s, t, i] + self.m.g[t, s, i]
                         sum2 += self.m.l[i, t]
                 self.m.polytomy_constraints_set_l.add(
-                    self.clone_tree.n_sites * sum1 >= sum2 + self.clone_tree.n_sites * self.m.l[i, s] - self.clone_tree.n_sites)
+                    self.phylogeny.n_locations * sum1 >= sum2 + self.phylogeny.n_locations * self.m.l[i, s] - self.phylogeny.n_locations)
 
     def _add_original_edges_compatibility_constraints(self):
         self.m.orig_edge = pyo.ConstraintList()
         for s in self.Sigma:
             for t in self.Sigma:
                 for (i, j) in self.E:
                     self.m.orig_edge.add(
@@ -221,38 +220,38 @@
     def add_constraints_for_z(self):
         self.m.constraints_z = pyo.ConstraintList()
         for s in self.Sigma:
             for t in self.Sigma:
                 if s != t:
                     for k in self.L:
                         sum1 = 0
-                        path_k = self.clone_tree.paths[k[0]]
+                        path_k = self.phylogeny.paths[k[0]]
                         for uv in path_k:
                             sum1 += self.m.g[s, t, uv]
                             sum1 += self.m.p[s, t, uv]
                         self.m.constraints_z.add(self.m.z[s, t] >= sum1)
                 else:
                     self.m.constraints_z.add(self.m.z[s, t] == 0)
 
     def add_constraints_for_z_b_R_suboptimal(self):
         self.m.constraints_zbr = pyo.ConstraintList()
         for s in self.Sigma:
             for t in self.Sigma:
                 if s != t:
                     sum3 = 0
                     for k in self.L:
-                        path_k = self.clone_tree.paths[k[0]]
+                        path_k = self.phylogeny.paths[k[0]]
                         sum1 = sum((self.m.g[s, t, uv] + self.m.p[s, t, uv]) for uv in path_k)
                         self.m.constraints_zbr.add(self.m.z[s, t] >= sum1)
                         self.m.constraints_zbr.add(
-                            self.m.z[s, t] <= sum1 + self.clone_tree.max_height * (1 - self.m.b[s, t, k]))
+                            self.m.z[s, t] <= sum1 + self.phylogeny.max_height * (1 - self.m.b[s, t, k]))
                         self.m.constraints_zbr.add(
                             self.m.z[s, t] - sum1 >= 1 - self.m.R[s, t, k])
                         self.m.constraints_zbr.add(
-                            self.m.z[s, t] - sum1 <= self.clone_tree.max_height * (1 - self.m.R[s, t, k]))
+                            self.m.z[s, t] - sum1 <= self.phylogeny.max_height * (1 - self.m.R[s, t, k]))
                         self.m.constraints_zbr.add(
                             self.m.b[s, t, k] >= self.m.R[s, t, k] - sum3)
                         sum3 += self.m.R[s, t, k]
                     sum2 = sum(self.m.b[s, t, k] for k in self.L)
                     self.m.constraints_zbr.add(sum2 == 1)
                 else:
                     self.m.constraints_zbr.add(self.m.z[s, t] == 0)
@@ -281,15 +280,15 @@
                         self.m.addConstr(self.m.q[s] >= self.m.g[s, t, i])
                         sum1 += self.m.g[s, t, i]
             self.m.constraints_s_suboptimal.add(self.q[s] <= sum1)
 
     def add_constraints_binary(self):
         self.m.constraints_binary = pyo.ConstraintList()
         for i in self.V:
-            delta_i = self.clone_tree.get_children_arcs(i[0])
+            delta_i = self.phylogeny.get_children_arcs(i[0])
             if len(delta_i) <= 2:
                 sum1 = 0
                 for s in self.Sigma:
                     sum1 += self.m.l[i, s]
                 self.m.constraints_binary.add(sum1 == 1)
             else:
                 for s in self.Sigma:
@@ -323,15 +322,15 @@
         best_obj_val = opt._solver_model.PoolObjVal
         for e in range(opt._solver_model.SolCount):
             opt._solver_model.params.SolutionNumber = e
             if opt._solver_model.PoolObjVal - best_obj_val > 0.5:
                 return e
         return opt._solver_model.SolCount
 
-    def solve(self, solver, nSolutions, logfile=None, n_threads=1, raw=False):
+    def solve(self, solver, nSolutions, logfile="", n_threads=0, raw=False):
         if solver == 'gurobi':
             opt = SolverFactory("gurobi", solver_io='python', options={ 'MIPGap': 0, 'PoolSolutions': nSolutions, 'PoolSearchMode': 2, 'threads': n_threads, 'LogToConsole': 0, 'LogFile': logfile})
             opt.solve(self.m, load_solutions=True, tee=True)
             if self.suboptimal_mode and self.specific_mig_comig is None:
                 n_actual_solutions = opt._solver_model.SolCount
             else:
                 n_actual_solutions = self._count_optimal_solution(opt)
@@ -386,46 +385,46 @@
                                 'aug_mig_graph': G, 'n_mig': int(mu), 'n_comig': int(gamma),#}
                                   'other': {'r': r, 'z': z, 'p':p, 'b':b}}
                 if self.seeding_site:
                     sigma = 0
                     for s in self.Sigma:
                         if opt._pyomo_var_to_solver_var_map[self.m.q[s]].Xn > 0.5:
                             sigma += 1
-                    solution_raw['n_seedingsites'] = sigma
+                    solution_raw['n_seedinglocations'] = sigma
                 solutions_raw.append(solution_raw)
         if raw:
             return solutions_raw
         else:
-            return SolutionSet([(RefinedCloneTree(self.clone_tree, raw), MigrationGraph(raw)) for raw in solutions_raw])
+            return SolutionSet([(RefinedPhylogeny(self.phylogeny, raw), MigrationGraph(raw)) for raw in solutions_raw])
 
 
 def process_args():
     parser = argparse.ArgumentParser(description='MACH2')
 
-    parser.add_argument('clone_tree', type=str, help='Input clone tree')
+    parser.add_argument('phylogeny', type=str, help='Input clone tree')
     parser.add_argument('leaf_labeling', type=str, help='Input leaf labeling')
 
     parser.add_argument('-p', '--primary', type=str, help='Primary anatomical site')
     parser.add_argument('-c', '--colormap', metavar='COLORMAP', type=str, help='Color map file', action='store')
     parser.add_argument('--log', action='store_true', default=False, help='Outputs Gurobi logging')
     parser.add_argument('-o', '--output', action='store', default=None, help='Output folder')
     parser.add_argument('-N', '--nsolutions', type=int, help='Maximum number of solutions retained', default=10)
     parser.add_argument('-C', '--count_solutions', action='store_true', default=False, help='Only prints the number of solutions\
         (default=False)')
-    parser.add_argument('-t', '--threads', type=int, help='Number of threads')
+    parser.add_argument('-t', '--threads', type=int, help='Number of threads', default=0)
     parser.add_argument('-s', '--suboptimal', action='store_true', default=False, help='Returns suboptimal solutions without duplicates, \
         may be slow (default=False)')
-    parser.add_argument('-S', '--seeding_sites', action='store_true', default=False, help='Minimizes the number of seeding sites \
+    parser.add_argument('-S', '--seeding_locations', action='store_true', default=False, help='Minimizes the number of seeding locations \
         too (default=False)')
 
     return parser.parse_args()
 
 def main():
     args = process_args()
-    clone_tree = CloneTree.from_file(args.clone_tree, args.leaf_labeling)
+    phylogeny = Phylogeny.from_file(args.phylogeny, args.leaf_labeling)
 
     if args.output is None:
         output_str = '.'
     else:
         output_str = args.output
         if not os.path.exists(output_str):
             os.makedirs(output_str)
@@ -437,36 +436,36 @@
 
     if args.log == True:
         logfile = f'{output_str}/{primary_str}-log.txt'
     else:
         logfile = ''
 
     start_t = time.time()
-    solver = MACH(clone_tree, primary_site=args.primary, suboptimal_mode=args.suboptimal, seeding_site=args.seeding_sites)
+    solver = MACH(phylogeny, primary_site=args.primary, suboptimal_mode=args.suboptimal, seeding_site=args.seeding_locations)
     solutions = solver.solve('gurobi', args.nsolutions, logfile=logfile, n_threads=args.threads, raw=False)
     total_t = time.time() - start_t
 
     if args.count_solutions:
-        if args.seeding_sites:
-            print(f'{primary_str}-\t{int(solutions[0].n_migrations)}\t{int(solutions[0].n_comigrations)}\t{int(solutions[0].n_seeding_sites)}\t\
+        if args.seeding_locations:
+            print(f'{primary_str}-\t{int(solutions[0].n_migrations)}\t{int(solutions[0].n_comigrations)}\t{int(solutions[0].n_seeding_locations)}\t\
                 {len(solutions)}')
         else:
             print(f'{primary_str}-\t{int(solutions[0].n_migrations)}\t{int(solutions[0].n_comigrations)}\t{len(solutions)}')
     else:
         if args.colormap:
-            colormap = utils.process_colormap(colormap_filename=args.colormap)
+            colormap = utils.process_colormap_file(args.colormap)
         else:
-            colormap = utils.get_colormap(clone_tree.sites)
+            colormap = utils.get_colormap(phylogeny.locations)
         
         padding = len(str(len(solutions)))
 
         for e, soln in enumerate(solutions):
-            primary_str = soln.clone_tree.primary_site
-            soln.clone_tree.write_dot(f'{output_str}/{primary_str}-T-{str(e).zfill(padding)}.dot', colormap=colormap)
-            soln.clone_tree.write_tree(f'{output_str}/{primary_str}-T-{str(e).zfill(padding)}.tree')
-            soln.clone_tree.write_labeling(f'{output_str}/{primary_str}-T-{str(e).zfill(padding)}.labeling')
+            primary_str = soln.phylogeny.primary_site
+            soln.phylogeny.write_dot(f'{output_str}/{primary_str}-T-{str(e).zfill(padding)}.dot', colormap=colormap)
+            soln.phylogeny.write_tree(f'{output_str}/{primary_str}-T-{str(e).zfill(padding)}.tree')
+            soln.phylogeny.write_labeling(f'{output_str}/{primary_str}-T-{str(e).zfill(padding)}.labeling')
             soln.migration_graph.write_dot(f'{output_str}/{primary_str}-G-{str(e).zfill(padding)}.dot', colormap=colormap)
             soln.migration_graph.write_graph(f'{output_str}/{primary_str}-G-{str(e).zfill(padding)}.graph')
             print(f'{primary_str}-\t{e}\t{soln.n_migrations}\t{soln.n_comigrations}\t{total_t}')
 
 if __name__ == '__main__':
     main()
```

### Comparing `mach2-0.0.2/src/mach2/migrationgraph.py` & `mach2-0.0.3/src/mach2/migrationgraph.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,19 +6,19 @@
     def __init__(self, raw):
         G_raw = raw['aug_mig_graph']
         self.graph = nx.MultiDiGraph()
         for i in G_raw.values():
             for s, t in i:
                 if s != t:
                     self.graph.add_edge(s, t)
-        self.sites = [i for i in self.graph.nodes]
+        self.locations = [i for i in self.graph.nodes]
         self.n_mig = raw['n_mig']
         self.n_comig = raw['n_comig']
-        if 'n_seedingsites' in raw:
-            self.n_seedingsites = raw['n_seedingsites']
+        if 'n_seedinglocations' in raw:
+            self.n_seedinglocations = raw['n_seedinglocations']
 
     def has_migration(self, a, b):
         return self.graph.number_of_edges(a,b) > 0
     
     def n_migrations(self, a, b):
         return self.graph.number_of_edges(a,b)
     
@@ -47,28 +47,31 @@
             for edge in G_digraph.edges:
                 f.write(f'{edge[0]} {edge[1]} {self.graph.number_of_edges(edge[0], edge[1])}\n')
 
     def draw(self, colormap=None, colormap_file=None):
         import graphviz as gv
         if colormap is None:
             if colormap_file is None:
-                colormap = utils.get_colormap(self.sites)
+                colormap = utils.get_colormap(self.locations)
             else:
                 colormap = utils.process_colormap_file(colormap_file)
         g = gv.Digraph(node_attr={'shape': 'box', 'penwidth': '3', 'colorscheme': 'set19'}, edge_attr={'penwidth': '3', 'colorscheme': 'set19'})
         for s in self.graph.nodes:
             g.node(s, color=str(colormap[s]))
         for s, t, _ in self.graph.edges:
             g.edge(s, t, color=f"{colormap[s]};0.5:{colormap[t]}")
         return g
+    
+    def _repr_mimebundle_(self, include=None, exclude=None, **_):
+        return self.draw()._repr_mimebundle_(include=include, exclude=exclude)
 
     def write_dot(self, filename, colormap=None, colormap_file=None):
         if colormap is None:
             if colormap_file is None:
-                colormap = utils.get_colormap(self.sites)
+                colormap = utils.get_colormap(self.locations)
             else:
                 colormap = utils.process_colormap_file(colormap_file)
         node_index = {j:i for i,j in enumerate(self.graph.nodes)}
         with open(filename, 'w+') as f:
             f.write('digraph G {\n')
             for s in self.graph.nodes:
                 f.write(f'\t{node_index[s]} [shape=box,penwidth=3,colorscheme=set19,color={colormap[s]},' + f'label="{s}"]\n')
```

### Comparing `mach2-0.0.2/src/mach2/solutionset.py` & `mach2-0.0.3/src/mach2/solutionset.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,26 +5,26 @@
 
 
 class SolutionSet:
 
     class Solution:
 
         def __init__(self, tree, graph):
-            self.clone_tree = tree
+            self.phylogeny = tree
             self.migration_graph = graph
-            self.sites = self.clone_tree.sites
+            self.locations = self.phylogeny.locations
             self.n_migrations = self.migration_graph.n_mig
             self.n_comigrations = self.migration_graph.n_comig
 
     def __init__(self, sol_list):
         self.solution_set_whole = [SolutionSet.Solution(tree, graph) for (tree, graph) in sol_list]
         self.solution_set = defaultdict(set)
         for solution in self.solution_set_whole:
-            self.solution_set[solution.clone_tree.primary_site].add(solution)
-        self.sites = sol_list[0][0].sites
+            self.solution_set[solution.phylogeny.primary_site].add(solution)
+        self.locations = sol_list[0][0].locations
 
     def __len__(self):
         return len(self.solution_set_whole)
     
     def __getitem__(self, key):
         if type(key) == type('a'):
             return self.solution_set[key]
@@ -47,31 +47,31 @@
 
     def summary(self, primary=None, colormap=None, colormap_file=None, consider_multi_edges=False):
         if primary is None:
             sol_set = self.solution_set_whole
         else:
             sol_set = self.solution_set[primary]
         summary_graph = defaultdict(int)
-        sites = set()
+        locations = set()
         max_val = 0
         for solution in sol_set:
             for u1, v1 in solution.migration_graph.migration_edges():
                 summary_graph[(u1, v1)] += 1
                 if max_val < summary_graph[(u1, v1)]:
                     max_val = summary_graph[(u1, v1)]
-                sites.update([u1, v1])
+                locations.update([u1, v1])
 
         import graphviz as gv
         if colormap is None:
             if colormap_file is None:
-                colormap = utils.get_colormap(self.sites)
+                colormap = utils.get_colormap(self.locations)
             else:
                 colormap = utils.process_colormap_file(colormap_file)
         dot = gv.Digraph(engine='dot')
-        for i in sites:
+        for i in locations:
             dot.node(i, colorscheme='set19', color=str(
                 colormap[i]), shape='box', penwidth='3')
 
         for uv in summary_graph:
             dot.edge(uv[0], uv[1], penwidth=str(summary_graph[uv] * 5/max_val),
                      colorscheme='set19', color=f'{colormap[uv[0]]};0.5:{colormap[uv[1]]}')
             
@@ -79,50 +79,50 @@
     
     def summary_dot(self, filename, primary=None, colormap=None, colormap_file=None, consider_multi_edges=False):
         if primary is None:
             sol_set = self.solution_set_whole
         else:
             sol_set = self.solution_set[primary]
         summary_graph = defaultdict(int)
-        sites = set()
+        locations = set()
         max_val = 0
         for solution in sol_set:
             for u1, v1 in solution.migration_graph.migration_edges():
                 summary_graph[(u1, v1)] += 1
                 if max_val < summary_graph[(u1, v1)]:
                     max_val = summary_graph[(u1, v1)]
-                sites.update([u1, v1])
+                locations.update([u1, v1])
 
         import graphviz as gv
         if colormap is None:
             if colormap_file is None:
-                colormap = utils.get_colormap(self.sites)
+                colormap = utils.get_colormap(self.locations)
             else:
                 colormap = utils.process_colormap_file(colormap_file)
-        node_index = {j:i for i,j in enumerate(sites)}
+        node_index = {j:i for i,j in enumerate(locations)}
         with open(filename, 'w+') as f:
             f.write('digraph G {\n')
-            for s in sites:
+            for s in locations:
                 f.write(f'\t{node_index[s]} [shape=box,penwidth=3,colorscheme=set19,color={colormap[s]},' + f'label="{s}"]\n')
             for st in summary_graph:
                 f.write(f'\t{node_index[st[0]]} -> {node_index[st[1]]} [penwidth={summary_graph[st] * 5/max_val},colorscheme=set19,' +
                             f'color="{colormap[st[0]]};0.5:{colormap[st[1]]}"]\n')
             f.write('}\n')
 
     # def summary_write(self, filename, primary=None):
     #     if primary is None:
     #         sol_set = self.solution_set_whole
     #     else:
     #         sol_set = self.solution_set[primary]
     #     summary_graph = defaultdict(int)
-    #     sites = set()
+    #     locations = set()
     #     max_val = 0
     #     for solution in sol_set:
     #         for u1, v1 in solution.migration_graph.migration_edges():
     #             summary_graph[(u1, v1)] += 1
     #             if max_val < summary_graph[(u1, v1)]:
     #                 max_val = summary_graph[(u1, v1)]
-    #             sites.update([u1, v1])
+    #             locations.update([u1, v1])
 
     #     with open(filename, 'w+') as f:
     #         for st in summary_graph:
     #             f.write(f'{st[0]}\t{st[1]}\t{summary_graph[st] * 5/max_val}\n')
```

### Comparing `mach2-0.0.2/PKG-INFO` & `mach2-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mach2
-Version: 0.0.2
+Version: 0.0.3
 Summary: Migration Analysis of Clonal History 2
 Keywords: Computational biology Bioinformatics Cancer Metastasis Phylogeny
 Author-Email: Mrinmoy Saha Roddur <mroddur2@illinois.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, Mrinmoy Saha Roddur, Vikram Ramavarapu, Simone Zaccaria, Mohammed El-Kebir
         All rights reserved.
@@ -35,38 +35,37 @@
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Project-URL: Homepage, https://github.com/elkebir-group/MACH2
 Project-URL: Bug tracker, https://github.com/elkebir-group/MACH2/issues
 Requires-Python: >=3.7
-Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pyomo
 Requires-Dist: networkx
-Requires-Dist: gurobi
+Requires-Dist: gurobipy
 Requires-Dist: jupyterlab; extra == "jupyter"
 Requires-Dist: python-graphviz; extra == "jupyter"
 Provides-Extra: jupyter
 Description-Content-Type: text/markdown
 
 # MACH2
 
 A mathematical framework for inferring migration histories of metastatic cancer from clone phylogeny and the location of extant clones.
 
 ## Table of contents
 
-1. Installation
-        - Prerequisite
-        - Install using `pip`
-2. Usage instruction
-        - I/O formats
-        - Input
-        - Output
-        - Usage
+1. [Installation](#installation)  
+        - [Prerequisite](#prerequisite)  
+        - [Install using `pip`](#install-using-pip)
+2. [Usage instruction](#usage-instruction)  
+        - [I/O formats](#i-o-formats)  
+        - [Input](#input)  
+        - [Output](#output)  
+        - [Usage](#usage)  
 
 ## 1. Installation
 
 ### Prerequisites
 
 - **Python** - `MACH2` requires Python 3.7 or newer.
 - **ILP solver** - `MACH2` requires an ILP solver installed to solve **PMH-TR**. Currently `MACH2` only supports `Gurobi optimizer`, but we are going to add support for more ILP solvers in the future. `MACH2` requires a valid Gurobi installation and license key. The location of Gurobi should be present in `LD_LIBRARY_PATH` (linux) and `DYLD_LIBRARY_PATH` (macOS) the license key should be saved in the environment variable `GRB_LICENSE_KEY`.
```

