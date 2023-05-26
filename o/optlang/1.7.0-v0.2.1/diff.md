# Comparing `tmp/optlang-1.7.0.tar.gz` & `tmp/optlang-v0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "optlang-1.7.0.tar", last modified: Fri May 26 15:39:42 2023, max compression
+gzip compressed data, was "dist/optlang-v0.2.1.tar", last modified: Wed Apr 15 20:40:21 2015, max compression
```

## Comparing `optlang-1.7.0.tar` & `optlang-v0.2.1.tar`

### file list

```diff
@@ -1,57 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:42.896425 optlang-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11325 2023-05-26 15:39:28.000000 optlang-1.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 15:39:28.000000 optlang-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-26 15:39:42.896425 optlang-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6717 2023-05-26 15:39:28.000000 optlang-1.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-26 15:39:42.900425 optlang-1.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-26 15:39:28.000000 optlang-1.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:42.892425 optlang-1.7.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:42.900425 optlang-1.7.0/src/optlang/
--rw-r--r--   0 runner    (1001) docker     (123)     3226 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-26 15:39:42.900425 optlang-1.7.0/src/optlang/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    30584 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/coinor_cbc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    40948 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/cplex_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7667 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/duality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6172 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/expression_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/glpk_exact_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    35709 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/glpk_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    31219 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/gurobi_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12977 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/inspyred_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    60731 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    33889 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/osqp_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    24812 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/scipy_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     4052 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/symbolics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:42.896425 optlang-1.7.0/src/optlang/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40341 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/abstract_test_cases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:42.896425 optlang-1.7.0/src/optlang/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1577 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/data/parse_the_final_netlib_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     3697 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_change_solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    27774 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_coinor_cbc_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9073 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    33151 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_cplex_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_duality.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_elements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_expression_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)    19505 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_glpk_exact_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    24465 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_glpk_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    26280 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_gurobi_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_inspyred_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     9659 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)    26629 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_osqp_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    12415 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_scipy_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_symbolics.py
--rw-r--r--   0 runner    (1001) docker     (123)     9552 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11006 2023-05-26 15:39:28.000000 optlang-1.7.0/src/optlang/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 15:39:42.896425 optlang-1.7.0/src/optlang.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8090 2023-05-26 15:39:42.000000 optlang-1.7.0/src/optlang.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-26 15:39:42.000000 optlang-1.7.0/src/optlang.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:39:42.000000 optlang-1.7.0/src/optlang.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 15:39:42.000000 optlang-1.7.0/src/optlang.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-26 15:39:42.000000 optlang-1.7.0/src/optlang.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 15:39:42.000000 optlang-1.7.0/src/optlang.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-26 15:39:28.000000 optlang-1.7.0/versioneer.py
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-04-15 20:40:21.000000 optlang-v0.2.1/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      760 2015-04-15 20:40:21.000000 optlang-v0.2.1/PKG-INFO
+-rw-rw-r--   0 travis    (1000) travis    (1000)    36722 2015-04-15 20:37:12.000000 optlang-v0.2.1/versioneer.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     2345 2015-04-15 20:37:12.000000 optlang-v0.2.1/setup.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)      173 2015-04-15 20:37:12.000000 optlang-v0.2.1/setup.cfg
+-rw-rw-r--   0 travis    (1000) travis    (1000)       38 2015-04-15 20:37:12.000000 optlang-v0.2.1/requirements.txt
+-rw-rw-r--   0 travis    (1000) travis    (1000)     3806 2015-04-15 20:37:12.000000 optlang-v0.2.1/README.md
+-rw-rw-r--   0 travis    (1000) travis    (1000)    11325 2015-04-15 20:37:12.000000 optlang-v0.2.1/LICENSE
+drwxrwxr-x   0 travis    (1000) travis    (1000)        0 2015-04-15 20:40:21.000000 optlang-v0.2.1/optlang/
+-rw-rw-r--   0 travis    (1000) travis    (1000)      418 2015-04-15 20:40:21.000000 optlang-v0.2.1/optlang/_version.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     4488 2015-04-15 20:37:12.000000 optlang-v0.2.1/optlang/util.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    31043 2015-04-15 20:37:12.000000 optlang-v0.2.1/optlang/interface.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    12982 2015-04-15 20:37:12.000000 optlang-v0.2.1/optlang/inspyred_interface.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    35231 2015-04-15 20:37:12.000000 optlang-v0.2.1/optlang/glpk_interface.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)    30109 2015-04-15 20:37:12.000000 optlang-v0.2.1/optlang/cplex_interface.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     5987 2015-04-15 20:37:12.000000 optlang-v0.2.1/optlang/container.py
+-rw-rw-r--   0 travis    (1000) travis    (1000)     1392 2015-04-15 20:37:12.000000 optlang-v0.2.1/optlang/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `optlang-1.7.0/LICENSE` & `optlang-v0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `optlang-1.7.0/src/optlang/coinor_cbc_interface.py` & `optlang-v0.2.1/optlang/cplex_interface.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,814 +9,692 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+"""Solver interface for the IBM ILOG CPLEX Optimization Studio solver.
 
-"""
-Interface for the Python MIP (Mixed-Integer Linear Programming) Tools.
-
-Wraps the MIP solver by subclassing and extending :class:`Model`,
+Wraps the GLPK solver by subclassing and extending :class:`Model`,
 :class:`Variable`, and :class:`Constraint` from :mod:`interface`.
-
-MIP is an open source MILP Python wrapper around the open-source COIN-OR
-Branch-&-Cut CBC solver. To use MIP you need to install the 'mip'
-python package (with pip or from https://www.python-mip.com/)
-and make sure that 'import mip' runs without error.
 """
-import logging
-
+import collections
 import six
 
-from optlang.util import inheritdocstring, TemporaryFilename
-from optlang.expression_parsing import parse_optimization_expression
-from optlang import interface
-from optlang import symbolics
-
-from math import isclose, ceil, floor
+if six.PY3:
+    from io import StringIO
+else:
+    from StringIO import StringIO
 
-try:
-    import mip
-except ImportError:
-    raise ImportError("The coinor_cbc_interface requires mip!")
+import sys
 
+import logging
 
 log = logging.getLogger(__name__)
 
-_MIP_STATUS_TO_STATUS = {
-    mip.OptimizationStatus.CUTOFF: interface.CUTOFF,
-    mip.OptimizationStatus.ERROR: interface.ABORTED,
-    mip.OptimizationStatus.FEASIBLE: interface.FEASIBLE,
-    mip.OptimizationStatus.INFEASIBLE: interface.INFEASIBLE,
-    mip.OptimizationStatus.INT_INFEASIBLE: interface.SPECIAL,
-    mip.OptimizationStatus.LOADED: interface.LOADED,
-    mip.OptimizationStatus.NO_SOLUTION_FOUND: interface.NOFEASIBLE,
-    mip.OptimizationStatus.OPTIMAL: interface.OPTIMAL,
-    mip.OptimizationStatus.UNBOUNDED: interface.UNBOUNDED,
-    mip.OptimizationStatus.OTHER: interface.SPECIAL
-}
+import tempfile
+import sympy
+from sympy.core.add import _unevaluated_Add
+from sympy.core.mul import _unevaluated_Mul
+import cplex
+from optlang import interface
 
-_MIP_VTYPE_TO_VTYPE = {
-    mip.CONTINUOUS: 'continuous',
-    mip.INTEGER: 'integer',
-    mip.BINARY: 'binary'
+_CPLEX_STATUS_TO_STATUS = {
+    cplex.Cplex.solution.status.MIP_abort_feasible: interface.ABORTED,
+    cplex.Cplex.solution.status.MIP_abort_infeasible: interface.ABORTED,
+    cplex.Cplex.solution.status.MIP_dettime_limit_feasible: interface.TIME_LIMIT,
+    cplex.Cplex.solution.status.MIP_dettime_limit_infeasible: interface.TIME_LIMIT,
+    cplex.Cplex.solution.status.MIP_feasible: interface.FEASIBLE,
+    cplex.Cplex.solution.status.MIP_feasible_relaxed_inf: interface.SPECIAL,
+    cplex.Cplex.solution.status.MIP_feasible_relaxed_quad: interface.SPECIAL,
+    cplex.Cplex.solution.status.MIP_feasible_relaxed_sum: interface.SPECIAL,
+    cplex.Cplex.solution.status.MIP_infeasible: interface.INFEASIBLE,
+    cplex.Cplex.solution.status.MIP_infeasible_or_unbounded: interface.INFEASIBLE_OR_UNBOUNDED,
+    cplex.Cplex.solution.status.MIP_optimal: interface.OPTIMAL,
+    cplex.Cplex.solution.status.MIP_optimal_infeasible: interface.SPECIAL,
+    cplex.Cplex.solution.status.MIP_optimal_relaxed_inf: interface.SPECIAL,
+    cplex.Cplex.solution.status.MIP_optimal_relaxed_sum: interface.SPECIAL,
+    cplex.Cplex.solution.status.MIP_time_limit_feasible: interface.TIME_LIMIT,
+    cplex.Cplex.solution.status.MIP_time_limit_infeasible: interface.TIME_LIMIT,
+    cplex.Cplex.solution.status.MIP_unbounded: interface.UNBOUNDED,
+    cplex.Cplex.solution.status.abort_dettime_limit: interface.ABORTED,
+    cplex.Cplex.solution.status.abort_dual_obj_limit: interface.ABORTED,
+    cplex.Cplex.solution.status.abort_iteration_limit: interface.ABORTED,
+    cplex.Cplex.solution.status.abort_obj_limit: interface.ABORTED,
+    cplex.Cplex.solution.status.abort_primal_obj_limit: interface.ABORTED,
+    cplex.Cplex.solution.status.abort_relaxed: interface.ABORTED,
+    cplex.Cplex.solution.status.abort_time_limit: interface.TIME_LIMIT,
+    cplex.Cplex.solution.status.abort_user: interface.ABORTED,
+    cplex.Cplex.solution.status.conflict_abort_contradiction: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_abort_dettime_limit: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_abort_iteration_limit: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_abort_memory_limit: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_abort_node_limit: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_abort_obj_limit: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_abort_time_limit: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_abort_user: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_feasible: interface.SPECIAL,
+    cplex.Cplex.solution.status.conflict_minimal: interface.SPECIAL,
+    cplex.Cplex.solution.status.fail_feasible: interface.SPECIAL,
+    cplex.Cplex.solution.status.fail_feasible_no_tree: interface.SPECIAL,
+    cplex.Cplex.solution.status.fail_infeasible: interface.SPECIAL,
+    cplex.Cplex.solution.status.fail_infeasible_no_tree: interface.SPECIAL,
+    cplex.Cplex.solution.status.feasible: interface.FEASIBLE,
+    cplex.Cplex.solution.status.feasible_relaxed_inf: interface.SPECIAL,
+    cplex.Cplex.solution.status.feasible_relaxed_quad: interface.SPECIAL,
+    cplex.Cplex.solution.status.feasible_relaxed_sum: interface.SPECIAL,
+    cplex.Cplex.solution.status.first_order: interface.SPECIAL,
+    cplex.Cplex.solution.status.infeasible: interface.INFEASIBLE,
+    cplex.Cplex.solution.status.infeasible_or_unbounded: interface.INFEASIBLE_OR_UNBOUNDED,
+    cplex.Cplex.solution.status.mem_limit_feasible: interface.MEMORY_LIMIT,
+    cplex.Cplex.solution.status.mem_limit_infeasible: interface.MEMORY_LIMIT,
+    cplex.Cplex.solution.status.node_limit_feasible: interface.NODE_LIMIT,
+    cplex.Cplex.solution.status.node_limit_infeasible: interface.NODE_LIMIT,
+    cplex.Cplex.solution.status.num_best: interface.NUMERIC,
+    cplex.Cplex.solution.status.optimal: interface.OPTIMAL,
+    cplex.Cplex.solution.status.optimal_face_unbounded: interface.SPECIAL,
+    cplex.Cplex.solution.status.optimal_infeasible: interface.SPECIAL,
+    cplex.Cplex.solution.status.optimal_populated: interface.SPECIAL,
+    cplex.Cplex.solution.status.optimal_populated_tolerance: interface.SPECIAL,
+    cplex.Cplex.solution.status.optimal_relaxed_inf: interface.SPECIAL,
+    cplex.Cplex.solution.status.optimal_relaxed_quad: interface.SPECIAL,
+    cplex.Cplex.solution.status.optimal_relaxed_sum: interface.SPECIAL,
+    cplex.Cplex.solution.status.optimal_tolerance: interface.SPECIAL,
+    cplex.Cplex.solution.status.populate_solution_limit: interface.SPECIAL,
+    cplex.Cplex.solution.status.solution_limit: interface.SPECIAL,
+    cplex.Cplex.solution.status.unbounded: interface.UNBOUNDED,
+    102: interface.OPTIMAL # CPXMIP_OPTIMAL_TOL not covered by python bindings???
 }
 
-_VTYPE_TO_MIP_VTYPE = dict(
-    [(val, key) for key, val in six.iteritems(_MIP_VTYPE_TO_VTYPE)]
-)
+_CPLEX_VTYPE_TO_VTYPE = {'C': 'continuous', 'I': 'integer', 'B': 'binary'}
+# FIXME: what about 'S': 'semi_continuous', 'N': 'semi_integer'
 
-_DIR_TO_MIP_DIR = {
-    'max': mip.MAXIMIZE,
-    'min': mip.MINIMIZE
-}
-
-_MIP_DIR_TO_DIR = dict(
-    [(val, key) for key, val in six.iteritems(_DIR_TO_MIP_DIR)]
+_VTYPE_TO_CPLEX_VTYPE = dict(
+    [(val, key) for key, val in six.iteritems(_CPLEX_VTYPE_TO_VTYPE)]
 )
 
-# Needs to be used for to_bound during _initialize_model_from_problem
-INFINITY = 1.7976931348623157e+308
 
-def to_float(number, is_lb=True):
-    """Converts None type and sympy.core.numbers.Float to float."""
-    if number is not None:
-        return float(number)
-    if is_lb:
-        return -INFINITY
-    return INFINITY
-
-def to_bound(number):
-    """Convert float with infs to None."""
-    if abs(number) == INFINITY:
-        return None
-    return number
-
-def to_symbolic_expr(coeffs):
-    """Converts coeffs dict to symbolic expression."""
-    return symbolics.add([var * coef for var, coef in coeffs.items()
-                          if not isclose(0, to_float(coef))])
+def _constraint_lb_and_ub_to_cplex_sense_rhs_and_range_value(lb, ub):
+    """Helper function used by Constraint and Model"""
+    if lb is None and ub is None:
+        # FIXME: use cplex.infinity
+        raise Exception("Free constraint ...")
+    elif lb is None:
+        sense = 'L'
+        rhs = float(ub)
+        range_value = 0.
+    elif ub is None:
+        sense = 'G'
+        rhs = float(lb)
+        range_value = 0.
+    elif lb == ub:
+        sense = 'E'
+        rhs = float(lb)
+        range_value = 0.
+    else:
+        sense = 'R'
+        rhs = float(lb)
+        range_value = float(ub - lb)
+    return sense, rhs, range_value
 
-@six.add_metaclass(inheritdocstring)
 class Variable(interface.Variable):
+    """CPLEX variable interface."""
+
     def __init__(self, name, *args, **kwargs):
         super(Variable, self).__init__(name, **kwargs)
 
     @interface.Variable.lb.setter
     def lb(self, value):
-        interface.Variable.lb.fset(self, value)
+        super(Variable, self.__class__).lb.fset(self, value)
         if self.problem is not None:
-            self.problem._update_var_lb(self.name, value)
+            self.problem.problem.variables.set_lower_bounds(self.name, value)
 
     @interface.Variable.ub.setter
     def ub(self, value):
-        interface.Variable.ub.fset(self, value)
-        if self.problem is not None:
-            self.problem._update_var_ub(self.name, value)
-
-    def set_bounds(self, lb, ub):
-        super(Variable, self).set_bounds(lb, ub)
+        super(Variable, self.__class__).ub.fset(self, value)
         if self.problem is not None:
-            self.problem._update_var_lb(self.name, lb)
-            self.problem._update_var_ub(self.name, ub)
+            self.problem.problem.variables.set_upper_bounds(self.name, value)
 
     @interface.Variable.type.setter
     def type(self, value):
-        if not value in _VTYPE_TO_MIP_VTYPE:
-            raise ValueError(
-                'COIN-OR CBC cannot handle variables of type %s. ' % value +
-                'The following variable types are available:\n' +
-                ' '.join(_VTYPE_TO_MIP_VTYPE.keys()))
-
-        if self.problem is not None:
-            self.problem._update_var_type(self.name, _VTYPE_TO_MIP_VTYPE[value])
-        interface.Variable.type.fset(self, value)
-
-        if value == 'integer':
-            if self.lb is not None:
-                self.lb = ceil(self.lb)
-            if self.ub is not None:
-                self.ub = floor(self.ub)
-        elif value == 'binary':
-            self.lb, self.ub = 0, 1
+        if self.problem is not None:
+            try:
+                cplex_kind = _VTYPE_TO_CPLEX_VTYPE[value]
+            except KeyError:
+                raise Exception("CPLEX cannot handle variables of type %s. \
+                            The following variable types are available:\n" +
+                                " ".join(_VTYPE_TO_CPLEX_VTYPE.keys()))
+            self.problem.problem.variables.set_types(self.name, cplex_kind)
+        super(Variable, self).__setattr__('type', value)
+
 
     @property
     def primal(self):
-        if self.problem is None:
+        if self.problem:
+            primal_from_solver = self.problem.problem.solution.get_values(self.name)
+            return self._round_primal_to_bounds(primal_from_solver)
+        else:
             return None
-        return self.problem._var_primal(self.name)
 
     @property
     def dual(self):
-        if self.type != 'continuous':
-            raise ValueError('Dual is only available for continuous variables')
-        if self.problem is None:
+        if self.problem is not None:
+            if self.problem.problem.get_problem_type() != self.problem.problem.problem_type.LP: # cplex cannot determine reduced costs for MILP problems ...
+                return None
+            return self.problem.problem.solution.get_reduced_costs(self.name)
+        else:
             return None
-        return self.problem._var_dual(self.name)
 
-    @interface.Variable.name.setter
-    def name(self, value):
-        super(Variable, Variable).name.fset(self, value)
-        if getattr(self, 'problem', None) is not None:
-            raise Exception('COIN-OR CBC doesn\'t support variable name change')
 
-
-@six.add_metaclass(inheritdocstring)
 class Constraint(interface.Constraint):
-    _INDICATOR_CONSTRAINT_SUPPORT = False
+    """CPLEX solver interface"""
+
+    _INDICATOR_CONSTRAINT_SUPPORT = True
 
-    def __init__(self, expression, sloppy=False, *args, **kwargs):
-        self._changed_expression = {}
-        super(Constraint, self).__init__(expression, sloppy=sloppy, *args, **kwargs)
-
-    def constraint_name(self, is_lb):
-        if is_lb:
-            return 'c_' + self.name + '_lower'
-        return 'c_' + self.name + '_upper'
+    def __init__(self, expression, *args, **kwargs):
+        super(Constraint, self).__init__(expression, *args, **kwargs)
+
+    # TODO: get expression from solver structure
+    def _get_expression(self):
+        if self.problem is not None:
+            cplex_problem = self.problem.problem
+            cplex_row = cplex_problem.linear_constraints.get_rows(self.name)
+            variables = self.problem.variables
+            expression = sympy.Add._from_args([sympy.Mul._from_args((sympy.RealNumber(cplex_row.val[i]), variables[ind])) for i, ind in enumerate(cplex_row.ind)])
+            self._expression = expression
+        return self._expression
+
+    def _set_coefficients_low_level(self, variables_coefficients_dict):
+        self_name = self.name
+        if self.is_Linear:
+            cplex_format = [(self_name, variable.name, coefficient) for variable, coefficient in six.iteritems(variables_coefficients_dict)]
+            self.problem.problem.linear_constraints.set_coefficients(cplex_format)
+        else:
+            raise Exception('_set_coefficients_low_level works only with linear constraints in the cplex interface.')
+
+    @property
+    def problem(self):
+        return self._problem
+
+    @problem.setter
+    def problem(self, value):
+        if value is None:
+            # Update expression from solver instance one last time
+            self._get_expression()
+            self._problem = None
+        else:
+            self._problem = value
 
     @property
     def primal(self):
-        if getattr(self, 'problem', None) is not None \
-           and self.problem.status == interface.OPTIMAL:
-            if self.lb is not None:
-                return self.problem._constr_primal(self, True)
-            if self.ub is not None:
-                return self.problem._constr_primal(self, False)
-        return None
+        if self.problem is not None:
+            return self.problem.problem.solution.get_activity_levels(self.name)
+        else:
+            return None
 
     @property
     def dual(self):
-        if getattr(self, 'problem', None) is None:
+        if self.problem is not None:
+            return self.problem.problem.solution.get_dual_values(self.name)
+        else:
             return None
-        if self.lb is not None:
-            return self.problem._constr_dual(self, True)
-        if self.ub is not None:
-            return self.problem._constr_dual(self, False)
-        return None
-
-    def _update_bound(self, new, old, is_lb):
-        """Updates associated mip model with new constraint bounds."""
-        if getattr(self, 'problem', None) is None:
-            return
-
-        if old is None and new is not None:
-            self.problem._add_mip_constraint(self, is_lb)
-        elif new is None and old is not None:
-            self.problem._remove_mip_constraint(self, is_lb)
-        elif new is not None and old is not None:
-            self.problem._update_constraint_bound(self, is_lb)
-
-    @interface.Constraint.lb.setter
-    def lb(self, value):
-        self._check_valid_lower_bound(value)
-        self._lb, old_lb = value, getattr(self, '_lb', None)
-        self._update_bound(value, old_lb, True)
-
-    @interface.Constraint.ub.setter
-    def ub(self, value):
-        self._check_valid_upper_bound(value)
-        self._ub, old_ub = value, getattr(self, '_ub', None)
-        self._update_bound(value, old_ub, False)
-
-    @interface.Constraint.name.setter
-    def name(self, value):
-        super(Constraint, Constraint).name.fset(self, value)
-        if getattr(self, 'problem', None) is not None:
-            raise Exception('COIN-OR CBC doesn\'t support constraint name change')
-
-    def _get_expression(self):
-        if (self.problem is not None and self._changed_expression and
-            len(self.problem._variables) > 0):
-
-            coeffs = self._expression.as_coefficients_dict()
-
-            new_vars = set(self._changed_expression) - set(coeffs)
-
-            self._expression += symbolics.add([var * self._changed_expression[var]
-                                              for var in new_vars])
 
-            # Substitute var in expression with var * coef / old_coef
-            updates = {var: var * coef / coeffs[var]
-                       for var, coef in self._changed_expression.items()
-                       if var not in new_vars}
-
-            self._expression = self._expression.subs(updates)
-            self._changed_expression = {}
-
-        return self._expression
-
-    def _get_mip_constr_expr(self):
-        """Returns mip coefficient dictionary."""
-        mip_constr = self.problem.problem.constr_by_name
-        constr = mip_constr(self.constraint_name(is_lb=False))
-        sign = 1
-        if constr is None:
-            constr = mip_constr(self.constraint_name(is_lb=True))
-            sign = -1
-        return (sign * constr.expr).expr
-
-    def set_linear_coefficients(self, coefficients):
-        if self.problem is None:
-            raise Exception('Can\'t change coefficients if constraint is not associated with a model.')
-
-        self.problem.update()
-
-        mip_var = self.problem.problem.var_by_name
-
-        expr = self._get_mip_constr_expr()
-        names = set(var.name for var in coefficients)
-
-        constr = mip.xsum(mip_var('v_' + var.name) * coef
-                       for var, coef in coefficients.items()) \
-               + mip.xsum(var * coef for var, coef in expr.items()
-                       if var.name[2:] not in names)
-
-        self.problem._remove_mip_constraint(self, True)
-        self.problem._remove_mip_constraint(self, False)
-        self.problem._add_mip_constraint(self, True, constr)
-        self.problem._add_mip_constraint(self, False, constr)
-
-        self._changed_expression.update(coefficients)
-
-    def get_linear_coefficients(self, variables):
-        if self.problem is None:
-            raise Exception('Can\'t get coefficients from solver if constraint is not in a model')
-
-        self.problem.update()
-        mip_var = self.problem.problem.var_by_name
-        expr = self._get_mip_constr_expr()
-        return {v: expr.get(mip_var('v_' + v.name), 0) for v in variables}
+    # TODO: Refactor to use properties
+    def __setattr__(self, name, value):
+        try:
+            old_name = self.name  # TODO: This is a hack
+        except AttributeError:
+            pass
+        super(Constraint, self).__setattr__(name, value)
+        if getattr(self, 'problem', None):
+
+            if name == 'name':
+                if self.indicator_variable is not None:
+                    raise NotImplementedError("Unfortunately, the CPLEX python bindings don't support changing an indicator constraint's name")
+                else:
+                    # TODO: the following needs to deal with quadratic constraints
+                    self.problem.problem.linear_constraints.set_names(old_name, value)
+
+            elif name == 'lb' or name == 'ub':
+                if self.indicator_variable is not None:
+                    raise NotImplementedError("Unfortunately, the CPLEX python bindings don't support changing an indicator constraint's bounds")
+                if name == 'lb':
+                    sense, rhs, range_value = _constraint_lb_and_ub_to_cplex_sense_rhs_and_range_value(value, self.ub)
+                elif name == 'ub':
+                    sense, rhs, range_value = _constraint_lb_and_ub_to_cplex_sense_rhs_and_range_value(self.lb, value)
+                if self.is_Linear:
+                    self.problem.problem.linear_constraints.set_rhs(self.name, rhs)
+                    self.problem.problem.linear_constraints.set_senses(self.name, sense)
+                    self.problem.problem.linear_constraints.set_range_values(self.name, range_value)
+
+            elif name == 'expression':
+                pass
+
+    def __iadd__(self, other):
+        # if self.problem is not None:
+        #     self.problem._add_to_constraint(self.index, other)
+        if self.problem is not None:
+            problem_reference = self.problem
+            self.problem._remove_constraint(self)
+            super(Constraint, self).__iadd__(other)
+            problem_reference._add_constraint(self, sloppy=False)
+        else:
+            super(Constraint, self).__iadd__(other)
+        return self
 
 
-@six.add_metaclass(inheritdocstring)
 class Objective(interface.Objective):
-    def __init__(self, expression, sloppy=False, **kwargs):
-        self._changed_expression = {}
-        super(Objective, self).__init__(expression, sloppy=sloppy, **kwargs)
-        if not (sloppy or self.is_Linear):
-            raise ValueError(
-                'COIN-OR CBC only supports linear objectives. %s is not linear.' % self)
+    def __init__(self, *args, **kwargs):
+        super(Objective, self).__init__(*args, **kwargs)
 
     @property
     def value(self):
-        if getattr(self, 'problem', None) is None:
-            return None
-        return self.problem.problem.objective_value
+        return self.problem.problem.solution.get_objective_value()
 
-    @interface.Objective.direction.setter
-    def direction(self, value):
-        super(Objective, self.__class__).direction.fset(self, value)
-        if getattr(self, 'problem', None) is not None:
-            self.problem.problem.sense = _DIR_TO_MIP_DIR[value]
+    def __setattr__(self, name, value):
 
-    def _get_expression(self):
-        if (self.problem is not None and self._changed_expression and
-            len(self.problem._variables) > 0):
+        if getattr(self, 'problem', None):
+            if name == 'direction':
+                self.problem.problem.objective.set_sense(
+                    {'min': self.problem.problem.objective.sense.minimize, 'max': self.problem.problem.objective.sense.maximize}[value])
+            super(Objective, self).__setattr__(name, value)
+        else:
+            super(Objective, self).__setattr__(name, value)
 
-            coeffs = self._expression.as_coefficients_dict()
 
-            new_vars = set(self._changed_expression) - set(coeffs)
+class Configuration(interface.MathematicalProgrammingConfiguration):
+    def __init__(self, presolve=False, verbosity=0, timeout=None, *args, **kwargs):
+        super(Configuration, self).__init__(*args, **kwargs)
+        self.presolve = presolve
+        self.verbosity = verbosity
+        self.timeout = timeout
 
-            self._expression += symbolics.add([var * self._changed_expression[var]
-                                              for var in new_vars])
+    @property
+    def presolve(self):
+        return self._presolve
 
-            # Substitute var in expression with var * coef / old_coef
-            updates = {var: var * coef / coeffs[var]
-                       for var, coef in self._changed_expression.items()
-                       if var not in new_vars}
+    @presolve.setter
+    def presolve(self, value):
+        if self.problem is not None:
+            presolve = self.problem.problem.parameters.preprocessing.presolve
+            if value == True:
+                presolve.set(presolve.values.on)
+            elif value == False:
+                presolve.set(presolve.values.off)
+            else:
+                raise ValueError('%s is not boolean argument for presolve property.')
+        self._presolve = value
 
-            self._expression = self._expression.subs(updates)
-            self._changed_expression = {}
+    @property
+    def verbosity(self):
+        return self._verbosity
 
-        return self._expression
+    @verbosity.setter
+    def verbosity(self, value):
 
-    def set_linear_coefficients(self, coefficients):
-        if self.problem is None:
-            raise Exception('Can\'t change coefficients if objective is not associated with a model.')
-
-        self.problem.update()
-        model = self.problem.problem
-        expr = model.objective.expr
-        names = set(var.name for var in coefficients)
-
-        obj = mip.xsum(model.var_by_name('v_' + var.name) * coef
-                       for var, coef in coefficients.items()) \
-            + mip.xsum(var * coef for var, coef in expr.items()
-                       if var.name[2:] not in names) \
-            + model.objective.const
-
-        # TODO: why does this not work? It would likely be faster
-        # obj_update = mip.xsum(model.var_by_name('v_' + var.name) * coef
-        #                       for var, coef in coefficients.items()) \
-        #            - mip.xsum(-var * coef for var, coef in expr.items()
-        #                       if var.name[2:] in names)
-        # model.objective.add_expr(obj_update)
-
-        self._changed_expression.update(coefficients)
-        model.objective = obj
-
-    def get_linear_coefficients(self, variables):
-        if self.problem is None:
-            raise Exception('Can\'t get coefficients from solver if objective is not in a model')
-
-        self.problem.update()
-
-        coeffs = self.problem.problem.objective.expr
-        mip_var = self.problem.problem.var_by_name
-        return {v: coeffs.get(mip_var('v_' + v.name), 0) for v in variables}
+        class StreamHandler(StringIO):
 
+            def __init__(self, logger, *args, **kwargs):
+                StringIO.__init__(self, *args, **kwargs)
+                self.logger = logger
 
-@six.add_metaclass(inheritdocstring)
-class Configuration(interface.MathematicalProgrammingConfiguration):
-    def __init__(self, verbosity=0, timeout=None, presolve='auto',
-                 max_nodes=None, max_solutions=None, relax=False,
-                 emphasis=0, cuts=-1, threads=0, *args, **kwargs):
-        super(Configuration, self).__init__(*args, **kwargs)
+        class ErrorStreamHandler(StreamHandler):
 
-        self.verbosity = verbosity
+            def flush(self):
+                self.logger.error(self.getvalue())
 
-        # Enables/disables pre-processing. Pre-processing tries to improve your MIP
-        # formulation. -1 means automatic, 0 means off and 1 means on.
-        self.presolve = presolve
+        class WarningStreamHandler(StreamHandler):
 
-        # Time limit in seconds for search
-        self.timeout = timeout
+            def flush(self):
+                self.logger.warn(self.getvalue())
 
-        # Maximum number of nodes to be explored in the search tree
-        self.max_nodes = max_nodes
+        class LogStreamHandler(StreamHandler):
 
-        # Solution limit, search will be stopped when max_solutions are found
-        self.max_solutions = max_solutions
+            def flush(self):
+                self.logger.debug(self.getvalue())
 
-        # If true only the linear programming relaxation will be solved, i.e.
-        # integrality constraints will be temporarily discarded. Changes the
-        # type of all integer and binary variables to continuous. Bounds are preserved.
-        self.relax = relax
-
-        # 0. default setting: tries to balance between the search of improved feasible
-        #    solutions and improvedlower bounds
-        # 1. feasibility: focus on finding improved feasible solutions in the first
-        #    moments of the search process,activates heuristics
-        # 2. optimality: activates procedures that produce improved lower bounds,
-        #    focusing in pruning thesearch tree even if the production of the first
-        #    feasible solutions is delayed
-        self.emphasis = emphasis
-
-        # Controls the generation of cutting planes, -1 means automatic,
-        # 0 disables completely, 1 (de-fault) generates cutting planes in
-        # a moderate way, 2 generates cutting planes aggressively and 3
-        # generates even more cutting planes. Cutting planes usually improve
-        # the LP relaxation bound but also make the solution time of the LP
-        # relaxation larger, so the overall effect is hardto predict and
-        # experimenting different values for this parameter may be beneficial.
-        self.cuts = cuts
-
-        # Number of threads to be used when solving the problem. 0 uses solver
-        # default configuration, -1 uses the number of available processing cores
-        # and >= 1 uses the specified number of threads. An increased number of
-        # threads may improve the solution time but also increases the memory consumption
-        self.threads = threads
-
-        if 'tolerances' in kwargs:
-            for key, val in six.iteritems(kwargs['tolerances']):
-                if key in self._tolerance_functions():
-                    setattr(self.tolerances, key, val)
+        class ResultsStreamHandler(StreamHandler):
 
-    @property
-    def verbosity(self):
-        return self._verbosity
+            def flush(self):
+                self.logger.debug(self.getvalue())
 
-    @verbosity.setter
-    def verbosity(self, value):
+        logger = logging.getLogger()
+        logger.setLevel(logging.CRITICAL)
+        error_stream_handler = ErrorStreamHandler(logger)
+        warning_stream_handler = WarningStreamHandler(logger)
+        log_stream_handler = LogStreamHandler(logger)
+        results_stream_handler = LogStreamHandler(logger)
+        if self.problem is not None:
+            problem = self.problem.problem
+            if value == 0:
+                problem.set_error_stream(error_stream_handler)
+                problem.set_warning_stream(warning_stream_handler)
+                problem.set_log_stream(log_stream_handler)
+                problem.set_results_stream(results_stream_handler)
+            elif value == 1:
+                problem.set_error_stream(sys.stderr)
+                problem.set_warning_stream(warning_stream_handler)
+                problem.set_log_stream(log_stream_handler)
+                problem.set_results_stream(results_stream_handler)
+            elif value == 2:
+                problem.set_error_stream(sys.stderr)
+                problem.set_warning_stream(sys.stderr)
+                problem.set_log_stream(log_stream_handler)
+                problem.set_results_stream(results_stream_handler)
+            elif value == 3:
+                problem.set_error_stream(sys.stderr)
+                problem.set_warning_stream(sys.stderr)
+                problem.set_log_stream(sys.stdout)
+                problem.set_results_stream(sys.stdout)
+            else:
+                raise Exception(
+                    "%s is not a valid verbosity level ranging between 0 and 3."
+                    % value
+                )
         self._verbosity = value
-        if getattr(self, 'problem', None) is not None:
-            self.problem.problem.verbose = int(value > 1)
-
-    @property
-    def presolve(self):
-        return self._presolve
-
-    @presolve.setter
-    def presolve(self, value):
-        self._presolve = value
-        if getattr(self, 'problem', None) is not None:
-            value = -1 if value == 'auto' else int(value)
-            self.problem.problem.preprocess = value
 
     @property
     def timeout(self):
         return self._timeout
 
     @timeout.setter
     def timeout(self, value):
+        if self.problem is not None:
+            if value is None:
+                self.problem.problem.parameters.timelimit.reset()
+            else:
+                self.problem.problem.parameters.timelimit.set(value)
         self._timeout = value
-        if getattr(self, 'problem', None) is not None:
-            if value is not None:
-                self.problem.problem.max_seconds = value
 
-    @property
-    def max_nodes(self):
-        return self._max_nodes
 
-    @max_nodes.setter
-    def max_nodes(self, value):
-        self._max_nodes = value
-        if getattr(self, 'problem', None) is not None:
-            if value is not None:
-                self.problem.problem.max_nodes = value
-
-    @property
-    def max_solutions(self):
-        return self._max_solutions
+class Model(interface.Model):
+    def __init__(self, problem=None, *args, **kwargs):
 
-    @max_solutions.setter
-    def max_solutions(self, value):
-        self._max_solutions = value
-        if getattr(self, 'problem', None) is not None:
-            if value is not None:
-                self.problem.problem.max_solutions = value
+        super(Model, self).__init__(*args, **kwargs)
 
-    @property
-    def relax(self):
-        return self._relax
+        if problem is None:
+            self.problem = cplex.Cplex()
 
-    @relax.setter
-    def relax(self, value):
-        self._relax = value
+        elif isinstance(problem, cplex.Cplex):
+            self.problem = problem
+            zipped_var_args = zip(self.problem.variables.get_names(),
+                                  self.problem.variables.get_lower_bounds(),
+                                  self.problem.variables.get_upper_bounds()
+            )
+            for name, lb, ub in zipped_var_args:
+                var = Variable(name, lb=lb, ub=ub, problem=self)
+                super(Model, self)._add_variable(var)  # This avoids adding the variable to the glpk problem
+            zipped_constr_args = zip(self.problem.linear_constraints.get_names(),
+                                     self.problem.linear_constraints.get_rows(),
+                                     self.problem.linear_constraints.get_senses(),
+                                     self.problem.linear_constraints.get_rhs()
 
-    @property
-    def emphasis(self):
-        return self._emphasis
+            )
+            variables = self.variables
+            for name, row, sense, rhs in zipped_constr_args:
+                constraint_variables = [variables[i - 1] for i in row.ind]
+                lhs = _unevaluated_Add(*[val * variables[i - 1] for i, val in zip(row.ind, row.val)])
+                if isinstance(lhs, int):
+                    lhs = sympy.Integer(lhs)
+                elif isinstance(lhs, float):
+                    lhs = sympy.RealNumber(lhs)
+                if sense == 'E':
+                    constr = Constraint(lhs, lb=rhs, ub=rhs, name=name, problem=self)
+                elif sense == 'G':
+                    constr = Constraint(lhs, lb=rhs, name=name, problem=self)
+                elif sense == 'L':
+                    constr = Constraint(lhs, ub=rhs, name=name, problem=self)
+                elif sense == 'R':
+                    range_val = self.problem.linear_constraints.get_rhs(name)
+                    if range_val > 0:
+                        constr = Constraint(lhs, lb=rhs, ub=rhs + range_val, name=name, problem=self)
+                    else:
+                        constr = Constraint(lhs, lb=rhs + range_val, ub=rhs, name=name, problem=self)
+                else:
+                    raise Exception('%s is not a recognized constraint sense.' % sense)
+
+                for variable in constraint_variables:
+                    try:
+                        self._variables_to_constraints_mapping[variable.name].add(name)
+                    except KeyError:
+                        self._variables_to_constraints_mapping[variable.name] = set([name])
+
+                super(Model, self)._add_constraint(
+                    constr,
+                    sloppy=True
+                )
+            try:
+                objective_name = self.problem.objective.get_name()
+            except cplex.exceptions.CplexSolverError as e:
+                if 'CPLEX Error  1219:' not in str(e):
+                    raise e
+            else:
+                self._objective = Objective(
+                    _unevaluated_Add(*[_unevaluated_Mul(sympy.RealNumber(coeff), variables[index]) for index, coeff in
+                                       enumerate(self.problem.objective.get_linear()) if coeff != 0.]),
+                    problem=self,
+                    direction={self.problem.objective.sense.minimize: 'min', self.problem.objective.sense.maximize: 'max'}[
+                        self.problem.objective.get_sense()],
+                    name=objective_name
+                )
+        else:
+            raise Exception("Provided problem is not a valid CPLEX model.")
+        self.configuration = Configuration(problem=self, verbosity=0)
 
-    @emphasis.setter
-    def emphasis(self, value):
-        self._emphasis = value
-        if getattr(self, 'problem', None) is not None:
-            self.problem.problem.emphasis = value
+    def __getstate__(self):
+        tmp_file = tempfile.mktemp(suffix=".sav")
+        self.problem.write(tmp_file)
+        cplex_binary = open(tmp_file, 'rb').read()
+        repr_dict = {'cplex_binary': cplex_binary, 'status': self.status, 'config': self.configuration}
+        return repr_dict
+
+    def __setstate__(self, repr_dict):
+        tmp_file = tempfile.mktemp(suffix=".sav")
+        open(tmp_file, 'wb').write(repr_dict['cplex_binary'])
+        problem = cplex.Cplex(tmp_file)
+        if repr_dict['status'] == 'optimal':
+            # turn off logging completely, get's configured later
+            problem.set_error_stream(None)
+            problem.set_warning_stream(None)
+            problem.set_log_stream(None)
+            problem.set_results_stream(None)
+            problem.solve()  # since the start is an optimal solution, nothing will happen here
+        self.__init__(problem=problem)
+        self.configuration = Configuration.clone(repr_dict['config'], problem=self)
 
     @property
-    def cuts(self):
-        return self._cuts
+    def objective(self):
+        return self._objective
 
-    @cuts.setter
-    def cuts(self, value):
-        self._cuts = value
-        if getattr(self, 'problem', None) is not None:
-            self.problem.problem.cuts = value
+    @objective.setter
+    def objective(self, value):
+        super(Model, self.__class__).objective.fset(self, value)
+        for i in range(len(self.problem.objective.get_linear())):
+            self.problem.objective.set_linear(i, 0.)
+        expression = self._objective.expression
+        if isinstance(expression, float) or isinstance(expression, int) or expression.is_Number:
+            pass
+        else:
+            if expression.is_Symbol:
+                self.problem.objective.set_linear(expression.name, 1.)
+            if expression.is_Mul:
+                coeff, var = expression.args
+                self.problem.objective.set_linear(var.name, float(coeff))
+            elif expression.is_Add:
+                for term in expression.args:
+                    coeff, var = term.args
+                    self.problem.objective.set_linear(var.name, float(coeff))
+            else:
+                raise ValueError(
+                    "Provided objective %s doesn't seem to be appropriate." %
+                    self._objective)
+            self.problem.objective.set_sense(
+                {'min': self.problem.objective.sense.minimize, 'max': self.problem.objective.sense.maximize}[
+                    value.direction])
+        self.problem.objective.set_name(value.name)
+        value.problem = self
 
     @property
-    def threads(self):
-        return self._threads
-
-    @threads.setter
-    def threads(self, value):
-        self._threads = value
-        if getattr(self, 'problem', None) is not None:
-            self.problem.problem.threads = value
-
-    def __getstate__(self):
-        return {
-            'presolve': self.presolve,
-            'timeout': self.timeout,
-            'verbosity': self.verbosity,
-            'max_nodes': self.max_nodes,
-            'max_solutions': self.max_solutions,
-            'relax': self.relax,
-            'emphasis': self.emphasis,
-            'cuts': self.cuts,
-            'threads': self.threads,
-            'tolerances': {
-                'feasibility': self.tolerances.feasibility,
-                'optimality': self.tolerances.optimality,
-                'integrality': self.tolerances.integrality
-                }
-            }
-
-    def __setstate__(self, state):
-        for key, val in six.iteritems(state):
-            if key != 'tolerances':
-                setattr(self, key, val)
-        # TODO: remove if check before final merge. Only here for backwards
-        #       compatability for current pickle files stored in cobrapy
-        if 'tolerances' in state:
-            for key, val in six.iteritems(state['tolerances']):
-                if key in self._tolerance_functions():
-                    setattr(self.tolerances, key, val)
-
-    def _get_feasibility(self):
-        return self.problem.problem.infeas_tol
-
-    def _set_feasibility(self, value):
-        self.problem.problem.infeas_tol = value
-
-    def _get_integrality(self):
-        return self.problem.problem.integer_tol
-
-    def _set_integrality(self, value):
-        self.problem.problem.integer_tol = value
-
-    def _get_optimality(self):
-        return self.problem.problem.max_mip_gap_abs
-
-    def _set_optimality(self, value):
-        self.problem.problem.max_mip_gap_abs = value
-
-    def _tolerance_functions(self):
-        return {
-            # 1e-6. Tightening this value can increase the numerical precision
-            # but also probably increasethe running time. As floating point
-            # computations always involve some loss of precision, values too
-            # close to zero will likely render some models impossible to optimize.
-            'feasibility': (
-                self._get_feasibility,
-                self._set_feasibility
-            ),
-            # Tolerance for the quality of the optimal solution, if a solution with
-            # cost c and a lower bound b are available and c - b < mip_gap_abs,
-            # the search will be concluded
-            'optimality': (
-                self._get_optimality,
-                self._set_optimality
-            ),
-            # Maximum distance to the nearest integer for a variable to be
-            # considered with an integervalue. Default value: 1e-6. Tightening
-            # this value can increase the numerical precision but also probably
-            # increase the running time. As floating point computations always
-            # involve someloss of precision, values too close to zero will likely
-            # render some models impossible to optimize.
-            'integrality': (
-                self._get_integrality,
-                self._set_integrality
-            )
-        }
-
+    def primal_values(self):
+        if self.problem:
+            primal_values = collections.OrderedDict()
+            for variable, primal in zip(self.variables, self.problem.solution.get_values()):
+                primal_values[variable.name] = variable._round_primal_to_bounds(primal)
+            return primal_values
+        else:
+            return None
 
-@six.add_metaclass(inheritdocstring)
-class Model(interface.Model):
+    @property
+    def reduced_costs(self):
+        if self.problem:
+            return collections.OrderedDict(
+                zip([variable.name for variable in self.variables], self.problem.solution.get_reduced_costs()))
+        else:
+            return None
 
-    def _initialize_problem(self):
-        self.problem = mip.Model(solver_name=mip.CBC)
+    @property
+    def dual_values(self):
+        if self.problem:
+            return collections.OrderedDict(
+                zip([constraint.name for constraint in self.constraints], self.problem.solution.get_activity_levels()))
+        else:
+            return None
 
-    def _initialize_model_from_problem(self, problem):
-        if not isinstance(problem, mip.Model):
-            raise TypeError('Problem must be an instance of mip.Model, not ' + repr(type(problem)))
-
-        # Set problem
-        self.problem = problem
-
-        self.variables.clear()
-        # Set variables
-        for v in problem.vars:
-            self.variables.append(Variable(name=v.name[2:],
-                                           lb=to_bound(v.lb),
-                                           ub=to_bound(v.ub),
-                                           type=_MIP_VTYPE_TO_VTYPE[v.var_type],
-                                           problem=self))
-
-        self.constraints.clear()
-        # Set constraints
-        for c in problem.constrs:
-            name, suffix = c.name[2:-6], c.name[-6:]
-            if name not in self.constraints:
-                expr = sum(coef * self.variables[var.name[2:]]
-                           for var, coef in c.expr.expr.items())
-                if suffix == '_lower':
-                    expr *= -1
-                self.constraints.append(Constraint(expr, name=name, problem=self))
+    @property
+    def shadow_prices(self):
+        if self.problem:
+            return collections.OrderedDict(
+                zip([constraint.name for constraint in self.constraints], self.problem.solution.get_dual_values()))
+        else:
+            return None
 
-            if suffix == '_lower':
-                self.constraints[name].lb = to_bound(-1*c.rhs)
-            else:
-                self.constraints[name].ub = to_bound(c.rhs)
 
-        # Set objective
-        terms = sum(coef * self.variables[var.name[2:]]
-                    for var, coef in problem.objective.expr.items())
-        self._objective = Objective(terms + problem.objective.const,
-                              direction=_MIP_DIR_TO_DIR[problem.sense],
-                              problem=self)
-
-    def _var_primal(self, name):
-        primal = self.problem.var_by_name('v_' + name).x
-        return 0. if primal is None else primal
-
-    def _var_dual(self, name):
-        dual = self.problem.var_by_name('v_' + name).rc
-        return 0. if dual is None else dual
-
-    def _get_primal_values(self):
-        if getattr(self, '_status', '') == 'optimal':
-            return super(Model, self)._get_primal_values()
-        return [0. for _ in self.variables]
-
-    def _get_reduced_costs(self):
-        if getattr(self, '_status', '') == 'optimal':
-            return super(Model, self)._get_reduced_costs()
-        return [0. for _ in self.variables]
-
-    def _update_var_lb(self, name, lb):
-        self.problem.var_by_name('v_' + name).lb = to_float(lb, True)
-
-    def _update_var_ub(self, name, ub):
-        self.problem.var_by_name('v_' + name).ub = to_float(ub, False)
-
-    def _update_var_type(self, name, var_type):
-        self.problem.var_by_name('v_' + name).var_type = var_type
-
-    def _add_variables(self, variables):
-        super(Model, self)._add_variables(variables)
-        for var in variables:
-            # TODO: may need to handle obj, column options
-            self.problem.add_var(name='v_' + var.name,
-                                 var_type=_VTYPE_TO_MIP_VTYPE[var.type],
-                                 lb=to_float(var.lb, True),
-                                 ub=to_float(var.ub, False))
+    def __str__(self):
+        tmp_file = tempfile.mktemp(suffix=".lp")
+        self.problem.write(tmp_file)
+        cplex_form = open(tmp_file).read()
+        return cplex_form
+
+    def optimize(self):
+        self.problem.solve()
+        cplex_status = self.problem.solution.get_status()
+        self._status = _CPLEX_STATUS_TO_STATUS[cplex_status]
+        return self.status
+
+    @staticmethod
+    def _cplex_sense_to_sympy(sense, translation=None):
+        if not translation: translation = {'E': '==', 'L': '<', 'G': '>'}
+        try:
+            return translation[sense]
+        except KeyError as e:
+            raise Exception(' '.join(('Sense', sense, 'is not a proper relational operator, e.g. >, <, == etc.')))
+
+    def _add_variable(self, variable):
+        super(Model, self)._add_variable(variable)
+        if variable.lb is None:
+            lb = -cplex.infinity
+        else:
+            lb = variable.lb
+        if variable.ub is None:
+            ub = cplex.infinity
+        else:
+            ub = variable.ub
+        vtype = _VTYPE_TO_CPLEX_VTYPE[variable.type]
+        if vtype == 'C':  # this is needed because CPLEX will automatically set the problem_type to MILP if types are specified
+            self.problem.variables.add([0.], lb=[lb], ub=[ub], names=[variable.name])
+        else:
+            self.problem.variables.add([0.], lb=[lb], ub=[ub], types=[vtype], names=[variable.name])
+        variable.problem = self
+        return variable
 
     def _remove_variables(self, variables):
-        # TODO: optimization for removing all variables?
-        if self.objective is not None:
-            self.objective._changed_expression.update({var: 0 for var in variables})
-        mip_vars = []
-        for var in variables:
-            name = var.name
-            del self._variables_to_constraints_mapping[name]
-            var.problem = None
-            del self._variables[name]
-            mip_vars.append(self.problem.var_by_name('v_' + name))
-        self.problem.remove(mip_vars)
-
-    def _constr_primal(self, con, is_lb):
-        slack = self.problem.constr_by_name(con.constraint_name(is_lb)).slack
-        return con.lb + slack if is_lb else con.ub - slack
-
-    def _constr_dual(self, con, is_lb):
-        return self.problem.constr_by_name(con.constraint_name(is_lb)).pi
-
-    def _get_constraint_values(self):
-        if getattr(self, '_status', '') == 'optimal':
-            return super(Model, self)._get_constraint_values()
-        return [0. for _ in self.constraints]
-
-    def _get_shadow_prices(self):
-        if getattr(self, '_status', '') == 'optimal':
-            return super(Model, self)._get_shadow_prices()
-        return [0. for _ in self.constraints]
-
-    def _update_constraint_bound(self, con, is_lb):
-        name = con.constraint_name(is_lb)
-        constr = self.problem.constr_by_name(name)
-        constr.rhs = to_float(-1*con.lb if is_lb else con.ub)
-
-    def _expr_to_mip_expr(self, expr):
-        """Parses mip linear expression from expression."""
-        if hasattr(expr, "expression") and symbolics.USE_SYMENGINE:
-            expr._expression = expr.expression.expand()
-        offset, coeffs, _ = parse_optimization_expression(expr)
-        return offset + mip.xsum(to_float(coef) * self.problem.var_by_name('v_' + var.name)
-                                 for var, coef in coeffs.items())
-
-    def _remove_mip_constraint(self, con, is_lb):
-        name = con.constraint_name(is_lb)
-        constr = self.problem.constr_by_name(name)
-        if constr is not None:
-            self.problem.remove(constr)
-
-    def _add_mip_constraint(self, con, is_lb=True, constr=None):
-        # Optimization for precomputing the parsed constr expression
-        if constr is None:
-            constr = self._expr_to_mip_expr(con)
-
-        # TODO: check if mip supports indicator_variable
-        name = con.constraint_name(is_lb)
-        if is_lb and con.lb is not None:
-           self.problem.add_constr(-constr <= -con.lb, name)
-        elif not is_lb and con.ub is not None:
-            self.problem.add_constr(constr <= con.ub, name)
-
-    def _add_constraints(self, constraints, sloppy=False):
-        super(Model, self)._add_constraints(constraints, sloppy=sloppy)
-        for con in constraints:
-            constr = self._expr_to_mip_expr(con)
-            # Attempt to add lb and ub constraints
-            self._add_mip_constraint(con, True, constr)
-            self._add_mip_constraint(con, False, constr)
-
-    def _remove_constraints(self, constraints):
-        not_removed = True
-        if len(constraints) > 350:  # Need to figure out a good threshold here
-            keys = map(lambda c: c.name, constraints)
-            self._constraints = self._constraints.fromkeys(set(self._constraints.keys()).difference(set(keys)))
-            not_removed = False
-
-        cons = []
-        for con in constraints:
-
-            if not_removed:
-                try:
-                    del self._constraints[con.name]
-                except KeyError:
-                    raise LookupError("Constraint %s not in solver" % con)
-                con.problem = None
-
-            cl = self.problem.constr_by_name(con.constraint_name(True))
-            cu = self.problem.constr_by_name(con.constraint_name(False))
-            if cl is not None:
-                cons.append(cl)
-            if cu is not None:
-                cons.append(cu)
-
-        self.problem.remove(cons)
-
-    def _optimize(self):
-        if self.configuration.relax:
-            self.problem.relax()
-            self._initialize_model_from_problem(self.problem)
-
-        status = self.problem.optimize()
-        # TODO: make more robust. See glpk_interface.py
-        return _MIP_STATUS_TO_STATUS[status]
-
-    @interface.Model.objective.setter
-    def objective(self, value):
-        super(Model, Model).objective.fset(self, value)
-        self.update()
-        self.problem.objective = self._expr_to_mip_expr(value)
-        self.problem.sense = _DIR_TO_MIP_DIR[value.direction]
-        value.problem = self
+        # Not calling parent method to avoid expensive variable removal from sympy expressions
+        self.problem.variables.delete([variable.name for variable in variables])
+        for variable in variables:
+            del self._variables_to_constraints_mapping[variable.name]
+            variable.problem = None
+            del self.variables[variable.name]
+
+    def _add_constraint(self, constraint, sloppy=False):
+        super(Model, self)._add_constraint(constraint, sloppy=sloppy)
+        constraint._problem = None
+        if constraint.is_Linear:
+            if constraint.expression.is_Add:
+                coeff_dict = constraint.expression.as_coefficients_dict()
+                indices = [var.name for var in coeff_dict.keys()]
+                values = [float(val) for val in coeff_dict.values()]
+            elif constraint.expression.is_Mul:
+                variable = list(constraint.expression.atoms(sympy.Symbol))[0]
+                indices = [variable.name]
+                values = [float(constraint.expression.coeff(variable))]
+            elif constraint.expression.is_Atom:
+                indices = [constraint.expression.name]
+                values = [1.]
+            else:
+                raise ValueError('Something is fishy with constraint %s' % constraint)
 
-    def __copy__(self):
-        cls = self.__class__
-        result = cls.__new__(cls)
-        result.__dict__.update(self.__dict__)
-        return result
-
-    def to_lp(self):
-        self.update()
-
-        lp_form = ('Maximize' if self.problem.sense == mip.MAXIMIZE else 'Minimize') + '\n'
-        for i, (var, coef) in enumerate(self.problem.objective.expr.items()):
-            if i == 0:
-                lp_form += f'OBJROW: {coef} {var.name}'
+            sense, rhs, range_value = _constraint_lb_and_ub_to_cplex_sense_rhs_and_range_value(constraint.lb, constraint.ub)
+            if constraint.indicator_variable is None:
+                self.problem.linear_constraints.add(
+                    lin_expr=[cplex.SparsePair(ind=indices, val=values)], senses=[sense], rhs=[rhs],
+                    range_values=[range_value], names=[constraint.name])
             else:
-                sign = '+' if coef > 0 else '-'
-                lp_form += f' {sign} {abs(coef)} {var.name}'
+                if sense == 'R':
+                    raise ValueError('CPLEX does not support indicator constraints that have both an upper and lower bound.')
+                else:
+                    self.problem.indicator_constraints.add(
+                        lin_expr=cplex.SparsePair(ind=indices, val=values), sense=sense, rhs=rhs, name=constraint.name,
+                        indvar=constraint.indicator_variable.name, complemented=abs(constraint.active_when)-1)
+        # TODO: Implement quadratic constraints
+        elif constraint.is_Quadratic:
+            raise NotImplementedError('Quadratic constraints (like %s) are not supported yet.' % constraint)
+        else:
+            raise ValueError("CPLEX only supports linear or quadratic constraints. %s is neither linear nor quadratic." % constraint)
+        constraint.problem = self
+        return constraint
 
-        lp_form += '\nSubject To\n'
-        for con in self.problem.constrs:
-            lp_form += f'{con}\n'
-
-        lp_form += 'Bounds\n'
-        for v in self.problem.vars:
-            lp_form += f'{v.lb} <= {v} <= {v.ub}\n'
-        lp_form += 'End\n'
-
-        return lp_form
-
-    @classmethod
-    def from_lp(cls, lp_form):
-        problem = mip.Model(solver_name=mip.CBC)
-        with TemporaryFilename(suffix=".lp", content=lp_form) as tmp_file_name:
-            problem.read(tmp_file_name)
-        model = cls(problem=problem)
-        return model
+    def _remove_constraints(self, constraints):
+        super(Model, self)._remove_constraints(constraints)
+        for constraint in constraints:
+            if constraint.is_Linear:
+                self.problem.linear_constraints.delete(constraint.name)
+            elif constraint.is_Quadratic:
+                self.problem.quadratic_constraints.delete(constraint.name)
+
+
+if __name__ == '__main__':
+
+    from optlang.cplex_interface import Model, Variable, Constraint, Objective
+
+    x1 = Variable('x1', lb=0)
+    x2 = Variable('x2', lb=0)
+    x3 = Variable('x3', lb=0)
+    c1 = Constraint(x1 + x2 + x3, ub=100, name='c1')
+    c2 = Constraint(10 * x1 + 4 * x2 + 5 * x3, ub=600, name='c2')
+    c3 = Constraint(2 * x1 + 2 * x2 + 6 * x3, ub=300, name='c3')
+    obj = Objective(10 * x1 + 6 * x2 + 4 * x3, direction='max')
+    model = Model(name='Simple model')
+    model.objective = obj
+    model.add([c1, c2, c3])
+    print(model)
+    status = model.optimize()
+    print("status:", model.status)
+    print("objective value:", model.objective.value)
+
+    for var_name, var in model.variables.items():
+        print(var_name, "=", var.primal)
+
+
+        # from cplex import Cplex
+        # problem = Cplex()
+        # problem.read("../tests/data/model.lp")
+
+        # solver = Model(problem=problem)
+        # print solver
+        # solver.optimize()
+        # print solver.objective.value
+        # solver.add(z)
+        # solver.add(constr)
+        # # print solver
+        # print solver.optimize()
+        # print solver.objective
```

### Comparing `optlang-1.7.0/src/optlang/glpk_interface.py` & `optlang-v0.2.1/optlang/glpk_interface.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,46 +10,45 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-"""
-Interface for the GNU Linear Programming Kit (GLPK).
+"""Interface for the GNU Linear Programming Kit (GLPK)
 
 Wraps the GLPK solver by subclassing and extending :class:`Model`,
 :class:`Variable`, and :class:`Constraint` from :mod:`interface`.
-
-GLPK is an open source LP solver, with MILP capabilities.
-To use GLPK you need to install the 'swiglpk' python package (with pip or from http://github.com/biosustain/swiglpk)
-and make sure that 'import swiglpk' runs without error.
 """
-import logging
 
 import six
+import collections
 
-from optlang.util import inheritdocstring, TemporaryFilename
-from optlang.expression_parsing import parse_optimization_expression
-from optlang import interface
-from optlang import symbolics
+import tempfile
+import sympy
+from sympy.core.add import _unevaluated_Add
+from sympy.core.mul import _unevaluated_Mul
+
+import logging
+log = logging.getLogger(__name__)
 
 from swiglpk import glp_find_col, glp_get_col_prim, glp_get_col_dual, GLP_CV, GLP_IV, GLP_BV, GLP_UNDEF, GLP_FEAS, \
     GLP_INFEAS, GLP_NOFEAS, GLP_OPT, GLP_UNBND, \
     glp_set_col_kind, glp_find_row, glp_get_row_prim, glp_get_row_dual, glp_get_obj_val, glp_set_obj_dir, glp_init_smcp, \
     glp_init_iocp, GLP_MIN, GLP_MAX, glp_iocp, glp_smcp, GLP_ON, GLP_OFF, GLP_MSG_OFF, GLP_MSG_ERR, GLP_MSG_ON, \
     GLP_MSG_ALL, glp_term_out, glp_create_index, glp_create_prob, glp_get_num_rows, glp_get_num_cols, glp_get_col_name, \
-    glp_get_col_lb, glp_get_col_ub, glp_get_col_kind, glp_set_prob_name, glp_read_prob, glp_set_obj_coef, glp_simplex, \
-    glp_intopt, glp_get_status, glp_add_cols, \
+    glp_get_col_lb, glp_get_col_ub, glp_get_col_kind, glp_set_prob_name, glp_read_prob, glp_copy_prob, \
+    glp_set_obj_coef, glp_simplex, glp_intopt, glp_get_status, glp_add_cols, \
     glp_set_col_name, intArray, glp_del_cols, glp_add_rows, glp_set_row_name, doubleArray, glp_write_lp, glp_write_prob, \
     glp_set_mat_row, glp_set_col_bnds, glp_set_row_bnds, GLP_FR, GLP_UP, GLP_LO, GLP_FX, GLP_DB, glp_del_rows, \
     glp_get_mat_row, glp_get_row_ub, glp_get_row_type, glp_get_row_lb, glp_get_row_name, glp_get_obj_coef, \
-    glp_get_obj_dir, glp_scale_prob, GLP_SF_AUTO, glp_get_num_int, glp_mip_col_val, \
-    glp_mip_obj_val, glp_mip_status, GLP_ETMLIM, glp_adv_basis, glp_read_lp, glp_mip_row_val, \
-    get_col_primals, get_col_duals, get_row_primals, get_row_duals
+    glp_get_obj_dir, glp_scale_prob, GLP_SF_AUTO, glp_get_num_int, glp_get_num_bin, glp_version, glp_mip_col_val, \
+    glp_mip_obj_val, glp_mip_status, GLP_ETMLIM
+
+from optlang import interface
 
 
 _GLPK_STATUS_TO_STATUS = {
     GLP_UNDEF: interface.UNDEFINED,
     GLP_FEAS: interface.FEASIBLE,
     GLP_INFEAS: interface.INFEASIBLE,
     GLP_NOFEAS: interface.INFEASIBLE,
@@ -63,143 +62,130 @@
     GLP_BV: 'binary'
 }
 
 _VTYPE_TO_GLPK_VTYPE = dict(
     [(val, key) for key, val in six.iteritems(_GLPK_VTYPE_TO_VTYPE)]
 )
 
-log = logging.getLogger(__name__)
-
 
-def _glpk_validate_id(name):
-    if name is None:
-        return
-    if len(name) > 256:
-        raise ValueError("GLPK does not support ID's longer than 256 characters")
-
-
-@six.add_metaclass(inheritdocstring)
 class Variable(interface.Variable):
+    """..."""
+
     def __init__(self, name, index=None, *args, **kwargs):
-        _glpk_validate_id(name)
         super(Variable, self).__init__(name, **kwargs)
 
     @property
-    def _index(self):
-        if self.problem is not None:
+    def index(self):
+        try:
             i = glp_find_col(self.problem.problem, str(self.name))
             if i != 0:
                 return i
             else:
                 raise IndexError(
-                    "Could not determine column index for variable %s" % self)
-        else:
+                    "Could not determine row index for variable %s" % self)
+        except:
             return None
 
     @interface.Variable.lb.setter
     def lb(self, value):
         interface.Variable.lb.fset(self, value)
-        if self.problem is not None:
-            self.problem._glpk_set_col_bounds(self)
+        self.problem._glpk_set_col_bounds(self)
 
     @interface.Variable.ub.setter
     def ub(self, value):
         interface.Variable.ub.fset(self, value)
-        if self.problem is not None:
-            self.problem._glpk_set_col_bounds(self)
-
-    def set_bounds(self, lb, ub):
-        super(Variable, self).set_bounds(lb, ub)
-        if self.problem is not None:
-            self.problem._glpk_set_col_bounds(self)
+        self.problem._glpk_set_col_bounds(self)
 
     @interface.Variable.type.setter
     def type(self, value):
         try:
             glpk_kind = _VTYPE_TO_GLPK_VTYPE[value]
         except KeyError:
-            raise ValueError(
-                "GLPK cannot handle variables of type %s. The following variable types are available:\n" +
-                " ".join(_VTYPE_TO_GLPK_VTYPE.keys())
-            )
-        if self.problem is not None:
-            glp_set_col_kind(self.problem.problem, self._index, glpk_kind)
+            raise Exception("GLPK cannot handle variables of type %s. \
+                        The following variable types are available:\n" +
+                            " ".join(_VTYPE_TO_GLPK_VTYPE.keys()))
+        glp_set_col_kind(self.problem.problem, self.index, glpk_kind)
         interface.Variable.type.fset(self, value)
 
-    def _get_primal(self):
-        if self.problem._glpk_is_mip():
-            primal_from_solver = glp_mip_col_val(self.problem.problem, self._index)
+    @property
+    def primal(self):
+        if self.problem:
+            if self.type == "continuous":
+                primal_from_solver = glp_get_col_prim(self.problem.problem, self.index)
+            elif self.type in ["binary", "integer"]:
+                primal_from_solver = glp_mip_col_val(self.problem.problem, self.index)
+            else:
+                raise TypeError("Unknown variable type")
+            return self._round_primal_to_bounds(primal_from_solver)
         else:
-            primal_from_solver = glp_get_col_prim(self.problem.problem, self._index)
-        return primal_from_solver
+            return None
 
     @property
     def dual(self):
         if self.problem:
-            if self.problem.is_integer:
-                raise ValueError("Dual values are not well-defined for integer problems")
-            return glp_get_col_dual(self.problem.problem, self._index)
+            return glp_get_col_dual(self.problem.problem, self.index)
         else:
             return None
 
-    @interface.Variable.name.setter
-    def name(self, value):
-        old_name = getattr(self, "name", None)
-        super(Variable, Variable).name.fset(self, value)
-        _glpk_validate_id(value)
-        if getattr(self, 'problem', None) is not None:
-            glp_set_col_name(self.problem.problem, glp_find_col(self.problem.problem, old_name), str(value))
+    def __setattr__(self, name, value):
+        try:
+            old_name = self.name  # TODO: This is a hack
+        except AttributeError:
+            pass
+        super(Variable, self).__setattr__(name, value)
+        if getattr(self, 'problem', None):
+            if name == 'name':
+                glp_set_col_name(self.problem.problem, glp_find_col(self.problem.problem, old_name), str(value))
 
 
-@six.add_metaclass(inheritdocstring)
 class Constraint(interface.Constraint):
+    """GLPK solver interface"""
+
     _INDICATOR_CONSTRAINT_SUPPORT = False
 
     def __init__(self, expression, sloppy=False, *args, **kwargs):
-        _glpk_validate_id(kwargs.get("name", "GoodName"))
         super(Constraint, self).__init__(expression, sloppy=sloppy, *args, **kwargs)
         if not sloppy:
             if not self.is_Linear:
                 raise ValueError(
                     "GLPK only supports linear constraints. %s is not linear." % self)
 
     def _get_expression(self):
         if self.problem is not None:
             col_num = glp_get_num_cols(self.problem.problem)
             ia = intArray(col_num + 1)
             da = doubleArray(col_num + 1)
-            nnz = glp_get_mat_row(self.problem.problem, self._index, ia, da)
-            constraint_variables = [self.problem._variables[glp_get_col_name(self.problem.problem, ia[i])] for i in
+            nnz = glp_get_mat_row(self.problem.problem, self.index, ia, da)
+            # variables = self.problem.variables
+            # constraint_variables = [variables[ia[i] - 1] for i in range(1, nnz + 1)]
+            constraint_variables = [self.problem.variables[glp_get_col_name(self.problem.problem, ia[i])] for i in
                                     range(1, nnz + 1)]
-            expression = symbolics.add(
-                [symbolics.mul((symbolics.Real(da[i]), constraint_variables[i - 1])) for i in
+            expression = sympy.Add._from_args(
+                [sympy.Mul._from_args((sympy.RealNumber(da[i]), constraint_variables[i - 1])) for i in
                  range(1, nnz + 1)])
             self._expression = expression
         return self._expression
 
-    @interface.Constraint.lb.setter
-    def lb(self, value):
-        super(Constraint, Constraint).lb.fset(self, value)
-        if self.problem is not None:
-            self.problem._glpk_set_row_bounds(self)
-
-    @interface.Constraint.ub.setter
-    def ub(self, value):
-        super(Constraint, Constraint).ub.fset(self, value)
-        if self.problem is not None:
-            self.problem._glpk_set_row_bounds(self)
-
-    @interface.OptimizationExpression.name.setter
-    def name(self, value):
-        _glpk_validate_id(value)
-        old_name = getattr(self, 'name', None)
-        super(Constraint, Constraint).name.fset(self, value)
-        self._name = value
+    def _set_coefficients_low_level(self, variables_coefficients_dict):
         if self.problem is not None:
-            glp_set_row_name(self.problem.problem, glp_find_row(self.problem.problem, old_name), str(value))
+            problem = self.problem.problem
+            indices_coefficients_dict = dict([(variable.index, coefficient) for variable, coefficient in six.iteritems(variables_coefficients_dict)])
+            num_cols = glp_get_num_cols(problem)
+            ia = intArray(num_cols + 1)
+            da = doubleArray(num_cols + 1)
+            index = self.index
+            num = glp_get_mat_row(self.problem.problem, index, ia, da)
+            for i in range(1, num +1):
+                try:
+                    da[i] = indices_coefficients_dict[ia[i]]
+                except KeyError:
+                    pass
+            print(glp_set_mat_row(self.problem.problem, index, num, ia, da))
+        else:
+            raise Exception('_set_coefficients_low_level works only if a constraint is associated with a solver instance.')
 
     @property
     def problem(self):
         return self._problem
 
     @problem.setter
     def problem(self, value):
@@ -207,214 +193,191 @@
             # Update expression from solver instance one last time
             self._get_expression()
             self._problem = None
         else:
             self._problem = value
 
     @property
-    def _index(self):
+    def index(self):
         try:
             i = glp_find_row(self.problem.problem, str(self.name))
             if i != 0:
                 return i
             else:
                 raise IndexError(
                     "Could not determine row index for variable %s" % self)
-        except Exception:  # TODO Change to specific exception type
+        except:
             return None
 
     @property
     def primal(self):
         if self.problem is not None:
-            if self.problem._glpk_is_mip():
-                primal_from_solver = glp_mip_row_val(self.problem.problem, self._index)
-            else:
-                primal_from_solver = glp_get_row_prim(self.problem.problem, self._index)
-            # return self._round_primal_to_bounds(primal_from_solver)  # Test assertions fail
-            return primal_from_solver
+            return glp_get_row_prim(self.problem.problem, self.index)
         else:
             return None
 
     @property
     def dual(self):
         if self.problem is not None:
-            if self.problem.is_integer:
-                raise ValueError("Dual values are not well-defined for integer problems")
-            return glp_get_row_dual(self.problem.problem, self._index)
+            return glp_get_row_dual(self.problem.problem, self.index)
         else:
             return None
 
+    @property
+    def problem(self):
+        return self._problem
+
+    @problem.setter
+    def problem(self, value):
+        if value is None:
+            # Update expression from solver instance one last time
+            self._get_expression()
+            self._problem = None
+        else:
+            self._problem = value
+
+    def __setattr__(self, name, value):
+        try:
+            old_name = self.name  # TODO: This is a hack
+        except AttributeError:
+            pass
+        super(Constraint, self).__setattr__(name, value)
+        if getattr(self, 'problem', None):
+            if name == 'name':
+                glp_set_row_name(self.problem.problem, glp_find_row(self.problem.problem, old_name), str(value))
+            elif name == 'lb' or name == 'ub':
+                self.problem._glpk_set_row_bounds(self)
+
     def __iadd__(self, other):
+        # if self.problem is not None:
+        # self.problem._add_to_constraint(self.index, other)
         if self.problem is not None:
             problem_reference = self.problem
             self.problem._remove_constraint(self)
             super(Constraint, self).__iadd__(other)
             problem_reference._add_constraint(self, sloppy=False)
         else:
             super(Constraint, self).__iadd__(other)
         return self
 
-    def set_linear_coefficients(self, coefficients):
+    def __isub__(self, other):
+        super(Constraint, self).__isub__(other)
         if self.problem is not None:
-            problem = self.problem.problem
-            self.problem.update()
-
-            num_cols = glp_get_num_cols(problem)
-
-            ia = intArray(num_cols + 1)
-            va = doubleArray(num_cols + 1)
-
-            num_rows = glp_get_mat_row(self.problem.problem, self._index, ia, va)
-            variables_and_coefficients = {var.name: coeff for var, coeff in six.iteritems(coefficients)}
-
-            final_variables_and_coefficients = {
-                glp_get_col_name(problem, ia[i]): va[i] for i in range(1, num_rows + 1)
-            }
-            final_variables_and_coefficients.update(variables_and_coefficients)
-
-            ia = intArray(num_cols + 1)
-            va = doubleArray(num_cols + 1)
-
-            for i, (name, coeff) in enumerate(six.iteritems(final_variables_and_coefficients)):
-                ia[i + 1] = self.problem._variables[name]._index
-                va[i + 1] = float(coeff)
+            problem_reference = self.problem
+            self.problem._remove_constraint(self)
+            problem_reference._add_constraint(self, sloppy=False)
+        return self
 
-            glp_set_mat_row(problem, self._index, len(final_variables_and_coefficients), ia, va)
-        else:
-            raise Exception("Can't change coefficients if constraint is not associated with a model.")
+    def __imul__(self, other):
+        super(Constraint, self).__imul__(other)
+        if self.problem is not None:
+            problem_reference = self.problem
+            self.problem._remove_constraint(self)
+            problem_reference._add_constraint(self, sloppy=False)
+        return self
 
-    def get_linear_coefficients(self, variables):
+    def __idiv__(self, other):
+        super(Constraint, self).__idiv__(other)
         if self.problem is not None:
-            self.problem.update()
-            num_cols = glp_get_num_cols(self.problem.problem)
-            ia = intArray(num_cols + 1)
-            da = doubleArray(num_cols + 1)
-            nnz = glp_get_mat_row(self.problem.problem, self._index, ia, da)
-            coefs = dict.fromkeys(variables, 0.0)
-            coefs.update({
-                self.problem._variables[ia[i + 1] - 1]: da[i + 1]
-                for i in range(nnz)
-                if self.problem._variables[ia[i + 1] - 1] in variables})
-            return coefs
-        else:
-            raise Exception("Can't get coefficients from solver if constraint is not in a model")
+            problem_reference = self.problem
+            self.problem._remove_constraint(self)
+            problem_reference._add_constraint(self, sloppy=False)
+        return self
 
 
-@six.add_metaclass(inheritdocstring)
 class Objective(interface.Objective):
-    def __init__(self, expression, sloppy=False, **kwargs):
-        if len(kwargs.get("name", "")) > 256:
-            raise ValueError("GLPK does not support ID's longer than 256 characters")
-        super(Objective, self).__init__(expression, sloppy=sloppy, **kwargs)
-        self._expression_expired = False
-        if not (sloppy or self.is_Linear):
+    def __init__(self, *args, **kwargs):
+        super(Objective, self).__init__(*args, **kwargs)
+        if not self.is_Linear:
             raise ValueError(
                 "GLPK only supports linear objectives. %s is not linear." % self)
 
     def _get_expression(self):
-        if self.problem is not None and self._expression_expired:
-            variables = self.problem._variables
-
+        if self.problem is not None:
+            variables = self.problem.variables
             def term_generator():
                 for index in range(1, glp_get_num_cols(self.problem.problem) + 1):
                     coeff = glp_get_obj_coef(self.problem.problem, index)
                     if coeff != 0.:
-                        yield (symbolics.Real(coeff), variables[index - 1])
-
-            expression = symbolics.add([symbolics.mul(term) for term in term_generator()])
-            self._expression = expression + getattr(self.problem, "_objective_offset", 0)
-            self._expression_expired = False
+                        yield (sympy.RealNumber(coeff), variables[index - 1])
+            expression = sympy.Add._from_args([sympy.Mul._from_args(term) for term in term_generator()])
+            self._expression = expression
         return self._expression
 
     @property
     def value(self):
-        if getattr(self, 'problem', None) is not None:
-            offset = getattr(self.problem, '_objective_offset', 0)
-            if self.problem._glpk_is_mip():
-                return glp_mip_obj_val(self.problem.problem) + offset
-            else:
-                return glp_get_obj_val(self.problem.problem) + offset
+        if (glp_get_num_int(self.problem.problem) + glp_get_num_bin(self.problem.problem)) > 0:
+            return glp_mip_obj_val(self.problem.problem)
         else:
-            return None
+            return glp_get_obj_val(self.problem.problem)
 
-    @interface.Objective.direction.setter
-    def direction(self, value):
-        if getattr(self, 'problem', None) is not None:
-            glp_set_obj_dir(self.problem.problem, {'min': GLP_MIN, 'max': GLP_MAX}[value])
-        super(Objective, Objective).direction.__set__(self, value)
+    def __setattr__(self, name, value):
+
+        if getattr(self, 'problem', None):
+            if name == 'direction':
+                glp_set_obj_dir(self.problem.problem,
+                                {'min': GLP_MIN, 'max': GLP_MAX}[value])
+            super(Objective, self).__setattr__(name, value)
+        else:
+            super(Objective, self).__setattr__(name, value)
 
     def __iadd__(self, other):
         self.problem = None
         super(Objective, self).__iadd__(other)
         if self.problem is not None:
             self.problem.objective = self
         return self
 
-    def __imul__(self, other):
+    def __isub__(self, other):
         self.problem = None
-        super(Objective, self).__imul__(other)
+        super(Objective, self).__isub__(other)
         if self.problem is not None:
             self.problem.objective = self
         return self
 
-    def set_linear_coefficients(self, coefficients):
+    def __imul__(self, other):
+        self.problem = None
+        super(Objective, self).__imul__(other)
         if self.problem is not None:
-            self.problem.update()
-            for variable, coefficient in coefficients.items():
-                glp_set_obj_coef(self.problem.problem, variable._index, float(coefficient))
-            self._expression_expired = True
-        else:
-            raise Exception("Can't change coefficients if objective is not associated with a model.")
+            self.problem.objective = self
+        return self
 
-    def get_linear_coefficients(self, variables):
+    def __idiv__(self, other):
+        self.problem = None
+        super(Objective, self).__idiv__(other)
         if self.problem is not None:
-            self.problem.update()
-            return {var: glp_get_obj_coef(self.problem.problem, var._index) for var in variables}
-        else:
-            raise Exception("Can't get coefficients from solver if objective is not in a model")
+            self.problem.objective = self
+        return self
 
 
-@six.add_metaclass(inheritdocstring)
 class Configuration(interface.MathematicalProgrammingConfiguration):
-    def __init__(self, presolve="auto", verbosity=0, timeout=None, *args, **kwargs):
+    """docstring for Configuration"""
+
+    def __init__(self, presolve=False, verbosity=0, timeout=None, *args, **kwargs):
         super(Configuration, self).__init__(*args, **kwargs)
         self._smcp = glp_smcp()
         self._iocp = glp_iocp()
         glp_init_smcp(self._smcp)
         glp_init_iocp(self._iocp)
         self._max_time = min(self._smcp.tm_lim, self._iocp.tm_lim)
         self.presolve = presolve
         self.verbosity = verbosity
         self.timeout = timeout
-        if "tolerances" in kwargs:
-            for key, val in six.iteritems(kwargs["tolerances"]):
-                try:
-                    setattr(self.tolerances, key, val)
-                except AttributeError:
-                    pass
 
     def __getstate__(self):
-        return {'presolve': self.presolve,
-                'verbosity': self.verbosity,
-                'timeout': self.timeout,
-                'tolerances': {"feasibility": self.tolerances.feasibility}
-                }
+        return {'presolve': self.presolve, 'verbosity': self.verbosity, 'timeout': self.timeout}
 
     def __setstate__(self, state):
         self.__init__()
         for key, val in six.iteritems(state):
-            if key != "tolerances":
-                setattr(self, key, val)
-        for key, val in six.iteritems(state["tolerances"]):
-            if key in self._tolerance_functions():
-                setattr(self.tolerances, key, val)
+            setattr(self, key, val)
 
     def _set_presolve(self, value):
-        self._smcp.presolve = {False: GLP_OFF, True: GLP_ON, "auto": GLP_OFF}[value]
-        self._iocp.presolve = {False: GLP_OFF, True: GLP_ON, "auto": GLP_ON}[value]
+        self._smcp.presolve = {False: GLP_OFF, True: GLP_ON}[value]
+        self._iocp.presolve = {False: GLP_OFF, True: GLP_ON}[value]
 
     def _set_verbosity(self, value):
         if value == 0:
             glp_term_out(GLP_OFF)
             self._smcp.msg_lev = GLP_MSG_OFF
             self._iocp.msg_lev = GLP_MSG_OFF
         elif value == 1:
@@ -426,45 +389,27 @@
             self._smcp.msg_lev = GLP_MSG_ON
             self._iocp.msg_lev = GLP_MSG_ON
         elif value == 3:
             glp_term_out(GLP_ON)
             self._smcp.msg_lev = GLP_MSG_ALL
             self._iocp.msg_lev = GLP_MSG_ALL
         else:
-            raise ValueError(
+            raise Exception(
                 "%s is not a valid verbosity level ranging between 0 and 3."
                 % value
             )
 
     def _set_timeout(self, value):
         if value is None:
             self._smcp.tm_lim = self._max_time
             self._iocp.tm_lim = self._max_time
         else:
             self._smcp.tm_lim = value * 1000  # milliseconds to seconds
             self._iocp.tm_lim = value * 1000
 
-    def _get_feasibility(self):
-        return getattr(self._smcp, "tol_bnd")
-
-    def _set_feasibility(self, value):
-        return setattr(self._smcp, "tol_bnd", value)
-
-    def _get_integrality(self):
-        return getattr(self._iocp, "tol_int")
-
-    def _set_integrality(self, value):
-        return setattr(self._iocp, "tol_int", value)
-
-    def _tolerance_functions(self):
-        return {
-            "feasibility": (self._get_feasibility, self._set_feasibility),
-            "integrality": (self._get_integrality, self._set_integrality)
-        }
-
     @property
     def presolve(self):
         return self._presolve
 
     @presolve.setter
     def presolve(self, value):
         self._set_presolve(value)
@@ -484,200 +429,229 @@
         return self._timeout
 
     @timeout.setter
     def timeout(self, value):
         self._set_timeout(value)
         self._timeout = value
 
-
-@six.add_metaclass(inheritdocstring)
 class Model(interface.Model):
-    def _initialize_problem(self):
-        self.problem = glp_create_prob()
-        glp_create_index(self.problem)
-        if self.name is not None:
-            _glpk_validate_id(self.name)
-            glp_set_prob_name(self.problem, str(self.name))
-
-    def _initialize_model_from_problem(self, problem):
-        try:
-            self.problem = problem
-            glp_create_index(self.problem)
-        except TypeError:
-            raise TypeError("Provided problem is not a valid GLPK model.")
-        row_num = glp_get_num_rows(self.problem)
-        col_num = glp_get_num_cols(self.problem)
-        for i in range(1, col_num + 1):
-            var = Variable(
-                glp_get_col_name(self.problem, i),
-                lb=glp_get_col_lb(self.problem, i),
-                ub=glp_get_col_ub(self.problem, i),
-                problem=self,
-                type=_GLPK_VTYPE_TO_VTYPE[
-                    glp_get_col_kind(self.problem, i)]
-            )
-            # This avoids adding the variable to the glpk problem
-            super(Model, self)._add_variables([var])
-        variables = self.variables
+    """GLPK solver interface"""
 
-        for j in range(1, row_num + 1):
-            ia = intArray(col_num + 1)
-            da = doubleArray(col_num + 1)
-            nnz = glp_get_mat_row(self.problem, j, ia, da)
-            constraint_variables = [variables[ia[i] - 1] for i in range(1, nnz + 1)]
+    def __init__(self, problem=None, *args, **kwargs):
 
-            # Since constraint expressions are lazily retrieved from the solver they don't have to be built here
-            # lhs = _unevaluated_Add(*[da[i] * constraint_variables[i - 1]
-            #                         for i in range(1, nnz + 1)])
-            lhs = 0
-
-            glpk_row_type = glp_get_row_type(self.problem, j)
-            if glpk_row_type == GLP_FX:
-                row_lb = glp_get_row_lb(self.problem, j)
-                row_ub = row_lb
-            elif glpk_row_type == GLP_LO:
-                row_lb = glp_get_row_lb(self.problem, j)
-                row_ub = None
-            elif glpk_row_type == GLP_UP:
-                row_lb = None
-                row_ub = glp_get_row_ub(self.problem, j)
-            elif glpk_row_type == GLP_DB:
-                row_lb = glp_get_row_lb(self.problem, j)
-                row_ub = glp_get_row_ub(self.problem, j)
-            elif glpk_row_type == GLP_FR:
-                row_lb = None
-                row_ub = None
-            else:
-                raise Exception(
-                    "Currently, optlang does not support glpk row type %s"
-                    % str(glpk_row_type)
-                )
-                log.exception()
-            if isinstance(lhs, int):
-                lhs = symbolics.Integer(lhs)
-            elif isinstance(lhs, float):
-                lhs = symbolics.Real(lhs)
-            constraint_id = glp_get_row_name(self.problem, j)
-            for variable in constraint_variables:
-                try:
-                    self._variables_to_constraints_mapping[variable.name].add(constraint_id)
-                except KeyError:
-                    self._variables_to_constraints_mapping[variable.name] = set([constraint_id])
+        super(Model, self).__init__(*args, **kwargs)
 
-            super(Model, self)._add_constraints(
-                [Constraint(lhs, lb=row_lb, ub=row_ub, name=constraint_id, problem=self, sloppy=True)],
-                sloppy=True
-            )
+        self.configuration = Configuration()
 
-        term_generator = (
-            (glp_get_obj_coef(self.problem, index), variables[index - 1])
-            for index in range(1, glp_get_num_cols(problem) + 1)
-        )
-        self._objective = Objective(
-            symbolics.add(
-                [symbolics.mul((symbolics.Real(term[0]), term[1])) for term in term_generator if
-                 term[0] != 0.]
-            ),
-            problem=self,
-            direction={GLP_MIN: 'min', GLP_MAX: 'max'}[glp_get_obj_dir(self.problem)])
+        if problem is None:
+            self.problem = glp_create_prob()
+            glp_create_index(self.problem)
+            if self.name is not None:
+                glp_set_prob_name(self.problem, str(self.name))
 
-    @classmethod
-    def from_lp(cls, lp_form):
-        problem = glp_create_prob()
-        with TemporaryFilename(suffix=".lp", content=lp_form) as tmp_file_name:
-            glp_read_lp(problem, None, tmp_file_name)
-        model = cls(problem=problem)
-        return model
+        else:
+            try:
+                self.problem = problem
+                glp_create_index(self.problem)
+            except TypeError:
+                raise TypeError("Provided problem is not a valid GLPK model.")
+            row_num = glp_get_num_rows(self.problem)
+            col_num = glp_get_num_cols(self.problem)
+            for i in range(1, col_num + 1):
+                var = Variable(
+                    glp_get_col_name(self.problem, i),
+                    lb=glp_get_col_lb(self.problem, i),
+                    ub=glp_get_col_ub(self.problem, i),
+                    problem=self,
+                    type=_GLPK_VTYPE_TO_VTYPE[
+                        glp_get_col_kind(self.problem, i)]
+                )
+                # This avoids adding the variable to the glpk problem
+                super(Model, self)._add_variable(var)
+            variables = self.variables
+
+            for j in range(1, row_num + 1):
+                ia = intArray(col_num + 1)
+                da = doubleArray(col_num + 1)
+                nnz = glp_get_mat_row(self.problem, j, ia, da)
+                constraint_variables = [variables[ia[i] - 1] for i in range(1, nnz + 1)]
+                lhs = _unevaluated_Add(*[da[i] * constraint_variables[i - 1]
+                                         for i in range(1, nnz + 1)])
+                glpk_row_type = glp_get_row_type(self.problem, j)
+                if glpk_row_type == GLP_FX:
+                    row_lb = glp_get_row_lb(self.problem, j)
+                    row_ub = row_lb
+                elif glpk_row_type == GLP_LO:
+                    row_lb = glp_get_row_lb(self.problem, j)
+                    row_ub = None
+                elif glpk_row_type == GLP_UP:
+                    row_lb = None
+                    row_ub = glp_get_row_ub(self.problem, j)
+                elif glpk_row_type == GLP_DB:
+                    row_lb = glp_get_row_lb(self.problem, j)
+                    row_ub = glp_get_row_ub(self.problem, j)
+                elif glpk_row_type == GLP_FR:
+                    row_lb = None
+                    row_ub = None
+                else:
+                    raise Exception(
+                        "Currently, optlang does not support glpk row type %s"
+                        % str(glpk_row_type)
+                    )
+                    log.exception()
+                if isinstance(lhs, int):
+                    lhs = sympy.Integer(lhs)
+                elif isinstance(lhs, float):
+                    lhs = sympy.RealNumber(lhs)
+                constraint_id = glp_get_row_name(self.problem, j)
+                for variable in constraint_variables:
+                    try:
+                        self._variables_to_constraints_mapping[variable.name].add(constraint_id)
+                    except KeyError:
+                        self._variables_to_constraints_mapping[variable.name] = set([constraint_id])
+
+                super(Model, self)._add_constraint(
+                    Constraint(lhs, lb=row_lb, ub=row_ub, name=constraint_id, problem=self), sloppy=True)
+
+            term_generator = (
+                (glp_get_obj_coef(self.problem, index), variables[index - 1])
+                for index in range(1, glp_get_num_cols(problem) + 1)
+            )
+            self._objective = Objective(
+                _unevaluated_Add(
+                    *[_unevaluated_Mul(sympy.RealNumber(term[0]), term[1]) for term in term_generator if
+                      term[0] != 0.]),
+                problem=self,
+                direction={GLP_MIN: 'min', GLP_MAX:
+                    'max'}[glp_get_obj_dir(self.problem)]
+            )
+        glp_scale_prob(self.problem, GLP_SF_AUTO)
 
     def __getstate__(self):
         glpk_repr = self._glpk_representation()
         repr_dict = {'glpk_repr': glpk_repr, 'glpk_status': self.status, 'config': self.configuration}
         return repr_dict
 
     def __setstate__(self, repr_dict):
-        with TemporaryFilename(suffix=".glpk", content=repr_dict["glpk_repr"]) as tmp_file_name:
-            problem = glp_create_prob()
-            code = glp_read_prob(problem, 0, tmp_file_name)
-            if code != 0:
-                with open(tmp_file_name) as tmp_file:
-                    invalid_problem = tmp_file.read()
-                raise Exception("The GLPK file " + tmp_file_name +
-                                " does not seem to contain a valid GLPK problem:\n\n" +
-                                invalid_problem)
+        tmp_file = tempfile.mktemp(suffix=".glpk")
+        open(tmp_file, 'w').write(repr_dict['glpk_repr'])
+        problem = glp_create_prob()
+        glp_read_prob(problem, 0, tmp_file)
         self.__init__(problem=problem)
         self.configuration = Configuration.clone(repr_dict['config'], problem=self)
         if repr_dict['glpk_status'] == 'optimal':
             self.optimize()  # since the start is an optimal solution, nothing will happen here
 
-    # def __del__(self):  # To make sure that the glpk problem is deleted when this is garbage collected
-    # Gotcha: When objects with a __del__ method are part of a referencing cycle, the entire
-    #         cycle is never automatically garbage collected
-    #     glp_delete_prob(self.problem)
+    # def __copy__(self):
+    #     return Model(problem=self.problem)
+    #
+    # def __deepcopy__(self, memo):
+    #     copy_problem = glp_create_prob()
+    #     glp_copy_prob(copy_problem, self.problem, GLP_ON)
+    #     return Model(problem=copy_problem)
 
     @property
     def objective(self):
         return self._objective
 
     @objective.setter
     def objective(self, value):
-        value.problem = None
+        value.problem = None  # TODO: temporary fix to allow for objectives that already have a problem set
         if self._objective is not None:
-            variables = self.objective.variables
-            for variable in variables:
-                if variable._index is not None:
-                    glp_set_obj_coef(self.problem, variable._index, 0.)
+            for variable in self.objective.variables:
+                if variable.index is not None:
+                    glp_set_obj_coef(self.problem, variable.index, 0.)
         super(Model, self.__class__).objective.fset(self, value)
-        self.update()
+        expression = self._objective._expression
+        if isinstance(expression, float) or isinstance(expression, int) or expression.is_Number:
+            pass
+        else:
+            if expression.is_Symbol:
+                glp_set_obj_coef(self.problem, expression.index, 1.)
+            if expression.is_Mul:
+                coeff, var = expression.args
+                glp_set_obj_coef(self.problem, var.index, float(coeff))
+            elif expression.is_Add:
+                for term in expression.args:
+                    coeff, var = term.args
+                    glp_set_obj_coef(self.problem, var.index, float(coeff))
+            else:
+                raise ValueError(
+                    "Provided objective %s doesn't seem to be appropriate." %
+                    self._objective)
+            glp_set_obj_dir(
+                self.problem,
+                {'min': GLP_MIN, 'max': GLP_MAX}[self._objective.direction]
+            )
+        value.problem = self
 
-        offset, coef_dict, _ = parse_optimization_expression(value, linear=True)
-        self._objective_offset = offset
+    @property
+    def primal_values(self):
+        if self.problem:
+            primal_values = collections.OrderedDict()
+            for index, variable in enumerate(self.variables):
+                if variable.type == "continuous":
+                    value = glp_get_col_prim(self.problem, index+1)
+                elif variable.type in ["binary", "integer"]:
+                    value = glp_mip_col_val(self.problem, index+1)
+                else:
+                    raise TypeError("Unknown variable type")
+                primal_values[variable.name] = variable._round_primal_to_bounds(value)
+            return primal_values
+        else:
+            return None
 
-        for var, coef in coef_dict.items():
-            glp_set_obj_coef(self.problem, var._index, float(coef))
+    @property
+    def reduced_costs(self):
+        if self.problem:
+            reduced_costs = collections.OrderedDict()
+            for index, variable in enumerate(self.variables):
+                if variable.type == "continuous":
+                    value = glp_get_col_dual(self.problem, index+1)
+                elif variable.type in ["binary", "integer"]:
+                    value = glp_mip_col_val(self.problem, index+1)
+                else:
+                    raise TypeError("Unknown variable type")
+                reduced_costs[variable.name] = value
+            return reduced_costs
+        else:
+            return None
 
-        glp_set_obj_dir(
-            self.problem,
-            {'min': GLP_MIN, 'max': GLP_MAX}[self._objective.direction]
-        )
-        value.problem = self
+    @property
+    def dual_values(self):
+        if self.problem:
+            dual_values = collections.OrderedDict()
+            for index, constraint in enumerate(self.constraints):
+                value = glp_get_row_prim(self.problem, index+1)
+                dual_values[constraint.name] = value
+            return dual_values
+        else:
+            return None
 
-    def _get_primal_values(self):
-        return get_col_primals(self.problem)
+    @property
+    def shadow_prices(self):
+        if self.problem:
+            shadow_prices = collections.OrderedDict()
+            for index, constraint in enumerate(self.constraints):
+                value = glp_get_row_dual(self.problem, index+1)
+                shadow_prices[constraint.name] = value
+            return shadow_prices
+        else:
+            return None
 
-    def _get_reduced_costs(self):
-        if self.is_integer:
-            raise ValueError("Dual values are not well-defined for integer problems")
-        return get_col_duals(self.problem)
-
-    def _get_constraint_values(self):
-        return get_row_primals(self.problem)
-
-    def _get_shadow_prices(self):
-        if self.is_integer:
-            raise ValueError("Dual values are not well-defined for integer problems")
-        return get_row_duals(self.problem)
-
-    def to_lp(self):
-        self.update()
-        with TemporaryFilename(suffix=".lp") as tmp_file_name:
-            code = glp_write_lp(self.problem, None, tmp_file_name)
-            if code != 0:
-                raise Exception("GLPK could not successfully create the LP.")
-            with open(tmp_file_name) as tmp_file:
-                lp_form = tmp_file.read()
-        return lp_form
+    def __str__(self):
+        tmp_file = tempfile.mktemp(suffix=".lp")
+        glp_write_lp(self.problem, None, tmp_file)
+        cplex_form = open(tmp_file).read()
+        return cplex_form
 
     def _glpk_representation(self):
-        self.update()
-        with TemporaryFilename(suffix=".glpk") as tmp_file_name:
-            code = glp_write_prob(self.problem, 0, tmp_file_name)
-            if code != 0:
-                raise Exception("GLPK could not successfully create the GLPK file.")
-            with open(tmp_file_name, "r") as tmp_file:
-                glpk_form = tmp_file.read()
+        tmp_file = tempfile.mktemp(suffix=".glpk")
+        glp_write_prob(self.problem, 0, tmp_file)
+        glpk_form = open(tmp_file).read()
         return glpk_form
 
     def _run_glp_simplex(self):
         return_value = glp_simplex(self.problem, self.configuration._smcp)
         glpk_status = glp_get_status(self.problem)
         if return_value == 0:
             status = _GLPK_STATUS_TO_STATUS[glpk_status]
@@ -698,161 +672,188 @@
             status = interface.TIME_LIMIT
         else:
             status = _GLPK_STATUS_TO_STATUS[glpk_status]
             if status == interface.UNDEFINED:
                 log.debug("Status undefined. GLPK status code returned by glp_intopt was %d" % return_value)
         return status
 
-    def _optimize(self):
-        glp_scale_prob(self.problem, GLP_SF_AUTO)
+    def optimize(self):
         status = self._run_glp_simplex()
 
-        # Sometimes GLPK gets itself stuck with an invalid basis. This will help it get rid of it.
-        if status == interface.UNDEFINED and self.configuration.presolve is not True:
-            glp_adv_basis(self.problem, 0)
-            status = self._run_glp_simplex()
-
-        if status == interface.UNDEFINED and self.configuration.presolve is True:
-            # If presolve is on, status will be undefined if not optimal
-            self.configuration.presolve = False
-            status = self._run_glp_simplex()
+        if status == interface.UNDEFINED or status == interface.INFEASIBLE:
+            # Let's see if the presolver and some scaling can fix this issue
+            glp_scale_prob(self.problem, GLP_SF_AUTO)
+            original_presolve_setting = self.configuration.presolve
             self.configuration.presolve = True
-        if self._glpk_is_mip():
+            status = self._run_glp_simplex()
+            self.configuration.presolve = original_presolve_setting
+        if (glp_get_num_int(self.problem) + glp_get_num_bin(self.problem)) > 0:
             status = self._run_glp_mip()
             if status == 'undefined' or status == 'infeasible':
                 # Let's see if the presolver and some scaling can fix this issue
+                glp_scale_prob(self.problem, GLP_SF_AUTO)
                 original_presolve_setting = self.configuration.presolve
                 self.configuration.presolve = True
                 status = self._run_glp_mip()
                 self.configuration.presolve = original_presolve_setting
+        self._status = status
         return status
 
-    def _add_variables(self, variables):
-        for variable in variables:
-            glp_add_cols(self.problem, 1)
-            index = glp_get_num_cols(self.problem)
-            glp_set_col_name(self.problem, index, str(variable.name))
-            variable.problem = self
-            self._glpk_set_col_bounds(variable)
-            glp_set_col_kind(self.problem, variable._index, _VTYPE_TO_GLPK_VTYPE[variable.type])
-        super(Model, self)._add_variables(variables)
+    def _add_variable(self, variable):
+        super(Model, self)._add_variable(variable)
+        glp_add_cols(self.problem, 1)
+        index = glp_get_num_cols(self.problem)
+        glp_set_col_name(self.problem, index, str(variable.name))
+        variable.problem = self
+        self._glpk_set_col_bounds(variable)
+        glp_set_col_kind(self.problem, variable.index, _VTYPE_TO_GLPK_VTYPE[variable.type])
+        return variable
 
     def _remove_variables(self, variables):
         if len(variables) > 0:
+
             if len(variables) > 350:
-                delete_indices = [variable._index - 1 for variable in variables]
-                keep_indices = [i for i in range(0, len(self._variables)) if i not in delete_indices]
-                self._variables = self._variables.fromkeys(keep_indices)
+                delete_indices = [variable.index - 1 for variable in variables]
+                keep_indices = [i for i in range(0, len(self.variables)) if i not in delete_indices]
+                self._variables = self.variables.fromkeys(keep_indices)
             else:
                 for variable in variables:
-                    del self._variables[variable.name]
+                    del self.variables[variable.name]
 
             num = intArray(len(variables) + 1)
             for i, variable in enumerate(variables):
-                num[i + 1] = variable._index
+                num[i + 1] = variable.index
             glp_del_cols(self.problem, len(variables), num)
 
             for variable in variables:
                 del self._variables_to_constraints_mapping[variable.name]
                 variable.problem = None
 
-    def _add_constraints(self, constraints, sloppy=False):
-        super(Model, self)._add_constraints(constraints, sloppy=sloppy)
-        for constraint in constraints:
-            constraint._problem = None  # This needs to be done in order to not trigger constraint._get_expression()
-            glp_add_rows(self.problem, 1)
-            index = glp_get_num_rows(self.problem)
-            glp_set_row_name(self.problem, index, str(constraint.name))
-            num_cols = glp_get_num_cols(self.problem)
-            index_array = intArray(num_cols + 1)
-            value_array = doubleArray(num_cols + 1)
-            num_vars = 0  # constraint.variables is too expensive for large problems
-
-            offset, coef_dict, _ = parse_optimization_expression(constraint, linear=True)
-
-            num_vars = len(coef_dict)
-            for i, (var, coef) in enumerate(coef_dict.items()):
-                index_array[i + 1] = var._index
-                value_array[i + 1] = float(coef)
-
-            glp_set_mat_row(self.problem, index, num_vars,
-                            index_array, value_array)
-            constraint._problem = self
-            self._glpk_set_row_bounds(constraint)
+    # def _add_constraints_low_level(self, variable_ids, coefficients, lb=None, ub=None):
+    #     glp_add_rows(self.problem, len(variable_ids))
+    #     index = glp_get_num_rows(self.problem)
+    #     glp_set_row_name(self.problem, index, constraint.name)
+    #     num_vars = len(constraint.variables)
+    #     index_array = intArray(num_vars + 1)
+    #     value_array = doubleArray(num_vars + 1)
+
+    def _add_constraint(self, constraint, sloppy=False):
+        super(Model, self)._add_constraint(constraint, sloppy=sloppy)
+        constraint._problem = None  # This needs to be dones in order to not trigger constraint._get_expression()
+        glp_add_rows(self.problem, 1)
+        index = glp_get_num_rows(self.problem)
+        glp_set_row_name(self.problem, index, str(constraint.name))
+        num_cols = glp_get_num_cols(self.problem)
+        index_array = intArray(num_cols + 1)
+        value_array = doubleArray(num_cols + 1)
+        num_vars = 0  # constraint.variables is too expensive for large problems
+        if constraint.expression.is_Atom and constraint.expression.is_Symbol:
+            var = constraint.expression
+            index_array[1] = var.index
+            value_array[1] = 1
+            num_vars += 1
+        elif constraint.expression.is_Mul:
+            args = constraint.expression.args
+            if len(args) > 2:
+                raise Exception(
+                    "Term(s) %s from constraint %s is not a proper linear term." % (args, constraint))
+            coeff = float(args[0])
+            var = args[1]
+            index_array[1] = var.index
+            value_array[1] = coeff
+            num_vars += 1
+        else:
+            for i, term in enumerate(constraint.expression.args):
+                args = term.args
+                if args == ():
+                    assert term.is_Symbol
+                    coeff = 1
+                    var = term
+                elif len(args) == 2:
+                    assert args[0].is_Number
+                    assert args[1].is_Symbol
+                    var = args[1]
+                    coeff = float(args[0])
+                elif len(args) > 2:
+                    raise Exception(
+                        "Term %s from constraint %s is not a proper linear term." % (term, constraint))
+                index_array[i + 1] = var.index
+                value_array[i + 1] = coeff
+                num_vars += 1
+        glp_set_mat_row(self.problem, index, num_vars,
+                        index_array, value_array)
+        constraint._problem = self
+        self._glpk_set_row_bounds(constraint)
 
     def _glpk_set_col_bounds(self, variable):
         if variable.lb is None and variable.ub is None:
             # 0.'s are ignored
-            glp_set_col_bnds(self.problem, variable._index, GLP_FR, 0., 0.)
+            glp_set_col_bnds(self.problem, variable.index, GLP_FR, 0., 0.)
         elif variable.lb is None:
             # 0. is ignored
-            glp_set_col_bnds(self.problem, variable._index,
+            glp_set_col_bnds(self.problem, variable.index,
                              GLP_UP, 0., float(variable.ub))
         elif variable.ub is None:
             # 0. is ignored
-            glp_set_col_bnds(self.problem, variable._index,
+            glp_set_col_bnds(self.problem, variable.index,
                              GLP_LO, float(variable.lb), 0.)
         elif variable.lb == variable.ub:
-            glp_set_col_bnds(self.problem, variable._index,
+            glp_set_col_bnds(self.problem, variable.index,
                              GLP_FX, float(variable.lb), float(variable.lb))
         elif variable.lb < variable.ub:
-            glp_set_col_bnds(self.problem, variable._index,
+            glp_set_col_bnds(self.problem, variable.index,
                              GLP_DB, float(variable.lb), float(variable.ub))
         elif variable.lb > variable.ub:
             raise ValueError(
                 "Lower bound %f is larger than upper bound %f in variable %s" %
                 (variable.lb, variable.ub, variable))
         else:
             raise Exception(
                 "Something is wrong with the provided bounds %f and %f in variable %s" %
                 (variable.lb, variable.ub, variable))
 
-    def _glpk_is_mip(self):
-        return glp_get_num_int(self.problem) > 0
-
-    @property
-    def is_integer(self):
-        return self._glpk_is_mip()
-
     def _glpk_set_row_bounds(self, constraint):
         if constraint.lb is None and constraint.ub is None:
             # 0.'s are ignored
-            glp_set_row_bnds(self.problem, constraint._index, GLP_FR, 0., 0.)
+            glp_set_row_bnds(self.problem, constraint.index, GLP_FR, 0., 0.)
         elif constraint.lb is None:
             # 0. is ignored
-            glp_set_row_bnds(self.problem, constraint._index,
+            glp_set_row_bnds(self.problem, constraint.index,
                              GLP_UP, 0., float(constraint.ub))
         elif constraint.ub is None:
             # 0. is ignored
-            glp_set_row_bnds(self.problem, constraint._index,
+            glp_set_row_bnds(self.problem, constraint.index,
                              GLP_LO, float(constraint.lb), 0.)
         elif constraint.lb == constraint.ub:
-            glp_set_row_bnds(self.problem, constraint._index,
+            glp_set_row_bnds(self.problem, constraint.index,
                              GLP_FX, float(constraint.lb), float(constraint.lb))
         elif constraint.lb < constraint.ub:
-            glp_set_row_bnds(self.problem, constraint._index,
+            glp_set_row_bnds(self.problem, constraint.index,
                              GLP_DB, float(constraint.lb), float(constraint.ub))
         elif constraint.lb > constraint.ub:
             raise ValueError(
                 "Lower bound %f is larger than upper bound %f in constraint %s" %
                 (constraint.lb, constraint.ub, constraint))
         else:
             raise Exception(
                 "Something is wrong with the provided bounds %f and %f in constraint %s" %
                 (constraint.lb, constraint.ub, constraint))
 
     def _remove_constraints(self, constraints):
         if len(constraints) > 0:
-            constraint_indices = [constraint._index for constraint in constraints]
+            constraint_indices = [constraint.index for constraint in constraints]
             super(Model, self)._remove_constraints(constraints)
             num = intArray(len(constraints) + 1)
             for i, constraint_index in enumerate(constraint_indices):
                 num[i + 1] = constraint_index
             glp_del_rows(self.problem, len(constraints), num)
 
+    def _set_linear_objective_term(self, variable, coefficient):
+        glp_set_obj_coef(self.problem, variable.index, coefficient)
+
 
 if __name__ == '__main__':
     import pickle
 
     x1 = Variable('x1', lb=0)
     x2 = Variable('x2', lb=0)
     x3 = Variable('x3', lb=0)
@@ -868,16 +869,18 @@
     print("objective value:", model.objective.value)
 
     for var_name, var in model.variables.items():
         print(var_name, "=", var.primal)
 
     print(model)
 
+    from swiglpk import glp_read_lp
+
     problem = glp_create_prob()
-    glp_read_lp(problem, None, "tests/data/model.lp")
+    glp_read_lp(problem, None, "../tests/data/model.lp")
 
     solver = Model(problem=problem)
     print(solver.optimize())
     print(solver.objective)
 
     import time
 
@@ -885,8 +888,8 @@
     print("pickling")
     pickle_string = pickle.dumps(solver)
     resurrected_solver = pickle.loads(pickle_string)
     t2 = time.time()
     print("Execution time: %s" % (t2 - t1))
 
     resurrected_solver.optimize()
-    print("Halelujah!", resurrected_solver.objective.value)
+    print("Halelujah!", resurrected_solver.objective.value)
```

### Comparing `optlang-1.7.0/src/optlang/inspyred_interface.py` & `optlang-v0.2.1/optlang/inspyred_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,20 +16,23 @@
 
 """Interface to the inspyred heuristic optimization framework
 
 Wraps the GLPK solver by subclassing and extending :class:`Model`,
 :class:`Variable`, and :class:`Constraint` from :mod:`interface`.
 """
 
-import logging
 import random
+import logging
+
 import types
 
+
 log = logging.getLogger(__name__)
 import sympy
+import inspyred
 import interface
 
 
 class Variable(interface.Variable):
     def __init__(self, *args, **kwargs):
         super(Variable, self).__init__(*args, **kwargs)
 
@@ -199,18 +202,18 @@
     @algorithm.setter
     def algorithm(self, value):
         init = False
         try:
             previous_selector = self._algorithm.selector
             previous_variator = self._algorithm.variator
             previous_replacer = self._algorithm.replacer
-            # previous_migrator = self._algorithm.migrator
-            # previous_archiver = self._algorithm.archiver
-            # previous_observer = self._algorithm.observer
-            # previous_terminator = self._algorithm.terminator
+            previous_migrator = self._algorithm.migrator
+            previous_archiver = self._algorithm.archiver
+            previous_observer = self._algorithm.observer
+            previous_terminator = self._algorithm.terminator
         except AttributeError:
             init = True
 
         if value == "EvolutionaryComputation":
             self._algorithm = inspyred.ec.EvolutionaryComputation
         elif value == "GeneticAlgorithm" or value == "GA":
             self._algorithm = inspyred.ec.GA(random)
@@ -228,26 +231,24 @@
             self._algorithm = inspyred.emo.NSGA2(random)
         elif value == "PAES":
             self._algorithm = inspyred.emo.PAES(random)
         elif value == "Pareto":
             self._algorithm = inspyred.emo.Pareto(random)
         else:
             raise ValueError(
-                "%s is not a supported. Try one of the following instead:"
-                "'GeneticAlgorithm', 'ParticleSwarmOptimization', 'EvolutionaryStrategy'."
-                "TODO: be more specific here")
+                "%s is not a supported. Try one of the following instead: 'GeneticAlgorithm', 'ParticleSwarmOptimization', 'EvolutionaryStrategy'. TODO: be more specific here")
         # self._algorithm.terminator = self._default_terminator
         if init is False:
             self._algorithm.selector = previous_selector
             self._algorithm.variator = previous_variator
             self._algorithm.replacer = previous_replacer
-            # previous_migrator = self._algorithm.migrator
-            # previous_archiver = self._algorithm.archiver
-            # previous_observer = self._algorithm.observer
-            # previous_terminator = self._algorithm.terminator
+            previous_migrator = self._algorithm.migrator
+            previous_archiver = self._algorithm.archiver
+            previous_observer = self._algorithm.observer
+            previous_terminator = self._algorithm.terminator
             # TODO: setting a new algorithm should recycle old variators, selectors etc.
 
     def _evolve_kwargs(self):
         """Filter None keyword arguments. Intended to be passed on to algorithm.evolve(...)"""
         valid_evolve_kwargs = (
             'max_generations', 'max_evaluations', 'pop_size', 'neighborhood_size', 'tournament_size', 'mutation_rate')
         filtered_evolve_kwargs = dict()
@@ -262,14 +263,15 @@
 class Model(interface.Model):
     """Interface"""
 
     def __init__(self, algorithm=None, *args, **kwargs):
         super(Model, self).__init__(*args, **kwargs)
         self.configuration = Configuration()
         if algorithm is None:
+            # TODO: pick something smart?
             self.configuration.algorithm = "GA"
         else:
             self.configuration.algorithm = algorithm
         self._bounder = VariableBounder(self)
         self._generator = self._generator
 
     def _generator(self, random, args):
@@ -329,26 +331,25 @@
     print("The global minimum at (x,y) = (1,1) is", rosenbrock_obj.expression.subs({x: 1, y: 1}))
 
     problem = Model(name='rosenbrock', algorithm='PSO')
     # problem = Model(name='rosenbrock')
 
     problem.objective = rosenbrock_obj
 
-
     def my_observer(population, num_generations, num_evaluations, args):
         best = max(population)
         print(('{0:6} -- {1} : {2}'.format(num_generations,
-                                           best.fitness,
-                                           str(best.candidate))))
-
+                                          best.fitness,
+                                          str(best.candidate))))
 
     problem.configuration.max_generations = 100
     problem.configuration.terminator = inspyred.ec.terminators.generation_termination
     problem.configuration.observer = my_observer
     problem.configuration.selector = inspyred.ec.selectors.tournament_selection
     final_pop = problem.optimize()
     fitnesses = [individual.fitness for individual in final_pop]
     print(fitnesses)
     print("mean", numpy.mean(fitnesses))
     print("max", numpy.max(fitnesses))
     print("min", numpy.min(fitnesses))
     # print numpy.std(fitnesses)
+
```

### Comparing `optlang-1.7.0/src/optlang/osqp_interface.py` & `optlang-v0.2.1/optlang/interface.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,932 +9,880 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-"""Solver interface for the OSQP solver.
 
-Wraps the OSQP solver by subclassing and extending :class:`Model`,
-:class:`Variable`, and :class:`Constraint` from :mod:`interface`.
-
-To use this interface, install the OSQP solver and the bundled python
-interface.
-Make sure that 'import osqp' runs without error.
+"""Abstract solver interface definitions (:class:`Model`, :class:`Variable`,
+:class:`Constraint`, :class:`Objective`) intended to be subclassed and
+extended for individual solvers.
 """
+import inspect
+
 import logging
+import random
+import uuid
 import six
-import pickle
-import numpy as np
-from numpy import array, concatenate, Infinity, zeros, isnan
-
-from optlang import interface, symbolics, available_solvers
-from optlang.util import inheritdocstring
-from optlang.expression_parsing import parse_optimization_expression
-from optlang.exceptions import SolverError
 
-from scipy.sparse import csc_matrix
+import types
+import collections
 
-from optlang.symbolics import add, mul
+import sys
 
 log = logging.getLogger(__name__)
 
-try:
-    import osqp as osqp
-except ImportError:
-    try:
-        import cuosqp as osqp
+import sympy
+from sympy.core.singleton import S
+from sympy.core.logic import fuzzy_bool
+
+from .container import Container
+
+OPTIMAL = 'optimal'
+UNDEFINED = 'undefined'
+FEASIBLE = 'feasible'
+INFEASIBLE = 'infeasible'
+NOFEASIBLE = 'nofeasible'
+UNBOUNDED = 'unbounded'
+INFEASIBLE_OR_UNBOUNDED = 'infeasible_or_unbouned'
+LOADED = 'loaded'
+CUTOFF = 'cutoff'
+ITERATION_LIMIT = 'iteration_limit'
+MEMORY_LIMIT = 'memory_limit'
+NODE_LIMIT = 'node_limit'
+TIME_LIMIT = 'time_limit'
+SOLUTION_LIMIT = 'solution_limit'
+INTERRUPTED = 'interrupted'
+NUMERIC = 'numeric'
+SUBOPTIMAL = 'suboptimal'
+INPROGRESS = 'in_progress'
+ABORTED = 'aborted'
+SPECIAL = 'check_original_solver_status'
 
-        log.warning(
-            "cuOSQP is still experimental and may not work for all problems. "
-            "It may not converge as fast as the normal osqp package or not "
-            "converge at all."
-        )
-    except ImportError:
-        raise ImportError("The osqp_interface requires osqp or cuosqp!")
-
-
-_STATUS_MAP = {
-    "interrupted by user": interface.ABORTED,
-    "run time limit reached": interface.TIME_LIMIT,
-    "feasible": interface.FEASIBLE,
-    "primal infeasible": interface.INFEASIBLE,
-    "dual infeasible": interface.INFEASIBLE,
-    "primal infeasible inaccurate": interface.INFEASIBLE,
-    "dual infeasible inaccurate": interface.INFEASIBLE,
-    "solved inaccurate": interface.NUMERIC,
-    "solved": interface.OPTIMAL,
-    "maximum iterations reached": interface.ITERATION_LIMIT,
-    "unsolved": interface.SPECIAL,
-    "problem non convex": interface.SPECIAL,
-    "non-existing-status": "Here for testing that missing statuses are handled.",
-}
-
-_LP_METHODS = ("auto", "primal")
-
-_QP_METHODS = ("auto", "primal")
-
-_TYPES = ("continuous",)
-
-
-class OSQPProblem(object):
-    """A concise representation of an OSQP problem.
-
-    OSQP assumes that the problem will be pretty much immutable. This is
-    a small intermediate layer based on dictionaries that is fast to modify
-    but can also be converted to an OSQP problem without too much hassle.
+
+
+# noinspection PyShadowingBuiltins
+class Variable(sympy.Symbol):
+    """Optimization variables.
+
+    Extends sympy Symbol with optimization specific attributes and methods.
+
+    Attributes
+    ----------
+    name: str
+        The variable's name.
+    lb: float or None, optional
+        The lower bound, if None then -inf.
+    ub: float or None, optional
+        The upper bound, if None then inf.
+    type: str, optional
+        The variable type, 'continuous' or 'integer' or 'binary'.
+    problem: Model or None, optional
+        A reference to the optimization model the variable belongs to.
+
+    Examples
+    --------
+    >>> Variable('x', lb=-10, ub=10)
+    '-10 <= x <= 10'
     """
 
-    def __init__(self):
-        self.variables = set()
-        self.constraints = set()
-        self.constraint_coefs = dict()
-        self.constraint_lbs = dict()
-        self.constraint_ubs = dict()
-        self.variable_lbs = dict()
-        self.variable_ubs = dict()
-        self.obj_linear_coefs = dict()
-        self.obj_quadratic_coefs = dict()
-        self.primals = {}
-        self.cprimals = {}
-        self.duals = {}
-        self.vduals = {}
-        self.obj_value = None
-        self.direction = -1
-        self.info = None
-        self.status = None
-        self.settings = {
-            "linsys_solver": "qdldl",
-            "max_iter": 100000,
-            "eps_abs": 1e-6,
-            "eps_rel": 1e-6,
-            "eps_prim_inf": 1e-6,
-            "eps_dual_inf": 1e-6,
-            "polish": True,
-            "verbose": False,
-            "scaling": 0,
-            "time_limit": 0,
-            "adaptive_rho": True,
-            "rho": 1.0,
-            "alpha": 1.6,
-        }
-        self.__solution = None
-
-    def build(self):
-        """Build the problem instance."""
-        d = self.direction
-        vmap = dict(zip(self.variables, range(len(self.variables))))
-        nv = len(self.variables)
-        cmap = dict(zip(self.constraints, range(len(self.constraints))))
-        nc = len(self.constraints)
-        if len(self.obj_quadratic_coefs) > 0:
-            P = array(
-                [
-                    [vmap[vn[0]], vmap[vn[1]], coef * d * 2.0]
-                    for vn, coef in six.iteritems(self.obj_quadratic_coefs)
-                ]
-            )
-            P = csc_matrix(
-                (P[:, 2], (P[:, 0].astype("int64"), P[:, 1].astype("int64"))),
-                shape=(nv, nv),
-            )
-        else:
-            P = None
-        q = zeros(nv)
-        q[[vmap[vn] for vn in self.obj_linear_coefs]] = list(
-            self.obj_linear_coefs.values()
-        )
-        q = q * d
-        Av = array([[vmap[k] + nc, vmap[k], 1.0] for k in self.variables])
-        vbounds = array(
-            [[self.variable_lbs[vn], self.variable_ubs[vn]] for vn in self.variables]
-        )
-        if len(self.constraint_coefs) > 0:
-            A = array(
-                [
-                    [cmap[vn[0]], vmap[vn[1]], coef]
-                    for vn, coef in six.iteritems(self.constraint_coefs)
-                ]
-            )
-            bounds = array(
-                [
-                    [self.constraint_lbs[cn], self.constraint_ubs[cn]]
-                    for cn in self.constraints
-                ]
-            )
-            A = concatenate((A, Av))
-            bounds = concatenate((bounds, vbounds))
-        else:
-            A = Av
-            bounds = vbounds
-        if A.shape[0] == 0:
-            A = None
-        else:
-            A = csc_matrix(
-                (A[:, 2], (A[:, 0].astype("int64"), A[:, 1].astype("int64"))),
-                shape=(nc + nv, nv),
-            )
-        return P, q, A, bounds
+    @staticmethod
+    def __test_valid_lower_bound(type, value, name):
+        if value is not None:
+            if type == 'integer' and value % 1 != 0.:
+                raise ValueError(
+                    'The provided lower bound %g cannot be assigned to integer variable %s (%g mod 1 != 0).' % (
+                        value, name, value))
+        if type == 'binary' and (value is None or value != 0):
+            raise ValueError(
+                'The provided lower bound %s cannot be assigned to binary variable %s.' % (value, name))
 
-    def solve(self):
-        """Solve the OSQP problem."""
-        settings = self.settings.copy()
-        P, q, A, bounds = self.build()
-        solver = osqp.OSQP()
-        if P is None:
-            # see https://github.com/cvxgrp/cvxpy/issues/898
-            settings.update({"adaptive_rho": 0, "rho": 1.0, "alpha": 1.0})
-        solver.setup(P=P, q=q, A=A, l=bounds[:, 0], u=bounds[:, 1], **settings)  # noqa
-        if self.__solution is not None:
-            if self.still_valid(A, bounds):
-                solver.warm_start(x=self.__solution["x"], y=self.__solution["y"])
-                solver.update_settings(rho=self.__solution["rho"])
-        solution = solver.solve()
-        nc = len(self.constraints)
-        nv = len(self.variables)
-        if not solution.x[0] is None:
-            self.primals = dict(zip(self.variables, solution.x))
-            self.vduals = dict(zip(self.variables, solution.y[nc : (nc + nv)]))
-            if nc > 0:
-                self.cprimals = dict(zip(self.constraints, A.dot(solution.x)[0:nc]))
-                self.duals = dict(zip(self.constraints, solution.y[0:nc]))
-        if not isnan(solution.info.obj_val):
-            self.obj_value = solution.info.obj_val * self.direction
-            self.status = solution.info.status
-        else:
-            self.status = "primal infeasible"
-            self.obj_value = None
-        self.info = solution.info
-        self.__solution = {
-            "x": solution.x,
-            "y": solution.y,
-            "rho": solution.info.rho_estimate,
-        }
-
-    def reset(self, everything=False):
-        """Reset the public solver solution."""
-        self.info = None
-        self.primals = {}
-        self.cprimals = {}
-        self.duals = {}
-        self.vduals = {}
-        if everything:
-            self.__solution = None
-
-    def still_valid(self, A, bounds):
-        """Check if previous solutions is still feasible."""
-        if len(self.__solution["x"]) != len(self.variables) or len(
-            self.__solution["y"]
-        ) != len(self.constraints):
-            return False
-        c = A.dot(self.__solution["x"])
-        ea = self.settings["eps_abs"]
-        er = self.settings["eps_rel"]
-        valid = np.all(
-            (c + er * np.abs(c) + ea >= bounds[:, 0])
-            & (c - er * np.abs(c) - ea <= bounds[:, 1])
-        )
-        return valid
-
-    def clean(self):
-        """Remove unused variables and constraints."""
-        self.reset()
-        self.variable_lbs = {
-            k: v for k, v in six.iteritems(self.variable_lbs) if k in self.variables
-        }
-        self.variable_ubs = {
-            k: v for k, v in six.iteritems(self.variable_ubs) if k in self.variables
-        }
-        self.constraint_coefs = {
-            k: v
-            for k, v in six.iteritems(self.constraint_coefs)
-            if k[0] in self.constraints and k[1] in self.variables
-        }
-        self.obj_linear_coefs = {
-            k: v for k, v in six.iteritems(self.obj_linear_coefs) if k in self.variables
-        }
-        self.obj_quadratic_coefs = {
-            k: v
-            for k, v in six.iteritems(self.obj_quadratic_coefs)
-            if k[0] in self.variables and k[1] in self.variables
-        }
-        self.constraint_lbs = {
-            k: v for k, v in six.iteritems(self.constraint_lbs) if k in self.constraints
-        }
-        self.constraint_ubs = {
-            k: v for k, v in six.iteritems(self.constraint_ubs) if k in self.constraints
-        }
-
-    def rename_constraint(self, old, new):
-        """Rename a constraint."""
-        self.reset()
-        self.constraints.remove(old)
-        self.constraints.add(new)
-        name_map = {k: k for k in self.constraints}
-        name_map[old] = new
-        self.constraint_coefs = {
-            (name_map[k[0]], k[1]): v for k, v in six.iteritems(self.constraint_coefs)
-        }
-        self.constraint_lbs[new] = self.constraint_lbs.pop(old)
-        self.constraint_ubs[new] = self.constraint_ubs.pop(old)
-
-    def rename_variable(self, old, new):
-        """Rename a variable."""
-        self.reset()
-        self.variables.remove(old)
-        self.variables.add(new)
-        name_map = {k: k for k in self.variables}
-        name_map[old] = new
-        self.constraint_coefs = {
-            (k[0], name_map[k[1]]): v for k, v in six.iteritems(self.constraint_coefs)
-        }
-        self.obj_quadratic_coefs = {
-            (name_map[k[0]], name_map[k[1]]): v
-            for k, v in six.iteritems(self.obj_quadratic_coefs)
-        }
-        self.obj_linear_coefs = {
-            name_map[k]: v for k, v in six.iteritems(self.obj_linear_coefs)
-        }
-        self.variable_lbs[new] = self.variable_lbs.pop(old)
-        self.variable_ubs[new] = self.variable_ubs.pop(old)
-
-
-@six.add_metaclass(inheritdocstring)
-class Variable(interface.Variable):
-    def __init__(self, name, *args, **kwargs):
-        super(Variable, self).__init__(name, **kwargs)
+    @staticmethod
+    def __test_valid_upper_bound(type, value, name):
+        if value is not None:
+            if type == 'integer' and value % 1 != 0.:
+                raise ValueError(
+                    'The provided upper bound %s cannot be assigned to integer variable %s (%s mod 1 != 0).' % (
+                        value, name, value))
+        if type == 'binary' and (value is None or value != 1):
+            raise ValueError(
+                'The provided upper bound %s cannot be assigned to binary variable %s.' % (value, name))
 
-    @interface.Variable.type.setter
-    def type(self, value):
-        if self.problem is not None:
-            if value not in _TYPES:
+    @classmethod
+    def clone(cls, variable, **kwargs):
+        return cls(variable.name, lb=variable.lb, ub=variable.ub, type=variable.type, **kwargs)
+
+    def __new__(cls, name, **assumptions):
+
+        if assumptions.get('zero', False):
+            return S.Zero
+        is_commutative = fuzzy_bool(assumptions.get('commutative', True))
+        if is_commutative is None:
+            raise ValueError(
+                '''Symbol commutativity must be True or False.''')
+        assumptions['commutative'] = is_commutative
+        for key in assumptions.keys():
+            assumptions[key] = bool(assumptions[key])
+        return sympy.Symbol.__xnew__(cls, name, uuid=str(int(round(1e16*random.random()))), **assumptions) # uuid.uuid1()
+
+    def __init__(self, name, lb=None, ub=None, type="continuous", problem=None, *args, **kwargs):
+        for char in name:
+            if char.isspace():
                 raise ValueError(
-                    "OSQP cannot handle variables of type '%s'. " % value
-                    + "The following variable types are available: "
-                    + ", ".join(_TYPES)
-                )
-        super(Variable, Variable).type.fset(self, value)
+                    'Variable names cannot contain whitespace characters. "%s" contains whitespace character "%s".' % (
+                        name, char))
+        sympy.Symbol.__init__(name, *args, **kwargs)  #TODO: change this back to use super
+        self._lb = lb
+        self._ub = ub
+        if self._lb is None and type == 'binary':
+            self._lb = 0.
+        if self._ub is None and type == 'binary':
+            self._ub = 1.
+        self.__test_valid_lower_bound(type, self._lb, name)
+        self.__test_valid_upper_bound(type, self._ub, name)
+        self._type = type
+        self.problem = problem
+
+    @property
+    def lb(self):
+        return self._lb
+
+    @lb.setter
+    def lb(self, value):
+        if hasattr(self, 'ub') and self.ub is not None and value is not None and value > self.ub:
+            raise ValueError(
+                'The provided lower bound %g is larger than the upper bound %g of variable %s.' % (
+                    value, self.ub, self))
+        self.__test_valid_lower_bound(self.type, value, self.name)
+        self._lb = value
+
+    @property
+    def ub(self):
+        return self._ub
+
+    @ub.setter
+    def ub(self, value):
+        if hasattr(self, 'lb') and self.lb is not None and value is not None and value < self.lb:
+            raise ValueError(
+                'The provided upper bound %g is smaller than the lower bound %g of variable %s.' % (
+                    value, self.lb, self))
+        self.__test_valid_upper_bound(self.type, value, self.name)
+        self._ub = value
+
+    @property
+    def type(self):
+        return self._type
+
+    @type.setter
+    def type(self, value):
+        if value == 'continuous':
+            self._type = value
+        elif value == 'integer':
+            self._type = value
+            try:
+                self.lb = round(self.lb)
+            except TypeError:
+                pass
+            try:
+                self.ub = round(self.ub)
+            except TypeError:
+                pass
+        elif value == 'binary':
+            self._type = value
+            self._lb = 0
+            self._ub = 1
+        else:
+            raise ValueError(
+                "'%s' is not a valid variable type. Choose between 'continuous, 'integer', or 'binary'." % value)
 
-    def _get_primal(self):
-        return self.problem.problem.primals.get(self.name, None)
+    @property
+    def primal(self):
+        return None
 
     @property
     def dual(self):
-        if self.problem is not None:
-            return self.problem.problem.vduals.get(self.name, None)
         return None
 
-    @interface.Variable.name.setter
-    def name(self, value):
-        old_name = getattr(self, "name", None)
-        super(Variable, Variable).name.fset(self, value)
-        if getattr(self, "problem", None) is not None:
-            if old_name != value:
-                self.problem.problem.rename_variable(old_name, value)
-
-
-@six.add_metaclass(inheritdocstring)
-class Constraint(interface.Constraint):
-    _INDICATOR_CONSTRAINT_SUPPORT = False
-
-    def __init__(self, expression, sloppy=False, *args, **kwargs):
-        super(Constraint, self).__init__(expression, *args, sloppy=sloppy, **kwargs)
-
-    def set_linear_coefficients(self, coefficients):
-        if self.problem is not None:
-            self.problem.update()
-            self.problem.problem.reset()
-            for var, coef in six.iteritems(coefficients):
-                self.problem.problem.constraint_coefs[(self.name, var.name)] = float(
-                    coef
-                )
-        else:
-            raise Exception(
-                "Can't change coefficients if constraint is not associated "
-                "with a model."
-            )
+    def __str__(self):
+        """Print a string representation of variable.
 
-    def get_linear_coefficients(self, variables):
-        if self.problem is not None:
-            self.problem.update()
-            coefs = {
-                v: self.problem.problem.constraint_coefs.get((self.name, v.name), 0.0)
-                for v in variables
-            }
-            return coefs
+        Examples
+        --------
+        >>> Variable('x', lb=-10, ub=10)
+        '-10 <= x <= 10'
+        """
+        if self.lb is not None:
+            lb_str = str(self.lb) + " <= "
         else:
-            raise Exception(
-                "Can't get coefficients from solver if constraint is not " "in a model"
-            )
+            lb_str = ""
+        if self.ub is not None:
+            ub_str = " <= " + str(self.ub)
+        else:
+            ub_str = ""
+        return ''.join((lb_str, super(Variable, self).__str__(), ub_str))
+
+    def __repr__(self):
+        """Does exactly the same as __str__ for now."""
+        return self.__str__()
 
-    def _get_expression(self):
-        if self.problem is not None:
-            variables = self.problem._variables
-            all_coefs = self.problem.problem.constraint_coefs
-            coefs = [(v, all_coefs.get((self.name, v.name), 0.0)) for v in variables]
-            expression = add([mul((symbolics.Real(co), v)) for (v, co) in coefs])
+    def __getstate__(self):
+        return self.__dict__
+
+    def __setstate__(self, state):
+        self.__dict__ = state
+
+    def _round_primal_to_bounds(self, primal, tolerance=1e-6):
+        if (primal >= self.lb or self.lb is None) and (primal <= self.ub or self.ub is None):
+                return primal
+        else:
+            if (primal <= self.lb) and ((self.lb - primal) <= tolerance):
+                return self.lb
+            elif (primal >= self.ub) and ((self.ub - primal) >= -tolerance):
+                return self.ub
+            else:
+                raise AssertionError('The primal value %s returned by the solver is out of bounds for variable %s (lb=%s, ub=%s)' % (primal, self.name, self.lb, self.ub))
+
+
+# noinspection PyPep8Naming
+class OptimizationExpression(object):
+    """Abstract base class for Objective and Constraint."""
+
+    @classmethod
+    def _substitute_variables(cls, expression, model=None, **kwargs):
+        """Substitutes variables in (optimization)expression (constraint/objective) with variables of the appropriate interface type.
+        Attributes
+        ----------
+        expression: Constraint, Objective
+            An optimization expression.
+        problem: Model or None, optional
+            A reference to an optimization model that should be searched for appropriate variables first.
+        """
+        interface = sys.modules[cls.__module__]
+        variable_substitutions = dict()
+        for variable in expression.variables:
+            if model is not None and variable.name in model.variables:
+                # print variable.name, id(variable.problem)
+                variable_substitutions[variable] = model.variables[variable.name]
+            else:
+                variable_substitutions[variable] = interface.Variable.clone(variable)
+        adjusted_expression = expression.expression.xreplace(variable_substitutions)
+        return adjusted_expression
+
+    def __init__(self, expression, name=None, problem=None, sloppy=False, *args, **kwargs):
+        super(OptimizationExpression, self).__init__(*args, **kwargs)
+        if sloppy:
             self._expression = expression
-        return self._expression
+        else:
+            self._expression = self._canonicalize(expression)
+        if name is None:
+            self.name = str(uuid.uuid1())
+        else:
+            self.name = name
+        self._problem = problem
 
     @property
     def problem(self):
         return self._problem
 
     @problem.setter
     def problem(self, value):
-        if value is None:
-            # Update expression from solver instance one last time
-            self._get_expression()
         self._problem = value
 
+    def _get_expression(self):
+        return self._expression
+
     @property
-    def primal(self):
-        if self.problem is None:
-            return None
-        return self.problem.problem.cprimals.get(self.name, None)
+    def expression(self):
+        """The mathematical expression defining the objective/constraint."""
+        return self._get_expression()
 
     @property
-    def dual(self):
-        if self.problem is None:
-            return None
-        d = self.problem.problem.duals.get(self.name, None)
-        if d is not None:
-            d = -d
-        return d
-
-    @interface.Constraint.name.setter
-    def name(self, value):
-        old_name = self.name
-        super(Constraint, Constraint).name.fset(self, value)
-        if getattr(self, "problem", None) is not None:
-            if old_name != value:
-                self.problem.problem.rename_constraint(old_name, value)
+    def variables(self):
+        """Variables in constraint."""
+        return self.expression.atoms(sympy.Symbol)
 
-    @interface.Constraint.lb.setter
-    def lb(self, value):
-        self._check_valid_lower_bound(value)
-        if getattr(self, "problem", None) is not None:
-            lb = -Infinity if value is None else float(value)
-            self.problem.problem.constraint_lbs[self.name] = lb
-        self._lb = value
+    def _canonicalize(self, expression):
+        if isinstance(expression, float):
+            return sympy.RealNumber(expression)
+        elif isinstance(expression, int):
+            return sympy.Integer(expression)
+        else:
+            return expression
 
-    @interface.Constraint.ub.setter
-    def ub(self, value):
-        self._check_valid_upper_bound(value)
-        if getattr(self, "problem", None) is not None:
-            ub = Infinity if value is None else float(value)
-            self.problem.problem.constraint_ubs[self.name] = ub
-        self._ub = value
+    @property
+    def is_Linear(self):
+        """Returns True if constraint is linear (read-only)."""
+        return all((len(key.free_symbols)<2 and (key.is_Add or key.is_Mul or key.is_Atom) for key in self.expression.as_coefficients_dict().keys()))
 
-    def __iadd__(self, other):
-        # if self.problem is not None:
-        #     self.problem._add_to_constraint(self.index, other)
-        if self.problem is not None:
-            problem_reference = self.problem
-            self.problem._remove_constraint(self)
-            super(Constraint, self).__iadd__(other)
-            problem_reference._add_constraint(self, sloppy=False)
+    @property
+    def is_Quadratic(self):
+        """Returns True if constraint is quadratic (read-only)."""
+        try:
+            poly = self.expression.as_poly(*self.expression.atoms(sympy.Symbol))
+        except sympy.PolynomialError:
+            poly = None
+        if poly is not None and poly.is_quadratic and not poly.is_linear:
+            return True
         else:
-            super(Constraint, self).__iadd__(other)
+            return False
+
+    def __iadd__(self, other):
+        self._expression += other
+        # self.expression = sympy.Add._from_args((self.expression, other))
         return self
 
+    def __isub__(self, other):
+        self._expression -= other
+        return self
 
-@six.add_metaclass(inheritdocstring)
-class Objective(interface.Objective):
-    def __init__(self, expression, sloppy=False, **kwargs):
-        super(Objective, self).__init__(expression, sloppy=sloppy, **kwargs)
-        self._expression_expired = False
-        if not (sloppy or self.is_Linear or self.is_Quadratic):
-            raise ValueError("OSQP only supports linear and quadratic objectives.")
+    def __imul__(self, other):
+        self._expression *= other
+        return self
 
-    @property
-    def value(self):
-        if getattr(self, "problem", None) is None:
-            return None
-        if self.problem.problem.obj_value is None:
-            return None
-        return self.problem.problem.obj_value + self.problem._objective_offset
+    def __idiv__(self, other):
+        self._expression /= other
+        return self
 
-    @interface.Objective.direction.setter
-    def direction(self, value):
-        super(Objective, Objective).direction.__set__(self, value)
-        if value == "min":
-            self.problem.problem.direction = 1
-        else:
-            self.problem.problem.direction = -1
+    def __itruediv__(self, other):
+        self._expression /= other
+        return self
 
-    def _get_expression(self):
-        if (
-            self.problem is not None
-            and self._expression_expired
-            and len(self.problem._variables) > 0
-        ):
-            model = self.problem
-            vars = model._variables
-            expression = add(
-                [
-                    coef * vars[vn]
-                    for vn, coef in six.iteritems(model.problem.obj_linear_coefs)
-                ]
-            )
-            q_ex = add(
-                [
-                    coef * vars[vn[0]] * vars[vn[1]]
-                    for vn, coef in six.iteritems(model.problem.obj_quadratic_coefs)
-                ]
-            )
-            expression += q_ex
-            self._expression = expression
-            self._expression_expired = False
-        return self._expression
 
-    def set_linear_coefficients(self, coefficients):
-        if self.problem is not None:
-            self.problem.update()
-            for v, coef in six.iteritems(coefficients):
-                self.problem.problem.obj_linear_coefs[v.name] = float(coef)
-            self._expression_expired = True
-        else:
-            raise Exception(
-                "Can't change coefficients if objective is not associated "
-                "with a model."
-            )
+class Constraint(OptimizationExpression):
+    """Optimization constraint.
 
-    def get_linear_coefficients(self, variables):
-        if self.problem is not None:
-            self.problem.update()
-            coefs = {
-                v: self.problem.problem.obj_linear_coefs.get(v.name, 0.0)
-                for v in variables
-            }
-            return coefs
-        else:
-            raise Exception(
-                "Can't get coefficients from solver if objective " "is not in a model"
-            )
+    Wraps sympy expressions and extends them with optimization specific attributes and methods.
+
+    Attributes
+    ----------
+    expression: sympy
+        The mathematical expression defining the constraint.
+    name: str, optional
+        The constraint's name.
+    lb: float or None, optional
+        The lower bound, if None then -inf.
+    ub: float or None, optional
+        The upper bound, if None then inf.
+    indicator_variable: Variable
+        The indicator variable (needs to be binary).
+    active_when: 0 or 1 (default 0)
+        When the constraint should
+    problem: Model or None, optional
+        A reference to the optimization model the variable belongs to.
+    """
+
+    # @classmethod
+    # def clone(cls, constraint, model=None, **kwargs):
+    #     return cls(cls._substitute_variables(constraint, model=model), lb=constraint.lb, ub=constraint.ub,
+    #                name=constraint.name, problem=constraint.problem, sloppy=True, **kwargs)
+
+    _INDICATOR_CONSTRAINT_SUPPORT = True
 
+    @classmethod
+    def __check_valid_indicator_variable(cls, variable):
+        if variable is not None and not cls._INDICATOR_CONSTRAINT_SUPPORT:
+            raise Exception('Solver interface %s does not support indicator constraints' % cls.__module__)
+        if variable is not None and variable.type != 'binary':
+            raise ValueError('Provided indicator variable %s is not binary.' % variable)
+
+    @staticmethod
+    def __check_valid_active_when(active_when):
+        if active_when != 0 and active_when != 1:
+            raise ValueError('Provided active_when argument %s needs to be either 1 or 0' % active_when)
 
-@six.add_metaclass(inheritdocstring)
-class Configuration(interface.MathematicalProgrammingConfiguration):
-    def __init__(
-        self,
-        lp_method="primal",
-        presolve=False,
-        verbosity=0,
-        timeout=None,
-        qp_method="primal",
-        linear_solver="qdldl",
-        *args,
-        **kwargs
-    ):
-        super(Configuration, self).__init__(*args, **kwargs)
-        self.lp_method = lp_method
-        self.presolve = presolve
-        self.verbosity = verbosity
-        self.timeout = timeout
-        self.qp_method = qp_method
-        self.linear_solver = linear_solver
-        if "tolerances" in kwargs:
-            for key, val in six.iteritems(kwargs["tolerances"]):
-                if key in self._tolerance_functions():
-                    setattr(self.tolerances, key, val)
-
-    @property
-    def lp_method(self):
-        """The algorithm used to solve LP problems."""
-        return "primal"
-
-    @lp_method.setter
-    def lp_method(self, lp_method):
-        if lp_method not in _LP_METHODS:
+    @classmethod
+    def clone(cls, constraint, model=None, **kwargs):
+        return cls(cls._substitute_variables(constraint, model=model), lb=constraint.lb, ub=constraint.ub,
+                   indicator_variable=constraint.indicator_variable, active_when=constraint.active_when,
+                   name=constraint.name, sloppy=True, **kwargs)
+
+    def __init__(self, expression, lb=None, ub=None, indicator_variable=None, active_when=1, *args, **kwargs):
+        self.lb = lb
+        self.ub = ub
+        self.__check_valid_indicator_variable(indicator_variable)
+        self.__check_valid_active_when(active_when)
+        self._indicator_variable = indicator_variable
+        self._active_when = active_when
+        super(Constraint, self).__init__(expression, *args, **kwargs)
+
+    @property
+    def indicator_variable(self):
+        return self._indicator_variable
+
+    @indicator_variable.setter
+    def indicator_variable(self, value):
+        self.__check_valid_indicator_variable(value)
+        self._indicator_variable = value
+
+    @property
+    def active_when(self):
+        return self._active_when
+
+    @indicator_variable.setter
+    def indicator_variable(self, value):
+        self.__check_valid_active_when(value)
+        self._active_when = value
+
+    def __str__(self):
+        if self.lb is not None:
+            lhs = str(self.lb) + ' <= '
+        else:
+            lhs = ''
+        if self.ub is not None:
+            rhs = ' <= ' + str(self.ub)
+        else:
+            rhs = ''
+        if self.indicator_variable is not None:
+            lhs = self.indicator_variable.name + ' = ' + str(self.active_when) + ' -> ' + lhs
+        return str(self.name) + ": " + lhs + self.expression.__str__() + rhs
+
+    def _canonicalize(self, expression):
+        expression = super(Constraint, self)._canonicalize(expression)
+        if expression.is_Atom or expression.is_Mul:
+            return expression
+        lonely_coeffs = [arg for arg in expression.args if arg.is_Number]
+        if not lonely_coeffs:
+            return expression
+        assert len(lonely_coeffs) == 1
+        coeff = lonely_coeffs[0]
+        if self.lb is None and self.ub is None:
             raise ValueError(
-                "LP Method %s is not valid (choose one of: %s)"
-                % (lp_method, ", ".join(_LP_METHODS))
+                "%s cannot be shaped into canonical form if neither lower or upper constraint bounds are set."
+                % expression
             )
+        elif self.lb is not None:
+            expression = expression - coeff
+            self.lb = self.lb - coeff
+        else:
+            expression = expression - coeff
+            self.ub = self.ub - coeff
+        return expression
 
     @property
-    def linear_solver(self):
-        return self._linear_solver
+    def primal(self):
+        return None
 
-    @linear_solver.setter
-    def linear_solver(self, solver):
-        if solver not in ("qdldl", "mkl pardiso"):
-            raise ValueError(
-                "%s is not valid (choose either `qdldl` or `mkl pardiso`)" % solver
-            )
-        if getattr(self, "problem", None) is not None:
-            self.problem.problem.settings["linsys_solver"] = solver
-        self._linear_solver = solver
-
-    def _set_presolve(self, value):
-        if getattr(self, "problem", None) is not None:
-            if value is True:
-                self.problem.problem.settings["scaling"] = 10
-            elif value is False or value == "auto":
-                self.problem.problem.settings["scaling"] = 0
-            else:
-                raise ValueError(
-                    str(value) + " is not a valid presolve parameter. Must be True, "
-                    "False or 'auto'."
-                )
+    @property
+    def dual(self):
+        return None
+
+
+class Objective(OptimizationExpression):
+    """Objective function.
+
+    Attributes
+    ----------
+    expression: sympy
+        The mathematical expression defining the objective.
+    name: str, optional
+        The name of the constraint.
+    direction: 'max' or 'min'
+        The optimization direction.
+    value: float, read-only
+        The current objective value.
+    problem: solver
+        The low-level solver object.
+
+    """
+
+    @classmethod
+    def clone(cls, objective, model=None, **kwargs):
+        return cls(cls._substitute_variables(objective, model=model), name=objective.name,  # TODO: problem=model, (it's breaking cameo for some reason)
+                   direction=objective.direction, sloppy=True, **kwargs)
+
+    def __init__(self, expression, value=None, direction='max', *args, **kwargs):
+        self._value = value
+        self._direction = direction
+        super(Objective, self).__init__(expression, *args, **kwargs)
 
     @property
-    def presolve(self):
-        return self.problem.problem.settings["scaling"] > 0
+    def value(self):
+        return self._value
 
-    @presolve.setter
-    def presolve(self, value):
-        self._set_presolve(value)
-        self._presolve = value
+    def __str__(self):
+        return {'max': 'Maximize', 'min': 'Minimize'}[self.direction] + '\n' + str(self.expression)
+        # return ' '.join((self.direction, str(self.expression)))
+
+    def _canonicalize(self, expression):
+        """For example, changes x + y to 1.*x + 1.*y"""
+        expression = super(Objective, self)._canonicalize(expression)
+        expression *= 1.
+        return expression
+
+    @property
+    def direction(self):
+        """The direction of optimization. Either 'min' or 'max'."""
+        return self._direction
+
+    @direction.setter
+    def direction(self, value):
+        if value not in ['max', 'min']:
+            raise ValueError("Provided optimization direction %s is neither 'min' or 'max'." % value)
+        self._direction = value
+
+
+class Configuration(object):
+    """Optimization solver configuration."""
+
+    @classmethod
+    def clone(cls, config, problem=None, **kwargs):
+        properties = (k for k, v in inspect.getmembers(cls, predicate=inspect.isdatadescriptor) if not k.startswith('__'))
+        parameters = {property: getattr(config, property) for property in properties}
+        return cls(problem=problem, **parameters)
+
+    def __init__(self, problem=None, *args, **kwargs):
+        self.problem = problem
 
     @property
     def verbosity(self):
-        return self._verbosity
+        """Verbosity level.
+
+        0: no output
+        1: error and warning messages only
+        2: normal output
+        4: full output
+        """
+        raise NotImplementedError
 
     @verbosity.setter
     def verbosity(self, value):
-        if getattr(self, "problem", None) is not None:
-            self.problem.problem.settings["verbose"] = int(value > 0)
-        self._verbosity = value
+        raise NotImplementedError
 
     @property
     def timeout(self):
-        return self.problem.problem.settings["time_limit"]
+        raise NotImplementedError
 
     @timeout.setter
-    def timeout(self, value):
-        if getattr(self, "problem", None) is not None:
-            if value is None:
-                self.problem.problem.settings["time_limit"] = 0
-            else:
-                self.problem.problem.settings["time_limit"] = value
+    def timeout(self):
+        raise NotImplementedError
 
-    def __getstate__(self):
-        return {
-            "presolve": self.presolve,
-            "timeout": self.timeout,
-            "verbosity": self.verbosity,
-            "linear_solver": self.linear_solver,
-            "tolerances": {
-                "feasibility": self.tolerances.feasibility,
-                "optimality": self.tolerances.optimality,
-                "integrality": self.tolerances.integrality,
-            },
-        }
 
-    def __setstate__(self, state):
-        for key, val in six.iteritems(state):
-            if key != "tolerances":
-                setattr(self, key, val)
-        for key, val in six.iteritems(state["tolerances"]):
-            if key in self._tolerance_functions():
-                setattr(self.tolerances, key, val)
+class MathematicalProgrammingConfiguration(Configuration):
+    def __init__(self, *args, **kwargs):
+        super(MathematicalProgrammingConfiguration, self).__init__(*args, **kwargs)
 
     @property
-    def qp_method(self):
-        """Change the algorithm used to optimize QP problems."""
-        return "primal"
-
-    @qp_method.setter
-    def qp_method(self, value):
-        if value not in _QP_METHODS:
-            raise ValueError(
-                "%s is not a valid qp_method. Choose between %s"
-                % (value, str(_QP_METHODS))
-            )
-        self._qp_method = value
-
-    def _get_feasibility(self):
-        return self.problem.problem.settings["eps_prim_inf"]
-
-    def _set_feasibility(self, value):
-        self.problem.problem.settings["eps_prim_inf"] = value
-        self.problem.problem.settings["eps_dual_inf"] = value
+    def presolve(self):
+        raise NotImplementedError
 
-    def _get_integrality(self):
-        return 1e-6
+    @presolve.setter
+    def presolve(self, value):
+        raise NotImplementedError
 
-    def _set_integrality(self, value):
-        pass
 
-    def _get_optimality(self):
-        return self.problem.problem.settings["eps_abs"]
+class EvolutionaryOptimizationConfiguration(Configuration):
+    """docstring for HeuristicOptimization"""
 
-    def _set_optimality(self, value):
-        self.problem.problem.settings["eps_abs"] = value
-        self.problem.problem.settings["eps_rel"] = value
+    def __init__(self, *args, **kwargs):
+        super(EvolutionaryOptimizationConfiguration, self).__init__(*args, **kwargs)
 
-    def _tolerance_functions(self):
-        return {
-            "feasibility": (self._get_feasibility, self._set_feasibility),
-            "optimality": (self._get_optimality, self._set_optimality),
-            "integrality": (self._get_integrality, self._set_integrality),
-        }
 
+class Model(object):
+    """Optimization problem.
+
+    Attributes
+    ----------
+    objective: str
+        The objective function.
+    name: str, optional
+        The name of the optimization problem.
+    variables: Container, read-only
+        Contains the variables of the optimization problem.
+        The keys are the variable names and values are the actual variables.
+    constraints: Container, read-only
+         Contains the variables of the optimization problem.
+         The keys are the constraint names and values are the actual constraints.
+    status: str, read-only
+        The status of the optimization problem.
 
-@six.add_metaclass(inheritdocstring)
-class Model(interface.Model):
-    def _initialize_problem(self):
-        self.problem = OSQPProblem()
+    Examples
+    --------
 
-    def _initialize_model_from_problem(self, problem, vc_mapping=None, offset=0):
-        if not isinstance(problem, OSQPProblem):
-            raise TypeError("Provided problem is not a valid OSQP model.")
-        self.problem = problem
-        for name in self.problem.variables:
-            var = Variable(
-                name,
-                lb=self.problem.variable_lbs[name],
-                ub=self.problem.variable_ubs[name],
-                problem=self,
-            )
-            super(Model, self)._add_variables([var])
 
-        for name in self.problem.constraints:
-            # Since constraint expressions are lazily retrieved from the
-            # solver they don't have to be built here
-            lhs = symbolics.Integer(0)
-            constr = Constraint(
-                lhs,
-                lb=self.problem.constraint_lbs[name],
-                ub=self.problem.constraint_ubs[name],
-                name=name,
-                problem=self,
-            )
+    """
 
-            super(Model, self)._add_constraints([constr], sloppy=True)
+    @classmethod
+    def clone(cls, model):
+        interface = sys.modules[cls.__module__]
+        new_model = cls()
+        for constraint in model.constraints:
+            new_constraint = interface.Constraint.clone(constraint, model=new_model)
+            new_model._add_constraint(new_constraint)
+        if model.objective is not None:
+            new_model.objective = interface.Objective.clone(model.objective, model=new_model)
+        new_model.configuration = interface.Configuration.clone(model.configuration, problem=new_model)
+        return new_model
+
+    def __init__(self, name=None, objective=None, variables=None, constraints=None, *args, **kwargs):
+        super(Model, self).__init__(*args, **kwargs)
+        self._objective = objective
+        self._variables = Container()
+        self._constraints = Container()
+        self._variables_to_constraints_mapping = dict()
+        self._status = None
+        self.name = name
+        if variables is not None:
+            self.add(variables)
+        if constraints is not None:
+            self.add(constraints)
 
-        if vc_mapping is None:
-            for constr in self.constraints:
-                name = constr.name
-                for variable in constr.variables:
-                    try:
-                        self._variables_to_constraints_mapping[variable.name].add(name)
-                    except KeyError:
-                        self._variables_to_constraints_mapping[variable.name] = set(
-                            [name]
-                        )
-        else:
-            self._variables_to_constraints_mapping = vc_mapping
-
-        linear_expression = add(
-            [
-                coef * self._variables[vn]
-                for vn, coef in six.iteritems(self.problem.obj_linear_coefs)
-            ]
-        )
-        quadratic_expression = add(
-            [
-                coef * self._variables[vn[0]] * self._variables[vn[1]]
-                for vn, coef in six.iteritems(self.problem.obj_quadratic_coefs)
-            ]
-        )
-
-        self._objective_offset = offset
-        self._objective = Objective(
-            linear_expression + quadratic_expression + offset,
-            problem=self,
-            direction={-1: "max", 1: "min"}[self.problem.direction],
-            name="osqp_objective",
-        )
+    @property
+    def interface(self):
+        return sys.modules[self.__module__]
 
     @property
     def objective(self):
         return self._objective
 
     @objective.setter
     def objective(self, value):
-        value.problem = None
-        if self._objective is not None:  # Reset previous objective
-            self.problem.obj_linear_coefs = dict()
-            self.problem.obj_quadratic_coefs = dict()
-        super(Model, self.__class__).objective.fset(self, value)
-        self.update()
-        expression = self._objective._expression
-        (
-            offset,
-            linear_coefficients,
-            quadratic_coeffients,
-        ) = parse_optimization_expression(value, quadratic=True, expression=expression)
-        self._objective_offset = offset
-        if linear_coefficients:
-            self.problem.obj_linear_coefs = {
-                v.name: float(c) for v, c in six.iteritems(linear_coefficients)
-            }
-
-        for key, coef in six.iteritems(quadratic_coeffients):
-            if len(key) == 1:
-                var = six.next(iter(key))
-                self.problem.obj_quadratic_coefs[(var.name, var.name)] = float(coef)
+        try:
+            for atom in value.expression.atoms(sympy.Symbol):
+                if isinstance(atom, Variable) and (atom.problem is None or atom.problem != self):
+                    self._add_variable(atom)
+        except AttributeError as e:
+            if isinstance(value.expression, six.types.FunctionType) or isinstance(value.expression, float):
+                pass
             else:
-                var1, var2 = key
-                self.problem.obj_quadratic_coefs[(var1.name, var2.name)] = 0.5 * float(
-                    coef
-                )
-                self.problem.obj_quadratic_coefs[(var2.name, var1.name)] = 0.5 * float(
-                    coef
-                )
-
-        self._set_objective_direction(value.direction)
-        value.problem = self
-
-    def _set_objective_direction(self, direction):
-        self.problem.direction = {"min": 1, "max": -1}[direction]
-
-    def _get_primal_values(self):
-        if len(self.problem.primals) == 0:
-            raise SolverError("The problem has not been solved yet!")
-        primal_values = [self.problem.primals[v.name] for v in self._variables]
-        return primal_values
-
-    def _get_reduced_costs(self):
-        if len(self.problem.duals) == 0:
-            raise SolverError("The problem has not been solved yet!")
-        reduced_costs = [self.problem.vduals[v.name] for v in self._variables]
-        return reduced_costs
-
-    def _get_constraint_values(self):
-        if len(self.problem.primals) == 0:
-            raise SolverError("The problem has not been solved yet!")
-        constraint_primals = [self.problem.cprimals[c.name] for c in self._constraints]
-        return constraint_primals
-
-    def _get_shadow_prices(self):
-        if len(self.problem.primals) == 0:
-            raise SolverError("The problem has not been solved yet!")
-        dual_values = [-self.problem.duals[c.name] for c in self._constraints]
-        return dual_values
-
-    @property
-    def is_integer(self):
-        return False
-
-    def _optimize(self):
-        self.update()
-        self.problem.solve()
-        osqp_status = self.problem.status
-        self._original_status = osqp_status
-        status = _STATUS_MAP[osqp_status]
-        return status
-
-    def _set_variable_bounds_on_problem(self, var_lb, var_ub):
-        self.problem.reset()
-        for var, val in var_lb:
-            lb = -Infinity if val is None else float(val)
-            self.problem.variable_lbs[var.name] = lb
-        for var, val in var_ub:
-            ub = Infinity if val is None else val
-            self.problem.variable_ubs[var.name] = float(ub)
-
-    def _add_variables(self, variables):
-        super(Model, self)._add_variables(variables)
-        self.problem.reset()
-        for variable in variables:
-            lb = -Infinity if variable.lb is None else float(variable.lb)
-            ub = Infinity if variable.ub is None else float(variable.ub)
-            self.problem.variables.add(variable.name)
-            self.problem.variable_lbs[variable.name] = lb
-            self.problem.variable_ubs[variable.name] = ub
-            variable.problem = self
+                raise AttributeError(e)
+        self._objective = value
+        self._objective.problem = self
+
+    @property
+    def variables(self):
+        return self._variables
+
+    @property
+    def constraints(self):
+        return self._constraints
+
+    @property
+    def status(self):
+        return self._status
+
+    @property
+    def primal_values(self):
+        # Fallback, if nothing faster is available
+        return collections.OrderedDict([(variable.name, variable.primal) for variable in self.variables])
+
+    @property
+    def reduced_costs(self):
+        # Fallback, if nothing faster is available
+        return collections.OrderedDict([(variable.name, variable.dual) for variable in self.variables])
+
+    @property
+    def dual_values(self):
+        # Fallback, if nothing faster is available
+        return collections.OrderedDict([(constraint.name, constraint.primal) for constraint in self.constraint])
+
+    @property
+    def shadow_prices(self):
+        # Fallback, if nothing faster is available
+        return collections.OrderedDict([(constraint.name, constraint.dual) for constraint in self.constraint])
+
+    def __str__(self):
+        return '\n'.join((
+            str(self.objective),
+            "subject to",
+            '\n'.join([str(constr) for constr in self.constraints]),
+            'Bounds',
+            '\n'.join([str(var) for var in self.variables])
+        ))
+
+    # @property
+    # def interface(self):
+    #     return sys.modules[self.__module__]
+
+    def add(self, stuff):
+        """Add variables and constraints.
+
+        Parameters
+        ----------
+        stuff : iterable, Variable, Constraint
+            Either an iterable containing variables and constraints or a single variable or constraint.
+
+        Returns
+        -------
+        None
+
+
+        """
+        if isinstance(stuff, collections.Iterable):
+            for elem in stuff:
+                self.add(elem)
+        elif isinstance(stuff, Variable):
+            if stuff.__module__ != self.__module__:
+                raise TypeError("Cannot add Variable %s of interface type %s to model of type %s." % (
+                    stuff, stuff.__module__, self.__module__))
+            self._add_variable(stuff)
+        elif isinstance(stuff, Constraint):
+            if stuff.__module__ != self.__module__:
+                raise TypeError("Cannot add Constraint %s of interface type %s to model of type %s." % (
+                    stuff, stuff.__module__, self.__module__))
+            self._add_constraint(stuff)
+        elif isinstance(stuff, Objective):
+            if stuff.__module__ != self.__module__:
+                raise TypeError("Cannot set Objective %s of interface type %s to model of type %s." % (
+                    stuff, stuff.__module__, self.__module__))
+            self.objective = stuff
+        else:
+            raise TypeError("Cannot add %s. It is neither a Variable, Constraint, or Objective." % stuff)
+
+    def remove(self, stuff):
+        """Remove variables and constraints.
+
+        Parameters
+        ----------
+        stuff : iterable, str, Variable, Constraint
+            Either an iterable containing variables and constraints to be removed from the model or a single variable or contstraint (or their names).
+
+        Returns
+        -------
+        None
+        """
+        if isinstance(stuff, str):
+            try:
+                variable = self.variables[stuff]
+                self._remove_variable(variable)
+            except KeyError:
+                try:
+                    constraint = self.constraints[stuff]
+                    self._remove_constraint(constraint)
+                except KeyError:
+                    raise LookupError(
+                        "%s is neither a variable nor a constraint in the current solver instance." % stuff)
+        elif isinstance(stuff, Variable):
+            self._remove_variable(stuff)
+        elif isinstance(stuff, Constraint):
+            self._remove_constraint(stuff)
+        elif isinstance(stuff, collections.Iterable):
+            element_types = set((elem.__class__ for elem in stuff))
+            if len(element_types) == 1:
+                element_type = element_types.pop()
+                if issubclass(element_type, Variable):
+                    self._remove_variables(stuff)
+                elif issubclass(element_type, Constraint):
+                    self._remove_constraints(stuff)
+                else:
+                    raise TypeError("Cannot remove %s. It is neither a variable nor a constraint." % stuff)
+            else:
+                for elem in stuff:
+                    self.remove(elem)
+        elif isinstance(stuff, Objective):
+            raise TypeError(
+                "Cannot remove objective %s. Use model.objective = Objective(...) to change the current objective." % stuff)
+        else:
+            raise TypeError(
+                "Cannot remove %s. It neither a variable or constraint." % stuff)
+
+    def optimize(self):
+        """Solve the optimization problem.
+
+        Returns
+        -------
+        status: str
+            Solution status.
+        """
+        raise NotImplementedError(
+            "You're using the high level interface to optlang. Problems cannot be optimized in this mode. Choose from one of the solver specific interfaces.")
+
+    def _add_variable(self, variable):
+        self.variables.append(variable)
+        self._variables_to_constraints_mapping[variable.name] = set([])
+        variable.problem = self
+
+        return variable
 
     def _remove_variables(self, variables):
-        # Not calling parent method to avoid expensive variable removal from sympy expressions
-        if self.objective is not None:
-            self.objective._expression = self.objective.expression.xreplace(
-                {var: 0 for var in variables}
-            )
+
+        for variable in variables:
+            try:
+                var = self.variables[variable.name]
+            except KeyError:
+                raise LookupError("Variable %s not in solver" % var)
+
+        constraint_ids = set()
         for variable in variables:
+            constraint_ids.update(self._variables_to_constraints_mapping[variable.name])
             del self._variables_to_constraints_mapping[variable.name]
             variable.problem = None
-            del self._variables[variable.name]
-            self.problem.variables.remove(variable.name)
-        self.problem.clean()
-
-    def _add_constraints(self, constraints, sloppy=False):
-        super(Model, self)._add_constraints(constraints, sloppy=sloppy)
-        self.problem.reset()
-        for constraint in constraints:
-            constraint._problem = None  # This needs to be done in order to not trigger constraint._get_expression()
-            if constraint.is_Linear:
-                _, coeff_dict, _ = parse_optimization_expression(constraint)
-                lb = -Infinity if constraint.lb is None else float(constraint.lb)
-                ub = Infinity if constraint.ub is None else float(constraint.ub)
-                self.problem.constraints.add(constraint.name)
-                self.problem.constraint_coefs.update(
-                    {
-                        (constraint.name, v.name): float(co)
-                        for v, co in six.iteritems(coeff_dict)
-                    }
-                )
-                self.problem.constraint_lbs[constraint.name] = lb
-                self.problem.constraint_ubs[constraint.name] = ub
-                constraint.problem = self
-            elif constraint.is_Quadratic:
-                raise NotImplementedError(
-                    "Quadratic constraints (like %s) are not supported "
-                    "in OSQP yet." % constraint
-                )
-            else:
-                raise ValueError(
-                    "OSQP only supports linear or quadratic constraints. "
-                    "%s is neither linear nor quadratic." % constraint
-                )
+            del self.variables[variable.name]
+
+        replacements = dict([(variable, 0) for variable in variables])
+        for constraint_id in constraint_ids:
+            constraint = self.constraints[constraint_id]
+            constraint._expression = constraint.expression.xreplace(replacements)
+
+        self.objective._expression = self.objective.expression.xreplace(replacements)
+
+    def _remove_variable(self, variable):
+        self._remove_variables([variable])
+
+    def _add_constraint(self, constraint, sloppy=False):
+        constraint_id = constraint.name
+        if sloppy is False:
+            variables = constraint.variables
+            if constraint.indicator_variable is not None:
+                variables.add(constraint.indicator_variable)
+            for var in variables:
+                if var.problem is not self:
+                    self._add_variable(var)
+                try:
+                    self._variables_to_constraints_mapping[var.name].add(constraint_id)
+                except KeyError:
+                    self._variables_to_constraints_mapping[var.name] = set([constraint_id])
+        self.constraints.append(constraint)
+        constraint._problem = self
 
     def _remove_constraints(self, constraints):
-        super(Model, self)._remove_constraints(constraints)
-        for constraint in constraints:
-            self.problem.constraints.remove(constraint.name)
-        self.problem.clean()
-
-    def _get_variable_indices(self, names):
-        vmap = dict(zip(self.variables, range(len(self.variables))))
-        return [vmap[n] for n in names]
-
-    def __setstate__(self, d):
-        self.__init__()
-        osqp = pickle.loads(d["osqp"])
-        # workaround to conserve the order
-        osqp.variables = d["variables"]
-        osqp.constraints = d["constraints"]
-        self._initialize_model_from_problem(
-            osqp, vc_mapping=d["v_to_c"], offset=d["offset"]
-        )
-        osqp.variables = set(osqp.variables)
-        osqp.constraints = set(osqp.constraints)
-        self.configuration = Configuration()
-        self.configuration.problem = self
-        self.configuration.__setstate__(d["config"])
+        keys = [constraint.name for constraint in constraints]
+        if len(constraints) > 350:  # Need to figure out a good threshold here
+            self._constraints = self.constraints.fromkeys(set(self.constraints.keys()).difference(set(keys)))
+        else:
+            for constraint in constraints:
+                try:
+                    del self.constraints[constraint.name]
+                except KeyError:
+                    raise LookupError("Constraint %s not in solver" % constraint)
+                else:
+                    constraint.problem = None
+
+    def _remove_constraint(self, constraint):
+        self._remove_constraints([constraint])
+
+    def _set_linear_objective_term(self, variable, coefficient):
+        # TODO: the is extremely slow for objectives with many terms
+        if variable in self.objective.expression.atoms(sympy.Symbol):
+            a = sympy.Wild('a', exclude=[variable])
+            (new_expression, map) = self.objective.expression.replace(lambda expr: expr.match(a*variable), lambda expr: coefficient*variable, simultaneous=False, map=True)
+            self.objective.expression = new_expression
+        else:
+            self.objective.expression = sympy.Add._from_args((self.objective.expression, sympy.Mul._from_args((sympy.RealNumber(coefficient), variable))))
+
+if __name__ == '__main__':
+    # Example workflow
+
+    x1 = Variable('x1', lb=0)
+    x2 = Variable('x2', lb=0)
+    x3 = Variable('x3', lb=0)
+    c1 = Constraint(x1 + x2 + x3, ub=100)
+    c2 = Constraint(10 * x1 + 4 * x2 + 5 * x3, ub=600)
+    c3 = Constraint(2 * x1 + 2 * x2 + 6 * x3, ub=300)
+    obj = Objective(10 * x1 + 6 * x2 + 4 * x3, direction='max')
+    model = Model(name='Simple model')
+    model.objective = obj
+    model.add([c1, c2, c3])
 
-    def __getstate__(self):
-        self.problem.reset()
-        self.update()
-        return {
-            "osqp": pickle.dumps(self.problem),
-            "variables": [v.name for v in self._variables],
-            "constraints": [c.name for c in self._constraints],
-            "v_to_c": self._variables_to_constraints_mapping,
-            "config": self.configuration.__getstate__(),
-            "offset": getattr(self, "_objective_offset", 0.0),
-        }
+    try:
+        sol = model.optimize()
+    except NotImplementedError as e:
+        print(e)
 
-    @classmethod
-    def from_lp(self, lp_problem_str):
-        """Read a model from an LP file.
+    print(model)
+    print(model.variables)
 
-        OSQP does not have an integrated LP reader so it will either use
-        cplex or glpk to read the model. This means that QP problems will
-        currently require cplex to be read :(
-        """
-        if available_solvers["CPLEX"]:
-            from optlang import cplex_interface
+    # model.remove(x1)
+
+    import optlang
 
-            mod = cplex_interface.Model.from_lp(lp_problem_str)
-            mod.configuration.lp_method = "auto"
-            mod.configuration.qp_method = "auto"
-            return super(Model, self).clone(mod)
-        else:
-            from optlang import glpk_interface
-
-            mod = glpk_interface.Model.from_lp(lp_problem_str)
-            mod.configuration.lp_method = "auto"
-            return super(Model, self).clone(mod)
+    model.interface = optlang.glpk_interface
```

