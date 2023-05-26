# Comparing `tmp/hiperwalk-2.0a0.tar.gz` & `tmp/hiperwalk-2.0a1.tar.gz`

## Comparing `hiperwalk-2.0a0.tar` & `hiperwalk-2.0a1.tar`

### file list

```diff
@@ -1,100 +1,95 @@
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/.readthedocs.yaml
--rwxr-xr-x   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/build_and_upload_to_pypi
--rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/config.py
--rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/custom.nbl
--rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/custom.py
--rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/distance.py
--rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/dtqw1d.nbl
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/dtqw1d.py
--rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/dtqw2d.nbl
--rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/dtqw2d.py
--rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/gnuplot.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/hiperwalk.py
--rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/install.sh
--rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/ioFunctions.py
--rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/neblina.py
--rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/operators.py
--rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/parsing.py
--rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/run.py
--rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/staggered1d.nbl
--rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/staggered1d.py
--rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/staggered2d.nbl
--rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/staggered2d.py
--rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/standardDeviation.py
--rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/state.py
--rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/testmode.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/walks.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/examples/coined1D.in
--rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/examples/coined2D.in
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/examples/custom.in
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/examples/psi0.dat
--rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/examples/staggered1D.in
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/examples/staggered2D.in
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/examples/u0.dat
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/Archive/examples/u1.dat
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/Makefile
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/README.md
--rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/conf.py
--rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/go
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/index.rst
--rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/make.bat
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/requirements.txt
--rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/test_docs
--rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/_static/switcher.json
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/_templates/autoclass.rst
--rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/_templates/autofunctions.rst
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/_templates/automodule.rst
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/_templates/autosummary/class.rst
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/development/index.rst
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/documentation/graph.rst
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/documentation/index.rst
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/documentation/plot.rst
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/documentation/quantum_walk.rst
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/graphviz/coined-cycle-edges-labels.dot
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/graphviz/coined-model-edges-labels.dot
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/graphviz/coined-model-sample.dot
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/graphviz/coined-segment-edges-labels.dot
--rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/install/index.rst
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/docs/tutorial/index.rst
--rw-r--r--   0        0        0      557 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/animated-quantum-week-coined.py
--rw-r--r--   0        0        0      380 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/coined-cycle.py
--rw-r--r--   0        0        0      955 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/coined-graph.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/coined-line.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/coined-segment.py
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/continuous-cycle.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/continuous-graph.py
--rw-r--r--   0        0        0      497 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/non-hpc-coined-line.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/quantum-week-coined.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/quantum-week-continuous.py
--rw-r--r--   0        0        0      334 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/examples/refactor.py
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/__init__.py
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/_constants.py
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/graph/__init__.py
--rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/graph/cycle.py
--rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/graph/graph.py
--rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/graph/lattice.py
--rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/graph/line.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/plot/__init__.py
--rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/plot/_animation.py
--rw-r--r--   0        0        0    26324 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/plot/_plot.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/quantum_walk/__init__.py
--rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/quantum_walk/_pyneblina_interface.py
--rw-r--r--   0        0        0    33983 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/quantum_walk/coined_walk.py
--rw-r--r--   0        0        0    10615 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/quantum_walk/continuous_walk.py
--rw-r--r--   0        0        0    16413 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/hiperwalk/quantum_walk/quantum_walk.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/__init__.py
--rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/run_all.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/run_hpc.sh
--rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/run_nonhpc.sh
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/test_constants.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/unitary/__init__.py
--rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/unitary/coined_cycle.py
--rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/unitary/coined_line.py
--rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/unitary/coined_segment.py
--rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/unitary/continuous_graph.py
--rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/tests/unitary/lattice_uniform_state.py
--rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/.gitignore
--rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/LICENSE
--rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/README.md
--rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/pyproject.toml
--rw-r--r--   0        0        0    11966 2020-02-02 00:00:00.000000 hiperwalk-2.0a0/PKG-INFO
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/.readthedocs.yaml
+-rwxr-xr-x   0        0        0       62 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/build_and_upload_to_pypi
+-rw-r--r--   0        0        0     3980 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/config.py
+-rw-r--r--   0        0        0     4261 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/custom.nbl
+-rw-r--r--   0        0        0      570 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/custom.py
+-rwxr-xr-x   0        0        0     1734 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/distance.py
+-rw-r--r--   0        0        0     3052 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/dtqw1d.nbl
+-rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/dtqw1d.py
+-rw-r--r--   0        0        0     3190 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/dtqw2d.nbl
+-rw-r--r--   0        0        0     2275 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/dtqw2d.py
+-rw-r--r--   0        0        0    12690 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/gnuplot.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/hiperwalk.py
+-rwxr-xr-x   0        0        0      909 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/install.sh
+-rw-r--r--   0        0        0     3662 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/ioFunctions.py
+-rw-r--r--   0        0        0    22919 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/neblina.py
+-rw-r--r--   0        0        0    29012 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/operators.py
+-rw-r--r--   0        0        0    17101 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/parsing.py
+-rw-r--r--   0        0        0      551 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/run.py
+-rw-r--r--   0        0        0     2787 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/staggered1d.nbl
+-rw-r--r--   0        0        0     2333 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/staggered1d.py
+-rw-r--r--   0        0        0     3043 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/staggered2d.nbl
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/staggered2d.py
+-rw-r--r--   0        0        0     4244 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/standardDeviation.py
+-rw-r--r--   0        0        0    12276 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/state.py
+-rw-r--r--   0        0        0    24726 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/testmode.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/walks.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/coined1D.in
+-rw-r--r--   0        0        0      403 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/coined2D.in
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/custom.in
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/psi0.dat
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/staggered1D.in
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/staggered2D.in
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/u0.dat
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/Archive/examples/u1.dat
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/Makefile
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/README.md
+-rw-r--r--   0        0        0     3064 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/conf.py
+-rwxr-xr-x   0        0        0       53 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/go
+-rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/index.rst
+-rw-r--r--   0        0        0      804 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/make.bat
+-rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/requirements.txt
+-rwxr-xr-x   0        0        0       13 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/test_docs
+-rw-r--r--   0        0        0      269 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_static/switcher.json
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_templates/autoclass.rst
+-rw-r--r--   0        0        0      347 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_templates/autofunctions.rst
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_templates/automodule.rst
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/_templates/autosummary/class.rst
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/development/index.rst
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/documentation/graph.rst
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/documentation/index.rst
+-rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/documentation/plot.rst
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/documentation/quantum_walk.rst
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/graphviz/coined-cycle-edges-labels.dot
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/graphviz/coined-model-edges-labels.dot
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/graphviz/coined-model-sample.dot
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/graphviz/coined-segment-edges-labels.dot
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/install/index.rst
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/docs/tutorial/index.rst
+-rw-r--r--   0        0        0      558 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/coined-diagonal-lattice.py
+-rw-r--r--   0        0        0      270 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/continuous-cycle.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/deleteme.py
+-rw-r--r--   0        0        0     1170 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/hypercube.py
+-rw-r--r--   0        0        0      367 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/refactor.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/examples/renato.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/__init__.py
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/_constants.py
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/__init__.py
+-rw-r--r--   0        0        0     5220 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/cycle.py
+-rw-r--r--   0        0        0     3595 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/graph.py
+-rw-r--r--   0        0        0    11813 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/lattice.py
+-rw-r--r--   0        0        0     3708 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/graph/line.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/plot/__init__.py
+-rw-r--r--   0        0        0    11851 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/plot/_animation.py
+-rw-r--r--   0        0        0    26324 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/plot/_plot.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/__init__.py
+-rw-r--r--   0        0        0    11524 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/_pyneblina_interface.py
+-rw-r--r--   0        0        0    33983 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/coined_walk.py
+-rw-r--r--   0        0        0    10615 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/continuous_walk.py
+-rw-r--r--   0        0        0    16420 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/hiperwalk/quantum_walk/quantum_walk.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/__init__.py
+-rwxr-xr-x   0        0        0      123 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/run_all.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/run_hpc.sh
+-rwxr-xr-x   0        0        0      124 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/run_nonhpc.sh
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/test_constants.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/__init__.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/coined_cycle.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/coined_line.py
+-rw-r--r--   0        0        0     2149 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/coined_segment.py
+-rw-r--r--   0        0        0     6758 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/continuous_graph.py
+-rw-r--r--   0        0        0      421 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/tests/unitary/lattice_uniform_state.py
+-rw-r--r--   0        0        0      836 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/.gitignore
+-rw-r--r--   0        0        0     7560 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/LICENSE
+-rw-r--r--   0        0        0     1914 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/README.md
+-rw-r--r--   0        0        0     1153 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/pyproject.toml
+-rw-r--r--   0        0        0    11956 2020-02-02 00:00:00.000000 hiperwalk-2.0a1/PKG-INFO
```

### Comparing `hiperwalk-2.0a0/Archive/config.py` & `hiperwalk-2.0a1/Archive/config.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/custom.nbl` & `hiperwalk-2.0a1/Archive/custom.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/custom.py` & `hiperwalk-2.0a1/Archive/custom.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/distance.py` & `hiperwalk-2.0a1/Archive/distance.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/dtqw1d.nbl` & `hiperwalk-2.0a1/Archive/dtqw1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/dtqw1d.py` & `hiperwalk-2.0a1/Archive/dtqw1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/dtqw2d.nbl` & `hiperwalk-2.0a1/Archive/dtqw2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/dtqw2d.py` & `hiperwalk-2.0a1/Archive/dtqw2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/gnuplot.py` & `hiperwalk-2.0a1/Archive/gnuplot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/hiperwalk.py` & `hiperwalk-2.0a1/Archive/hiperwalk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/install.sh` & `hiperwalk-2.0a1/Archive/install.sh`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/ioFunctions.py` & `hiperwalk-2.0a1/Archive/ioFunctions.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/neblina.py` & `hiperwalk-2.0a1/Archive/neblina.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/operators.py` & `hiperwalk-2.0a1/Archive/operators.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/parsing.py` & `hiperwalk-2.0a1/Archive/parsing.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/run.py` & `hiperwalk-2.0a1/Archive/run.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/staggered1d.nbl` & `hiperwalk-2.0a1/Archive/staggered1d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/staggered1d.py` & `hiperwalk-2.0a1/Archive/staggered1d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/staggered2d.nbl` & `hiperwalk-2.0a1/Archive/staggered2d.nbl`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/staggered2d.py` & `hiperwalk-2.0a1/Archive/staggered2d.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/standardDeviation.py` & `hiperwalk-2.0a1/Archive/standardDeviation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/state.py` & `hiperwalk-2.0a1/Archive/state.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/testmode.py` & `hiperwalk-2.0a1/Archive/testmode.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/Archive/walks.py` & `hiperwalk-2.0a1/Archive/walks.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/docs/Makefile` & `hiperwalk-2.0a1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/docs/conf.py` & `hiperwalk-2.0a1/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 # -- Project information -----------------------------------------------------
 
 project = 'Hiperwalk'
 copyright = '2023'
 author = 'Gustavo Bezerra'
 
 # The full version, including alpha/beta/rc tags
-release = '2.0a0'
+release = '2.0a1'
 version = 'stable'
 
 
 # -- General configuration ---------------------------------------------------
 
 # Add any Sphinx extension module names here, as strings. They can be
 # extensions coming with Sphinx (named 'sphinx.ext.*') or your custom
```

### Comparing `hiperwalk-2.0a0/docs/index.rst` & `hiperwalk-2.0a1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/docs/make.bat` & `hiperwalk-2.0a1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/docs/_templates/automodule.rst` & `hiperwalk-2.0a1/docs/_templates/automodule.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/docs/development/index.rst` & `hiperwalk-2.0a1/docs/development/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/docs/graphviz/coined-model-edges-labels.dot` & `hiperwalk-2.0a1/docs/graphviz/coined-model-edges-labels.dot`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/docs/install/index.rst` & `hiperwalk-2.0a1/docs/install/index.rst`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/_constants.py` & `hiperwalk-2.0a1/hiperwalk/_constants.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+__version__ = '2.0a1'
+
 #Declares data types according to neblina-core
 #TODO: make it so it is not hardcoded
 NEBLINA_FLOAT = 2
 NEBLINA_COMPLEX = 13 
 
 from sys import modules as sys_modules
```

### Comparing `hiperwalk-2.0a0/hiperwalk/graph/cycle.py` & `hiperwalk-2.0a1/hiperwalk/graph/cycle.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/graph/graph.py` & `hiperwalk-2.0a1/hiperwalk/graph/graph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/graph/lattice.py` & `hiperwalk-2.0a1/hiperwalk/graph/lattice.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/graph/line.py` & `hiperwalk-2.0a1/hiperwalk/graph/line.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/plot/_animation.py` & `hiperwalk-2.0a1/hiperwalk/plot/_animation.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/plot/_plot.py` & `hiperwalk-2.0a1/hiperwalk/plot/_plot.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/quantum_walk/_pyneblina_interface.py` & `hiperwalk-2.0a1/hiperwalk/quantum_walk/_pyneblina_interface.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/quantum_walk/coined_walk.py` & `hiperwalk-2.0a1/hiperwalk/quantum_walk/coined_walk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/quantum_walk/continuous_walk.py` & `hiperwalk-2.0a1/hiperwalk/quantum_walk/continuous_walk.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/hiperwalk/quantum_walk/quantum_walk.py` & `hiperwalk-2.0a1/hiperwalk/quantum_walk/quantum_walk.py`

 * *Files 0% similar despite different names*

```diff
@@ -503,15 +503,15 @@
 
         ###############################
         ### simulate implemantation ###
         ###############################
 
         time = np.array(self._time_to_tuple(time))
         if self._evolution is None:
-            self._evolution = self.get_evolution()
+            self._evolution = self.get_evolution(hpc=hpc)
 
         if not np.all([e.is_integer() for e in time]):
             raise ValueError("`time` has non-int entry.")
 
         start, end, step = time
```

### Comparing `hiperwalk-2.0a0/tests/unitary/coined_cycle.py` & `hiperwalk-2.0a1/tests/unitary/coined_cycle.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/tests/unitary/coined_line.py` & `hiperwalk-2.0a1/tests/unitary/coined_line.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/tests/unitary/coined_segment.py` & `hiperwalk-2.0a1/tests/unitary/coined_segment.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/tests/unitary/continuous_graph.py` & `hiperwalk-2.0a1/tests/unitary/continuous_graph.py`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/.gitignore` & `hiperwalk-2.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/LICENSE` & `hiperwalk-2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/README.md` & `hiperwalk-2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `hiperwalk-2.0a0/pyproject.toml` & `hiperwalk-2.0a1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "hiperwalk"
-version = "2.0a0"
+version = "2.0a1"
 description = "High-Performance Quantum Walk Simulator"
 license = {file="LICENSE"}
 readme = "README.md"
 authors = [
   { name="Gustavo Bezerra", email="gbezerra@posgrad.lncc.br" },
   { name="Paulo Motta", email="prmottajr@gmail.com" },
   { name="Renato Portugal", email="portugal@lncc.br" },
@@ -22,15 +22,15 @@
 	"scipy>=1.10",
 	"networkx>=3.1",
 	"matplotlib>=3.7",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
-	"License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)",
+	"License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)",
 	"Operating System :: POSIX :: Linux",
 ]
 
 
 [project.optional-dependencies]
 test = [
 	"pytest",
```

### Comparing `hiperwalk-2.0a0/PKG-INFO` & `hiperwalk-2.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiperwalk
-Version: 2.0a0
+Version: 2.0a1
 Summary: High-Performance Quantum Walk Simulator
 Project-URL: homepage, http://qubit.lncc.br/qwalk/
 Project-URL: documentation, https://hiperwalk.readthedocs.io/
 Project-URL: source, https://github.com/hiperwalk/hiperwalk
 Author-email: Gustavo Bezerra <gbezerra@posgrad.lncc.br>, Paulo Motta <prmottajr@gmail.com>, Renato Portugal <portugal@lncc.br>
 Maintainer-email: Hiperwalk Organization <hiperwalk@gmail.com>
 License: GNU Lesser General Public License
@@ -167,15 +167,15 @@
         
         If the Library as you received it specifies that a proxy can decide
         whether future versions of the GNU Lesser General Public License shall
         apply, that proxy's public statement of acceptance of any version is
         permanent authorization for you to choose that version for the
         Library.
 License-File: LICENSE
-Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.7
 Requires-Dist: matplotlib>=3.7
 Requires-Dist: networkx>=3.1
 Requires-Dist: numpy>=1.24
```

