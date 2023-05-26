# Comparing `tmp/liionpack-0.3.5.tar.gz` & `tmp/liionpack-0.3.6.tar.gz`

## Comparing `liionpack-0.3.5.tar` & `liionpack-0.3.6.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 liionpack-0.3.5/.git-blame-ignore-revs
--rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 liionpack-0.3.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 liionpack-0.3.5/.readthedocs.yaml
--rw-r--r--   0        0        0     5307 2020-02-02 00:00:00.000000 liionpack-0.3.5/CHANGELOG.md
--rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 liionpack-0.3.5/asv.conf.json
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 liionpack-0.3.5/environment.yml
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.5/mkdocs.yml
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 liionpack-0.3.5/.github/codecov.yml
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 liionpack-0.3.5/.github/ISSUE_TEMPLATE/bug_report.yml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 liionpack-0.3.5/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 liionpack-0.3.5/.github/ISSUE_TEMPLATE/feature_request.yml
--rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 liionpack-0.3.5/.github/workflows/periodic_benchmarks.yml
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 liionpack-0.3.5/.github/workflows/publish_pypi.yml
--rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 liionpack-0.3.5/.github/workflows/run_benchmarks_over_history.yml
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 liionpack-0.3.5/.github/workflows/test_on_push.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.5/benchmarks/__init__.py
--rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 liionpack-0.3.5/benchmarks/benchmarks.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/about.md
--rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/conduct.md
--rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/contributing.md
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/index.md
--rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/install.md
--rw-r--r--   0        0        0   203695 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/liionpack.png
--rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/mathjax-config.js
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/reference.md
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/requirements.txt
--rw-r--r--   0        0        0   428208 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/01 Getting Started.ipynb
--rw-r--r--   0        0        0   258064 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/02 Using inputs.ipynb
--rw-r--r--   0        0        0   115177 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/03 Experiments.ipynb
--rw-r--r--   0        0        0   320758 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/04 Initial SoC.ipynb
--rw-r--r--   0        0        0   939974 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/05 Drive cycles.ipynb
--rw-r--r--   0        0        0   894028 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/06 Changing a model.ipynb
--rw-r--r--   0        0        0   131502 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/07 Visualizing larger packs.ipynb
--rw-r--r--   0        0        0  1291981 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/08 SEI degradation model.ipynb
--rw-r--r--   0        0        0   322325 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/examples/09 Terminal locations.ipynb
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 liionpack-0.3.5/docs/stylesheets/extra.css
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/basic_16p2s.py
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/big_circuit.py
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/different_initial_soc.py
--rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/draw_circuit.py
--rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/draw_terminals.py
--rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/drive_cycle.py
--rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/drive_cycle_comparison.py
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/load_4p1s.py
--rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/mixed_terminals.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/paper_example.py
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/save_output.py
--rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/step_external_variable.py
--rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 liionpack-0.3.5/examples/thermal_external.py
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/__init__.py
--rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/definitions.py
--rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/logger.py
--rw-r--r--   0        0        0    25031 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/netlist_utils.py
--rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/plots.py
--rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/protocols.py
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/sim_utils.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/simulations.py
--rw-r--r--   0        0        0    15962 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/solver_utils.py
--rw-r--r--   0        0        0    18667 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/solvers.py
--rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/utils.py
--rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/circuits/4p1s.asc
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/circuits/4p1s.cir
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 liionpack-0.3.5/liionpack/circuits/4p1s.txt
--rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 liionpack-0.3.5/paper/paper.bib
--rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 liionpack-0.3.5/paper/paper.md
--rw-r--r--   0        0        0   100911 2020-02-02 00:00:00.000000 liionpack-0.3.5/paper/paper_figures/Figure_0.png
--rw-r--r--   0        0        0   113147 2020-02-02 00:00:00.000000 liionpack-0.3.5/paper/paper_figures/Figure_1.png
--rw-r--r--   0        0        0    40455 2020-02-02 00:00:00.000000 liionpack-0.3.5/paper/paper_figures/Figure_2.png
--rw-r--r--   0        0        0    33408 2020-02-02 00:00:00.000000 liionpack-0.3.5/paper/paper_figures/Figure_3.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/integration/__init__.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/integration/test_1p1s.py
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/integration/test_all_solvers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/__init__.py
--rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_logger.py
--rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_netlist_utils.py
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_notebooks.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_plots.py
--rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_protocols.py
--rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_sim_utils.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_simulations.py
--rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_solver_utils.py
--rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_solvers.py
--rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 liionpack-0.3.5/tests/unit/test_utils.py
--rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 liionpack-0.3.5/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 liionpack-0.3.5/LICENSE
--rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 liionpack-0.3.5/README.md
--rw-r--r--   0        0        0     1359 2020-02-02 00:00:00.000000 liionpack-0.3.5/pyproject.toml
--rw-r--r--   0        0        0     5933 2020-02-02 00:00:00.000000 liionpack-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 liionpack-0.3.6/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 liionpack-0.3.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 liionpack-0.3.6/.readthedocs.yaml
+-rw-r--r--   0        0        0     5597 2020-02-02 00:00:00.000000 liionpack-0.3.6/CHANGELOG.md
+-rw-r--r--   0        0        0     6883 2020-02-02 00:00:00.000000 liionpack-0.3.6/asv.conf.json
+-rw-r--r--   0        0        0      786 2020-02-02 00:00:00.000000 liionpack-0.3.6/environment.yml
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.6/mkdocs.yml
+-rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/codecov.yml
+-rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/ISSUE_TEMPLATE/bug_report.yml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      902 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/ISSUE_TEMPLATE/feature_request.yml
+-rw-r--r--   0        0        0     2286 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/workflows/periodic_benchmarks.yml
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/workflows/publish_pypi.yml
+-rw-r--r--   0        0        0     2986 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/workflows/run_benchmarks_over_history.yml
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 liionpack-0.3.6/.github/workflows/test_on_push.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.6/benchmarks/__init__.py
+-rw-r--r--   0        0        0     3552 2020-02-02 00:00:00.000000 liionpack-0.3.6/benchmarks/benchmarks.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/about.md
+-rw-r--r--   0        0        0     5218 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/conduct.md
+-rw-r--r--   0        0        0    18625 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/contributing.md
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/index.md
+-rw-r--r--   0        0        0     2244 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/install.md
+-rw-r--r--   0        0        0   203695 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/liionpack.png
+-rw-r--r--   0        0        0      730 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/mathjax-config.js
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/reference.md
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/requirements.txt
+-rw-r--r--   0        0        0   428208 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/01 Getting Started.ipynb
+-rw-r--r--   0        0        0   258064 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/02 Using inputs.ipynb
+-rw-r--r--   0        0        0   115177 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/03 Experiments.ipynb
+-rw-r--r--   0        0        0   320758 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/04 Initial SoC.ipynb
+-rw-r--r--   0        0        0   939974 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/05 Drive cycles.ipynb
+-rw-r--r--   0        0        0   894028 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/06 Changing a model.ipynb
+-rw-r--r--   0        0        0   131502 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/07 Visualizing larger packs.ipynb
+-rw-r--r--   0        0        0  1291981 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/08 SEI degradation model.ipynb
+-rw-r--r--   0        0        0   322325 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/examples/09 Terminal locations.ipynb
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 liionpack-0.3.6/docs/stylesheets/extra.css
+-rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/basic_16p2s.py
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/big_circuit.py
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/different_initial_soc.py
+-rw-r--r--   0        0        0      979 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/draw_circuit.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/draw_terminals.py
+-rw-r--r--   0        0        0      962 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/drive_cycle.py
+-rw-r--r--   0        0        0     4039 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/drive_cycle_comparison.py
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/load_4p1s.py
+-rw-r--r--   0        0        0     1044 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/mixed_terminals.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/paper_example.py
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/save_output.py
+-rw-r--r--   0        0        0     2218 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/step_external_variable.py
+-rw-r--r--   0        0        0      980 2020-02-02 00:00:00.000000 liionpack-0.3.6/examples/thermal_external.py
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/__init__.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/definitions.py
+-rw-r--r--   0        0        0     2198 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/logger.py
+-rw-r--r--   0        0        0    25031 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/netlist_utils.py
+-rw-r--r--   0        0        0    11346 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/plots.py
+-rw-r--r--   0        0        0     1496 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/protocols.py
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/sim_utils.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/simulations.py
+-rw-r--r--   0        0        0    16012 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/solver_utils.py
+-rw-r--r--   0        0        0    18667 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/solvers.py
+-rw-r--r--   0        0        0     5343 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/utils.py
+-rw-r--r--   0        0        0     2749 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/circuits/4p1s.asc
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/circuits/4p1s.cir
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 liionpack-0.3.6/liionpack/circuits/4p1s.txt
+-rw-r--r--   0        0        0     3521 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper.bib
+-rw-r--r--   0        0        0    11210 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper.md
+-rw-r--r--   0        0        0   100911 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper_figures/Figure_0.png
+-rw-r--r--   0        0        0   113147 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper_figures/Figure_1.png
+-rw-r--r--   0        0        0    40455 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper_figures/Figure_2.png
+-rw-r--r--   0        0        0    33408 2020-02-02 00:00:00.000000 liionpack-0.3.6/paper/paper_figures/Figure_3.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/integration/__init__.py
+-rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/integration/test_1p1s.py
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/integration/test_all_solvers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/__init__.py
+-rw-r--r--   0        0        0     1313 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_logger.py
+-rw-r--r--   0        0        0     4963 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_netlist_utils.py
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_notebooks.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_plots.py
+-rw-r--r--   0        0        0     2856 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_protocols.py
+-rw-r--r--   0        0        0     1424 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_sim_utils.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_simulations.py
+-rw-r--r--   0        0        0     3570 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_solver_utils.py
+-rw-r--r--   0        0        0     4817 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_solvers.py
+-rw-r--r--   0        0        0     2702 2020-02-02 00:00:00.000000 liionpack-0.3.6/tests/unit/test_utils.py
+-rw-r--r--   0        0        0     1300 2020-02-02 00:00:00.000000 liionpack-0.3.6/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 liionpack-0.3.6/LICENSE
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 liionpack-0.3.6/README.md
+-rw-r--r--   0        0        0     1376 2020-02-02 00:00:00.000000 liionpack-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0     5958 2020-02-02 00:00:00.000000 liionpack-0.3.6/PKG-INFO
```

### Comparing `liionpack-0.3.5/CHANGELOG.md` & `liionpack-0.3.6/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 
 - ([#PR](link))
 
 ## Breaking changes
 
 - ([#PR](link))
 
+# [v0.3.6](https://github.com/pybamm-team/liionpack/)
+
+
+## Bug fixes
+
+- Fix a RunTimeError introduced by change to latest version of casadi that PyBaMM now supports. Solution returned by casadi no longer contains initial state. ([#259](https://github.com/pybamm-team/liionpack/pull/259))
+
+
 # [v0.3.5](https://github.com/pybamm-team/liionpack/) - 2023-04-05
 
 ## Features
 
 - Add pre commit and migrate to ruff ([#232](https://github.com/pybamm-team/liionpack/pull/232))
 
 ## Bug fixes
```

### Comparing `liionpack-0.3.5/asv.conf.json` & `liionpack-0.3.6/asv.conf.json`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/environment.yml` & `liionpack-0.3.6/environment.yml`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,9 @@
   - pip:
     - pybamm>=23.3
     - ipdb
     - ruff
     - mkdocstrings-python-legacy
     - mkdocs-material
     - mkdocs-jupyter
+    - nbconvert
     - -e .
```

### Comparing `liionpack-0.3.5/mkdocs.yml` & `liionpack-0.3.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/.github/ISSUE_TEMPLATE/bug_report.yml` & `liionpack-0.3.6/.github/ISSUE_TEMPLATE/bug_report.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/.github/ISSUE_TEMPLATE/feature_request.yml` & `liionpack-0.3.6/.github/ISSUE_TEMPLATE/feature_request.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/.github/workflows/periodic_benchmarks.yml` & `liionpack-0.3.6/.github/workflows/periodic_benchmarks.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/.github/workflows/publish_pypi.yml` & `liionpack-0.3.6/.github/workflows/publish_pypi.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/.github/workflows/run_benchmarks_over_history.yml` & `liionpack-0.3.6/.github/workflows/run_benchmarks_over_history.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/.github/workflows/test_on_push.yml` & `liionpack-0.3.6/.github/workflows/test_on_push.yml`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/benchmarks/benchmarks.py` & `liionpack-0.3.6/benchmarks/benchmarks.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/conduct.md` & `liionpack-0.3.6/docs/conduct.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/contributing.md` & `liionpack-0.3.6/docs/contributing.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/index.md` & `liionpack-0.3.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/install.md` & `liionpack-0.3.6/docs/install.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/liionpack.png` & `liionpack-0.3.6/docs/liionpack.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/mathjax-config.js` & `liionpack-0.3.6/docs/mathjax-config.js`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/01 Getting Started.ipynb` & `liionpack-0.3.6/docs/examples/01 Getting Started.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/02 Using inputs.ipynb` & `liionpack-0.3.6/docs/examples/02 Using inputs.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/03 Experiments.ipynb` & `liionpack-0.3.6/docs/examples/03 Experiments.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/04 Initial SoC.ipynb` & `liionpack-0.3.6/docs/examples/04 Initial SoC.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/05 Drive cycles.ipynb` & `liionpack-0.3.6/docs/examples/05 Drive cycles.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/06 Changing a model.ipynb` & `liionpack-0.3.6/docs/examples/06 Changing a model.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/07 Visualizing larger packs.ipynb` & `liionpack-0.3.6/docs/examples/07 Visualizing larger packs.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/08 SEI degradation model.ipynb` & `liionpack-0.3.6/docs/examples/08 SEI degradation model.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/docs/examples/09 Terminal locations.ipynb` & `liionpack-0.3.6/docs/examples/09 Terminal locations.ipynb`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/basic_16p2s.py` & `liionpack-0.3.6/examples/basic_16p2s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/big_circuit.py` & `liionpack-0.3.6/examples/big_circuit.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/different_initial_soc.py` & `liionpack-0.3.6/examples/different_initial_soc.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/draw_circuit.py` & `liionpack-0.3.6/examples/draw_circuit.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/draw_terminals.py` & `liionpack-0.3.6/examples/draw_terminals.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/drive_cycle.py` & `liionpack-0.3.6/examples/drive_cycle.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/drive_cycle_comparison.py` & `liionpack-0.3.6/examples/drive_cycle_comparison.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/load_4p1s.py` & `liionpack-0.3.6/examples/load_4p1s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/mixed_terminals.py` & `liionpack-0.3.6/examples/mixed_terminals.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/paper_example.py` & `liionpack-0.3.6/examples/paper_example.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/save_output.py` & `liionpack-0.3.6/examples/save_output.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/step_external_variable.py` & `liionpack-0.3.6/examples/step_external_variable.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/examples/thermal_external.py` & `liionpack-0.3.6/examples/thermal_external.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/__init__.py` & `liionpack-0.3.6/liionpack/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,8 +40,8 @@
 from .definitions import MODULE_DIR
 from .definitions import CIRCUIT_DIR
 from .solvers import CasadiManager
 from .solvers import RayManager
 from .solvers import GenericActor
 from .solvers import RayActor
 
-__version__ = "0.3.5"
+__version__ = "0.3.6"
```

### Comparing `liionpack-0.3.5/liionpack/logger.py` & `liionpack-0.3.6/liionpack/logger.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/netlist_utils.py` & `liionpack-0.3.6/liionpack/netlist_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/plots.py` & `liionpack-0.3.6/liionpack/plots.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/protocols.py` & `liionpack-0.3.6/liionpack/protocols.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/sim_utils.py` & `liionpack-0.3.6/liionpack/sim_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/simulations.py` & `liionpack-0.3.6/liionpack/simulations.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/solver_utils.py` & `liionpack-0.3.6/liionpack/solver_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             x0 = solutions[k].y[:len_rhs, -1]
             z0 = solutions[k].y[len_rhs:, -1]
         temp = inputs_dict[k]
         inputs = casadi.vertcat(*[x for x in temp.values()] + [t_min])
         ninputs = len(temp.values())
         # Call the integrator once, with the grid
         casadi_sol = integrator(x0=x0, z0=z0, p=inputs)
-        xf = casadi_sol["xf"]
+        xf = casadi.horzcat(x0, casadi_sol["xf"])
         zf = casadi_sol["zf"]
         if zf.is_empty():
             y_sol = xf
         else:
             y_sol = casadi.vertcat(xf, zf)
         xend = y_sol[:, -1]
         sol.append(pybamm.Solution(t_eval, y_sol, model, inputs_dict[k]))
@@ -211,23 +211,23 @@
     # p = casadi.horzcat(*zip(inputs, external_variables, [t_min]*N))
     # inputs_with_tmin = casadi.vertcat(inputs, np.asarray(t_min))
     # Call the integrator once, with the grid
     timer = pybamm.Timer()
     tic = timer.time()
     casadi_sol = integrator(x0=x0, z0=z0, p=inputs)
     integration_time = timer.time()
-    nt = len(t_eval)
+    nt = len(t_eval[1:])
     xf = casadi_sol["xf"]
     zf = casadi_sol["zf"]
     sol = []
     xend = []
     events_eval = []
     for i in range(N):
         start = i * nt
-        y_diff = xf[:, start : start + nt]
+        y_diff = casadi.horzcat(x0[:, i], xf[:, start : start + nt])
         if zf.is_empty():
             y_sol = y_diff
         else:
             y_alg = zf[:, start : start + nt]
             y_sol = casadi.vertcat(y_diff, y_alg)
         xend.append(y_sol[:, -1])
         # Not sure how to index into zf - need an example
```

### Comparing `liionpack-0.3.5/liionpack/solvers.py` & `liionpack-0.3.6/liionpack/solvers.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/utils.py` & `liionpack-0.3.6/liionpack/utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/circuits/4p1s.asc` & `liionpack-0.3.6/liionpack/circuits/4p1s.asc`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/liionpack/circuits/4p1s.cir` & `liionpack-0.3.6/liionpack/circuits/4p1s.cir`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/paper/paper.bib` & `liionpack-0.3.6/paper/paper.bib`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/paper/paper.md` & `liionpack-0.3.6/paper/paper.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/paper/paper_figures/Figure_0.png` & `liionpack-0.3.6/paper/paper_figures/Figure_0.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/paper/paper_figures/Figure_1.png` & `liionpack-0.3.6/paper/paper_figures/Figure_1.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/paper/paper_figures/Figure_2.png` & `liionpack-0.3.6/paper/paper_figures/Figure_2.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/paper/paper_figures/Figure_3.png` & `liionpack-0.3.6/paper/paper_figures/Figure_3.png`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/integration/test_1p1s.py` & `liionpack-0.3.6/tests/integration/test_1p1s.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/integration/test_all_solvers.py` & `liionpack-0.3.6/tests/integration/test_all_solvers.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_logger.py` & `liionpack-0.3.6/tests/unit/test_logger.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_netlist_utils.py` & `liionpack-0.3.6/tests/unit/test_netlist_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_notebooks.py` & `liionpack-0.3.6/tests/unit/test_notebooks.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_plots.py` & `liionpack-0.3.6/tests/unit/test_plots.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_protocols.py` & `liionpack-0.3.6/tests/unit/test_protocols.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_sim_utils.py` & `liionpack-0.3.6/tests/unit/test_sim_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_simulations.py` & `liionpack-0.3.6/tests/unit/test_simulations.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_solver_utils.py` & `liionpack-0.3.6/tests/unit/test_solver_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_solvers.py` & `liionpack-0.3.6/tests/unit/test_solvers.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/tests/unit/test_utils.py` & `liionpack-0.3.6/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/.gitignore` & `liionpack-0.3.6/.gitignore`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/LICENSE` & `liionpack-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/README.md` & `liionpack-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `liionpack-0.3.5/pyproject.toml` & `liionpack-0.3.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -37,14 +37,15 @@
     "pybamm>=23.3",
     "ray",
     "redis",
     "scikit-spatial",
     "scipy",
     "textwrapper",
     "tqdm",
+    "nbconvert",
 ]
 dynamic = [
     "version",
 ]
 
 [project.urls]
 "Bug Tracker" = "https://github.com/pybamm-team/liionpack/issues"
```

### Comparing `liionpack-0.3.5/PKG-INFO` & `liionpack-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: liionpack
-Version: 0.3.5
+Version: 0.3.6
 Summary: A battery pack simulator for PyBaMM
 Project-URL: Bug Tracker, https://github.com/pybamm-team/liionpack/issues
 Project-URL: Changelog, https://github.com/pybamm-team/liionpack/blob/develop/CHANGELOG.md
 Project-URL: Documentation, https://liionpack.readthedocs.io/en/latest/
 Project-URL: Homepage, https://github.com/pybamm-team/liionpack
 Author-email: Tom Tranter <t.g.tranter@gmail.com>
 License-Expression: MIT
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
 Requires-Dist: ipython
 Requires-Dist: lcapy
 Requires-Dist: matplotlib
+Requires-Dist: nbconvert
 Requires-Dist: networkx
 Requires-Dist: numpy
 Requires-Dist: openpyxl
 Requires-Dist: pandas
 Requires-Dist: plotly
 Requires-Dist: pybamm>=23.3
 Requires-Dist: ray
```

