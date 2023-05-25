# Comparing `tmp/didppy-0.3.4.tar.gz` & `tmp/didppy-0.4.0.tar.gz`

## Comparing `didppy-0.3.4.tar` & `didppy-0.4.0.tar`

### file list

```diff
@@ -1,154 +1,151 @@
--rw-r--r--   0        0        0      377 1970-01-01 00:00:00.000000 didppy-0.3.4/local_dependencies/dypdl/Cargo.toml
--rw-r--r--   0      501       20     5194 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/README.md
--rw-r--r--   0      501       20     3301 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/base_case.rs
--rw-r--r--   0      501       20     1344 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/effect.rs
--rw-r--r--   0      501       20    16931 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/argument_expression.rs
--rw-r--r--   0      501       20    59188 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/condition.rs
--rw-r--r--   0      501       20   290240 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/continuous_expression.rs
--rw-r--r--   0      501       20    36620 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/continuous_vector_expression.rs
--rw-r--r--   0      501       20    88634 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/element_expression.rs
--rw-r--r--   0      501       20   134795 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/integer_expression.rs
--rw-r--r--   0      501       20    25379 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/integer_vector_expression.rs
--rw-r--r--   0      501       20    18114 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/numeric_operator.rs
--rw-r--r--   0      501       20    62551 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/numeric_table_expression.rs
--rw-r--r--   0      501       20     4969 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/reference_expression.rs
--rw-r--r--   0      501       20    48744 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/set_condition.rs
--rw-r--r--   0      501       20   114732 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/set_expression.rs
--rw-r--r--   0      501       20   135581 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/set_reduce_expression.rs
--rw-r--r--   0      501       20    15550 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/table_expression.rs
--rw-r--r--   0      501       20    56292 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/table_vector_expression.rs
--rw-r--r--   0      501       20     1787 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/util.rs
--rw-r--r--   0      501       20    19963 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression/vector_expression.rs
--rw-r--r--   0      501       20     1500 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/expression.rs
--rw-r--r--   0      501       20    26414 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/grounded_condition.rs
--rw-r--r--   0      501       20   650168 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/lib.rs
--rw-r--r--   0      501       20   131318 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/state.rs
--rw-r--r--   0      501       20    18956 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/table.rs
--rw-r--r--   0      501       20    46003 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/table_data.rs
--rw-r--r--   0      501       20    84395 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/table_registry.rs
--rw-r--r--   0      501       20    55902 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/transition.rs
--rw-r--r--   0      501       20      438 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/util.rs
--rw-r--r--   0      501       20     3450 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl/src/variable_type.rs
--rw-r--r--   0        0        0      405 1970-01-01 00:00:00.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/Cargo.toml
--rw-r--r--   0      501       20     1685 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/README.md
--rw-r--r--   0      501       20     3915 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/caasdy.rs
--rw-r--r--   0      501       20     3922 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_acps.rs
--rw-r--r--   0      501       20     3867 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_apps.rs
--rw-r--r--   0      501       20     3559 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_breadth_first_search.rs
--rw-r--r--   0      501       20     4414 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_cabs.rs
--rw-r--r--   0      501       20     3645 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_cbfs.rs
--rw-r--r--   0      501       20     3773 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_dbdfs.rs
--rw-r--r--   0      501       20     3984 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_dfbb.rs
--rw-r--r--   0      501       20     3425 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_weighted_astar.rs
--rw-r--r--   0      501       20     8062 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/expression_beam_search.rs
--rw-r--r--   0      501       20     1711 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/f_evaluator_type.rs
--rw-r--r--   0      501       20     1192 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/lib.rs
--rw-r--r--   0      501       20    10895 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/acps.rs
--rw-r--r--   0      501       20    12016 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/apps.rs
--rw-r--r--   0      501       20     9941 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/beam_search.rs
--rw-r--r--   0      501       20    10115 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/best_first_search.rs
--rw-r--r--   0      501       20     9967 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/breadth_first_search.rs
--rw-r--r--   0      501       20    10642 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cabs.rs
--rw-r--r--   0      501       20    10414 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cbfs.rs
--rw-r--r--   0      501       20    19258 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam.rs
--rw-r--r--   0      501       20     8068 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam_search_node.rs
--rw-r--r--   0      501       20      930 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam_search_problem_instance.rs
--rw-r--r--   0      501       20     2153 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/bfs_node.rs
--rw-r--r--   0      501       20    37845 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/f_node.rs
--rw-r--r--   0      501       20    47180 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/hashable_state.rs
--rw-r--r--   0      501       20     3549 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/lazy_search_node.rs
--rw-r--r--   0      501       20      222 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/prioritized_node.rs
--rw-r--r--   0      501       20    20071 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node.rs
--rw-r--r--   0      501       20    49429 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/state_registry.rs
--rw-r--r--   0      501       20    17046 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/successor_generator.rs
--rw-r--r--   0      501       20     3608 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_chain.rs
--rw-r--r--   0      501       20    28031 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_with_custom_cost.rs
--rw-r--r--   0      501       20     1971 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/util.rs
--rw-r--r--   0      501       20     1016 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure.rs
--rw-r--r--   0      501       20    10386 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dbdfs.rs
--rw-r--r--   0      501       20     8338 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dfbb.rs
--rw-r--r--   0      501       20     8947 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dfbbbfs.rs
--rw-r--r--   0      501       20    14198 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dijkstra.rs
--rw-r--r--   0      501       20     7077 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/forward_recursion.rs
--rw-r--r--   0      501       20    16651 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/rollout.rs
--rw-r--r--   0      501       20     3780 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/search.rs
--rw-r--r--   0      501       20     3707 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/util.rs
--rw-r--r--   0      501       20      918 2023-05-13 01:44:59.000000 didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm.rs
--rw-r--r--   0        0        0      748 1970-01-01 00:00:00.000000 didppy-0.3.4/Cargo.toml
--rw-r--r--   0      501       20      705 2023-05-13 01:44:59.000000 didppy-0.3.4/.gitignore
--rw-r--r--   0      501       20     1872 2023-05-13 01:44:59.000000 didppy-0.3.4/README.md
--rw-r--r--   0      501       20       71 2023-05-13 01:44:59.000000 didppy-0.3.4/build.rs
--rw-r--r--   0      501       20      634 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/Makefile
--rw-r--r--   0      501       20    29958 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/_static/images/TSPTW.png
--rw-r--r--   0      501       20      645 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/_templates/autosummary/class.rst
--rw-r--r--   0      501       20     8470 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/advanced-tutorials/forced-transitions.rst
--rw-r--r--   0      501       20     6060 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/advanced-tutorials/general-cost.rst
--rw-r--r--   0      501       20      250 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/advanced-tutorials.rst
--rw-r--r--   0      501       20     1931 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/api-reference.rst
--rw-r--r--   0      501       20     2246 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/conf.py
--rw-r--r--   0      501       20     4189 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/debugging/common-mistakes.rst
--rw-r--r--   0      501       20     5687 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/debugging/state.rst
--rw-r--r--   0      501       20     2881 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/debugging/validate.rst
--rw-r--r--   0      501       20      255 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/debugging.rst
--rw-r--r--   0      501       20     2237 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/examples.rst
--rw-r--r--   0      501       20     1086 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/index.rst
--rw-r--r--   0      501       20      800 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/make.bat
--rw-r--r--   0      501       20     1494 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/papers.rst
--rw-r--r--   0      501       20     4205 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/quickstart.rst
--rw-r--r--   0      501       20     7668 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/ref.bib
--rw-r--r--   0      501       20       67 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/references.rst
--rw-r--r--   0      501       20       45 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/requirements.txt
--rw-r--r--   0      501       20     4859 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/solver-selection.rst
--rw-r--r--   0      501       20    28129 2023-05-13 01:44:59.000000 didppy-0.3.4/docs/tutorial.rst
--rw-r--r--   0      501       20     2617 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/README.md
--rw-r--r--   0      501       20    10326 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/bin-packing.ipynb
--rw-r--r--   0      501       20     9176 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/cvrp.ipynb
--rw-r--r--   0      501       20     5949 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/graph-clear.ipynb
--rw-r--r--   0      501       20     4906 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/knapsack.ipynb
--rw-r--r--   0      501       20     9295 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/m-pdtsp.ipynb
--rw-r--r--   0      501       20     6910 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/mosp.ipynb
--rw-r--r--   0      501       20     9923 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/salbp-1.ipynb
--rw-r--r--   0      501       20     5293 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/single-machine.ipynb
--rw-r--r--   0      501       20     7666 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/talent-scheduling.ipynb
--rw-r--r--   0      501       20     8093 2023-05-13 01:44:59.000000 didppy-0.3.4/examples/tsptw.ipynb
--rw-r--r--   0      501       20      584 2023-05-13 01:44:59.000000 didppy-0.3.4/pyproject.toml
--rw-r--r--   0      501       20     9027 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/acps.rs
--rw-r--r--   0      501       20     9135 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/apps.rs
--rw-r--r--   0      501       20     8285 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/breadth_first_search.rs
--rw-r--r--   0      501       20     8500 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/caasdy.rs
--rw-r--r--   0      501       20     8418 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/cabs.rs
--rw-r--r--   0      501       20     8193 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/cbfs.rs
--rw-r--r--   0      501       20     8461 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/dbdfs.rs
--rw-r--r--   0      501       20     8253 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/dfbb.rs
--rw-r--r--   0      501       20     5103 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/dijkstra.rs
--rw-r--r--   0      501       20    13229 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/expression_beam_search.rs
--rw-r--r--   0      501       20     1675 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/f_operator.rs
--rw-r--r--   0      501       20     3616 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/forward_recursion.rs
--rw-r--r--   0      501       20     8124 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/weighted_astar.rs
--rw-r--r--   0      501       20     6297 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver/wrapped_solver.rs
--rw-r--r--   0      501       20      728 2023-05-13 01:44:59.000000 didppy-0.3.4/src/heuristic_search_solver.rs
--rw-r--r--   0      501       20     2919 2023-05-13 01:44:59.000000 didppy-0.3.4/src/lib.rs
--rw-r--r--   0      501       20   376402 2023-05-13 01:44:59.000000 didppy-0.3.4/src/model/expression.rs
--rw-r--r--   0      501       20     4897 2023-05-13 01:44:59.000000 didppy-0.3.4/src/model/state.rs
--rw-r--r--   0      501       20   172084 2023-05-13 01:44:59.000000 didppy-0.3.4/src/model/table.rs
--rw-r--r--   0      501       20    44254 2023-05-13 01:44:59.000000 didppy-0.3.4/src/model/transition.rs
--rw-r--r--   0      501       20   543965 2023-05-13 01:44:59.000000 didppy-0.3.4/src/model.rs
--rw-r--r--   0      501       20     2741 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_acps.py
--rw-r--r--   0      501       20     2741 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_apps.py
--rw-r--r--   0      501       20     2687 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_bradth_first_search.py
--rw-r--r--   0      501       20     2627 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_caasdy.py
--rw-r--r--   0      501       20     2561 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_cabs.py
--rw-r--r--   0      501       20     2617 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_cbfs.py
--rw-r--r--   0      501       20     2658 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_dbdfs.py
--rw-r--r--   0      501       20     2617 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_dfbb.py
--rw-r--r--   0      501       20     1565 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_dijkstra.py
--rw-r--r--   0      501       20     1613 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_expression_beam_search.py
--rw-r--r--   0      501       20     1589 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_forward_recursion.py
--rw-r--r--   0      501       20     2727 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/heuristic_search_solver/test_weighted_astar.py
--rw-r--r--   0      501       20    85219 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/model/test_expression.py
--rw-r--r--   0      501       20     6576 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/model/test_state.py
--rw-r--r--   0      501       20    66254 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/model/test_table.py
--rw-r--r--   0      501       20    16456 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/model/test_transition.py
--rw-r--r--   0      501       20    54164 2023-05-13 01:44:59.000000 didppy-0.3.4/tests/test_model.py
--rw-r--r--   0      501       20    12339 2023-05-13 01:44:59.000000 didppy-0.3.4/Cargo.lock
--rw-r--r--   0        0        0     2322 1970-01-01 00:00:00.000000 didppy-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      549 1970-01-01 00:00:00.000000 didppy-0.4.0/local_dependencies/dypdl/Cargo.toml
+-rw-r--r--   0      501       20     5194 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/README.md
+-rw-r--r--   0      501       20     9080 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/base_case.rs
+-rw-r--r--   0      501       20     1344 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/effect.rs
+-rw-r--r--   0      501       20    16931 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/argument_expression.rs
+-rw-r--r--   0      501       20    59188 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/condition.rs
+-rw-r--r--   0      501       20   290240 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/continuous_expression.rs
+-rw-r--r--   0      501       20    36620 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/continuous_vector_expression.rs
+-rw-r--r--   0      501       20    88634 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/element_expression.rs
+-rw-r--r--   0      501       20   134795 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/integer_expression.rs
+-rw-r--r--   0      501       20    25379 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/integer_vector_expression.rs
+-rw-r--r--   0      501       20    18114 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/numeric_operator.rs
+-rw-r--r--   0      501       20    62551 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/numeric_table_expression.rs
+-rw-r--r--   0      501       20     4969 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/reference_expression.rs
+-rw-r--r--   0      501       20    48744 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/set_condition.rs
+-rw-r--r--   0      501       20   114732 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/set_expression.rs
+-rw-r--r--   0      501       20   135581 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/set_reduce_expression.rs
+-rw-r--r--   0      501       20    15550 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/table_expression.rs
+-rw-r--r--   0      501       20    56292 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/table_vector_expression.rs
+-rw-r--r--   0      501       20     1787 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/util.rs
+-rw-r--r--   0      501       20    19963 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression/vector_expression.rs
+-rw-r--r--   0      501       20     1500 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/expression.rs
+-rw-r--r--   0      501       20    26414 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/grounded_condition.rs
+-rw-r--r--   0      501       20   671792 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/lib.rs
+-rw-r--r--   0      501       20   131319 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/state.rs
+-rw-r--r--   0      501       20    18956 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/table.rs
+-rw-r--r--   0      501       20    46003 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/table_data.rs
+-rw-r--r--   0      501       20    84395 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/table_registry.rs
+-rw-r--r--   0      501       20    57672 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/transition.rs
+-rw-r--r--   0      501       20      438 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/util.rs
+-rw-r--r--   0      501       20     3476 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl/src/variable_type.rs
+-rw-r--r--   0        0        0      578 1970-01-01 00:00:00.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/Cargo.toml
+-rw-r--r--   0      501       20     1631 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/README.md
+-rw-r--r--   0      501       20     4995 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/caasdy.rs
+-rw-r--r--   0      501       20     5025 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_acps.rs
+-rw-r--r--   0      501       20     4970 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_apps.rs
+-rw-r--r--   0      501       20     4699 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_breadth_first_search.rs
+-rw-r--r--   0      501       20     5107 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_cabs.rs
+-rw-r--r--   0      501       20     4706 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_cbfs.rs
+-rw-r--r--   0      501       20     4778 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_dbdfs.rs
+-rw-r--r--   0      501       20     4472 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_dfbb.rs
+-rw-r--r--   0      501       20     4807 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_weighted_astar.rs
+-rw-r--r--   0      501       20     7488 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/expression_beam_search.rs
+-rw-r--r--   0      501       20     1717 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/f_evaluator_type.rs
+-rw-r--r--   0      501       20     1230 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/lib.rs
+-rw-r--r--   0      501       20    13643 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/acps.rs
+-rw-r--r--   0      501       20    13189 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/apps.rs
+-rw-r--r--   0      501       20    10454 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/beam_search.rs
+-rw-r--r--   0      501       20     9953 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/best_first_search.rs
+-rw-r--r--   0      501       20    11475 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/breadth_first_search.rs
+-rw-r--r--   0      501       20    10748 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cabs.rs
+-rw-r--r--   0      501       20    10449 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cbfs.rs
+-rw-r--r--   0      501       20    15763 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam.rs
+-rw-r--r--   0      501       20    47180 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/hashable_state.rs
+-rw-r--r--   0      501       20      835 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/bfs_node.rs
+-rw-r--r--   0      501       20    28848 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/cost_node.rs
+-rw-r--r--   0      501       20    34204 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/custom_f_node.rs
+-rw-r--r--   0      501       20    48547 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/f_node.rs
+-rw-r--r--   0      501       20    52543 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node/weighted_f_node.rs
+-rw-r--r--   0      501       20      237 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/search_node.rs
+-rw-r--r--   0      501       20    63006 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/state_registry.rs
+-rw-r--r--   0      501       20    20278 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/successor_generator.rs
+-rw-r--r--   0      501       20    12373 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_custom_cost.rs
+-rw-r--r--   0      501       20    10595 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition/transition_with_id.rs
+-rw-r--r--   0      501       20      167 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition.rs
+-rw-r--r--   0      501       20     3808 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_chain.rs
+-rw-r--r--   0      501       20     1971 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/util.rs
+-rw-r--r--   0      501       20      713 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure.rs
+-rw-r--r--   0      501       20    11942 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dbdfs.rs
+-rw-r--r--   0      501       20     9330 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dfbb.rs
+-rw-r--r--   0      501       20     7031 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/forward_recursion.rs
+-rw-r--r--   0      501       20    27771 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/rollout.rs
+-rw-r--r--   0      501       20     4791 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/search.rs
+-rw-r--r--   0      501       20    11386 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/util.rs
+-rw-r--r--   0      501       20      988 2023-05-25 22:02:32.000000 didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm.rs
+-rw-r--r--   0        0        0      920 1970-01-01 00:00:00.000000 didppy-0.4.0/Cargo.toml
+-rw-r--r--   0      501       20      705 2023-05-25 22:02:32.000000 didppy-0.4.0/.gitignore
+-rw-r--r--   0      501       20     1872 2023-05-25 22:02:32.000000 didppy-0.4.0/README.md
+-rw-r--r--   0      501       20       71 2023-05-25 22:02:32.000000 didppy-0.4.0/build.rs
+-rw-r--r--   0      501       20      634 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/Makefile
+-rw-r--r--   0      501       20    29958 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/_static/images/TSPTW.png
+-rw-r--r--   0      501       20      645 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0      501       20     8470 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/advanced-tutorials/forced-transitions.rst
+-rw-r--r--   0      501       20     6060 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/advanced-tutorials/general-cost.rst
+-rw-r--r--   0      501       20      250 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/advanced-tutorials.rst
+-rw-r--r--   0      501       20     1912 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/api-reference.rst
+-rw-r--r--   0      501       20     2246 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/conf.py
+-rw-r--r--   0      501       20     4189 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/debugging/common-mistakes.rst
+-rw-r--r--   0      501       20     5939 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/debugging/state.rst
+-rw-r--r--   0      501       20     2881 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/debugging/validate.rst
+-rw-r--r--   0      501       20      255 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/debugging.rst
+-rw-r--r--   0      501       20     2237 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/examples.rst
+-rw-r--r--   0      501       20     1086 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/index.rst
+-rw-r--r--   0      501       20      800 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/make.bat
+-rw-r--r--   0      501       20     1494 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/papers.rst
+-rw-r--r--   0      501       20     4205 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/quickstart.rst
+-rw-r--r--   0      501       20     7668 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/ref.bib
+-rw-r--r--   0      501       20       67 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/references.rst
+-rw-r--r--   0      501       20       45 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/requirements.txt
+-rw-r--r--   0      501       20     4797 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/solver-selection.rst
+-rw-r--r--   0      501       20    28927 2023-05-25 22:02:32.000000 didppy-0.4.0/docs/tutorial.rst
+-rw-r--r--   0      501       20     2617 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/README.md
+-rw-r--r--   0      501       20    10351 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/bin-packing.ipynb
+-rw-r--r--   0      501       20     9197 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/cvrp.ipynb
+-rw-r--r--   0      501       20     5970 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/graph-clear.ipynb
+-rw-r--r--   0      501       20     4927 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/knapsack.ipynb
+-rw-r--r--   0      501       20     9316 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/m-pdtsp.ipynb
+-rw-r--r--   0      501       20     6931 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/mosp.ipynb
+-rw-r--r--   0      501       20     9948 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/salbp-1.ipynb
+-rw-r--r--   0      501       20     5314 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/single-machine.ipynb
+-rw-r--r--   0      501       20     7687 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/talent-scheduling.ipynb
+-rw-r--r--   0      501       20     8114 2023-05-25 22:02:32.000000 didppy-0.4.0/examples/tsptw.ipynb
+-rw-r--r--   0      501       20      582 2023-05-25 22:02:32.000000 didppy-0.4.0/pyproject.toml
+-rw-r--r--   0      501       20     9328 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/acps.rs
+-rw-r--r--   0      501       20     9251 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/apps.rs
+-rw-r--r--   0      501       20     8726 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/breadth_first_search.rs
+-rw-r--r--   0      501       20     8606 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/caasdy.rs
+-rw-r--r--   0      501       20     9260 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/cabs.rs
+-rw-r--r--   0      501       20     8297 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/cbfs.rs
+-rw-r--r--   0      501       20     8792 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/dbdfs.rs
+-rw-r--r--   0      501       20     8235 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/dfbb.rs
+-rw-r--r--   0      501       20    13995 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/expression_beam_search.rs
+-rw-r--r--   0      501       20     1755 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/f_operator.rs
+-rw-r--r--   0      501       20     3804 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/forward_recursion.rs
+-rw-r--r--   0      501       20     8314 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/weighted_astar.rs
+-rw-r--r--   0      501       20     6297 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver/wrapped_solver.rs
+-rw-r--r--   0      501       20      684 2023-05-25 22:02:32.000000 didppy-0.4.0/src/heuristic_search_solver.rs
+-rw-r--r--   0      501       20     2914 2023-05-25 22:02:32.000000 didppy-0.4.0/src/lib.rs
+-rw-r--r--   0      501       20   377271 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model/expression.rs
+-rw-r--r--   0      501       20     4897 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model/state.rs
+-rw-r--r--   0      501       20   172084 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model/table.rs
+-rw-r--r--   0      501       20    44011 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model/transition.rs
+-rw-r--r--   0      501       20   546337 2023-05-25 22:02:32.000000 didppy-0.4.0/src/model.rs
+-rw-r--r--   0      501       20     2741 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_acps.py
+-rw-r--r--   0      501       20     2741 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_apps.py
+-rw-r--r--   0      501       20     2687 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_bradth_first_search.py
+-rw-r--r--   0      501       20     2627 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_caasdy.py
+-rw-r--r--   0      501       20     2561 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_cabs.py
+-rw-r--r--   0      501       20     2617 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_cbfs.py
+-rw-r--r--   0      501       20     2658 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_dbdfs.py
+-rw-r--r--   0      501       20     2617 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_dfbb.py
+-rw-r--r--   0      501       20     1613 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_expression_beam_search.py
+-rw-r--r--   0      501       20     1589 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_forward_recursion.py
+-rw-r--r--   0      501       20     2727 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/heuristic_search_solver/test_weighted_astar.py
+-rw-r--r--   0      501       20    85219 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/model/test_expression.py
+-rw-r--r--   0      501       20     6576 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/model/test_state.py
+-rw-r--r--   0      501       20    66254 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/model/test_table.py
+-rw-r--r--   0      501       20    16456 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/model/test_transition.py
+-rw-r--r--   0      501       20    56856 2023-05-25 22:02:32.000000 didppy-0.4.0/tests/test_model.py
+-rw-r--r--   0      501       20    12339 2023-05-25 22:02:32.000000 didppy-0.4.0/Cargo.lock
+-rw-r--r--   0        0        0     2532 1970-01-01 00:00:00.000000 didppy-0.4.0/PKG-INFO
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl/README.md` & `didppy-0.4.0/local_dependencies/dypdl/README.md`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/effect.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/effect.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/argument_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/argument_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/condition.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/condition.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/continuous_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/continuous_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/continuous_vector_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/continuous_vector_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/element_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/element_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/integer_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/integer_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/integer_vector_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/integer_vector_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/numeric_operator.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/numeric_operator.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/numeric_table_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/numeric_table_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/reference_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/reference_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/set_condition.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/set_condition.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/set_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/set_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/set_reduce_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/set_reduce_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/table_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/table_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/table_vector_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/table_vector_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/util.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/util.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression/vector_expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression/vector_expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/expression.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/expression.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/grounded_condition.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/grounded_condition.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/lib.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/lib.rs`

 * *Files 1% similar despite different names*

```diff
@@ -227,15 +227,15 @@
     /// Tables of constants.
     pub table_registry: TableRegistry,
     /// State constraints.
     pub state_constraints: Vec<GroundedCondition>,
     /// Base cases.
     pub base_cases: Vec<BaseCase>,
     /// Explicit definitions of base states.
-    pub base_states: Vec<State>,
+    pub base_states: Vec<(State, Option<CostExpression>)>,
     /// Specifying how to compute the value of a state from applicable transitions.
     pub reduce_function: ReduceFunction,
     /// Type of the cost.
     pub cost_type: CostType,
     /// Forward transitions.
     pub forward_transitions: Vec<Transition>,
     /// Forward forced transitions.
@@ -302,18 +302,68 @@
     pub fn is_base<U: StateInterface>(&self, state: &U) -> bool {
         self.base_cases
             .iter()
             .any(|case| case.is_satisfied(state, &self.table_registry))
             || self
                 .base_states
                 .iter()
-                .any(|base| base.is_satisfied(state, &self.state_metadata))
+                .any(|(base, _)| base.is_satisfied(state, &self.state_metadata))
     }
 
-    /// Evaluate the dual bound given a state.
+    /// Evaluates the base cost given a state.
+    ///
+    /// Returns `None` if the state does not satisfy any base case.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// use dypdl::prelude::*;
+    ///
+    /// let mut model = Model::default();
+    /// let variable = model.add_integer_variable("variable", 2).unwrap();
+    /// let state = model.target.clone();
+    ///
+    /// let a = Condition::comparison_i(ComparisonOperator::Ge, variable, 0);
+    /// let b = Condition::comparison_i(ComparisonOperator::Le, variable, 1);
+    /// model.add_base_case(vec![a, b]).unwrap();
+    /// assert!(!model.is_base(&state));
+    ///
+    /// let a = Condition::comparison_i(ComparisonOperator::Ge, variable, 0);
+    /// let b = Condition::comparison_i(ComparisonOperator::Le, variable, 2);
+    /// model.add_base_case(vec![a, b]).unwrap();
+    /// assert!(model.is_base(&state));
+    /// ```
+    pub fn eval_base_cost<T: variable_type::Numeric + Ord, U: StateInterface>(
+        &self,
+        state: &U,
+    ) -> Option<T> {
+        let costs = self
+            .base_cases
+            .iter()
+            .filter_map(|case| case.eval_cost(state, &self.table_registry))
+            .chain(self.base_states.iter().filter_map(|(base, cost)| {
+                if base.is_satisfied(state, &self.state_metadata) {
+                    Some(
+                        cost.as_ref()
+                            .map_or_else(T::zero, |cost| cost.eval(state, &self.table_registry)),
+                    )
+                } else {
+                    None
+                }
+            }));
+
+        match self.reduce_function {
+            ReduceFunction::Min => costs.min(),
+            ReduceFunction::Max => costs.max(),
+            ReduceFunction::Sum => costs.reduce(|acc, e| acc + e),
+            ReduceFunction::Product => costs.reduce(|acc, e| acc * e),
+        }
+    }
+
+    /// Evaluates the dual bound given a state.
     ///
     /// # Panics
     ///
     /// Panics if the cost of the transitioned state is used or a min/max reduce operation is performed on an empty set or vector in a dual bound.
     ///
     /// # Examples
     ///
@@ -385,31 +435,31 @@
     >(
         &self,
         state: &S,
         cost: U,
         transition: &T,
         cost_bound: Option<U>,
     ) -> Option<(R, U)> {
+        let successor = transition.apply(state, &self.table_registry);
+
+        if !self.check_constraints(&successor) {
+            return None;
+        }
+
         let successor_cost = transition.eval_cost(cost, state, &self.table_registry);
 
         if cost_bound.map_or(false, |bound| match self.reduce_function {
             ReduceFunction::Max => successor_cost <= bound,
             ReduceFunction::Min => successor_cost >= bound,
             _ => false,
         }) {
             return None;
         }
 
-        let successor = transition.apply(state, &self.table_registry);
-
-        if self.check_constraints(&successor) {
-            Some((successor, successor_cost))
-        } else {
-            None
-        }
+        Some((successor, successor_cost))
     }
 
     /// Validate a solution consists of forward transitions.
     ///
     /// # Panics
     ///
     /// Panics if the cost of the transitioned state is used or a min/max reduce operation is performed on an empty set or vector in a precondition or an effect of a transition.
@@ -426,23 +476,29 @@
     /// transition.set_cost(IntegerExpression::Cost + 1);
     ///
     /// let transitions = [transition];
     /// let cost = 1;
     ///
     /// assert!(model.validate_forward(&transitions, cost, true));
     /// ```
-    pub fn validate_forward<T: variable_type::Numeric + fmt::Display>(
+    pub fn validate_forward<T: variable_type::Numeric + fmt::Display + Ord>(
         &self,
         transitions: &[Transition],
         cost: T,
         show_message: bool,
     ) -> bool {
         let mut state_vec = vec![self.target.clone()];
         for (i, transition) in transitions.iter().enumerate() {
             let state = state_vec.last().unwrap();
+            if self.is_base(state) {
+                if show_message {
+                    println!("The {} th state satisfies a base case while there are {} transitions left.", i, transitions.len() - i);
+                }
+                return false;
+            }
             if !transition.is_applicable(state, &self.table_registry) {
                 if show_message {
                     println!(
                         "The {} th transition {} is not applicable.",
                         i,
                         transition.get_full_name()
                     );
@@ -454,21 +510,23 @@
                 if show_message {
                     println!("The {} th state does not satisfy state constraints", i + 1);
                 }
                 return false;
             }
             state_vec.push(next_state);
         }
-        if !self.is_base(state_vec.last().unwrap()) {
+        let mut validation_cost = if let Some(cost) = self.eval_base_cost(state_vec.last().unwrap())
+        {
+            cost
+        } else {
             if show_message {
                 println!("The last state is not a base state.")
             }
             return false;
-        }
-        let mut validation_cost = T::zero();
+        };
         state_vec.pop();
         for (state, transition) in state_vec.into_iter().zip(transitions).rev() {
             validation_cost = transition.eval_cost(validation_cost, &state, &self.table_registry);
         }
         if cost != validation_cost && show_message {
             println!("The cost {} does not match the actual cost {}. This is possibly due to the cost is continuous.", cost, validation_cost)
         }
@@ -656,15 +714,15 @@
 
     /// Adds and returns an element variable.
     ///
     /// The value in the target state must be specified.
     ///
     /// # Errors
     ///
-    /// If the name is already used, the object type is not in the model, or the target value is greater than or equal to the number of the objects.
+    /// If the name is already used, or the object type is not in the model.
     ///
     /// # Examples
     ///
     /// ```
     /// use dypdl::prelude::*;
     ///
     /// let mut model = Model::default();
@@ -677,29 +735,20 @@
         name: T,
         ob: ObjectType,
         target: Element,
     ) -> Result<ElementVariable, ModelErr>
     where
         String: From<T>,
     {
-        let n = self.get_number_of_objects(ob)?;
-        if target >= n {
-            Err(ModelErr::new(format!(
-                "target value for element variable {} >= #objects ({})",
-                String::from(name),
-                n
-            )))
-        } else {
-            let v = self.state_metadata.add_element_variable(name, ob)?;
-            self.target
-                .signature_variables
-                .element_variables
-                .push(target);
-            Ok(v)
-        }
+        let v = self.state_metadata.add_element_variable(name, ob)?;
+        self.target
+            .signature_variables
+            .element_variables
+            .push(target);
+        Ok(v)
     }
 
     /// Returns an element resource variable given a name.
     ///
     /// # Errors
     ///
     /// If no such variable.
@@ -725,15 +774,15 @@
 
     /// Adds and returns an element resource variable.
     ///
     /// The value in the target state must be specified.
     ///
     /// # Errors
     ///
-    /// If the name is already used, the object type is not in the model, or the target value is greater than or equal to the number of the objects.
+    /// If the name is already used, or the object type is not in the model.
     ///
     /// # Examples
     ///
     /// ```
     /// use dypdl::prelude::*;
     ///
     /// let mut model = Model::default();
@@ -747,31 +796,22 @@
         ob: ObjectType,
         less_is_better: bool,
         target: Element,
     ) -> Result<ElementResourceVariable, ModelErr>
     where
         String: From<T>,
     {
-        let n = self.get_number_of_objects(ob)?;
-        if target >= n {
-            Err(ModelErr::new(format!(
-                "target value for element resource variable {} >= #objects ({})",
-                String::from(name),
-                n
-            )))
-        } else {
-            let v = self
-                .state_metadata
-                .add_element_resource_variable(name, ob, less_is_better)?;
-            self.target
-                .resource_variables
-                .element_variables
-                .push(target);
-            Ok(v)
-        }
+        let v = self
+            .state_metadata
+            .add_element_resource_variable(name, ob, less_is_better)?;
+        self.target
+            .resource_variables
+            .element_variables
+            .push(target);
+        Ok(v)
     }
 
     /// Returns a set variable given a name.
     ///
     /// # Errors
     ///
     /// If no such variable.
@@ -1163,16 +1203,44 @@
             _ => {}
         }
         self.state_constraints
             .push(GroundedCondition::from(simplified));
         Ok(())
     }
 
+    fn check_and_simplify_conditions(
+        &self,
+        conditions: Vec<expression::Condition>,
+    ) -> Result<Vec<GroundedCondition>, ModelErr> {
+        let mut simplified_conditions = Vec::with_capacity(conditions.len());
+
+        for condition in conditions {
+            self.check_expression(&condition, false)?;
+            let simplified = condition.simplify(&self.table_registry);
+
+            match simplified {
+                expression::Condition::Constant(true) => {
+                    eprintln!("base case condition {:?} is always satisfied", condition)
+                }
+                expression::Condition::Constant(false) => {
+                    eprintln!("base case condition {:?} cannot be satisfied", condition)
+                }
+                _ => {}
+            }
+
+            simplified_conditions.push(GroundedCondition::from(simplified));
+        }
+
+        Ok(simplified_conditions)
+    }
+
     /// Adds a base case.
     ///
+    /// The cost of a base case is assumed to be zero.
+    ///
     /// # Errors
     ///
     /// If a condition is invalid, e.g., it uses variables not existing in this model or the state of the transitioned state.
     ///
     /// # Examples
     ///
     /// ```
@@ -1186,59 +1254,114 @@
     /// assert!(model.add_base_case(vec![a, b]).is_ok());
     /// ```
     #[inline]
     pub fn add_base_case(
         &mut self,
         conditions: Vec<expression::Condition>,
     ) -> Result<(), ModelErr> {
-        let mut simplified_conditions = Vec::with_capacity(conditions.len());
-        for condition in &conditions {
-            self.check_expression(condition, false)?;
-            let simplified = condition.simplify(&self.table_registry);
-            match simplified {
-                expression::Condition::Constant(true) => {
-                    eprintln!("base case condition {:?} is always satisfied", condition)
-                }
-                expression::Condition::Constant(false) => {
-                    eprintln!("base case condition {:?} cannot be satisfied", condition)
-                }
-                _ => {}
+        let conditions = self.check_and_simplify_conditions(conditions)?;
+        self.base_cases.push(BaseCase::from(conditions));
+        Ok(())
+    }
+
+    fn check_and_simplify_cost<T>(
+        &self,
+        cost: T,
+        allow_cost: bool,
+    ) -> Result<CostExpression, ModelErr>
+    where
+        CostExpression: From<T>,
+    {
+        match CostExpression::from(cost) {
+            CostExpression::Integer(cost) => {
+                self.check_expression(&cost, allow_cost)?;
+                Ok(cost.simplify(&self.table_registry).into())
+            }
+            CostExpression::Continuous(cost) => {
+                self.check_expression(&cost, allow_cost)?;
+                Ok(cost.simplify(&self.table_registry).into())
             }
-            simplified_conditions.push(simplified);
         }
-        self.base_cases.push(BaseCase::new(
-            simplified_conditions
-                .into_iter()
-                .map(GroundedCondition::from)
-                .collect(),
-        ));
+    }
+
+    /// Adds a base case with its cost.
+    ///
+    /// # Errors
+    ///
+    /// If a condition is invalid, e.g., it uses variables not existing in this model or the state of the transitioned state.
+    ///
+    /// # Examples
+    ///
+    /// ```
+    /// use dypdl::prelude::*;
+    ///
+    /// let mut model = Model::default();
+    /// let variable = model.add_integer_variable("variable", 2).unwrap();
+    ///
+    /// let a = Condition::comparison_i(ComparisonOperator::Ge, variable, 0);
+    /// let b = Condition::comparison_i(ComparisonOperator::Le, variable, 1);
+    /// let cost = 1;
+    /// assert!(model.add_base_case_with_cost(vec![a, b], 1).is_ok());
+    /// ```
+    #[inline]
+    pub fn add_base_case_with_cost<T>(
+        &mut self,
+        conditions: Vec<expression::Condition>,
+        cost: T,
+    ) -> Result<(), ModelErr>
+    where
+        CostExpression: From<T>,
+    {
+        let conditions = self.check_and_simplify_conditions(conditions)?;
+        let cost = self.check_and_simplify_cost(cost, false)?;
+        self.base_cases
+            .push(BaseCase::with_cost::<CostExpression>(conditions, cost));
         Ok(())
     }
 
     /// Check if a state is valid.
     ///
     /// # Errors
     ///
     /// If a state is invalid, e.g., it contains variables not existing in this model.
+    #[inline]
     pub fn check_state<'a, T: StateInterface>(&self, state: &'a T) -> Result<(), ModelErr>
     where
         &'a T: panic::UnwindSafe,
     {
         self.state_metadata.check_state(state)
     }
 
     /// Adds a base state.
     ///
+    /// The cost of the state is assumed to be zero.
+    ///
     /// # Errors
     ///
     /// If a state is invalid, e.g., it contains variables not existing in this model.
     #[inline]
     pub fn add_base_state(&mut self, state: State) -> Result<(), ModelErr> {
         self.check_state(&state)?;
-        self.base_states.push(state);
+        self.base_states.push((state, None));
+        Ok(())
+    }
+
+    /// Adds a base state with its cost.
+    ///
+    /// # Errors
+    ///
+    /// If a state is invalid, e.g., it contains variables not existing in this model.
+    #[inline]
+    pub fn add_base_state_with_cost<T>(&mut self, state: State, cost: T) -> Result<(), ModelErr>
+    where
+        CostExpression: From<T>,
+    {
+        self.check_state(&state)?;
+        let cost = self.check_and_simplify_cost(cost, false)?;
+        self.base_states.push((state, Some(cost)));
         Ok(())
     }
 
     /// Returns the reduce function.
     #[inline]
     pub fn get_reduce_function(&self) -> ReduceFunction {
         self.reduce_function.clone()
@@ -1790,42 +1913,24 @@
     /// # Errors
     ///
     /// If the variable is not in the model.
     fn set_target(&mut self, variable: T, target: U) -> Result<(), ModelErr>;
 }
 
 impl AccessTarget<ElementVariable, Element> for Model {
-    /// Returns the value in the target state.
-    ///
-    /// # Errors
-    ///
-    /// If the variable is not in the model.
     fn get_target(&self, variable: ElementVariable) -> Result<Element, ModelErr> {
         self.state_metadata.check_variable(variable)?;
         Ok(self.target.get_element_variable(variable.id()))
     }
 
-    /// Set the value in the target state
-    ///
-    /// # Errors
-    ///
-    /// If the variable is not in the model.
     fn set_target(&mut self, variable: ElementVariable, target: Element) -> Result<(), ModelErr> {
         let ob = self.get_object_type_of(variable)?;
-        let n = self.get_number_of_objects(ob)?;
-        if target >= n {
-            Err(ModelErr::new(format!(
-                "target value for element variable id {} >= #objects ({})",
-                variable.id(),
-                n
-            )))
-        } else {
-            self.target.signature_variables.element_variables[variable.id()] = target;
-            Ok(())
-        }
+        let _ = self.get_number_of_objects(ob)?;
+        self.target.signature_variables.element_variables[variable.id()] = target;
+        Ok(())
     }
 }
 
 impl AccessTarget<ElementResourceVariable, Element> for Model {
     fn get_target(&self, variable: ElementResourceVariable) -> Result<Element, ModelErr> {
         self.state_metadata.check_variable(variable)?;
         Ok(self.target.get_element_resource_variable(variable.id()))
@@ -1833,25 +1938,17 @@
 
     fn set_target(
         &mut self,
         variable: ElementResourceVariable,
         target: Element,
     ) -> Result<(), ModelErr> {
         let ob = self.get_object_type_of(variable)?;
-        let n = self.get_number_of_objects(ob)?;
-        if target >= n {
-            Err(ModelErr::new(format!(
-                "target value for element variable id {} >= #objects ({})",
-                variable.id(),
-                n
-            )))
-        } else {
-            self.target.resource_variables.element_variables[variable.id()] = target;
-            Ok(())
-        }
+        let _ = self.get_number_of_objects(ob)?;
+        self.target.resource_variables.element_variables[variable.id()] = target;
+        Ok(())
     }
 }
 
 impl AccessTarget<SetVariable, Set> for Model {
     fn get_target(&self, variable: SetVariable) -> Result<Set, ModelErr> {
         self.state_metadata.check_variable(variable)?;
         Ok(self.target.get_set_variable(variable.id()).clone())
@@ -3049,44 +3146,257 @@
             ],
             ..Default::default()
         };
         assert!(!model.check_constraints(&state));
     }
 
     #[test]
-    fn is_base() {
+    fn is_base_case() {
         let state = state::State::default();
         let model = Model {
-            base_cases: vec![BaseCase::new(vec![GroundedCondition {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::Constant(true),
                 ..Default::default()
             }])],
             ..Default::default()
         };
         assert!(model.is_base(&state));
+    }
+
+    #[test]
+    fn is_not_base_case() {
+        let state = state::State::default();
         let model = Model {
-            base_cases: vec![BaseCase::new(vec![GroundedCondition {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::Constant(false),
                 ..Default::default()
             }])],
             ..Default::default()
         };
         assert!(!model.is_base(&state));
+    }
+
+    #[test]
+    fn is_base_state() {
+        let state = state::State::default();
         let model = Model {
-            base_cases: vec![BaseCase::new(vec![GroundedCondition {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::Constant(false),
                 ..Default::default()
             }])],
-            base_states: vec![state::State::default()],
+            base_states: vec![(state::State::default(), None)],
             ..Default::default()
         };
         assert!(model.is_base(&state));
     }
 
     #[test]
+    fn eval_base_cost_zero() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(false),
+                        ..Default::default()
+                    }],
+                    1,
+                ),
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(true),
+                        ..Default::default()
+                    }],
+                    2,
+                ),
+            ],
+            base_states: vec![(state::State::default(), None)],
+            reduce_function: ReduceFunction::Min,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost(&state), Some(0));
+    }
+
+    #[test]
+    fn eval_base_cost_min_some() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(false),
+                        ..Default::default()
+                    }],
+                    1,
+                ),
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(true),
+                        ..Default::default()
+                    }],
+                    2,
+                ),
+            ],
+            base_states: vec![(state::State::default(), Some(CostExpression::from(3)))],
+            reduce_function: ReduceFunction::Min,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost(&state), Some(2));
+    }
+
+    #[test]
+    fn eval_base_cost_min_none() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![BaseCase::with_cost(
+                vec![GroundedCondition {
+                    condition: Condition::Constant(false),
+                    ..Default::default()
+                }],
+                1,
+            )],
+            reduce_function: ReduceFunction::Min,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost::<Integer, _>(&state), None);
+    }
+
+    #[test]
+    fn eval_base_cost_max_some() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(false),
+                        ..Default::default()
+                    }],
+                    1,
+                ),
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(true),
+                        ..Default::default()
+                    }],
+                    2,
+                ),
+            ],
+            base_states: vec![(state::State::default(), Some(CostExpression::from(3)))],
+            reduce_function: ReduceFunction::Max,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost(&state), Some(3));
+    }
+
+    #[test]
+    fn eval_base_cost_max_none() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![BaseCase::with_cost(
+                vec![GroundedCondition {
+                    condition: Condition::Constant(false),
+                    ..Default::default()
+                }],
+                1,
+            )],
+            reduce_function: ReduceFunction::Max,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost::<Integer, _>(&state), None);
+    }
+
+    #[test]
+    fn eval_base_cost_sum() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(false),
+                        ..Default::default()
+                    }],
+                    1,
+                ),
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(true),
+                        ..Default::default()
+                    }],
+                    2,
+                ),
+            ],
+            base_states: vec![(state::State::default(), Some(CostExpression::from(3)))],
+            reduce_function: ReduceFunction::Sum,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost(&state), Some(5));
+    }
+
+    #[test]
+    fn eval_base_cost_sum_none() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![BaseCase::with_cost(
+                vec![GroundedCondition {
+                    condition: Condition::Constant(false),
+                    ..Default::default()
+                }],
+                1,
+            )],
+            reduce_function: ReduceFunction::Sum,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost::<Integer, _>(&state), None);
+    }
+
+    #[test]
+    fn eval_base_cost_product() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(false),
+                        ..Default::default()
+                    }],
+                    1,
+                ),
+                BaseCase::with_cost(
+                    vec![GroundedCondition {
+                        condition: Condition::Constant(true),
+                        ..Default::default()
+                    }],
+                    2,
+                ),
+            ],
+            base_states: vec![(state::State::default(), Some(CostExpression::from(3)))],
+            reduce_function: ReduceFunction::Product,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost(&state), Some(6));
+    }
+
+    #[test]
+    fn eval_base_cost_product_none() {
+        let state = state::State::default();
+        let model = Model {
+            base_cases: vec![BaseCase::with_cost(
+                vec![GroundedCondition {
+                    condition: Condition::Constant(false),
+                    ..Default::default()
+                }],
+                1,
+            )],
+            reduce_function: ReduceFunction::Product,
+            ..Default::default()
+        };
+        assert_eq!(model.eval_base_cost::<Integer, _>(&state), None);
+    }
+
+    #[test]
     fn has_resource_variables() {
         let model = Model::default();
         assert!(!model.has_resource_variables());
         let model = Model {
             state_metadata: StateMetadata {
                 integer_resource_variable_names: vec![String::from("v")],
                 integer_less_is_better: vec![true],
@@ -3506,15 +3816,15 @@
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(0)),
                 ),
                 ..Default::default()
             }],
-            base_cases: vec![BaseCase::new(vec![GroundedCondition {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(2)),
                 ),
                 ..Default::default()
             }])],
@@ -3584,14 +3894,220 @@
             model.forward_forced_transitions[0].clone(),
             model.forward_transitions[0].clone(),
         ];
         assert!(model.validate_forward(&transitions, 1, true));
     }
 
     #[test]
+    fn validate_forward_true_base_cost() {
+        let name_to_integer_variable = FxHashMap::default();
+        let model = Model {
+            state_metadata: StateMetadata {
+                integer_variable_names: vec![String::from("v1")],
+                name_to_integer_variable,
+                ..Default::default()
+            },
+            target: State {
+                signature_variables: SignatureVariables {
+                    integer_variables: vec![0],
+                    ..Default::default()
+                },
+                ..Default::default()
+            },
+            state_constraints: vec![GroundedCondition {
+                condition: Condition::ComparisonI(
+                    ComparisonOperator::Ge,
+                    Box::new(IntegerExpression::Variable(0)),
+                    Box::new(IntegerExpression::Constant(0)),
+                ),
+                ..Default::default()
+            }],
+            base_cases: vec![BaseCase::with_cost(
+                vec![GroundedCondition {
+                    condition: Condition::ComparisonI(
+                        ComparisonOperator::Ge,
+                        Box::new(IntegerExpression::Variable(0)),
+                        Box::new(IntegerExpression::Constant(2)),
+                    ),
+                    ..Default::default()
+                }],
+                1,
+            )],
+            forward_transitions: vec![
+                Transition {
+                    name: String::from("increase"),
+                    effect: Effect {
+                        integer_effects: vec![(
+                            0,
+                            IntegerExpression::BinaryOperation(
+                                BinaryOperator::Add,
+                                Box::new(IntegerExpression::Variable(0)),
+                                Box::new(IntegerExpression::Constant(1)),
+                            ),
+                        )],
+                        ..Default::default()
+                    },
+                    cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
+                        BinaryOperator::Add,
+                        Box::new(IntegerExpression::Cost),
+                        Box::new(IntegerExpression::Constant(1)),
+                    )),
+                    ..Default::default()
+                },
+                Transition {
+                    name: String::from("decrease"),
+                    effect: Effect {
+                        integer_effects: vec![(
+                            0,
+                            IntegerExpression::BinaryOperation(
+                                BinaryOperator::Sub,
+                                Box::new(IntegerExpression::Variable(0)),
+                                Box::new(IntegerExpression::Constant(1)),
+                            ),
+                        )],
+                        ..Default::default()
+                    },
+                    cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
+                        BinaryOperator::Add,
+                        Box::new(IntegerExpression::Cost),
+                        Box::new(IntegerExpression::Constant(1)),
+                    )),
+                    ..Default::default()
+                },
+            ],
+            forward_forced_transitions: vec![Transition {
+                name: String::from("forced increase"),
+                preconditions: vec![GroundedCondition {
+                    condition: Condition::ComparisonI(
+                        ComparisonOperator::Eq,
+                        Box::new(IntegerExpression::Variable(0)),
+                        Box::new(IntegerExpression::Constant(0)),
+                    ),
+                    ..Default::default()
+                }],
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(1))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Cost),
+                ..Default::default()
+            }],
+            ..Default::default()
+        };
+
+        let transitions = vec![
+            model.forward_forced_transitions[0].clone(),
+            model.forward_transitions[0].clone(),
+        ];
+        assert!(model.validate_forward(&transitions, 2, true));
+    }
+
+    #[test]
+    fn validate_forward_base_case_false() {
+        let name_to_integer_variable = FxHashMap::default();
+        let model = Model {
+            state_metadata: StateMetadata {
+                integer_variable_names: vec![String::from("v1")],
+                name_to_integer_variable,
+                ..Default::default()
+            },
+            target: State {
+                signature_variables: SignatureVariables {
+                    integer_variables: vec![0],
+                    ..Default::default()
+                },
+                ..Default::default()
+            },
+            state_constraints: vec![GroundedCondition {
+                condition: Condition::ComparisonI(
+                    ComparisonOperator::Ge,
+                    Box::new(IntegerExpression::Variable(0)),
+                    Box::new(IntegerExpression::Constant(0)),
+                ),
+                ..Default::default()
+            }],
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
+                condition: Condition::ComparisonI(
+                    ComparisonOperator::Ge,
+                    Box::new(IntegerExpression::Variable(0)),
+                    Box::new(IntegerExpression::Constant(2)),
+                ),
+                ..Default::default()
+            }])],
+            forward_transitions: vec![
+                Transition {
+                    name: String::from("increase"),
+                    effect: Effect {
+                        integer_effects: vec![(
+                            0,
+                            IntegerExpression::BinaryOperation(
+                                BinaryOperator::Add,
+                                Box::new(IntegerExpression::Variable(0)),
+                                Box::new(IntegerExpression::Constant(1)),
+                            ),
+                        )],
+                        ..Default::default()
+                    },
+                    cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
+                        BinaryOperator::Add,
+                        Box::new(IntegerExpression::Cost),
+                        Box::new(IntegerExpression::Constant(1)),
+                    )),
+                    ..Default::default()
+                },
+                Transition {
+                    name: String::from("decrease"),
+                    effect: Effect {
+                        integer_effects: vec![(
+                            0,
+                            IntegerExpression::BinaryOperation(
+                                BinaryOperator::Sub,
+                                Box::new(IntegerExpression::Variable(0)),
+                                Box::new(IntegerExpression::Constant(1)),
+                            ),
+                        )],
+                        ..Default::default()
+                    },
+                    cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
+                        BinaryOperator::Add,
+                        Box::new(IntegerExpression::Cost),
+                        Box::new(IntegerExpression::Constant(1)),
+                    )),
+                    ..Default::default()
+                },
+            ],
+            forward_forced_transitions: vec![Transition {
+                name: String::from("forced increase"),
+                preconditions: vec![GroundedCondition {
+                    condition: Condition::ComparisonI(
+                        ComparisonOperator::Eq,
+                        Box::new(IntegerExpression::Variable(0)),
+                        Box::new(IntegerExpression::Constant(0)),
+                    ),
+                    ..Default::default()
+                }],
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(1))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Cost),
+                ..Default::default()
+            }],
+            ..Default::default()
+        };
+
+        let transitions = vec![
+            model.forward_forced_transitions[0].clone(),
+            model.forward_transitions[0].clone(),
+            model.forward_transitions[0].clone(),
+        ];
+        assert!(!model.validate_forward(&transitions, 1, true));
+    }
+
+    #[test]
     fn validate_forward_state_constraint_false() {
         let name_to_integer_variable = FxHashMap::default();
         let model = Model {
             state_metadata: StateMetadata {
                 integer_variable_names: vec![String::from("v1")],
                 name_to_integer_variable,
                 ..Default::default()
@@ -3607,15 +4123,15 @@
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(0)),
                 ),
                 ..Default::default()
             }],
-            base_cases: vec![BaseCase::new(vec![GroundedCondition {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(2)),
                 ),
                 ..Default::default()
             }])],
@@ -3692,15 +4208,15 @@
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(0)),
                 ),
                 ..Default::default()
             }],
-            base_cases: vec![BaseCase::new(vec![GroundedCondition {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(2)),
                 ),
                 ..Default::default()
             }])],
@@ -3793,15 +4309,15 @@
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(0)),
                 ),
                 ..Default::default()
             }],
-            base_cases: vec![BaseCase::new(vec![GroundedCondition {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(2)),
                 ),
                 ..Default::default()
             }])],
@@ -3891,15 +4407,15 @@
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(0)),
                 ),
                 ..Default::default()
             }],
-            base_cases: vec![BaseCase::new(vec![GroundedCondition {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(2)),
                 ),
                 ..Default::default()
             }])],
@@ -4051,18 +4567,14 @@
         assert!(ob.is_ok());
         let ob = ob.unwrap();
         let v = model.add_element_variable(String::from("v"), ob, 2);
         assert!(v.is_ok());
         let v = v.unwrap();
         let v2 = model.add_element_variable(String::from("v"), ob, 2);
         assert!(v2.is_err());
-        let v2 = model.add_element_variable(String::from("v2"), ob, 10);
-        assert!(v2.is_err());
-        let result = model.set_target(v, 10);
-        assert!(result.is_err());
 
         let mut model = Model::default();
         let v2 = model.add_element_variable(String::from("v3"), ob, 2);
         assert!(v2.is_err());
         let ob2 = model.get_object_type_of(v);
         assert!(ob2.is_err());
         let target = model.get_target(v);
@@ -4110,18 +4622,14 @@
         assert!(ob.is_ok());
         let ob = ob.unwrap();
         let v = model.add_element_resource_variable(String::from("v"), ob, true, 2);
         assert!(v.is_ok());
         let v = v.unwrap();
         let v2 = model.add_element_resource_variable(String::from("v"), ob, true, 2);
         assert!(v2.is_err());
-        let v2 = model.add_element_resource_variable(String::from("v2"), ob, true, 10);
-        assert!(v2.is_err());
-        let result = model.set_target(v, 10);
-        assert!(result.is_err());
 
         let mut model = Model::default();
         let v2 = model.add_element_resource_variable(String::from("v3"), ob, true, 2);
         assert!(v2.is_err());
         let ob2 = model.get_object_type_of(v);
         assert!(ob2.is_err());
         let target = model.get_target(v);
@@ -5984,15 +6492,15 @@
         let v = v.unwrap();
         let condition =
             Condition::comparison_i(ComparisonOperator::Ge, v, 3) & Condition::Constant(true);
         let result = model.add_base_case(vec![condition]);
         assert!(result.is_ok());
         assert_eq!(
             model.base_cases,
-            vec![BaseCase::new(vec![GroundedCondition {
+            vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(v.id())),
                     Box::new(IntegerExpression::Constant(3))
                 ),
                 ..Default::default()
             }])]
@@ -6009,14 +6517,65 @@
         let condition = Condition::comparison_i(ComparisonOperator::Ge, v, 0);
         let result = model.add_base_case(vec![condition]);
         assert!(result.is_err());
         assert_eq!(model.base_cases, vec![]);
     }
 
     #[test]
+    fn add_base_case_with_cost_ok() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable(String::from("v"), 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+        let condition =
+            Condition::comparison_i(ComparisonOperator::Ge, v, 3) & Condition::Constant(true);
+        let result = model.add_base_case_with_cost(vec![condition], 1);
+        assert!(result.is_ok());
+        assert_eq!(
+            model.base_cases,
+            vec![BaseCase::with_cost(
+                vec![GroundedCondition {
+                    condition: Condition::ComparisonI(
+                        ComparisonOperator::Ge,
+                        Box::new(IntegerExpression::Variable(v.id())),
+                        Box::new(IntegerExpression::Constant(3))
+                    ),
+                    ..Default::default()
+                }],
+                1
+            )]
+        )
+    }
+
+    #[test]
+    fn add_base_case_with_cost_err_conditions() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable(String::from("v"), 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+        let mut model = Model::default();
+        let condition = Condition::comparison_i(ComparisonOperator::Ge, v, 0);
+        let result = model.add_base_case_with_cost(vec![condition], 1);
+        assert!(result.is_err());
+        assert_eq!(model.base_cases, vec![]);
+    }
+
+    #[test]
+    fn add_base_case_with_cost_err_cost() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable(String::from("v"), 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+        let condition = Condition::comparison_i(ComparisonOperator::Ge, v, 3);
+        let result = model.add_base_case_with_cost(vec![condition], IntegerExpression::Cost);
+        assert!(result.is_err());
+        assert_eq!(model.base_cases, vec![]);
+    }
+
+    #[test]
     fn check_state_ok() {
         let mut model = Model::default();
         let v = model.add_integer_variable(String::from("v"), 0);
         assert!(v.is_ok());
         assert!(model.check_state(&model.target).is_ok());
     }
 
@@ -6032,28 +6591,63 @@
     #[test]
     fn add_base_state_ok() {
         let mut model = Model::default();
         let v = model.add_integer_variable(String::from("v"), 0);
         assert!(v.is_ok());
         let state = model.target.clone();
         assert!(model.add_base_state(state).is_ok());
-        assert_eq!(model.base_states, vec![model.target.clone()]);
+        assert_eq!(model.base_states, vec![(model.target.clone(), None)]);
     }
 
     #[test]
     fn add_base_state_err() {
         let mut model = Model::default();
         let v = model.add_integer_variable(String::from("v"), 0);
         assert!(v.is_ok());
         let state = State::default();
         assert!(model.add_base_state(state).is_err());
         assert_eq!(model.base_states, vec![]);
     }
 
     #[test]
+    fn add_base_state_with_cost_ok() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable(String::from("v"), 0);
+        assert!(v.is_ok());
+        let state = model.target.clone();
+        assert!(model.add_base_state_with_cost(state, 1).is_ok());
+        assert_eq!(
+            model.base_states,
+            vec![(model.target.clone(), Some(CostExpression::from(1)))]
+        );
+    }
+
+    #[test]
+    fn add_base_state_with_cost_err_state() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable(String::from("v"), 0);
+        assert!(v.is_ok());
+        let state = State::default();
+        assert!(model.add_base_state(state).is_err());
+        assert_eq!(model.base_states, vec![]);
+    }
+
+    #[test]
+    fn add_base_state_with_cost_err_cost() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable(String::from("v"), 0);
+        assert!(v.is_ok());
+        let state = model.target.clone();
+        assert!(model
+            .add_base_state_with_cost(state, IntegerExpression::Cost)
+            .is_err());
+        assert_eq!(model.base_states, vec![]);
+    }
+
+    #[test]
     fn reduce_function() {
         let mut model = Model {
             reduce_function: ReduceFunction::Min,
             ..Default::default()
         };
         assert_eq!(model.get_reduce_function(), ReduceFunction::Min);
         model.set_reduce_function(ReduceFunction::Max);
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/state.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/state.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1249,15 +1249,15 @@
             &mut self.element_variable_names,
             &mut self.name_to_element_variable,
         )?;
         self.element_variable_to_object.push(ob.id());
         Ok(ElementVariable(id))
     }
 
-    /// Returns an element resouce variable given a name.
+    /// Returns an element resource variable given a name.
     ///
     /// # Errors
     ///
     /// If no such variable.
     #[inline]
     pub fn get_element_resource_variable(
         &self,
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/table.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/table.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/table_data.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/table_data.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/table_registry.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/table_registry.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/transition.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/transition.rs`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 use crate::grounded_condition;
 use crate::state::{
     ContinuousResourceVariable, ContinuousVariable, ElementResourceVariable, ElementVariable,
     IntegerResourceVariable, IntegerVariable, SetVariable, State, StateInterface, VectorVariable,
 };
 use crate::table_registry;
 use crate::util::ModelErr;
-use crate::variable_type::{Element, FromNumeric, Numeric};
+use crate::variable_type::{Continuous, Element, FromNumeric, Numeric};
 use std::fmt::Debug;
 
 /// Wrapper for an integer expression or a continuous expression.
 #[derive(Debug, PartialEq, Clone)]
 pub enum CostExpression {
     /// Integer numeric expression.
     Integer(IntegerExpression),
@@ -25,26 +25,47 @@
 impl Default for CostExpression {
     /// Returns `CostExpression::Integer(IntegerExpression::Cost)`.
     fn default() -> Self {
         Self::Integer(IntegerExpression::Cost)
     }
 }
 
-impl From<IntegerExpression> for CostExpression {
-    fn from(cost: IntegerExpression) -> Self {
-        Self::Integer(cost)
+impl<T> From<T> for CostExpression
+where
+    IntegerExpression: From<T>,
+{
+    fn from(cost: T) -> Self {
+        Self::Integer(IntegerExpression::from(cost))
     }
 }
 
 impl From<ContinuousExpression> for CostExpression {
     fn from(cost: ContinuousExpression) -> Self {
         Self::Continuous(cost)
     }
 }
 
+impl From<Continuous> for CostExpression {
+    fn from(cost: Continuous) -> Self {
+        Self::from(ContinuousExpression::from(cost))
+    }
+}
+
+impl From<ContinuousVariable> for CostExpression {
+    fn from(cost: ContinuousVariable) -> Self {
+        Self::from(ContinuousExpression::from(cost))
+    }
+}
+
+impl From<ContinuousResourceVariable> for CostExpression {
+    fn from(cost: ContinuousResourceVariable) -> Self {
+        Self::from(ContinuousExpression::from(cost))
+    }
+}
+
 impl CostExpression {
     /// Returns the evaluation result.
     ///
     /// # Panics
     ///
     /// Panics if the cost of the transition state is used or a min/max reduce operation is performed on an empty set or vector.
     ///
@@ -499,14 +520,15 @@
 mod tests {
     use super::*;
     use crate::expression::*;
     use crate::state;
     use crate::table;
     use crate::table_data;
     use crate::variable_type::*;
+    use crate::StateMetadata;
     use rustc_hash::FxHashMap;
 
     fn generate_registry() -> table_registry::TableRegistry {
         let tables_1d = vec![table::Table1D::new(vec![10, 20, 30])];
         let mut name_to_table_1d = FxHashMap::default();
         name_to_table_1d.insert(String::from("f1"), 0);
 
@@ -555,25 +577,64 @@
     #[test]
     fn cost_expression_default() {
         let expression = CostExpression::default();
         assert_eq!(expression, CostExpression::Integer(IntegerExpression::Cost));
     }
 
     #[test]
-    fn cost_expression_from() {
+    fn cost_expression_from_integer() {
         let expression = CostExpression::from(IntegerExpression::Cost);
         assert_eq!(expression, CostExpression::Integer(IntegerExpression::Cost));
+    }
+
+    #[test]
+    fn cost_expression_from_continuous_expression() {
         let expression = CostExpression::from(ContinuousExpression::Cost);
         assert_eq!(
             expression,
             CostExpression::Continuous(ContinuousExpression::Cost)
         );
     }
 
     #[test]
+    fn cost_expression_from_continuous() {
+        let expression = CostExpression::from(1.0);
+        assert_eq!(
+            expression,
+            CostExpression::Continuous(ContinuousExpression::Constant(1.0))
+        );
+    }
+
+    #[test]
+    fn cost_expression_from_continuous_variable() {
+        let mut metadata = StateMetadata::default();
+        let var = metadata.add_continuous_variable("var");
+        assert!(var.is_ok());
+        let var = var.unwrap();
+        let expression = CostExpression::from(var);
+        assert_eq!(
+            expression,
+            CostExpression::Continuous(ContinuousExpression::Variable(0))
+        );
+    }
+
+    #[test]
+    fn cost_expression_from_continuous_resource_variable() {
+        let mut metadata = StateMetadata::default();
+        let var = metadata.add_continuous_resource_variable("var", false);
+        assert!(var.is_ok());
+        let var = var.unwrap();
+        let expression = CostExpression::from(var);
+        assert_eq!(
+            expression,
+            CostExpression::Continuous(ContinuousExpression::ResourceVariable(0))
+        );
+    }
+
+    #[test]
     fn cost_expression_eval() {
         let state = generate_state();
         let registry = generate_registry();
 
         let expression = CostExpression::Integer(IntegerExpression::BinaryOperation(
             BinaryOperator::Add,
             Box::new(IntegerExpression::Constant(1)),
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl/src/variable_type.rs` & `didppy-0.4.0/local_dependencies/dypdl/src/variable_type.rs`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 /// Numeric value.
 pub trait Numeric:
     num_traits::Num
     + ToNumeric
     + FromNumeric
     + num_traits::FromPrimitive
     + num_traits::Signed
+    + num_traits::Bounded
     + Copy
     + Sum
     + Product
     + PartialOrd
     + str::FromStr
     + fmt::Debug
     + default::Default
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/README.md` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -9,32 +9,31 @@
 
 [API Documentation](https://docs.rs/dypdl-heuristic-search)
 
 ## Example
 
 ```rust
 use dypdl::prelude::*;
-use dypdl_heuristic_search::{FEvaluatorType, create_dual_bound_cabs};
-use dypdl_heuristic_search::search_algorithm::util::Parameters;
+use dypdl_heuristic_search::{CabsParameters, create_dual_bound_cabs, FEvaluatorType};
 use std::rc::Rc;
 
 let mut model = Model::default();
 let variable = model.add_integer_variable("variable", 0).unwrap();
 model.add_base_case(
     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 ).unwrap();
 let mut increment = Transition::new("increment");
 increment.set_cost(IntegerExpression::Cost + 1);
 increment.add_effect(variable, variable + 1).unwrap();
 model.add_forward_transition(increment.clone()).unwrap();
 model.add_dual_bound(IntegerExpression::from(0)).unwrap();
 
 let model = Rc::new(model);
-let parameters = Parameters::default();
+let parameters = CabsParameters::default();
 let f_evaluator_type = FEvaluatorType::Plus;
 
-let mut solver = create_dual_bound_cabs(model, parameters, f_evaluator_type, 1, false);
+let mut solver = create_dual_bound_cabs(model, parameters, f_evaluator_type);
 let solution = solver.search().unwrap();
 assert_eq!(solution.cost, Some(1));
 assert_eq!(solution.transitions, vec![increment]);
 assert!(!solution.is_infeasible);
 ```
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/caasdy.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_dbdfs.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,122 @@
 use super::f_evaluator_type::FEvaluatorType;
-use super::search_algorithm::data_structure::state_registry::StateInRegistry;
-use super::search_algorithm::data_structure::{FNode, SuccessorGenerator};
-use super::search_algorithm::util::{ForwardSearchParameters, Parameters};
-use super::search_algorithm::{BestFirstSearch, Search};
-use dypdl::variable_type;
+use super::search_algorithm::{
+    CostNode, Dbdfs, DbdfsParameters, FNode, Search, SearchInput, SuccessorGenerator,
+};
+use dypdl::{variable_type, Transition};
 use std::fmt;
 use std::rc::Rc;
 use std::str;
 
-/// Creates a cost-algebraic A* solver for DyPDL (CAASDy).
+/// Creates a Discrepancy-Bounded Depth-First Search (DBDFS) solver using the dual bound as a heuristic function.
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 /// `f_evaluator_type` must be specified appropriately according to the cost expressions.
 ///
-/// It uses the dual bound defined in the DyPDL model as a heuristic function.
-///
 /// # References
 ///
-/// Ryo Kuroiwa and J. Christopher Beck. "Domain-Independent Dynamic Programming: Generic State Space Search for Combinatorial Optimization,"
+/// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
-/// Stephen Edelkamp, Shahid Jabbar, Alberto Lluch Lafuente. "Cost-Algebraic Heuristic Search,"
-/// Proceedings of the 20th National Conference on Artificial Intelligence (AAAI), pp. 1362-1367, 2005.
-///
-/// Peter E. Hart, Nills J. Nilsson, Bertram Raphael. "A Formal Basis for the Heuristic Determination of Minimum Cost Paths",
-/// IEEE Transactions of Systems Science and Cybernetics, vol. SSC-4(2), pp. 100-107, 1968.
+/// J. Christopher Beck. "Discrepancy-Bounded Depth First Search,"
+/// Second International Workshop on Integration of AI and OR Technologies in Constraint Programming for Combinatorial Optimization Problems (CPAIOR), 2000.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::{FEvaluatorType, create_caasdy};
-/// use dypdl_heuristic_search::search_algorithm::util::Parameters;
+/// use dypdl_heuristic_search::{create_dual_bound_dbdfs, DbdfsParameters, FEvaluatorType};
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
 /// model.add_dual_bound(IntegerExpression::from(0)).unwrap();
 ///
 /// let model = Rc::new(model);
-/// let parameters = Parameters::default();
+/// let parameters = DbdfsParameters::default();
 /// let f_evaluator_type = FEvaluatorType::Plus;
 ///
-/// let mut solver = create_caasdy(model, parameters, f_evaluator_type, None);
+/// let mut solver = create_dual_bound_dbdfs(model, parameters, f_evaluator_type);
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub fn create_caasdy<T>(
+pub fn create_dual_bound_dbdfs<T>(
     model: Rc<dypdl::Model>,
-    parameters: Parameters<T>,
+    parameters: DbdfsParameters<T>,
     f_evaluator_type: FEvaluatorType,
-    initial_registry_capacity: Option<usize>,
 ) -> Box<dyn Search<T>>
 where
     T: variable_type::Numeric + fmt::Display + Ord + 'static,
     <T as str::FromStr>::Err: fmt::Debug,
 {
-    let generator = SuccessorGenerator::from_model(model.clone(), false);
-    let parameters = ForwardSearchParameters {
-        generator,
-        parameters,
-        initial_registry_capacity,
-    };
-    let h_evaluator = |state: &StateInRegistry, model: &dypdl::Model| {
-        Some(model.eval_dual_bound(state).unwrap_or_else(T::zero))
+    let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+    let base_cost_evaluator = move |cost, base_cost| f_evaluator_type.eval(cost, base_cost);
+    let cost = match f_evaluator_type {
+        FEvaluatorType::Plus => T::zero(),
+        FEvaluatorType::Product => T::one(),
+        FEvaluatorType::Max => T::min_value(),
+        FEvaluatorType::Min => T::max_value(),
+        FEvaluatorType::Overwrite => T::zero(),
     };
-    let (f_pruning, f_evaluator_type) = if model.has_dual_bounds() {
-        (true, f_evaluator_type)
+
+    if model.has_dual_bounds() {
+        let state = model.target.clone();
+        let h_evaluator = move |state: &_| model.eval_dual_bound(state);
+        let f_evaluator = move |g, h, _: &_| f_evaluator_type.eval(g, h);
+        let node = FNode::generate_root_node(
+            state,
+            cost,
+            &generator.model,
+            &h_evaluator,
+            &f_evaluator,
+            parameters.parameters.primal_bound,
+        );
+        let input = SearchInput {
+            node,
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator =
+            move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+                node.insert_successor_node(
+                    transition,
+                    registry,
+                    &h_evaluator,
+                    &f_evaluator,
+                    primal_bound,
+                )
+            };
+        Box::new(Dbdfs::<_, FNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+        ))
     } else {
-        (false, FEvaluatorType::Plus)
-    };
-    let f_evaluator =
-        move |g, h, _: &StateInRegistry, _: &dypdl::Model| f_evaluator_type.eval(g, h);
-    Box::new(BestFirstSearch::<_, FNode<_>, _, _>::new(
-        model,
-        h_evaluator,
-        f_evaluator,
-        f_pruning,
-        true,
-        true,
-        parameters,
-    ))
+        let node = CostNode::generate_root_node(model.target.clone(), cost, &model);
+        let input = SearchInput {
+            node: Some(node),
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator = |node: &CostNode<_>, transition, registry: &mut _, _| {
+            node.insert_successor_node(transition, registry)
+        };
+        Box::new(Dbdfs::<_, CostNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+        ))
+    }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_acps.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_dfbb.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 use super::f_evaluator_type::FEvaluatorType;
-use super::search_algorithm::data_structure::state_registry::StateInRegistry;
-use super::search_algorithm::data_structure::{FNode, SuccessorGenerator};
-use super::search_algorithm::util::{
-    ForwardSearchParameters, Parameters, ProgressiveSearchParameters,
+use super::search_algorithm::{
+    CostNode, Dfbb, FNode, Parameters, Search, SearchInput, SuccessorGenerator,
 };
-use super::search_algorithm::Acps;
-use super::search_algorithm::Search;
-use dypdl::variable_type;
+use dypdl::{variable_type, Transition};
 use std::fmt;
 use std::rc::Rc;
 use std::str;
 
-/// Creates an Anytime Column Progressive Search (ACPS) solver using the dual bound as a heuristic function.
+/// Creates a DFBB solver using the dual bound as a heuristic function.
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 /// `f_evaluator_type` must be specified appropriately according to the cost expressions.
 ///
 /// # References
 ///
-/// Ryo Kuroiwa and J. Christopher Beck."Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,""
+/// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
-/// Sataya Gautam Vadlamudi, Piyush Gaurav, Sandip Aine, and Partha Pratim Chakrabarti. "Anytime Column Search,""
-/// Proceedings of AI 2012: Advances in Artificial Intelligence, pp. 254-255, 2012.
-///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::{FEvaluatorType, create_dual_bound_acps};
-/// use dypdl_heuristic_search::search_algorithm::util::{Parameters, ProgressiveSearchParameters};
+/// use dypdl_heuristic_search::{create_dual_bound_dfbb, FEvaluatorType, Parameters};
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
@@ -43,55 +35,86 @@
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
 /// model.add_dual_bound(IntegerExpression::from(0)).unwrap();
 ///
 /// let model = Rc::new(model);
 /// let parameters = Parameters::default();
-/// let progressive_parameters = ProgressiveSearchParameters::default();
 /// let f_evaluator_type = FEvaluatorType::Plus;
 ///
-/// let mut solver = create_dual_bound_acps(
-///     model, parameters, progressive_parameters, f_evaluator_type, None
-/// );
+/// let mut solver = create_dual_bound_dfbb(model, parameters, f_evaluator_type);
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub fn create_dual_bound_acps<T>(
+pub fn create_dual_bound_dfbb<T>(
     model: Rc<dypdl::Model>,
     parameters: Parameters<T>,
-    progressive_parameters: ProgressiveSearchParameters,
     f_evaluator_type: FEvaluatorType,
-    initial_registry_capacity: Option<usize>,
 ) -> Box<dyn Search<T>>
 where
     T: variable_type::Numeric + fmt::Display + Ord + 'static,
     <T as str::FromStr>::Err: fmt::Debug,
 {
-    let generator = SuccessorGenerator::from_model(model.clone(), false);
-    let parameters = ForwardSearchParameters {
-        generator,
-        parameters,
-        initial_registry_capacity,
-    };
-    let h_evaluator = |state: &StateInRegistry, model: &dypdl::Model| {
-        Some(model.eval_dual_bound(state).unwrap_or_else(T::zero))
+    let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+    let base_cost_evaluator = move |cost, base_cost| f_evaluator_type.eval(cost, base_cost);
+    let cost = match f_evaluator_type {
+        FEvaluatorType::Plus => T::zero(),
+        FEvaluatorType::Product => T::one(),
+        FEvaluatorType::Max => T::min_value(),
+        FEvaluatorType::Min => T::max_value(),
+        FEvaluatorType::Overwrite => T::zero(),
     };
-    let (f_pruning, f_evaluator_type) = if model.has_dual_bounds() {
-        (true, f_evaluator_type)
+
+    if model.has_dual_bounds() {
+        let state = model.target.clone();
+        let h_evaluator = move |state: &_| model.eval_dual_bound(state);
+        let f_evaluator = move |g, h, _: &_| f_evaluator_type.eval(g, h);
+        let node = FNode::generate_root_node(
+            state,
+            cost,
+            &generator.model,
+            &h_evaluator,
+            &f_evaluator,
+            parameters.primal_bound,
+        );
+        let input = SearchInput {
+            node,
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator =
+            move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+                node.insert_successor_node(
+                    transition,
+                    registry,
+                    &h_evaluator,
+                    &f_evaluator,
+                    primal_bound,
+                )
+            };
+
+        Box::new(Dfbb::<_, FNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+        ))
     } else {
-        (false, FEvaluatorType::Plus)
-    };
-    let f_evaluator =
-        move |g, h, _: &StateInRegistry, _: &dypdl::Model| f_evaluator_type.eval(g, h);
-    Box::new(Acps::<_, FNode<_>, _, _>::new(
-        model,
-        h_evaluator,
-        f_evaluator,
-        f_pruning,
-        true,
-        progressive_parameters,
-        parameters,
-    ))
+        let node = CostNode::generate_root_node(model.target.clone(), cost, &model);
+        let input = SearchInput {
+            node: Some(node),
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator = |node: &CostNode<_>, transition, registry: &mut _, _| {
+            node.insert_successor_node(transition, registry)
+        };
+        Box::new(Dfbb::<_, CostNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+        ))
+    }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_apps.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_apps.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,39 @@
 use super::f_evaluator_type::FEvaluatorType;
-use super::search_algorithm::data_structure::state_registry::StateInRegistry;
-use super::search_algorithm::data_structure::FNode;
-use super::search_algorithm::util::{
-    ForwardSearchParameters, Parameters, ProgressiveSearchParameters,
+use super::search_algorithm::{
+    Apps, CostNode, FNode, Parameters, ProgressiveSearchParameters, Search, SearchInput,
+    SuccessorGenerator,
 };
-use super::search_algorithm::Search;
-use super::search_algorithm::{Apps, SuccessorGenerator};
-use dypdl::variable_type;
+use dypdl::{variable_type, Transition};
 use std::fmt;
 use std::rc::Rc;
 use std::str;
 
 /// Creates an Anytime Progressive Pack Search (APPS) solver using the dual bound as a heuristic function.
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 /// `f_evaluator_type` must be specified appropriately according to the cost expressions.
 ///
 /// # References
 ///
-/// Ryo Kuroiwa and J. Christopher Beck."Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,""
+/// Ryo Kuroiwa and J. Christopher Beck."Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
 /// Sataya Gautam Vadlamudi, Sandip Aine, Partha Pratim Chakrabarti. "Anytime Pack Search,"
 /// Natural Computing, vol. 15(3), pp. 395-414, 2016
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::{FEvaluatorType, create_dual_bound_apps};
-/// use dypdl_heuristic_search::search_algorithm::util::{Parameters, ProgressiveSearchParameters};
+/// use dypdl_heuristic_search::{
+///     create_dual_bound_apps, FEvaluatorType, Parameters, ProgressiveSearchParameters
+/// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
@@ -47,51 +45,87 @@
 ///
 /// let model = Rc::new(model);
 /// let parameters = Parameters::default();
 /// let progressive_parameters = ProgressiveSearchParameters::default();
 /// let f_evaluator_type = FEvaluatorType::Plus;
 ///
 /// let mut solver = create_dual_bound_apps(
-///     model, parameters, progressive_parameters, f_evaluator_type, None
+///     model, parameters, f_evaluator_type, progressive_parameters
 /// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
 pub fn create_dual_bound_apps<T>(
     model: Rc<dypdl::Model>,
     parameters: Parameters<T>,
-    progressive_parameters: ProgressiveSearchParameters,
     f_evaluator_type: FEvaluatorType,
-    initial_registry_capacity: Option<usize>,
+    progressive_parameters: ProgressiveSearchParameters,
 ) -> Box<dyn Search<T>>
 where
     T: variable_type::Numeric + fmt::Display + Ord + 'static,
     <T as str::FromStr>::Err: fmt::Debug,
 {
-    let generator = SuccessorGenerator::from_model(model.clone(), false);
-    let parameters = ForwardSearchParameters {
-        generator,
-        parameters,
-        initial_registry_capacity,
-    };
-    let h_evaluator = |state: &StateInRegistry, model: &dypdl::Model| {
-        Some(model.eval_dual_bound(state).unwrap_or_else(T::zero))
+    let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+    let base_cost_evaluator = move |cost, base_cost| f_evaluator_type.eval(cost, base_cost);
+    let cost = match f_evaluator_type {
+        FEvaluatorType::Plus => T::zero(),
+        FEvaluatorType::Product => T::one(),
+        FEvaluatorType::Max => T::min_value(),
+        FEvaluatorType::Min => T::max_value(),
+        FEvaluatorType::Overwrite => T::zero(),
     };
-    let (f_pruning, f_evaluator_type) = if model.has_dual_bounds() {
-        (true, f_evaluator_type)
+
+    if model.has_dual_bounds() {
+        let state = model.target.clone();
+        let h_evaluator = move |state: &_| model.eval_dual_bound(state);
+        let f_evaluator = move |g, h, _: &_| f_evaluator_type.eval(g, h);
+        let node = FNode::generate_root_node(
+            state,
+            cost,
+            &generator.model,
+            &h_evaluator,
+            &f_evaluator,
+            parameters.primal_bound,
+        );
+        let input = SearchInput {
+            node,
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator =
+            move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+                node.insert_successor_node(
+                    transition,
+                    registry,
+                    &h_evaluator,
+                    &f_evaluator,
+                    primal_bound,
+                )
+            };
+        Box::new(Apps::<_, FNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+            progressive_parameters,
+        ))
     } else {
-        (false, FEvaluatorType::Plus)
-    };
-    let f_evaluator =
-        move |g, h, _: &StateInRegistry, _: &dypdl::Model| f_evaluator_type.eval(g, h);
-    Box::new(Apps::<_, FNode<_>, _, _>::new(
-        model,
-        h_evaluator,
-        f_evaluator,
-        f_pruning,
-        true,
-        progressive_parameters,
-        parameters,
-    ))
+        let node = CostNode::generate_root_node(model.target.clone(), cost, &model);
+        let input = SearchInput {
+            node: Some(node),
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator = |node: &CostNode<_>, transition, registry: &mut _, _| {
+            node.insert_successor_node(transition, registry)
+        };
+        Box::new(Apps::<_, CostNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+            progressive_parameters,
+        ))
+    }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_cabs.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_acps.rs`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,39 @@
 use super::f_evaluator_type::FEvaluatorType;
-use super::search_algorithm::data_structure::beam::Beam;
-use super::search_algorithm::data_structure::state_registry::StateInRegistry;
-use super::search_algorithm::data_structure::SuccessorGenerator;
-use super::search_algorithm::util::Parameters;
-use super::search_algorithm::Cabs;
-use super::search_algorithm::Search;
-use crate::search_algorithm::data_structure::BeamSearchNode;
-use crate::search_algorithm::BeamSearchParameters;
-use dypdl::{variable_type, ReduceFunction};
+use super::search_algorithm::{
+    Acps, CostNode, FNode, Parameters, ProgressiveSearchParameters, Search, SearchInput,
+    SuccessorGenerator,
+};
+use dypdl::{variable_type, Transition};
 use std::fmt;
 use std::rc::Rc;
 use std::str;
 
-/// Creates a Complete Anytime Beam Search (CABS) solver using the dual bound as a heuristic function.
-///
-/// It iterates beam search with exponentially increasing beam width.
-/// `beam_size` specifies the initial beam width.
+/// Creates an Anytime Column Progressive Search (ACPS) solver using the dual bound as a heuristic function.
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 /// `f_evaluator_type` must be specified appropriately according to the cost expressions.
 ///
-/// Beam search searches layer by layer, where the i th layer contains states that can be reached with i transitions.
-/// By default, this solver only keeps states in the current layer to check for duplicates.
-/// If `keep_all_layers` is `true`, this solver keeps states in all layers to check for duplicates.
-///
 /// # References
 ///
-/// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
+/// Ryo Kuroiwa and J. Christopher Beck."Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
-/// Weixiong Zhang. "Complete Anytime Beam Search,"
-/// Proceedings of the 15th National Conference on Artificial Intelligence/Innovative Applications of Artificial Intelligence (AAAI/IAAI), pp. 425-430, 1998.
+/// Sataya Gautam Vadlamudi, Piyush Gaurav, Sandip Aine, and Partha Pratim Chakrabarti. "Anytime Column Search,""
+/// Proceedings of AI 2012: Advances in Artificial Intelligence, pp. 254-255, 2012.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::{FEvaluatorType, create_dual_bound_cabs};
-/// use dypdl_heuristic_search::search_algorithm::util::Parameters;
+/// use dypdl_heuristic_search::{
+///     create_dual_bound_acps, FEvaluatorType, Parameters, ProgressiveSearchParameters
+/// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
@@ -51,54 +41,91 @@
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
 /// model.add_dual_bound(IntegerExpression::from(0)).unwrap();
 ///
 /// let model = Rc::new(model);
 /// let parameters = Parameters::default();
+/// let progressive_parameters = ProgressiveSearchParameters::default();
 /// let f_evaluator_type = FEvaluatorType::Plus;
 ///
-/// let mut solver = create_dual_bound_cabs(model, parameters, f_evaluator_type, 1, false);
+/// let mut solver = create_dual_bound_acps(
+///     model, parameters, f_evaluator_type, progressive_parameters
+/// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub fn create_dual_bound_cabs<T>(
+pub fn create_dual_bound_acps<T>(
     model: Rc<dypdl::Model>,
     parameters: Parameters<T>,
     f_evaluator_type: FEvaluatorType,
-    beam_size: usize,
-    keep_all_layers: bool,
+    progressive_parameters: ProgressiveSearchParameters,
 ) -> Box<dyn Search<T>>
 where
     T: variable_type::Numeric + fmt::Display + Ord + 'static,
     <T as str::FromStr>::Err: fmt::Debug,
 {
-    let beam_constructor = Beam::<T, T, BeamSearchNode<T, T>>::new;
-    let generator = SuccessorGenerator::from_model_without_custom_cost(model.clone(), false);
-    let h_evaluator = |state: &StateInRegistry, model: &dypdl::Model| {
-        Some(model.eval_dual_bound(state).unwrap_or_else(T::zero))
+    let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+    let base_cost_evaluator = move |cost, base_cost| f_evaluator_type.eval(cost, base_cost);
+    let cost = match f_evaluator_type {
+        FEvaluatorType::Plus => T::zero(),
+        FEvaluatorType::Product => T::one(),
+        FEvaluatorType::Max => T::min_value(),
+        FEvaluatorType::Min => T::max_value(),
+        FEvaluatorType::Overwrite => T::zero(),
     };
-    let (f_pruning, f_evaluator_type) = if model.has_dual_bounds() {
-        (true, f_evaluator_type)
+
+    if model.has_dual_bounds() {
+        let state = model.target.clone();
+        let h_evaluator = move |state: &_| model.eval_dual_bound(state);
+        let f_evaluator = move |g, h, _: &_| f_evaluator_type.eval(g, h);
+        let node = FNode::generate_root_node(
+            state,
+            cost,
+            &generator.model,
+            &h_evaluator,
+            &f_evaluator,
+            parameters.primal_bound,
+        );
+        let input = SearchInput {
+            node,
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator =
+            move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+                node.insert_successor_node(
+                    transition,
+                    registry,
+                    &h_evaluator,
+                    &f_evaluator,
+                    primal_bound,
+                )
+            };
+        Box::new(Acps::<_, FNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+            progressive_parameters,
+        ))
     } else {
-        (false, FEvaluatorType::Plus)
-    };
-    let f_evaluator =
-        move |g, h, _: &StateInRegistry, _: &dypdl::Model| f_evaluator_type.eval(g, h);
-    let parameters = BeamSearchParameters {
-        beam_size,
-        maximize: model.reduce_function == ReduceFunction::Max,
-        f_pruning,
-        f_bound: None,
-        keep_all_layers,
-        parameters,
-    };
-    Box::new(Cabs::new(
-        generator,
-        h_evaluator,
-        f_evaluator,
-        beam_constructor,
-        parameters,
-    ))
+        let node = CostNode::generate_root_node(model.target.clone(), cost, &model);
+        let input = SearchInput {
+            node: Some(node),
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator = |node: &CostNode<_>, transition, registry: &mut _, _| {
+            node.insert_successor_node(transition, registry)
+        };
+        Box::new(Acps::<_, CostNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+            progressive_parameters,
+        ))
+    }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_dfbb.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/dual_bound_cbfs.rs`

 * *Files 21% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 use super::f_evaluator_type::FEvaluatorType;
-use super::search_algorithm::data_structure::state_registry::StateInRegistry;
-use super::search_algorithm::data_structure::{FNode, SuccessorGenerator};
-use super::search_algorithm::util::{ForwardSearchParameters, Parameters};
-use super::search_algorithm::Search;
-use super::search_algorithm::{Dfbb, DfbbBfs};
-use dypdl::variable_type;
+use super::search_algorithm::{
+    Cbfs, CostNode, FNode, Parameters, Search, SearchInput, SuccessorGenerator,
+};
+use dypdl::{variable_type, Transition};
 use std::fmt;
 use std::rc::Rc;
 use std::str;
 
-/// Creates a DFBB solver using the dual bound as a heuristic function.
+/// Creates a Cyclic Best-First Search (CBFS) solver using the dual bound as a heuristic function.
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 /// `f_evaluator_type` must be specified appropriately according to the cost expressions.
 ///
-/// `bfs_tie_breaking` specifies if the tie-breaking strategy is best-first.
-///
-/// It uses `h_evaluator` and `f_evaluator` for pruning.
-/// If `h_evaluator` returns `None`, the state is pruned.
-/// If `f_pruning` and `f_evaluator` returns a value that exceeds the primal bound, the state is pruned.
-///
 /// # References
 ///
 /// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
+/// Gio K. Kao, Edward C. Sewell, and Sheldom H. Jacobson. "A Branch, Bound and Remember Algorithm for the 1|r_i|Σt_i scheduling problem,"
+/// Journal of Scheduling, vol. 12(2), pp. 163-175, 2009.
+///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::{FEvaluatorType, create_dual_bound_dfbb};
-/// use dypdl_heuristic_search::search_algorithm::util::Parameters;
+/// use dypdl_heuristic_search::{create_dual_bound_cbfs, FEvaluatorType, Parameters};
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
@@ -46,59 +40,84 @@
 /// model.add_forward_transition(increment.clone()).unwrap();
 /// model.add_dual_bound(IntegerExpression::from(0)).unwrap();
 ///
 /// let model = Rc::new(model);
 /// let parameters = Parameters::default();
 /// let f_evaluator_type = FEvaluatorType::Plus;
 ///
-/// let mut solver = create_dual_bound_dfbb(model, parameters, true, f_evaluator_type, None);
+/// let mut solver = create_dual_bound_cbfs(model, parameters, f_evaluator_type);
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub fn create_dual_bound_dfbb<T>(
+pub fn create_dual_bound_cbfs<T>(
     model: Rc<dypdl::Model>,
     parameters: Parameters<T>,
-    bfs_tie_breaking: bool,
     f_evaluator_type: FEvaluatorType,
-    initial_registry_capacity: Option<usize>,
 ) -> Box<dyn Search<T>>
 where
     T: variable_type::Numeric + fmt::Display + Ord + 'static,
     <T as str::FromStr>::Err: fmt::Debug,
 {
-    let generator = SuccessorGenerator::from_model(model.clone(), false);
-    let parameters = ForwardSearchParameters {
-        generator,
-        parameters,
-        initial_registry_capacity,
-    };
-    let h_evaluator = |state: &StateInRegistry, model: &dypdl::Model| {
-        Some(model.eval_dual_bound(state).unwrap_or_else(T::zero))
+    let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+    let base_cost_evaluator = move |cost, base_cost| f_evaluator_type.eval(cost, base_cost);
+    let cost = match f_evaluator_type {
+        FEvaluatorType::Plus => T::zero(),
+        FEvaluatorType::Product => T::one(),
+        FEvaluatorType::Max => T::min_value(),
+        FEvaluatorType::Min => T::max_value(),
+        FEvaluatorType::Overwrite => T::zero(),
     };
-    let (f_pruning, f_evaluator_type) = if model.has_dual_bounds() {
-        (true, f_evaluator_type)
-    } else {
-        (false, FEvaluatorType::Plus)
-    };
-    let f_evaluator =
-        move |g, h, _: &StateInRegistry, _: &dypdl::Model| f_evaluator_type.eval(g, h);
 
-    if bfs_tie_breaking {
-        Box::new(DfbbBfs::<_, FNode<_>, _, _>::new(
-            model,
-            h_evaluator,
-            f_evaluator,
-            f_pruning,
+    if model.has_dual_bounds() {
+        let state = model.target.clone();
+        let h_evaluator = move |state: &_| model.eval_dual_bound(state);
+        let f_evaluator = move |g, h, _: &_| f_evaluator_type.eval(g, h);
+        let node = FNode::generate_root_node(
+            state,
+            cost,
+            &generator.model,
+            &h_evaluator,
+            &f_evaluator,
+            parameters.primal_bound,
+        );
+        let input = SearchInput {
+            node,
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator =
+            move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+                node.insert_successor_node(
+                    transition,
+                    registry,
+                    &h_evaluator,
+                    &f_evaluator,
+                    primal_bound,
+                )
+            };
+
+        Box::new(Cbfs::<_, FNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
             parameters,
         ))
     } else {
-        Box::new(Dfbb::new(
-            model,
-            h_evaluator,
-            f_evaluator,
-            f_pruning,
+        let node = CostNode::generate_root_node(model.target.clone(), cost, &model);
+        let input = SearchInput {
+            node: Some(node),
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator = move |node: &CostNode<_>, transition, registry: &mut _, _| {
+            node.insert_successor_node(transition, registry)
+        };
+        Box::new(Cbfs::<_, CostNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
             parameters,
         ))
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/dual_bound_weighted_astar.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/caasdy.rs`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,41 @@
 use super::f_evaluator_type::FEvaluatorType;
-use super::search_algorithm::data_structure::state_registry::StateInRegistry;
-use super::search_algorithm::data_structure::{FNode, SuccessorGenerator};
-use super::search_algorithm::util::{ForwardSearchParameters, Parameters};
-use super::search_algorithm::{BestFirstSearch, Search};
-use dypdl::variable_type;
-use dypdl::Continuous;
+use super::search_algorithm::{
+    BestFirstSearch, CostNode, FNode, Parameters, Search, SearchInput, SuccessorGenerator,
+};
+use dypdl::{variable_type, Transition};
 use std::fmt;
 use std::rc::Rc;
 use std::str;
 
-/// Creates a weighted A* solver using the dual bound as a heuristic function.
+/// Creates a cost-algebraic A* solver for DyPDL (CAASDy).
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 /// `f_evaluator_type` must be specified appropriately according to the cost expressions.
 ///
 /// It uses the dual bound defined in the DyPDL model as a heuristic function.
 ///
+/// # References
+///
+/// Ryo Kuroiwa and J. Christopher Beck. "Domain-Independent Dynamic Programming: Generic State Space Search for Combinatorial Optimization,"
+/// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
+///
+/// Stephen Edelkamp, Shahid Jabbar, Alberto Lluch Lafuente. "Cost-Algebraic Heuristic Search,"
+/// Proceedings of the 20th National Conference on Artificial Intelligence (AAAI), pp. 1362-1367, 2005.
+///
+/// Peter E. Hart, Nills J. Nilsson, Bertram Raphael. "A Formal Basis for the Heuristic Determination of Minimum Cost Paths",
+/// IEEE Transactions of Systems Science and Cybernetics, vol. SSC-4(2), pp. 100-107, 1968.
+///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::{FEvaluatorType, create_dual_bound_weighted_astar};
-/// use dypdl_heuristic_search::search_algorithm::util::Parameters;
+/// use dypdl_heuristic_search::{create_caasdy, FEvaluatorType, Parameters};
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
@@ -37,53 +45,84 @@
 /// model.add_forward_transition(increment.clone()).unwrap();
 /// model.add_dual_bound(IntegerExpression::from(0)).unwrap();
 ///
 /// let model = Rc::new(model);
 /// let parameters = Parameters::default();
 /// let f_evaluator_type = FEvaluatorType::Plus;
 ///
-/// let mut solver = create_dual_bound_weighted_astar(
-///     model, parameters, 1.1, f_evaluator_type, None
-/// );
+/// let mut solver = create_caasdy(model, parameters, f_evaluator_type);
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub fn create_dual_bound_weighted_astar<T>(
+pub fn create_caasdy<T>(
     model: Rc<dypdl::Model>,
     parameters: Parameters<T>,
-    weight: Continuous,
     f_evaluator_type: FEvaluatorType,
-    initial_registry_capacity: Option<usize>,
 ) -> Box<dyn Search<T>>
 where
     T: variable_type::Numeric + fmt::Display + Ord + 'static,
     <T as str::FromStr>::Err: fmt::Debug,
 {
-    let generator = SuccessorGenerator::from_model(model.clone(), false);
-    let parameters = ForwardSearchParameters {
-        generator,
-        parameters,
-        initial_registry_capacity,
-    };
-    let h_evaluator = |state: &StateInRegistry, model: &dypdl::Model| {
-        Some(model.eval_dual_bound(state).unwrap_or_else(T::zero))
+    let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+    let base_cost_evaluator = move |cost, base_cost| f_evaluator_type.eval(cost, base_cost);
+    let cost = match f_evaluator_type {
+        FEvaluatorType::Plus => T::zero(),
+        FEvaluatorType::Product => T::one(),
+        FEvaluatorType::Max => T::min_value(),
+        FEvaluatorType::Min => T::max_value(),
+        FEvaluatorType::Overwrite => T::zero(),
     };
-    let (f_pruning, f_evaluator_type) = if model.has_dual_bounds() {
-        (true, f_evaluator_type)
+
+    if model.has_dual_bounds() {
+        let state = model.target.clone();
+        let h_evaluator = move |state: &_| model.eval_dual_bound(state);
+        let f_evaluator = move |g, h, _: &_| f_evaluator_type.eval(g, h);
+        let node = FNode::generate_root_node(
+            state,
+            cost,
+            &generator.model,
+            &h_evaluator,
+            &f_evaluator,
+            parameters.primal_bound,
+        );
+        let input = SearchInput {
+            node,
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator =
+            move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+                node.insert_successor_node(
+                    transition,
+                    registry,
+                    &h_evaluator,
+                    &f_evaluator,
+                    primal_bound,
+                )
+            };
+
+        Box::new(BestFirstSearch::<_, FNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+        ))
     } else {
-        (false, FEvaluatorType::Plus)
-    };
-    let f_evaluator = move |g, h: T, _: &StateInRegistry, _: &dypdl::Model| {
-        f_evaluator_type.eval(g, T::from_continuous(weight * h.to_continuous()))
-    };
-    Box::new(BestFirstSearch::<_, FNode<_>, _, _>::new(
-        model,
-        h_evaluator,
-        f_evaluator,
-        f_pruning,
-        true,
-        weight <= 1.0,
-        parameters,
-    ))
+        let node = CostNode::generate_root_node(model.target.clone(), cost, &model);
+        let input = SearchInput {
+            node: Some(node),
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator = |node: &CostNode<_>, transition, registry: &mut _, _| {
+            node.insert_successor_node(transition, registry)
+        };
+        Box::new(BestFirstSearch::<_, CostNode<_>, _, _>::new(
+            input,
+            transition_evaluator,
+            base_cost_evaluator,
+            parameters,
+        ))
+    }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/expression_beam_search.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/expression_beam_search.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,12 @@
 use super::f_evaluator_type::FEvaluatorType;
-use super::search_algorithm::data_structure::beam::Beam;
-use super::search_algorithm::data_structure::state_registry::StateInRegistry;
-use super::search_algorithm::data_structure::{
-    BeamSearchNode, BeamSearchProblemInstance, SuccessorGenerator, TransitionWithCustomCost,
+use super::search_algorithm::{
+    beam_search, BeamSearchParameters, CustomFNode, Search, SearchInput, Solution,
+    SuccessorGenerator,
 };
-use super::search_algorithm::util::Parameters;
-use super::search_algorithm::Search;
-use super::search_algorithm::Solution;
-use super::search_algorithm::{beam_search, BeamSearchParameters};
 use dypdl::variable_type;
 use dypdl::CostType;
 use std::error::Error;
 use std::fmt;
 use std::rc::Rc;
 
 /// Beam search solver using user-defined cost functions.
@@ -26,189 +21,189 @@
 /// The user-defined cost and the heuristic value are combined by `f_evaluator_type` to guide the search.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
 /// use dypdl::variable_type::OrderedContinuous;
-/// use dypdl_heuristic_search::{FEvaluatorType, ExpressionBeamSearch, CustomExpressionParameters};
-/// use dypdl_heuristic_search::search_algorithm::{BeamSearchParameters, Search};
+/// use dypdl_heuristic_search::{
+///     BeamSearchParameters, FEvaluatorType, ExpressionBeamSearch, CustomExpressionParameters,
+///     Search,
+/// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
 /// model.add_dual_bound(IntegerExpression::from(0)).unwrap();
 ///
 /// let model = Rc::new(model);
-/// let parameters = BeamSearchParameters::<Integer, OrderedContinuous> {
-///     beam_size: 1,
-///     maximize: true,
-///     ..Default::default()
-/// };
+/// let parameters = BeamSearchParameters::default();
 /// let f_evaluator_type = FEvaluatorType::Plus;
 /// let custom_expression_parameters = CustomExpressionParameters {
 ///     custom_costs: vec![CostExpression::from(ContinuousExpression::Cost + 1.5)],
 ///     forced_custom_costs: Vec::default(),
 ///     h_expression: Some(CostExpression::from(ContinuousExpression::from(variable))),
+///     f_evaluator_type: FEvaluatorType::Plus,
 ///     custom_cost_type: CostType::Continuous,
+///     maximize: true,
 /// };
 ///
-/// let mut solver = ExpressionBeamSearch::new(
-///     model, parameters, custom_expression_parameters, f_evaluator_type
+/// let mut solver = ExpressionBeamSearch::<_, OrderedContinuous>::new(
+///     model, parameters, f_evaluator_type, custom_expression_parameters,
 /// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
 pub struct ExpressionBeamSearch<T, U>
 where
     T: variable_type::Numeric + fmt::Display + 'static,
     U: variable_type::Numeric + fmt::Display + 'static,
 {
     model: Rc<dypdl::Model>,
-    parameters: BeamSearchParameters<T, U>,
+    parameters: BeamSearchParameters<T>,
     custom_expression_parameters: CustomExpressionParameters,
     f_evaluator_type: FEvaluatorType,
     terminated: bool,
     solution: Solution<T>,
+    phantom: std::marker::PhantomData<U>,
 }
 
 /// Parameters for custom cost expressions.
 pub struct CustomExpressionParameters {
     /// Custom cost expressions for transitions.
     pub custom_costs: Vec<dypdl::CostExpression>,
     /// Custom cost expressions for forced transitions.
     pub forced_custom_costs: Vec<dypdl::CostExpression>,
     /// Expression for cost estimate .
     pub h_expression: Option<dypdl::CostExpression>,
+    /// The evaluator type to combine the g- and h-values.
+    pub f_evaluator_type: FEvaluatorType,
     /// Type of the custom cost.
     pub custom_cost_type: CostType,
+    /// Maximize or not.
+    pub maximize: bool,
 }
 
 impl<T, U> ExpressionBeamSearch<T, U>
 where
     T: variable_type::Numeric + fmt::Display + 'static,
-    U: variable_type::Numeric + fmt::Display + 'static,
+    U: variable_type::Numeric + Ord + fmt::Display + 'static,
 {
     /// Create a new beam search solver using user-defined cost functions.
     pub fn new(
         model: Rc<dypdl::Model>,
-        parameters: BeamSearchParameters<T, U>,
-        custom_expression_parameters: CustomExpressionParameters,
+        parameters: BeamSearchParameters<T>,
         f_evaluator_type: FEvaluatorType,
+        custom_expression_parameters: CustomExpressionParameters,
     ) -> ExpressionBeamSearch<T, U> {
         let f_evaluator_type = if custom_expression_parameters.h_expression.is_some() {
             f_evaluator_type
         } else {
             FEvaluatorType::Plus
         };
 
         ExpressionBeamSearch {
             model,
             parameters,
             custom_expression_parameters,
             f_evaluator_type,
             terminated: false,
             solution: Solution::default(),
-        }
-    }
-
-    fn solve_inner<H>(
-        &self,
-        model: Rc<dypdl::Model>,
-        generator: SuccessorGenerator<TransitionWithCustomCost>,
-        h_evaluator: H,
-    ) -> Solution<T>
-    where
-        U: variable_type::Numeric + Ord + fmt::Display + 'static,
-        H: Fn(&StateInRegistry, &dypdl::Model) -> Option<U>,
-    {
-        let beam_constructor = |beam_size| Beam::<T, U, BeamSearchNode<T, U>>::new(beam_size);
-        let parameters = BeamSearchParameters {
-            beam_size: self.parameters.beam_size,
-            maximize: self.parameters.maximize,
-            keep_all_layers: self.parameters.keep_all_layers,
-            f_pruning: self.parameters.f_pruning,
-            f_bound: None,
-            parameters: Parameters {
-                primal_bound: None,
-                time_limit: self.parameters.parameters.time_limit,
-                get_all_solutions: self.parameters.parameters.get_all_solutions,
-                quiet: self.parameters.parameters.quiet,
-            },
-        };
-        let f_evaluator =
-            move |g, h, _: &StateInRegistry, _: &dypdl::Model| self.f_evaluator_type.eval(g, h);
-        let target = StateInRegistry::from(model.target.clone());
-        let problem = BeamSearchProblemInstance {
-            generator,
-            cost: T::zero(),
-            g: U::zero(),
-            target,
-            solution_suffix: &[],
-        };
-        let solution = beam_search(
-            &problem,
-            &beam_constructor,
-            &h_evaluator,
-            f_evaluator,
-            parameters,
-        );
-
-        Solution {
-            cost: solution.cost,
-            best_bound: solution.best_bound,
-            is_optimal: solution.is_optimal,
-            is_infeasible: solution.is_infeasible,
-            transitions: solution
-                .transitions
-                .into_iter()
-                .map(dypdl::Transition::from)
-                .collect(),
-            expanded: solution.expanded,
-            generated: solution.generated,
-            time: solution.time,
-            time_out: solution.time_out,
+            phantom: std::marker::PhantomData,
         }
     }
 }
 
 impl<T, U> Search<T> for ExpressionBeamSearch<T, U>
 where
-    T: variable_type::Numeric + fmt::Display + 'static,
+    T: variable_type::Numeric + Ord + fmt::Display + 'static,
     U: variable_type::Numeric + Ord + fmt::Display + 'static,
 {
     fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
         if self.terminated {
             return Ok((self.solution.clone(), true));
         }
 
         let generator = SuccessorGenerator::from_model_with_custom_costs(
             self.model.clone(),
             &self.custom_expression_parameters.custom_costs,
             &self.custom_expression_parameters.forced_custom_costs,
             false,
         );
 
-        let h_evaluator = |state: &StateInRegistry, model: &dypdl::Model| {
+        let h_evaluator = |state: &_| {
             Some(
                 self.custom_expression_parameters
                     .h_expression
                     .as_ref()
                     .map_or(U::zero(), |expression| {
-                        expression.eval(state, &model.table_registry)
+                        expression.eval(state, &self.model.table_registry)
                     }),
             )
         };
-        let solution = self.solve_inner(self.model.clone(), generator, h_evaluator);
+        let f_evaluator = |g, h, _: &_| {
+            self.custom_expression_parameters
+                .f_evaluator_type
+                .eval(g, h)
+        };
+        let node = CustomFNode::generate_root_node(
+            self.model.target.clone(),
+            T::zero(),
+            U::zero(),
+            &h_evaluator,
+            &f_evaluator,
+            self.custom_expression_parameters.maximize,
+        );
+        let input = SearchInput {
+            node,
+            generator,
+            solution_suffix: &[],
+        };
+        let transition_evaluator = |node: &CustomFNode<_, _>, transition, _| {
+            node.generate_successor_node(
+                transition,
+                &self.model,
+                &h_evaluator,
+                &f_evaluator,
+                self.custom_expression_parameters.maximize,
+            )
+        };
+        let base_cost_evaluator = |cost, base_cost| self.f_evaluator_type.eval(cost, base_cost);
+
+        let solution = beam_search::<_, CustomFNode<T, U>, _, _, _>(
+            &input,
+            transition_evaluator,
+            base_cost_evaluator,
+            self.parameters,
+        );
+
         self.terminated = true;
-        Ok((solution, true))
+
+        Ok((
+            Solution {
+                cost: solution.cost,
+                best_bound: solution.best_bound,
+                is_optimal: solution.is_optimal,
+                is_infeasible: solution.is_infeasible,
+                transitions: solution
+                    .transitions
+                    .into_iter()
+                    .map(dypdl::Transition::from)
+                    .collect(),
+                expanded: solution.expanded,
+                generated: solution.generated,
+                time: solution.time,
+                time_out: solution.time_out,
+            },
+            true,
+        ))
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/f_evaluator_type.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/f_evaluator_type.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use dypdl::variable_type;
 use std::cmp;
 
 /// How to combine the g-value and the h-value to compute the f-value.
-#[derive(Debug, PartialEq, Eq, Clone)]
+#[derive(Debug, PartialEq, Eq, Clone, Copy)]
 pub enum FEvaluatorType {
     /// f = g + h.
     Plus,
     /// f = max(g, h).
     Max,
     /// f = min(g, h).
     Min,
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/lib.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/lib.rs`

 * *Files 13% similar despite different names*

```diff
@@ -23,9 +23,11 @@
 pub use dual_bound_cbfs::create_dual_bound_cbfs;
 pub use dual_bound_dbdfs::create_dual_bound_dbdfs;
 pub use dual_bound_dfbb::create_dual_bound_dfbb;
 pub use dual_bound_weighted_astar::create_dual_bound_weighted_astar;
 pub use expression_beam_search::{CustomExpressionParameters, ExpressionBeamSearch};
 pub use f_evaluator_type::FEvaluatorType;
 pub use search_algorithm::data_structure::TransitionWithCustomCost;
-pub use search_algorithm::util::{Parameters, ProgressiveSearchParameters};
-pub use search_algorithm::{Dijkstra, ForwardRecursion, Search, Solution};
+pub use search_algorithm::{
+    BeamSearchParameters, BrfsParameters, CabsParameters, DbdfsParameters, ForwardRecursion,
+    Parameters, ProgressiveSearchParameters, Search, Solution,
+};
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/acps.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/breadth_first_search.rs`

 * *Files 12% similar despite different names*

```diff
@@ -1,314 +1,309 @@
-use super::data_structure::state_registry::{StateInRegistry, StateRegistry};
-use super::data_structure::{exceed_bound, BfsNodeInterface, SuccessorGenerator};
-use super::search::{Search, Solution};
-use super::util;
-use dypdl::variable_type;
-use std::collections;
+use super::data_structure::{exceed_bound, BfsNode, StateRegistry, SuccessorGenerator};
+use super::rollout::get_solution_cost_and_suffix;
+use super::search::{Parameters, Search, SearchInput, Solution};
+use super::util::{update_bound_if_better, update_solution, TimeKeeper};
+use dypdl::{variable_type, Transition, TransitionInterface};
+use std::collections::VecDeque;
 use std::error::Error;
 use std::fmt;
+use std::mem;
 use std::rc::Rc;
 
-/// Anytime Column Progressive Search (ACPS).
+/// Parameters for breadth-first search (BrFS).
+#[derive(Debug, PartialEq, Clone, Copy, Default)]
+pub struct BrfsParameters<T> {
+    /// Keep nodes in all layers for duplicate detection.
+    ///
+    /// BrFS searches layer by layer, where the i th layer contains states that can be reached with i transitions.
+    /// By default, BrFS only keeps states in the current layer to check for duplicates.
+    /// If `keep_all_layers` is `true`, BrFS keeps states in all layers to check for duplicates.
+    pub keep_all_layers: bool,
+    /// Common parameters.
+    pub parameters: Parameters<T>,
+}
+
+/// Breadth-first search solver.
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 ///
-/// It uses `h_evaluator` and `f_evaluator` for pruning.
-/// If `h_evaluator` returns `None`, the state is pruned.
-/// If `f_pruning` and `f_evaluator` returns a value that exceeds the primal bound, the state is pruned.
-///
-/// `ordered_by_f` indicates if the open list is ordered by the f-value.
-///
-/// # References
+/// It searches nodes in the breadth-first order.
 ///
-/// Ryo Kuroiwa and J. Christopher Beck."Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,""
-/// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
-///
-/// Sataya Gautam Vadlamudi, Piyush Gaurav, Sandip Aine, and Partha Pratim Chakrabarti. "Anytime Column Search,""
-/// Proceedings of AI 2012: Advances in Artificial Intelligence, pp. 254-255, 2012.
+/// Type parameter `N` is a node type that implements `BfsNode`.
+/// Type parameter `E` is a type of a function that evaluates a transition and insert a successor node into a state registry.
+/// The last argument of the function is the primal bound of the solution cost.
+/// Type parameter `B` is a type of a function that combines the g-value (the cost to a state) and the base cost.
+/// It should be the same function as the cost expression, e.g., `cost + base_cost` for `cost + w`.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{Acps, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::FNode;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
-/// };
-/// use dypdl_heuristic_search::search_algorithm::util::{
-///     ForwardSearchParameters, Parameters, ProgressiveSearchParameters,
+/// use dypdl_heuristic_search::{BrfsParameters, Search};
+/// use dypdl_heuristic_search::search_algorithm::{
+///     BreadthFirstSearch, FNode, SearchInput, SuccessorGenerator,
 /// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let h_evaluator = |_: &_, _: &_| Some(0);
-/// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-///
 /// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model(model.clone(), false);
-/// let progressive_parameters = ProgressiveSearchParameters::default();
-/// let parameters = ForwardSearchParameters {
+///
+/// let state = model.target.clone();
+/// let cost = 0;
+/// let h_evaluator = |_: &_| Some(0);
+/// let f_evaluator = |g, h, _: &_| g + h;
+/// let primal_bound = None;
+/// let node = FNode::generate_root_node(
+///     state,
+///     cost,
+///     &model,
+///     &h_evaluator,
+///     &f_evaluator,
+///     primal_bound,
+/// );
+/// let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+/// let input = SearchInput {
+///     node,
 ///     generator,
-///     parameters: Parameters::default(),
-///     initial_registry_capacity: None
+///     solution_suffix: &[],
 /// };
+/// let transition_evaluator =
+///     move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+///         node.insert_successor_node(
+///             transition,
+///             registry,
+///             &h_evaluator,
+///             &f_evaluator,
+///             primal_bound,
+///         )
+///     };
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let parameters = BrfsParameters::default();
 ///
-/// let mut solver = Acps::<_, FNode<_>, _, _>::new(
-///     model, h_evaluator, f_evaluator, true, true, progressive_parameters, parameters
+/// let mut solver = BreadthFirstSearch::<_, FNode<_>, _, _>::new(
+///     input, transition_evaluator, base_cost_evaluator, parameters,
 /// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub struct Acps<T, N, H, F>
+pub struct BreadthFirstSearch<'a, T, N, E, B, V = Transition>
 where
-    T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    T: variable_type::Numeric + fmt::Display + Ord + 'static,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    generator: SuccessorGenerator,
-    h_evaluator: H,
-    f_evaluator: F,
-    f_pruning: bool,
-    ordered_by_f: bool,
-    progressive_parameters: util::ProgressiveSearchParameters,
+    generator: SuccessorGenerator<V>,
+    suffix: &'a [V],
+    transition_evaluator: E,
+    base_cost_evaluator: B,
+    keep_all_layers: bool,
     primal_bound: Option<T>,
+    get_all_solutions: bool,
     quiet: bool,
-    width: usize,
-    open: Vec<collections::BinaryHeap<Rc<N>>>,
+    open: VecDeque<Rc<N>>,
+    next_open: VecDeque<Rc<N>>,
     registry: StateRegistry<T, N>,
-    time_keeper: util::TimeKeeper,
+    layer_index: usize,
+    layer_dual_bound: Option<T>,
+    time_keeper: TimeKeeper,
     solution: Solution<T>,
 }
 
-impl<T, N, H, F> Acps<T, N, H, F>
+impl<'a, T, N, E, B, V> BreadthFirstSearch<'a, T, N, E, B, V>
 where
-    T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    T: variable_type::Numeric + fmt::Display + Ord + 'static,
+    N: BfsNode<T, V> + Clone,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    /// Create a new ACPS solver.
+    /// Create a new breadth-first search solver.
     pub fn new(
-        model: Rc<dypdl::Model>,
-        h_evaluator: H,
-        f_evaluator: F,
-        f_pruning: bool,
-        ordered_by_f: bool,
-        progressive_parameters: util::ProgressiveSearchParameters,
-        parameters: util::ForwardSearchParameters<T>,
-    ) -> Acps<T, N, H, F> {
-        let time_keeper = parameters
+        input: SearchInput<'a, N, V>,
+        transition_evaluator: E,
+        base_cost_evaluator: B,
+        parameters: BrfsParameters<T>,
+    ) -> BreadthFirstSearch<'a, T, N, E, B, V> {
+        let mut time_keeper = parameters
             .parameters
             .time_limit
-            .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
+            .map_or_else(TimeKeeper::default, TimeKeeper::with_time_limit);
+        let get_all_solutions = parameters.parameters.get_all_solutions;
         let primal_bound = parameters.parameters.primal_bound;
         let quiet = parameters.parameters.quiet;
+        let mut open = VecDeque::new();
+        let next_open = VecDeque::new();
+        let mut registry = StateRegistry::new(input.generator.model.clone());
 
-        let mut open = vec![collections::BinaryHeap::new()];
-        let mut registry = StateRegistry::new(model);
-
-        if let Some(capacity) = parameters.initial_registry_capacity {
+        if let Some(capacity) = parameters.parameters.initial_registry_capacity {
             registry.reserve(capacity);
         }
 
         let mut solution = Solution::default();
-
-        if let Some((node, h, f)) =
-            N::generate_initial_node(&mut registry, &h_evaluator, &f_evaluator)
-        {
-            open[0].push(node);
+        if let Some(node) = input.node.clone() {
+            let (node, _) = registry.insert(node).unwrap();
+            open.push_back(node);
             solution.generated += 1;
-
-            if !quiet {
-                println!("Initial h = {}", h);
-            }
-
-            if f_pruning {
-                solution.best_bound = Some(f);
-            }
         } else {
             solution.is_infeasible = true;
         }
 
-        Acps {
-            generator: parameters.generator,
-            h_evaluator,
-            f_evaluator,
-            f_pruning,
-            ordered_by_f,
-            progressive_parameters,
+        time_keeper.stop();
+
+        BreadthFirstSearch {
+            generator: input.generator,
+            suffix: input.solution_suffix,
+            transition_evaluator,
+            base_cost_evaluator,
+            keep_all_layers: parameters.keep_all_layers,
             primal_bound,
+            get_all_solutions,
             quiet,
-            width: progressive_parameters.init,
             open,
+            next_open,
             registry,
+            layer_index: 0,
+            layer_dual_bound: None,
             time_keeper,
             solution,
         }
     }
 }
 
-impl<T, N, H, F> Search<T> for Acps<T, N, H, F>
+impl<'a, T, N, E, B, V> Search<T> for BreadthFirstSearch<'a, T, N, E, B, V>
 where
-    T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    T: variable_type::Numeric + fmt::Display + Ord + 'static,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
     fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
         if self.solution.is_terminated() {
             return Ok((self.solution.clone(), true));
         }
 
-        let mut i = 0;
-        let mut no_node = true;
+        self.time_keeper.start();
+        let model = &self.generator.model;
+        let suffix = self.suffix;
 
         loop {
-            let mut j = 0;
-            let mut goal_found = false;
-
-            while j < self.width && !self.open[i].is_empty() {
-                let node = self.open[i].pop().unwrap();
-
-                if node.closed() {
-                    continue;
+            if self.open.is_empty() {
+                if let Some(bound) = self.layer_dual_bound {
+                    self.solution.time = self.time_keeper.elapsed_time();
+                    update_bound_if_better(&mut self.solution, bound, model, self.quiet);
                 }
 
-                node.close();
-
-                let f = node.get_bound(self.registry.model());
-
-                if self.f_pruning
-                    && self.ordered_by_f
-                    && exceed_bound(self.registry.model(), f, self.primal_bound)
-                {
-                    self.open[i].clear();
-                    break;
+                if !self.quiet {
+                    println!(
+                        "Searched layer: {}, expanded: {}, elapsed time: {}",
+                        self.layer_index,
+                        self.solution.expanded,
+                        self.time_keeper.elapsed_time()
+                    );
                 }
 
-                if no_node {
-                    no_node = false;
+                if self.next_open.is_empty() {
+                    break;
                 }
 
-                if self.registry.model().is_base(node.state()) {
-                    if exceed_bound(self.registry.model(), node.cost(), self.primal_bound) {
-                        continue;
-                    } else {
-                        if !goal_found {
-                            goal_found = true;
-                        }
-
-                        if !self.quiet {
-                            println!(
-                                "New primal bound: {}, expanded: {}",
-                                node.cost(),
-                                self.solution.expanded
-                            );
-                        }
-
-                        let cost = node.cost();
-                        self.solution.cost = Some(cost);
-                        self.solution.transitions = node.transitions();
-                        self.primal_bound = Some(cost);
+                mem::swap(&mut self.open, &mut self.next_open);
 
-                        if let Some(bound) = self.solution.best_bound {
-                            self.solution.is_optimal = cost == bound;
+                if !self.keep_all_layers {
+                    self.registry.clear();
+                }
 
-                            if self.solution.is_optimal {
-                                self.solution.time = self.time_keeper.elapsed_time();
+                self.layer_index += 1;
+                self.layer_dual_bound = None;
+            }
 
-                                return Ok((self.solution.clone(), true));
-                            }
-                        }
+            while let Some(node) = self.open.pop_front() {
+                if node.is_closed() {
+                    continue;
+                }
+                node.close();
 
+                if let Some(dual_bound) = node.bound(model) {
+                    if exceed_bound(model, dual_bound, self.primal_bound) {
                         continue;
                     }
                 }
 
-                if self.time_keeper.check_time_limit() {
-                    if !self.quiet {
-                        println!("Reached time limit.");
-                        println!("Expanded: {}", self.solution.expanded);
+                if let Some((cost, suffix)) =
+                    get_solution_cost_and_suffix(model, &*node, suffix, &self.base_cost_evaluator)
+                {
+                    if !exceed_bound(model, cost, self.primal_bound) {
+                        self.primal_bound = Some(cost);
+                        let time = self.time_keeper.elapsed_time();
+                        update_solution(&mut self.solution, &*node, cost, suffix, time, self.quiet);
+                        self.time_keeper.stop();
+
+                        return Ok((self.solution.clone(), self.solution.is_optimal));
+                    } else if self.get_all_solutions {
+                        let mut solution = self.solution.clone();
+                        let time = self.time_keeper.elapsed_time();
+                        update_solution(&mut solution, &*node, cost, suffix, time, true);
+                        self.time_keeper.stop();
+
+                        return Ok((solution, false));
                     }
+                    continue;
+                }
 
+                if self.time_keeper.check_time_limit(self.quiet) {
                     self.solution.time_out = true;
                     self.solution.time = self.time_keeper.elapsed_time();
+                    self.time_keeper.stop();
 
                     return Ok((self.solution.clone(), true));
                 }
 
                 self.solution.expanded += 1;
 
-                let primal_bound = if self.f_pruning {
-                    self.primal_bound
-                } else {
-                    None
-                };
-
                 for transition in self.generator.applicable_transitions(node.state()) {
-                    let successor = node.generate_successor(
+                    if let Some((successor, new_generated)) = (self.transition_evaluator)(
+                        &node,
                         transition,
                         &mut self.registry,
-                        &self.h_evaluator,
-                        &self.f_evaluator,
-                        primal_bound,
-                    );
-
-                    if let Some((successor, _, _, new_generated)) = successor {
-                        while i + 1 >= self.open.len() {
-                            self.open.push(collections::BinaryHeap::new());
+                        self.primal_bound,
+                    ) {
+                        if let Some(bound) = successor.bound(model) {
+                            if !exceed_bound(model, bound, self.layer_dual_bound) {
+                                self.layer_dual_bound = Some(bound);
+                            }
                         }
 
-                        self.open[i + 1].push(successor);
+                        self.next_open.push_back(successor);
 
                         if new_generated {
                             self.solution.generated += 1;
                         }
                     }
                 }
-
-                j += 1;
-            }
-
-            if no_node && i + 1 == self.open.len() {
-                break;
-            } else if i + 1 == self.open.len() {
-                if self.progressive_parameters.reset && goal_found {
-                    self.width = self.progressive_parameters.init;
-                } else {
-                    self.width = self.progressive_parameters.increase_width(self.width);
-                }
-
-                if goal_found {
-                    self.solution.time = self.time_keeper.elapsed_time();
-
-                    return Ok((self.solution.clone(), false));
-                } else {
-                    i = 0;
-                    no_node = true;
-                }
-            } else {
-                i += 1;
             }
         }
 
         self.solution.is_infeasible = self.solution.cost.is_none();
         self.solution.is_optimal = self.solution.cost.is_some();
+        self.solution.best_bound = self.solution.cost;
         self.solution.time = self.time_keeper.elapsed_time();
+        self.time_keeper.stop();
         Ok((self.solution.clone(), true))
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/apps.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dbdfs.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,330 +1,341 @@
-use super::data_structure::state_registry::{StateInRegistry, StateRegistry};
-use super::data_structure::{exceed_bound, BfsNodeInterface, SuccessorGenerator};
-use super::util;
-use super::{Search, Solution};
-use dypdl::variable_type;
-use std::collections;
+use super::data_structure::{exceed_bound, BfsNode, StateRegistry, SuccessorGenerator};
+use super::rollout::get_solution_cost_and_suffix;
+use super::search::{Parameters, Search, SearchInput, Solution};
+use super::util::{print_dual_bound, update_solution, TimeKeeper};
+use dypdl::{variable_type, Transition, TransitionInterface};
 use std::error::Error;
 use std::fmt;
+use std::mem;
 use std::rc::Rc;
 
-/// Anytime Pack Progressive Search (APPS).
+/// Parameters for best-first search.
+#[derive(Debug, PartialEq, Clone, Copy)]
+pub struct DbdfsParameters<T> {
+    /// Width of the discrepancy to search.
+    pub width: usize,
+    /// Common parameters.
+    pub parameters: Parameters<T>,
+}
+
+impl<T: Default> Default for DbdfsParameters<T> {
+    fn default() -> Self {
+        Self {
+            width: 1,
+            parameters: Parameters::default(),
+        }
+    }
+}
+
+/// Discrepancy-Bounded Depth-First Search (DBDFS).
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 ///
-/// It uses `h_evaluator` and `f_evaluator` for pruning.
-/// If `h_evaluator` returns `None`, the state is pruned.
-/// If `f_pruning` and `f_evaluator` returns a value that exceeds the primal bound, the state is pruned.
-///
-/// `ordered_by_f` indicates if the open list is ordered by the f-value.
+/// It performs depth-first search where the discrepancy of searched nodes is bounded.
+/// When a node has the discrepancy of `d`, its best successor has the discrepancy of `d`,
+/// and other.successors have the discrepancy of `d + 1`.
+///
+/// Type parameter `N` is a node type that implements `BfsNode`.
+/// Type parameter `E` is a type of a function that evaluates a transition and insert a successor node into a state registry.
+/// The last argument of the function is the primal bound of the solution cost.
+/// Type parameter `B` is a type of a function that combines the g-value (the cost to a state) and the base cost.
+/// It should be the same function as the cost expression, e.g., `cost + base_cost` for `cost + w`.
 ///
 /// # References
 ///
 /// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
-/// Sataya Gautam Vadlamudi, Sandip Aine, Partha Pratim Chakrabarti. "Anytime Pack Search,"
-/// Natural Computing, vol. 15(3), pp. 395-414, 2016
+/// J. Christopher Beck. "Discrepancy-Bounded Depth First Search,"
+/// Second International Workshop on Integration of AI and OR Technologies in Constraint Programming for Combinatorial Optimization Problems (CPAIOR), 2000.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{Apps, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::FNode;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
-/// };
-/// use dypdl_heuristic_search::search_algorithm::util::{
-///     ForwardSearchParameters, Parameters, ProgressiveSearchParameters,
+/// use dypdl_heuristic_search::{DbdfsParameters, Parameters, Search};
+/// use dypdl_heuristic_search::search_algorithm::{
+///     Dbdfs, FNode, SearchInput, SuccessorGenerator,
 /// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let h_evaluator = |_: &_, _: &_| Some(0);
-/// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-///
 /// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model(model.clone(), false);
-/// let progressive_parameters = ProgressiveSearchParameters::default();
-/// let parameters = ForwardSearchParameters {
+///
+/// let state = model.target.clone();
+/// let cost = 0;
+/// let h_evaluator = |_: &_| Some(0);
+/// let f_evaluator = |g, h, _: &_| g + h;
+/// let primal_bound = None;
+/// let node = FNode::generate_root_node(
+///     state,
+///     cost,
+///     &model,
+///     &h_evaluator,
+///     &f_evaluator,
+///     primal_bound,
+/// );
+/// let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+/// let input = SearchInput {
+///     node,
 ///     generator,
-///     parameters: Parameters::default(),
-///     initial_registry_capacity: None
+///     solution_suffix: &[],
 /// };
+/// let transition_evaluator =
+///     move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+///         node.insert_successor_node(
+///             transition,
+///             registry,
+///             &h_evaluator,
+///             &f_evaluator,
+///             primal_bound,
+///         )
+///     };
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let parameters = DbdfsParameters::default();
 ///
-/// let mut solver = Apps::<_, FNode<_>, _, _>::new(
-///     model, h_evaluator, f_evaluator, true, true, progressive_parameters, parameters
+/// let mut solver = Dbdfs::<_, FNode<_>, _, _>::new(
+///     input, transition_evaluator, base_cost_evaluator, parameters,
 /// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub struct Apps<T, N, H, F>
+pub struct Dbdfs<'a, T, N, E, B, V = Transition>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    generator: SuccessorGenerator,
-    h_evaluator: H,
-    f_evaluator: F,
-    f_pruning: bool,
-    ordered_by_f: bool,
-    progressive_parameters: util::ProgressiveSearchParameters,
+    generator: SuccessorGenerator<V>,
+    suffix: &'a [V],
+    transition_evaluator: E,
+    base_cost_evaluator: B,
     primal_bound: Option<T>,
     get_all_solutions: bool,
     quiet: bool,
     width: usize,
-    open: collections::BinaryHeap<Rc<N>>,
-    children: collections::BinaryHeap<Rc<N>>,
-    suspend: collections::BinaryHeap<Rc<N>>,
+    discrepancy_limit: usize,
+    open: Vec<(Rc<N>, usize)>,
+    next_open: Vec<(Rc<N>, usize)>,
     registry: StateRegistry<T, N>,
-    goal_found: bool,
-    time_keeper: util::TimeKeeper,
+    time_keeper: TimeKeeper,
     solution: Solution<T>,
 }
 
-impl<T, N, H, F> Apps<T, N, H, F>
+impl<'a, T, N, E, B, V> Dbdfs<'a, T, N, E, B, V>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    /// Create a new APPS solver.
+    /// Create a new DBDFS solver.
     pub fn new(
-        model: Rc<dypdl::Model>,
-        h_evaluator: H,
-        f_evaluator: F,
-        f_pruning: bool,
-        ordered_by_f: bool,
-        progressive_parameters: util::ProgressiveSearchParameters,
-        parameters: util::ForwardSearchParameters<T>,
-    ) -> Apps<T, N, H, F> {
-        let time_keeper = parameters
+        input: SearchInput<'a, N, V>,
+        transition_evaluator: E,
+        base_cost_evaluator: B,
+        parameters: DbdfsParameters<T>,
+    ) -> Dbdfs<'a, T, N, E, B, V> {
+        let mut time_keeper = parameters
             .parameters
             .time_limit
-            .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
+            .map_or_else(TimeKeeper::default, TimeKeeper::with_time_limit);
         let primal_bound = parameters.parameters.primal_bound;
         let get_all_solutions = parameters.parameters.get_all_solutions;
         let quiet = parameters.parameters.quiet;
 
-        let mut open = collections::BinaryHeap::new();
-        let children = collections::BinaryHeap::new();
-        let suspend = collections::BinaryHeap::new();
-        let mut registry = StateRegistry::new(model);
+        let mut open = Vec::new();
+        let next_open = Vec::new();
+        let mut registry = StateRegistry::<_, _>::new(input.generator.model.clone());
 
-        if let Some(capacity) = parameters.initial_registry_capacity {
+        if let Some(capacity) = parameters.parameters.initial_registry_capacity {
             registry.reserve(capacity);
         }
 
         let mut solution = Solution::default();
 
-        if let Some((node, h, f)) =
-            N::generate_initial_node(&mut registry, &h_evaluator, &f_evaluator)
-        {
-            open.push(node);
+        if let Some(node) = input.node {
+            let (node, _) = registry.insert(node).unwrap();
+            solution.best_bound = node.bound(&input.generator.model);
+            open.push((node, 0));
             solution.generated += 1;
 
             if !quiet {
-                println!("Initial h = {}", h);
-            }
-
-            if f_pruning {
-                solution.best_bound = Some(f);
+                solution.time = time_keeper.elapsed_time();
+                print_dual_bound(&solution);
             }
         } else {
             solution.is_infeasible = true;
         }
 
-        Apps {
-            generator: parameters.generator,
-            h_evaluator,
-            f_evaluator,
-            f_pruning,
-            ordered_by_f,
-            progressive_parameters,
+        let discrepancy_limit = parameters.width - 1;
+
+        if !quiet {
+            println!("Initial discrepancy limit: {}", discrepancy_limit);
+        }
+
+        time_keeper.stop();
+
+        Dbdfs {
+            generator: input.generator,
+            suffix: input.solution_suffix,
+            transition_evaluator,
+            base_cost_evaluator,
             primal_bound,
             get_all_solutions,
             quiet,
-            width: progressive_parameters.init,
+            width: parameters.width,
+            discrepancy_limit,
             open,
-            children,
-            suspend,
+            next_open,
             registry,
-            goal_found: false,
             time_keeper,
             solution,
         }
     }
 }
 
-impl<T, N, H, F> Search<T> for Apps<T, N, H, F>
+impl<'a, T, N, E, B, V> Search<T> for Dbdfs<'a, T, N, E, B, V>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
     fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
-        if self.solution.is_terminated() {
-            return Ok((self.solution.clone(), true));
-        }
+        self.time_keeper.start();
+        let model = &self.generator.model;
 
-        while !self.open.is_empty() || !self.suspend.is_empty() {
-            // Run out current candidates
+        while !self.open.is_empty() || !self.next_open.is_empty() {
             if self.open.is_empty() {
-                if self.progressive_parameters.reset && self.goal_found {
-                    self.width = self.progressive_parameters.init;
-                } else {
-                    self.width = self.progressive_parameters.increase_width(self.width);
-                }
+                mem::swap(&mut self.open, &mut self.next_open);
+                self.discrepancy_limit += self.width;
 
-                while self.open.len() < self.width {
-                    if let Some(node) = self.suspend.pop() {
-                        self.open.push(node);
-                    } else {
-                        break;
-                    }
+                if !self.quiet {
+                    println!(
+                        "New discrepancy limit: {}, expanded: {}, elapsed time: {}",
+                        self.discrepancy_limit,
+                        self.solution.expanded,
+                        self.time_keeper.elapsed_time()
+                    );
                 }
-
-                self.goal_found = false;
             }
 
-            while !self.open.is_empty() {
-                while !self.open.is_empty() {
-                    let node = self.open.pop().unwrap();
+            let (node, discrepancy) = self.open.pop().unwrap();
 
-                    if node.closed() {
-                        continue;
-                    }
+            if node.is_closed() {
+                continue;
+            }
+            node.close();
 
-                    node.close();
+            if let Some(dual_bound) = node.bound(model) {
+                if exceed_bound(model, dual_bound, self.primal_bound) {
+                    continue;
+                }
+            }
 
-                    let f = node.get_bound(self.registry.model());
+            if let Some((cost, suffix)) =
+                get_solution_cost_and_suffix(model, &*node, self.suffix, &self.base_cost_evaluator)
+            {
+                if !exceed_bound(model, cost, self.primal_bound) {
+                    self.primal_bound = Some(cost);
+                    let time = self.time_keeper.elapsed_time();
+                    update_solution(&mut self.solution, &*node, cost, suffix, time, self.quiet);
+                    self.time_keeper.stop();
+
+                    return Ok((self.solution.clone(), self.solution.is_optimal));
+                } else if self.get_all_solutions {
+                    let mut solution = self.solution.clone();
+                    let time = self.time_keeper.elapsed_time();
+                    update_solution(&mut solution, &*node, cost, suffix, time, true);
+                    self.time_keeper.stop();
 
-                    if self.f_pruning
-                        && self.ordered_by_f
-                        && exceed_bound(self.registry.model(), f, self.primal_bound)
-                    {
-                        self.open.clear();
-                        break;
-                    }
+                    return Ok((solution, false));
+                }
+                continue;
+            }
 
-                    if self.registry.model().is_base(node.state()) {
-                        if exceed_bound(self.registry.model(), node.cost(), self.primal_bound) {
-                            if self.get_all_solutions {
-                                let mut solution = self.solution.clone();
-                                solution.cost = Some(node.cost());
-                                solution.transitions = node.transitions();
-                                solution.time = self.time_keeper.elapsed_time();
-
-                                return Ok((solution, false));
-                            }
-
-                            continue;
-                        } else {
-                            if !self.goal_found {
-                                self.goal_found = true;
-                            }
-
-                            if !self.quiet {
-                                println!(
-                                    "New primal bound: {}, expanded: {}",
-                                    node.cost(),
-                                    self.solution.expanded
-                                );
-                            }
-
-                            let cost = node.cost();
-                            self.solution.cost = Some(cost);
-                            self.solution.transitions = node.transitions();
-                            self.primal_bound = Some(cost);
-
-                            if let Some(bound) = self.solution.best_bound {
-                                self.solution.is_optimal = cost == bound;
-                            }
+            if self.time_keeper.check_time_limit(self.quiet) {
+                self.solution.time_out = true;
+                self.solution.time = self.time_keeper.elapsed_time();
+                self.time_keeper.stop();
 
-                            self.solution.time = self.time_keeper.elapsed_time();
+                return Ok((self.solution.clone(), true));
+            }
 
-                            return Ok((self.solution.clone(), self.solution.is_optimal));
-                        }
-                    }
+            self.solution.expanded += 1;
 
-                    if self.time_keeper.check_time_limit() {
-                        if !self.quiet {
-                            println!("Reached time limit.");
-                            println!("Expanded: {}", self.solution.expanded);
-                        }
+            let mut successors = vec![];
 
-                        self.solution.time_out = true;
-                        self.solution.time = self.time_keeper.elapsed_time();
+            for transition in self.generator.applicable_transitions(node.state()) {
+                if let Some((successor, new_generated)) = (self.transition_evaluator)(
+                    &node,
+                    transition,
+                    &mut self.registry,
+                    self.primal_bound,
+                ) {
+                    successors.push(successor);
 
-                        return Ok((self.solution.clone(), true));
+                    if new_generated {
+                        self.solution.generated += 1;
                     }
+                }
+            }
 
-                    self.solution.expanded += 1;
+            successors.sort();
 
-                    let primal_bound = if self.f_pruning {
-                        self.primal_bound
-                    } else {
-                        None
-                    };
-
-                    for transition in self.generator.applicable_transitions(node.state()) {
-                        let successor = node.generate_successor(
-                            transition,
-                            &mut self.registry,
-                            &self.h_evaluator,
-                            &self.f_evaluator,
-                            primal_bound,
-                        );
-
-                        if let Some((successor, _, _, new_generated)) = successor {
-                            self.children.push(successor);
-
-                            if new_generated {
-                                self.solution.generated += 1;
-                            }
-                        }
-                    }
-                }
+            if let Some(best) = successors.pop() {
+                let mut successors = successors
+                    .into_iter()
+                    .map(|x| (x, discrepancy + 1))
+                    .collect();
 
-                while self.open.len() < self.width {
-                    if let Some(node) = self.children.pop() {
-                        if !node.closed() {
-                            self.open.push(node);
-                        }
-                    } else {
-                        break;
-                    }
+                if discrepancy < self.discrepancy_limit {
+                    self.open.append(&mut successors);
+                } else {
+                    self.next_open.append(&mut successors);
                 }
 
-                while let Some(node) = self.children.pop() {
-                    if !node.closed() {
-                        self.suspend.push(node);
-                    }
-                }
+                self.open.push((best, discrepancy));
             }
         }
 
         self.solution.is_infeasible = self.solution.cost.is_none();
         self.solution.is_optimal = self.solution.cost.is_some();
+        self.solution.best_bound = self.solution.cost;
         self.solution.time = self.time_keeper.elapsed_time();
+        self.time_keeper.stop();
         Ok((self.solution.clone(), true))
     }
 }
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use dypdl::Integer;
+
+    #[test]
+    fn parameters_default() {
+        let parameters = DbdfsParameters::<Integer>::default();
+        assert_eq!(parameters.width, 1);
+        assert_eq!(parameters.parameters, Parameters::default());
+    }
+}
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/beam_search.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/beam_search.rs`

 * *Files 11% similar despite different names*

```diff
@@ -1,280 +1,309 @@
-use super::data_structure::beam::{BeamInterface, InformationInBeam};
-use super::data_structure::state_registry::{StateInRegistry, StateRegistry};
-use super::data_structure::{
-    exceed_bound, BeamSearchProblemInstance, CustomCostNodeInterface, CustomCostParent,
-    TransitionWithCustomCost,
-};
-use super::rollout::rollout;
-use super::search::Solution;
-use super::util;
-use dypdl::variable_type;
+use super::data_structure::{exceed_bound, Beam, BfsNode, StateRegistry};
+use super::rollout::get_solution_cost_and_suffix;
+use super::search::{Parameters, SearchInput, Solution};
+use super::util::TimeKeeper;
+use dypdl::{variable_type, TransitionInterface};
+use std::fmt::Display;
 use std::mem;
 use std::rc::Rc;
 
 /// Parameters for beam search.
-#[derive(Debug, PartialEq, Clone, Copy, Default)]
-pub struct BeamSearchParameters<T, U> {
-    /// Beam size.
+#[derive(Debug, PartialEq, Clone, Copy)]
+pub struct BeamSearchParameters<T> {
+    /// Beam size, the number of nodes to keep at each layer.
     pub beam_size: usize,
-    /// Maximize.
-    pub maximize: bool,
-    /// Use f-values for pruning.
-    pub f_pruning: bool,
-    /// Bound for the f-value.
-    pub f_bound: Option<U>,
     /// Keep nodes in all layers for duplicate detection.
     ///
     /// Beam search searches layer by layer, where the i th layer contains states that can be reached with i transitions.
-    /// By default, this solver only keeps states in the current layer to check for duplicates.
-    /// If `keep_all_layers` is `true`, this solver keeps states in all layers to check for duplicates.
+    /// By default, beam search only keeps states in the current layer to check for duplicates.
+    /// If `keep_all_layers` is `true`, beam search keeps states in all layers to check for duplicates.
     pub keep_all_layers: bool,
     /// Common parameters.
-    pub parameters: util::Parameters<T>,
+    pub parameters: Parameters<T>,
+}
+
+impl<T: Default> Default for BeamSearchParameters<T> {
+    fn default() -> Self {
+        Self {
+            beam_size: 1,
+            keep_all_layers: false,
+            parameters: Parameters::default(),
+        }
+    }
 }
 
 /// Performs beam search.
 ///
 /// This function uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 ///
-/// The f-value, the priority of a node, is computed by f_evaluator, which is a function of the g-value, the h-value, and the state.
-/// The h-value is computed by h_evaluator.
-/// At each depth, the top beam_size nodes minimizing (maximizing) the f-values are kept if `maximize == false` (`true`).
+/// It keeps the best `beam_size` nodes at each layer.
+///
+/// Type parameter `N` is a node type that implements `BfsNode`.
+/// Type parameter `E` is a type of a function that evaluates a transition and generate a successor node.
+/// The last argument of the function is the primal bound of the solution cost.
+/// Type parameter `B` is a type of a function that combines the g-value (the cost to a state) and the base cost.
+/// It should be the same function as the cost expression, e.g., `cost + base_cost` for `cost + w`.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{beam_search, BeamSearchParameters, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::beam::Beam;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::{
-///     BeamSearchNode, BeamSearchProblemInstance, TransitionWithCustomCost,
-/// };
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
+/// use dypdl_heuristic_search::Search;
+/// use dypdl_heuristic_search::search_algorithm::{
+///     beam_search, BeamSearchParameters, FNode, SearchInput, SuccessorGenerator,
 /// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let h_evaluator = |_: &_, _: &_| Some(0);
-/// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-///
 /// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model_without_custom_cost(model.clone(), false);
-/// let problem = BeamSearchProblemInstance {
-///     target: model.target.clone().into(),
+///
+/// let state = model.target.clone();
+/// let cost = 0;
+/// let h_evaluator = |_: &_| Some(0);
+/// let f_evaluator = |g, h, _: &_| g + h;
+/// let primal_bound = None;
+/// let node = FNode::generate_root_node(
+///     state,
+///     cost,
+///     &model,
+///     &h_evaluator,
+///     &f_evaluator,
+///     primal_bound,
+/// );
+/// let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+/// let input = SearchInput {
+///     node,
 ///     generator,
-///     cost: 0,
-///     g: 0,
 ///     solution_suffix: &[],
 /// };
-/// let parameters = BeamSearchParameters { beam_size: 1, ..Default::default() };
-/// let beam_constructor = |beam_size| Beam::<_, _, BeamSearchNode<_, _>>::new(beam_size);
-/// let solution = beam_search(&problem, &beam_constructor, h_evaluator, f_evaluator, parameters);
+/// let transition_evaluator = move |node: &FNode<_>, transition, primal_bound| {
+///     node.generate_successor_node(
+///         transition,
+///         &model,
+///         &h_evaluator,
+///         &f_evaluator,
+///         primal_bound,
+///     )
+/// };
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let parameters = BeamSearchParameters::default();
+/// let solution = beam_search(
+///     &input, transition_evaluator, base_cost_evaluator, parameters,
+/// );
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions.len(), 1);
 /// assert_eq!(Transition::from(solution.transitions[0].clone()), increment);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub fn beam_search<T, U, I, B, C, H, F>(
-    problem: &BeamSearchProblemInstance<T, U>,
-    beam_constructor: &C,
-    h_evaluator: H,
-    f_evaluator: F,
-    parameters: BeamSearchParameters<T, U>,
-) -> Solution<T, TransitionWithCustomCost>
+pub fn beam_search<'a, T, N, E, B, V>(
+    input: &'a SearchInput<'a, N, V>,
+    transition_evaluator: E,
+    base_cost_evaluator: B,
+    parameters: BeamSearchParameters<T>,
+) -> Solution<T, V>
 where
-    T: variable_type::Numeric,
-    U: variable_type::Numeric + Ord,
-    I: InformationInBeam<T, U> + CustomCostNodeInterface<T, U>,
-    B: BeamInterface<T, U, I>,
-    C: Fn(usize) -> B,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<U>,
-    F: Fn(U, U, &StateInRegistry, &dypdl::Model) -> U,
+    T: variable_type::Numeric + Ord + Display,
+    N: BfsNode<T, V> + Clone,
+    E: Fn(&N, Rc<V>, Option<T>) -> Option<N>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
 {
     let time_keeper = parameters
         .parameters
         .time_limit
-        .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
+        .map_or_else(TimeKeeper::default, TimeKeeper::with_time_limit);
     let quiet = parameters.parameters.quiet;
-    let maximize = parameters.maximize;
     let mut primal_bound = parameters.parameters.primal_bound;
-    let f_bound = if parameters.f_pruning {
-        parameters.f_bound
-    } else {
-        None
-    };
-    let keep_all_layers = parameters.keep_all_layers;
 
-    let model = &problem.generator.model;
-    let generator = &problem.generator;
-    let mut current_beam = beam_constructor(parameters.beam_size);
-    let mut next_beam = beam_constructor(parameters.beam_size);
+    let model = &input.generator.model;
+    let generator = &input.generator;
+    let suffix = input.solution_suffix;
+    let mut current_beam = Beam::<_, _>::new(parameters.beam_size);
+    let mut next_beam = Beam::<_, _, _>::new(parameters.beam_size);
     let mut registry = StateRegistry::new(model.clone());
-    registry.reserve(current_beam.capacity());
-
-    let cost = problem.cost;
-    let g = problem.g;
-    let initial_state = problem.target.clone();
-
-    let h = h_evaluator(&initial_state, model);
-
-    if h.is_none() {
-        return Solution {
-            is_infeasible: true,
-            ..Default::default()
-        };
-    }
-
-    let h = h.unwrap();
-    let f = f_evaluator(g, h, &initial_state, model);
+    let capacity = parameters
+        .parameters
+        .initial_registry_capacity
+        .unwrap_or_else(|| current_beam.capacity());
+    registry.reserve(capacity);
 
-    if f_bound.map_or(false, |bound| {
-        (maximize && f <= bound) || (!maximize && f >= bound)
-    }) {
+    let node = if let Some(node) = input.node.clone() {
+        node
+    } else {
         return Solution {
             is_infeasible: true,
             ..Default::default()
         };
-    }
+    };
 
-    let (g, f) = if maximize { (-g, -f) } else { (g, f) };
-    let constructor = |state, cost, _: Option<&_>| Some(I::new(g, f, state, cost, None, None));
-    current_beam.insert(&mut registry, initial_state, cost, g, f, constructor);
+    current_beam.insert(&mut registry, node);
 
-    if !keep_all_layers {
+    if !parameters.keep_all_layers {
         registry.clear();
     }
 
     let mut expanded = 0;
     let mut generated = 1;
     let mut pruned = false;
+    let mut best_dual_bound = None;
+    let mut layer_index = 0;
 
     while !current_beam.is_empty() {
-        let mut incumbent: Option<(Rc<I>, T, _)> = None;
+        let mut incumbent = None;
+        let mut layer_dual_bound = None;
+        let previously_pruned = pruned;
 
         for node in current_beam.drain() {
-            if let Some(result) = rollout(node.state(), node.cost(), problem.solution_suffix, model)
-            {
-                if result.is_base {
-                    if !exceed_bound(model, result.cost, primal_bound) {
-                        primal_bound = Some(node.cost());
-                        incumbent = Some((node, result.cost, result.transitions));
-                    }
-
+            if let Some(dual_bound) = node.bound(model) {
+                if exceed_bound(model, dual_bound, primal_bound) {
                     continue;
                 }
             }
 
-            if time_keeper.check_time_limit() {
-                if !quiet {
-                    println!("Reached time limit.");
+            if let Some((cost, suffix)) =
+                get_solution_cost_and_suffix(model, &*node, suffix, &base_cost_evaluator)
+            {
+                if !exceed_bound(model, cost, primal_bound) {
+                    primal_bound = Some(cost);
+                    incumbent = Some((node, cost, suffix));
+
+                    if Some(cost) == best_dual_bound {
+                        break;
+                    }
                 }
+                continue;
+            }
 
-                return incumbent.map_or_else(
+            if time_keeper.check_time_limit(quiet) {
+                let solution = incumbent.map_or_else(
                     || Solution {
                         expanded,
                         generated,
                         time: time_keeper.elapsed_time(),
                         time_out: true,
                         ..Default::default()
                     },
                     |(node, cost, suffix)| {
                         let mut transitions = node.transitions();
                         transitions.extend_from_slice(suffix);
                         Solution {
                             cost: Some(cost),
+                            best_bound: best_dual_bound,
                             transitions,
                             expanded,
                             generated,
                             time: time_keeper.elapsed_time(),
                             time_out: true,
                             ..Default::default()
                         }
                     },
                 );
+
+                return solution;
             }
 
             if pruned && incumbent.is_some() {
                 continue;
             }
 
             expanded += 1;
 
-            let parent = CustomCostParent {
-                state: node.state(),
-                cost: node.cost(),
-                g: if maximize { -node.g() } else { node.g() },
-            };
-
             for transition in generator.applicable_transitions(node.state()) {
-                if let Some((state, cost, g, f)) = transition.generate_successor_state(
-                    &parent,
-                    model,
-                    f_bound,
-                    &h_evaluator,
-                    &f_evaluator,
-                    maximize,
-                ) {
-                    let (g, f) = if maximize { (-g, -f) } else { (g, f) };
-                    let constructor = |state, cost, _: Option<&_>| {
-                        Some(I::new(g, f, state, cost, Some(&node), Some(transition)))
-                    };
-                    let (new_generated, beam_pruning) =
-                        next_beam.insert(&mut registry, state, cost, g, f, constructor);
+                if let Some(successor) = transition_evaluator(&node, transition, primal_bound) {
+                    if let Some(bound) = successor.bound(model) {
+                        if !exceed_bound(model, bound, layer_dual_bound) {
+                            layer_dual_bound = Some(bound);
+                        }
+                    }
+
+                    let (new_generated, beam_pruning) = next_beam.insert(&mut registry, successor);
 
                     if !pruned && beam_pruning {
                         pruned = true;
                     }
 
                     if new_generated {
                         generated += 1;
                     }
                 }
             }
         }
 
         if !quiet {
-            println!("Expanded: {}", expanded);
+            println!(
+                "Searched layer: {}, expanded: {}, elapsed time: {}",
+                layer_index,
+                expanded,
+                time_keeper.elapsed_time()
+            );
+        }
+
+        if let (false, Some(value)) = (previously_pruned, layer_dual_bound) {
+            if best_dual_bound.map_or(true, |bound| !exceed_bound(model, bound, Some(value))) {
+                best_dual_bound = layer_dual_bound;
+            }
         }
 
         if let Some((node, cost, suffix)) = &incumbent {
             let mut transitions = node.transitions();
             transitions.extend_from_slice(suffix);
+            let is_optimal = (!pruned && next_beam.is_empty()) || Some(*cost) == best_dual_bound;
 
             return Solution {
                 cost: Some(*cost),
+                best_bound: if is_optimal {
+                    Some(*cost)
+                } else {
+                    best_dual_bound
+                },
                 transitions,
                 expanded,
                 generated,
-                is_optimal: !pruned && next_beam.is_empty(),
+                is_optimal,
                 time: time_keeper.elapsed_time(),
                 ..Default::default()
             };
         }
 
         mem::swap(&mut current_beam, &mut next_beam);
 
-        if !keep_all_layers {
+        if !parameters.keep_all_layers {
             registry.clear();
         }
+
+        layer_index += 1;
     }
 
     Solution {
+        is_infeasible: !pruned,
+        best_bound: if pruned { best_dual_bound } else { None },
         expanded,
         generated,
-        is_infeasible: !pruned,
         time: time_keeper.elapsed_time(),
         ..Default::default()
     }
 }
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+    use dypdl::Integer;
+
+    #[test]
+    fn parameters_default() {
+        let parameters = BeamSearchParameters::<Integer>::default();
+        assert_eq!(parameters.beam_size, 1);
+        assert!(!parameters.keep_all_layers);
+        assert_eq!(parameters.parameters, Parameters::default());
+    }
+}
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/best_first_search.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/best_first_search.rs`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-use super::data_structure::state_registry::{StateInRegistry, StateRegistry};
-use super::data_structure::{
-    exceed_bound, BfsNodeInterface, HashableSignatureVariables, SuccessorGenerator,
-};
-use super::search::{Search, Solution};
-use super::util;
-use dypdl::{variable_type, ReduceFunction};
+use super::data_structure::{exceed_bound, BfsNode, StateRegistry, SuccessorGenerator};
+use super::rollout::get_solution_cost_and_suffix;
+use super::search::{Parameters, Search, SearchInput, Solution};
+use super::util::{update_bound_if_better, update_solution, TimeKeeper};
+use dypdl::{variable_type, Transition, TransitionInterface};
 use std::collections::BinaryHeap;
 use std::error::Error;
 use std::fmt;
 use std::marker::PhantomData;
 use std::rc::Rc;
 
 /// Best-first search solver.
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 ///
-/// It uses `h_evaluator` and `f_evaluator` for pruning.
-/// If `h_evaluator` returns `None`, the state is pruned.
-/// If `f_pruning` and `f_evaluator` returns a value that exceeds the primal bound, the state is pruned.
+/// It searches a node in the best-first order.
 ///
-/// `ordered_by_f` indicates if the open list is ordered by the f-value.
-///
-/// `is_optimal` indicates if the optimality is guaranteed.
+/// Type parameter `N` is a node type that implements `BfsNode`.
+/// Type parameter `E` is a type of a function that evaluates a transition and insert a successor node into a state registry.
+/// The last argument of the function is the primal bound of the solution cost.
+/// Type parameter `B` is a type of a function that combines the g-value (the cost to a state) and the base cost.
+/// It should be the same function as the cost expression, e.g., `cost + base_cost` for `cost + w`.
 ///
 /// # References
 ///
 /// Ryo Kuroiwa and J. Christopher Beck. "Domain-Independent Dynamic Programming: Generic State Space Search for Combinatorial Optimization,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
 /// Stephen Edelkamp, Shahid Jabbar, Alberto Lluch Lafuente. "Cost-Algebraic Heuristic Search,"
@@ -36,249 +34,233 @@
 /// Peter E. Hart, Nills J. Nilsson, Bertram Raphael. "A Formal Basis for the Heuristic Determination of Minimum Cost Paths",
 /// IEEE Transactions of Systems Science and Cybernetics, vol. SSC-4(2), pp. 100-107, 1968.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{BestFirstSearch, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::FNode;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
-/// };
-/// use dypdl_heuristic_search::search_algorithm::util::{
-///     ForwardSearchParameters, Parameters,
+/// use dypdl_heuristic_search::{Parameters, Search};
+/// use dypdl_heuristic_search::search_algorithm::{
+///     BestFirstSearch, FNode, SearchInput, SuccessorGenerator,
 /// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let h_evaluator = |_: &_, _: &_| Some(0);
-/// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-///
 /// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model(model.clone(), false);
-/// let parameters = ForwardSearchParameters {
+///
+/// let state = model.target.clone();
+/// let cost = 0;
+/// let h_evaluator = |_: &_| Some(0);
+/// let f_evaluator = |g, h, _: &_| g + h;
+/// let primal_bound = None;
+/// let node = FNode::generate_root_node(
+///     state,
+///     cost,
+///     &model,
+///     &h_evaluator,
+///     &f_evaluator,
+///     primal_bound,
+/// );
+/// let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+/// let input = SearchInput {
+///     node,
 ///     generator,
-///     parameters: Parameters::default(),
-///     initial_registry_capacity: None
+///     solution_suffix: &[],
 /// };
+/// let transition_evaluator =
+///     move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+///         node.insert_successor_node(
+///             transition,
+///             registry,
+///             &h_evaluator,
+///             &f_evaluator,
+///             primal_bound,
+///         )
+///     };
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let parameters = Parameters::default();
 ///
 /// let mut solver = BestFirstSearch::<_, FNode<_>, _, _>::new(
-///     model, h_evaluator, f_evaluator, true, true, true, parameters
+///     input, transition_evaluator, base_cost_evaluator, parameters,
 /// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub struct BestFirstSearch<T, N, H, F>
+pub struct BestFirstSearch<'a, T, N, E, B, V = Transition>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    generator: SuccessorGenerator,
-    h_evaluator: H,
-    f_evaluator: F,
-    f_pruning: bool,
-    ordered_by_f: bool,
-    is_optimal: bool,
+    generator: SuccessorGenerator<V>,
+    suffix: &'a [V],
+    transition_evaluator: E,
+    base_cost_evaluator: B,
     primal_bound: Option<T>,
     get_all_solutions: bool,
     quiet: bool,
     open: BinaryHeap<Rc<N>>,
     registry: StateRegistry<T, N>,
-    time_keeper: util::TimeKeeper,
+    time_keeper: TimeKeeper,
     solution: Solution<T>,
     phantom: PhantomData<N>,
 }
 
-impl<T, N, H, F> BestFirstSearch<T, N, H, F>
+impl<'a, T, N, E, B, V> BestFirstSearch<'a, T, N, E, B, V>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    /// Create a new best-first search solver.
+    /// Creates a new best-first search solver.
     pub fn new(
-        model: Rc<dypdl::Model>,
-        h_evaluator: H,
-        f_evaluator: F,
-        f_pruning: bool,
-        ordered_by_f: bool,
-        is_optimal: bool,
-        parameters: util::ForwardSearchParameters<T>,
-    ) -> BestFirstSearch<T, N, H, F> {
-        let time_keeper = parameters
-            .parameters
+        input: SearchInput<'a, N, V>,
+        transition_evaluator: E,
+        base_cost_evaluator: B,
+        parameters: Parameters<T>,
+    ) -> BestFirstSearch<T, N, E, B, V> {
+        let mut time_keeper = parameters
             .time_limit
-            .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
-        let primal_bound = parameters.parameters.primal_bound;
-        let get_all_solutions = parameters.parameters.get_all_solutions;
-        let quiet = parameters.parameters.quiet;
+            .map_or_else(TimeKeeper::default, TimeKeeper::with_time_limit);
+        let primal_bound = parameters.primal_bound;
+        let get_all_solutions = parameters.get_all_solutions;
+        let quiet = parameters.quiet;
 
         let mut open = BinaryHeap::new();
-        let mut registry = StateRegistry::new(model);
+        let mut registry = StateRegistry::new(input.generator.model.clone());
 
         if let Some(capacity) = parameters.initial_registry_capacity {
             registry.reserve(capacity);
         }
 
         let mut solution = Solution::default();
-
-        if let Some((node, h, f)) =
-            N::generate_initial_node(&mut registry, &h_evaluator, &f_evaluator)
-        {
+        if let Some(node) = input.node {
+            let (node, _) = registry.insert(node).unwrap();
             open.push(node);
             solution.generated += 1;
-
-            if !quiet {
-                println!("Initial h = {}", h);
-            }
-
-            if f_pruning && is_optimal {
-                solution.best_bound = Some(f);
-            }
         } else {
             solution.is_infeasible = true;
         }
 
+        time_keeper.stop();
+
         BestFirstSearch {
-            generator: parameters.generator,
-            h_evaluator,
-            f_evaluator,
-            f_pruning,
-            ordered_by_f,
-            is_optimal,
+            generator: input.generator,
+            suffix: input.solution_suffix,
+            transition_evaluator,
+            base_cost_evaluator,
             primal_bound,
             get_all_solutions,
             quiet,
             open,
             registry,
             time_keeper,
             solution,
             phantom: PhantomData::default(),
         }
     }
 }
 
-impl<T, N, H, F> Search<T> for BestFirstSearch<T, N, H, F>
+impl<'a, T, N, E, B, V> Search<T> for BestFirstSearch<'a, T, N, E, B, V>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry<Rc<HashableSignatureVariables>>, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry<Rc<HashableSignatureVariables>>, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
     fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
-        let minimize = self.registry.model().reduce_function == ReduceFunction::Min;
+        self.time_keeper.start();
+        let model = &self.generator.model;
 
         while let Some(node) = self.open.pop() {
-            if node.closed() {
+            if node.is_closed() {
                 continue;
             }
-
             node.close();
 
-            let f = node.get_bound(self.registry.model());
-
-            if self.f_pruning
-                && self.ordered_by_f
-                && exceed_bound(self.registry.model(), f, self.primal_bound)
-            {
-                self.open.clear();
-                break;
-            }
-
-            if let Some(best_bound) = self.solution.best_bound {
-                if (minimize && f > best_bound) || (!minimize && f < best_bound) {
-                    self.solution.best_bound = Some(f);
-
-                    if !self.quiet {
-                        println!("f = {}, expanded: {}", f, self.solution.expanded);
+            if let Some(dual_bound) = node.bound(model) {
+                if exceed_bound(model, dual_bound, self.primal_bound) {
+                    if N::ordered_by_bound() {
+                        self.open.clear();
                     }
+                    continue;
                 }
-            }
-
-            if self.registry.model().is_base(node.state()) {
-                if exceed_bound(self.registry.model(), node.cost(), self.primal_bound) {
-                    if self.get_all_solutions {
-                        let mut solution = self.solution.clone();
-                        solution.cost = Some(node.cost());
-                        solution.transitions = node.transitions();
-                        solution.time = self.time_keeper.elapsed_time();
 
-                        return Ok((solution, false));
-                    }
+                if N::ordered_by_bound() || self.open.is_empty() {
+                    self.solution.time = self.time_keeper.elapsed_time();
+                    update_bound_if_better(&mut self.solution, dual_bound, model, self.quiet);
+                }
+            }
 
-                    continue;
-                } else {
-                    let cost = node.cost();
-                    self.solution.cost = Some(cost);
+            if let Some((cost, suffix)) =
+                get_solution_cost_and_suffix(model, &*node, self.suffix, &self.base_cost_evaluator)
+            {
+                if !exceed_bound(model, cost, self.primal_bound) {
                     self.primal_bound = Some(cost);
-                    self.solution.transitions = node.transitions();
-
-                    if let Some(best_bound) = self.solution.best_bound {
-                        self.solution.is_optimal = cost == best_bound;
-                    }
-
-                    self.solution.time = self.time_keeper.elapsed_time();
+                    let time = self.time_keeper.elapsed_time();
+                    update_solution(&mut self.solution, &*node, cost, suffix, time, self.quiet);
+                    self.time_keeper.stop();
 
                     return Ok((self.solution.clone(), self.solution.is_optimal));
-                }
-            }
+                } else if self.get_all_solutions {
+                    let mut solution = self.solution.clone();
+                    let time = self.time_keeper.elapsed_time();
+                    update_solution(&mut solution, &*node, cost, suffix, time, true);
+                    self.time_keeper.stop();
 
-            if self.time_keeper.check_time_limit() {
-                if !self.quiet {
-                    println!("Reached time limit.");
-                    println!("Expanded: {}", self.solution.expanded);
+                    return Ok((solution, false));
                 }
+                continue;
+            }
 
+            if self.time_keeper.check_time_limit(self.quiet) {
                 self.solution.time_out = true;
                 self.solution.time = self.time_keeper.elapsed_time();
+                self.time_keeper.stop();
 
                 return Ok((self.solution.clone(), true));
             }
 
             self.solution.expanded += 1;
 
-            let primal_bound = if self.f_pruning {
-                self.primal_bound
-            } else {
-                None
-            };
-
             for transition in self.generator.applicable_transitions(node.state()) {
-                let successor = node.generate_successor(
+                if let Some((successor, new_generated)) = (self.transition_evaluator)(
+                    &node,
                     transition,
                     &mut self.registry,
-                    &self.h_evaluator,
-                    &self.f_evaluator,
-                    primal_bound,
-                );
-
-                if let Some((successor, _, _, new_generated)) = successor {
+                    self.primal_bound,
+                ) {
                     self.open.push(successor);
 
                     if new_generated {
                         self.solution.generated += 1;
                     }
                 }
             }
         }
 
         self.solution.is_infeasible = self.solution.cost.is_none();
-        self.solution.is_optimal = self.is_optimal && self.solution.cost.is_some();
+        self.solution.is_optimal = self.solution.cost.is_some();
+        self.solution.best_bound = self.solution.cost;
         self.solution.time = self.time_keeper.elapsed_time();
+        self.time_keeper.stop();
         Ok((self.solution.clone(), true))
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/breadth_first_search.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cbfs.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,267 +1,287 @@
-use super::data_structure::state_registry::{StateInRegistry, StateInformation, StateRegistry};
-use super::data_structure::{
-    exceed_bound, SearchNode, SuccessorGenerator, TransitionChainInterface,
-};
-use super::search::{Search, Solution};
-use super::util;
-use super::util::ForwardSearchParameters;
-use dypdl::variable_type;
-use std::collections::VecDeque;
+use super::data_structure::{exceed_bound, BfsNode, StateRegistry};
+use super::rollout::get_solution_cost_and_suffix;
+use super::search::{Parameters, Search, SearchInput, Solution};
+use super::util::{print_dual_bound, update_solution, TimeKeeper};
+use super::SuccessorGenerator;
+use dypdl::{variable_type, Transition, TransitionInterface};
+use std::collections;
 use std::error::Error;
 use std::fmt;
-use std::mem;
 use std::rc::Rc;
 
-/// Breadth-first search solver.
+/// Cyclic Best-First Search (CBFS).
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 ///
-/// It uses `h_evaluator` and `f_evaluator` for pruning.
-/// If `h_evaluator` returns `None`, the state is pruned.
-/// If `f_pruning` and `f_evaluator` returns a value that exceeds the primal bound, the state is pruned.
-///
-/// Breadth-first searches layer by layer, where the i th layer contains states that can be reached with i transitions.
-/// By default, this solver only keeps states in the current layer to check for duplicates.
-/// If `keep_all_layers` is `true`, this solver keeps states in all layers to check for duplicates.
+/// It expands the best node from the current layer and then goes to the next layer.
+///
+/// Type parameter `N` is a node type that implements `BfsNode`.
+/// Type parameter `E` is a type of a function that evaluates a transition and insert a successor node into a state registry.
+/// The last argument of the function is the primal bound of the solution cost.
+/// Type parameter `B` is a type of a function that combines the g-value (the cost to a state) and the base cost.
+/// It should be the same function as the cost expression, e.g., `cost + base_cost` for `cost + w`.
+///
+/// # References
+///
+/// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
+/// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
+///
+/// Gio K. Kao, Edward C. Sewell, and Sheldom H. Jacobson. "A Branch, Bound and Remember Algorithm for the 1|r_i|Σt_i scheduling problem,"
+/// Journal of Scheduling, vol. 12(2), pp. 163-175, 2009.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{BreadthFirstSearch, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
-/// };
-/// use dypdl_heuristic_search::search_algorithm::util::{
-///     ForwardSearchParameters, Parameters,
+/// use dypdl_heuristic_search::{Parameters, Search};
+/// use dypdl_heuristic_search::search_algorithm::{
+///     Cbfs, FNode, SearchInput, SuccessorGenerator,
 /// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let h_evaluator = |_: &_, _: &_| Some(0);
-/// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-///
 /// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model(model.clone(), false);
-/// let parameters = ForwardSearchParameters {
+///
+/// let state = model.target.clone();
+/// let cost = 0;
+/// let h_evaluator = |_: &_| Some(0);
+/// let f_evaluator = |g, h, _: &_| g + h;
+/// let primal_bound = None;
+/// let node = FNode::generate_root_node(
+///     state,
+///     cost,
+///     &model,
+///     &h_evaluator,
+///     &f_evaluator,
+///     primal_bound,
+/// );
+/// let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+/// let input = SearchInput {
+///     node,
 ///     generator,
-///     parameters: Parameters::default(),
-///     initial_registry_capacity: None
+///     solution_suffix: &[],
 /// };
+/// let transition_evaluator =
+///     move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+///         node.insert_successor_node(
+///             transition,
+///             registry,
+///             &h_evaluator,
+///             &f_evaluator,
+///             primal_bound,
+///         )
+///     };
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let parameters = Parameters::default();
 ///
-/// let mut solver = BreadthFirstSearch::new(
-///     model, h_evaluator, f_evaluator, true, true, parameters
+/// let mut solver = Cbfs::<_, FNode<_>, _, _>::new(
+///     input, transition_evaluator, base_cost_evaluator, parameters,
 /// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub struct BreadthFirstSearch<T, H, F>
+pub struct Cbfs<'a, T, N, E, B, V = Transition>
 where
-    T: variable_type::Numeric + fmt::Display + Ord + 'static,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    generator: SuccessorGenerator,
-    h_evaluator: H,
-    f_evaluator: F,
-    f_pruning: bool,
-    keep_all_layers: bool,
+    generator: SuccessorGenerator<V>,
+    suffix: &'a [V],
+    transition_evaluator: E,
+    base_cost_evaluator: B,
     primal_bound: Option<T>,
     get_all_solutions: bool,
     quiet: bool,
-    open: VecDeque<Rc<SearchNode<T>>>,
-    next_open: VecDeque<Rc<SearchNode<T>>>,
-    registry: StateRegistry<T, SearchNode<T>>,
-    current_depth: usize,
-    time_keeper: util::TimeKeeper,
+    open: Vec<collections::BinaryHeap<Rc<N>>>,
+    registry: StateRegistry<T, N>,
+    time_keeper: TimeKeeper,
     solution: Solution<T>,
 }
 
-impl<T, H, F> BreadthFirstSearch<T, H, F>
+impl<'a, T, N, E, B, V> Cbfs<'a, T, N, E, B, V>
 where
-    T: variable_type::Numeric + fmt::Display + Ord + 'static,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    /// Create a new breadth-first search solver.
+    /// Create a new CBFS solver.
     pub fn new(
-        model: Rc<dypdl::Model>,
-        h_evaluator: H,
-        f_evaluator: F,
-        f_pruning: bool,
-        keep_all_layers: bool,
-        parameters: ForwardSearchParameters<T>,
-    ) -> BreadthFirstSearch<T, H, F> {
+        input: SearchInput<'a, N, V>,
+        transition_evaluator: E,
+        base_cost_evaluator: B,
+        parameters: Parameters<T>,
+    ) -> Cbfs<'a, T, N, E, B, V> {
         let time_keeper = parameters
-            .parameters
             .time_limit
-            .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
-        let get_all_solutions = parameters.parameters.get_all_solutions;
-        let primal_bound = parameters.parameters.primal_bound;
-        let quiet = parameters.parameters.quiet;
-        let mut open = VecDeque::new();
-        let next_open = VecDeque::new();
-        let mut registry = StateRegistry::new(model);
+            .map_or_else(TimeKeeper::default, TimeKeeper::with_time_limit);
+        let primal_bound = parameters.primal_bound;
+        let get_all_solutions = parameters.get_all_solutions;
+        let quiet = parameters.quiet;
+
+        let mut open = vec![collections::BinaryHeap::new()];
+        let mut registry = StateRegistry::<_, _>::new(input.generator.model.clone());
 
         if let Some(capacity) = parameters.initial_registry_capacity {
             registry.reserve(capacity);
         }
 
         let mut solution = Solution::default();
-        let node = SearchNode::generate_initial_node(&mut registry).unwrap();
-        open.push_back(node);
-        solution.generated += 1;
-
-        BreadthFirstSearch {
-            generator: parameters.generator,
-            h_evaluator,
-            f_evaluator,
-            f_pruning,
-            keep_all_layers,
+
+        if let Some(node) = input.node {
+            let (node, _) = registry.insert(node).unwrap();
+            solution.generated += 1;
+            solution.best_bound = node.bound(&input.generator.model);
+            open[0].push(node);
+
+            if !quiet {
+                solution.time = time_keeper.elapsed_time();
+                print_dual_bound(&solution);
+            }
+        } else {
+            solution.is_infeasible = true;
+        }
+
+        Cbfs {
+            generator: input.generator,
+            suffix: input.solution_suffix,
+            transition_evaluator,
+            base_cost_evaluator,
             primal_bound,
             get_all_solutions,
             quiet,
             open,
-            next_open,
             registry,
-            current_depth: 0,
             time_keeper,
             solution,
         }
     }
 }
 
-impl<T, H, F> Search<T> for BreadthFirstSearch<T, H, F>
+impl<'a, T, N, E, B, V> Search<T> for Cbfs<'a, T, N, E, B, V>
 where
-    T: variable_type::Numeric + fmt::Display + Ord + 'static,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
     fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
-        loop {
-            if self.open.is_empty() {
-                if !self.quiet {
-                    println!("Searched depth: {}", self.current_depth);
-                }
-
-                if self.next_open.is_empty() {
-                    break;
-                }
+        if self.solution.is_terminated() {
+            return Ok((self.solution.clone(), true));
+        }
 
-                mem::swap(&mut self.open, &mut self.next_open);
+        self.time_keeper.start();
+        let model = &self.generator.model;
+        let suffix = self.suffix;
+        let mut i = 0;
+        let mut no_node = true;
 
-                if !self.keep_all_layers {
-                    self.registry.clear();
-                }
-
-                self.current_depth += 1;
-            }
-
-            while let Some(node) = self.open.pop_front() {
-                if *node.closed.borrow() {
+        loop {
+            if let Some(node) = self.open[i].pop() {
+                if node.is_closed() {
                     continue;
                 }
+                node.close();
 
-                *node.closed.borrow_mut() = true;
-
-                if self.registry.model().is_base(node.state()) {
-                    if exceed_bound(self.registry.model(), node.cost(), self.primal_bound) {
-                        if self.get_all_solutions {
-                            let mut solution = self.solution.clone();
-                            solution.cost = Some(node.cost());
-                            solution.transitions = node
-                                .transitions
-                                .as_ref()
-                                .map_or_else(Vec::new, |transitions| transitions.transitions());
-                            solution.time = self.time_keeper.elapsed_time();
-
-                            return Ok((solution, false));
+                if let Some(dual_bound) = node.bound(model) {
+                    if exceed_bound(model, dual_bound, self.primal_bound) {
+                        if N::ordered_by_bound() {
+                            self.open[i].clear();
                         }
-
                         continue;
-                    } else {
-                        if !self.quiet {
-                            println!(
-                                "New primal bound: {}, expanded: {}",
-                                node.cost(),
-                                self.solution.expanded
-                            );
-                        }
+                    }
+                }
 
-                        let cost = node.cost();
-                        self.solution.cost = Some(cost);
-                        self.solution.transitions = node
-                            .transitions
-                            .as_ref()
-                            .map_or_else(Vec::new, |transitions| transitions.transitions());
+                if no_node {
+                    no_node = false;
+                }
+
+                if let Some((cost, suffix)) =
+                    get_solution_cost_and_suffix(model, &*node, suffix, &self.base_cost_evaluator)
+                {
+                    if !exceed_bound(model, cost, self.primal_bound) {
                         self.primal_bound = Some(cost);
-                        self.solution.time = self.time_keeper.elapsed_time();
+                        let time = self.time_keeper.elapsed_time();
+                        update_solution(&mut self.solution, &*node, cost, suffix, time, self.quiet);
+                        self.time_keeper.stop();
+
+                        return Ok((self.solution.clone(), self.solution.is_optimal));
+                    } else if self.get_all_solutions {
+                        let mut solution = self.solution.clone();
+                        let time = self.time_keeper.elapsed_time();
+                        update_solution(&mut solution, &*node, cost, suffix, time, true);
+                        self.time_keeper.stop();
 
-                        return Ok((self.solution.clone(), false));
+                        return Ok((solution, false));
                     }
+                    continue;
                 }
 
-                if self.time_keeper.check_time_limit() {
-                    if !self.quiet {
-                        println!("Expanded: {}", self.solution.expanded);
-                    }
-
+                if self.time_keeper.check_time_limit(self.quiet) {
                     self.solution.time_out = true;
                     self.solution.time = self.time_keeper.elapsed_time();
+                    self.time_keeper.stop();
 
                     return Ok((self.solution.clone(), true));
                 }
 
                 self.solution.expanded += 1;
 
                 for transition in self.generator.applicable_transitions(node.state()) {
-                    if let Some((successor, new_generated)) =
-                        node.generate_successor(transition, &mut self.registry, None)
-                    {
-                        if new_generated {
-                            self.solution.generated += 1;
+                    if let Some((successor, new_generated)) = (self.transition_evaluator)(
+                        &node,
+                        transition,
+                        &mut self.registry,
+                        self.primal_bound,
+                    ) {
+                        while i + 1 >= self.open.len() {
+                            self.open.push(collections::BinaryHeap::new());
                         }
 
-                        if let (true, Some(bound)) = (self.f_pruning, self.primal_bound) {
-                            if let Some(h) = (self.h_evaluator)(node.state(), self.registry.model())
-                            {
-                                let f = (self.f_evaluator)(
-                                    node.cost(),
-                                    h,
-                                    node.state(),
-                                    self.registry.model(),
-                                );
-
-                                if exceed_bound(self.registry.model(), f, Some(bound)) {
-                                    continue;
-                                }
-                            } else {
-                                continue;
-                            }
-                        }
+                        self.open[i + 1].push(successor);
 
-                        self.next_open.push_back(successor);
+                        if new_generated {
+                            self.solution.generated += 1;
+                        }
                     }
                 }
             }
+
+            if no_node && i + 1 == self.open.len() {
+                break;
+            } else if i + 1 == self.open.len() {
+                i = 0;
+                no_node = true;
+            } else {
+                i += 1;
+            }
         }
 
         self.solution.is_infeasible = self.solution.cost.is_none();
         self.solution.is_optimal = self.solution.cost.is_some();
+        self.solution.best_bound = self.solution.cost;
         self.solution.time = self.time_keeper.elapsed_time();
+        self.time_keeper.stop();
         Ok((self.solution.clone(), true))
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cabs.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dfbb.rs`

 * *Files 19% similar despite different names*

```diff
@@ -1,269 +1,259 @@
-use super::beam_search::{beam_search, BeamSearchParameters};
-use super::data_structure::beam::{BeamInterface, InformationInBeam};
-use super::data_structure::state_registry::StateInRegistry;
-use super::data_structure::{
-    BeamSearchProblemInstance, CustomCostNodeInterface, SuccessorGenerator,
-    TransitionWithCustomCost,
-};
-use super::search::{Search, Solution};
-use super::util;
-use dypdl::variable_type;
+use super::data_structure::{exceed_bound, BfsNode, StateRegistry, SuccessorGenerator};
+use super::rollout::get_solution_cost_and_suffix;
+use super::search::{Parameters, Search, SearchInput, Solution};
+use super::util::{self, print_dual_bound, update_solution};
+use dypdl::{variable_type, Transition, TransitionInterface};
 use std::error::Error;
 use std::fmt;
-use std::marker::PhantomData;
-use std::str;
+use std::rc::Rc;
 
-/// Complete Anytime Beam Search (CABS).
-///
-/// It iterates beam search with exponentially increasing beam width.
+/// Depth-First Branch-and-Bound which expands child nodes in the best-first order (DFBBBFS).
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 ///
-/// It uses `h_evaluator` and `f_evaluator` for pruning.
-/// If `h_evaluator` returns `None`, the state is pruned.
-/// If `parameters.f_pruning` and `f_evaluator` returns a value that exceeds the f bound, the state is pruned.
+/// It expands nodes in the depth-first order, but successor nodes are ordered by the best-first order.
 ///
-/// Beam search searches layer by layer, where the i th layer contains states that can be reached with i transitions.
-/// By default, this solver only keeps states in the current layer to check for duplicates.
-/// If `parameters.keep_all_layers` is `true`, this solver keeps states in all layers to check for duplicates.
+/// Type parameter `N` is a node type that implements `BfsNode`.
+/// Type parameter `E` is a type of a function that evaluates a transition and insert a successor node into a state registry.
+/// The last argument of the function is the primal bound of the solution cost.
+/// Type parameter `B` is a type of a function that combines the g-value (the cost to a state) and the base cost.
+/// It should be the same function as the cost expression, e.g., `cost + base_cost` for `cost + w`.
 ///
 /// # References
 ///
-/// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,""
+/// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
-/// Weixiong Zhang. "Complete Anytime Beam Search,"
-/// Proceedings of the 15th National Conference on Artificial Intelligence/Innovative Applications of Artificial Intelligence (AAAI/IAAI), pp. 425-430, 1998.
-///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::beam::Beam;
-/// use dypdl_heuristic_search::search_algorithm::{BeamSearchParameters, Cabs, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::BeamSearchNode;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
+/// use dypdl_heuristic_search::{Parameters, Search};
+/// use dypdl_heuristic_search::search_algorithm::{
+///     Dfbb, FNode, SearchInput, SuccessorGenerator,
 /// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let h_evaluator = |_: &_, _: &_| Some(0);
-/// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-///
 /// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model_without_custom_cost(model.clone(), false);
-/// let beam_constructor = |beam_size| Beam::<_, _, BeamSearchNode<_, _>>::new(beam_size);
-/// let parameters = BeamSearchParameters { beam_size: 1, ..Default::default() };
 ///
-/// let mut solver = Cabs::new(
-///     generator, h_evaluator, f_evaluator, beam_constructor, parameters
+/// let state = model.target.clone();
+/// let cost = 0;
+/// let h_evaluator = |_: &_| Some(0);
+/// let f_evaluator = |g, h, _: &_| g + h;
+/// let primal_bound = None;
+/// let node = FNode::generate_root_node(
+///     state,
+///     cost,
+///     &model,
+///     &h_evaluator,
+///     &f_evaluator,
+///     primal_bound,
+/// );
+/// let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+/// let input = SearchInput {
+///     node,
+///     generator,
+///     solution_suffix: &[],
+/// };
+/// let transition_evaluator =
+///     move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+///         node.insert_successor_node(
+///             transition,
+///             registry,
+///             &h_evaluator,
+///             &f_evaluator,
+///             primal_bound,
+///         )
+///     };
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let parameters = Parameters::default();
+///
+/// let mut solver = Dfbb::<_, FNode<_>, _, _>::new(
+///     input, transition_evaluator, base_cost_evaluator, parameters,
 /// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub struct Cabs<'a, T, I, B, C, H, F>
+pub struct Dfbb<'a, T, N, E, B, V = Transition>
 where
-    T: variable_type::Numeric + fmt::Display + Ord,
-    <T as str::FromStr>::Err: fmt::Debug,
-    I: InformationInBeam<T, T> + CustomCostNodeInterface<T, T>,
-    B: BeamInterface<T, T, I>,
-    C: Fn(usize) -> B,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    problem: BeamSearchProblemInstance<'a, T, T>,
-    h_evaluator: H,
-    f_evaluator: F,
-    beam_constructor: C,
-    maximize: bool,
-    f_pruning: bool,
-    keep_all_layers: bool,
+    generator: SuccessorGenerator<V>,
+    suffix: &'a [V],
+    transition_evaluator: E,
+    base_cost_evaluator: B,
     primal_bound: Option<T>,
+    get_all_solutions: bool,
     quiet: bool,
-    beam_size: usize,
+    open: Vec<Rc<N>>,
+    registry: StateRegistry<T, N>,
     time_keeper: util::TimeKeeper,
-    solution: Solution<T, TransitionWithCustomCost>,
-    phantom: PhantomData<I>,
+    solution: Solution<T>,
 }
 
-impl<'a, T, I, B, C, H, F> Cabs<'a, T, I, B, C, H, F>
+impl<'a, T, N, E, B, V> Dfbb<'a, T, N, E, B, V>
 where
-    T: variable_type::Numeric + fmt::Display + Ord,
-    <T as str::FromStr>::Err: fmt::Debug,
-    I: InformationInBeam<T, T> + CustomCostNodeInterface<T, T>,
-    B: BeamInterface<T, T, I>,
-    C: Fn(usize) -> B,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    /// Create a new CABS solver.
+    /// Create a new DFBB solver.
     pub fn new(
-        generator: SuccessorGenerator<TransitionWithCustomCost>,
-        h_evaluator: H,
-        f_evaluator: F,
-        beam_constructor: C,
-        parameters: BeamSearchParameters<T, T>,
-    ) -> Cabs<'a, T, I, B, C, H, F> {
-        let time_keeper = parameters
-            .parameters
+        input: SearchInput<'a, N, V>,
+        transition_evaluator: E,
+        base_cost_evaluator: B,
+        parameters: Parameters<T>,
+    ) -> Dfbb<'a, T, N, E, B, V> {
+        let mut time_keeper = parameters
             .time_limit
             .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
-        let target = StateInRegistry::from(generator.model.target.clone());
-        let problem = BeamSearchProblemInstance {
-            generator,
-            target,
-            cost: T::zero(),
-            g: T::zero(),
-            solution_suffix: &[],
-        };
-        Cabs {
-            problem,
-            h_evaluator,
-            f_evaluator,
-            beam_constructor,
-            maximize: parameters.maximize,
-            f_pruning: parameters.f_pruning,
-            keep_all_layers: parameters.keep_all_layers,
-            primal_bound: parameters.parameters.primal_bound,
-            quiet: parameters.parameters.quiet,
-            beam_size: parameters.beam_size,
-            time_keeper,
-            solution: Solution::default(),
-            phantom: PhantomData::default(),
+        let primal_bound = parameters.primal_bound;
+        let get_all_solutions = parameters.get_all_solutions;
+        let quiet = parameters.quiet;
+
+        let mut open = Vec::new();
+        let mut registry = StateRegistry::<_, _>::new(input.generator.model.clone());
+
+        if let Some(capacity) = parameters.initial_registry_capacity {
+            registry.reserve(capacity);
         }
-    }
 
-    //// Search for the next solution, returning the solution using `TransitionWithCustomCost`.
-    pub fn search_inner(&mut self) -> (Solution<T, TransitionWithCustomCost>, bool) {
-        while !self.solution.is_terminated() {
-            if !self.quiet {
-                println!(
-                    "Beam size: {}, expanded: {}",
-                    self.beam_size, self.solution.expanded
-                );
+        let mut solution = Solution::default();
+
+        if let Some(node) = input.node {
+            let (node, _) = registry.insert(node).unwrap();
+            solution.best_bound = node.bound(&input.generator.model);
+            open.push(node);
+            solution.generated += 1;
+
+            if !quiet {
+                solution.time = time_keeper.elapsed_time();
+                print_dual_bound(&solution);
             }
+        } else {
+            solution.is_infeasible = true;
+        }
 
-            let beam_constructor = |beam_size| (self.beam_constructor)(beam_size);
-            let parameters = BeamSearchParameters {
-                beam_size: self.beam_size,
-                maximize: self.maximize,
-                keep_all_layers: self.keep_all_layers,
-                f_pruning: self.f_pruning,
-                f_bound: self.primal_bound,
-                parameters: util::Parameters {
-                    primal_bound: self.primal_bound,
-                    get_all_solutions: false,
-                    quiet: true,
-                    time_limit: self.time_keeper.remaining_time_limit(),
-                },
-            };
-            let result = beam_search(
-                &self.problem,
-                &beam_constructor,
-                &self.h_evaluator,
-                &self.f_evaluator,
-                parameters,
-            );
-            self.solution.expanded += result.expanded;
-            self.solution.generated += result.generated;
-            self.beam_size *= 2;
-
-            match result.cost {
-                Some(new_cost) => {
-                    let found_better = self.solution.cost.map_or(true, |current_cost| {
-                        match self.problem.generator.model.reduce_function {
-                            dypdl::ReduceFunction::Max => new_cost > current_cost,
-                            dypdl::ReduceFunction::Min => new_cost < current_cost,
-                            _ => false,
-                        }
-                    });
-
-                    if found_better || result.is_optimal {
-                        self.solution.transitions = result.transitions;
-                        self.solution.cost = Some(new_cost);
-                        self.primal_bound = Some(new_cost);
-                        self.solution.is_optimal = result.is_optimal;
-                        self.solution.time = self.time_keeper.elapsed_time();
-
-                        if !self.quiet {
-                            println!(
-                                "New primal bound: {}, expanded: {}",
-                                new_cost, self.solution.expanded
-                            );
-                        }
+        time_keeper.stop();
 
-                        return (self.solution.clone(), result.is_optimal);
-                    }
-                }
-                _ => {
-                    if !self.quiet {
-                        println!("Failed to find a solution.");
-                    }
+        Dfbb {
+            generator: input.generator,
+            suffix: input.solution_suffix,
+            transition_evaluator,
+            base_cost_evaluator,
+            primal_bound,
+            get_all_solutions,
+            quiet,
+            open,
+            registry,
+            time_keeper,
+            solution,
+        }
+    }
+}
 
-                    if result.is_infeasible {
-                        self.solution.is_optimal = self.solution.cost.is_some();
-                        self.solution.is_infeasible = self.solution.cost.is_none();
-                        self.solution.time = self.time_keeper.elapsed_time();
-                    }
+impl<'a, T, N, E, B, V> Search<T> for Dfbb<'a, T, N, E, B, V>
+where
+    T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
+{
+    fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
+        self.time_keeper.start();
+        let model = &self.generator.model;
+
+        while let Some(node) = self.open.pop() {
+            if node.is_closed() {
+                continue;
+            }
+            node.close();
+
+            if let Some(dual_bound) = node.bound(model) {
+                if exceed_bound(model, dual_bound, self.primal_bound) {
+                    continue;
                 }
             }
 
-            if result.time_out {
-                if !self.quiet {
-                    println!("Reached time limit.");
+            if let Some((cost, suffix)) =
+                get_solution_cost_and_suffix(model, &*node, self.suffix, &self.base_cost_evaluator)
+            {
+                if !exceed_bound(model, cost, self.primal_bound) {
+                    self.primal_bound = Some(cost);
+                    let time = self.time_keeper.elapsed_time();
+                    update_solution(&mut self.solution, &*node, cost, suffix, time, self.quiet);
+                    self.time_keeper.stop();
+
+                    return Ok((self.solution.clone(), self.solution.is_optimal));
+                } else if self.get_all_solutions {
+                    let mut solution = self.solution.clone();
+                    let time = self.time_keeper.elapsed_time();
+                    update_solution(&mut solution, &*node, cost, suffix, time, true);
+                    self.time_keeper.stop();
+
+                    return Ok((solution, false));
                 }
+                continue;
+            }
 
-                self.solution.time = self.time_keeper.elapsed_time();
+            if self.time_keeper.check_time_limit(self.quiet) {
                 self.solution.time_out = true;
+                self.solution.time = self.time_keeper.elapsed_time();
+
+                return Ok((self.solution.clone(), true));
             }
-        }
 
-        (self.solution.clone(), true)
-    }
-}
+            self.solution.expanded += 1;
 
-impl<'a, T, I, B, C, H, F> Search<T> for Cabs<'a, T, I, B, C, H, F>
-where
-    T: variable_type::Numeric + fmt::Display + Ord,
-    <T as str::FromStr>::Err: fmt::Debug,
-    I: InformationInBeam<T, T> + CustomCostNodeInterface<T, T>,
-    B: BeamInterface<T, T, I>,
-    C: Fn(usize) -> B,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
-{
-    fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
-        let (solution, is_terminated) = self.search_inner();
-        let solution = Solution {
-            cost: solution.cost,
-            best_bound: solution.best_bound,
-            is_optimal: solution.is_optimal,
-            is_infeasible: solution.is_infeasible,
-            transitions: solution
-                .transitions
-                .into_iter()
-                .map(dypdl::Transition::from)
-                .collect(),
-            expanded: solution.expanded,
-            generated: solution.generated,
-            time: solution.time,
-            time_out: solution.time_out,
-        };
+            let mut successors = vec![];
+
+            for transition in self.generator.applicable_transitions(node.state()) {
+                if let Some((successor, new_generated)) = (self.transition_evaluator)(
+                    &node,
+                    transition,
+                    &mut self.registry,
+                    self.primal_bound,
+                ) {
+                    successors.push(successor);
+
+                    if new_generated {
+                        self.solution.generated += 1;
+                    }
+                }
+            }
+
+            successors.sort();
+            self.open.append(&mut successors);
+        }
 
-        Ok((solution, is_terminated))
+        self.solution.is_infeasible = self.solution.cost.is_none();
+        self.solution.is_optimal = self.solution.cost.is_some();
+        self.solution.best_bound = self.solution.cost;
+        self.solution.time = self.time_keeper.elapsed_time();
+        self.time_keeper.stop();
+        Ok((self.solution.clone(), true))
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/cbfs.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/apps.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,287 +1,346 @@
-use super::data_structure::state_registry::{StateInRegistry, StateRegistry};
-use super::data_structure::{exceed_bound, BfsNodeInterface, SuccessorGenerator};
-use super::search::{Search, Solution};
-use super::util;
-use dypdl::variable_type;
+use super::acps::ProgressiveSearchParameters;
+use super::data_structure::{exceed_bound, BfsNode, StateRegistry, SuccessorGenerator};
+use super::rollout::get_solution_cost_and_suffix;
+use super::util::{print_dual_bound, update_solution, TimeKeeper};
+use super::{Parameters, Search, SearchInput, Solution};
+use dypdl::{variable_type, Transition, TransitionInterface};
 use std::collections;
 use std::error::Error;
 use std::fmt;
 use std::rc::Rc;
 
-/// Cyclic Best-First Search (CBFS).
+/// Anytime Pack Progressive Search (APPS).
 ///
 /// This solver uses forward search based on the shortest path problem.
 /// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
 /// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
 ///
-/// It uses `h_evaluator` and `f_evaluator` for pruning.
-/// If `h_evaluator` returns `None`, the state is pruned.
-/// If `f_pruning` and `f_evaluator` returns a value that exceeds the primal bound, the state is pruned.
-///
-/// `ordered_by_f` indicates if the open list is ordered by the f-value.
+/// Type parameter `N` is a node type that implements `BfsNode`.
+/// Type parameter `E` is a type of a function that evaluates a transition and insert a successor node into a state registry.
+/// The last argument of the function is the primal bound of the solution cost.
+/// Type parameter `B` is a type of a function that combines the g-value (the cost to a state) and the base cost.
+/// It should be the same function as the cost expression, e.g., `cost + base_cost` for `cost + w`.
 ///
 /// # References
 ///
-/// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,""
+/// Ryo Kuroiwa and J. Christopher Beck. "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
-/// Gio K. Kao, Edward C. Sewell, and Sheldom H. Jacobson. "A Branch, Bound and Remember Algorithm for the 1|r_i|Σt_i scheduling problem,"
-/// Journal of Scheduling, vol. 12(2), pp. 163-175, 2009.
+/// Sataya Gautam Vadlamudi, Sandip Aine, Partha Pratim Chakrabarti. "Anytime Pack Search,"
+/// Natural Computing, vol. 15(3), pp. 395-414, 2016
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{Cbfs, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::FNode;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
-/// };
-/// use dypdl_heuristic_search::search_algorithm::util::{
-///     ForwardSearchParameters, Parameters,
+/// use dypdl_heuristic_search::{Parameters, ProgressiveSearchParameters, Search};
+/// use dypdl_heuristic_search::search_algorithm::{
+///     Apps, FNode, SearchInput, SuccessorGenerator,
 /// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let h_evaluator = |_: &_, _: &_| Some(0);
-/// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-///
 /// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model(model.clone(), false);
-/// let parameters = ForwardSearchParameters {
+///
+/// let state = model.target.clone();
+/// let cost = 0;
+/// let h_evaluator = |_: &_| Some(0);
+/// let f_evaluator = |g, h, _: &_| g + h;
+/// let primal_bound = None;
+/// let node = FNode::generate_root_node(
+///     state,
+///     cost,
+///     &model,
+///     &h_evaluator,
+///     &f_evaluator,
+///     primal_bound,
+/// );
+/// let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+/// let input = SearchInput {
+///     node,
 ///     generator,
-///     parameters: Parameters::default(),
-///     initial_registry_capacity: None
+///     solution_suffix: &[],
 /// };
-///
-/// let mut solver = Cbfs::<_, FNode<_>, _, _>::new(model, h_evaluator, f_evaluator, true, true, parameters);
+/// let transition_evaluator =
+///     move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+///         node.insert_successor_node(
+///             transition,
+///             registry,
+///             &h_evaluator,
+///             &f_evaluator,
+///             primal_bound,
+///         )
+///     };
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let parameters = Parameters::default();
+/// let progressive_parameters = ProgressiveSearchParameters::default();
+///
+/// let mut solver = Apps::<_, FNode<_>, _, _>::new(
+///     input, transition_evaluator, base_cost_evaluator, parameters, progressive_parameters,
+/// );
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub struct Cbfs<T, N, H, F>
+pub struct Apps<'a, T, N, E, B, V = Transition>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    generator: SuccessorGenerator,
-    h_evaluator: H,
-    f_evaluator: F,
-    f_pruning: bool,
-    ordered_by_f: bool,
+    generator: SuccessorGenerator<V>,
+    suffix: &'a [V],
+    transition_evaluator: E,
+    base_cost_evaluator: B,
+    progressive_parameters: ProgressiveSearchParameters,
     primal_bound: Option<T>,
     get_all_solutions: bool,
     quiet: bool,
-    open: Vec<collections::BinaryHeap<Rc<N>>>,
+    width: usize,
+    open: collections::BinaryHeap<Rc<N>>,
+    children: collections::BinaryHeap<Rc<N>>,
+    suspend: collections::BinaryHeap<Rc<N>>,
     registry: StateRegistry<T, N>,
-    time_keeper: util::TimeKeeper,
+    goal_found: bool,
+    time_keeper: TimeKeeper,
     solution: Solution<T>,
 }
 
-impl<T, N, H, F> Cbfs<T, N, H, F>
+impl<'a, T, N, E, B, V> Apps<'a, T, N, E, B, V>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    /// Create a new CBFS solver.
+    /// Creates a new APPS solver.
     pub fn new(
-        model: Rc<dypdl::Model>,
-        h_evaluator: H,
-        f_evaluator: F,
-        f_pruning: bool,
-        ordered_by_f: bool,
-        parameters: util::ForwardSearchParameters<T>,
-    ) -> Cbfs<T, N, H, F> {
+        input: SearchInput<'a, N, V>,
+        transition_evaluator: E,
+        base_cost_evaluator: B,
+        parameters: Parameters<T>,
+        progressive_parameters: ProgressiveSearchParameters,
+    ) -> Apps<'a, T, N, E, B, V> {
         let time_keeper = parameters
-            .parameters
             .time_limit
-            .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
-        let primal_bound = parameters.parameters.primal_bound;
-        let get_all_solutions = parameters.parameters.get_all_solutions;
-        let quiet = parameters.parameters.quiet;
-
-        let mut open = vec![collections::BinaryHeap::new()];
-        let mut registry = StateRegistry::new(model);
+            .map_or_else(TimeKeeper::default, TimeKeeper::with_time_limit);
+        let primal_bound = parameters.primal_bound;
+        let get_all_solutions = parameters.get_all_solutions;
+        let quiet = parameters.quiet;
+
+        let mut open = collections::BinaryHeap::new();
+        let children = collections::BinaryHeap::new();
+        let suspend = collections::BinaryHeap::new();
+        let mut registry = StateRegistry::<_, _>::new(input.generator.model.clone());
 
         if let Some(capacity) = parameters.initial_registry_capacity {
             registry.reserve(capacity);
         }
 
         let mut solution = Solution::default();
 
-        if let Some((node, h, f)) =
-            N::generate_initial_node(&mut registry, &h_evaluator, &f_evaluator)
-        {
-            open[0].push(node);
+        if let Some(node) = input.node {
+            let (node, _) = registry.insert(node).unwrap();
             solution.generated += 1;
+            solution.best_bound = node.bound(&input.generator.model);
+            open.push(node);
 
             if !quiet {
-                println!("Initial h = {}", h);
-            }
-
-            if f_pruning {
-                solution.best_bound = Some(f);
+                solution.time = time_keeper.elapsed_time();
+                print_dual_bound(&solution);
             }
         } else {
             solution.is_infeasible = true;
         }
 
-        Cbfs {
-            generator: parameters.generator,
-            h_evaluator,
-            f_evaluator,
-            f_pruning,
-            ordered_by_f,
+        Apps {
+            generator: input.generator,
+            suffix: input.solution_suffix,
+            transition_evaluator,
+            base_cost_evaluator,
+            progressive_parameters,
             primal_bound,
             get_all_solutions,
             quiet,
+            width: progressive_parameters.init,
             open,
+            children,
+            suspend,
             registry,
+            goal_found: false,
             time_keeper,
             solution,
         }
     }
 }
 
-impl<T, N, H, F> Search<T> for Cbfs<T, N, H, F>
+impl<'a, T, N, E, B, V> Search<T> for Apps<'a, T, N, E, B, V>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
-    N: BfsNodeInterface<T>,
-    H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-    F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
     fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
-        let mut i = 0;
-        let mut no_node = true;
+        if self.solution.is_terminated() {
+            return Ok((self.solution.clone(), true));
+        }
 
-        loop {
-            if let Some(node) = self.open[i].pop() {
-                if node.closed() {
-                    continue;
+        self.time_keeper.start();
+        let model = &self.generator.model;
+        let suffix = self.suffix;
+
+        while !self.open.is_empty() || !self.children.is_empty() || !self.suspend.is_empty() {
+            if self.open.is_empty() {
+                while self.open.len() < self.width {
+                    if let Some(node) = self.children.pop() {
+                        if node.is_closed() {
+                            continue;
+                        }
+                        if let Some(bound) = node.bound(model) {
+                            if exceed_bound(model, bound, self.primal_bound) {
+                                if N::ordered_by_bound() {
+                                    self.children.clear();
+                                }
+                                continue;
+                            }
+                        }
+                        self.open.push(node);
+                    } else {
+                        break;
+                    }
                 }
 
-                node.close();
-
-                let f = node.get_bound(self.registry.model());
-
-                if self.f_pruning
-                    && self.ordered_by_f
-                    && exceed_bound(self.registry.model(), f, self.primal_bound)
-                {
-                    self.open[i].clear();
-                } else {
-                    if no_node {
-                        no_node = false;
+                while let Some(node) = self.children.pop() {
+                    if node.is_closed() {
+                        continue;
                     }
-
-                    if self.registry.model().is_base(node.state()) {
-                        if exceed_bound(self.registry.model(), node.cost(), self.primal_bound) {
-                            if self.get_all_solutions {
-                                let mut solution = self.solution.clone();
-                                solution.cost = Some(node.cost());
-                                solution.transitions = node.transitions();
-                                solution.time = self.time_keeper.elapsed_time();
-
-                                return Ok((solution, false));
+                    if let Some(bound) = node.bound(model) {
+                        if exceed_bound(model, bound, self.primal_bound) {
+                            if N::ordered_by_bound() {
+                                self.children.clear();
                             }
-
                             continue;
-                        } else {
-                            if !self.quiet {
-                                println!(
-                                    "New primal bound: {}, expanded: {}",
-                                    node.cost(),
-                                    self.solution.expanded
-                                );
-                            }
+                        }
+                    }
+                    self.suspend.push(node);
+                }
 
-                            let cost = node.cost();
-                            self.solution.cost = Some(cost);
-                            self.solution.time = self.time_keeper.elapsed_time();
-                            self.solution.transitions = node.transitions();
-                            self.primal_bound = Some(cost);
+                // Run out current candidates
+                if self.open.is_empty() {
+                    if self.progressive_parameters.reset && self.goal_found {
+                        self.width = self.progressive_parameters.init;
+                    } else {
+                        self.width = self.progressive_parameters.increase_width(self.width);
+                    }
 
-                            if let Some(bound) = self.solution.best_bound {
-                                self.solution.is_optimal = cost == bound;
+                    while self.open.len() < self.width {
+                        if let Some(node) = self.suspend.pop() {
+                            if node.is_closed() {
+                                continue;
                             }
-
-                            self.solution.time = self.time_keeper.elapsed_time();
-
-                            return Ok((self.solution.clone(), self.solution.is_optimal));
+                            if let Some(bound) = node.bound(model) {
+                                if exceed_bound(model, bound, self.primal_bound) {
+                                    if N::ordered_by_bound() {
+                                        self.suspend.clear();
+                                    }
+                                    continue;
+                                }
+                            }
+                            self.open.push(node);
+                        } else {
+                            break;
                         }
                     }
 
-                    if self.time_keeper.check_time_limit() {
-                        if !self.quiet {
-                            println!("Reached time limit.");
-                            println!("Expanded: {}", self.solution.expanded);
+                    self.goal_found = false;
+                }
+            }
+
+            while let Some(node) = self.open.pop() {
+                if node.is_closed() {
+                    continue;
+                }
+                node.close();
+
+                if let Some(dual_bound) = node.bound(model) {
+                    if exceed_bound(model, dual_bound, self.primal_bound) {
+                        if N::ordered_by_bound() {
+                            self.open.clear();
                         }
+                        continue;
+                    }
+                }
 
-                        self.solution.time_out = true;
-                        self.solution.time = self.time_keeper.elapsed_time();
+                if let Some((cost, suffix)) =
+                    get_solution_cost_and_suffix(model, &*node, suffix, &self.base_cost_evaluator)
+                {
+                    if !exceed_bound(model, cost, self.primal_bound) {
+                        self.primal_bound = Some(cost);
+                        let time = self.time_keeper.elapsed_time();
+                        update_solution(&mut self.solution, &*node, cost, suffix, time, self.quiet);
+                        self.time_keeper.stop();
+
+                        return Ok((self.solution.clone(), self.solution.is_optimal));
+                    } else if self.get_all_solutions {
+                        let mut solution = self.solution.clone();
+                        let time = self.time_keeper.elapsed_time();
+                        update_solution(&mut solution, &*node, cost, suffix, time, true);
+                        self.time_keeper.stop();
 
-                        return Ok((self.solution.clone(), true));
+                        return Ok((solution, false));
                     }
+                    continue;
+                }
 
-                    self.solution.expanded += 1;
+                if self.time_keeper.check_time_limit(self.quiet) {
+                    self.solution.time_out = true;
+                    self.solution.time = self.time_keeper.elapsed_time();
+                    self.time_keeper.stop();
 
-                    let primal_bound = if self.f_pruning {
-                        self.primal_bound
-                    } else {
-                        None
-                    };
+                    return Ok((self.solution.clone(), true));
+                }
 
-                    for transition in self.generator.applicable_transitions(node.state()) {
-                        let successor = node.generate_successor(
-                            transition,
-                            &mut self.registry,
-                            &self.h_evaluator,
-                            &self.f_evaluator,
-                            primal_bound,
-                        );
-
-                        if let Some((successor, _, _, new_generated)) = successor {
-                            while i + 1 >= self.open.len() {
-                                self.open.push(collections::BinaryHeap::new());
-                            }
+                self.solution.expanded += 1;
 
-                            self.open[i + 1].push(successor);
+                for transition in self.generator.applicable_transitions(node.state()) {
+                    if let Some((successor, new_generated)) = (self.transition_evaluator)(
+                        &node,
+                        transition,
+                        &mut self.registry,
+                        self.primal_bound,
+                    ) {
+                        self.children.push(successor);
 
-                            if new_generated {
-                                self.solution.generated += 1;
-                            }
+                        if new_generated {
+                            self.solution.generated += 1;
                         }
                     }
                 }
             }
-
-            if no_node && i + 1 == self.open.len() {
-                break;
-            } else if i + 1 == self.open.len() {
-                i = 0;
-                no_node = true;
-            } else {
-                i += 1;
-            }
         }
 
         self.solution.is_infeasible = self.solution.cost.is_none();
         self.solution.is_optimal = self.solution.cost.is_some();
+        self.solution.best_bound = self.solution.cost;
         self.solution.time = self.time_keeper.elapsed_time();
+        self.time_keeper.stop();
         Ok((self.solution.clone(), true))
     }
 }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/beam.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,308 +1,239 @@
 //! A module for beam.
 
 use super::hashable_state::HashableSignatureVariables;
-use super::prioritized_node::PrioritizedNode;
 use super::state_registry::{StateInRegistry, StateInformation, StateRegistry};
 use core::ops::Deref;
 use dypdl::variable_type::Numeric;
+use dypdl::StateInterface;
+use std::cmp::Reverse;
 use std::collections;
 use std::fmt::Debug;
 use std::hash::Hash;
-use std::marker::PhantomData;
 use std::rc::Rc;
 
-/// State information in beam.
-pub trait InformationInBeam<T, U, K = Rc<HashableSignatureVariables>>:
-    Ord + StateInformation<T, K> + PrioritizedNode<U> + InBeam
+/// An draining iterator for `Beam`
+pub struct BeamDrain<'a, T, I, V = Rc<I>, K = Rc<HashableSignatureVariables>>
 where
     T: Numeric,
-    U: Numeric,
+    I: StateInformation<T, K>,
     K: Hash + Eq + Clone + Debug,
+    V: Ord + Deref<Target = I>,
 {
+    queue_iter: collections::binary_heap::Drain<'a, Reverse<V>>,
+    phantom: std::marker::PhantomData<(T, I, K)>,
 }
 
-/// Trait to check if it is included in the beam.
-pub trait InBeam {
-    /// Returns if it is included in the beam.
-    fn in_beam(&self) -> bool;
-
-    /// Remove it from the beam.
-    fn remove_from_beam(&self);
-}
-
-/// An draining iterator for `Beam`
-pub struct BeamDrain<'a, I: InBeam, V: Ord + Deref<Target = I>> {
-    queue_iter: collections::binary_heap::Drain<'a, V>,
-}
-
-impl<'a, I: InBeam, V: Ord + Deref<Target = I>> Iterator for BeamDrain<'a, I, V> {
-    type Item = V;
-
-    fn next(&mut self) -> Option<Self::Item> {
-        match self.queue_iter.next() {
-            Some(node) if !node.in_beam() => self.next(),
-            node => node,
-        }
-    }
-}
-
-/// Trait representing beam.
-///
-/// It keeps the best `capacity` nodes according to some criteria based on the f- and g-values.
-pub trait BeamInterface<
-    T,
-    U,
-    I,
-    V = Rc<I>,
-    K = Rc<HashableSignatureVariables>,
-    R = Rc<dypdl::Model>,
-> where
+impl<'a, T, I, V, K> Iterator for BeamDrain<'a, T, I, V, K>
+where
     T: Numeric,
-    U: Numeric,
-    I: InformationInBeam<T, U, K>,
-    V: Deref<Target = I> + From<I> + Clone + Ord,
+    I: StateInformation<T, K>,
     K: Hash + Eq + Clone + Debug,
-    R: Deref<Target = dypdl::Model>,
+    V: Ord + Deref<Target = I>,
 {
-    /// Returns true if no state in beam and false otherwise.
-    fn is_empty(&self) -> bool;
-
-    /// Returns the capacity of the beam.
-    fn capacity(&self) -> usize;
-
-    /// Removes nodes from the beam, returning all removed nodes as an iterator.
-    fn drain(&mut self) -> BeamDrain<'_, I, V>;
-
-    /// Insert a node if it is not dominated  and its f-value is sufficient.
-    ///
-    /// The first returned value represents if a new search node (not an update version of an existing node) is generated.
-    /// The second returned value represents if the pruning due to the beam size happened.
-    fn insert<F>(
-        &mut self,
-        registry: &mut StateRegistry<T, I, V, K, R>,
-        state: StateInRegistry<K>,
-        cost: T,
-        g: U,
-        f: U,
-        constructor: F,
-    ) -> (bool, bool)
-    where
-        F: FnOnce(StateInRegistry<K>, T, Option<&I>) -> Option<I>;
-}
-
-/// Common structure of beam.
-#[derive(Debug, Clone)]
-pub struct BeamBase<I: InBeam, V: Ord + Deref<Target = I>> {
-    /// Priority queue to store nodes.
-    pub queue: collections::BinaryHeap<V>,
-}
+    type Item = V;
 
-impl<I: InBeam, V: Ord + Deref<Target = I>> BeamBase<I, V> {
-    /// Removes nodes from the beam, returning all removed nodes as an iterator.
-    #[inline]
-    pub fn drain(&mut self) -> BeamDrain<'_, I, V> {
-        BeamDrain {
-            queue_iter: self.queue.drain(),
+    fn next(&mut self) -> Option<Self::Item> {
+        match self.queue_iter.next() {
+            Some(node) if node.0.is_closed() => self.next(),
+            node => node.map(|node| node.0),
         }
     }
 }
 
 /// Beam for beam search.
 ///
-/// It only keeps the best `capacity` nodes that minimizes the f-value.
-/// If the f-values are the same, it prefers a node with a larger g-value.
+/// It only keeps the best `capacity` nodes that maximizes the f-value and h-value.
+/// Nodes must be ordered by f-values and h-values, implementing Ord trait.
+/// If you want to keep the best nodes that minimizes the f- and h-value, use negative values.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::BeamSearchNode;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::state_registry::*;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::beam::*;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::CustomCostNodeInterface;
+/// use dypdl_heuristic_search::search_algorithm::{
+///     FNode, StateInRegistry, StateRegistry,
+/// };
+/// use dypdl_heuristic_search::search_algorithm::data_structure::{
+///     Beam, GetTransitions, StateInformation,
+/// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let signature = model.add_integer_variable("signature", 1).unwrap();
 /// let resource = model.add_integer_resource_variable("resource", false, 1).unwrap();
-/// let parent = StateInRegistry::<Rc<_>>::from(model.target.clone());
-/// let parent_cost = 0;
 ///
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 2);
 /// increment.add_effect(signature, signature + 1).unwrap();
+/// let increment = Rc::new(increment);
 ///
 /// let mut decrement = Transition::new("decrement");
 /// decrement.set_cost(IntegerExpression::Cost + 3);
 /// decrement.add_effect(signature, signature - 1).unwrap();
+/// let decrement = Rc::new(decrement);
 ///
 /// let mut produce = Transition::new("produce");
 /// produce.set_cost(IntegerExpression::Cost + 1);
 /// produce.add_effect(signature, signature + 1).unwrap();
 /// produce.add_effect(resource, resource + 1).unwrap();
+/// let produce = Rc::new(produce);
 ///
 /// let model = Rc::new(model);
-/// let mut registry = StateRegistry::<_, BeamSearchNode<_, _>>::new(model.clone());
-/// let constructor = |state, cost, _: Option<&_>| {
-///     Some(BeamSearchNode::new(cost, cost, state, cost, None, None))
-/// };
+/// let mut registry = StateRegistry::new(model.clone());
+///
+/// let h_evaluator = |_: &StateInRegistry| Some(0);
+/// let f_evaluator = |g, h, _: &StateInRegistry| g + h;
+/// let node = FNode::generate_root_node(
+///     model.target.clone(), 0, &model, &h_evaluator, &f_evaluator, None,
+/// ).unwrap();
 ///
 /// let mut beam = Beam::new(1);
-/// assert!(BeamInterface::<_, _, _>::is_empty(&beam));
-/// assert_eq!(BeamInterface::<_, _, _>::capacity(&beam), 1);
+/// assert!(beam.is_empty());
+/// assert_eq!(beam.capacity(), 1);
 ///
-/// let state: StateInRegistry = increment.apply(&parent, &model.table_registry);
-/// let cost = increment.eval_cost(parent_cost, &parent, &model.table_registry);
-/// let (generated, pruned) = beam.insert(&mut registry, state, cost, cost, cost, constructor);
+/// let successor = node.generate_successor_node(
+///     increment, &model, &h_evaluator, &f_evaluator, None,
+/// ).unwrap();
+/// let (generated, pruned) = beam.insert(&mut registry, successor);
 /// assert!(generated);
 /// assert!(!pruned);
 ///
-/// let state: StateInRegistry = decrement.apply(&parent, &model.table_registry);
-/// let cost = increment.eval_cost(parent_cost, &parent, &model.table_registry);
-/// let (generated, pruned) = beam.insert(&mut registry, state, cost, cost, cost, constructor);
+/// let successor = node.generate_successor_node(
+///     decrement, &model, &h_evaluator, &f_evaluator, None,
+/// ).unwrap();
+/// let (generated, pruned) = beam.insert(&mut registry, successor);
 /// assert!(!generated);
 /// assert!(pruned);
 ///
-/// let state: StateInRegistry = produce.apply(&parent, &model.table_registry);
-/// let cost = produce.eval_cost(parent_cost, &parent, &model.table_registry);
-/// let (generated, pruned) = beam.insert(&mut registry, state.clone(), cost, cost, cost, constructor);
+/// let successor = node.generate_successor_node(
+///     produce.clone(), &model, &h_evaluator, &f_evaluator, None,
+/// ).unwrap();
+/// let state = successor.state().clone();
+/// let (generated, pruned) = beam.insert(&mut registry, successor);
 /// assert!(!generated);
 /// assert!(!pruned);
 ///
-/// let expected = Rc::new(BeamSearchNode { g: cost, f: cost, state, cost, ..Default::default() });
-/// let mut iter = BeamInterface::<_, _, _>::drain(&mut beam);
-/// let node = iter.next().unwrap();
-/// assert_eq!(node.g, expected.g);
-/// assert_eq!(node.f, expected.f);
-/// assert_eq!(node.state, expected.state);
-/// assert_eq!(node.cost, expected.cost);
+/// let mut iter = beam.drain();
+/// let node: Rc<FNode<_>> = iter.next().unwrap();
+/// assert_eq!(node.state(), &state);
+/// assert_eq!(node.cost(&model), 1);
+/// assert_eq!(node.bound(&model), Some(1));
+/// assert_eq!(node.transitions(), vec![(*produce).clone()]);
 /// assert_eq!(iter.next(), None);
 /// ```
 #[derive(Debug, Clone)]
-pub struct Beam<T, U, I, V = Rc<I>, K = Rc<HashableSignatureVariables>>
+pub struct Beam<T, I, V = Rc<I>, K = Rc<HashableSignatureVariables>>
 where
     T: Numeric,
-    U: Numeric + Ord,
-    I: InformationInBeam<T, U, K>,
+    I: StateInformation<T, K>,
     V: Deref<Target = I> + From<I> + Clone + Ord,
     K: Hash + Eq + Clone + Debug,
 {
     /// Capacity of the beam, or the beam size.
     pub capacity: usize,
     size: usize,
-    beam: BeamBase<I, V>,
-    phantom: PhantomData<(T, U, K)>,
+    queue: collections::BinaryHeap<Reverse<V>>,
+    phantom: std::marker::PhantomData<(T, I, K)>,
 }
 
-impl<T, U, I, V, K> Beam<T, U, I, V, K>
+impl<T, I, V, K> Beam<T, I, V, K>
 where
     T: Numeric,
-    U: Numeric + Ord,
-    I: InformationInBeam<T, U, K>,
+    I: StateInformation<T, K> + Ord,
     V: Deref<Target = I> + From<I> + Clone + Ord,
     K: Hash + Eq + Clone + Debug,
 {
     /// Creates a new beam with a given capacity.
     #[inline]
-    pub fn new(capacity: usize) -> Beam<T, U, I, V, K> {
+    pub fn new(capacity: usize) -> Beam<T, I, V, K> {
         Beam {
             capacity,
             size: 0,
-            beam: BeamBase {
-                queue: collections::BinaryHeap::with_capacity(capacity),
-            },
-            phantom: PhantomData::default(),
+            queue: collections::BinaryHeap::with_capacity(capacity),
+            phantom: std::marker::PhantomData,
         }
     }
 
     /// Removes a node having the lowest priority from the beam.
     pub fn pop(&mut self) -> Option<V> {
-        self.beam.queue.pop().map(|node| {
-            node.remove_from_beam();
+        self.queue.pop().map(|node| {
+            node.0.close();
             self.size -= 1;
             self.clean_garbage();
-            node
+            node.0
         })
     }
 
     fn clean_garbage(&mut self) {
-        let mut peek = self.beam.queue.peek();
+        let mut peek = self.queue.peek();
 
-        while peek.map_or(false, |node| !node.in_beam()) {
-            self.beam.queue.pop();
-            peek = self.beam.queue.peek();
+        while peek.map_or(false, |node| node.0.is_closed()) {
+            self.queue.pop();
+            peek = self.queue.peek();
         }
     }
-}
 
-impl<T, U, I, V, K, R> BeamInterface<T, U, I, V, K, R> for Beam<T, U, I, V, K>
-where
-    T: Numeric,
-    U: Numeric + Ord,
-    I: InformationInBeam<T, U, K>,
-    V: Deref<Target = I> + From<I> + Clone + Ord,
-    K: Hash + Eq + Clone + Debug,
-    R: Deref<Target = dypdl::Model>,
-    StateInRegistry<K>: dypdl::StateInterface,
-{
+    /// Returns true if no state in beam and false otherwise.
     #[inline]
-    fn is_empty(&self) -> bool {
+    pub fn is_empty(&self) -> bool {
         self.size == 0
     }
 
+    /// Returns the capacity of the beam.
     #[inline]
-    fn capacity(&self) -> usize {
+    pub fn capacity(&self) -> usize {
         self.capacity
     }
 
+    /// Removes nodes from the beam, returning all removed nodes as an iterator.
     #[inline]
-    fn drain(&mut self) -> BeamDrain<'_, I, V> {
+    pub fn drain(&mut self) -> BeamDrain<'_, T, I, V, K> {
         self.size = 0;
-        self.beam.drain()
+        BeamDrain {
+            queue_iter: self.queue.drain(),
+            phantom: std::marker::PhantomData,
+        }
     }
 
-    fn insert<F>(
+    /// Insert a node if it is not dominated and its h- and f-value are sufficiently large to be top `capacity` nodes.
+    ///
+    /// The first returned value represents if a new search node (not an update version of an existing node) is generated.
+    /// The second returned value represents if the pruning due to the beam size happened.
+    pub fn insert<R>(
         &mut self,
         registry: &mut StateRegistry<T, I, V, K, R>,
-        state: StateInRegistry<K>,
-        cost: T,
-        g: U,
-        f: U,
-        constructor: F,
+        node: I,
     ) -> (bool, bool)
     where
-        F: FnOnce(StateInRegistry<K>, T, Option<&I>) -> Option<I>,
+        R: Deref<Target = dypdl::Model>,
+        StateInRegistry<K>: StateInterface,
     {
-        if self.size < self.capacity
-            || self.beam.queue.peek().map_or(true, |node| {
-                (f < node.f()) || (f == node.f() && g > node.g())
-            })
-        {
+        if self.size < self.capacity || self.queue.peek().map_or(true, |peek| node > *peek.0) {
             let mut generated = false;
             let mut beam_pruning = false;
 
-            if let Some((node, dominated)) = registry.insert(state, cost, constructor) {
+            if let Some((node, dominated)) = registry.insert(node) {
                 if let Some(dominated) = dominated {
-                    if dominated.in_beam() {
-                        dominated.remove_from_beam();
+                    if !dominated.is_closed() {
+                        dominated.close();
                         self.size -= 1;
                         self.clean_garbage();
                     }
                 } else {
                     generated = true;
                 }
 
                 if self.size == self.capacity {
                     self.pop();
                     beam_pruning = true;
                 }
 
                 if self.size < self.capacity {
-                    self.beam.queue.push(node);
+                    self.queue.push(Reverse(node));
                     self.size += 1;
                 }
             }
 
             (generated, beam_pruning)
         } else {
             (false, true)
@@ -310,207 +241,192 @@
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::super::hashable_state::HashableSignatureVariables;
     use super::*;
-    use std::cell::RefCell;
+    use dypdl::Model;
+    use std::cell::Cell;
     use std::cmp::Ordering;
 
     #[derive(Debug)]
     struct MockInBeam {
         state: StateInRegistry,
         cost: i32,
-        g: i32,
+        h: i32,
         f: i32,
-        in_beam: RefCell<bool>,
+        closed: Cell<bool>,
     }
 
     impl StateInformation<i32> for MockInBeam {
         fn state(&self) -> &StateInRegistry {
             &self.state
         }
 
-        fn cost(&self) -> i32 {
+        fn state_mut(&mut self) -> &mut StateInRegistry {
+            &mut self.state
+        }
+
+        fn cost(&self, _: &Model) -> i32 {
             self.cost
         }
+
+        fn bound(&self, _: &Model) -> Option<i32> {
+            Some(self.f)
+        }
+
+        fn is_closed(&self) -> bool {
+            self.closed.get()
+        }
+
+        fn close(&self) {
+            self.closed.set(true);
+        }
     }
 
     impl PartialEq for MockInBeam {
         #[inline]
         fn eq(&self, other: &Self) -> bool {
-            self.f == other.f && self.g == other.g
+            self.f == other.f && self.h == other.h
         }
     }
 
     impl Eq for MockInBeam {}
 
     impl Ord for MockInBeam {
         fn cmp(&self, other: &Self) -> Ordering {
             match self.f.cmp(&other.f) {
-                Ordering::Equal => other.g.cmp(&self.g),
+                Ordering::Equal => self.h.cmp(&other.h),
                 result => result,
             }
         }
     }
 
     impl PartialOrd for MockInBeam {
         fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
             Some(self.cmp(other))
         }
     }
 
-    impl PrioritizedNode<i32> for MockInBeam {
-        fn g(&self) -> i32 {
-            self.g
-        }
-
-        fn f(&self) -> i32 {
-            self.f
-        }
-    }
-
-    impl InBeam for MockInBeam {
-        fn in_beam(&self) -> bool {
-            *self.in_beam.borrow()
-        }
-
-        fn remove_from_beam(&self) {
-            *self.in_beam.borrow_mut() = false;
-        }
-    }
-
-    impl InformationInBeam<i32, i32> for MockInBeam {}
-
     #[test]
     fn normal_beam_capacity() {
         let model = Rc::new(dypdl::Model::default());
         let mut registry = StateRegistry::new(model);
-        let mut beam = Beam::<i32, i32, MockInBeam>::new(2);
-        assert_eq!(BeamInterface::<i32, i32, MockInBeam>::capacity(&beam), 2);
+        let mut beam = Beam::<_, _>::new(2);
+        assert_eq!(beam.capacity(), 2);
         let state = StateInRegistry::default();
         let cost = 0;
-        let g = 0;
-        let f = 1;
-        let constructor = |state, cost, _: Option<&_>| {
-            Some(MockInBeam {
-                state,
-                cost,
-                g,
-                f,
-                in_beam: RefCell::new(true),
-            })
+        let h = -1;
+        let f = -1;
+        let node = MockInBeam {
+            state,
+            cost,
+            h,
+            f,
+            closed: Cell::new(false),
         };
-        let (generated, beam_pruning) = beam.insert(&mut registry, state, cost, g, f, constructor);
+        let (generated, beam_pruning) = beam.insert(&mut registry, node);
         assert!(generated);
         assert!(!beam_pruning);
-        assert_eq!(BeamInterface::<i32, i32, MockInBeam>::capacity(&beam), 2);
+        assert_eq!(beam.capacity(), 2);
     }
 
     #[test]
     fn normal_beam_is_empty() {
         let model = Rc::new(dypdl::Model::default());
         let mut registry = StateRegistry::new(model);
-        let mut beam = Beam::<i32, i32, MockInBeam>::new(2);
-        assert!(BeamInterface::<i32, i32, MockInBeam>::is_empty(&beam));
+        let mut beam = Beam::<_, _, Rc<_>>::new(2);
+        assert!(beam.is_empty());
         let state = StateInRegistry::default();
         let cost = 0;
-        let g = 0;
-        let f = 1;
-        let constructor = |state, cost, _: Option<&_>| {
-            Some(MockInBeam {
-                state,
-                cost,
-                g,
-                f,
-                in_beam: RefCell::new(true),
-            })
+        let h = -1;
+        let f = -1;
+        let node = MockInBeam {
+            state,
+            cost,
+            h,
+            f,
+            closed: Cell::new(false),
         };
-        let (generated, beam_pruning) = beam.insert(&mut registry, state, cost, g, f, constructor);
+        let (generated, beam_pruning) = beam.insert(&mut registry, node);
         assert!(generated);
         assert!(!beam_pruning);
-        assert!(!BeamInterface::<i32, i32, MockInBeam>::is_empty(&beam));
+        assert!(!beam.is_empty());
     }
 
     #[test]
     fn normal_beam_pop() {
         let model = Rc::new(dypdl::Model::default());
-        let mut registry = StateRegistry::<i32, MockInBeam>::new(model);
+        let mut registry = StateRegistry::<i32, MockInBeam>::new(model.clone());
         let mut beam = Beam::new(1);
 
         let peek = beam.pop();
         assert_eq!(peek, None);
 
         let state = StateInRegistry {
             signature_variables: Rc::new(HashableSignatureVariables {
                 integer_variables: vec![1, 2, 3],
                 ..Default::default()
             }),
             ..Default::default()
         };
         let cost = 1;
-        let g = 0;
-        let f = 2;
-        let constructor = |state, cost, _: Option<&_>| {
-            Some(MockInBeam {
-                state,
-                cost,
-                g,
-                f,
-                in_beam: RefCell::new(true),
-            })
+        let h = -1;
+        let f = -2;
+        let node = MockInBeam {
+            state,
+            cost,
+            h,
+            f,
+            closed: Cell::new(false),
         };
-        let (generated, beam_pruning) = beam.insert(&mut registry, state, cost, g, f, constructor);
+        let (generated, beam_pruning) = beam.insert(&mut registry, node);
         assert!(generated);
         assert!(!beam_pruning);
 
         let state = StateInRegistry {
             signature_variables: Rc::new(HashableSignatureVariables {
                 integer_variables: vec![1, 2, 3],
                 ..Default::default()
             }),
             ..Default::default()
         };
         let cost = 0;
-        let g = 0;
-        let f = 1;
-        let constructor = |state, cost, _: Option<&_>| {
-            Some(MockInBeam {
-                state,
-                cost,
-                g,
-                f,
-                in_beam: RefCell::new(true),
-            })
+        let h = -1;
+        let f = -1;
+        let node = MockInBeam {
+            state,
+            cost,
+            h,
+            f,
+            closed: Cell::new(false),
         };
-        let (generated, beam_pruning) = beam.insert(&mut registry, state, cost, g, f, constructor);
+        let (generated, beam_pruning) = beam.insert(&mut registry, node);
         assert!(!generated);
         assert!(!beam_pruning);
 
         let state = StateInRegistry {
             signature_variables: Rc::new(HashableSignatureVariables {
                 integer_variables: vec![2, 3, 4],
                 ..Default::default()
             }),
             ..Default::default()
         };
         let cost = 0;
-        let g = 0;
-        let f = 2;
-        let constructor = |state, cost, _: Option<&_>| {
-            Some(MockInBeam {
-                state,
-                cost,
-                g,
-                f,
-                in_beam: RefCell::new(true),
-            })
+        let h = -2;
+        let f = -2;
+        let node = MockInBeam {
+            state,
+            cost,
+            h,
+            f,
+            closed: Cell::new(false),
         };
-        let (generated, beam_pruning) = beam.insert(&mut registry, state, cost, g, f, constructor);
+        let (generated, beam_pruning) = beam.insert(&mut registry, node);
         assert!(!generated);
         assert!(beam_pruning);
 
         let peek = beam.pop();
         assert!(peek.is_some());
         let node = peek.unwrap();
         assert_eq!(
@@ -519,111 +435,101 @@
                 signature_variables: Rc::new(HashableSignatureVariables {
                     integer_variables: vec![1, 2, 3],
                     ..Default::default()
                 }),
                 ..Default::default()
             },
         );
-        assert_eq!(node.cost(), 0);
-        assert_eq!(node.g(), 0);
-        assert_eq!(node.f(), 1);
-        assert!(!node.in_beam());
+        assert_eq!(node.cost(&model), 0);
+        assert!(node.is_closed());
         let peek = beam.pop();
         assert_eq!(peek, None);
     }
 
     #[test]
     fn normal_beam_drain() {
         let model = Rc::new(dypdl::Model::default());
-        let mut registry = StateRegistry::<i32, MockInBeam>::new(model);
+        let mut registry = StateRegistry::<i32, MockInBeam>::new(model.clone());
         let mut beam = Beam::new(1);
 
         let state = StateInRegistry {
             signature_variables: Rc::new(HashableSignatureVariables {
                 integer_variables: vec![1, 2, 3],
                 ..Default::default()
             }),
             ..Default::default()
         };
         let cost = 1;
-        let g = 0;
-        let f = 2;
-        let constructor = |state, cost, _: Option<&_>| {
-            Some(MockInBeam {
-                state,
-                cost,
-                g,
-                f,
-                in_beam: RefCell::new(true),
-            })
+        let h = -1;
+        let f = -2;
+        let node = MockInBeam {
+            state,
+            cost,
+            h,
+            f,
+            closed: Cell::new(false),
         };
-        let (generated, beam_pruning) = beam.insert(&mut registry, state, cost, g, f, constructor);
+        let (generated, beam_pruning) = beam.insert(&mut registry, node);
         assert!(generated);
         assert!(!beam_pruning);
 
         let state = StateInRegistry {
             signature_variables: Rc::new(HashableSignatureVariables {
                 integer_variables: vec![1, 2, 3],
                 ..Default::default()
             }),
             ..Default::default()
         };
         let cost = 0;
-        let g = 0;
-        let f = 1;
-        let constructor = |state, cost, _: Option<&_>| {
-            Some(MockInBeam {
-                state,
-                cost,
-                g,
-                f,
-                in_beam: RefCell::new(true),
-            })
+        let h = -1;
+        let f = -1;
+        let node = MockInBeam {
+            state,
+            cost,
+            h,
+            f,
+            closed: Cell::new(false),
         };
-        let (generated, beam_pruning) = beam.insert(&mut registry, state, cost, g, f, constructor);
+        let (generated, beam_pruning) = beam.insert(&mut registry, node);
         assert!(!generated);
         assert!(!beam_pruning);
 
         let state = StateInRegistry {
             signature_variables: Rc::new(HashableSignatureVariables {
                 integer_variables: vec![2, 3, 4],
                 ..Default::default()
             }),
             ..Default::default()
         };
         let cost = 0;
-        let g = 0;
-        let f = 2;
-        let constructor = |state, cost, _: Option<&_>| {
-            Some(MockInBeam {
-                state,
-                cost,
-                g,
-                f,
-                in_beam: RefCell::new(true),
-            })
+        let h = -2;
+        let f = -2;
+        let node = MockInBeam {
+            state,
+            cost,
+            h,
+            f,
+            closed: Cell::new(false),
         };
-        let (generated, beam_pruning) = beam.insert(&mut registry, state, cost, g, f, constructor);
+        let (generated, beam_pruning) = beam.insert(&mut registry, node);
         assert!(!generated);
         assert!(beam_pruning);
 
-        let mut iter = BeamInterface::<i32, i32, MockInBeam>::drain(&mut beam);
+        let mut iter = beam.drain();
         let peek = iter.next();
         assert!(peek.is_some());
         let node = peek.unwrap();
         assert_eq!(
             node.state,
             StateInRegistry {
                 signature_variables: Rc::new(HashableSignatureVariables {
                     integer_variables: vec![1, 2, 3],
                     ..Default::default()
                 }),
                 ..Default::default()
             },
         );
-        assert_eq!(node.cost(), 0);
-        assert_eq!(node.g(), 0);
-        assert_eq!(node.f(), 1);
-        assert!(node.in_beam());
+        assert_eq!(node.cost(&model), 0);
+        assert!(!node.is_closed());
         assert_eq!(iter.next(), None);
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/f_node.rs` & `didppy-0.4.0/src/model/transition.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,1083 +1,1262 @@
-use super::bfs_node::BfsNodeInterface;
-use super::hashable_state::HashableSignatureVariables;
-use super::state_registry::{StateInRegistry, StateInformation, StateRegistry};
-use super::transition_chain::{TransitionChain, TransitionChainInterface};
-use super::util::exceed_bound;
-use dypdl::variable_type::Numeric;
-use dypdl::ReduceFunction;
-use std::cell::RefCell;
-use std::cmp::Ordering;
-use std::rc::Rc;
+use crate::ModelPy;
 
-/// Node ordered by the f-value.
-///
-/// Nodes are totally ordered by their f-values, and tie is broken by the h-values.
-///
-/// # Examples
-///
-/// ```
-/// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::{
-///     FNode, BfsNodeInterface,
-/// };
-/// use dypdl_heuristic_search::search_algorithm::data_structure::state_registry::{
-///     StateInformation, StateInRegistry, StateRegistry,
-/// };
-/// use std::rc::Rc;
-///
-/// let mut model = Model::default();
-/// let variable = model.add_integer_variable("variable", 0).unwrap();
-///
-/// let model = Rc::new(model);
-/// let mut registry = StateRegistry::new(model.clone());
-///
-/// let h_evaluator = |_: &_, _: &_| Some(0);
-/// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-///
-/// let (node, h, f) = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator).unwrap();
-/// assert_eq!(h, 0);
-/// assert_eq!(f, 0);
-/// assert_eq!(node.state(), &StateInRegistry::from(model.target.clone()));
-/// assert_eq!(node.cost(), 0);
-/// assert_eq!(node.get_bound(&model), 0);
-/// assert!(!node.closed());
-/// assert_eq!(node.transitions(), vec![]);
-///
-/// node.close();
-/// assert!(node.closed());
-///
-/// let mut transition = Transition::new("transition");
-/// transition.set_cost(IntegerExpression::Cost + 1);
-/// transition.add_effect(variable, variable + 1).unwrap();
-/// let expected_state: StateInRegistry = transition.apply(&model.target, &model.table_registry);
-///
-/// let (successor, h, f, generated) = node.generate_successor(
-///     Rc::new(transition.clone()), &mut registry, h_evaluator, f_evaluator, None
-/// ).unwrap();
-/// assert_eq!(h, 0);
-/// assert_eq!(f, 1);
-/// assert!(generated);
-/// assert_eq!(successor.state(), &expected_state);
-/// assert_eq!(successor.cost(), 1);
-/// assert_eq!(successor.get_bound(&model), 1);
-/// assert!(!successor.closed());
-/// assert_eq!(successor.transitions(), vec![transition]);
-/// ```
-#[derive(Debug, Default)]
-pub struct FNode<T: Numeric> {
-    g: T,
-    h: T,
-    f: T,
-    state: StateInRegistry<Rc<HashableSignatureVariables>>,
-    closed: RefCell<bool>,
-    transitions: Option<Rc<TransitionChain>>,
+use super::expression::*;
+use super::state::StatePy;
+use dypdl::expression::*;
+use dypdl::prelude::*;
+use dypdl::TransitionInterface;
+use pyo3::exceptions::PyRuntimeError;
+use pyo3::prelude::*;
+
+#[derive(FromPyObject, Debug, PartialEq, Clone)]
+pub enum CostUnion {
+    #[pyo3(transparent)]
+    Int(IntUnion),
+    #[pyo3(transparent)]
+    Float(FloatUnion),
 }
 
-impl<T: Numeric + PartialOrd> PartialEq for FNode<T> {
-    /// Nodes are compared by their f- and h-values.
-    /// This does not mean that the nodes are the same.
-    #[inline]
-    fn eq(&self, other: &Self) -> bool {
-        self.f == other.f && self.h == other.h
+impl From<CostUnion> for CostExpression {
+    fn from(cost: CostUnion) -> Self {
+        match cost {
+            CostUnion::Int(cost) => CostExpression::Integer(IntegerExpression::from(cost)),
+            CostUnion::Float(cost) => CostExpression::Continuous(ContinuousExpression::from(cost)),
+        }
     }
 }
 
-impl<T: Numeric + Ord> Eq for FNode<T> {}
+#[derive(FromPyObject, Debug, Clone, Copy, PartialEq)]
+pub enum IntOrFloat {
+    #[pyo3(transparent, annotation = "int")]
+    Int(Integer),
+    #[pyo3(transparent, annotation = "float")]
+    Float(Continuous),
+}
 
-impl<T: Numeric + Ord> Ord for FNode<T> {
-    #[inline]
-    fn cmp(&self, other: &Self) -> Ordering {
-        match self.f.cmp(&other.f) {
-            Ordering::Equal => self.h.cmp(&other.h),
-            result => result,
+impl IntoPy<Py<PyAny>> for IntOrFloat {
+    fn into_py(self, py: Python<'_>) -> Py<PyAny> {
+        match self {
+            Self::Int(int) => int.into_py(py),
+            Self::Float(float) => float.into_py(py),
         }
     }
 }
-
-impl<T: Numeric + Ord> PartialOrd for FNode<T> {
-    #[inline]
-    fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
-        Some(self.cmp(other))
+/// Transition.
+///
+/// An effect on a variable can be accessed by :code:`transition[var]`, where :code:`transition` is :class:`Transition` and
+/// :code:`var` is either of :class:`ElementVar`, :class:`ElementResourceVar`, :class:`SetVar`, :class:`IntVar`, :class:`IntResourceVar`, :class:`FloatVar`, and :class:`FloatResourceVar`.
+///
+/// Parameters
+/// ----------
+/// name: str
+///     Name of the transition.
+/// cost: IntExpr, IntVar, IntResourceVar, FloatExpr, FloatVar, FloatResourceVar, int, float, or None, default: None
+///     Cost expression.
+///     :func:`IntExpr.state_cost()` or :func:`FloatExpr.state_cost()` can be used to represent the cost of the transitioned state.
+///     If :code:`None`, :func:`IntExpr.state_cost()` is used.
+/// preconditions: list of Condition or None, default: None
+///     Preconditions, which must be satisfied by a state to be applicable.
+/// effects: list of tuple of a variable and an expression or None, default: None
+///     Effects, a sequence of tuple of a variable and an expression.
+///     Instead of an expression, a variable or an immediate value can be used.
+///
+/// Raises
+/// ------
+/// RuntimeError
+///     If multiple effects are defined for the same variable.
+/// TypeError
+///     If the types of a variable and an expression in :code:`effects` mismatch.
+///
+/// Examples
+/// --------
+/// >>> import didppy as dp
+/// >>> model = dp.Model()
+/// >>> var = model.add_int_var(target=4)
+/// >>> t = dp.Transition(
+/// ...     name="t",
+/// ...     cost=dp.IntExpr.state_cost() + 1,
+/// ...     preconditions=[var >= 1],
+/// ...     effects=[(var, var - 1)],
+/// ... )
+/// >>> state = model.target_state
+/// >>> t.cost.eval_cost(0, state, model)
+/// 1
+/// >>> t.cost = dp.IntExpr.state_cost() + 2
+/// >>> t.cost.eval_cost(0, state, model)
+/// 2
+/// >>> preconditions = t.preconditions
+/// >>> preconditions[0].eval(state, model)
+/// True
+/// >>> t[var].eval(state, model)
+/// 3
+/// >>> t[var] = var + 1
+/// >>> t[var].eval(state, model)
+/// 5
+#[pyclass(name = "Transition")]
+#[pyo3(text_signature = "(name, cost=None, preconditions=None, effects=None)")]
+#[derive(Debug, PartialEq, Clone, Default)]
+pub struct TransitionPy(Transition);
+
+impl From<TransitionPy> for Transition {
+    fn from(transition: TransitionPy) -> Self {
+        transition.0
     }
 }
 
-impl<T: Numeric> StateInformation<T, Rc<HashableSignatureVariables>> for FNode<T> {
-    #[inline]
-    fn state(&self) -> &StateInRegistry<Rc<HashableSignatureVariables>> {
-        &self.state
-    }
-
-    #[inline]
-    fn cost(&self) -> T {
-        self.g
+impl From<Transition> for TransitionPy {
+    fn from(transition: Transition) -> Self {
+        TransitionPy(transition)
     }
 }
 
-impl<T: Numeric + Ord> BfsNodeInterface<T> for FNode<T> {
-    fn generate_initial_node<H, F>(
-        registry: &mut StateRegistry<T, Self>,
-        h_evaluator: H,
-        f_evaluator: F,
-    ) -> Option<(Rc<Self>, T, T)>
-    where
-        H: Fn(&StateInRegistry<Rc<HashableSignatureVariables>>, &dypdl::Model) -> Option<T>,
-        F: Fn(T, T, &StateInRegistry<Rc<HashableSignatureVariables>>, &dypdl::Model) -> T,
-    {
-        let initial_state = StateInRegistry::from(registry.model().target.clone());
-        let g = T::zero();
-        let h = h_evaluator(&initial_state, registry.model())?;
-        let f = f_evaluator(g, h, &initial_state, registry.model());
+impl TransitionPy {
+    pub fn inner_as_ref(&self) -> &Transition {
+        &self.0
+    }
 
-        let (h_priority, f_priority) = if registry.model().reduce_function == ReduceFunction::Min {
-            (-h, -f)
-        } else {
-            (h, f)
-        };
-        let constructor = |state: StateInRegistry, g: T, _: Option<&FNode<T>>| {
-            Some(FNode {
-                state,
-                g,
-                h: h_priority,
-                f: f_priority,
-                ..Default::default()
-            })
-        };
-        let (node, _) = registry.insert(initial_state, g, constructor)?;
-        Some((node, h, f))
+    fn get_effect<T: Clone>(var_id: usize, effects: &[(usize, T)]) -> Option<T> {
+        for (id, effect) in effects {
+            if *id == var_id {
+                return Some(effect.clone());
+            }
+        }
+        None
     }
 
-    fn generate_successor<H, F>(
-        &self,
-        transition: Rc<dypdl::Transition>,
-        registry: &mut StateRegistry<T, Self>,
-        h_evaluator: H,
-        f_evaluator: F,
-        primal_bound: Option<T>,
-    ) -> Option<(Rc<FNode<T>>, T, T, bool)>
-    where
-        H: Fn(&StateInRegistry, &dypdl::Model) -> Option<T>,
-        F: Fn(T, T, &StateInRegistry, &dypdl::Model) -> T,
-    {
-        let (state, g) = registry.model().generate_successor_state(
-            self.state(),
-            self.cost(),
-            transition.as_ref(),
-            None,
-        )?;
+    fn set_effect<T: Clone>(var_id: usize, new_effect: T, effects: &mut Vec<(usize, T)>) {
+        for (id, effect) in effects.iter_mut() {
+            if *id == var_id {
+                *effect = new_effect;
+                return;
+            }
+        }
 
-        let h = h_evaluator(&state, registry.model())?;
-        let f = f_evaluator(g, h, &state, registry.model());
+        effects.push((var_id, new_effect));
+    }
+}
 
-        if exceed_bound(registry.model(), f, primal_bound) {
-            return None;
+#[pymethods]
+impl TransitionPy {
+    #[new]
+    #[pyo3(signature = (name, cost = None, preconditions = vec![], effects = vec![]))]
+    pub fn new_py(
+        name: &str,
+        cost: Option<CostUnion>,
+        preconditions: Option<Vec<ConditionPy>>,
+        effects: Option<Vec<(VarUnion, &PyAny)>>,
+    ) -> PyResult<TransitionPy> {
+        let mut transition = TransitionPy(Transition::new(name));
+        if let Some(cost) = cost {
+            transition.set_cost(cost);
+        }
+        if let Some(preconditions) = preconditions {
+            for condition in preconditions {
+                transition.add_precondition(condition);
+            }
         }
+        if let Some(effects) = effects {
+            for (var, expr) in effects {
+                transition.add_effect(var, expr)?;
+            }
+        }
+        Ok(transition)
+    }
 
-        let (h_priority, f_priority) = if registry.model().reduce_function == ReduceFunction::Min {
-            (-h, -f)
-        } else {
-            (h, f)
-        };
+    /// str : Name of the transition.
+    #[getter]
+    pub fn name(&self) -> String {
+        self.0.get_full_name()
+    }
 
-        let constructor = |state: StateInRegistry, g: T, _: Option<&FNode<T>>| {
-            Some(FNode {
-                state,
-                g,
-                h: h_priority,
-                f: f_priority,
-                closed: RefCell::new(false),
-                transitions: Some(Rc::new(TransitionChain::new(
-                    self.transitions.clone(),
-                    transition,
-                ))),
-            })
-        };
+    #[setter]
+    pub fn set_name(&mut self, name: &str) {
+        self.0.name = name.to_string();
+    }
 
-        let (successor, dominated) = registry.insert(state, g, constructor)?;
+    /// IntExpr or FloatExpr : Cost expression.
+    #[getter]
+    pub fn cost(&self) -> IntOrFloatExpr {
+        self.0.cost.clone().into()
+    }
 
-        let mut generated = true;
+    #[setter]
+    fn set_cost(&mut self, cost: CostUnion) {
+        match cost {
+            CostUnion::Int(cost) => self.0.set_cost(IntegerExpression::from(cost)),
+            CostUnion::Float(cost) => self.0.set_cost(ContinuousExpression::from(cost)),
+        }
+    }
 
-        if let Some(dominated) = dominated {
-            if !*dominated.closed.borrow() {
-                *dominated.closed.borrow_mut() = true;
-                generated = false;
+    /// list of Condition : Preconditions.   
+    /// Note that the preconditions and their order might be changed due to internal optimizations.
+    #[getter]
+    fn preconditions(&self) -> Vec<ConditionPy> {
+        self.0
+            .get_preconditions()
+            .into_iter()
+            .map(ConditionPy::from)
+            .collect()
+    }
+
+    /// add_precondition(condition)
+    ///
+    /// Adds a precondition to the transition.
+    ///
+    /// Parameters
+    /// ----------
+    /// condition: Condition
+    ///     Precondition.
+    ///
+    /// Examples
+    /// --------
+    /// >>> import didppy as dp
+    /// >>> model = dp.Model()
+    /// >>> var = model.add_int_var(target=4)
+    /// >>> t = dp.Transition(name="t")
+    /// >>> t.add_precondition(var >= 1)
+    /// >>> t.preconditions[0].eval(model.target_state, model)
+    /// True
+    #[pyo3(signature = (condition))]
+    fn add_precondition(&mut self, condition: ConditionPy) {
+        self.0.add_precondition(condition.into())
+    }
+
+    fn __getitem__(&self, var: VarUnion) -> ExprUnion {
+        match var {
+            VarUnion::Element(var) => {
+                let id = ElementVariable::from(var).id();
+                let effect = Self::get_effect(id, &self.0.effect.element_effects);
+
+                if let Some(effect) = effect {
+                    ExprUnion::Element(ElementExprPy::from(effect))
+                } else {
+                    ExprUnion::Element(ElementExprPy::from(ElementExpression::from(var)))
+                }
+            }
+            VarUnion::ElementResource(var) => {
+                let id = ElementResourceVariable::from(var).id();
+                let effect = Self::get_effect(id, &self.0.effect.element_resource_effects);
+
+                if let Some(effect) = effect {
+                    ExprUnion::Element(ElementExprPy::from(effect))
+                } else {
+                    ExprUnion::Element(ElementExprPy::from(ElementExpression::from(var)))
+                }
+            }
+            VarUnion::Set(var) => {
+                let id = SetVariable::from(var).id();
+                let effect = Self::get_effect(id, &self.0.effect.set_effects);
+
+                if let Some(effect) = effect {
+                    ExprUnion::Set(SetExprPy::from(effect))
+                } else {
+                    ExprUnion::Set(SetExprPy::from(SetExpression::from(var)))
+                }
+            }
+            VarUnion::Int(var) => {
+                let id = IntegerVariable::from(var).id();
+                let effect = Self::get_effect(id, &self.0.effect.integer_effects);
+
+                if let Some(effect) = effect {
+                    ExprUnion::Int(IntExprPy::from(effect))
+                } else {
+                    ExprUnion::Int(IntExprPy::from(IntegerExpression::from(var)))
+                }
+            }
+            VarUnion::IntResource(var) => {
+                let id = IntegerResourceVariable::from(var).id();
+                let effect = Self::get_effect(id, &self.0.effect.integer_resource_effects);
+
+                if let Some(effect) = effect {
+                    ExprUnion::Int(IntExprPy::from(effect))
+                } else {
+                    ExprUnion::Int(IntExprPy::from(IntegerExpression::from(var)))
+                }
+            }
+            VarUnion::Float(var) => {
+                let id = ContinuousVariable::from(var).id();
+                let effect = Self::get_effect(id, &self.0.effect.continuous_effects);
+
+                if let Some(effect) = effect {
+                    ExprUnion::Float(FloatExprPy::from(effect))
+                } else {
+                    ExprUnion::Float(FloatExprPy::from(ContinuousExpression::from(var)))
+                }
+            }
+            VarUnion::FloatResource(var) => {
+                let id = ContinuousResourceVariable::from(var).id();
+                let effect = Self::get_effect(id, &self.0.effect.continuous_resource_effects);
+
+                if let Some(effect) = effect {
+                    ExprUnion::Float(FloatExprPy::from(effect))
+                } else {
+                    ExprUnion::Float(FloatExprPy::from(ContinuousExpression::from(var)))
+                }
             }
         }
-
-        Some((successor, h, f, generated))
     }
 
-    fn closed(&self) -> bool {
-        *self.closed.borrow()
+    fn __setitem__(&mut self, var: VarUnion, expr: &PyAny) -> PyResult<()> {
+        match var {
+            VarUnion::Element(var) => {
+                let var = ElementVariable::from(var);
+                let expr: ElementUnion = expr.extract()?;
+                let expr = ElementExpression::from(expr);
+                Self::set_effect(var.id(), expr, &mut self.0.effect.element_effects);
+            }
+            VarUnion::ElementResource(var) => {
+                let var = ElementResourceVariable::from(var);
+                let expr: ElementUnion = expr.extract()?;
+                let expr = ElementExpression::from(expr);
+                Self::set_effect(var.id(), expr, &mut self.0.effect.element_resource_effects);
+            }
+            VarUnion::Set(var) => {
+                let var = SetVariable::from(var);
+                let expr: SetUnion = expr.extract()?;
+                let expr = SetExpression::from(expr);
+                Self::set_effect(var.id(), expr, &mut self.0.effect.set_effects);
+            }
+            VarUnion::Int(var) => {
+                let var = IntegerVariable::from(var);
+                let expr: IntUnion = expr.extract()?;
+                let expr = IntegerExpression::from(expr);
+                Self::set_effect(var.id(), expr, &mut self.0.effect.integer_effects);
+            }
+            VarUnion::IntResource(var) => {
+                let var = IntegerResourceVariable::from(var);
+                let expr: IntUnion = expr.extract()?;
+                let expr = IntegerExpression::from(expr);
+                Self::set_effect(var.id(), expr, &mut self.0.effect.integer_resource_effects);
+            }
+            VarUnion::Float(var) => {
+                let var = ContinuousVariable::from(var);
+                let expr: FloatUnion = expr.extract()?;
+                let expr = ContinuousExpression::from(expr);
+                Self::set_effect(var.id(), expr, &mut self.0.effect.continuous_effects);
+            }
+            VarUnion::FloatResource(var) => {
+                let var = ContinuousResourceVariable::from(var);
+                let expr: FloatUnion = expr.extract()?;
+                let expr = ContinuousExpression::from(expr);
+                Self::set_effect(
+                    var.id(),
+                    expr,
+                    &mut self.0.effect.continuous_resource_effects,
+                );
+            }
+        };
+        Ok(())
     }
 
-    fn close(&self) {
-        *self.closed.borrow_mut() = true;
+    /// add_effect(var, expr)
+    ///
+    /// Adds an effect to the transition.
+    ///
+    /// Parameters
+    /// ----------
+    /// var: ElementVar, ElementResourceVar, SetVar, IntVar, IntResourceVar, FloatVar, or FloatResourceVar
+    ///     Variable to update.
+    /// expr: ElementExpr, ElementVar, ElementResourceVar, SetExpr, SetVar, SetConst, IntExpr, IntVar, IntResourceVar, FloatExpr, FloatVar, FloatResourceVar, int, or float
+    ///     Expression to update the variable.
+    ///
+    /// Raises
+    /// ------
+    /// TypeError
+    ///     If the types of :code:`var` and :code:`expr` mismatch.
+    ///
+    /// Examples
+    /// --------
+    /// >>> import didppy as dp
+    /// >>> model = dp.Model()
+    /// >>> var = model.add_int_var(target=4)
+    /// >>> t = dp.Transition(name="t")
+    /// >>> t.add_effect(var, var + 1)
+    /// >>> t[var].eval(model.target_state, model)
+    /// 5
+    #[pyo3(signature = (var, expr))]
+    fn add_effect(&mut self, var: VarUnion, expr: &PyAny) -> PyResult<()> {
+        let result = match var {
+            VarUnion::Element(var) => {
+                let expr: ElementUnion = expr.extract()?;
+                self.0
+                    .add_effect(ElementVariable::from(var), ElementExpression::from(expr))
+            }
+            VarUnion::ElementResource(var) => {
+                let expr: ElementUnion = expr.extract()?;
+                self.0.add_effect(
+                    ElementResourceVariable::from(var),
+                    ElementExpression::from(expr),
+                )
+            }
+            VarUnion::Set(var) => {
+                let expr: SetUnion = expr.extract()?;
+                self.0
+                    .add_effect(SetVariable::from(var), SetExpression::from(expr))
+            }
+            VarUnion::Int(var) => {
+                let expr: IntUnion = expr.extract()?;
+                self.0
+                    .add_effect(IntegerVariable::from(var), IntegerExpression::from(expr))
+            }
+            VarUnion::IntResource(var) => {
+                let expr: IntUnion = expr.extract()?;
+                self.0.add_effect(
+                    IntegerResourceVariable::from(var),
+                    IntegerExpression::from(expr),
+                )
+            }
+            VarUnion::Float(var) => {
+                let expr: FloatUnion = expr.extract()?;
+                self.0.add_effect(
+                    ContinuousVariable::from(var),
+                    ContinuousExpression::from(expr),
+                )
+            }
+            VarUnion::FloatResource(var) => {
+                let expr: FloatUnion = expr.extract()?;
+                self.0.add_effect(
+                    ContinuousResourceVariable::from(var),
+                    ContinuousExpression::from(expr),
+                )
+            }
+        };
+        match result {
+            Ok(()) => Ok(()),
+            Err(err) => Err(PyRuntimeError::new_err(err.to_string())),
+        }
     }
 
-    fn get_bound(&self, model: &dypdl::Model) -> T {
-        if model.reduce_function == ReduceFunction::Min {
-            -self.f
+    /// is_applicable(state, model)
+    ///
+    /// Checks if the transition is applicable in the given state.
+    ///
+    /// Parameters
+    /// ----------
+    /// state: State
+    ///     State to check.
+    /// model: Model
+    ///     DyPDL model.
+    ///
+    /// Returns
+    /// -------
+    /// bool
+    ///     True if the transition is applicable in the given state.
+    ///
+    /// Raises
+    /// ------
+    /// PanicException
+    ///     If preconditions are invalid.
+    ///
+    /// Examples
+    /// --------
+    /// >>> import didppy as dp
+    /// >>> model = dp.Model()
+    /// >>> var = model.add_int_var(target=4)
+    /// >>> t = dp.Transition(name="t", preconditions=[var >= 0])
+    /// >>> t.is_applicable(model.target_state, model)
+    /// True
+    #[pyo3(signature = (state, model))]
+    fn is_applicable(&self, state: &StatePy, model: &ModelPy) -> bool {
+        self.0
+            .is_applicable(state.inner_as_ref(), &model.inner_as_ref().table_registry)
+    }
+
+    /// apply(state, model)
+    ///
+    /// Applies the transition to the given state.
+    ///
+    /// Parameters
+    /// ----------
+    /// state: State
+    ///     State to apply the transition to.
+    /// model: Model
+    ///     DyPDL model.
+    ///
+    /// Returns
+    /// -------
+    /// State
+    ///    State after applying the transition.
+    ///
+    /// Raises
+    /// ------
+    /// PanicException
+    ///     If preconditions are invalid.
+    ///
+    /// Examples
+    /// --------
+    /// >>> import didppy as dp
+    /// >>> model = dp.Model()
+    /// >>> var = model.add_int_var(target=4)
+    /// >>> t = dp.Transition(name="t", effects=[(var, var + 1)])
+    /// >>> state = t.apply(model.target_state, model)
+    /// >>> state[var]
+    /// 5
+    #[pyo3(signature = (state, model))]
+    fn apply(&self, state: &mut StatePy, model: &ModelPy) -> StatePy {
+        self.0
+            .apply(state.inner_as_ref(), &model.inner_as_ref().table_registry)
+    }
+
+    /// eval_cost(cost, state, model)
+    ///
+    /// Evaluates the cost of the transition in the given state.
+    ///
+    /// Parameters
+    /// ----------
+    /// cost: int or float
+    ///     Cost of the next state.
+    /// state: State
+    ///     Current state.
+    /// model: Model
+    ///     DyPDL model.
+    ///
+    /// Returns
+    /// -------
+    /// int or float
+    ///     Cost of the transition.
+    ///
+    /// Raises
+    /// ------
+    /// TypeError
+    ///     If the type of :code:`cost` mismatches the cost type of :code:`model`.
+    /// PanicException
+    ///     If the cost expression is invalid.
+    ///
+    /// Examples
+    /// --------
+    /// >>> import didppy as dp
+    /// >>> model = dp.Model()
+    /// >>> var = model.add_int_var(target=4)
+    /// >>> t = dp.Transition(name="t", cost=dp.IntExpr.state_cost() + 1)
+    /// >>> t.eval_cost(1, model.target_state, model)
+    /// 2
+    #[pyo3(signature = (cost, state, model))]
+    fn eval_cost(&self, cost: &PyAny, state: &StatePy, model: &ModelPy) -> PyResult<IntOrFloat> {
+        if model.float_cost() {
+            let cost = cost.extract()?;
+            Ok(IntOrFloat::Float(self.0.eval_cost(
+                cost,
+                state.inner_as_ref(),
+                &model.inner_as_ref().table_registry,
+            )))
         } else {
-            self.f
+            let cost = cost.extract()?;
+            Ok(IntOrFloat::Int(self.0.eval_cost(
+                cost,
+                state.inner_as_ref(),
+                &model.inner_as_ref().table_registry,
+            )))
         }
     }
-
-    fn transitions(&self) -> Vec<dypdl::Transition> {
-        self.transitions
-            .as_ref()
-            .map_or_else(Vec::new, |transitions| transitions.transitions())
-    }
 }
 
 #[cfg(test)]
 mod tests {
-    use super::super::hashable_state::HashableSignatureVariables;
     use super::*;
-    use dypdl::expression::*;
-    use dypdl::prelude::*;
-    use dypdl::Effect;
     use dypdl::GroundedCondition;
-    use rustc_hash::FxHashMap;
 
     #[test]
-    fn node_state() {
-        let node = FNode {
-            state: StateInRegistry {
-                signature_variables: Rc::new(HashableSignatureVariables {
-                    integer_variables: vec![1, 2, 3],
-                    ..Default::default()
-                }),
-                ..Default::default()
-            },
-            g: 1,
-            h: 2,
-            f: 3,
-            closed: RefCell::new(false),
-            transitions: None,
-        };
-        assert_eq!(node.state(), &node.state);
+    fn cost_expression_from_cost_union_int() {
+        let cost = CostUnion::Int(IntUnion::Const(0));
+        assert_eq!(
+            CostExpression::from(cost),
+            CostExpression::Integer(IntegerExpression::Constant(0))
+        );
     }
 
     #[test]
-    fn node_cost() {
-        let node = FNode {
-            state: StateInRegistry::default(),
-            g: 1,
-            h: 2,
-            f: 3,
-            closed: RefCell::new(false),
-            transitions: None,
-        };
-        assert_eq!(node.cost(), 1);
+    fn cost_expression_from_cost_union_float() {
+        let cost = CostUnion::Float(FloatUnion::Const(0.0));
+        assert_eq!(
+            CostExpression::from(cost),
+            CostExpression::Continuous(ContinuousExpression::Constant(0.0))
+        );
     }
 
     #[test]
-    fn node_eq() {
-        let node1 = FNode {
-            state: StateInRegistry {
-                signature_variables: Rc::new(HashableSignatureVariables {
-                    integer_variables: vec![1, 2, 3],
-                    ..Default::default()
-                }),
-                ..Default::default()
-            },
-            g: 1,
-            h: 2,
-            f: 3,
-            closed: RefCell::new(false),
-            transitions: None,
-        };
-        let node2 = FNode {
-            state: StateInRegistry {
-                signature_variables: Rc::new(HashableSignatureVariables {
-                    integer_variables: vec![4, 2, 3],
-                    ..Default::default()
-                }),
-                ..Default::default()
-            },
-            g: 1,
-            h: 2,
-            f: 3,
-            closed: RefCell::new(false),
-            transitions: None,
-        };
-        assert_eq!(node1, node2);
-        assert!(node1 >= node2);
-        assert!(node1 <= node2);
-        assert!(node2 >= node1);
-        assert!(node2 <= node1);
+    fn transition_from() {
+        let transition = TransitionPy(Transition::default());
+        assert_eq!(Transition::from(transition), Transition::default());
     }
 
     #[test]
-    fn node_lt() {
-        let node1 = FNode {
-            state: StateInRegistry {
-                signature_variables: Rc::new(HashableSignatureVariables {
-                    integer_variables: vec![1, 2, 3],
-                    ..Default::default()
-                }),
-                ..Default::default()
-            },
-            g: 1,
-            h: 2,
-            f: 3,
-            closed: RefCell::new(false),
-            transitions: None,
-        };
-        let node2 = FNode {
-            state: StateInRegistry {
-                signature_variables: Rc::new(HashableSignatureVariables {
-                    integer_variables: vec![4, 2, 3],
-                    ..Default::default()
-                }),
+    fn new() {
+        let transition = Transition::default();
+        assert_eq!(
+            TransitionPy::from(transition),
+            TransitionPy(Transition::default())
+        );
+    }
+
+    #[test]
+    fn new_py_with_none_ok() {
+        let result = TransitionPy::new_py("t", None, None, None);
+        assert!(result.is_ok());
+        assert_eq!(
+            result.unwrap(),
+            TransitionPy(Transition {
+                name: String::from("t"),
+                preconditions: vec![],
+                effect: dypdl::Effect::default(),
                 ..Default::default()
-            },
-            g: 2,
-            h: 2,
-            f: 4,
-            closed: RefCell::new(false),
-            transitions: None,
-        };
-        assert!(node1 < node2);
-        assert!(node1 <= node2);
-        assert!(node2 > node1);
-        assert!(node2 >= node1);
+            })
+        );
     }
 
     #[test]
-    fn node_lt_tie_breaking() {
-        let node1 = FNode {
-            state: StateInRegistry {
-                signature_variables: Rc::new(HashableSignatureVariables {
-                    integer_variables: vec![1, 2, 3],
+    fn new_py_ok() {
+        pyo3::prepare_freethreaded_python();
+
+        let mut model = Model::default();
+        let v1 = model.add_integer_variable("v1", 0);
+        assert!(v1.is_ok());
+        let v1 = v1.unwrap();
+        let v2 = model.add_continuous_variable("v2", 0.0);
+        assert!(v2.is_ok());
+        let v2 = v2.unwrap();
+
+        let preconditions = vec![
+            ConditionPy::from(Condition::Constant(true)),
+            ConditionPy::from(Condition::Constant(false)),
+        ];
+        let result = Python::with_gil(|py| {
+            let v1 = VarUnion::Int(IntVarPy::from(v1));
+            let v2 = VarUnion::Float(FloatVarPy::from(v2));
+            let expr1 = IntExprPy::from(IntegerExpression::Constant(1)).into_py(py);
+            let expr2 = FloatExprPy::from(ContinuousExpression::Constant(2.0)).into_py(py);
+            let effects = vec![(v1, expr1.as_ref(py)), (v2, expr2.as_ref(py))];
+            TransitionPy::new_py("t", None, Some(preconditions), Some(effects))
+        });
+        assert!(result.is_ok());
+        assert_eq!(
+            result.unwrap(),
+            TransitionPy(Transition {
+                name: String::from("t"),
+                preconditions: vec![
+                    GroundedCondition {
+                        condition: Condition::Constant(true),
+                        ..Default::default()
+                    },
+                    GroundedCondition {
+                        condition: Condition::Constant(false),
+                        ..Default::default()
+                    },
+                ],
+                effect: dypdl::Effect {
+                    integer_effects: vec![(v1.id(), IntegerExpression::Constant(1))],
+                    continuous_effects: vec![(v2.id(), ContinuousExpression::Constant(2.0))],
                     ..Default::default()
-                }),
+                },
                 ..Default::default()
-            },
-            g: 1,
-            h: 2,
-            f: 3,
-            closed: RefCell::new(false),
-            transitions: None,
-        };
-        let node2 = FNode {
-            state: StateInRegistry {
-                signature_variables: Rc::new(HashableSignatureVariables {
-                    integer_variables: vec![4, 2, 3],
+            })
+        );
+    }
+
+    #[test]
+    fn new_py_with_cost_ok() {
+        pyo3::prepare_freethreaded_python();
+
+        let mut model = Model::default();
+        let v1 = model.add_integer_variable("v1", 0);
+        assert!(v1.is_ok());
+        let v1 = v1.unwrap();
+        let v2 = model.add_continuous_variable("v2", 0.0);
+        assert!(v2.is_ok());
+        let v2 = v2.unwrap();
+
+        let cost = CostUnion::Int(IntUnion::Const(0));
+        let preconditions = vec![
+            ConditionPy::from(Condition::Constant(true)),
+            ConditionPy::from(Condition::Constant(false)),
+        ];
+        let result = Python::with_gil(|py| {
+            let v1 = VarUnion::Int(IntVarPy::from(v1));
+            let expr1 = IntExprPy::from(IntegerExpression::Constant(1)).into_py(py);
+            let v2 = VarUnion::Float(FloatVarPy::from(v2));
+            let expr2 = FloatExprPy::from(ContinuousExpression::Constant(2.0)).into_py(py);
+            let effects = vec![(v1, expr1.as_ref(py)), (v2, expr2.as_ref(py))];
+            TransitionPy::new_py("t", Some(cost), Some(preconditions), Some(effects))
+        });
+        assert!(result.is_ok());
+        assert_eq!(
+            result.unwrap(),
+            TransitionPy(Transition {
+                name: String::from("t"),
+                cost: CostExpression::Integer(IntegerExpression::Constant(0)),
+                preconditions: vec![
+                    GroundedCondition {
+                        condition: Condition::Constant(true),
+                        ..Default::default()
+                    },
+                    GroundedCondition {
+                        condition: Condition::Constant(false),
+                        ..Default::default()
+                    },
+                ],
+                effect: dypdl::Effect {
+                    integer_effects: vec![(v1.id(), IntegerExpression::Constant(1))],
+                    continuous_effects: vec![(v2.id(), ContinuousExpression::Constant(2.0))],
                     ..Default::default()
-                }),
+                },
                 ..Default::default()
-            },
-            g: 0,
-            h: 3,
-            f: 3,
-            closed: RefCell::new(false),
-            transitions: None,
-        };
-        assert!(node1 < node2);
-        assert!(node1 <= node2);
-        assert!(node2 > node1);
-        assert!(node2 >= node1);
+            })
+        );
     }
 
     #[test]
-    fn generate_initial_node_minimization() {
-        let model = Rc::new(Model {
-            reduce_function: ReduceFunction::Min,
-            ..Default::default()
+    fn new_err() {
+        let mut model = Model::default();
+        let v1 = model.add_integer_variable("v1", 0);
+        assert!(v1.is_ok());
+        let v1 = v1.unwrap();
+
+        let preconditions = vec![
+            ConditionPy::from(Condition::Constant(true)),
+            ConditionPy::from(Condition::Constant(false)),
+        ];
+        let result = Python::with_gil(|py| {
+            let v1 = VarUnion::Int(IntVarPy::from(v1));
+            let expr1 = ElementExprPy::from(ElementExpression::Constant(1)).into_py(py);
+            let effects = vec![(v1, expr1.as_ref(py))];
+            TransitionPy::new_py("t", None, Some(preconditions), Some(effects))
         });
-        let mut registry = StateRegistry::new(model.clone());
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 1;
-        let result = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        let (node, h, f) = result.unwrap();
-        assert_eq!(node.state, StateInRegistry::from(model.target.clone()));
-        assert_eq!(node.g, 0);
-        assert_eq!(node.h, -1);
-        assert_eq!(node.f, -1);
-        assert!(!*node.closed.borrow());
-        assert_eq!(node.transitions, None);
-        assert_eq!(h, 1);
-        assert_eq!(f, 1);
+        assert!(result.is_err());
     }
 
     #[test]
-    fn generate_initial_node_maximization() {
-        let model = Rc::new(Model {
-            reduce_function: ReduceFunction::Max,
+    fn name() {
+        let transition = TransitionPy(Transition {
+            name: String::from("t"),
             ..Default::default()
         });
-        let mut registry = StateRegistry::new(model.clone());
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 1;
-        let result = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        let (node, h, f) = result.unwrap();
-        assert_eq!(node.state, StateInRegistry::from(model.target.clone()));
-        assert_eq!(node.g, 0);
-        assert_eq!(node.h, 1);
-        assert_eq!(node.f, 1);
-        assert!(!*node.closed.borrow());
-        assert_eq!(node.transitions, None);
-        assert_eq!(h, 1);
-        assert_eq!(f, 1);
+        assert_eq!(transition.name(), String::from("t"));
     }
 
     #[test]
-    fn generate_initial_node_pruned_by_h() {
-        let mut name_to_integer_variable = FxHashMap::default();
-        name_to_integer_variable.insert(String::from("v1"), 0);
-        let model = Rc::new(Model::default());
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| None;
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 1;
-        let result = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert_eq!(result, None)
+    fn set_cost_int() {
+        let mut transition = TransitionPy(Transition::default());
+        transition.set_cost(CostUnion::Int(IntUnion::Const(0)));
+        assert_eq!(
+            transition,
+            TransitionPy(Transition {
+                cost: CostExpression::Integer(IntegerExpression::Constant(0)),
+                ..Default::default()
+            })
+        );
     }
 
     #[test]
-    fn generate_initial_node_pruned_by_duplicate() {
-        let model = Rc::new(Model::default());
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 1;
-        let result = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert!(result.is_some());
-        let result = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert_eq!(result, None);
+    fn set_cost_float() {
+        let mut transition = TransitionPy(Transition::default());
+        transition.set_cost(CostUnion::Float(FloatUnion::Const(0.0)));
+        assert_eq!(
+            transition,
+            TransitionPy(Transition {
+                cost: CostExpression::Continuous(ContinuousExpression::Constant(0.0)),
+                ..Default::default()
+            })
+        );
     }
 
     #[test]
-    fn generate_successor_minimize() {
-        let mut name_to_integer_resource_variable = FxHashMap::default();
-        name_to_integer_resource_variable.insert(String::from("v1"), 0);
-        name_to_integer_resource_variable.insert(String::from("v2"), 1);
-
-        let model = Rc::new(Model {
-            state_metadata: StateMetadata {
-                integer_resource_variable_names: vec![String::from("v1"), String::from("v2")],
-                name_to_integer_resource_variable,
-                integer_less_is_better: vec![true, false],
-                ..Default::default()
-            },
-            target: State {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![0, 0],
+    fn add_precondition() {
+        let mut transition = TransitionPy(Transition::default());
+        transition.add_precondition(ConditionPy::from(Condition::Constant(true)));
+        assert_eq!(
+            transition,
+            TransitionPy(Transition {
+                preconditions: vec![GroundedCondition {
+                    condition: Condition::Constant(true),
                     ..Default::default()
-                },
+                }],
                 ..Default::default()
-            },
-            reduce_function: ReduceFunction::Min,
-            ..Default::default()
-        });
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 2;
-
-        let node = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert!(node.is_some());
-        let (node, _, _) = node.unwrap();
-
-        let transition = Rc::new(Transition {
-            name: String::from("increase"),
-            effect: Effect {
-                integer_resource_effects: vec![
-                    (
-                        0,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(0)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                    (
-                        1,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(1)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                ],
-                ..Default::default()
-            },
-            cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(1)),
-            )),
-            ..Default::default()
-        });
-        let result = node.generate_successor(
-            transition.clone(),
-            &mut registry,
-            h_evaluator,
-            f_evaluator,
-            None,
+            })
         );
-        assert!(result.is_some());
-        let (successor, h, f, generated) = result.unwrap();
+    }
+
+    #[test]
+    fn add_element_effect_ok() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_element_variable("v", ob, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Element(ElementVarPy::from(v));
+            let expr = ElementExprPy::from(ElementExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_ok());
         assert_eq!(
-            successor.state,
-            StateInRegistry {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![1, 1],
+            transition,
+            TransitionPy(Transition {
+                effect: dypdl::Effect {
+                    element_effects: vec![(v.id(), ElementExpression::Constant(0))],
                     ..Default::default()
                 },
                 ..Default::default()
-            },
-        );
-        assert_eq!(
-            successor.transitions,
-            Some(Rc::new(TransitionChain::new(
-                node.transitions.clone(),
-                transition
-            )))
+            })
         );
-        assert_eq!(successor.h, -1);
-        assert_eq!(successor.f, -2);
-        assert_eq!(h, 1);
-        assert_eq!(f, 2);
-        assert!(generated);
-        assert!(!*node.closed.borrow());
     }
 
     #[test]
-    fn generate_successor_maximize() {
-        let mut name_to_integer_resource_variable = FxHashMap::default();
-        name_to_integer_resource_variable.insert(String::from("v1"), 0);
-        name_to_integer_resource_variable.insert(String::from("v2"), 1);
-
-        let model = Rc::new(Model {
-            state_metadata: StateMetadata {
-                integer_resource_variable_names: vec![String::from("v1"), String::from("v2")],
-                name_to_integer_resource_variable,
-                integer_less_is_better: vec![true, false],
-                ..Default::default()
-            },
-            target: State {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![0, 0],
-                    ..Default::default()
-                },
-                ..Default::default()
-            },
-            reduce_function: ReduceFunction::Max,
-            ..Default::default()
+    fn add_element_effect_type_err() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_element_variable("v", ob, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Element(ElementVarPy::from(v));
+            let expr = IntExprPy::from(IntegerExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
         });
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 2;
-
-        let node = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert!(node.is_some());
-        let (node, _, _) = node.unwrap();
-
-        let transition = Rc::new(Transition {
-            name: String::from("increase"),
-            effect: Effect {
-                integer_resource_effects: vec![
-                    (
-                        0,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(0)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                    (
-                        1,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(1)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                ],
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_element_effect_duplicate_err() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_element_variable("v", ob, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition {
+            effect: dypdl::Effect {
+                element_effects: vec![(v.id(), ElementExpression::Constant(0))],
                 ..Default::default()
             },
-            cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(1)),
-            )),
             ..Default::default()
         });
-        let result = node.generate_successor(
-            transition.clone(),
-            &mut registry,
-            h_evaluator,
-            f_evaluator,
-            None,
-        );
-        assert!(result.is_some());
-        let (successor, h, f, generated) = result.unwrap();
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Element(ElementVarPy::from(v));
+            let expr = ElementExprPy::from(ElementExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_element_resource_effect_ok() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_element_resource_variable("v", ob, false, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::ElementResource(ElementResourceVarPy::from(v));
+            let expr = ElementExprPy::from(ElementExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_ok());
         assert_eq!(
-            successor.state,
-            StateInRegistry {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![1, 1],
+            transition,
+            TransitionPy(Transition {
+                effect: dypdl::Effect {
+                    element_resource_effects: vec![(v.id(), ElementExpression::Constant(0))],
                     ..Default::default()
                 },
                 ..Default::default()
-            },
-        );
-        assert_eq!(
-            successor.transitions,
-            Some(Rc::new(TransitionChain::new(
-                node.transitions.clone(),
-                transition
-            )))
+            })
         );
-        assert_eq!(successor.h, 1);
-        assert_eq!(successor.f, 2);
-        assert_eq!(h, 1);
-        assert_eq!(f, 2);
-        assert!(generated);
-        assert!(!*node.closed.borrow());
     }
 
     #[test]
-    fn generate_successor_dominate() {
-        let mut name_to_integer_resource_variable = FxHashMap::default();
-        name_to_integer_resource_variable.insert(String::from("v1"), 0);
-        name_to_integer_resource_variable.insert(String::from("v2"), 1);
-
-        let model = Rc::new(Model {
-            state_metadata: StateMetadata {
-                integer_resource_variable_names: vec![String::from("v1"), String::from("v2")],
-                name_to_integer_resource_variable,
-                integer_less_is_better: vec![false, false],
-                ..Default::default()
-            },
-            target: State {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![0, 0],
-                    ..Default::default()
-                },
-                ..Default::default()
-            },
-            reduce_function: ReduceFunction::Min,
-            ..Default::default()
+    fn add_element_resource_effect_type_err() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_element_resource_variable("v", ob, false, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::ElementResource(ElementResourceVarPy::from(v));
+            let expr = IntExprPy::from(IntegerExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
         });
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 2;
-
-        let node = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert!(node.is_some());
-        let (node, _, _) = node.unwrap();
-
-        let transition = Rc::new(Transition {
-            name: String::from("increase"),
-            effect: Effect {
-                integer_resource_effects: vec![
-                    (
-                        0,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(0)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                    (
-                        1,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(1)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                ],
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_element_resource_effect_duplicate_err() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_element_resource_variable("v", ob, false, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition {
+            effect: dypdl::Effect {
+                element_resource_effects: vec![(v.id(), ElementExpression::Constant(0))],
                 ..Default::default()
             },
-            cost: CostExpression::Integer(IntegerExpression::Cost),
             ..Default::default()
         });
-        let result = node.generate_successor(
-            transition.clone(),
-            &mut registry,
-            h_evaluator,
-            f_evaluator,
-            None,
-        );
-        assert!(result.is_some());
-        let (successor, h, f, generated) = result.unwrap();
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::ElementResource(ElementResourceVarPy::from(v));
+            let expr = ElementExprPy::from(ElementExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_set_effect_ok() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_set_variable("v", ob, Set::with_capacity(10));
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Set(SetVarPy::from(v));
+            let expr = SetConstPy::from(Set::with_capacity(10)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_ok());
         assert_eq!(
-            successor.state,
-            StateInRegistry {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![1, 1],
+            transition,
+            TransitionPy(Transition {
+                effect: dypdl::Effect {
+                    set_effects: vec![(
+                        v.id(),
+                        SetExpression::Reference(ReferenceExpression::Constant(
+                            Set::with_capacity(10)
+                        ))
+                    )],
                     ..Default::default()
                 },
                 ..Default::default()
-            },
-        );
-        assert_eq!(
-            successor.transitions,
-            Some(Rc::new(TransitionChain::new(
-                node.transitions.clone(),
-                transition
-            )))
+            })
         );
-        assert_eq!(successor.h, -1);
-        assert_eq!(successor.f, -2);
-        assert_eq!(h, 1);
-        assert_eq!(f, 2);
-        assert!(!generated);
-        assert!(*node.closed.borrow());
     }
 
     #[test]
-    fn generate_successor_pruned_by_constraint() {
-        let mut name_to_integer_resource_variable = FxHashMap::default();
-        name_to_integer_resource_variable.insert(String::from("v1"), 0);
-        name_to_integer_resource_variable.insert(String::from("v2"), 1);
-
-        let model = Rc::new(Model {
-            state_metadata: StateMetadata {
-                integer_resource_variable_names: vec![String::from("v1"), String::from("v2")],
-                name_to_integer_resource_variable,
-                integer_less_is_better: vec![false, false],
-                ..Default::default()
-            },
-            state_constraints: vec![GroundedCondition {
-                condition: Condition::ComparisonI(
-                    ComparisonOperator::Le,
-                    Box::new(IntegerExpression::ResourceVariable(0)),
-                    Box::new(IntegerExpression::Constant(0)),
-                ),
-                ..Default::default()
-            }],
-            target: State {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![0, 0],
-                    ..Default::default()
-                },
-                ..Default::default()
-            },
-            reduce_function: ReduceFunction::Min,
-            ..Default::default()
+    fn add_set_effect_type_err() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_set_variable("v", ob, Set::with_capacity(10));
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Set(SetVarPy::from(v));
+            let expr = IntExprPy::from(IntegerExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
         });
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 1;
-
-        let node = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert!(node.is_some());
-        let (node, _, _) = node.unwrap();
-
-        let transition = Rc::new(Transition {
-            name: String::from("increase"),
-            effect: Effect {
-                integer_resource_effects: vec![
-                    (
-                        0,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(0)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                    (
-                        1,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(1)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                ],
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_set_effect_duplicate_err() {
+        let mut model = Model::default();
+        let ob = model.add_object_type("something", 10);
+        assert!(ob.is_ok());
+        let ob = ob.unwrap();
+        let v = model.add_set_variable("v", ob, Set::with_capacity(10));
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition {
+            effect: dypdl::Effect {
+                set_effects: vec![(
+                    v.id(),
+                    SetExpression::Reference(ReferenceExpression::Constant(Set::with_capacity(10))),
+                )],
                 ..Default::default()
             },
-            cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(1)),
-            )),
             ..Default::default()
         });
-        let result =
-            node.generate_successor(transition, &mut registry, h_evaluator, f_evaluator, None);
-        assert_eq!(result, None);
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Set(SetVarPy::from(v));
+            let expr = SetConstPy::from(Set::with_capacity(10)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_err());
     }
 
     #[test]
-    fn generate_successor_pruned_by_h() {
-        let mut name_to_integer_resource_variable = FxHashMap::default();
-        name_to_integer_resource_variable.insert(String::from("v1"), 0);
-        name_to_integer_resource_variable.insert(String::from("v2"), 1);
-
-        let model = Rc::new(Model {
-            state_metadata: StateMetadata {
-                integer_resource_variable_names: vec![String::from("v1"), String::from("v2")],
-                name_to_integer_resource_variable,
-                integer_less_is_better: vec![false, false],
-                ..Default::default()
-            },
-            target: State {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![0, 0],
+    fn add_int_effect_ok() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable("v", 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Int(IntVarPy::from(v));
+            let expr = IntExprPy::from(IntegerExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_ok());
+        assert_eq!(
+            transition,
+            TransitionPy(Transition {
+                effect: dypdl::Effect {
+                    integer_effects: vec![(v.id(), IntegerExpression::Constant(0))],
                     ..Default::default()
                 },
                 ..Default::default()
-            },
-            reduce_function: ReduceFunction::Min,
-            ..Default::default()
+            })
+        );
+    }
+
+    #[test]
+    fn add_int_effect_type_err() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable("v", 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Int(IntVarPy::from(v));
+            let expr = ElementExprPy::from(ElementExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
         });
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 1;
-
-        let node = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert!(node.is_some());
-        let (node, _, _) = node.unwrap();
-
-        let transition = Rc::new(Transition {
-            name: String::from("increase"),
-            effect: Effect {
-                integer_resource_effects: vec![
-                    (
-                        0,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(0)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                    (
-                        1,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(1)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                ],
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_int_effect_duplicate_err() {
+        let mut model = Model::default();
+        let v = model.add_integer_variable("v", 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition {
+            effect: dypdl::Effect {
+                integer_effects: vec![(v.id(), IntegerExpression::Constant(0))],
                 ..Default::default()
             },
-            cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(1)),
-            )),
             ..Default::default()
         });
-        let h_evaluator = |_: &StateInRegistry, _: &Model| None;
-        let result =
-            node.generate_successor(transition, &mut registry, h_evaluator, f_evaluator, None);
-        assert_eq!(result, None);
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Int(IntVarPy::from(v));
+            let expr = IntExprPy::from(IntegerExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_err());
     }
 
     #[test]
-    fn generate_successor_pruned_by_bound() {
-        let mut name_to_integer_resource_variable = FxHashMap::default();
-        name_to_integer_resource_variable.insert(String::from("v1"), 0);
-        name_to_integer_resource_variable.insert(String::from("v2"), 1);
-
-        let model = Rc::new(Model {
-            state_metadata: StateMetadata {
-                integer_resource_variable_names: vec![String::from("v1"), String::from("v2")],
-                name_to_integer_resource_variable,
-                integer_less_is_better: vec![false, false],
-                ..Default::default()
-            },
-            target: State {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![0, 0],
+    fn add_int_resource_effect_ok() {
+        let mut model = Model::default();
+        let v = model.add_integer_resource_variable("v", false, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::IntResource(IntResourceVarPy::from(v));
+            let expr = IntExprPy::from(IntegerExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_ok());
+        assert_eq!(
+            transition,
+            TransitionPy(Transition {
+                effect: dypdl::Effect {
+                    integer_resource_effects: vec![(v.id(), IntegerExpression::Constant(0))],
                     ..Default::default()
                 },
                 ..Default::default()
-            },
-            reduce_function: ReduceFunction::Min,
-            ..Default::default()
+            })
+        );
+    }
+
+    #[test]
+    fn add_int_resource_effect_type_err() {
+        let mut model = Model::default();
+        let v = model.add_integer_resource_variable("v", false, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::IntResource(IntResourceVarPy::from(v));
+            let expr = ElementExprPy::from(ElementExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
         });
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 1;
-
-        let node = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert!(node.is_some());
-        let (node, _, _) = node.unwrap();
-
-        let transition = Rc::new(Transition {
-            name: String::from("increase"),
-            effect: Effect {
-                integer_resource_effects: vec![
-                    (
-                        0,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(0)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                    (
-                        1,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(1)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                ],
+        assert!(result.is_err());
+    }
+
+    #[test]
+    fn add_int_resource_effect_duplicate_err() {
+        let mut model = Model::default();
+        let v = model.add_integer_resource_variable("v", false, 0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition {
+            effect: dypdl::Effect {
+                integer_resource_effects: vec![(v.id(), IntegerExpression::Constant(0))],
                 ..Default::default()
             },
-            cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(1)),
-            )),
             ..Default::default()
         });
-        let result =
-            node.generate_successor(transition, &mut registry, h_evaluator, f_evaluator, Some(1));
-        assert_eq!(result, None);
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::IntResource(IntResourceVarPy::from(v));
+            let expr = IntExprPy::from(IntegerExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_err());
     }
 
     #[test]
-    fn generate_successor_dominated() {
-        let mut name_to_integer_resource_variable = FxHashMap::default();
-        name_to_integer_resource_variable.insert(String::from("v1"), 0);
-        name_to_integer_resource_variable.insert(String::from("v2"), 1);
-
-        let model = Rc::new(Model {
-            state_metadata: StateMetadata {
-                integer_resource_variable_names: vec![String::from("v1"), String::from("v2")],
-                name_to_integer_resource_variable,
-                integer_less_is_better: vec![true, true],
-                ..Default::default()
-            },
-            target: State {
-                resource_variables: ResourceVariables {
-                    integer_variables: vec![0, 0],
+    fn add_float_effect_ok() {
+        let mut model = Model::default();
+        let v = model.add_continuous_variable("v", 0.0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Float(FloatVarPy::from(v));
+            let expr = FloatExprPy::from(ContinuousExpression::Constant(0.0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_ok());
+        assert_eq!(
+            transition,
+            TransitionPy(Transition {
+                effect: dypdl::Effect {
+                    continuous_effects: vec![(v.id(), ContinuousExpression::Constant(0.0))],
                     ..Default::default()
                 },
                 ..Default::default()
-            },
-            reduce_function: ReduceFunction::Min,
-            ..Default::default()
-        });
-        let mut registry = StateRegistry::new(model);
-        let h_evaluator = |_: &StateInRegistry, _: &Model| Some(1);
-        let f_evaluator = |_, _, _: &StateInRegistry, _: &Model| 1;
-
-        let node = FNode::generate_initial_node(&mut registry, h_evaluator, f_evaluator);
-        assert!(node.is_some());
-        let (node, _, _) = node.unwrap();
-
-        let transition = Rc::new(Transition {
-            name: String::from("increase"),
-            effect: Effect {
-                integer_resource_effects: vec![
-                    (
-                        0,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(0)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                    (
-                        1,
-                        IntegerExpression::BinaryOperation(
-                            BinaryOperator::Add,
-                            Box::new(IntegerExpression::ResourceVariable(1)),
-                            Box::new(IntegerExpression::Constant(1)),
-                        ),
-                    ),
-                ],
-                ..Default::default()
-            },
-            cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(1)),
-            )),
-            ..Default::default()
-        });
-        let result =
-            node.generate_successor(transition, &mut registry, h_evaluator, f_evaluator, None);
-        assert_eq!(result, None);
+            })
+        );
     }
 
     #[test]
-    fn node_close() {
-        let node = FNode::<i32> {
-            closed: RefCell::new(false),
-            ..Default::default()
-        };
-        assert!(!node.closed());
-        node.close();
-        assert!(node.closed());
+    fn add_float_effect_type_err() {
+        let mut model = Model::default();
+        let v = model.add_continuous_variable("v", 0.0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Float(FloatVarPy::from(v));
+            let expr = ElementExprPy::from(ElementExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_err());
     }
 
     #[test]
-    fn node_no_transition() {
-        let node = FNode::<i32> {
-            transitions: None,
+    fn add_float_effect_duplicate_err() {
+        let mut model = Model::default();
+        let v = model.add_continuous_variable("v", 0.0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition {
+            effect: dypdl::Effect {
+                continuous_effects: vec![(v.id(), ContinuousExpression::Constant(0.0))],
+                ..Default::default()
+            },
             ..Default::default()
-        };
-        assert_eq!(node.transitions(), vec![]);
+        });
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::Float(FloatVarPy::from(v));
+            let expr = FloatExprPy::from(ContinuousExpression::Constant(0.0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_err());
     }
 
     #[test]
-    fn node_transitions() {
-        let parent = Rc::new(TransitionChain::new(
-            None,
-            Rc::new(Transition {
-                name: String::from("t1"),
-                ..Default::default()
-            }),
-        ));
+    fn add_float_resource_effect_ok() {
+        let mut model = Model::default();
+        let v = model.add_continuous_resource_variable("v", false, 0.0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
 
-        let node = FNode::<i32> {
-            transitions: Some(Rc::new(TransitionChain::new(
-                Some(parent),
-                Rc::new(Transition {
-                    name: String::from("t2"),
-                    ..Default::default()
-                }),
-            ))),
-            ..Default::default()
-        };
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::FloatResource(FloatResourceVarPy::from(v));
+            let expr = FloatExprPy::from(ContinuousExpression::Constant(0.0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_ok());
         assert_eq!(
-            node.transitions(),
-            vec![
-                Transition {
-                    name: String::from("t1"),
+            transition,
+            TransitionPy(Transition {
+                effect: dypdl::Effect {
+                    continuous_resource_effects: vec![(
+                        v.id(),
+                        ContinuousExpression::Constant(0.0)
+                    )],
                     ..Default::default()
                 },
-                Transition {
-                    name: String::from("t2"),
-                    ..Default::default()
-                },
-            ]
+                ..Default::default()
+            })
         );
     }
 
     #[test]
-    fn get_bound_minimization() {
-        let model = Rc::new(Model {
-            reduce_function: ReduceFunction::Min,
-            ..Default::default()
+    fn add_float_resource_effect_type_err() {
+        let mut model = Model::default();
+        let v = model.add_continuous_resource_variable("v", false, 0.0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition::default());
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::FloatResource(FloatResourceVarPy::from(v));
+            let expr = ElementExprPy::from(ElementExpression::Constant(0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
         });
-        let node = FNode {
-            f: -1,
-            ..Default::default()
-        };
-        assert_eq!(node.get_bound(&model), 1);
+        assert!(result.is_err());
     }
 
     #[test]
-    fn get_bound_maximization() {
-        let model = Rc::new(Model {
-            reduce_function: ReduceFunction::Max,
+    fn add_float_resource_effect_duplicate_err() {
+        let mut model = Model::default();
+        let v = model.add_continuous_resource_variable("v", false, 0.0);
+        assert!(v.is_ok());
+        let v = v.unwrap();
+
+        let mut transition = TransitionPy(Transition {
+            effect: dypdl::Effect {
+                continuous_resource_effects: vec![(v.id(), ContinuousExpression::Constant(0.0))],
+                ..Default::default()
+            },
             ..Default::default()
         });
-        let node = FNode {
-            f: 1,
-            ..Default::default()
-        };
-        assert_eq!(node.get_bound(&model), 1);
+        let result = Python::with_gil(|py| {
+            let v = VarUnion::FloatResource(FloatResourceVarPy::from(v));
+            let expr = FloatExprPy::from(ContinuousExpression::Constant(0.0)).into_py(py);
+            transition.add_effect(v, expr.as_ref(py))
+        });
+        assert!(result.is_err());
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/hashable_state.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/hashable_state.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/successor_generator.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/successor_generator.rs`

 * *Files 20% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 /// Generator of applicable transitions.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::*;
+/// use dypdl_heuristic_search::search_algorithm::SuccessorGenerator;
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 ///
 /// let mut increment = Transition::new("increment");
 /// increment.add_effect(variable, variable + 1).unwrap();
@@ -161,72 +161,49 @@
             iter: self.forced_transitions.iter(),
             forced: true,
             end: false,
         }
     }
 }
 
-impl<T, U, R> SuccessorGenerator<T, U, R>
+impl<U, R> SuccessorGenerator<Transition, U, R>
 where
-    T: TransitionInterface,
-    U: Deref<Target = T> + Clone,
-    R: Deref<Target = dypdl::Model>,
-{
-    /// Returns a new successor generator.
-    pub fn new(
-        forced_transitions: Vec<U>,
-        transitions: Vec<U>,
-        backward: bool,
-        model: R,
-    ) -> SuccessorGenerator<T, U, R> {
-        SuccessorGenerator {
-            forced_transitions,
-            transitions,
-            backward,
-            model,
-        }
-    }
-}
-
-impl<T, U, R> SuccessorGenerator<T, U, R>
-where
-    T: TransitionInterface + From<Transition>,
-    U: Deref<Target = T> + Clone + From<T>,
+    U: Deref<Target = Transition> + Clone + From<Transition>,
     R: Deref<Target = dypdl::Model>,
 {
     /// Returns a successor generator given a model and the direction.
-    pub fn from_model(model: R, backward: bool) -> SuccessorGenerator<T, U, R> {
+    pub fn from_model(model: R, backward: bool) -> Self {
         let forced_transitions = if backward {
             &model.backward_forced_transitions
         } else {
             &model.forward_forced_transitions
         };
-        let forced_transitions = forced_transitions
-            .iter()
-            .map(|t| U::from(T::from(t.clone())))
-            .collect();
+        let forced_transitions = forced_transitions.iter().cloned().map(U::from).collect();
 
         let transitions = if backward {
             &model.backward_transitions
         } else {
             &model.forward_transitions
         };
-        let transitions = transitions
-            .iter()
-            .map(|t| U::from(T::from(t.clone())))
-            .collect();
+        let transitions = transitions.iter().cloned().map(U::from).collect();
 
-        SuccessorGenerator::new(forced_transitions, transitions, backward, model)
+        SuccessorGenerator {
+            forced_transitions,
+            transitions,
+            backward,
+            model,
+        }
     }
 }
 
 #[cfg(test)]
 mod tests {
     use super::*;
     use dypdl::expression::*;
+    use dypdl::prelude::*;
     use dypdl::GroundedCondition;
     use rustc_hash::FxHashMap;
     use std::rc::Rc;
 
     fn generate_model() -> dypdl::Model {
         dypdl::Model {
             state_metadata: dypdl::StateMetadata {
@@ -470,8 +447,92 @@
         let mut transitions = generator.applicable_transitions(&state);
         assert_eq!(
             transitions.next(),
             Some(Rc::new(model.backward_forced_transitions[1].clone()))
         );
         assert_eq!(transitions.next(), None);
     }
+
+    #[test]
+    fn from_model_forward() {
+        let mut model = Model::default();
+        let mut transition1 = Transition::new("transition1");
+        transition1.set_cost(IntegerExpression::Cost + 1);
+        let result = model.add_forward_transition(transition1.clone());
+        assert!(result.is_ok());
+        let mut transition2 = Transition::new("transition2");
+        transition2.set_cost(IntegerExpression::Cost + 2);
+        let result = model.add_forward_transition(transition2.clone());
+        assert!(result.is_ok());
+        let mut transition3 = Transition::new("transition3");
+        transition3.set_cost(IntegerExpression::Cost + 3);
+        let result = model.add_forward_forced_transition(transition3.clone());
+        assert!(result.is_ok());
+        let mut transition4 = Transition::new("transition4");
+        transition4.set_cost(IntegerExpression::Cost + 4);
+        let result = model.add_forward_forced_transition(transition4.clone());
+        assert!(result.is_ok());
+        let mut transition5 = Transition::new("transition5");
+        transition5.set_cost(IntegerExpression::Cost + 5);
+        let result = model.add_backward_transition(transition5.clone());
+        assert!(result.is_ok());
+        let mut transition6 = Transition::new("transition6");
+        transition6.set_cost(IntegerExpression::Cost + 6);
+        let result = model.add_backward_forced_transition(transition6.clone());
+        assert!(result.is_ok());
+        let model = Rc::new(model);
+
+        let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+
+        assert_eq!(generator.model, model);
+        assert_eq!(
+            generator.transitions,
+            vec![Rc::new(transition1,), Rc::new(transition2,),]
+        );
+        assert_eq!(
+            generator.forced_transitions,
+            vec![Rc::new(transition3,), Rc::new(transition4,),]
+        );
+    }
+
+    #[test]
+    fn from_model_backward() {
+        let mut model = Model::default();
+        let mut transition1 = Transition::new("transition1");
+        transition1.set_cost(IntegerExpression::Cost + 1);
+        let result = model.add_backward_transition(transition1.clone());
+        assert!(result.is_ok());
+        let mut transition2 = Transition::new("transition2");
+        transition2.set_cost(IntegerExpression::Cost + 2);
+        let result = model.add_backward_transition(transition2.clone());
+        assert!(result.is_ok());
+        let mut transition3 = Transition::new("transition3");
+        transition3.set_cost(IntegerExpression::Cost + 3);
+        let result = model.add_backward_forced_transition(transition3.clone());
+        assert!(result.is_ok());
+        let mut transition4 = Transition::new("transition4");
+        transition4.set_cost(IntegerExpression::Cost + 4);
+        let result = model.add_backward_forced_transition(transition4.clone());
+        assert!(result.is_ok());
+        let mut transition5 = Transition::new("transition5");
+        transition5.set_cost(IntegerExpression::Cost + 5);
+        let result = model.add_forward_transition(transition5.clone());
+        assert!(result.is_ok());
+        let mut transition6 = Transition::new("transition6");
+        transition6.set_cost(IntegerExpression::Cost + 6);
+        let result = model.add_forward_forced_transition(transition6.clone());
+        assert!(result.is_ok());
+        let model = Rc::new(model);
+
+        let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), true);
+
+        assert_eq!(generator.model, model);
+        assert_eq!(
+            generator.transitions,
+            vec![Rc::new(transition1,), Rc::new(transition2,),]
+        );
+        assert_eq!(
+            generator.forced_transitions,
+            vec![Rc::new(transition3,), Rc::new(transition4,),]
+        );
+    }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_chain.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_chain.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 use core::ops::Deref;
 use dypdl::{Transition, TransitionInterface};
 use std::rc::Rc;
 
+/// Trait to get a sequence of transitions.
+pub trait GetTransitions<V = Transition> {
+    /// Returns transitions to reach this node.
+    fn transitions(&self) -> Vec<V>;
+}
+
 /// Chain of transitions.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
 /// use dypdl_heuristic_search::search_algorithm::data_structure::{
-///     TransitionChainInterface, TransitionChain
+///     RcChain, TransitionChain
 /// };
 /// use std::rc::Rc;
 ///
 /// let t1 = Transition::new("t1");
-/// let chain = Rc::new(TransitionChain::new(None, Rc::new(t1.clone())));
+/// let chain = Rc::new(RcChain::new(None, Rc::new(t1.clone())));
 /// assert_eq!(chain.last(), &t1);
 /// assert_eq!(chain.parent(), None);
 /// assert_eq!(chain.transitions(), vec![t1.clone()]);
 ///
 /// let t2 = Transition::new("t2");
-/// let new_chain = Rc::new(TransitionChain::new(Some(chain.clone()), Rc::new(t2.clone())));
+/// let new_chain = Rc::new(RcChain::new(Some(chain.clone()), Rc::new(t2.clone())));
 /// assert_eq!(new_chain.last(), &t2);
 /// assert_eq!(new_chain.parent(), Some(&chain));
 /// assert_eq!(new_chain.transitions(), vec![t1, t2]);
 /// ```
-pub trait TransitionChainInterface<T = Transition, R = Rc<T>, P = Rc<Self>>
+pub trait TransitionChain<T = Transition, R = Rc<T>, P = Rc<Self>>
 where
     T: TransitionInterface + Clone,
     R: Deref<Target = T>,
     P: Deref<Target = Self>,
     Transition: From<T>,
 {
     /// Returns a new transition chain.
@@ -54,25 +60,33 @@
         result.reverse();
         result
     }
 }
 
 /// Chain of transitions implemented by a linked list of `Rc`.
 #[derive(PartialEq, Debug)]
-pub struct TransitionChain {
+pub struct RcChain<T = Transition>
+where
+    T: TransitionInterface + Clone,
+    Transition: From<T>,
+{
     parent: Option<Rc<Self>>,
-    last: Rc<Transition>,
+    last: Rc<T>,
 }
 
-impl TransitionChainInterface for TransitionChain {
-    fn new(parent: Option<Rc<Self>>, last: Rc<Transition>) -> Self {
+impl<T> TransitionChain<T> for RcChain<T>
+where
+    T: TransitionInterface + Clone,
+    Transition: From<T>,
+{
+    fn new(parent: Option<Rc<Self>>, last: Rc<T>) -> Self {
         Self { parent, last }
     }
 
-    fn last(&self) -> &Transition {
+    fn last(&self) -> &T {
         &self.last
     }
 
     fn parent(&self) -> Option<&Rc<Self>> {
         self.parent.as_ref()
     }
 }
@@ -83,45 +97,45 @@
 
     #[test]
     fn new_no_parent() {
         let op1 = Rc::new(dypdl::Transition {
             name: String::from("op1"),
             ..Default::default()
         });
-        let chain = TransitionChain::new(None, op1.clone());
+        let chain = RcChain::new(None, op1.clone());
         assert_eq!(chain.parent(), None);
         assert_eq!(chain.last(), &*op1);
     }
 
     #[test]
     fn new_with_parent() {
         let op1 = Rc::new(dypdl::Transition {
             name: String::from("op1"),
             ..Default::default()
         });
-        let chain1 = Rc::new(TransitionChain::new(None, op1));
+        let chain1 = Rc::new(RcChain::new(None, op1));
         let op2 = Rc::new(dypdl::Transition {
             name: String::from("op2"),
             ..Default::default()
         });
-        let chain2 = TransitionChain::new(Some(chain1.clone()), op2.clone());
+        let chain2 = RcChain::new(Some(chain1.clone()), op2.clone());
         assert_eq!(chain2.parent(), Some(&chain1));
         assert_eq!(chain2.last(), &*op2);
     }
 
     #[test]
     fn trace_transitions_test() {
         let op1 = dypdl::Transition {
             name: String::from("op1"),
             ..Default::default()
         };
-        let chain1 = Rc::new(TransitionChain::new(None, Rc::new(op1.clone())));
+        let chain1 = Rc::new(RcChain::new(None, Rc::new(op1.clone())));
         let op2 = dypdl::Transition {
             name: String::from("op2"),
             ..Default::default()
         };
-        let chain2 = Rc::new(TransitionChain::new(Some(chain1), Rc::new(op2.clone())));
+        let chain2 = Rc::new(RcChain::new(Some(chain1), Rc::new(op2.clone())));
         let result = chain2.transitions();
         let expected = vec![op1, op2];
         assert_eq!(result, expected);
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/transition_with_custom_cost.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/rollout.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,807 +1,848 @@
-use super::hashable_state::HashableSignatureVariables;
-use super::prioritized_node::PrioritizedNode;
-use super::state_registry::{StateInRegistry, StateInformation};
-use super::successor_generator::SuccessorGenerator;
-use super::transition_chain::TransitionChainInterface;
-use core::ops::Deref;
+use super::data_structure::StateInformation;
+use super::StateInRegistry;
 use dypdl::variable_type::Numeric;
-use dypdl::{CostExpression, StateInterface, Transition, TransitionInterface};
+use dypdl::{Model, State, StateInterface, TransitionInterface};
 use std::fmt::Debug;
 use std::hash::Hash;
-use std::rc::Rc;
 
-/// Transition with a customized cost expression.
-#[derive(Debug, PartialEq, Clone, Default)]
-pub struct TransitionWithCustomCost {
-    /// Transition.
-    pub transition: Transition,
-    /// Customized cost expression.
-    pub custom_cost: CostExpression,
-    /// If forced.
-    pub forced: bool,
-    /// ID.
-    pub id: usize,
+/// Result of a rollout.
+#[derive(PartialEq, Clone, Debug)]
+pub struct RolloutResult<'a, S, U, T>
+where
+    S: StateInterface + From<State>,
+    U: Numeric,
+    T: TransitionInterface,
+{
+    /// State resulting from the rollout.
+    /// None if no transition is applied.
+    pub state: Option<S>,
+    /// Cost.
+    pub cost: U,
+    /// Transitions applied.
+    pub transitions: &'a [T],
+    /// If a base case is reached.
+    pub is_base: bool,
 }
 
-impl TransitionInterface for TransitionWithCustomCost {
-    #[inline]
-    fn is_applicable<S: dypdl::StateInterface>(
-        &self,
-        state: &S,
-        registry: &dypdl::TableRegistry,
-    ) -> bool {
-        self.transition.is_applicable(state, registry)
-    }
-
-    #[inline]
-    fn apply<S: dypdl::StateInterface, T: From<dypdl::State>>(
-        &self,
-        state: &S,
-        registry: &dypdl::TableRegistry,
-    ) -> T {
-        self.transition.apply(state, registry)
-    }
-
-    #[inline]
-    fn eval_cost<U: Numeric, T: dypdl::StateInterface>(
-        &self,
-        cost: U,
-        state: &T,
-        registry: &dypdl::TableRegistry,
-    ) -> U {
-        self.transition.eval_cost(cost, state, registry)
+/// Returns the result of a rollout.
+///
+/// Returns `None` if the rollout fails,
+/// e.g., if a transition is not applicable or a state constraint is violated.
+///
+/// # Panics
+///
+/// If expressions in the model or transitions are invalid.
+///
+/// # Examples
+///
+/// ```
+/// use dypdl::prelude::*;
+/// use dypdl_heuristic_search::search_algorithm::rollout;
+///
+/// let mut model = Model::default();
+/// let variable = model.add_integer_variable("variable", 1).unwrap();
+/// model.add_state_constraint(
+///     Condition::comparison_i(ComparisonOperator::Ne, variable, 3)
+/// ).unwrap();
+/// model.add_base_case(
+///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 4)]
+/// ).unwrap();
+/// let state = model.target.clone();
+///
+/// let mut increment = Transition::new("increment");
+/// increment.set_cost(IntegerExpression::Cost + 2);
+/// increment.add_effect(variable, variable + 1).unwrap();
+///
+/// let mut double = Transition::new("increment");
+/// double.set_cost(IntegerExpression::Cost + 3);
+/// double.add_effect(variable, variable * 2).unwrap();
+///
+/// let transitions = [increment.clone(), double.clone(), increment.clone()];
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let expected_state: State = increment.apply(&state, &model.table_registry);
+/// let expected_state: State = double.apply(&expected_state, &model.table_registry);
+/// let result = rollout(&state, 0, &transitions, &base_cost_evaluator, &model).unwrap();
+/// assert_eq!(result.state, Some(expected_state));
+/// assert_eq!(result.cost, 5);
+/// assert_eq!(result.transitions, &transitions[..2]);
+/// assert!(result.is_base);
+///
+/// let transitions = [double.clone(), increment.clone()];
+/// assert_eq!(rollout(&state, 0, &transitions, base_cost_evaluator, &model), None);
+/// ```
+pub fn rollout<'a, S, U, T, B>(
+    state: &S,
+    cost: U,
+    transitions: &'a [T],
+    base_cost_evaluator: B,
+    model: &Model,
+) -> Option<RolloutResult<'a, S, U, T>>
+where
+    S: StateInterface + From<State>,
+    U: Numeric + Ord,
+    T: TransitionInterface,
+    B: Fn(U, U) -> U,
+{
+    if let Some(base_cost) = model.eval_base_cost(state) {
+        return Some(RolloutResult {
+            state: None,
+            cost: base_cost_evaluator(cost, base_cost),
+            transitions: &transitions[..0],
+            is_base: true,
+        });
     }
-}
 
-impl From<TransitionWithCustomCost> for Transition {
-    fn from(transition: TransitionWithCustomCost) -> Self {
-        transition.transition
-    }
-}
+    let mut current_state;
+    let mut parent_state = state;
+    let mut cost = cost;
+
+    for (i, t) in transitions.iter().enumerate() {
+        if !t.is_applicable(parent_state, &model.table_registry) {
+            return None;
+        }
 
-impl<U, R> SuccessorGenerator<TransitionWithCustomCost, U, R>
-where
-    U: Deref<Target = TransitionWithCustomCost> + Clone + From<TransitionWithCustomCost>,
-    R: Deref<Target = dypdl::Model>,
-{
-    /// Returns a successor generator given a model and the direction.
-    pub fn from_model_without_custom_cost(
-        model: R,
-        backward: bool,
-    ) -> SuccessorGenerator<TransitionWithCustomCost, U, R> {
-        let forced_transitions = if backward {
-            &model.backward_forced_transitions
-        } else {
-            &model.forward_forced_transitions
-        };
-        let forced_transitions = forced_transitions
-            .iter()
-            .enumerate()
-            .map(|(id, t)| {
-                U::from(TransitionWithCustomCost {
-                    transition: t.clone(),
-                    custom_cost: t.cost.clone(),
-                    forced: true,
-                    id,
-                })
-            })
-            .collect();
+        let state = t.apply(parent_state, &model.table_registry);
 
-        let transitions = if backward {
-            &model.backward_transitions
-        } else {
-            &model.forward_transitions
-        };
-        let transitions = transitions
-            .iter()
-            .enumerate()
-            .map(|(id, t)| {
-                U::from(TransitionWithCustomCost {
-                    transition: t.clone(),
-                    custom_cost: t.cost.clone(),
-                    forced: false,
-                    id,
-                })
-            })
-            .collect();
+        if !model.check_constraints(&state) {
+            return None;
+        }
 
-        SuccessorGenerator::new(forced_transitions, transitions, backward, model)
-    }
+        cost = t.eval_cost(cost, parent_state, &model.table_registry);
 
-    /// Returns a successor generator returning applicable transitions with customized cost expressions.
-    pub fn from_model_with_custom_costs(
-        model: R,
-        custom_costs: &[CostExpression],
-        forced_custom_costs: &[CostExpression],
-        backward: bool,
-    ) -> SuccessorGenerator<TransitionWithCustomCost, U, R> {
-        let forced_transitions = if backward {
-            &model.backward_forced_transitions
-        } else {
-            &model.forward_forced_transitions
-        };
-        let forced_transitions = forced_transitions
-            .iter()
-            .enumerate()
-            .zip(forced_custom_costs)
-            .map(|((id, t), c)| {
-                U::from(TransitionWithCustomCost {
-                    transition: t.clone(),
-                    custom_cost: c.simplify(&model.table_registry),
-                    forced: true,
-                    id,
-                })
-            })
-            .collect();
+        if let Some(base_cost) = model.eval_base_cost(&state) {
+            return Some(RolloutResult {
+                state: Some(state),
+                cost: base_cost_evaluator(cost, base_cost),
+                transitions: &transitions[..i + 1],
+                is_base: true,
+            });
+        }
 
-        let transitions = if backward {
-            &model.backward_transitions
-        } else {
-            &model.forward_transitions
-        };
-        let transitions = transitions
-            .iter()
-            .enumerate()
-            .zip(custom_costs)
-            .map(|((id, t), c)| {
-                U::from(TransitionWithCustomCost {
-                    transition: t.clone(),
-                    custom_cost: c.simplify(&model.table_registry),
-                    forced: false,
-                    id,
-                })
-            })
-            .collect();
-        SuccessorGenerator::new(forced_transitions, transitions, backward, model)
+        if i == transitions.len() - 1 {
+            return Some(RolloutResult {
+                state: Some(state),
+                cost,
+                transitions,
+                is_base: false,
+            });
+        }
+
+        current_state = state;
+        parent_state = &current_state;
     }
-}
 
-/// Parent information to generate a successor using a transition with a custom cost.
-#[derive(Clone)]
-pub struct CustomCostParent<'a, T: Numeric, U: Numeric, S: StateInterface = StateInRegistry> {
-    /// State.
-    pub state: &'a S,
-    /// Cost.
-    pub cost: T,
-    /// g-value.
-    pub g: U,
+    Some(RolloutResult {
+        state: None,
+        cost,
+        transitions,
+        is_base: false,
+    })
 }
 
-impl TransitionWithCustomCost {
-    /// Returns the successor state, its cost, g-value, and f-value.
-    ///
-    /// The successor is not generated if the `h_evaluator` returns `None`.
-    /// The `f_evaluator` takes the g- and h-values as input in addition to the state and the model.
-    ///
-    /// # Examples
-    ///
-    /// ```
-    /// use dypdl::prelude::*;
-    /// use dypdl_heuristic_search::search_algorithm::data_structure::{
-    ///     CustomCostParent, TransitionWithCustomCost
-    /// };
-    ///
-    /// let mut model = Model::default();
-    /// let variable = model.add_integer_variable("variable", 1).unwrap();
-    /// let state = model.target.clone();
-    ///
-    /// let mut transition = Transition::new("transition");
-    /// transition.set_cost(IntegerExpression::Cost + 1);
-    /// transition.add_effect(variable, variable + 1);
-    /// let transition = TransitionWithCustomCost {
-    ///     transition,
-    ///     custom_cost: CostExpression::from(ContinuousExpression::Cost + 1.5),
-    ///     forced: false,
-    ///     id: 0,
-    /// };
-    ///
-    /// let parent = CustomCostParent { state: &state, cost: 0, g: 0.0 };
-    /// let h_evaluator = |_: &_, _: &_| Some(0.0);
-    /// let f_evaluator = |g, h, _: &_, _: &_| g + h;
-    /// let expected_state = transition.apply(parent.state, &model.table_registry);
-    /// let result = transition.generate_successor_state(
-    ///     &parent, &model, None, h_evaluator, f_evaluator, false
-    /// );
-    /// assert_eq!(result, Some((expected_state, 1, 1.5, 1.5)));
-    /// ```
-    pub fn generate_successor_state<T, U, S, H, F>(
-        &self,
-        parent: &CustomCostParent<'_, T, U, S>,
-        model: &dypdl::Model,
-        bound: Option<U>,
-        h_evaluator: H,
-        f_evaluator: F,
-        maximize: bool,
-    ) -> Option<(S, T, U, U)>
-    where
-        T: Numeric,
-        U: Numeric,
-        S: StateInterface + From<dypdl::State>,
-        H: Fn(&S, &dypdl::Model) -> Option<U>,
-        F: Fn(U, U, &S, &dypdl::Model) -> U,
-    {
-        let state = self.apply(parent.state, &model.table_registry);
-
-        if model.check_constraints(&state) {
-            let g = self
-                .custom_cost
-                .eval_cost(parent.g, parent.state, &model.table_registry);
-            let h = h_evaluator(&state, model)?;
-            let f = f_evaluator(g, h, &state, model);
-
-            if bound.map_or(false, |bound| {
-                (maximize && f <= bound) || (!maximize && f >= bound)
-            }) {
-                return None;
-            }
-
-            let cost = self.eval_cost(parent.cost, parent.state, &model.table_registry);
-
-            Some((state, cost, g, f))
-        } else {
-            None
-        }
+/// Get the solution cost and suffix if the rollout of the transitions from the node succeeds.
+///
+/// # Panics
+///
+/// If expressions in the model or transitions are invalid.
+///
+/// # Examples
+///
+/// ```
+/// use dypdl::prelude::*;
+/// use dypdl_heuristic_search::Solution;
+/// use dypdl_heuristic_search::search_algorithm::{
+///     FNode, StateInRegistry, get_solution_cost_and_suffix,
+/// };
+/// use dypdl_heuristic_search::search_algorithm::data_structure::GetTransitions;
+/// use dypdl_heuristic_search::search_algorithm::util::update_solution;
+/// use std::rc::Rc;
+///
+/// let mut model = Model::default();
+/// let var = model.add_integer_variable("var", 0).unwrap();
+/// model.add_base_case(vec![Condition::comparison_i(ComparisonOperator::Ge, var, 3)]).unwrap();
+///
+/// let mut transition = Transition::new("transition");
+/// transition.add_effect(var, var + 1).unwrap();
+/// transition.set_cost(IntegerExpression::Cost + 1);
+///
+/// let h_evaluator = |_: &StateInRegistry| Some(0);
+/// let f_evaluator = |g, h, _: &StateInRegistry| g + h;
+/// let node = FNode::generate_root_node(
+///     model.target.clone(), 0, &model, &h_evaluator, &f_evaluator, None,
+/// ).unwrap();
+/// let node = node.generate_successor_node(
+///     Rc::new(transition.clone()), &model, &h_evaluator, &f_evaluator, None,
+/// ).unwrap();
+///
+/// let suffix = [transition.clone(), transition.clone()];
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+/// let (cost, suffix) = get_solution_cost_and_suffix(
+///     &model, &node, &suffix, base_cost_evaluator,
+/// ).unwrap();
+///
+/// assert_eq!(cost, 3);
+/// assert_eq!(suffix, &[transition.clone(), transition]);
+/// ```
+pub fn get_solution_cost_and_suffix<'a, N, T, U, B, K>(
+    model: &Model,
+    node: &N,
+    transitions: &'a [T],
+    base_cost_evaluator: B,
+) -> Option<(U, &'a [T])>
+where
+    N: StateInformation<U, K>,
+    T: TransitionInterface,
+    U: Numeric + Ord,
+    B: Fn(U, U) -> U,
+    K: Hash + Eq + Clone + Debug,
+    StateInRegistry<K>: StateInterface + From<State>,
+{
+    let result = rollout(
+        node.state(),
+        node.cost(model),
+        transitions,
+        base_cost_evaluator,
+        model,
+    )?;
+
+    if result.is_base {
+        Some((result.cost, result.transitions))
+    } else {
+        None
     }
 }
 
-/// Chain of transitions with custom costs implemented by a linked list of `Rc`.
-#[derive(PartialEq, Debug)]
-pub struct TransitionWithCustomCostChain {
-    parent: Option<Rc<Self>>,
-    last: Rc<TransitionWithCustomCost>,
+/// Iterator returning the result of a transition trace.
+pub struct Trace<'a, S, U, T> {
+    state: S,
+    cost: U,
+    transitions: &'a [T],
+    model: &'a Model,
+    i: usize,
 }
 
-impl TransitionChainInterface<TransitionWithCustomCost> for TransitionWithCustomCostChain {
-    fn new(parent: Option<Rc<Self>>, last: Rc<TransitionWithCustomCost>) -> Self {
-        Self { parent, last }
-    }
+impl<'a, S, U, T> Iterator for Trace<'a, S, U, T>
+where
+    S: StateInterface + From<State> + Clone,
+    U: Numeric,
+    T: TransitionInterface,
+{
+    type Item = (S, U);
 
-    fn last(&self) -> &TransitionWithCustomCost {
-        &self.last
-    }
+    fn next(&mut self) -> Option<Self::Item> {
+        if self.i > self.transitions.len() {
+            return None;
+        }
+
+        let result = Some((self.state.clone(), self.cost));
+
+        if self.i < self.transitions.len() {
+            self.cost = self.transitions[self.i].eval_cost(
+                self.cost,
+                &self.state,
+                &self.model.table_registry,
+            );
+            self.state = self.transitions[self.i].apply(&self.state, &self.model.table_registry);
+        }
 
-    fn parent(&self) -> Option<&Rc<Self>> {
-        self.parent.as_ref()
+        self.i += 1;
+
+        result
     }
 }
 
-/// A trait to get an iterator of pointers to TransitionsWithCustomCost.
-pub trait CustomCostNodeInterface<
-    T: Numeric,
+/// Returns the states and costs of a rollout without checking state constraints and base cases.
+///
+/// # Panics
+///
+/// If `transitions` is empty.
+///
+/// # Examples
+///
+/// ```
+/// use dypdl::prelude::*;
+/// use dypdl_heuristic_search::search_algorithm::get_trace;
+///
+/// let mut model = Model::default();
+/// let variable = model.add_integer_variable("variable", 1).unwrap();
+/// let state = model.target.clone();
+///
+/// let mut increment = Transition::new("increment");
+/// increment.set_cost(IntegerExpression::Cost + 2);
+/// increment.add_effect(variable, variable + 1).unwrap();
+///
+/// let mut double = Transition::new("double");
+/// double.set_cost(IntegerExpression::Cost + 3);
+/// double.add_effect(variable, variable * 2).unwrap();
+///
+/// let transitions = [increment.clone(), double.clone()];
+/// let mut iter = get_trace(&state, 0, &transitions, &model);
+///
+/// let expected_state: State = increment.apply(&state, &model.table_registry);
+/// assert_eq!(iter.next(), Some((expected_state.clone(), 2)));
+///
+/// let expected_state: State = double.apply(&expected_state, &model.table_registry);
+/// assert_eq!(iter.next(), Some((expected_state, 5)));
+///
+/// assert_eq!(iter.next(), None);
+/// ```
+pub fn get_trace<'a, S, U, T>(
+    state: &S,
+    cost: U,
+    transitions: &'a [T],
+    model: &'a Model,
+) -> Trace<'a, S, U, T>
+where
+    S: StateInterface + From<State>,
     U: Numeric,
-    K: Hash + Eq + Clone + Debug = Rc<HashableSignatureVariables>,
-    R: Deref<Target = TransitionWithCustomCost> = Rc<TransitionWithCustomCost>,
->: StateInformation<T, K> + PrioritizedNode<U>
+    T: TransitionInterface,
 {
-    /// Create a new node given a g-value, an f-value, a state, a cost, a parent, and a transition.
-    fn new(
-        g: U,
-        f: U,
-        state: StateInRegistry<K>,
-        cost: T,
-        parent: Option<&Self>,
-        transition: Option<R>,
-    ) -> Self;
+    let cost = transitions[0].eval_cost(cost, state, &model.table_registry);
+    let state = transitions[0].apply(state, &model.table_registry);
 
-    /// Get transitions.
-    fn transitions(&self) -> Vec<TransitionWithCustomCost>;
+    Trace {
+        state,
+        cost,
+        transitions: &transitions[1..],
+        model,
+        i: 0,
+    }
 }
 
 #[cfg(test)]
 mod tests {
+    use super::super::data_structure::FNode;
     use super::*;
     use dypdl::expression::*;
-    use dypdl::GroundedCondition;
-    use dypdl::SignatureVariables;
+    use dypdl::prelude::*;
+    use dypdl::{BaseCase, Effect, GroundedCondition};
     use std::rc::Rc;
 
-    struct MockCustomCostNode {
-        state: StateInRegistry,
-        cost: i32,
-        g: i32,
-        f: i32,
-    }
-
-    impl StateInformation<i32> for MockCustomCostNode {
-        fn cost(&self) -> i32 {
-            self.cost
-        }
-
-        fn state(&self) -> &StateInRegistry {
-            &self.state
-        }
-    }
-
-    impl PrioritizedNode<i32> for MockCustomCostNode {
-        fn f(&self) -> i32 {
-            self.f
-        }
-
-        fn g(&self) -> i32 {
-            self.g
-        }
-    }
-
-    impl CustomCostNodeInterface<i32, i32> for MockCustomCostNode {
-        fn new(
-            g: i32,
-            f: i32,
-            state: StateInRegistry<Rc<HashableSignatureVariables>>,
-            cost: i32,
-            _: Option<&Self>,
-            _: Option<Rc<TransitionWithCustomCost>>,
-        ) -> Self {
-            MockCustomCostNode { state, cost, g, f }
-        }
-
-        fn transitions(&self) -> Vec<TransitionWithCustomCost> {
-            Vec::default()
-        }
-    }
-
-    fn generate_model() -> dypdl::Model {
-        dypdl::Model {
-            forward_transitions: vec![Transition {
-                name: String::from("forward"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(1)),
-                )),
-                ..Default::default()
-            }],
-            forward_forced_transitions: vec![Transition {
-                name: String::from("forward_forced"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(2)),
-                )),
-                ..Default::default()
-            }],
-            backward_transitions: vec![Transition {
-                name: String::from("backward"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(3)),
-                )),
-                ..Default::default()
-            }],
-            backward_forced_transitions: vec![Transition {
-                name: String::from("backward_forced"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(4)),
-                )),
+    #[test]
+    fn rollout_some_without_transitions_base() {
+        let model = Model {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
+                condition: Condition::Constant(true),
                 ..Default::default()
-            }],
+            }])],
             ..Default::default()
-        }
+        };
+        let state = State::default();
+        let transitions = Vec::<Transition>::default();
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = rollout(&state, 1, &transitions, base_cost_evaluator, &model);
+        assert_eq!(
+            result,
+            Some(RolloutResult {
+                state: None,
+                cost: 1,
+                transitions: &transitions,
+                is_base: true,
+            })
+        );
     }
 
     #[test]
-    fn transition_with_custom_cost_to_transition() {
-        let transition = TransitionWithCustomCost {
-            transition: Transition {
-                preconditions: vec![GroundedCondition {
-                    condition: Condition::ComparisonI(
-                        ComparisonOperator::Le,
-                        Box::new(IntegerExpression::Variable(0)),
-                        Box::new(IntegerExpression::Constant(2)),
-                    ),
+    fn rollout_some_without_transitions_base_cost() {
+        let model = Model {
+            base_cases: vec![BaseCase::with_cost(
+                vec![GroundedCondition {
+                    condition: Condition::Constant(true),
                     ..Default::default()
                 }],
-                cost: CostExpression::Integer(IntegerExpression::Constant(3)),
+                1,
+            )],
+            ..Default::default()
+        };
+        let state = State::default();
+        let transitions = Vec::<Transition>::default();
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = rollout(&state, 1, &transitions, base_cost_evaluator, &model);
+        assert_eq!(
+            result,
+            Some(RolloutResult {
+                state: None,
+                cost: 2,
+                transitions: &transitions,
+                is_base: true,
+            })
+        );
+    }
+
+    #[test]
+    fn rollout_some_without_transitions_not_base() {
+        let model = Model {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
+                condition: Condition::Constant(false),
                 ..Default::default()
-            },
-            custom_cost: CostExpression::Integer(IntegerExpression::Constant(4)),
-            id: 0,
-            forced: false,
+            }])],
+            ..Default::default()
         };
-        let expected = Transition {
-            preconditions: vec![GroundedCondition {
+        let state = State::default();
+        let transitions = Vec::<Transition>::default();
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = rollout(&state, 1, &transitions, base_cost_evaluator, &model);
+        assert_eq!(
+            result,
+            Some(RolloutResult {
+                state: None,
+                cost: 1,
+                transitions: &transitions,
+                is_base: false,
+            })
+        );
+    }
+
+    #[test]
+    fn rollout_some_with_transitions_base() {
+        let model = Model {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::ComparisonI(
-                    ComparisonOperator::Le,
+                    ComparisonOperator::Ge,
                     Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(2)),
                 ),
                 ..Default::default()
-            }],
-            cost: CostExpression::Integer(IntegerExpression::Constant(3)),
+            }])],
             ..Default::default()
         };
-        assert_eq!(Transition::from(transition), expected);
+        let state = State {
+            signature_variables: SignatureVariables {
+                integer_variables: vec![0],
+                ..Default::default()
+            },
+            ..Default::default()
+        };
+        let transitions = vec![
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(1))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(3)),
+                ..Default::default()
+            },
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(2))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(4)),
+                ..Default::default()
+            },
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(3))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(5)),
+                ..Default::default()
+            },
+        ];
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = rollout(&state, 1, &transitions, base_cost_evaluator, &model);
+        assert_eq!(
+            result,
+            Some(RolloutResult {
+                state: Some(State {
+                    signature_variables: SignatureVariables {
+                        integer_variables: vec![2],
+                        ..Default::default()
+                    },
+                    ..Default::default()
+                }),
+                cost: 4,
+                transitions: &transitions[..2],
+                is_base: true
+            })
+        );
     }
 
     #[test]
-    fn is_applicable() {
-        let transition = Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                preconditions: vec![GroundedCondition {
+    fn rollout_some_with_transitions_base_cost() {
+        let model = Model {
+            base_cases: vec![BaseCase::with_cost(
+                vec![GroundedCondition {
                     condition: Condition::ComparisonI(
-                        ComparisonOperator::Le,
+                        ComparisonOperator::Ge,
                         Box::new(IntegerExpression::Variable(0)),
                         Box::new(IntegerExpression::Constant(2)),
                     ),
                     ..Default::default()
                 }],
-                ..Default::default()
-            },
-            custom_cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Mul,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(2)),
-            )),
-            id: 0,
-            forced: false,
-        });
-
-        let state = dypdl::State {
-            signature_variables: dypdl::SignatureVariables {
-                integer_variables: vec![2],
-                ..Default::default()
-            },
+                1,
+            )],
             ..Default::default()
         };
-        let registry = dypdl::TableRegistry::default();
-        assert!(transition.is_applicable(&state, &registry));
-        let state = dypdl::State {
-            signature_variables: dypdl::SignatureVariables {
-                integer_variables: vec![3],
+        let state = State {
+            signature_variables: SignatureVariables {
+                integer_variables: vec![0],
                 ..Default::default()
             },
             ..Default::default()
         };
-        assert!(!transition.is_applicable(&state, &registry));
-    }
-
-    #[test]
-    fn new() {
-        let model = Rc::new(generate_model());
-
-        let generator = SuccessorGenerator::from_model_without_custom_cost(model.clone(), false);
-
-        let transitions = vec![Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                name: String::from("forward"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(1)),
-                )),
-                ..Default::default()
-            },
-            custom_cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(1)),
-            )),
-            forced: false,
-            id: 0,
-        })];
-        let forced_transitions = vec![Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                name: String::from("forward_forced"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(2)),
-                )),
+        let transitions = vec![
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(1))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(3)),
                 ..Default::default()
             },
-            custom_cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(2)),
-            )),
-            forced: true,
-            id: 0,
-        })];
-        let expected = SuccessorGenerator::new(forced_transitions, transitions, false, model);
-        assert_eq!(generator, expected);
-    }
-
-    #[test]
-    fn new_backward() {
-        let model = Rc::new(generate_model());
-
-        let generator = SuccessorGenerator::from_model_without_custom_cost(model.clone(), true);
-        let transitions = vec![Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                name: String::from("backward"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(3)),
-                )),
-                ..Default::default()
-            },
-            custom_cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(3)),
-            )),
-            forced: false,
-            id: 0,
-        })];
-        let forced_transitions = vec![Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                name: String::from("backward_forced"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(4)),
-                )),
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(2))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(4)),
                 ..Default::default()
             },
-            custom_cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(IntegerExpression::Cost),
-                Box::new(IntegerExpression::Constant(4)),
-            )),
-            forced: true,
-            id: 0,
-        })];
-        let expected = SuccessorGenerator::new(forced_transitions, transitions, true, model);
-        assert_eq!(generator, expected);
-    }
-
-    #[test]
-    fn with_custom_costs() {
-        let model = Rc::new(generate_model());
-
-        let custom_costs = vec![CostExpression::Continuous(
-            ContinuousExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(ContinuousExpression::Constant(1.0)),
-                Box::new(ContinuousExpression::Constant(1.0)),
-            ),
-        )];
-        let forced_custom_costs = [CostExpression::Continuous(
-            ContinuousExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(ContinuousExpression::Constant(2.0)),
-                Box::new(ContinuousExpression::Constant(2.0)),
-            ),
-        )];
-        let generator = SuccessorGenerator::from_model_with_custom_costs(
-            model.clone(),
-            &custom_costs,
-            &forced_custom_costs,
-            false,
-        );
-        let transitions = vec![Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                name: String::from("forward"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(1)),
-                )),
-                ..Default::default()
-            },
-            custom_cost: CostExpression::Continuous(ContinuousExpression::Constant(2.0)),
-            forced: false,
-            id: 0,
-        })];
-        let forced_transitions = vec![Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                name: String::from("forward_forced"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(2)),
-                )),
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(3))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(5)),
                 ..Default::default()
             },
-            custom_cost: CostExpression::Continuous(ContinuousExpression::Constant(4.0)),
-            forced: true,
-            id: 0,
-        })];
-        let expected = SuccessorGenerator::new(forced_transitions, transitions, false, model);
-        assert_eq!(generator, expected);
+        ];
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = rollout(&state, 1, &transitions, base_cost_evaluator, &model);
+        assert_eq!(
+            result,
+            Some(RolloutResult {
+                state: Some(State {
+                    signature_variables: SignatureVariables {
+                        integer_variables: vec![2],
+                        ..Default::default()
+                    },
+                    ..Default::default()
+                }),
+                cost: 5,
+                transitions: &transitions[..2],
+                is_base: true
+            })
+        );
     }
 
     #[test]
-    fn with_custom_costs_backward() {
-        let model = Rc::new(generate_model());
-
-        let custom_costs = vec![CostExpression::Continuous(
-            ContinuousExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(ContinuousExpression::Constant(3.0)),
-                Box::new(ContinuousExpression::Constant(3.0)),
-            ),
-        )];
-        let forced_custom_costs = [CostExpression::Continuous(
-            ContinuousExpression::BinaryOperation(
-                BinaryOperator::Add,
-                Box::new(ContinuousExpression::Constant(4.0)),
-                Box::new(ContinuousExpression::Constant(4.0)),
-            ),
-        )];
-
-        let generator = SuccessorGenerator::from_model_with_custom_costs(
-            model.clone(),
-            &custom_costs,
-            &forced_custom_costs,
-            true,
-        );
-        let transitions = vec![Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                name: String::from("backward"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
-                    Box::new(IntegerExpression::Constant(3)),
-                )),
-                ..Default::default()
-            },
-            custom_cost: CostExpression::Continuous(ContinuousExpression::Constant(6.0)),
-            forced: false,
-            id: 0,
-        })];
-        let forced_transitions = vec![Rc::new(TransitionWithCustomCost {
-            transition: Transition {
-                name: String::from("backward_forced"),
-                cost: CostExpression::Integer(IntegerExpression::BinaryOperation(
-                    BinaryOperator::Add,
-                    Box::new(IntegerExpression::Cost),
+    fn rollout_some_with_transitions_not_base() {
+        let model = Model {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
+                condition: Condition::ComparisonI(
+                    ComparisonOperator::Ge,
+                    Box::new(IntegerExpression::Variable(0)),
                     Box::new(IntegerExpression::Constant(4)),
-                )),
+                ),
                 ..Default::default()
-            },
-            custom_cost: CostExpression::Continuous(ContinuousExpression::Constant(8.0)),
-            forced: true,
-            id: 0,
-        })];
-        let expected = SuccessorGenerator::new(forced_transitions, transitions, true, model);
-        assert_eq!(generator, expected);
-    }
-
-    #[test]
-    fn generate_successor_state_some() {
-        let model = dypdl::Model::default();
-        let state = dypdl::State {
+            }])],
+            ..Default::default()
+        };
+        let state = State {
             signature_variables: SignatureVariables {
                 integer_variables: vec![0],
                 ..Default::default()
             },
             ..Default::default()
         };
-        let transition = TransitionWithCustomCost {
-            transition: dypdl::Transition {
-                name: String::from("op1"),
-                cost: CostExpression::Integer(IntegerExpression::Constant(1)),
-                effect: dypdl::Effect {
+        let transitions = vec![
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(1))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(3)),
+                ..Default::default()
+            },
+            Transition {
+                effect: Effect {
                     integer_effects: vec![(0, IntegerExpression::Constant(2))],
                     ..Default::default()
                 },
+                cost: CostExpression::Integer(IntegerExpression::Constant(4)),
                 ..Default::default()
             },
-            custom_cost: CostExpression::Integer(IntegerExpression::Constant(3)),
-            forced: false,
-            id: 0,
-        };
-        let h_evaluator = |_: &dypdl::State, _: &dypdl::Model| Some(1);
-        let f_evaluator = |_, _, _: &dypdl::State, _: &dypdl::Model| 4;
-        let parent = CustomCostParent {
-            state: &state,
-            cost: 0,
-            g: 0,
-        };
-        let result = transition.generate_successor_state(
-            &parent,
-            &model,
-            None,
-            h_evaluator,
-            f_evaluator,
-            false,
-        );
-        assert!(result.is_some());
-        let (state, cost, g, f) = result.unwrap();
-        assert_eq!(
-            state,
-            dypdl::State {
-                signature_variables: SignatureVariables {
-                    integer_variables: vec![2],
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(3))],
                     ..Default::default()
                 },
+                cost: CostExpression::Integer(IntegerExpression::Constant(5)),
                 ..Default::default()
-            }
+            },
+        ];
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = rollout(&state, 1, &transitions, base_cost_evaluator, &model);
+        assert_eq!(
+            result,
+            Some(RolloutResult {
+                state: Some(State {
+                    signature_variables: SignatureVariables {
+                        integer_variables: vec![3],
+                        ..Default::default()
+                    },
+                    ..Default::default()
+                }),
+                cost: 5,
+                transitions: &transitions[..],
+                is_base: false
+            })
         );
-        assert_eq!(cost, 1);
-        assert_eq!(g, 3);
-        assert_eq!(f, 4);
     }
 
     #[test]
-    fn generate_successor_state_pruned_by_constraint() {
-        let model = dypdl::Model {
+    fn rollout_not_applicable() {
+        let model = Model::default();
+        let state = State::default();
+        let transitions = vec![Transition {
+            preconditions: vec![GroundedCondition {
+                condition: Condition::Constant(false),
+                ..Default::default()
+            }],
+            ..Default::default()
+        }];
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = rollout(&state, 1, &transitions, base_cost_evaluator, &model);
+        assert_eq!(result, None);
+    }
+
+    #[test]
+    fn rollout_violates_constraint() {
+        let model = Model {
             state_constraints: vec![GroundedCondition {
                 condition: Condition::Constant(false),
                 ..Default::default()
             }],
             ..Default::default()
         };
-        let state = dypdl::State::default();
-        let transition = TransitionWithCustomCost::default();
-        let h_evaluator = |_: &dypdl::State, _: &dypdl::Model| Some(1);
-        let f_evaluator = |_, _, _: &dypdl::State, _: &dypdl::Model| 4;
-        let parent = CustomCostParent {
-            state: &state,
-            cost: 0,
-            g: 0,
-        };
-        let result = transition.generate_successor_state(
-            &parent,
+        let state = State::default();
+        let transitions = vec![Transition::default()];
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = rollout(&state, 1, &transitions, base_cost_evaluator, &model);
+        assert_eq!(result, None);
+    }
+
+    #[test]
+    fn get_solution_cost_and_suffix_some() {
+        let mut model = Model::default();
+        let var = model.add_integer_variable("var", 0).unwrap();
+        let result = model.add_base_case(vec![Condition::comparison_i(
+            ComparisonOperator::Ge,
+            var,
+            3,
+        )]);
+        assert!(result.is_ok());
+
+        let mut transition = Transition::new("transition");
+        transition.add_effect(var, var + 1).unwrap();
+        transition.set_cost(IntegerExpression::Cost + 1);
+
+        let h_evaluator = |_: &StateInRegistry| Some(0);
+        let f_evaluator = |g, h, _: &StateInRegistry| g + h;
+        let node = FNode::generate_root_node(
+            model.target.clone(),
+            0,
             &model,
+            &h_evaluator,
+            &f_evaluator,
             None,
-            h_evaluator,
-            f_evaluator,
-            false,
         );
-        assert!(result.is_none());
+        assert!(node.is_some());
+        let node = node.unwrap();
+        let node = node.generate_successor_node(
+            Rc::new(transition.clone()),
+            &model,
+            &h_evaluator,
+            &f_evaluator,
+            None,
+        );
+        assert!(node.is_some());
+        let node = node.unwrap();
+
+        let suffix = [transition.clone(), transition.clone()];
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = get_solution_cost_and_suffix(&model, &node, &suffix, base_cost_evaluator);
+        assert!(result.is_some());
+        let (cost, suffix) = result.unwrap();
+        assert_eq!(cost, 3);
+        assert_eq!(suffix, &[transition.clone(), transition]);
     }
 
     #[test]
-    fn generate_successor_state_pruned_by_bound() {
-        let model = dypdl::Model::default();
-        let state = dypdl::State::default();
-        let transition = TransitionWithCustomCost::default();
-        let h_evaluator = |_: &dypdl::State, _: &dypdl::Model| Some(1);
-        let f_evaluator = |_, _, _: &dypdl::State, _: &dypdl::Model| 4;
-        let parent = CustomCostParent {
-            state: &state,
-            cost: 0,
-            g: 0,
-        };
-        let result = transition.generate_successor_state(
-            &parent,
+    fn get_solution_cost_and_suffix_some_with_base_cost() {
+        let mut model = Model::default();
+        let var = model.add_integer_variable("var", 0).unwrap();
+        let result = model.add_base_case_with_cost(
+            vec![Condition::comparison_i(ComparisonOperator::Ge, var, 3)],
+            1,
+        );
+        assert!(result.is_ok());
+
+        let mut transition = Transition::new("transition");
+        transition.add_effect(var, var + 1).unwrap();
+        transition.set_cost(IntegerExpression::Cost + 1);
+
+        let h_evaluator = |_: &StateInRegistry| Some(0);
+        let f_evaluator = |g, h, _: &StateInRegistry| g + h;
+        let node = FNode::generate_root_node(
+            model.target.clone(),
+            0,
+            &model,
+            &h_evaluator,
+            &f_evaluator,
+            None,
+        );
+        assert!(node.is_some());
+        let node = node.unwrap();
+        let node = node.generate_successor_node(
+            Rc::new(transition.clone()),
+            &model,
+            &h_evaluator,
+            &f_evaluator,
+            None,
+        );
+        assert!(node.is_some());
+        let node = node.unwrap();
+
+        let suffix = [transition.clone(), transition.clone()];
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = get_solution_cost_and_suffix(&model, &node, &suffix, base_cost_evaluator);
+        assert!(result.is_some());
+        let (cost, suffix) = result.unwrap();
+        assert_eq!(cost, 4);
+        assert_eq!(suffix, &[transition.clone(), transition]);
+    }
+
+    #[test]
+    fn get_solution_cost_and_suffix_none() {
+        let mut model = Model::default();
+        let var = model.add_integer_variable("var", 0).unwrap();
+        let result = model.add_base_case(vec![Condition::comparison_i(
+            ComparisonOperator::Ge,
+            var,
+            3,
+        )]);
+        assert!(result.is_ok());
+
+        let mut transition = Transition::new("transition");
+        transition.add_effect(var, var + 1).unwrap();
+        transition.set_cost(IntegerExpression::Cost + 1);
+
+        let h_evaluator = |_: &StateInRegistry| Some(0);
+        let f_evaluator = |g, h, _: &StateInRegistry| g + h;
+        let node = FNode::<_>::generate_root_node(
+            model.target.clone(),
+            0,
             &model,
-            Some(4),
-            h_evaluator,
-            f_evaluator,
-            false,
+            &h_evaluator,
+            &f_evaluator,
+            None,
         );
+        assert!(node.is_some());
+        let node = node.unwrap();
+
+        let suffix = [transition.clone(), transition.clone()];
+        let base_cost_evaluator = |cost, base_cost| cost + base_cost;
+        let result = get_solution_cost_and_suffix(&model, &node, &suffix, base_cost_evaluator);
         assert!(result.is_none());
     }
 
     #[test]
-    fn chain_new_no_parent() {
-        let op1 = Rc::new(TransitionWithCustomCost {
-            transition: dypdl::Transition {
-                name: String::from("op1"),
-                ..Default::default()
-            },
-            ..Default::default()
-        });
-        let chain = TransitionWithCustomCostChain::new(None, op1.clone());
-        assert_eq!(chain.parent(), None);
-        assert_eq!(chain.last(), &*op1);
+    #[should_panic]
+    fn trace_without_transitions() {
+        let model = Model::default();
+        let state = State::default();
+        let transitions = Vec::<Transition>::default();
+        get_trace(&state, 1, &transitions, &model);
     }
 
     #[test]
-    fn chain_new_with_parent() {
-        let op1 = Rc::new(TransitionWithCustomCost {
-            transition: dypdl::Transition {
-                name: String::from("op1"),
+    fn trace_with_transitions() {
+        let model = Model {
+            base_cases: vec![BaseCase::from(vec![GroundedCondition {
+                condition: Condition::ComparisonI(
+                    ComparisonOperator::Ge,
+                    Box::new(IntegerExpression::Variable(0)),
+                    Box::new(IntegerExpression::Constant(2)),
+                ),
                 ..Default::default()
-            },
+            }])],
             ..Default::default()
-        });
-        let chain1 = Rc::new(TransitionWithCustomCostChain::new(None, op1));
-        let op2 = Rc::new(TransitionWithCustomCost {
-            transition: dypdl::Transition {
-                name: String::from("op2"),
+        };
+        let state = State {
+            signature_variables: SignatureVariables {
+                integer_variables: vec![0],
                 ..Default::default()
             },
             ..Default::default()
-        });
-        let chain2 = TransitionWithCustomCostChain::new(Some(chain1.clone()), op2.clone());
-        assert_eq!(chain2.parent(), Some(&chain1));
-        assert_eq!(chain2.last(), &*op2);
+        };
+        let transitions = vec![
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(1))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(3)),
+                ..Default::default()
+            },
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(2))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(4)),
+                ..Default::default()
+            },
+            Transition {
+                effect: Effect {
+                    integer_effects: vec![(0, IntegerExpression::Constant(3))],
+                    ..Default::default()
+                },
+                cost: CostExpression::Integer(IntegerExpression::Constant(5)),
+                ..Default::default()
+            },
+        ];
+        let mut result = get_trace(&state, 1, &transitions, &model);
+        assert_eq!(
+            result.next(),
+            Some((
+                State {
+                    signature_variables: SignatureVariables {
+                        integer_variables: vec![1],
+                        ..Default::default()
+                    },
+                    ..Default::default()
+                },
+                3
+            ))
+        );
+        assert_eq!(
+            result.next(),
+            Some((
+                State {
+                    signature_variables: SignatureVariables {
+                        integer_variables: vec![2],
+                        ..Default::default()
+                    },
+                    ..Default::default()
+                },
+                4
+            ))
+        );
+        assert_eq!(
+            result.next(),
+            Some((
+                State {
+                    signature_variables: SignatureVariables {
+                        integer_variables: vec![3],
+                        ..Default::default()
+                    },
+                    ..Default::default()
+                },
+                5
+            ))
+        );
+        assert_eq!(result.next(), None);
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/util.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure/util.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/data_structure.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,33 +1,21 @@
 //! A module for data structures.
 
-pub mod beam;
-mod beam_search_node;
-mod beam_search_problem_instance;
-mod bfs_node;
-mod f_node;
+mod beam;
 mod hashable_state;
-mod lazy_search_node;
-mod prioritized_node;
 mod search_node;
-pub mod state_registry;
-pub mod successor_generator;
+mod state_registry;
+mod successor_generator;
+mod transition;
 mod transition_chain;
-mod transition_with_custom_cost;
 mod util;
 
-pub use beam_search_node::BeamSearchNode;
-pub use beam_search_problem_instance::BeamSearchProblemInstance;
-pub use bfs_node::BfsNodeInterface;
-pub use f_node::FNode;
+pub use beam::{Beam, BeamDrain};
 pub use hashable_state::{
     HashableSignatureVariables, HashableState, StateWithHashableSignatureVariables,
 };
-pub use lazy_search_node::LazySearchNode;
-pub use prioritized_node::PrioritizedNode;
-pub use search_node::SearchNode;
+pub use search_node::{BfsNode, CostNode, CustomFNode, FNode, WeightedFNode};
+pub use state_registry::{StateInRegistry, StateInformation, StateRegistry};
 pub use successor_generator::{ApplicableTransitions, SuccessorGenerator};
-pub use transition_chain::{TransitionChain, TransitionChainInterface};
-pub use transition_with_custom_cost::{
-    CustomCostNodeInterface, CustomCostParent, TransitionWithCustomCost,
-};
+pub use transition::{TransitionWithCustomCost, TransitionWithId};
+pub use transition_chain::{GetTransitions, RcChain, TransitionChain};
 pub use util::exceed_bound;
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/dijkstra.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/acps.rs`

 * *Files 24% similar despite different names*

```diff
@@ -1,443 +1,395 @@
-use super::data_structure::state_registry::{StateInRegistry, StateInformation, StateRegistry};
-use super::data_structure::{
-    LazySearchNode, SearchNode, SuccessorGenerator, TransitionChain, TransitionChainInterface,
-};
-use super::search::{Search, Solution};
-use super::util;
-use dypdl::{variable_type, TransitionInterface};
-use std::cmp::Ordering;
-use std::cmp::Reverse;
-use std::collections::BinaryHeap;
+use super::data_structure::{exceed_bound, BfsNode, StateRegistry, SuccessorGenerator};
+use super::rollout::get_solution_cost_and_suffix;
+use super::search::{Parameters, Search, SearchInput, Solution};
+use super::util::{print_dual_bound, update_solution, TimeKeeper};
+use dypdl::{variable_type, Transition, TransitionInterface};
+use std::cmp;
+use std::collections;
 use std::error::Error;
 use std::fmt;
 use std::rc::Rc;
-use std::str;
 
-/// Dijkstra's algorithm Solver.
-///
-/// This solver uses forward search based on the shortest path problem.
-/// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, or `min(cost, w)
-/// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
-/// In addition `w` must be non-negative, and the model must be minimization.
-///
-/// `lazy` indicates whether the solver uses lazy evaluation.
-///
-/// # Examples
-///
-/// ```
-/// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{Dijkstra, Search};
-/// use dypdl_heuristic_search::search_algorithm::util::{
-///     ForwardSearchParameters, Parameters,
-/// };
-/// use std::rc::Rc;
-///
-/// let mut model = Model::default();
-/// let variable = model.add_integer_variable("variable", 0).unwrap();
-/// model.add_base_case(
-///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
-/// ).unwrap();
-/// let mut increment = Transition::new("increment");
-/// increment.set_cost(IntegerExpression::Cost + 1);
-/// increment.add_effect(variable, variable + 1).unwrap();
-/// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let model = Rc::new(model);
-/// let parameters = Parameters::default();
-/// let mut solver = Dijkstra::new(model, parameters, false, None);
-/// let solution = solver.search().unwrap();
-/// assert_eq!(solution.cost, Some(1));
-/// assert_eq!(solution.transitions, vec![increment]);
-/// assert!(!solution.is_infeasible);
-/// ```
-pub struct Dijkstra<T>
-where
-    T: variable_type::Numeric + fmt::Display + Ord + 'static,
-    <T as str::FromStr>::Err: fmt::Debug,
-{
-    model: Rc<dypdl::Model>,
-    parameters: util::Parameters<T>,
-    lazy: bool,
-    initial_registry_capacity: Option<usize>,
-    terminated: bool,
-    solution: Solution<T>,
+/// Parameters for progressive search.
+#[derive(Clone, Copy, PartialEq, Eq)]
+pub struct ProgressiveSearchParameters {
+    /// The initial width.
+    pub init: usize,
+    /// The amount of increase.
+    pub step: usize,
+    /// The maximum value of the width.
+    pub bound: Option<usize>,
+    /// Whether reset the bound when a better solution is found.
+    pub reset: bool,
 }
 
-impl<T> Dijkstra<T>
-where
-    T: variable_type::Numeric + fmt::Display + Ord + 'static,
-    <T as str::FromStr>::Err: fmt::Debug,
-{
-    /// Create a new Dijkstra's algorithm solver.
-    pub fn new(
-        model: Rc<dypdl::Model>,
-        parameters: util::Parameters<T>,
-        lazy: bool,
-        initial_registry_capacity: Option<usize>,
-    ) -> Dijkstra<T> {
-        Dijkstra {
-            model,
-            parameters,
-            lazy,
-            initial_registry_capacity,
-            terminated: false,
-            solution: Solution::default(),
+impl ProgressiveSearchParameters {
+    /// Returns the increased width.
+    pub fn increase_width(&self, width: usize) -> usize {
+        if let Some(bound) = self.bound {
+            cmp::min(width + self.step, bound)
+        } else {
+            width + self.step
         }
     }
 }
 
-impl<T> Search<T> for Dijkstra<T>
-where
-    T: variable_type::Numeric + fmt::Display + Ord + 'static,
-    <T as str::FromStr>::Err: fmt::Debug,
-{
-    fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
-        if self.terminated {
-            return Ok((self.solution.clone(), true));
+impl Default for ProgressiveSearchParameters {
+    /// Returns parameters where the initial width is 1, the step is 1, no bound, and no reset.
+    fn default() -> Self {
+        Self {
+            init: 1,
+            step: 1,
+            bound: None,
+            reset: false,
         }
-
-        let generator = SuccessorGenerator::from_model(self.model.clone(), false);
-
-        self.solution = if self.lazy {
-            lazy_dijkstra(
-                &self.model,
-                generator,
-                self.parameters,
-                self.initial_registry_capacity,
-            )
-        } else {
-            dijkstra(
-                &self.model,
-                generator,
-                self.parameters,
-                self.initial_registry_capacity,
-            )
-        };
-        self.terminated = true;
-        Ok((self.solution.clone(), true))
     }
 }
 
-/// Performs Dijkstra's algorithm.
+/// Anytime Column Progressive Search (ACPS).
 ///
-/// `registry_capacity` is the initial capacity of the state registry.
+/// This solver uses forward search based on the shortest path problem.
+/// It only works with problems where the cost expressions are in the form of `cost + w`, `cost * w`, `max(cost, w)`, or `min(cost, w)`
+/// where `cost` is `IntegerExpression::Cost`or `ContinuousExpression::Cost` and `w` is a numeric expression independent of `cost`.
+///
+/// Type parameter `N` is a node type that implements `BfsNode`.
+/// Type parameter `E` is a type of a function that evaluates a transition and insert a successor node into a state registry.
+/// The last argument of the function is the primal bound of the solution cost.
+/// Type parameter `B` is a type of a function that combines the g-value (the cost to a state) and the base cost.
+/// It should be the same function as the cost expression, e.g., `cost + base_cost` for `cost + w`.
+///
+/// # References
+///
+/// Ryo Kuroiwa and J. Christopher Beck."Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
+/// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
+///
+/// Sataya Gautam Vadlamudi, Piyush Gaurav, Sandip Aine, and Partha Pratim Chakrabarti. "Anytime Column Search,""
+/// Proceedings of AI 2012: Advances in Artificial Intelligence, pp. 254-255, 2012.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{dijkstra, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
-/// };
-/// use dypdl_heuristic_search::search_algorithm::util::{
-///     ForwardSearchParameters, Parameters,
+/// use dypdl_heuristic_search::{Parameters, ProgressiveSearchParameters, Search};
+/// use dypdl_heuristic_search::search_algorithm::{
+///     Acps, FNode, SearchInput, SuccessorGenerator,
 /// };
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
-///
 /// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model(model.clone(), false);
+///
+/// let state = model.target.clone();
+/// let cost = 0;
+/// let h_evaluator = |_: &_| Some(0);
+/// let f_evaluator = |g, h, _: &_| g + h;
+/// let primal_bound = None;
+/// let node = FNode::generate_root_node(
+///     state,
+///     cost,
+///     &model,
+///     &h_evaluator,
+///     &f_evaluator,
+///     primal_bound,
+/// );
+/// let generator = SuccessorGenerator::<Transition>::from_model(model.clone(), false);
+/// let input = SearchInput {
+///     node,
+///     generator,
+///     solution_suffix: &[],
+/// };
+/// let transition_evaluator =
+///     move |node: &FNode<_>, transition, registry: &mut _, primal_bound| {
+///         node.insert_successor_node(
+///             transition,
+///             registry,
+///             &h_evaluator,
+///             &f_evaluator,
+///             primal_bound,
+///         )
+///     };
+/// let base_cost_evaluator = |cost, base_cost| cost + base_cost;
 /// let parameters = Parameters::default();
-/// let solution = dijkstra(&model, generator, parameters, None);
+/// let progressive_parameters = ProgressiveSearchParameters::default();
+///
+/// let mut solver = Acps::<_, FNode<_>, _, _>::new(
+///     input, transition_evaluator, base_cost_evaluator, parameters, progressive_parameters,
+/// );
+/// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
-pub fn dijkstra<T>(
-    model: &Rc<dypdl::Model>,
-    generator: SuccessorGenerator,
-    parameters: util::Parameters<T>,
-    registry_capacity: Option<usize>,
-) -> Solution<T>
+pub struct Acps<'a, T, N, E, B, V = Transition>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    let time_keeper = parameters
-        .time_limit
-        .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
-    let primal_bound = parameters.primal_bound;
-    let mut open = BinaryHeap::<Reverse<Rc<_>>>::default();
-    let mut registry = StateRegistry::new(model.clone());
-
-    if let Some(capacity) = registry_capacity {
-        registry.reserve(capacity);
-    }
-
-    let cost = T::zero();
-    let initial_state = StateInRegistry::from(model.target.clone());
-    let constructor = |state: StateInRegistry, cost: T, _: Option<&SearchNode<T>>| {
-        Some(SearchNode {
-            state,
-            cost,
-            ..Default::default()
-        })
-    };
-    let (initial_node, _) = registry.insert(initial_state, cost, constructor).unwrap();
-    open.push(Reverse(initial_node));
-    let mut expanded = 0;
-    let mut generated = 1;
-    let mut cost_max = T::zero();
-
-    while let Some(Reverse(node)) = open.pop() {
-        if *node.closed.borrow() {
-            continue;
-        }
-
-        *node.closed.borrow_mut() = true;
-
-        if node.cost() > cost_max {
-            cost_max = node.cost();
+    generator: SuccessorGenerator<V>,
+    suffix: &'a [V],
+    transition_evaluator: E,
+    base_cost_evaluator: B,
+    progressive_parameters: ProgressiveSearchParameters,
+    primal_bound: Option<T>,
+    get_all_solutions: bool,
+    quiet: bool,
+    width: usize,
+    open: Vec<collections::BinaryHeap<Rc<N>>>,
+    registry: StateRegistry<T, N>,
+    layer_index: usize,
+    node_index: usize,
+    no_node: bool,
+    goal_found: bool,
+    time_keeper: TimeKeeper,
+    solution: Solution<T>,
+}
 
-            if !parameters.quiet {
-                println!("cost = {}, expanded: {}", cost_max, expanded);
-            }
-        }
+impl<'a, T, N, E, B, V> Acps<'a, T, N, E, B, V>
+where
+    T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
+{
+    /// Creates a new ACPS solver.
+    pub fn new(
+        input: SearchInput<'a, N, V>,
+        transition_evaluator: E,
+        base_cost_evaluator: B,
+        parameters: Parameters<T>,
+        progressive_parameters: ProgressiveSearchParameters,
+    ) -> Acps<'a, T, N, E, B, V> {
+        let mut time_keeper = parameters
+            .time_limit
+            .map_or_else(TimeKeeper::default, TimeKeeper::with_time_limit);
+        let primal_bound = parameters.primal_bound;
+        let quiet = parameters.quiet;
 
-        if model.is_base(node.state()) {
-            return Solution {
-                cost: Some(node.cost()),
-                is_optimal: true,
-                transitions: node
-                    .transitions
-                    .as_ref()
-                    .map_or_else(Vec::new, |transition| transition.transitions()),
-                expanded,
-                generated,
-                time: time_keeper.elapsed_time(),
-                ..Default::default()
-            };
-        }
+        let mut open = vec![collections::BinaryHeap::new()];
+        let mut registry = StateRegistry::<_, _>::new(input.generator.model.clone());
 
-        if time_keeper.check_time_limit() {
-            return Solution {
-                best_bound: Some(cost_max),
-                expanded,
-                generated,
-                time: time_keeper.elapsed_time(),
-                time_out: true,
-                ..Default::default()
-            };
+        if let Some(capacity) = parameters.initial_registry_capacity {
+            registry.reserve(capacity);
         }
 
-        expanded += 1;
+        let mut solution = Solution::default();
 
-        for transition in generator.applicable_transitions(node.state()) {
-            if let Some((successor, new_generated)) =
-                node.generate_successor(transition, &mut registry, primal_bound)
-            {
-                open.push(Reverse(successor));
-
-                if new_generated {
-                    generated += 1;
-                }
+        if let Some(node) = input.node {
+            let (node, _) = registry.insert(node).unwrap();
+            solution.generated += 1;
+            solution.best_bound = node.bound(&input.generator.model);
+            open[0].push(node);
+
+            if !quiet {
+                solution.time = time_keeper.elapsed_time();
+                print_dual_bound(&solution);
             }
+        } else {
+            solution.is_infeasible = true;
         }
-    }
-
-    Solution {
-        is_infeasible: true,
-        expanded,
-        generated,
-        time: time_keeper.elapsed_time(),
-        ..Default::default()
-    }
-}
-
-/// Search node stored in the open list of lazy Dijkstra.
-#[derive(Debug, Clone)]
-pub struct DijkstraEdge<T: variable_type::Numeric + Ord> {
-    pub cost: T,
-    pub parent: Rc<LazySearchNode<T>>,
-    pub transition: Rc<dypdl::Transition>,
-}
 
-impl<T: variable_type::Numeric + Ord> PartialEq for DijkstraEdge<T> {
-    fn eq(&self, other: &Self) -> bool {
-        self.cost == other.cost
-    }
-}
-
-impl<T: variable_type::Numeric + Ord> Eq for DijkstraEdge<T> {}
+        time_keeper.stop();
 
-impl<T: variable_type::Numeric + Ord> Ord for DijkstraEdge<T> {
-    fn cmp(&self, other: &Self) -> Ordering {
-        self.cost.cmp(&other.cost)
-    }
-}
-
-impl<T: variable_type::Numeric + Ord> PartialOrd for DijkstraEdge<T> {
-    fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
-        Some(self.cmp(other))
+        Acps {
+            generator: input.generator,
+            suffix: input.solution_suffix,
+            transition_evaluator,
+            base_cost_evaluator,
+            progressive_parameters,
+            primal_bound,
+            get_all_solutions: parameters.get_all_solutions,
+            quiet,
+            width: progressive_parameters.init,
+            open,
+            registry,
+            layer_index: 0,
+            node_index: 0,
+            no_node: true,
+            goal_found: false,
+            time_keeper,
+            solution,
+        }
     }
 }
 
-/// Performs lazy Dijkstra's algorithm.
-///
-/// Pointers to parent nodes and transitions are stored in the open list, and a state is generated when it is expanded.
-///
-/// # Examples
-///
-/// ```
-/// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{lazy_dijkstra, Search};
-/// use dypdl_heuristic_search::search_algorithm::data_structure::successor_generator::{
-///     SuccessorGenerator
-/// };
-/// use dypdl_heuristic_search::search_algorithm::util::{
-///     ForwardSearchParameters, Parameters,
-/// };
-/// use std::rc::Rc;
-///
-/// let mut model = Model::default();
-/// let variable = model.add_integer_variable("variable", 0).unwrap();
-/// model.add_base_case(
-///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
-/// ).unwrap();
-/// let mut increment = Transition::new("increment");
-/// increment.set_cost(IntegerExpression::Cost + 1);
-/// increment.add_effect(variable, variable + 1).unwrap();
-/// model.add_forward_transition(increment.clone()).unwrap();
-///
-/// let model = Rc::new(model);
-/// let generator = SuccessorGenerator::from_model(model.clone(), false);
-/// let parameters = Parameters::default();
-/// let solution = lazy_dijkstra(&model, generator, parameters, None);
-/// assert_eq!(solution.cost, Some(1));
-/// assert_eq!(solution.transitions, vec![increment]);
-/// assert!(!solution.is_infeasible);
-/// ```
-pub fn lazy_dijkstra<T>(
-    model: &Rc<dypdl::Model>,
-    generator: SuccessorGenerator,
-    parameters: util::Parameters<T>,
-    registry_capacity: Option<usize>,
-) -> Solution<T>
+impl<'a, T, N, E, B, V> Search<T> for Acps<'a, T, N, E, B, V>
 where
     T: variable_type::Numeric + Ord + fmt::Display,
+    N: BfsNode<T, V>,
+    E: Fn(&N, Rc<V>, &mut StateRegistry<T, N>, Option<T>) -> Option<(Rc<N>, bool)>,
+    B: Fn(T, T) -> T,
+    V: TransitionInterface + Clone + Default,
+    Transition: From<V>,
 {
-    let time_keeper = parameters
-        .time_limit
-        .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
-    let primal_bound = parameters.primal_bound;
-    let mut open = BinaryHeap::default();
-    let mut registry = StateRegistry::<T, LazySearchNode<_>>::new(model.clone());
+    fn search_next(&mut self) -> Result<(Solution<T>, bool), Box<dyn Error>> {
+        if self.solution.is_terminated() {
+            return Ok((self.solution.clone(), true));
+        }
 
-    if let Some(capacity) = registry_capacity {
-        registry.reserve(capacity);
-    }
+        self.time_keeper.start();
+        let model = &self.generator.model;
+        let suffix = self.suffix;
+
+        loop {
+            while self.node_index < self.width && !self.open[self.layer_index].is_empty() {
+                let node = self.open[self.layer_index].pop().unwrap();
 
-    let cost = T::zero();
-    let initial_state = StateInRegistry::from(model.target.clone());
+                if node.is_closed() {
+                    continue;
+                }
+                node.close();
 
-    let constructor = |state: StateInRegistry, cost: T, _: Option<&LazySearchNode<T>>| {
-        Some(LazySearchNode {
-            state,
-            cost,
-            ..Default::default()
-        })
-    };
-    let (initial_node, _) = registry.insert(initial_state, cost, constructor).unwrap();
-
-    for transition in generator.applicable_transitions(&initial_node.state) {
-        let cost = transition.eval_cost(
-            initial_node.cost,
-            &initial_node.state,
-            &model.table_registry,
-        );
-        open.push(Reverse(DijkstraEdge {
-            cost,
-            parent: initial_node.clone(),
-            transition,
-        }));
-    }
+                if let Some(dual_bound) = node.bound(model) {
+                    if exceed_bound(model, dual_bound, self.primal_bound) {
+                        if N::ordered_by_bound() {
+                            self.open[self.layer_index].clear();
+                        }
+                        continue;
+                    }
+                }
 
-    let mut expanded = 0;
-    let mut cost_max = T::zero();
+                if self.no_node {
+                    self.no_node = false;
+                }
 
-    while let Some(Reverse(edge)) = open.pop() {
-        let state = edge
-            .transition
-            .apply(&edge.parent.state, &model.table_registry);
-        if !model.check_constraints(&state) {
-            continue;
-        }
-        let constructor = |state: StateInRegistry, cost: T, _: Option<&LazySearchNode<T>>| {
-            Some(LazySearchNode {
-                state,
-                cost,
-                transitions: Some(Rc::new(TransitionChain::new(
-                    edge.parent.transitions.clone(),
-                    edge.transition,
-                ))),
-            })
-        };
-        if let Some((node, _)) = registry.insert(state, edge.cost, constructor) {
-            expanded += 1;
+                if let Some((cost, suffix)) =
+                    get_solution_cost_and_suffix(model, &*node, suffix, &self.base_cost_evaluator)
+                {
+                    self.node_index += 1;
+
+                    if !exceed_bound(model, cost, self.primal_bound) {
+                        if !self.goal_found {
+                            self.goal_found = true;
+                        }
+
+                        self.primal_bound = Some(cost);
+                        let time = self.time_keeper.elapsed_time();
+                        update_solution(&mut self.solution, &*node, cost, suffix, time, self.quiet);
+                        self.time_keeper.stop();
+
+                        return Ok((self.solution.clone(), self.solution.is_optimal));
+                    } else if self.get_all_solutions {
+                        let mut solution = self.solution.clone();
+                        let time = self.time_keeper.elapsed_time();
+                        update_solution(&mut solution, &*node, cost, suffix, time, true);
+                        self.time_keeper.stop();
+
+                        return Ok((solution, false));
+                    }
+                    continue;
+                }
+
+                if self.time_keeper.check_time_limit(self.quiet) {
+                    self.solution.time_out = true;
+                    self.solution.time = self.time_keeper.elapsed_time();
+                    self.time_keeper.stop();
 
-            if node.cost > cost_max {
-                cost_max = node.cost;
-                if !parameters.quiet {
-                    println!("cost = {}, expanded: {}", cost_max, expanded);
+                    return Ok((self.solution.clone(), true));
                 }
-            }
 
-            if model.is_base(&node.state) {
-                return Solution {
-                    cost: Some(node.cost),
-                    is_optimal: true,
-                    transitions: node
-                        .transitions
-                        .as_ref()
-                        .map_or_else(Vec::new, |transition| transition.transitions()),
-                    expanded,
-                    generated: expanded,
-                    time: time_keeper.elapsed_time(),
-                    ..Default::default()
-                };
-            }
+                self.solution.expanded += 1;
 
-            if time_keeper.check_time_limit() {
-                return Solution {
-                    best_bound: Some(cost_max),
-                    expanded,
-                    generated: expanded,
-                    time: time_keeper.elapsed_time(),
-                    time_out: true,
-                    ..Default::default()
-                };
+                for transition in self.generator.applicable_transitions(node.state()) {
+                    if let Some((successor, new_generated)) = (self.transition_evaluator)(
+                        &node,
+                        transition,
+                        &mut self.registry,
+                        self.primal_bound,
+                    ) {
+                        while self.layer_index + 1 >= self.open.len() {
+                            self.open.push(collections::BinaryHeap::new());
+                        }
+
+                        self.open[self.layer_index + 1].push(successor);
+
+                        if new_generated {
+                            self.solution.generated += 1;
+                        }
+                    }
+                }
+
+                self.node_index += 1;
             }
 
-            for transition in generator.applicable_transitions(&node.state) {
-                let cost = transition.eval_cost(node.cost, &node.state, &model.table_registry);
+            self.node_index = 0;
 
-                if primal_bound.is_some() && cost >= primal_bound.unwrap() {
-                    continue;
+            if self.goal_found {
+                self.layer_index = 0;
+                self.no_node = true;
+                self.goal_found = false;
+
+                if self.progressive_parameters.reset {
+                    self.width = self.progressive_parameters.init;
+                } else {
+                    self.width = self.progressive_parameters.increase_width(self.width);
+                }
+            } else if self.layer_index + 1 == self.open.len() {
+                if self.no_node {
+                    break;
                 }
 
-                open.push(Reverse(DijkstraEdge {
-                    cost,
-                    parent: node.clone(),
-                    transition,
-                }));
+                self.layer_index = 0;
+                self.no_node = true;
+                self.width = self.progressive_parameters.increase_width(self.width);
+            } else {
+                self.layer_index += 1;
             }
         }
+
+        self.solution.is_infeasible = self.solution.cost.is_none();
+        self.solution.is_optimal = self.solution.cost.is_some();
+        self.solution.best_bound = self.solution.cost;
+        self.solution.time = self.time_keeper.elapsed_time();
+        self.time_keeper.stop();
+        Ok((self.solution.clone(), true))
+    }
+}
+
+#[cfg(test)]
+mod tests {
+    use super::*;
+
+    #[test]
+    fn progressive_increase_width() {
+        let parameters = ProgressiveSearchParameters {
+            init: 1,
+            step: 2,
+            bound: None,
+            reset: false,
+        };
+        assert_eq!(parameters.increase_width(3), 5);
+    }
+
+    #[test]
+    fn progressive_increase_width_bonded() {
+        let parameters = ProgressiveSearchParameters {
+            init: 1,
+            step: 2,
+            bound: Some(4),
+            reset: false,
+        };
+        assert_eq!(parameters.increase_width(3), 4);
     }
 
-    Solution {
-        is_infeasible: true,
-        expanded,
-        generated: expanded,
-        time: time_keeper.elapsed_time(),
-        ..Default::default()
+    #[test]
+    fn parameters_default() {
+        let parameters = ProgressiveSearchParameters::default();
+        assert_eq!(parameters.init, 1);
+        assert_eq!(parameters.step, 1);
+        assert_eq!(parameters.bound, None);
+        assert!(!parameters.reset);
     }
 }
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/forward_recursion.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/forward_recursion.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 use super::data_structure::{HashableState, SuccessorGenerator};
-use super::search::{Search, Solution};
+use super::search::{Parameters, Search, Solution};
 use super::util;
-use dypdl::{variable_type, TransitionInterface};
+use dypdl::{variable_type, Transition, TransitionInterface};
 use rustc_hash::FxHashMap;
 use std::error::Error;
 use std::fmt;
 use std::rc::Rc;
 use std::str;
 
 /// Forward recursion solver.
@@ -13,63 +13,57 @@
 /// It performs a naive recursion while memoizing all encountered states.
 /// It works only if the state space is acyclic.
 ///
 /// # Examples
 ///
 /// ```
 /// use dypdl::prelude::*;
-/// use dypdl_heuristic_search::search_algorithm::{ForwardRecursion, Search};
-/// use dypdl_heuristic_search::search_algorithm::util::Parameters;
+/// use dypdl_heuristic_search::{Search, Parameters};
+/// use dypdl_heuristic_search::search_algorithm::{ForwardRecursion};
 /// use std::rc::Rc;
 ///
 /// let mut model = Model::default();
 /// let variable = model.add_integer_variable("variable", 0).unwrap();
 /// model.add_base_case(
 ///     vec![Condition::comparison_i(ComparisonOperator::Ge, variable, 1)]
 /// ).unwrap();
 /// let mut increment = Transition::new("increment");
 /// increment.set_cost(IntegerExpression::Cost + 1);
 /// increment.add_effect(variable, variable + 1).unwrap();
 /// model.add_forward_transition(increment.clone()).unwrap();
 ///
 /// let model = Rc::new(model);
 /// let parameters = Parameters::default();
-/// let mut solver = ForwardRecursion::new(model, parameters, None);
+/// let mut solver = ForwardRecursion::new(model, parameters);
 /// let solution = solver.search().unwrap();
 /// assert_eq!(solution.cost, Some(1));
 /// assert_eq!(solution.transitions, vec![increment]);
 /// assert!(!solution.is_infeasible);
 /// ```
 pub struct ForwardRecursion<T>
 where
     T: variable_type::Numeric + fmt::Display + Ord + 'static,
     <T as str::FromStr>::Err: fmt::Debug,
 {
     model: Rc<dypdl::Model>,
-    parameters: util::Parameters<T>,
-    initial_registry_capacity: Option<usize>,
+    parameters: Parameters<T>,
     terminated: bool,
     solution: Solution<T>,
 }
 
 impl<T> ForwardRecursion<T>
 where
     T: variable_type::Numeric + fmt::Display + Ord + 'static,
     <T as str::FromStr>::Err: fmt::Debug,
 {
     /// Create a new forward recursion solver.
-    pub fn new(
-        model: Rc<dypdl::Model>,
-        parameters: util::Parameters<T>,
-        initial_registry_capacity: Option<usize>,
-    ) -> ForwardRecursion<T> {
+    pub fn new(model: Rc<dypdl::Model>, parameters: Parameters<T>) -> ForwardRecursion<T> {
         ForwardRecursion {
             model,
             parameters,
-            initial_registry_capacity,
             terminated: false,
             solution: Solution::default(),
         }
     }
 }
 
 impl<T> Search<T> for ForwardRecursion<T>
@@ -82,18 +76,18 @@
             return Ok((self.solution.clone(), true));
         }
 
         let time_keeper = self
             .parameters
             .time_limit
             .map_or_else(util::TimeKeeper::default, util::TimeKeeper::with_time_limit);
-        let generator = SuccessorGenerator::from_model(self.model.clone(), false);
+        let generator = SuccessorGenerator::<Transition>::from_model(self.model.clone(), false);
         let mut memo = FxHashMap::default();
 
-        if let Some(capacity) = self.initial_registry_capacity {
+        if let Some(capacity) = self.parameters.initial_registry_capacity {
             memo.reserve(capacity);
         }
 
         let state = HashableState::from(self.model.target.clone());
         self.solution.cost = forward_recursion(
             state,
             self.model.as_ref(),
@@ -113,45 +107,49 @@
                     state = transition.apply(&state, &self.model.table_registry);
                     self.solution.transitions.push(transition);
                 }
             }
             _ => {}
         }
 
-        self.solution.is_optimal = self.solution.cost.is_some()
-            && (self.model.reduce_function == dypdl::ReduceFunction::Max
-                || self.model.reduce_function == dypdl::ReduceFunction::Min);
+        if self.model.reduce_function == dypdl::ReduceFunction::Max
+            || self.model.reduce_function == dypdl::ReduceFunction::Min
+        {
+            self.solution.is_optimal = self.solution.cost.is_some();
+            self.solution.best_bound = self.solution.cost;
+        }
+
         self.solution.generated = self.solution.expanded;
         self.solution.is_infeasible = self.solution.cost.is_none();
         self.solution.time = time_keeper.elapsed_time();
 
         Ok((self.solution.clone(), true))
     }
 }
 
 type StateMemo<T> = FxHashMap<HashableState, (Option<T>, Option<Rc<dypdl::Transition>>)>;
 
 /// Performs a naive recursion while memoizing all encountered states.
-pub fn forward_recursion<T: variable_type::Numeric>(
+pub fn forward_recursion<T: variable_type::Numeric + Ord>(
     state: HashableState,
     model: &dypdl::Model,
     generator: &SuccessorGenerator,
     memo: &mut StateMemo<T>,
     time_keeper: &util::TimeKeeper,
     expanded: &mut usize,
 ) -> Option<T> {
-    if model.is_base(&state) {
-        return Some(T::zero());
+    if let Some(cost) = model.eval_base_cost(&state) {
+        return Some(cost);
     }
 
     if let Some((cost, _)) = memo.get(&state) {
         return *cost;
     }
 
-    if time_keeper.check_time_limit() {
+    if time_keeper.check_time_limit(true) {
         return None;
     }
 
     let mut cost = None;
     let mut best_transition = None;
     *expanded += 1;
```

### Comparing `didppy-0.3.4/local_dependencies/dypdl-heuristic-search/src/search_algorithm/search.rs` & `didppy-0.4.0/local_dependencies/dypdl-heuristic-search/src/search_algorithm/search.rs`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,76 @@
-use dypdl::variable_type;
+use super::data_structure::SuccessorGenerator;
+use dypdl::{variable_type::Numeric, Model, Transition, TransitionInterface};
 use std::error::Error;
+use std::{ops::Deref, rc::Rc};
+
+/// Input of a heuristic search solver.
+#[derive(Debug, PartialEq, Clone)]
+pub struct SearchInput<'a, N, V = Transition, D = Rc<V>, R = Rc<dypdl::Model>>
+where
+    V: TransitionInterface,
+    D: Deref<Target = V> + Clone,
+    R: Deref<Target = Model>,
+{
+    /// Root node.
+    pub node: Option<N>,
+    /// Successor generator.
+    pub generator: SuccessorGenerator<V, D, R>,
+    /// Suffix of the solution.
+    pub solution_suffix: &'a [V],
+}
+
+/// Common parameters for heuristic search solvers.
+#[derive(Debug, PartialEq, Clone, Copy, Default)]
+pub struct Parameters<T> {
+    /// Primal bound.
+    pub primal_bound: Option<T>,
+    /// Time limit.
+    pub time_limit: Option<f64>,
+    /// Returns all feasible solutions found.
+    pub get_all_solutions: bool,
+    /// Initial capacity of a data structure saving all states.
+    pub initial_registry_capacity: Option<usize>,
+    /// Suppress log output or not.
+    pub quiet: bool,
+}
 
 /// Information about a solution.
 #[derive(Debug, Default, PartialEq, Clone)]
-pub struct Solution<T: variable_type::Numeric, I = dypdl::Transition> {
+pub struct Solution<T: Numeric, V = Transition> {
     /// Solution cost.
     /// `None` if the model is infeasible.
     pub cost: Option<T>,
     /// Best dual bound.
     pub best_bound: Option<T>,
     /// Solved to optimality or not.
     pub is_optimal: bool,
     /// Infeasible model or not.
     pub is_infeasible: bool,
     /// Transitions corresponding to the solution.
-    pub transitions: Vec<I>,
+    pub transitions: Vec<V>,
     /// Number of expanded nodes.
     pub expanded: usize,
     /// Number of generated nodes.
     pub generated: usize,
     /// Elapsed time in seconds.
     pub time: f64,
     /// Whether to exceed the time limit
     pub time_out: bool,
 }
 
-impl<T: variable_type::Numeric, I> Solution<T, I> {
+impl<T: Numeric, V> Solution<T, V> {
     /// Returns whether the solution would never be improved.
     pub fn is_terminated(&self) -> bool {
         self.is_optimal || self.is_infeasible || self.time_out
     }
 }
 
 /// Trait representing an anytime search algorithm.
-pub trait Search<T: variable_type::Numeric> {
+pub trait Search<T: Numeric> {
     /// Searches for the best solution.
     ///
     /// # Errors
     /// If an error occurs during the search.
     fn search(&mut self) -> Result<Solution<T>, Box<dyn Error>> {
         loop {
             let (solution, terminated) = self.search_next()?;
```

### Comparing `didppy-0.3.4/Cargo.toml` & `didppy-0.4.0/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 [package]
 name = "didppy"
-version = "0.3.4"
+version = "0.4.0"
 edition = "2021"
+rust-version = "1.64"
 description = "Python interface for Dynamic Programming Description Language (DyPDL) and DyPDL solvers."
 license = "MIT OR Apache-2.0"
+authors = ["Ryo Kuroiwa <ryo.kuroiwa@mail.utoronto.ca>"]
+homepage = "https://didp.ai"
+repository = "https://github.com/domain-independent-dp/didp-rs"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "didppy"
 crate-type = ["cdylib"]
 
 [dependencies]
-dypdl = { path = "local_dependencies/dypdl", version = "0.3.4" }
-dypdl-heuristic-search = { path = "local_dependencies/dypdl-heuristic-search", version = "0.3.4" }
+dypdl = { path = "local_dependencies/dypdl", version = "0.4.0" }
+dypdl-heuristic-search = { path = "local_dependencies/dypdl-heuristic-search", version = "0.4.0" }
 rustc-hash = "1.1"
 
 [dependencies.pyo3]
 version = "0.18"
 
 [features]
 extension-module = ["pyo3/extension-module"]
```

### Comparing `didppy-0.3.4/.gitignore` & `didppy-0.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/README.md` & `didppy-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/Makefile` & `didppy-0.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/_static/images/TSPTW.png` & `didppy-0.4.0/docs/_static/images/TSPTW.png`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/_templates/autosummary/class.rst` & `didppy-0.4.0/docs/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/advanced-tutorials/forced-transitions.rst` & `didppy-0.4.0/docs/advanced-tutorials/forced-transitions.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -102,16 +102,16 @@
         came_to_location = scene_to_actors_table.union(already_shot)
         standby = scene_to_actors_table.union(remaining)
         on_location = scene_to_actors_table[s] | (came_to_location & standby)
 
         shoot = dp.Transition(
             name="shoot {}".format(s),
             cost=d[s] * actor_to_cost[on_location] + dp.IntExpr.state_cost(),
-            preconditions=[remaining.contains(s)],
             effects=[(remaining, remaining.remove(s))],
+            preconditions=[remaining.contains(s)],
         )
         model.add_transition(shoot)
 
     model.add_base_case([remaining.is_empty()])
 
     model.add_dual_bound(scene_to_min_cost[remaining])
 
@@ -145,19 +145,19 @@
         already_shot = remaining.complement()
         came_to_location = scene_to_actors_table.union(already_shot)
         standby = scene_to_actors_table.union(remaining)
 
         shoot = dp.Transition(
             name="forced shoot {}".format(s),
             cost=scene_to_min_cost[s] + dp.IntExpr.state_cost(),
+            effects=[(remaining, remaining.remove(s))],
             preconditions=[
                 remaining.contains(s),
                 scene_to_actors_table[s] == (came_to_location & standby),
             ],
-            effects=[(remaining, remaining.remove(s))],
         )
         model.add_transition(shoot, forced=True)
 
 Now, we have an additional precondition, :code:`scene_to_actors_table[s] == (came_to_location & standby)`, which corresponds to :math:`A_s = \bigcup_{s' \in S \setminus Q} A_{s'} \cap \bigcup_{s' \in Q} A_{s'}`.
 When registering this transition to the model, we use the argument :code:`forced=True` to indicate that this transition is a forced transition.
 
 Ordinarily, DIDPPy takes the minimum (or maximum) :code:`cost` over all transitions whose preconditions are satisfied.
```

### Comparing `didppy-0.3.4/docs/advanced-tutorials/general-cost.rst` & `didppy-0.4.0/docs/advanced-tutorials/general-cost.rst`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -78,19 +78,19 @@
     for c in range(n):
         close = dp.Transition(
             name="close {}".format(c),
             cost=dp.max(
                 ((opened & remaining) | (neighbor_table[c] - opened)).len(),
                 dp.IntExpr.state_cost(),
             ),
-            preconditions=[remaining.contains(c)],
             effects=[
                 (remaining, remaining.remove(c)),
                 (opened, opened | neighbor_table[c]),
             ],
+            preconditions=[remaining.contains(c)],
         )
         model.add_transition(close)
 
     model.add_base_case([remaining.is_empty()])
 
     model.add_dual_bound(0)
```

### Comparing `didppy-0.3.4/docs/api-reference.rst` & `didppy-0.4.0/docs/api-reference.rst`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,14 @@
    didppy.CBFS
    didppy.ACPS
    didppy.APPS
    didppy.DBDFS
    didppy.BreadthFirstSearch
    didppy.WeightedAstar
    didppy.ExpressionBeamSearch
-   didppy.Dijkstra
 
 Solution
 --------
 .. autosummary::
    :nosignatures:
    :toctree: _autosummary
```

### Comparing `didppy-0.3.4/docs/conf.py` & `didppy-0.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/debugging/common-mistakes.rst` & `didppy-0.4.0/docs/debugging/common-mistakes.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/debugging/state.rst` & `didppy-0.4.0/docs/debugging/state.rst`

 * *Files 5% similar despite different names*

```diff
@@ -122,33 +122,38 @@
     >>> next_state = transition.apply(state, model)
     >>> next_state[var]
     2
 
 Checking Base Cases
 -------------------
 
-We can check if a state satisfies the base cases with :meth:`~didppy.Model.is_base`.
+We can check if a state satisfies the base cases with :meth:`~didppy.Model.eval_base_cost`.
+If base cases are satisfied, the value of the state is returned.
+Otherwise, :code:`None` is returned.
 
 .. code-block:: python
 
     >>> import didppy as dp
     >>> model = dp.Model()
-    >>> var = model.add_int_var(target=0)
-    >>> model.add_base_case([var >= 2])
+    >>> var = model.add_int_var(target=2)
+    >>> model.add_base_case([var >= 2], cost=2)
     >>> state = model.target_state
-    >>> model.is_base(state)
-    False
+    >>> model.eval_base_cost(state)
+    2 
 
 We can get the base cases with :attr:`~didppy.Model.base_cases`.
+It returns a list of tuples of conditions (a list of conditions) and the cost.
 
 .. code-block:: python
 
     >>> base_cases = model.base_cases
-    >>> base_cases[0][0].eval(state, model)
-    False
+    >>> base_cases[0][0][0].eval(state, model)
+    True
+    >>> base_cases[0][1].eval(state, model)
+    2
 
 The order of base cases is preserved.
 
 Checking State Constraints
 --------------------------
 
 We can check if a state satisfies the state constraints with :meth:`~didppy.Model.check_state_constr`.
```

### Comparing `didppy-0.3.4/docs/debugging/validate.rst` & `didppy-0.4.0/docs/debugging/validate.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/examples.rst` & `didppy-0.4.0/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/index.rst` & `didppy-0.4.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/make.bat` & `didppy-0.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/papers.rst` & `didppy-0.4.0/docs/papers.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/quickstart.rst` & `didppy-0.4.0/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/ref.bib` & `didppy-0.4.0/docs/ref.bib`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/docs/solver-selection.rst` & `didppy-0.4.0/docs/solver-selection.rst`

 * *Files 2% similar despite different names*

```diff
@@ -72,11 +72,10 @@
 * :class:`~didppy.ACPS`
 * :class:`~didppy.APPS`
 * :class:`~didppy.DFBB`
 * :class:`~didppy.DBDFS`
 * :class:`~didppy.BreadthFirstSearch`
 * :class:`~didppy.WeightedAstar`
 * :class:`~didppy.ExpressionBeamSearch`
-* :class:`~didppy.Dijkstra` (also restricted to minimization)
 
 Currently, only :class:`~didppy.ForwardRecursion` supports arbitrary cost expressions.
 However, it does not support cyclic state spaces.
```

### Comparing `didppy-0.3.4/docs/tutorial.rst` & `didppy-0.4.0/docs/tutorial.rst`

 * *Files 3% similar despite different names*

```diff
@@ -120,15 +120,19 @@
 While :math:`i` is an integer, we define it as an :class:`~didppy.ElementVar`  as it represents an element in the set :math:`N`.
 There are some practical differences between :class:`~didppy.ElementVar` and :class:`~didppy.IntVar`:
 
 * :class:`~didppy.ElementVar` is nonnegative.
 * :class:`~didppy.ElementVar` can be used to describe changes and conditions on :class:`~didppy.SetVar`.
 * :class:`~didppy.ElementVar` can be used to access a value of a table (explained later).
 
-While we use the integer cost and an integer variable for :math:`t`, we can use the float cost and a float variable for :code:`t` by using :meth:`~didppy.Model.add_float_var` if we want to use continuous travel time.
+The value of an element variable should be an integer between :code:`0` and :code:`n - 1` as it represents an element in the set :math:`N`.
+However, you may want to make it larger than :code:`n - 1` for some cases (explained later).
+In fact, you can increase its value to an arbitrary large number.
+
+While we use the integer cost and an integer variable for :math:`t`, we can use the float cost and a float variable for :math:`t` by using :meth:`~didppy.Model.add_float_var` if we want to use continuous travel time.
 
 The value of :class:`~didppy.SetVar` is a set of elements in :math:`N`.
 Because the object type of :code:`unvisited` is customer, which has :code:`n` objects, :code:`unvisited` can contain :code:`0` to :code:`n - 1` (**not** :code:`1` **to** :code:`n`).
 
 State variables are defined with their *target values*, values in the target state.
 The objective of the DP model is to compute the value of the target state, i.e., :math:`U = N \setminus \{ 0 \}`, :math:`i = 0`, and :math:`t = 0`.
 The target value of an :class:`~didppy.SetVar` can be a :class:`list` or a :class:`set` in Python.
@@ -199,14 +203,21 @@
 We can use the values of state variables in the **left-hand side state** in :code:`cost`, :code:`preconditions`, and :code:`effects`.
 For example, :code:`location` corresponds to :math:`i` in :math:`V(U, i, t)`, so :code:`travel_time[location, j]` corresponds to :math:`c_{ij}`.
 Because :code:`location` is a state variable, :code:`travel_time[location, j]` is not just an :class:`int` but an *expression* (:class:`~didppy.IntExpr`), whose value is determined given a state inside the solver.
 Therefore, we cannot use :code:`c[location][j]` and need to register :code:`c` to the model as :code:`travel_time`.
 Also, :code:`travel_time[location, j]` must be used instead of :code:`travel_time[location][j]`.
 For :code:`ready_time` and :code:`due_time`, we can actually use :code:`a` and :code:`b` instead because they are not indexed by state variables.
 
+When using a state variable or an expression as an index of a table, the value must not exceed the size of the table:
+you need to make sure that :code:`j` in :code:`travel_time[location, j]` is not larger than :code:`n - 1`.
+If :code:`j > n - 1`, the solver raises an error during solving.
+However, sometimes, you may want to use :code:`j > n - 1` to represent a special case;
+in the knapsack problem in the :doc:`quick start <quickstart>`, :code:`i` becomes :code:`n` in a state where all decisions are made.
+Please make sure that you do not access any table using :code:`i` in such a state.
+
 *Preconditions* :code:`preconditions` make sure that the transition is considered only when :math:`j \in U` (:code:`unvisited.contains(j)`) and :math:`t + c_{ij} \leq b_j` (:code:`time + travel_time[location, j] <= due_time[j]`).
 The value of the left-hand side state is computed by taking the minimum (maximum for maximization) of :code:`cost` over all transitions whose preconditions are satisfied by the state.
 :code:`preconditions` are defined by a :class:`list` of :class:`~didppy.Condition`.
 
 *Effects* :code:`effects` describe how the right-hand side state is computed based on the left-hand side state.
 Effects are described by a :class:`list` of :class:`tuple` of a state variable and its updated value described by an expression.
 
@@ -259,20 +270,18 @@
 is a base case.
 In DIDPPy, a base case is defined by a :class:`list` of :class:`~didppy.Condition`.
 
 .. code-block:: python
 
     model.add_base_case([unvisited.is_empty(), location == 0])
 
-When all conditions in a base case are satisfied, the value of the state is 0, and no further transitions are applied.
+When all conditions in a base case are satisfied, the value of the state is constant, and no further transitions are applied.
+By default, the cost is assumed to be 0, but you can use an expression to compute the value given a state by using the argument :code:`cost` in :meth:`~didppy.Model.add_base_case`.
 We can define multiple independent base cases by calling :meth:`~didppy.Model.add_base_case` multiple times, with different sets of conditions.
-In that case, the value of a state is 0 if any of the base cases is satisfied.
-
-If we want to define conditions with which a state has a non-zero constant value, we need to introduce a dummy transition to the base case, which increases the value by the constant.
-Indeed, the transition :code:`return` can be viewed as such a dummy transition for an equation :math:`V(U, i, t) = c_{i0} \text{ if } U = \emptyset`. 
+In that case, the value of a state is the minimum/maximum of the values of the satisfied base cases in minimization/maximization.
 
 Solving the Model
 -----------------
 
 Now, we have defined a DP model.
 Let's use the :class:`~didppy.CABS` solver to solve this model.
```

### Comparing `didppy-0.3.4/examples/README.md` & `didppy-0.4.0/examples/README.md`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/examples/bin-packing.ipynb` & `didppy-0.4.0/examples/bin-packing.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997369528619529%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}, 6: {'source': {insert: [(9, '    if w[i] == c * 2 / 3\\n')], "*

 * *            'delete: [9]}}}'}*

```diff
@@ -87,15 +87,15 @@
             "id": "c6756083",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
@@ -142,15 +142,15 @@
                 "# The weight in the second term of the second bound.\n",
                 "weight_2_2 = [1 / 2 if w[i] == c / 2 else 0 for i in range(n)]\n",
                 "# The weight in the third bound (truncated to three decimal points).\n",
                 "weight_3 = [\n",
                 "    1.0\n",
                 "    if w[i] > c * 2 / 3\n",
                 "    else 2 / 3 // 0.001 * 1000\n",
-                "    if w[i] == c / 3\n",
+                "    if w[i] == c * 2 / 3\n",
                 "    else 0.5\n",
                 "    if w[i] > c / 3\n",
                 "    else 1 / 3 // 0.001 * 1000\n",
                 "    if w[i] == c / 3\n",
                 "    else 0.0\n",
                 "    for i in range(n)\n",
                 "]"
```

### Comparing `didppy-0.3.4/examples/cvrp.ipynb` & `didppy-0.4.0/examples/cvrp.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998070987654322%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}}"}*

```diff
@@ -78,15 +78,15 @@
             "id": "82147f5f",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
```

### Comparing `didppy-0.3.4/examples/graph-clear.ipynb` & `didppy-0.4.0/examples/graph-clear.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998070987654322%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}}"}*

```diff
@@ -50,15 +50,15 @@
             "id": "76e28461",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
```

### Comparing `didppy-0.3.4/examples/knapsack.ipynb` & `didppy-0.4.0/examples/knapsack.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998421717171717%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}}"}*

```diff
@@ -41,15 +41,15 @@
             "id": "86a40ebc",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
```

### Comparing `didppy-0.3.4/examples/m-pdtsp.ipynb` & `didppy-0.4.0/examples/m-pdtsp.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997745310245311%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}, 4: {'source': {insert: [(9, '# Number of commodities\\n')], "*

 * *            'delete: [9]}}}'}*

```diff
@@ -84,15 +84,15 @@
             "id": "9ae8059b",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
@@ -116,15 +116,15 @@
                 "# Edges\n",
                 "a = {\n",
                 "    (0, 1), (0, 2), (0, 3),\n",
                 "    (1, 2), (1, 3), (1, 4),\n",
                 "    (2, 1), (2, 3), (2, 4),\n",
                 "    (3, 1), (3, 2), (3, 4),\n",
                 "}\n",
-                "# Number of commidities\n",
+                "# Number of commodities\n",
                 "m = 2\n",
                 "# Capacity of the vehicle\n",
                 "q = 5\n",
                 "# Weights\n",
                 "w = [3, 4]\n",
                 "# Pick up points\n",
                 "p = [3, 2]\n",
```

### Comparing `didppy-0.3.4/examples/mosp.ipynb` & `didppy-0.4.0/examples/mosp.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997829861111112%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}, 8: {'source': {insert: [(24, '        "*

 * *            "preconditions=[remaining.contains(c)],\\n')], delete: [20]}}}"}*

```diff
@@ -59,15 +59,15 @@
             "id": "b18442f1",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
@@ -149,19 +149,19 @@
                 "for c in range(n):\n",
                 "    close = dp.Transition(\n",
                 "        name=\"close {}\".format(c),\n",
                 "        cost=dp.max(\n",
                 "            ((opened & remaining) | (neighbor_table[c] - opened)).len(),\n",
                 "            dp.IntExpr.state_cost(),\n",
                 "        ),\n",
-                "        preconditions=[remaining.contains(c)],\n",
                 "        effects=[\n",
                 "            (remaining, remaining.remove(c)),\n",
                 "            (opened, opened | neighbor_table[c]),\n",
                 "        ],\n",
+                "        preconditions=[remaining.contains(c)],\n",
                 "    )\n",
                 "    model.add_transition(close)\n",
                 "\n",
                 "model.add_base_case([remaining.is_empty()])\n",
                 "\n",
                 "model.add_dual_bound(0)"
             ]
```

### Comparing `didppy-0.3.4/examples/salbp-1.ipynb` & `didppy-0.4.0/examples/salbp-1.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9950021043771043%*

 * *Differences: {"'cells'": "{2: {'execution_count': 1, 'outputs': {0: {'text': ['Requirement already satisfied: "*

 * *            'didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}, 4: {'execution_count': 2}, 6: {'execution_count': 3, 'source': "*

 * *            "{insert: [(9, '    if t[i] == c * 2 / 3\\n')], delete: [9]}}, 8: {'execution_count': "*

 * *            "4}, 10: {'execution_count': 5}}"}*

```diff
@@ -73,23 +73,23 @@
             "metadata": {},
             "source": [
                 "## Install DIDPPy"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 1,
             "id": "07b4132e",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
@@ -99,15 +99,15 @@
             "metadata": {},
             "source": [
                 "## Data"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 2,
             "id": "2be75d7f",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Number of tasks\n",
                 "n = 5\n",
                 "# Cycle time\n",
@@ -124,29 +124,29 @@
             "metadata": {},
             "source": [
                 "## Preprocessing"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 3,
             "id": "4b1605e4",
             "metadata": {},
             "outputs": [],
             "source": [
                 "# The weight in the first term of the second bound.\n",
                 "weight_2_1 = [1 if t[i] > c / 2 else 0 for i in range(n)]\n",
                 "# The weight in the second term of the second bound.\n",
                 "weight_2_2 = [1 / 2 if t[i] == c / 2 else 0 for i in range(n)]\n",
                 "# The weight in the third bound (truncated to three decimal points).\n",
                 "weight_3 = [\n",
                 "    1.0\n",
                 "    if t[i] > c * 2 / 3\n",
                 "    else 2 / 3 // 0.001 * 1000\n",
-                "    if t[i] == c / 3\n",
+                "    if t[i] == c * 2 / 3\n",
                 "    else 0.5\n",
                 "    if t[i] > c / 3\n",
                 "    else 1 / 3 // 0.001 * 1000\n",
                 "    if t[i] == c / 3\n",
                 "    else 0.0\n",
                 "    for i in range(n)\n",
                 "]"
@@ -158,15 +158,15 @@
             "metadata": {},
             "source": [
                 "## Modeling"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 4,
             "id": "40abd606",
             "metadata": {},
             "outputs": [],
             "source": [
                 "import math\n",
                 "\n",
                 "import didppy as dp\n",
@@ -239,15 +239,15 @@
             "metadata": {},
             "source": [
                 "## Solving"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 5,
             "id": "ea0484bf",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
```

### Comparing `didppy-0.3.4/examples/single-machine.ipynb` & `didppy-0.4.0/examples/single-machine.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998070987654322%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}}"}*

```diff
@@ -49,15 +49,15 @@
             "id": "ee3d8e3f",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
```

### Comparing `didppy-0.3.4/examples/talent-scheduling.ipynb` & `didppy-0.4.0/examples/talent-scheduling.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997197472629862%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}, 6: {'source': {insert: [(28, '        "*

 * *            "preconditions=[remaining.contains(s)],\\n'), (44, '        effects=[(remaining, "*

 * *            "remaining.remove(s))],\\n')], delete: [48, 27]}}}"}*

```diff
@@ -65,15 +65,15 @@
             "id": "650fc341",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
@@ -142,16 +142,16 @@
                 "    came_to_location = scene_to_actors_table.union(already_shot)\n",
                 "    standby = scene_to_actors_table.union(remaining)\n",
                 "    on_location = scene_to_actors_table[s] | (came_to_location & standby)\n",
                 "\n",
                 "    shoot = dp.Transition(\n",
                 "        name=\"shoot {}\".format(s),\n",
                 "        cost=d[s] * actor_to_cost[on_location] + dp.IntExpr.state_cost(),\n",
-                "        preconditions=[remaining.contains(s)],\n",
                 "        effects=[(remaining, remaining.remove(s))],\n",
+                "        preconditions=[remaining.contains(s)],\n",
                 "    )\n",
                 "    model.add_transition(shoot)\n",
                 "\n",
                 "model.add_base_case([remaining.is_empty()])\n",
                 "\n",
                 "model.add_dual_bound(scene_to_min_cost[remaining])\n",
                 "\n",
@@ -159,19 +159,19 @@
                 "    already_shot = remaining.complement()\n",
                 "    came_to_location = scene_to_actors_table.union(already_shot)\n",
                 "    standby = scene_to_actors_table.union(remaining)\n",
                 "\n",
                 "    shoot = dp.Transition(\n",
                 "        name=\"forced shoot {}\".format(s),\n",
                 "        cost=scene_to_min_cost[s] + dp.IntExpr.state_cost(),\n",
+                "        effects=[(remaining, remaining.remove(s))],\n",
                 "        preconditions=[\n",
                 "            remaining.contains(s),\n",
                 "            scene_to_actors_table[s] == (came_to_location & standby),\n",
                 "        ],\n",
-                "        effects=[(remaining, remaining.remove(s))],\n",
                 "    )\n",
                 "    model.add_transition(shoot, forced=True)"
             ]
         },
         {
             "cell_type": "markdown",
             "id": "4020e1de",
```

### Comparing `didppy-0.3.4/examples/tsptw.ipynb` & `didppy-0.4.0/examples/tsptw.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998070987654322%*

 * *Differences: {"'cells'": "{2: {'outputs': {0: {'text': ['Requirement already satisfied: didppy in "*

 * *            '/home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages '*

 * *            "(0.4.0)\\r\\n']}}}}"}*

```diff
@@ -73,15 +73,15 @@
             "id": "ced536c2",
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Requirement already satisfied: didppy in /home/kuro/didppy-env/lib/python3.10/site-packages (0.3.2)\r\n"
+                        "Requirement already satisfied: didppy in /home/kuro/tidel/code/didp-rs/didppy/.venv/lib/python3.10/site-packages (0.4.0)\r\n"
                     ]
                 }
             ],
             "source": [
                 "!pip install didppy"
             ]
         },
```

### Comparing `didppy-0.3.4/pyproject.toml` & `didppy-0.4.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["maturin>=0.14,<0.15"]
+requires = ["maturin>=1.0,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "didppy"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/acps.rs` & `didppy-0.4.0/src/heuristic_search_solver/apps.rs`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{create_dual_bound_acps, FEvaluatorType, Search};
+use dypdl_heuristic_search::{
+    create_dual_bound_apps, FEvaluatorType, Parameters, ProgressiveSearchParameters, Search,
+};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
-/// Anytime Column Progressive Search (ACPS) solver.
+/// Anytime Pack Progressive Search (APPS) solver.
 ///
-/// This performs ACPS using the dual bound as the heuristic function.
+/// This performs APPS using the dual bound as the heuristic function.
 ///
 /// To apply this solver, the cost must be computed in the form of :code:`x + state_cost`, :code:`x * state_cost`, :code:`didppy.max(x, state_cost)`,
 /// or :code:`didppy.min(x, state_cost)` where, :code:`state_cost` is either of :meth:`IntExpr.state_cost()` and :meth:`FloatExpr.state_cost()`,
 /// and :code:`x` is a value independent of :code:`state_cost`.
-/// Otherwise, it cannot compute the cost correctly and may not produce the optimal solution.
+/// Otherwise, it may not produce the optimal solution.
 ///
 /// Parameters
 /// ----------
 /// model: Model
 ///     DyPDL model to solve.
 /// f_operator: FOperator, default: FOperator.Plus
 ///     Operator to combine a g-value and the dual bound to compute the f-value.
@@ -26,15 +28,16 @@
 ///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
 ///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
 ///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
 /// primal_bound: int, float, or None, default: None
 ///     Primal bound.
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
-///     The count starts when a solver is created.
+/// get_all_solutions: bool, default: False
+///     Return a solution if it is not improving when :code:`search_next()` is called.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
 /// initial_registry_capacity: int, default: 1000000
 ///     Initial size of the data structure storing all generated states.
 /// width_init: int, default: 1
 ///     Initial value of the width.
 /// width_step: int, default: 1
@@ -55,16 +58,16 @@
 ///
 /// References
 /// ----------
 /// Ryo Kuroiwa and J. Christopher Beck.
 /// "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
-/// Sataya Gautam Vadlamudi, Piyush Gaurav, Sandip Aine, and Partha Pratim Chakrabarti.
-/// "Anytime Column Search," Proceedings of AI 2012: Advances in Artificial Intelligence, pp. 254-255, 2012.
+/// Sataya Gautam Vadlamudi, Sandip Aine, Partha Pratim Chakrabarti.
+/// "Anytime Pack Search," Natural Computing, vol. 15(3), pp. 395-414, 2016.
 ///
 /// Examples
 /// --------
 /// Example with :code:`+` operator.
 ///
 /// >>> import didppy as dp
 /// >>> model = dp.Model()
@@ -73,17 +76,17 @@
 /// >>> t = dp.Transition(
 /// ...     name="decrement",
 /// ...     cost=1 + dp.IntExpr.state_cost(),
 /// ...     effects=[(x, x - 1)]
 /// ... )
 /// >>> model.add_transition(t)
 /// >>> model.add_dual_bound(x)
-/// >>> solver = dp.ACPS(model, quiet=True)
+/// >>> solver = dp.APPS(model, quiet=True)
 /// >>> solution = solver.search()
-/// >>> solution.cost
+/// >>> print(solution.cost)
 /// 1
 ///
 /// Example with :code:`max` operator.
 ///
 /// >>> import didppy as dp
 /// >>> model = dp.Model()
 /// >>> x = model.add_int_var(target=2)
@@ -91,53 +94,59 @@
 /// >>> t = dp.Transition(
 /// ...     name="decrement",
 /// ...     cost=dp.max(x, dp.IntExpr.state_cost()),
 /// ...     effects=[(x, x - 1)]
 /// ... )
 /// >>> model.add_transition(t)
 /// >>> model.add_dual_bound(x)
-/// >>> solver = dp.ACPS(model, f_operator=dp.FOperator.Max, quiet=True)
+/// >>> solver = dp.APPS(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
-/// >>> solution.cost
+/// >>> print(solution.cost)
 /// 2
-#[pyclass(unsendable, name = "ACPS")]
+#[pyclass(unsendable, name = "APPS")]
 #[pyo3(
-    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, quiet=False, initial_registry_capacity=1000000, width_init=1, width_step=1, width_bound=None, reset_width=False)"
+    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, get_all_solutions=False, quiet=False, initial_registry_capacity=1000000, width_init=1, width_step=1, width_bound=None, reset_width=False)"
 )]
-pub struct AcpsPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
+pub struct AppsPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
 
 #[pymethods]
-impl AcpsPy {
+impl AppsPy {
     #[new]
     #[pyo3(signature = (
         model,
         f_operator = FOperator::Plus,
         primal_bound = None,
         time_limit = None,
+        get_all_solutions = false,
         quiet = false,
         initial_registry_capacity = 1000000,
         width_init = 1,
         width_step = 1,
         width_bound = None,
         reset_width = false
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         model: &ModelPy,
         f_operator: FOperator,
         primal_bound: Option<&PyAny>,
         time_limit: Option<f64>,
+        get_all_solutions: bool,
         quiet: bool,
         initial_registry_capacity: usize,
         width_init: usize,
         width_step: usize,
         width_bound: Option<usize>,
         reset_width: bool,
-    ) -> PyResult<AcpsPy> {
-        let progressive_parameters = dypdl_heuristic_search::ProgressiveSearchParameters {
+    ) -> PyResult<AppsPy> {
+        if !quiet {
+            println!("Solver: APPS from DIDPPy v{}", env!("CARGO_PKG_VERSION"));
+        }
+
+        let progressive_parameters = ProgressiveSearchParameters {
             init: width_init,
             step: width_step,
             bound: width_bound,
             reset: reset_width,
         };
         let f_evaluator_type = FEvaluatorType::from(f_operator);
 
@@ -145,48 +154,48 @@
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(OrderedContinuous::from(
                     primal_bound.extract::<Continuous>()?,
                 ))
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
+            let parameters = Parameters::<OrderedContinuous> {
                 primal_bound,
                 time_limit,
-                get_all_solutions: false,
+                get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
-            let solver = create_dual_bound_acps::<OrderedContinuous>(
+            let solver = create_dual_bound_apps::<OrderedContinuous>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                progressive_parameters,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
+                progressive_parameters,
             );
-            Ok(AcpsPy(WrappedSolver::Float(solver)))
+            Ok(AppsPy(WrappedSolver::Float(solver)))
         } else {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(primal_bound.extract::<Integer>()?)
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
+            let parameters = Parameters::<Integer> {
                 primal_bound,
                 time_limit,
-                get_all_solutions: false,
+                get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
-            let solver = create_dual_bound_acps::<Integer>(
+            let solver = create_dual_bound_apps::<Integer>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                progressive_parameters,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
+                progressive_parameters,
             );
-            Ok(AcpsPy(WrappedSolver::Int(solver)))
+            Ok(AppsPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
     /// Search for the optimal solution of a DyPDL model.
     ///
@@ -209,15 +218,15 @@
     /// >>> t = dp.Transition(
     /// ...     name="decrement",
     /// ...     cost=1 + dp.IntExpr.state_cost(),
     /// ...     effects=[(x, x - 1)]
     /// ... )
     /// >>> model.add_transition(t)
     /// >>> model.add_dual_bound(x)
-    /// >>> solver = dp.ACPS(model, quiet=True)
+    /// >>> solver = dp.APPS(model, quiet=True)
     /// >>> solution = solver.search()
     /// >>> solution.cost
     /// 1
     #[pyo3(signature = ())]
     fn search(&mut self) -> PyResult<SolutionPy> {
         self.0.search()
     }
@@ -247,15 +256,15 @@
     /// >>> t = dp.Transition(
     /// ...     name="decrement",
     /// ...     cost=1 + dp.IntExpr.state_cost(),
     /// ...     effects=[(x, x - 1)]
     /// ... )
     /// >>> model.add_transition(t)
     /// >>> model.add_dual_bound(x)
-    /// >>> solver = dp.ACPS(model, quiet=True)
+    /// >>> solver = dp.APPS(model, quiet=True)
     /// >>> solution, terminated = solver.search_next()
     /// >>> solution.cost
     /// 1
     /// >>> terminated
     /// True
     #[pyo3(signature = ())]
     fn search_next(&mut self) -> PyResult<(SolutionPy, bool)> {
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/apps.rs` & `didppy-0.4.0/src/heuristic_search_solver/acps.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{create_dual_bound_apps, FEvaluatorType, Search};
+use dypdl_heuristic_search::{
+    create_dual_bound_acps, FEvaluatorType, Parameters, ProgressiveSearchParameters, Search,
+};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
-/// Anytime Pack Progressive Search (APPS) solver.
+/// Anytime Column Progressive Search (ACPS) solver.
 ///
-/// This performs APPS using the dual bound as the heuristic function.
+/// This performs ACPS using the dual bound as the heuristic function.
 ///
 /// To apply this solver, the cost must be computed in the form of :code:`x + state_cost`, :code:`x * state_cost`, :code:`didppy.max(x, state_cost)`,
 /// or :code:`didppy.min(x, state_cost)` where, :code:`state_cost` is either of :meth:`IntExpr.state_cost()` and :meth:`FloatExpr.state_cost()`,
 /// and :code:`x` is a value independent of :code:`state_cost`.
-/// Otherwise, it may not produce the optimal solution.
+/// Otherwise, it cannot compute the cost correctly and may not produce the optimal solution.
 ///
 /// Parameters
 /// ----------
 /// model: Model
 ///     DyPDL model to solve.
 /// f_operator: FOperator, default: FOperator.Plus
 ///     Operator to combine a g-value and the dual bound to compute the f-value.
@@ -26,15 +28,14 @@
 ///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
 ///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
 ///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
 /// primal_bound: int, float, or None, default: None
 ///     Primal bound.
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
-///     The count starts when a solver is created.
 /// get_all_solutions: bool, default: False
 ///     Return a solution if it is not improving when :code:`search_next()` is called.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
 /// initial_registry_capacity: int, default: 1000000
 ///     Initial size of the data structure storing all generated states.
 /// width_init: int, default: 1
@@ -57,16 +58,16 @@
 ///
 /// References
 /// ----------
 /// Ryo Kuroiwa and J. Christopher Beck.
 /// "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
 /// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
-/// Sataya Gautam Vadlamudi, Sandip Aine, Partha Pratim Chakrabarti.
-/// "Anytime Pack Search," Natural Computing, vol. 15(3), pp. 395-414, 2016.
+/// Sataya Gautam Vadlamudi, Piyush Gaurav, Sandip Aine, and Partha Pratim Chakrabarti.
+/// "Anytime Column Search," Proceedings of AI 2012: Advances in Artificial Intelligence, pp. 254-255, 2012.
 ///
 /// Examples
 /// --------
 /// Example with :code:`+` operator.
 ///
 /// >>> import didppy as dp
 /// >>> model = dp.Model()
@@ -75,17 +76,17 @@
 /// >>> t = dp.Transition(
 /// ...     name="decrement",
 /// ...     cost=1 + dp.IntExpr.state_cost(),
 /// ...     effects=[(x, x - 1)]
 /// ... )
 /// >>> model.add_transition(t)
 /// >>> model.add_dual_bound(x)
-/// >>> solver = dp.APPS(model, quiet=True)
+/// >>> solver = dp.ACPS(model, quiet=True)
 /// >>> solution = solver.search()
-/// >>> print(solution.cost)
+/// >>> solution.cost
 /// 1
 ///
 /// Example with :code:`max` operator.
 ///
 /// >>> import didppy as dp
 /// >>> model = dp.Model()
 /// >>> x = model.add_int_var(target=2)
@@ -93,26 +94,26 @@
 /// >>> t = dp.Transition(
 /// ...     name="decrement",
 /// ...     cost=dp.max(x, dp.IntExpr.state_cost()),
 /// ...     effects=[(x, x - 1)]
 /// ... )
 /// >>> model.add_transition(t)
 /// >>> model.add_dual_bound(x)
-/// >>> solver = dp.APPS(model, f_operator=dp.FOperator.Max, quiet=True)
+/// >>> solver = dp.ACPS(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
-/// >>> print(solution.cost)
+/// >>> solution.cost
 /// 2
-#[pyclass(unsendable, name = "APPS")]
+#[pyclass(unsendable, name = "ACPS")]
 #[pyo3(
-    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, quiet=False, initial_registry_capacity=1000000, width_init=1, width_step=1, width_bound=None, reset_width=False)"
+    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, get_all_solutions=False, quiet=False, initial_registry_capacity=1000000, width_init=1, width_step=1, width_bound=None, reset_width=False)"
 )]
-pub struct AppsPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
+pub struct AcpsPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
 
 #[pymethods]
-impl AppsPy {
+impl AcpsPy {
     #[new]
     #[pyo3(signature = (
         model,
         f_operator = FOperator::Plus,
         primal_bound = None,
         time_limit = None,
         get_all_solutions = false,
@@ -132,16 +133,20 @@
         get_all_solutions: bool,
         quiet: bool,
         initial_registry_capacity: usize,
         width_init: usize,
         width_step: usize,
         width_bound: Option<usize>,
         reset_width: bool,
-    ) -> PyResult<AppsPy> {
-        let progressive_parameters = dypdl_heuristic_search::ProgressiveSearchParameters {
+    ) -> PyResult<AcpsPy> {
+        if !quiet {
+            println!("Solver: ACPS from DIDPPy v{}", env!("CARGO_PKG_VERSION"));
+        }
+
+        let progressive_parameters = ProgressiveSearchParameters {
             init: width_init,
             step: width_step,
             bound: width_bound,
             reset: reset_width,
         };
         let f_evaluator_type = FEvaluatorType::from(f_operator);
 
@@ -149,48 +154,48 @@
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(OrderedContinuous::from(
                     primal_bound.extract::<Continuous>()?,
                 ))
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
+            let parameters = Parameters::<OrderedContinuous> {
                 primal_bound,
                 time_limit,
                 get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
-            let solver = create_dual_bound_apps::<OrderedContinuous>(
+            let solver = create_dual_bound_acps::<OrderedContinuous>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                progressive_parameters,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
+                progressive_parameters,
             );
-            Ok(AppsPy(WrappedSolver::Float(solver)))
+            Ok(AcpsPy(WrappedSolver::Float(solver)))
         } else {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(primal_bound.extract::<Integer>()?)
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
+            let parameters = Parameters::<Integer> {
                 primal_bound,
                 time_limit,
                 get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
-            let solver = create_dual_bound_apps::<Integer>(
+            let solver = create_dual_bound_acps::<Integer>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                progressive_parameters,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
+                progressive_parameters,
             );
-            Ok(AppsPy(WrappedSolver::Int(solver)))
+            Ok(AcpsPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
     /// Search for the optimal solution of a DyPDL model.
     ///
@@ -213,15 +218,15 @@
     /// >>> t = dp.Transition(
     /// ...     name="decrement",
     /// ...     cost=1 + dp.IntExpr.state_cost(),
     /// ...     effects=[(x, x - 1)]
     /// ... )
     /// >>> model.add_transition(t)
     /// >>> model.add_dual_bound(x)
-    /// >>> solver = dp.APPS(model, quiet=True)
+    /// >>> solver = dp.ACPS(model, quiet=True)
     /// >>> solution = solver.search()
     /// >>> solution.cost
     /// 1
     #[pyo3(signature = ())]
     fn search(&mut self) -> PyResult<SolutionPy> {
         self.0.search()
     }
@@ -251,15 +256,15 @@
     /// >>> t = dp.Transition(
     /// ...     name="decrement",
     /// ...     cost=1 + dp.IntExpr.state_cost(),
     /// ...     effects=[(x, x - 1)]
     /// ... )
     /// >>> model.add_transition(t)
     /// >>> model.add_dual_bound(x)
-    /// >>> solver = dp.APPS(model, quiet=True)
+    /// >>> solver = dp.ACPS(model, quiet=True)
     /// >>> solution, terminated = solver.search_next()
     /// >>> solution.cost
     /// 1
     /// >>> terminated
     /// True
     #[pyo3(signature = ())]
     fn search_next(&mut self) -> PyResult<(SolutionPy, bool)> {
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/breadth_first_search.rs` & `didppy-0.4.0/src/heuristic_search_solver/breadth_first_search.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{create_dual_bound_breadth_first_search, FEvaluatorType, Search};
+use dypdl_heuristic_search::{
+    create_dual_bound_breadth_first_search, BrfsParameters, FEvaluatorType, Parameters, Search,
+};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
 /// Breadth-first search solver.
 ///
 /// This performs breadth-first search using the dual bound as the heuristic function.
 ///
@@ -84,15 +86,15 @@
 /// >>> model.add_dual_bound(x)
 /// >>> solver = dp.BreadthFirstSearch(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 2
 #[pyclass(unsendable, name = "BreadthFirstSearch")]
 #[pyo3(
-    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, quiet=False, keep_all_layers=False)"
+    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, get_all_solutions=False, quiet=False, initial_registry_capacity=1000000, keep_all_layers=False)"
 )]
 pub struct BreadthFirstSearchPy(
     WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>,
 );
 
 #[pymethods]
 impl BreadthFirstSearchPy {
@@ -114,56 +116,67 @@
         primal_bound: Option<&PyAny>,
         time_limit: Option<f64>,
         get_all_solutions: bool,
         quiet: bool,
         initial_registry_capacity: usize,
         keep_all_layers: bool,
     ) -> PyResult<BreadthFirstSearchPy> {
+        if !quiet {
+            println!(
+                "Solver: BreadthFirstSearch from DIDPPy v{}",
+                env!("CARGO_PKG_VERSION")
+            );
+        }
+
         let f_evaluator_type = FEvaluatorType::from(f_operator);
 
         if model.float_cost() {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(OrderedContinuous::from(
                     primal_bound.extract::<Continuous>()?,
                 ))
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
-                primal_bound,
-                time_limit,
-                get_all_solutions,
-                quiet,
+            let parameters = BrfsParameters {
+                keep_all_layers,
+                parameters: Parameters::<OrderedContinuous> {
+                    primal_bound,
+                    time_limit,
+                    get_all_solutions,
+                    quiet,
+                    initial_registry_capacity: Some(initial_registry_capacity),
+                },
             };
             let solver = create_dual_bound_breadth_first_search::<OrderedContinuous>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
                 f_evaluator_type,
-                keep_all_layers,
-                Some(initial_registry_capacity),
             );
             Ok(BreadthFirstSearchPy(WrappedSolver::Float(solver)))
         } else {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(primal_bound.extract::<Integer>()?)
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
-                primal_bound,
-                time_limit,
-                get_all_solutions,
-                quiet,
+            let parameters = BrfsParameters {
+                keep_all_layers,
+                parameters: Parameters::<Integer> {
+                    primal_bound,
+                    time_limit,
+                    get_all_solutions,
+                    quiet,
+                    initial_registry_capacity: Some(initial_registry_capacity),
+                },
             };
             let solver = create_dual_bound_breadth_first_search::<Integer>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
                 f_evaluator_type,
-                keep_all_layers,
-                Some(initial_registry_capacity),
             );
             Ok(BreadthFirstSearchPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/caasdy.rs` & `didppy-0.4.0/src/heuristic_search_solver/caasdy.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{create_caasdy, FEvaluatorType, Search};
+use dypdl_heuristic_search::{create_caasdy, FEvaluatorType, Parameters, Search};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
 /// Cost-Algebraic A* Solver for DyPDL (CAASDy).
 ///
 /// This performs cost-algebraic A* using the dual bound as the heuristic function.
 ///
@@ -26,15 +26,14 @@
 ///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
 ///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
 ///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
 /// primal_bound: int, float, or None, default: None
 ///     Primal bound on the optimal cost (upper/lower bound for minimization/maximization).
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
-///     The count starts when a solver is created.
 /// get_all_solutions: bool, default: False
 ///     Return a new solution even if it is not improving when :code:`search_next()` is called.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
 /// initial_registry_capacity: int, default: 1000000
 ///     Initial size of the data structure storing all generated states.
 ///
@@ -96,15 +95,15 @@
 /// >>> model.add_dual_bound(x)
 /// >>> solver = dp.CAASDy(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 2
 #[pyclass(unsendable, name = "CAASDy")]
 #[pyo3(
-    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, quiet=False, initial_registry_capacity=1000000)"
+    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, get_all_solutions=False, quiet=False, initial_registry_capacity=1000000)"
 )]
 pub struct CaasdyPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
 
 #[pymethods]
 impl CaasdyPy {
     #[new]
     #[pyo3(signature = (
@@ -121,54 +120,58 @@
         f_operator: FOperator,
         primal_bound: Option<&PyAny>,
         time_limit: Option<f64>,
         get_all_solutions: bool,
         quiet: bool,
         initial_registry_capacity: usize,
     ) -> PyResult<CaasdyPy> {
+        if !quiet {
+            println!("Solver: CAASDy from DIDPPy v{}", env!("CARGO_PKG_VERSION"));
+        }
+
         let f_evaluator_type = FEvaluatorType::from(f_operator);
 
         if model.float_cost() {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(OrderedContinuous::from(
                     primal_bound.extract::<Continuous>()?,
                 ))
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
+            let parameters = Parameters::<OrderedContinuous> {
                 primal_bound,
                 time_limit,
                 get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
             let solver = create_caasdy(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
             );
             Ok(CaasdyPy(WrappedSolver::Float(solver)))
         } else {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(primal_bound.extract::<Integer>()?)
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
+            let parameters = Parameters::<Integer> {
                 primal_bound,
                 time_limit,
                 get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
             let solver = create_caasdy(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
             );
             Ok(CaasdyPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/cabs.rs` & `didppy-0.4.0/src/heuristic_search_solver/cabs.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{create_dual_bound_cabs, FEvaluatorType, Search};
+use dypdl_heuristic_search::{
+    create_dual_bound_cabs, BeamSearchParameters, CabsParameters, FEvaluatorType, Parameters,
+    Search,
+};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
 /// Complete Anytime Beam Search (CABS) solver.
 ///
 /// This performs CABS using the dual bound as the heuristic function.
 ///
@@ -30,19 +33,20 @@
 ///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
 ///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
 ///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
 /// initial_beam_size: int, default: 1
 ///     Initial beam size.
 /// keep_all_layers: bool, default: False
 ///     Keep all layers of the search graph for duplicate detection in memory.
+/// max_beam_size: int or None, default: None
+///     Maximum beam size.
 /// primal_bound: int, float, or None, default: None
 ///     Primal bound.
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
-///     The count starts when a solver is created.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
 ///
 /// Raises
 /// ------
 /// TypeError
 ///     If :code:`primal_bound` is :code:`float` and :code:`model` is float cost.
@@ -94,82 +98,100 @@
 /// >>> model.add_dual_bound(x)
 /// >>> solver = dp.CABS(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 2
 #[pyclass(unsendable, name = "CABS")]
 #[pyo3(
-    text_signature = "(model, f_operator=0, keep_all_layers=False, primal_bound=None, time_limit=None, quiet=False)"
+    text_signature = "(model, f_operator=0, initial_beam_size=1, keep_all_layers=False, max_beam_size=None, primal_bound=None, time_limit=None, quiet=False)"
 )]
 pub struct CabsPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
 
 #[pymethods]
 impl CabsPy {
     #[new]
     #[pyo3(signature = (
         model,
         f_operator = FOperator::Plus,
         initial_beam_size = 1,
         keep_all_layers = false,
+        max_beam_size = None,
         primal_bound = None,
         time_limit = None,
         quiet = false
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         model: &ModelPy,
         f_operator: FOperator,
         initial_beam_size: usize,
         keep_all_layers: bool,
+        max_beam_size: Option<usize>,
         primal_bound: Option<&PyAny>,
         time_limit: Option<f64>,
         quiet: bool,
     ) -> PyResult<CabsPy> {
+        if !quiet {
+            println!("Solver: CABS from DIDPPy v{}", env!("CARGO_PKG_VERSION"));
+        }
+
         let f_evaluator_type = FEvaluatorType::from(f_operator);
 
         if model.float_cost() {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(OrderedContinuous::from(
                     primal_bound.extract::<Continuous>()?,
                 ))
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
-                primal_bound,
-                time_limit,
-                get_all_solutions: false,
-                quiet,
+            let parameters = CabsParameters {
+                max_beam_size,
+                beam_search_parameters: BeamSearchParameters {
+                    beam_size: initial_beam_size,
+                    keep_all_layers,
+                    parameters: Parameters::<OrderedContinuous> {
+                        primal_bound,
+                        time_limit,
+                        get_all_solutions: false,
+                        quiet,
+                        initial_registry_capacity: None,
+                    },
+                },
             };
             let solver = create_dual_bound_cabs::<OrderedContinuous>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
                 f_evaluator_type,
-                initial_beam_size,
-                keep_all_layers,
             );
             Ok(CabsPy(WrappedSolver::Float(solver)))
         } else {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(primal_bound.extract::<Integer>()?)
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
-                primal_bound,
-                time_limit,
-                get_all_solutions: false,
-                quiet,
+            let parameters = CabsParameters {
+                max_beam_size,
+                beam_search_parameters: BeamSearchParameters {
+                    beam_size: initial_beam_size,
+                    keep_all_layers,
+                    parameters: Parameters::<Integer> {
+                        primal_bound,
+                        time_limit,
+                        get_all_solutions: false,
+                        quiet,
+                        initial_registry_capacity: None,
+                    },
+                },
             };
             let solver = create_dual_bound_cabs::<Integer>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
                 f_evaluator_type,
-                initial_beam_size,
-                keep_all_layers,
             );
             Ok(CabsPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/cbfs.rs` & `didppy-0.4.0/src/heuristic_search_solver/cbfs.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{create_dual_bound_cbfs, FEvaluatorType, Search};
+use dypdl_heuristic_search::{create_dual_bound_cbfs, FEvaluatorType, Parameters, Search};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
 /// Cyclic Best-First Search (CBFS) solver.
 ///
 /// This performs CBFS using the dual bound as the heuristic function.
 ///
@@ -26,15 +26,14 @@
 ///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
 ///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
 ///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
 /// primal_bound: int, float, or None, default: None
 ///     Primal bound.
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
-///     The count starts when a solver is created.
 /// get_all_solutions: bool, default: False
 ///     Return a solution if it is not improving when :code:`search_next()` is called.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
 /// initial_registry_capacity: int, default: 1000000
 ///     Initial size of the data structure storing all generated states.
 ///
@@ -92,15 +91,15 @@
 /// >>> model.add_dual_bound(x)
 /// >>> solver = dp.CBFS(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 2
 #[pyclass(unsendable, name = "CBFS")]
 #[pyo3(
-    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, quiet=False, initial_registry_capacity=1000000)"
+    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, get_all_solutions=False, quiet=False, initial_registry_capacity=1000000)"
 )]
 pub struct CbfsPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
 
 #[pymethods]
 impl CbfsPy {
     #[new]
     #[pyo3(signature = (
@@ -117,54 +116,58 @@
         f_operator: FOperator,
         primal_bound: Option<&PyAny>,
         time_limit: Option<f64>,
         get_all_solutions: bool,
         quiet: bool,
         initial_registry_capacity: usize,
     ) -> PyResult<CbfsPy> {
+        if !quiet {
+            println!("Solver: CBFS from DIDPPy v{}", env!("CARGO_PKG_VERSION"));
+        }
+
         let f_evaluator_type = FEvaluatorType::from(f_operator);
 
         if model.float_cost() {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(OrderedContinuous::from(
                     primal_bound.extract::<Continuous>()?,
                 ))
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
+            let parameters = Parameters::<OrderedContinuous> {
                 primal_bound,
                 time_limit,
                 get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
             let solver = create_dual_bound_cbfs::<OrderedContinuous>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
             );
             Ok(CbfsPy(WrappedSolver::Float(solver)))
         } else {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(primal_bound.extract::<Integer>()?)
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
+            let parameters = Parameters::<Integer> {
                 primal_bound,
                 time_limit,
                 get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
             let solver = create_dual_bound_cbfs::<Integer>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
             );
             Ok(CbfsPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/dbdfs.rs` & `didppy-0.4.0/src/heuristic_search_solver/dbdfs.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{create_dual_bound_dbdfs, FEvaluatorType, Search};
+use dypdl_heuristic_search::{
+    create_dual_bound_dbdfs, DbdfsParameters, FEvaluatorType, Parameters, Search,
+};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
 /// Discrepancy-Based Depth-First Search (DBDFS) solver.
 ///
 /// This performs DBDFS using the dual bound as the heuristic function.
 ///
@@ -26,15 +28,14 @@
 ///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
 ///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
 ///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
 /// primal_bound: int, float, or None, default: None
 ///     Primal bound.
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
-///     The count starts when a solver is created.
 /// get_all_solutions: bool, default: False
 ///     Return a solution if it is not improving when :code:`search_next()` is called.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
 /// initial_registry_capacity: int, default: 1000000
 ///     Initial size of the data structure storing all generated states.
 /// width: int, default: 1
@@ -94,15 +95,15 @@
 /// >>> model.add_dual_bound(x)
 /// >>> solver = dp.DBDFS(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 2
 #[pyclass(unsendable, name = "DBDFS")]
 #[pyo3(
-    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, quiet=False, initial_registry_capacity=1000000, width=1)"
+    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, get_all_solutions=False, quiet=False, initial_registry_capacity=1000000, width=1)"
 )]
 pub struct DbdfsPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
 
 #[pymethods]
 impl DbdfsPy {
     #[new]
     #[pyo3(signature = (
@@ -122,56 +123,64 @@
         primal_bound: Option<&PyAny>,
         time_limit: Option<f64>,
         get_all_solutions: bool,
         quiet: bool,
         initial_registry_capacity: usize,
         width: usize,
     ) -> PyResult<DbdfsPy> {
+        if !quiet {
+            println!("Solver: DBDFS from DIDPPy v{}", env!("CARGO_PKG_VERSION"));
+        }
+
         let f_evaluator_type = FEvaluatorType::from(f_operator);
 
         if model.float_cost() {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(OrderedContinuous::from(
                     primal_bound.extract::<Continuous>()?,
                 ))
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
-                primal_bound,
-                time_limit,
-                get_all_solutions,
-                quiet,
+            let parameters = DbdfsParameters::<OrderedContinuous> {
+                width,
+                parameters: Parameters::<OrderedContinuous> {
+                    primal_bound,
+                    time_limit,
+                    get_all_solutions,
+                    quiet,
+                    initial_registry_capacity: Some(initial_registry_capacity),
+                },
             };
             let solver = create_dual_bound_dbdfs::<OrderedContinuous>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                width,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
             );
             Ok(DbdfsPy(WrappedSolver::Float(solver)))
         } else {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(primal_bound.extract::<Integer>()?)
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
-                primal_bound,
-                time_limit,
-                get_all_solutions,
-                quiet,
+            let parameters = DbdfsParameters::<Integer> {
+                width,
+                parameters: Parameters::<Integer> {
+                    primal_bound,
+                    time_limit,
+                    get_all_solutions,
+                    quiet,
+                    initial_registry_capacity: Some(initial_registry_capacity),
+                },
             };
             let solver = create_dual_bound_dbdfs::<Integer>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                width,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
             );
             Ok(DbdfsPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/dfbb.rs` & `didppy-0.4.0/src/heuristic_search_solver/weighted_astar.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,80 +1,76 @@
 use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{create_dual_bound_dfbb, FEvaluatorType, Search};
+use dypdl_heuristic_search::{
+    create_dual_bound_weighted_astar, FEvaluatorType, Parameters, Search,
+};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
-/// Depth-first branch-and-bound (DFBB) solver.
+/// Weighted A* solver.
 ///
-/// This performs DFBB using the dual bound as the heuristic function.
+/// This performs weighted A* using the dual bound as the heuristic function.
 ///
 /// To apply this solver, the cost must be computed in the form of :code:`x + state_cost`, :code:`x * state_cost`, :code:`didppy.max(x, state_cost)`,
 /// or :code:`didppy.min(x, state_cost)` where, :code:`state_cost` is either of :meth:`IntExpr.state_cost()` and :meth:`FloatExpr.state_cost()`,
 /// and :code:`x` is a value independent of :code:`state_cost`.
+/// In addition, the model must be minimization.
 /// Otherwise, it cannot compute the cost correctly and may not produce the optimal solution.
 ///
 /// Parameters
 /// ----------
 /// model: Model
-///     DyPDL model to solve.
+///     DyPDL model to solve`time_limit` or .
+/// weight: int or float
+///     Weight of the h-value.
 /// f_operator: FOperator, default: FOperator.Plus
 ///     Operator to combine a g-value and the dual bound to compute the f-value.
 ///     If the cost is computed by :code:`+`, this should be :attr:`~FOperator.Plus`.
 ///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
 ///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
 ///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
 /// primal_bound: int, float, or None, default: None
 ///     Primal bound.
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
-///     The count starts when a solver is created.
 /// get_all_solutions: bool, default: False
 ///     Return a solution if it is not improving when :code:`search_next()` is called.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
 /// initial_registry_capacity: int, default: 1000000
 ///     Initial size of the data structure storing all generated states.
-/// bfs_tie_breaking: bool, default: False
-///     Visit child nodes in the order of the f-values.
 ///
 /// Raises
 /// ------
 /// TypeError
 ///     If the type of :code:`primal_bound` and the cost type of :code:`model` are different.
 /// OverflowError
 ///     If :code:`initial_registry_capacity` is negative.
 /// PanicException
 ///     If :code:`time_limit` is negative.
 ///
-/// References
-/// ----------
-/// Ryo Kuroiwa and J. Christopher Beck.
-/// "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
-/// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
-///
 /// Examples
-/// -------
+/// --------
 /// Example with :code:`+` operator.
 ///
 /// >>> import didppy as dp
 /// >>> model = dp.Model()
 /// >>> x = model.add_int_var(target=1)
 /// >>> model.add_base_case([x == 0])
 /// >>> t = dp.Transition(
 /// ...     name="decrement",
 /// ...     cost=1 + dp.IntExpr.state_cost(),
 /// ...     effects=[(x, x - 1)]
 /// ... )
 /// >>> model.add_transition(t)
 /// >>> model.add_dual_bound(x)
-/// >>> solver = dp.DFBB(model, quiet=True)
+/// >>> solver = dp.WeightedAstar(model, weight=1.5, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 1
 ///
 /// Example with :code:`max` operator.
 ///
 /// >>> import didppy as dp
@@ -84,98 +80,107 @@
 /// >>> t = dp.Transition(
 /// ...     name="decrement",
 /// ...     cost=dp.max(x, dp.IntExpr.state_cost()),
 /// ...     effects=[(x, x - 1)]
 /// ... )
 /// >>> model.add_transition(t)
 /// >>> model.add_dual_bound(x)
-/// >>> solver = dp.DFBB(model, f_operator=dp.FOperator.Max, quiet=True)
+/// >>> solver = dp.WeightedAstar(model, weight=1.5, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 2
-#[pyclass(unsendable, name = "DFBB")]
+#[pyclass(unsendable, name = "WeightedAstar")]
 #[pyo3(
-    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, quiet=False, bfs_tie_breaking=False)"
+    text_signature = "(model, weight, f_operator=0, primal_bound=None, time_limit=None, get_all_solutions=False, quiet=False, initial_registry_capacity=1000000)"
 )]
-pub struct DfbbPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
+pub struct WeightedAstarPy(
+    WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>,
+);
 
 #[pymethods]
-impl DfbbPy {
+impl WeightedAstarPy {
     #[new]
     #[pyo3(signature = (
         model,
+        weight,
         f_operator = FOperator::Plus,
         primal_bound = None,
         time_limit = None,
         get_all_solutions = false,
         quiet = false,
-        initial_registry_capacity = 1000000,
-        bfs_tie_breaking = false
+        initial_registry_capacity = 1000000
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         model: &ModelPy,
+        weight: Continuous,
         f_operator: FOperator,
         primal_bound: Option<&PyAny>,
         time_limit: Option<f64>,
         get_all_solutions: bool,
         quiet: bool,
         initial_registry_capacity: usize,
-        bfs_tie_breaking: bool,
-    ) -> PyResult<DfbbPy> {
+    ) -> PyResult<WeightedAstarPy> {
+        if !quiet {
+            println!(
+                "Solver: WeightedAstar from DIDPPy v{}",
+                env!("CARGO_PKG_VERSION")
+            );
+        }
+
         let f_evaluator_type = FEvaluatorType::from(f_operator);
 
         if model.float_cost() {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(OrderedContinuous::from(
                     primal_bound.extract::<Continuous>()?,
                 ))
             } else {
                 None
             };
             let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
                 primal_bound,
                 time_limit,
                 get_all_solutions,
+                initial_registry_capacity: Some(initial_registry_capacity),
                 quiet,
             };
-            let solver = create_dual_bound_dfbb::<OrderedContinuous>(
+            let solver = create_dual_bound_weighted_astar(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                bfs_tie_breaking,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
+                weight,
             );
-            Ok(DfbbPy(WrappedSolver::Float(solver)))
+            Ok(WeightedAstarPy(WrappedSolver::Float(solver)))
         } else {
             let primal_bound = if let Some(primal_bound) = primal_bound {
                 Some(primal_bound.extract::<Integer>()?)
             } else {
                 None
             };
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
+            let parameters = Parameters::<Integer> {
                 primal_bound,
                 time_limit,
                 get_all_solutions,
+                initial_registry_capacity: Some(initial_registry_capacity),
                 quiet,
             };
-            let solver = create_dual_bound_dfbb::<Integer>(
+            let solver = create_dual_bound_weighted_astar(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                bfs_tie_breaking,
                 f_evaluator_type,
-                Some(initial_registry_capacity),
+                weight,
             );
-            Ok(DfbbPy(WrappedSolver::Int(solver)))
+            Ok(WeightedAstarPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
-    /// Search for the optimal solution of a DyPDL model.
+    /// Search for a bounded-suboptimal solution of a DyPDL model.
     ///
     /// Returns
     /// -------
     /// Solution
     ///     Solution.
     ///
     /// Raises
@@ -192,15 +197,15 @@
     /// >>> t = dp.Transition(
     /// ...     name="decrement",
     /// ...     cost=1 + dp.IntExpr.state_cost(),
     /// ...     effects=[(x, x - 1)]
     /// ... )
     /// >>> model.add_transition(t)
     /// >>> model.add_dual_bound(x)
-    /// >>> solver = dp.DFBB(model, quiet=True)
+    /// >>> solver = dp.WeightedAstar(model, weight=1.5, quiet=True)
     /// >>> solution = solver.search()
     /// >>> solution.cost
     /// 1
     #[pyo3(signature = ())]
     fn search(&mut self) -> PyResult<SolutionPy> {
         self.0.search()
     }
@@ -230,15 +235,15 @@
     /// >>> t = dp.Transition(
     /// ...     name="decrement",
     /// ...     cost=1 + dp.IntExpr.state_cost(),
     /// ...     effects=[(x, x - 1)]
     /// ... )
     /// >>> model.add_transition(t)
     /// >>> model.add_dual_bound(x)
-    /// >>> solver = dp.DFBB(model, quiet=True)
+    /// >>> solver = dp.WeightedAstar(model, weight=1.5, quiet=True)
     /// >>> solution, terminated = solver.search_next()
     /// >>> solution.cost
     /// 1
     /// >>> terminated
     /// True
     #[pyo3(signature = ())]
     fn search_next(&mut self) -> PyResult<(SolutionPy, bool)> {
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/dijkstra.rs` & `didppy-0.4.0/src/heuristic_search_solver/dfbb.rs`

 * *Files 27% similar despite different names*

```diff
@@ -1,59 +1,79 @@
+use super::f_operator::FOperator;
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{Dijkstra, Search};
+use dypdl_heuristic_search::{create_dual_bound_dfbb, FEvaluatorType, Parameters, Search};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
-/// Dijkstra's algorithm solver.
+/// Depth-first branch-and-bound (DFBB) solver.
 ///
-/// This performs Dijkstra's algorithm.
+/// This performs DFBB using the dual bound as the heuristic function.
 ///
 /// To apply this solver, the cost must be computed in the form of :code:`x + state_cost`, :code:`x * state_cost`, :code:`didppy.max(x, state_cost)`,
 /// or :code:`didppy.min(x, state_cost)` where, :code:`state_cost` is either of :meth:`IntExpr.state_cost()` and :meth:`FloatExpr.state_cost()`,
 /// and :code:`x` is a value independent of :code:`state_cost`.
-/// In addition, the model must be minimization.
 /// Otherwise, it cannot compute the cost correctly and may not produce the optimal solution.
 ///
 /// Parameters
 /// ----------
 /// model: Model
 ///     DyPDL model to solve.
+/// f_operator: FOperator, default: FOperator.Plus
+///     Operator to combine a g-value and the dual bound to compute the f-value.
+///     If the cost is computed by :code:`+`, this should be :attr:`~FOperator.Plus`.
+///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
+///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
+///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
+/// primal_bound: int, float, or None, default: None
+///     Primal bound.
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
+/// get_all_solutions: bool, default: False
+///     Return a solution if it is not improving when :code:`search_next()` is called.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
 /// initial_registry_capacity: int, default: 1000000
 ///     Initial size of the data structure storing all generated states.
-/// lazy: bool, default: False
-///     Lazily generate a state when it is expanded.
+/// bfs_tie_breaking: bool, default: False
+///     Visit child nodes in the order of the f-values.
 ///
 /// Raises
 /// ------
+/// TypeError
+///     If the type of :code:`primal_bound` and the cost type of :code:`model` are different.
 /// OverflowError
 ///     If :code:`initial_registry_capacity` is negative.
+/// PanicException
+///     If :code:`time_limit` is negative.
+///
+/// References
+/// ----------
+/// Ryo Kuroiwa and J. Christopher Beck.
+/// "Solving Domain-Independent Dynamic Programming with Anytime Heuristic Search,"
+/// Proceedings of the 33rd International Conference on Automated Planning and Scheduling (ICAPS), 2023.
 ///
 /// Examples
-/// --------
+/// -------
 /// Example with :code:`+` operator.
 ///
 /// >>> import didppy as dp
 /// >>> model = dp.Model()
 /// >>> x = model.add_int_var(target=1)
 /// >>> model.add_base_case([x == 0])
 /// >>> t = dp.Transition(
 /// ...     name="decrement",
 /// ...     cost=1 + dp.IntExpr.state_cost(),
 /// ...     effects=[(x, x - 1)]
 /// ... )
 /// >>> model.add_transition(t)
 /// >>> model.add_dual_bound(x)
-/// >>> solver = dp.Dijkstra(model, quiet=True)
+/// >>> solver = dp.DFBB(model, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 1
 ///
 /// Example with :code:`max` operator.
 ///
 /// >>> import didppy as dp
@@ -63,69 +83,92 @@
 /// >>> t = dp.Transition(
 /// ...     name="decrement",
 /// ...     cost=dp.max(x, dp.IntExpr.state_cost()),
 /// ...     effects=[(x, x - 1)]
 /// ... )
 /// >>> model.add_transition(t)
 /// >>> model.add_dual_bound(x)
-/// >>> solver = dp.Dijkstra(model, f_operator=dp.FOperator.Max, quiet=True)
+/// >>> solver = dp.DFBB(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 2
-#[pyclass(unsendable, name = "Dijkstra")]
+#[pyclass(unsendable, name = "DFBB")]
 #[pyo3(
-    text_signature = "(model, time_limit=None, quiet=False, initial_registry_capacity=1000000, lazy=False)"
+    text_signature = "(model, f_operator=0, primal_bound=None, time_limit=None, get_all_solutions=False, quiet=False, initial_registry_capacity=1000000)"
 )]
-pub struct DijkstraPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
+pub struct DfbbPy(WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>);
 
 #[pymethods]
-impl DijkstraPy {
+impl DfbbPy {
     #[new]
     #[pyo3(signature = (
         model,
+        f_operator = FOperator::Plus,
+        primal_bound = None,
         time_limit = None,
+        get_all_solutions = false,
         quiet = false,
         initial_registry_capacity = 1000000,
-        lazy = false
     ))]
+    #[allow(clippy::too_many_arguments)]
     fn new(
         model: &ModelPy,
+        f_operator: FOperator,
+        primal_bound: Option<&PyAny>,
         time_limit: Option<f64>,
+        get_all_solutions: bool,
         quiet: bool,
         initial_registry_capacity: usize,
-        lazy: bool,
-    ) -> DijkstraPy {
+    ) -> PyResult<DfbbPy> {
+        if !quiet {
+            println!("Solver: DFBB from DIDPPy v{}", env!("CARGO_PKG_VERSION"));
+        }
+
+        let f_evaluator_type = FEvaluatorType::from(f_operator);
+
         if model.float_cost() {
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
-                primal_bound: None,
+            let primal_bound = if let Some(primal_bound) = primal_bound {
+                Some(OrderedContinuous::from(
+                    primal_bound.extract::<Continuous>()?,
+                ))
+            } else {
+                None
+            };
+            let parameters = Parameters::<OrderedContinuous> {
+                primal_bound,
                 time_limit,
-                get_all_solutions: false,
+                get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
-            let solver = Box::new(Dijkstra::<OrderedContinuous>::new(
+            let solver = create_dual_bound_dfbb::<OrderedContinuous>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                lazy,
-                Some(initial_registry_capacity),
-            ));
-            DijkstraPy(WrappedSolver::Float(solver))
+                f_evaluator_type,
+            );
+            Ok(DfbbPy(WrappedSolver::Float(solver)))
         } else {
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
-                primal_bound: None,
+            let primal_bound = if let Some(primal_bound) = primal_bound {
+                Some(primal_bound.extract::<Integer>()?)
+            } else {
+                None
+            };
+            let parameters = Parameters::<Integer> {
+                primal_bound,
                 time_limit,
-                get_all_solutions: false,
+                get_all_solutions,
                 quiet,
+                initial_registry_capacity: Some(initial_registry_capacity),
             };
-            let solver = Box::new(Dijkstra::<Integer>::new(
+            let solver = create_dual_bound_dfbb::<Integer>(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                lazy,
-                Some(initial_registry_capacity),
-            ));
-            DijkstraPy(WrappedSolver::Int(solver))
+                f_evaluator_type,
+            );
+            Ok(DfbbPy(WrappedSolver::Int(solver)))
         }
     }
 
     /// search()
     ///
     /// Search for the optimal solution of a DyPDL model.
     ///
@@ -148,16 +191,56 @@
     /// >>> t = dp.Transition(
     /// ...     name="decrement",
     /// ...     cost=1 + dp.IntExpr.state_cost(),
     /// ...     effects=[(x, x - 1)]
     /// ... )
     /// >>> model.add_transition(t)
     /// >>> model.add_dual_bound(x)
-    /// >>> solver = dp.Dijkstra(model, quiet=True)
+    /// >>> solver = dp.DFBB(model, quiet=True)
     /// >>> solution = solver.search()
-    /// >>> print(solution.cost)
+    /// >>> solution.cost
     /// 1
     #[pyo3(signature = ())]
     fn search(&mut self) -> PyResult<SolutionPy> {
         self.0.search()
     }
+
+    /// search_next()
+    ///
+    /// Search for the next solution of a DyPDL model.
+    ///
+    /// Returns
+    /// -------
+    /// solution: Solution
+    ///     Solution.
+    /// terminated: bool
+    ///     Whether the search is terminated.
+    ///
+    /// Raises
+    /// ------
+    /// PanicException
+    ///     If the model is invalid.
+    ///
+    /// Examples
+    /// --------
+    /// >>> import didppy as dp
+    /// >>> model = dp.Model()
+    /// >>> x = model.add_int_var(target=1)
+    /// >>> model.add_base_case([x == 0])
+    /// >>> t = dp.Transition(
+    /// ...     name="decrement",
+    /// ...     cost=1 + dp.IntExpr.state_cost(),
+    /// ...     effects=[(x, x - 1)]
+    /// ... )
+    /// >>> model.add_transition(t)
+    /// >>> model.add_dual_bound(x)
+    /// >>> solver = dp.DFBB(model, quiet=True)
+    /// >>> solution, terminated = solver.search_next()
+    /// >>> solution.cost
+    /// 1
+    /// >>> terminated
+    /// True
+    #[pyo3(signature = ())]
+    fn search_next(&mut self) -> PyResult<(SolutionPy, bool)> {
+        self.0.search_next()
+    }
 }
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/expression_beam_search.rs` & `didppy-0.4.0/src/heuristic_search_solver/expression_beam_search.rs`

 * *Files 6% similar despite different names*

```diff
@@ -26,42 +26,49 @@
 ///
 /// Parameters
 /// ----------
 /// model: Model
 ///     DyPDL model to solve.
 /// beam_size: int
 ///     Beam size.
-/// h_expression: IntExpr, IntVar, IntResourceVar, FloatExpr, FloatVar, FloatResourceVar, int, float, or None, default: None
-///     Expression to compute an h-value.
 /// custom_cost_dict: dict[str, Union[IntExpr|IntVar|IntResourceVar|FloatExpr|FloatVar|FloatResourceVar|int|float] or None, default: None
 ///     Expressions to compute g-values.
 ///     A g-value is the cost of the path from the target state to the current state.
 ///     A key is the name of a transition, and the value is an expression to compute a g-value.
 ///     An expression can use :code:`IntExpr.state_cost()` or :code:`FloatExpr.state_cost()`, which returns the current g-value.
 ///     If the name of a transition is not included, its cost expression is used.
 ///     If :code:`None`, the cost expressions in the DyPDL model are used for all transitions.
+/// h_expression: IntExpr, IntVar, IntResourceVar, FloatExpr, FloatVar, FloatResourceVar, int, float, or None, default: None
+///     Expression to compute an h-value.
 /// f_operator: FOperator, default: FOperator.Plus
-///     Operator to combine a g-value and the dual bound to compute the f-value.
+///     Operator to combine a g-value and the base cost.
 ///     If the cost is computed by :code:`+`, this should be :attr:`~FOperator.Plus`.
 ///     If the cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
 ///     If the cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
 ///     If the cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
 ///     This solver keeps top :code:`b` best nodes with regard to f-values at each depth.
+/// custom_f_operator: FOperator, default: FOperator.Plus
+///     Operator to combine a g-value and the h-value to compute the f-value.
+///     If the custom cost is computed by :code:`+`, this should be :attr:`~FOperator.Plus`.
+///     If the custom cost is computed by :code:`*`, this should be :attr:`~FOperator.Product`.
+///     If the custom cost is computed by :code:`max`, this should be :attr:`~FOperator.Max`.
+///     If the custom cost is computed by :code:`min`, this should be :attr:`~FOperator.Min`.
+///     This solver keeps top :code:`b` best nodes with regard to f-values at each depth.
 /// maximize: bool, default: False
 ///     Maximize f-values or not.
 ///     Greater f-values are better if :code:`True`, and smaller are better if :code:`False`.
 /// keep_all_layers: bool, default: False
 ///     Keep all layers of the search graph for duplicate detection in memory.
-/// float_custom_cost: bool or None, default: None
-///     Use continuous values for g-, h-, and f-values.
-///     The cost type of the model is used if :code:`None`.
 /// time_limit: int, float, or None, default: None
 ///     Time limit.
 /// quiet: bool, default: False
 ///     Suppress the log output or not.
+/// float_custom_cost: bool or None, default: None
+///     Use continuous values for g-, h-, and f-values.
+///     The cost type of the model is used if :code:`None`.
 ///
 /// Raises
 /// ------
 /// TypeError
 ///     If the custom cost type is int and :code:`h_evaluator` or a value in :code:`custom_cost_dict` is :code:`FloatExpr`, :code:`FloatVar`, :code:`FloatResourceVar`, or :code:`float`.
 /// OverflowError
 ///     If :code:`beam_size` is negative.
@@ -101,15 +108,15 @@
 /// >>> model.add_dual_bound(x)
 /// >>> solver = dp.ExpressionBeamSearch(model, f_operator=dp.FOperator.Max, quiet=True)
 /// >>> solution = solver.search()
 /// >>> print(solution.cost)
 /// 2
 #[pyclass(unsendable, name = "ExpressionBeamSearch")]
 #[pyo3(
-    text_signature = "(model, beam_size, h_expression=None, custom_cost_dict=None, f_operator=0, maximize=False, keep_all_layers=False, float_custom_cost=None, time_limit=None, quiet=False)"
+    text_signature = "(model, beam_size, custom_cost_dict=None, h_expression=None, f_operator=0, custom_f_operator=0, maximize=False, keep_all_layers=False, time_limit=None, quiet=False, float_custom_cost=None)"
 )]
 pub struct ExpressionBeamSearchPy(
     WrappedSolver<Box<dyn Search<Integer>>, Box<dyn Search<OrderedContinuous>>>,
 );
 
 impl ExpressionBeamSearchPy {
     fn create_custom_cost_vectors(
@@ -158,33 +165,42 @@
     #[new]
     #[pyo3(signature = (
         model,
         beam_size,
         custom_cost_dict = None,
         h_expression = None,
         f_operator = FOperator::Plus,
+        custom_f_operator = FOperator::Plus,
         maximize = false,
         keep_all_layers = false,
         time_limit = None,
         quiet = false,
         float_custom_cost = None,
     ))]
     #[allow(clippy::too_many_arguments)]
     fn new(
         model: &ModelPy,
         beam_size: usize,
         custom_cost_dict: Option<HashMap<String, CostUnion>>,
         h_expression: Option<CostUnion>,
         f_operator: FOperator,
+        custom_f_operator: FOperator,
         maximize: bool,
         keep_all_layers: bool,
         time_limit: Option<f64>,
         quiet: bool,
         float_custom_cost: Option<bool>,
     ) -> PyResult<ExpressionBeamSearchPy> {
+        if !quiet {
+            println!(
+                "Solver: ExpressionBeamSearch from DIDPPy v{}",
+                env!("CARGO_PKG_VERSION")
+            );
+        }
+
         let custom_cost_type =
             float_custom_cost.map_or(model.inner_as_ref().cost_type, |float_custom_cost| {
                 if float_custom_cost {
                     CostType::Continuous
                 } else {
                     CostType::Integer
                 }
@@ -196,105 +212,99 @@
             CostExpression::from(expression).simplify(&model.inner_as_ref().table_registry)
         });
         let f_evaluator_type = FEvaluatorType::from(f_operator);
         let custom_expression_parameters = CustomExpressionParameters {
             custom_costs,
             forced_custom_costs,
             h_expression,
+            f_evaluator_type: FEvaluatorType::from(custom_f_operator),
             custom_cost_type,
+            maximize,
         };
 
         match (model.float_cost(), custom_cost_type) {
             (true, CostType::Continuous) => {
                 let parameters = BeamSearchParameters {
                     beam_size,
-                    maximize,
-                    f_pruning: false,
-                    f_bound: None,
                     keep_all_layers,
                     parameters: Parameters::<OrderedContinuous> {
                         primal_bound: None,
                         time_limit,
                         get_all_solutions: false,
                         quiet,
+                        initial_registry_capacity: None,
                     },
                 };
                 let solver = Box::new(
                     ExpressionBeamSearch::<OrderedContinuous, OrderedContinuous>::new(
                         Rc::new(model.inner_as_ref().clone()),
                         parameters,
-                        custom_expression_parameters,
                         f_evaluator_type,
+                        custom_expression_parameters,
                     ),
                 );
                 Ok(ExpressionBeamSearchPy(WrappedSolver::Float(solver)))
             }
             (true, CostType::Integer) => {
                 let parameters = BeamSearchParameters {
                     beam_size,
-                    maximize,
-                    f_pruning: false,
-                    f_bound: None,
                     keep_all_layers,
                     parameters: Parameters::<OrderedContinuous> {
                         primal_bound: None,
                         time_limit,
                         get_all_solutions: false,
                         quiet,
+                        initial_registry_capacity: None,
                     },
                 };
                 let solver = Box::new(ExpressionBeamSearch::<OrderedContinuous, Integer>::new(
                     Rc::new(model.inner_as_ref().clone()),
                     parameters,
-                    custom_expression_parameters,
                     f_evaluator_type,
+                    custom_expression_parameters,
                 ));
                 Ok(ExpressionBeamSearchPy(WrappedSolver::Float(solver)))
             }
             (false, CostType::Continuous) => {
                 let parameters = BeamSearchParameters {
                     beam_size,
-                    maximize,
-                    f_pruning: false,
-                    f_bound: None,
                     keep_all_layers,
                     parameters: Parameters::<Integer> {
                         primal_bound: None,
                         time_limit,
                         get_all_solutions: false,
+                        initial_registry_capacity: None,
                         quiet,
                     },
                 };
                 let solver = Box::new(ExpressionBeamSearch::<Integer, OrderedContinuous>::new(
                     Rc::new(model.inner_as_ref().clone()),
                     parameters,
-                    custom_expression_parameters,
                     f_evaluator_type,
+                    custom_expression_parameters,
                 ));
                 Ok(ExpressionBeamSearchPy(WrappedSolver::Int(solver)))
             }
             (false, CostType::Integer) => {
                 let parameters = BeamSearchParameters {
                     beam_size,
-                    maximize,
-                    f_pruning: false,
-                    f_bound: None,
                     keep_all_layers,
                     parameters: Parameters::<Integer> {
                         primal_bound: None,
                         time_limit,
                         get_all_solutions: false,
+                        initial_registry_capacity: None,
                         quiet,
                     },
                 };
                 let solver = Box::new(ExpressionBeamSearch::<Integer, Integer>::new(
                     Rc::new(model.inner_as_ref().clone()),
                     parameters,
-                    custom_expression_parameters,
                     f_evaluator_type,
+                    custom_expression_parameters,
                 ));
                 Ok(ExpressionBeamSearchPy(WrappedSolver::Int(solver)))
             }
         }
     }
 
     /// search()
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/f_operator.rs` & `didppy-0.4.0/src/heuristic_search_solver/f_operator.rs`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 use dypdl_heuristic_search::FEvaluatorType;
 use pyo3::prelude::*;
 
 /// An enum representing an operator to compute the f-value combining an h-value and a g-value.
 ///
-/// :attr:`~FOperator.Plus` (0): f = g + h
+/// :attr:`~FOperator.Plus` (0): :code:`f = g + h`
 ///
-/// :attr:`~FOperator.Max` (1): f = max(g, h)
+/// :attr:`~FOperator.Max` (1): :code:`f = max(g, h)`
 ///
-/// :attr:`~FOperator.Min` (2): f = min(g, h)
+/// :attr:`~FOperator.Min` (2): :code:`f = min(g, h)`
 ///
-/// :attr:`~FOperator.Product` (3): f = g * h
+/// :attr:`~FOperator.Product` (3): :code:`f = g * h`
 ///
-/// :attr:`~FOperator.Overwrite` (4): f = h
+/// :attr:`~FOperator.Overwrite` (4): :code:`f = h`
 #[pyclass(name = "FOperator")]
 #[derive(Debug, PartialEq, Eq, Clone)]
 pub enum FOperator {
-    /// f = g + h
+    /// :code:`f = g + h`
     Plus = 0,
-    /// f = max(g, h)
+    /// :code:`f = max(g, h)`
     Max = 1,
-    /// f = min(g, h)
+    /// :code:`f = min(g, h)`
     Min = 2,
-    /// f = g * h
+    /// :code:`f = g * h`
     Product = 3,
-    /// f = h
+    /// :code:`f = h`
     Overwrite = 4,
 }
 
 impl From<FOperator> for FEvaluatorType {
     fn from(f_operator: FOperator) -> Self {
         match f_operator {
             FOperator::Plus => FEvaluatorType::Plus,
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/forward_recursion.rs` & `didppy-0.4.0/src/heuristic_search_solver/forward_recursion.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 use super::wrapped_solver::{SolutionPy, WrappedSolver};
 use crate::model::ModelPy;
 use dypdl::prelude::*;
 use dypdl::variable_type::OrderedContinuous;
-use dypdl_heuristic_search::{ForwardRecursion, Search};
+use dypdl_heuristic_search::{ForwardRecursion, Parameters, Search};
 use pyo3::prelude::*;
 use std::rc::Rc;
 
 /// Forward recursion solver.
 ///
 /// This performs forward recursion while memoizing encountered states.
 ///
@@ -45,38 +45,45 @@
     ))]
     fn new(
         model: &ModelPy,
         time_limit: Option<f64>,
         quiet: bool,
         initial_registry_capacity: usize,
     ) -> ForwardRecursionPy {
+        if !quiet {
+            println!(
+                "Solver: ForwardRecursion from DIDPPy v{}",
+                env!("CARGO_PKG_VERSION")
+            );
+        }
+
         if model.float_cost() {
-            let parameters = dypdl_heuristic_search::Parameters::<OrderedContinuous> {
+            let parameters = Parameters::<OrderedContinuous> {
                 primal_bound: None,
                 time_limit,
                 get_all_solutions: false,
+                initial_registry_capacity: Some(initial_registry_capacity),
                 quiet,
             };
             let solver = Box::new(ForwardRecursion::<OrderedContinuous>::new(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                Some(initial_registry_capacity),
             ));
             ForwardRecursionPy(WrappedSolver::Float(solver))
         } else {
-            let parameters = dypdl_heuristic_search::Parameters::<Integer> {
+            let parameters = Parameters::<Integer> {
                 primal_bound: None,
                 time_limit,
                 get_all_solutions: false,
+                initial_registry_capacity: Some(initial_registry_capacity),
                 quiet,
             };
             let solver = Box::new(ForwardRecursion::<Integer>::new(
                 Rc::new(model.inner_as_ref().clone()),
                 parameters,
-                Some(initial_registry_capacity),
             ));
             ForwardRecursionPy(WrappedSolver::Int(solver))
         }
     }
 
     /// search()
     ///
```

### Comparing `didppy-0.3.4/src/heuristic_search_solver/wrapped_solver.rs` & `didppy-0.4.0/src/heuristic_search_solver/wrapped_solver.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/src/heuristic_search_solver.rs` & `didppy-0.4.0/src/heuristic_search_solver.rs`

 * *Files 6% similar despite different names*

```diff
@@ -4,28 +4,26 @@
 mod apps;
 mod breadth_first_search;
 mod caasdy;
 mod cabs;
 mod cbfs;
 mod dbdfs;
 mod dfbb;
-mod dijkstra;
 mod expression_beam_search;
 mod f_operator;
 mod forward_recursion;
 mod weighted_astar;
 mod wrapped_solver;
 
 pub use acps::AcpsPy;
 pub use apps::AppsPy;
 pub use breadth_first_search::BreadthFirstSearchPy;
 pub use caasdy::CaasdyPy;
 pub use cabs::CabsPy;
 pub use cbfs::CbfsPy;
 pub use dbdfs::DbdfsPy;
 pub use dfbb::DfbbPy;
-pub use dijkstra::DijkstraPy;
 pub use expression_beam_search::ExpressionBeamSearchPy;
 pub use f_operator::FOperator;
 pub use forward_recursion::ForwardRecursionPy;
 pub use weighted_astar::WeightedAstarPy;
 pub use wrapped_solver::SolutionPy;
```

### Comparing `didppy-0.3.4/src/lib.rs` & `didppy-0.4.0/src/lib.rs`

 * *Files 4% similar despite different names*

```diff
@@ -58,11 +58,11 @@
     m.add_class::<heuristic_search_solver::CbfsPy>()?;
     m.add_class::<heuristic_search_solver::ExpressionBeamSearchPy>()?;
     m.add_class::<heuristic_search_solver::AcpsPy>()?;
     m.add_class::<heuristic_search_solver::AppsPy>()?;
     m.add_class::<heuristic_search_solver::DbdfsPy>()?;
     m.add_class::<heuristic_search_solver::ForwardRecursionPy>()?;
     m.add_class::<heuristic_search_solver::BreadthFirstSearchPy>()?;
-    m.add_class::<heuristic_search_solver::DijkstraPy>()?;
     m.add_class::<heuristic_search_solver::WeightedAstarPy>()?;
+    m.add("__version__", env!("CARGO_PKG_VERSION"))?;
     Ok(())
 }
```

### Comparing `didppy-0.3.4/src/model/expression.rs` & `didppy-0.4.0/src/model/expression.rs`

 * *Files 0% similar despite different names*

```diff
@@ -2300,14 +2300,23 @@
         match self {
             Self::Int(expr) => expr.into_py(py),
             Self::Float(expr) => expr.into_py(py),
         }
     }
 }
 
+impl From<CostExpression> for IntOrFloatExpr {
+    fn from(expr: CostExpression) -> Self {
+        match expr {
+            CostExpression::Integer(expr) => Self::Int(IntExprPy::from(expr)),
+            CostExpression::Continuous(expr) => Self::Float(FloatExprPy::from(expr)),
+        }
+    }
+}
+
 /// Integer expression.
 ///
 /// If an arithmetic operator (:code:`+`, :code:`-`, :code:`*`, :code:`//`, :code:`%`) with an :class:`IntExpr`, :class:`IntVar`, :class:`IntResourceVar`, or :class:`int` is applied, a new :class:`IntExpr` is returned.
 /// For division (`/`) and power (`**`), a :class:`FloatExpr` is returned.
 /// If an arithmetic operator with an :class:`FloatExpr`, :class:`FloatVar`, :class:`FloatResourceVar`, or :class:`float` is applied, a :class:`FloatExpr` is returned.
 /// If :func:`abs` is applied, a new :class:`IntExpr` is returned.
 ///
@@ -11331,8 +11340,26 @@
         let result = Python::with_gil(|py| {
             let x = x.into_py(py);
             let y = y.into_py(py);
             condition.if_then_else(x.as_ref(py), y.as_ref(py))
         });
         assert!(result.is_err());
     }
+
+    #[test]
+    fn int_or_float_expr_from_cost_expression_int() {
+        let expression = CostExpression::from(0);
+        assert_eq!(
+            IntOrFloatExpr::from(expression),
+            IntOrFloatExpr::Int(IntExprPy::from(IntegerExpression::Constant(0)))
+        )
+    }
+
+    #[test]
+    fn int_or_float_expr_from_cost_expression_float() {
+        let expression = CostExpression::from(0.0);
+        assert_eq!(
+            IntOrFloatExpr::from(expression),
+            IntOrFloatExpr::Float(FloatExprPy::from(ContinuousExpression::Constant(0.0)))
+        )
+    }
 }
```

### Comparing `didppy-0.3.4/src/model/state.rs` & `didppy-0.4.0/src/model/state.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/src/model/table.rs` & `didppy-0.4.0/src/model/table.rs`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/src/model.rs` & `didppy-0.4.0/src/model.rs`

 * *Files 1% similar despite different names*

```diff
@@ -658,15 +658,14 @@
     /// ElementVar
     ///     The variable.
     ///
     /// Raises
     /// ------
     /// RuntimeError
     ///     If :code:`object_type` is not included in the model.
-    ///     If :code:`target` is greater than or equal to the number of the objects.
     ///     If :code:`name` is already used.
     /// OverflowError
     ///     If :code:`target` is negative.
     ///
     /// Examples
     /// --------
     /// >>> import didppy as dp
@@ -756,15 +755,14 @@
     /// ElementResourceVar
     ///     The variable.
     ///
     /// Raises
     /// ------
     /// RuntimeError
     ///     If :code:`object_type` is not included in the model.
-    ///     If :code:`target` is greater than or equal to the number of the objects.
     ///     If :code:`name` is already used.
     /// OverflowError
     ///     If :code:`target` is negative.
     ///
     /// Examples
     /// --------
     /// >>> import didppy as dp
@@ -1364,15 +1362,14 @@
     ///
     /// Raises
     /// ------
     /// TypeError
     ///     If the types of :code:`var` and :code:`target` mismatch.
     /// RuntimeError
     ///     If the variable is not included in the model.
-    ///     If :code:`var` is :class:`ElementVar` or :class:`ElementResourceVar` and :code:`target` is greater than or equal to the number of the associated objects.
     ///     If :code:`var` is :class:`SetVar` and a value in :code:`target` is greater than or equal to the number of the associated objects.
     /// OverflowError
     ///     If :code:`var` is :class:`ElementVar` or :class:`ElementResourceVar` and :code:`target` is negative.
     ///     If :code:`var` is :class:`SetVar` and a value in :code:`target` is negative.
     ///
     /// Examples
     /// --------
@@ -1587,58 +1584,86 @@
     /// >>> model.check_state_constr(model.target_state)
     /// True
     #[pyo3(signature = (state))]
     fn check_state_constr(&self, state: &state::StatePy) -> bool {
         self.0.check_constraints(state.inner_as_ref())
     }
 
-    /// list of list of Conditions : Base cases.
+    /// list of tuple of list of Conditions and IntExpr or FloatExpr : Base cases with their cost expressions.
     #[getter]
-    fn base_cases(&self) -> Vec<Vec<ConditionPy>> {
+    fn base_cases(&self) -> Vec<(Vec<ConditionPy>, IntOrFloatExpr)> {
         self.0
             .base_cases
             .iter()
             .map(|base_case| {
-                Vec::from(base_case.clone())
-                    .into_iter()
-                    .map(|condition| ConditionPy::from(Condition::from(condition)))
-                    .collect()
+                let (conditions, cost) = base_case.clone().into();
+                (
+                    conditions.into_iter().map(ConditionPy::from).collect(),
+                    cost.map_or(
+                        IntOrFloatExpr::Int(IntExprPy::from(IntegerExpression::from(0))),
+                        IntOrFloatExpr::from,
+                    ),
+                )
             })
             .collect()
     }
 
-    /// add_base_case(conditions)
+    /// add_base_case(conditions, cost)
     ///
     /// Adds a base case to the model.
     ///
     /// Parameters
     /// ----------
     /// conditions: list of Condition
     ///     Base case.
+    /// cost: IntExpr, IntVar, IntResourceVar, FloatExpr, FloatVar, FloatResourceVar, int, float, or None, default: None
+    ///     Expression to compute the value of a base state.
+    ///     This expression can use state variables in the base state.
+    ///     :func:`IntExpr.state_cost()` and :func:`FloatExpr.state_cost()` are not allowed.
+    ///     If None, the value of the base state is 0.
+    ///     When a state satisfies multiple base cases, the minimum/maximum value is used in minimization/maximization.
     ///
     /// Raises
     /// ------
     /// RuntimeError
     ///     If one of :code:`conditions` is invalid.
     ///     E.g., it uses a variable not included in the model or the cost of the transitioned state.
     /// PanicException
     ///     If an index of a table is out of range.
+    ///     If :func:`IntExpr.state_cost()` or :func:`FloatExpr.state_cost()` is used in :code:`cost`.
     ///
     /// Examples
     /// --------
     /// >>> import didppy as dp
     /// >>> model = dp.Model()
     /// >>> var = model.add_int_var(target=4)
     /// >>> model.add_base_case([var >= 2, var <= 5])
     /// >>> model.is_base(model.target_state)
     /// True
-    #[pyo3(signature = (conditions))]
-    fn add_base_case(&mut self, conditions: Vec<ConditionPy>) -> PyResult<()> {
+    /// >>> model.eval_base_cost(model.target_state)
+    /// 0
+    /// >>> model.add_base_case([var >= 3, var <= 4], cost=-var)
+    /// >>> model.eval_base_cost(model.target_state)
+    /// -4
+    #[pyo3(signature = (conditions, cost = None))]
+    #[pyo3(text_signature = "(conditions, cost=None)")]
+    fn add_base_case(
+        &mut self,
+        conditions: Vec<ConditionPy>,
+        cost: Option<CostUnion>,
+    ) -> PyResult<()> {
         let conditions = conditions.into_iter().map(|x| x.into()).collect();
-        match self.0.add_base_case(conditions) {
+
+        let result = if let Some(cost) = cost {
+            self.0.add_base_case_with_cost(conditions, cost)
+        } else {
+            self.0.add_base_case(conditions)
+        };
+
+        match result {
             Ok(_) => Ok(()),
             Err(err) => Err(PyRuntimeError::new_err(err.to_string())),
         }
     }
 
     /// is_base(state)
     ///
@@ -1668,14 +1693,55 @@
     /// >>> model.is_base(model.target_state)
     /// True
     #[pyo3(signature = (state))]
     fn is_base(&self, state: &state::StatePy) -> bool {
         self.0.is_base(state.inner_as_ref())
     }
 
+    /// is_base(state)
+    ///
+    /// Evaluates the cost of a base state.
+    ///
+    /// Parameters
+    /// ----------
+    /// state: State
+    ///     State to be evaluated.
+    ///
+    /// Returns
+    /// -------
+    /// int, float, or None
+    ///     None if the state is a base state.
+    ///
+    /// Raises
+    /// ------
+    /// PanicException
+    ///     If base cases are invalid.
+    ///
+    /// Examples
+    /// --------
+    /// >>> import didppy as dp
+    /// >>> model = dp.Model()
+    /// >>> var = model.add_int_var(target=4)
+    /// >>> model.add_base_case([var == 4], cost=2)
+    /// >>> model.eval_base_cost(model.target_state)
+    /// 2
+    #[pyo3(signature = (state))]
+    fn eval_base_cost(&self, state: &state::StatePy) -> Option<IntOrFloat> {
+        match self.0.cost_type {
+            CostType::Integer => self
+                .0
+                .eval_base_cost(state.inner_as_ref())
+                .map(IntOrFloat::Int),
+            CostType::Continuous => self
+                .0
+                .eval_base_cost::<OrderedContinuous, _>(state.inner_as_ref())
+                .map(|x| IntOrFloat::Float(x.to_continuous())),
+        }
+    }
+
     /// get_transitions(forced, backward)
     ///
     /// Returns the transitions of the model.
     ///
     /// Parameters
     /// ----------
     /// forced: bool, default: False
@@ -1913,15 +1979,17 @@
     ) -> PyResult<bool> {
         let transitions = transitions
             .iter()
             .map(|t| Transition::from(t.clone()))
             .collect::<Vec<_>>();
         if self.float_cost() {
             let cost: Continuous = cost.extract()?;
-            Ok(self.0.validate_forward(&transitions, cost, !quiet))
+            Ok(self
+                .0
+                .validate_forward(&transitions, OrderedContinuous::from(cost), !quiet))
         } else {
             let cost: Integer = cost.extract()?;
             Ok(self.0.validate_forward(&transitions, cost, !quiet))
         }
     }
 
     /// add_element_table(table, default, name)
@@ -5315,23 +5383,26 @@
     #[test]
     fn add_base_case_ok() {
         let mut model = ModelPy::default();
         let v = model.add_int_var(0, None);
         assert!(v.is_ok());
         let v = v.unwrap();
         let v_id = IntegerVariable::from(v).id();
-        let result = model.add_base_case(vec![ConditionPy::from(Condition::ComparisonI(
-            ComparisonOperator::Gt,
-            Box::new(IntegerExpression::Variable(v_id)),
-            Box::new(IntegerExpression::Variable(0)),
-        ))]);
+        let result = model.add_base_case(
+            vec![ConditionPy::from(Condition::ComparisonI(
+                ComparisonOperator::Gt,
+                Box::new(IntegerExpression::Variable(v_id)),
+                Box::new(IntegerExpression::Variable(0)),
+            ))],
+            None,
+        );
         assert!(result.is_ok());
         assert_eq!(
             model.0.base_cases,
-            vec![BaseCase::new(vec![GroundedCondition {
+            vec![BaseCase::from(vec![GroundedCondition {
                 condition: Condition::ComparisonI(
                     ComparisonOperator::Gt,
                     Box::new(IntegerExpression::Variable(v_id)),
                     Box::new(IntegerExpression::Variable(0))
                 ),
                 ..Default::default()
             }])],
@@ -5343,19 +5414,22 @@
         let mut model = ModelPy::default();
         let v = model.add_int_var(0, None);
         assert!(v.is_ok());
         let v = v.unwrap();
         let v_id = IntegerVariable::from(v).id();
         let mut model = ModelPy::default();
         let snapshot = model.clone();
-        let result = model.add_base_case(vec![ConditionPy::from(Condition::ComparisonI(
-            ComparisonOperator::Gt,
-            Box::new(IntegerExpression::Variable(v_id)),
-            Box::new(IntegerExpression::Variable(0)),
-        ))]);
+        let result = model.add_base_case(
+            vec![ConditionPy::from(Condition::ComparisonI(
+                ComparisonOperator::Gt,
+                Box::new(IntegerExpression::Variable(v_id)),
+                Box::new(IntegerExpression::Variable(0)),
+            ))],
+            None,
+        );
         assert!(result.is_err());
         assert_eq!(model, snapshot);
     }
 
     #[test]
     fn set_minimize() {
         let mut model = ModelPy(Model {
```

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_acps.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_acps.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_apps.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_apps.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_bradth_first_search.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_bradth_first_search.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_caasdy.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_caasdy.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_cabs.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_cabs.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_cbfs.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_cbfs.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_dbdfs.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_dbdfs.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_dfbb.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_dfbb.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_dijkstra.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_forward_recursion.py`

 * *Files 16% similar despite different names*

```diff
@@ -16,27 +16,27 @@
     t = dp.Transition(
         name="decrement", cost=dp.IntExpr.state_cost() + 1, effects=[(var, var - 1)]
     )
     model.add_transition(t)
     model.add_dual_bound(0)
 
     with pytest.raises(error):
-        dp.Dijkstra(model, **kwargs)
+        dp.ForwardRecursion(model, **kwargs)
 
 
 def test_search():
     model = dp.Model()
     var = model.add_int_var(target=1)
     model.add_base_case([var == 0])
     t = dp.Transition(
         name="decrement", cost=dp.IntExpr.state_cost() + 1, effects=[(var, var - 1)]
     )
     model.add_transition(t)
     model.add_dual_bound(0)
-    solver = dp.Dijkstra(model)
+    solver = dp.ForwardRecursion(model)
     solution = solver.search()
 
     assert solution.cost == 1
     assert model.validate_forward(solution.transitions, solution.cost, quiet=True)
 
 
 def test_search_panic():
@@ -48,11 +48,11 @@
     t = dp.Transition(
         name="decrement",
         cost=dp.IntExpr.state_cost() + table[var + 1],
         effects=[(var, var - 1)],
     )
     model.add_transition(t)
     model.add_dual_bound(0)
-    solver = dp.Dijkstra(model)
+    solver = dp.ForwardRecursion(model)
 
     with pytest.raises(BaseException):
         solver.search()
```

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_expression_beam_search.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_expression_beam_search.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/heuristic_search_solver/test_forward_recursion.py` & `didppy-0.4.0/tests/heuristic_search_solver/test_weighted_astar.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import didppy as dp
 import pytest
 
 
 error_cases = [
-    ({"primal_bound": 1.5}, TypeError),
-    ({"initial_registry_capacity": -1}, OverflowError),
+    ({"weight": 1.5, "primal_bound": 1.5}, TypeError),
+    ({"weight": 1.5, "time_limit": -1}, BaseException),
+    ({"weight": 1.5, "initial_registry_capacity": -1}, OverflowError),
 ]
 
 
 @pytest.mark.parametrize("kwargs, error", error_cases)
 def test_error(kwargs, error):
     model = dp.Model()
     var = model.add_int_var(target=1)
@@ -16,27 +17,27 @@
     t = dp.Transition(
         name="decrement", cost=dp.IntExpr.state_cost() + 1, effects=[(var, var - 1)]
     )
     model.add_transition(t)
     model.add_dual_bound(0)
 
     with pytest.raises(error):
-        dp.ForwardRecursion(model, **kwargs)
+        dp.WeightedAstar(model, **kwargs)
 
 
 def test_search():
     model = dp.Model()
     var = model.add_int_var(target=1)
     model.add_base_case([var == 0])
     t = dp.Transition(
         name="decrement", cost=dp.IntExpr.state_cost() + 1, effects=[(var, var - 1)]
     )
     model.add_transition(t)
     model.add_dual_bound(0)
-    solver = dp.ForwardRecursion(model)
+    solver = dp.WeightedAstar(model, 1.5)
     solution = solver.search()
 
     assert solution.cost == 1
     assert model.validate_forward(solution.transitions, solution.cost, quiet=True)
 
 
 def test_search_panic():
@@ -48,11 +49,48 @@
     t = dp.Transition(
         name="decrement",
         cost=dp.IntExpr.state_cost() + table[var + 1],
         effects=[(var, var - 1)],
     )
     model.add_transition(t)
     model.add_dual_bound(0)
-    solver = dp.ForwardRecursion(model)
+    solver = dp.WeightedAstar(model, 1.5)
 
     with pytest.raises(BaseException):
         solver.search()
+
+
+def test_search_next():
+    model = dp.Model()
+    var = model.add_int_var(target=1)
+    model.add_base_case([var == 0])
+    t = dp.Transition(
+        name="decrement",
+        cost=dp.IntExpr.state_cost() + 1,
+        effects=[(var, var - 1)],
+    )
+    model.add_transition(t)
+    model.add_dual_bound(0)
+    solver = dp.WeightedAstar(model, 1.5)
+    solution, _ = solver.search_next()
+
+    assert solution.cost == 1
+    assert model.validate_forward(solution.transitions, solution.cost, quiet=True)
+
+
+def test_search_next_panic():
+    model = dp.Model()
+    obj = model.add_object_type(number=4)
+    var = model.add_element_var(object_type=obj, target=3)
+    table = model.add_int_table([1, 2, 3])
+    model.add_base_case([var == 0])
+    t = dp.Transition(
+        name="decrement",
+        cost=dp.IntExpr.state_cost() + table[var + 1],
+        effects=[(var, var - 1)],
+    )
+    model.add_transition(t)
+    model.add_dual_bound(0)
+    solver = dp.WeightedAstar(model, 1.5)
+
+    with pytest.raises(BaseException):
+        solver.search_next()
```

### Comparing `didppy-0.3.4/tests/model/test_expression.py` & `didppy-0.4.0/tests/model/test_expression.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/model/test_state.py` & `didppy-0.4.0/tests/model/test_state.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/model/test_table.py` & `didppy-0.4.0/tests/model/test_table.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/model/test_transition.py` & `didppy-0.4.0/tests/model/test_transition.py`

 * *Files identical despite different names*

### Comparing `didppy-0.3.4/tests/test_model.py` & `didppy-0.4.0/tests/test_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-import didppy as dp
 import pytest
 
+import didppy as dp
+
 
 def test_default():
     model = dp.Model()
 
     assert not model.maximize
     assert not model.float_cost
     assert model.state_constrs == []
@@ -126,15 +127,15 @@
     var = model.get_element_var("var")
     obj = model.get_object_type_of(var)
 
     assert model.get_number_of_object(obj) == 4
     assert model.get_target(var) == 1
 
 
-element_var_error_cases = [(-1, OverflowError), (4, RuntimeError), (1.5, TypeError)]
+element_var_error_cases = [(-1, OverflowError), (1.5, TypeError)]
 
 
 @pytest.mark.parametrize("value, error", element_var_error_cases)
 def test_add_element_var_error(value, error):
     model = dp.Model()
     obj = model.add_object_type(number=4)
 
@@ -534,18 +535,16 @@
         self.model.set_target(var, target)
 
         assert self.model.get_target(var) == expected
 
     error_cases = [
         (element_var, -1, OverflowError),
         (element_var, 1.5, TypeError),
-        (element_var, 4, RuntimeError),
         (element_resource_var, -1, OverflowError),
         (element_resource_var, 1.5, TypeError),
-        (element_resource_var, 4, RuntimeError),
         (set_var, {}, TypeError),
         (set_var, {-1}, TypeError),
         (set_var, {1.5}, TypeError),
         (set_var, {4}, RuntimeError),
         (int_var, 1.5, TypeError),
         (int_resource_var, 1.5, TypeError),
         (float_var, (), TypeError),
@@ -708,34 +707,70 @@
     int_var = model.add_int_var(target=3)
     state = model.target_state
 
     model.add_base_case([set_var.contains(0), set_var.contains(1)])
 
     assert len(model.base_cases) == 1
     assert len(model.base_cases[0]) == 2
-    assert model.base_cases[0][1].eval(state, model)
-    assert model.base_cases[0][1].eval(state, model)
+    assert model.base_cases[0][0][0].eval(state, model)
+    assert model.base_cases[0][0][1].eval(state, model)
+    assert model.base_cases[0][1].eval(state, model) == 0
 
     model.add_base_case([(int_var < 3) | ~set_var.contains(1)])
 
     assert len(model.base_cases) == 2
-    assert model.base_cases[0][1].eval(state, model)
-    assert model.base_cases[0][1].eval(state, model)
-    assert not model.base_cases[1][0].eval(state, model)
+    assert model.base_cases[0][0][0].eval(state, model)
+    assert model.base_cases[0][0][1].eval(state, model)
+    assert model.base_cases[0][1].eval(state, model) == 0
+    assert not model.base_cases[1][0][0].eval(state, model)
+    assert model.base_cases[1][1].eval(state, model) == 0
+
+
+def test_add_base_case_with_cost():
+    model = dp.Model()
+    obj = model.add_object_type(number=4)
+    set_var = model.add_set_var(object_type=obj, target=[0, 1])
+    int_var = model.add_int_var(target=3)
+    state = model.target_state
+
+    model.add_base_case([set_var.contains(0), set_var.contains(1)], cost=int_var + 1)
+
+    assert len(model.base_cases) == 1
+    assert len(model.base_cases[0]) == 2
+    assert model.base_cases[0][0][0].eval(state, model)
+    assert model.base_cases[0][0][1].eval(state, model)
+    assert model.base_cases[0][1].eval(state, model) == 4
+
+    model.add_base_case([(int_var < 3) | ~set_var.contains(1)], cost=2)
+
+    assert len(model.base_cases) == 2
+    assert model.base_cases[0][0][0].eval(state, model)
+    assert model.base_cases[0][0][1].eval(state, model)
+    assert model.base_cases[0][1].eval(state, model) == 4
+    assert not model.base_cases[1][0][0].eval(state, model)
+    assert model.base_cases[1][1].eval(state, model) == 2
 
 
 def test_add_base_case_error():
     model = dp.Model()
 
     with pytest.raises(RuntimeError):
         model.add_base_case([dp.IntExpr.state_cost() > 0])
 
 
 def test_add_base_case_panic():
     model = dp.Model()
+    int_var = model.add_int_var(target=3)
+
+    with pytest.raises(BaseException):
+        model.add_base_case([int_var > 0], cost=dp.IntExpr.state_cost())
+
+
+def test_add_base_case_panic_cost():
+    model = dp.Model()
     table = model.add_int_table([1, 2, 3])
 
     with pytest.raises(BaseException):
         model.add_base_case([table[4] > 0])
 
 
 def test_add_base_case_var_not_included_error():
@@ -793,14 +828,59 @@
     table = model.add_int_table([0, 1, 2, 3])
     model.add_base_case([table[var + 1] > 0])
 
     with pytest.raises(BaseException):
         model.is_base(model.target_state)
 
 
+def test_eval_base_cost_zero():
+    model = dp.Model()
+    obj = model.add_object_type(number=4)
+    set_var = model.add_set_var(object_type=obj, target=[0, 1])
+    int_var = model.add_int_var(target=3)
+    model.add_base_case([set_var.contains(0), set_var.contains(1)])
+    model.add_base_case([int_var < 2, int_var > 0])
+    state = model.target_state
+
+    assert model.eval_base_cost(state) == 0
+
+
+def test_eval_base_cost_some():
+    model = dp.Model()
+    model.maximize = False
+    obj = model.add_object_type(number=4)
+    set_var = model.add_set_var(object_type=obj, target=[0, 1])
+    int_var = model.add_int_var(target=3)
+    model.add_base_case([set_var.contains(0), set_var.contains(1)], cost=int_var)
+    model.add_base_case([int_var <= 3, int_var >= 2], cost=4)
+    model.add_base_case([int_var < 2, int_var > 0], cost=2)
+    state = model.target_state
+
+    assert model.eval_base_cost(state) == 3
+
+
+def test_eval_base_case_none():
+    model = dp.Model()
+    obj = model.add_object_type(number=4)
+    set_var = model.add_set_var(object_type=obj, target=[0, 1])
+    int_var = model.add_int_var(target=3)
+    model.add_base_case(
+        [
+            set_var.contains(0),
+            set_var.contains(1),
+            set_var.contains(2),
+        ],
+        cost=2,
+    )
+    model.add_base_case([int_var < 2, int_var > 0])
+    state = model.target_state
+
+    assert model.eval_base_cost(state) is None
+
+
 def test_add_transition():
     model = dp.Model()
 
     assert model.get_transitions() == []
     assert model.get_transitions(forced=False) == []
     assert model.get_transitions(forced=True) == []
```

### Comparing `didppy-0.3.4/Cargo.lock` & `didppy-0.4.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "didp-yaml"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "approx",
  "dypdl",
  "dypdl-heuristic-search",
  "lazy_static",
  "linked-hash-map",
  "num-traits",
@@ -50,37 +50,37 @@
  "serde_yaml",
  "tikv-jemallocator",
  "yaml-rust",
 ]
 
 [[package]]
 name = "didppy"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "dypdl",
  "dypdl-heuristic-search",
  "pyo3",
  "pyo3-build-config",
  "rustc-hash",
 ]
 
 [[package]]
 name = "dypdl"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "approx",
  "fixedbitset",
  "num-traits",
  "ordered-float",
  "rustc-hash",
 ]
 
 [[package]]
 name = "dypdl-heuristic-search"
-version = "0.3.4"
+version = "0.4.0"
 dependencies = [
  "dypdl",
  "ordered-float",
  "rustc-hash",
 ]
 
 [[package]]
```

### Comparing `didppy-0.3.4/PKG-INFO` & `didppy-0.4.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 Metadata-Version: 2.1
 Name: didppy
-Version: 0.3.4
+Version: 0.4.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Python interface for Dynamic Programming Description Language (DyPDL) and DyPDL solvers.
+Home-Page: https://didp.ai
+Author: Ryo Kuroiwa <ryo.kuroiwa@mail.utoronto.ca>
+Author-email: Ryo Kuroiwa <ryo.kuroiwa@mail.utoronto.ca>
 License: MIT OR Apache-2.0
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
+Project-URL: Source Code, https://github.com/domain-independent-dp/didp-rs
 
 [![PyPi version](https://img.shields.io/pypi/v/didppy.svg)](https://pypi.python.org/pypi/didppy/)
 [![](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/)
 [![crates.io](https://img.shields.io/crates/v/didppy)](https://crates.io/crates/didppy)
 [![minimum rustc 1.64](https://img.shields.io/badge/rustc-1.64+-blue.svg)](https://rust-lang.github.io/rfcs/2495-min-rust-version.html)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
 [![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
```

