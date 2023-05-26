# Comparing `tmp/qibolab-0.0.3.tar.gz` & `tmp/qibolab-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qibolab-0.0.3.tar", max compression
+gzip compressed data, was "qibolab-0.0.4.tar", max compression
```

## Comparing `qibolab-0.0.3.tar` & `qibolab-0.0.4.tar`

### file list

```diff
@@ -1,50 +1,56 @@
--rw-r--r--   0        0        0      204 2023-05-22 11:44:47.469454 qibolab-0.0.3/.readthedocs.yml
--rw-r--r--   0        0        0    11357 2023-05-22 11:44:47.469454 qibolab-0.0.3/LICENSE
--rw-r--r--   0        0        0     3266 2023-05-22 11:44:47.469454 qibolab-0.0.3/README.md
--rw-r--r--   0        0        0     1992 2023-05-22 11:44:47.529459 qibolab-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      110 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/__init__.py
--rw-r--r--   0        0        0     6327 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/backends.py
--rw-r--r--   0        0        0      109 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/designs/__init__.py
--rw-r--r--   0        0        0     4890 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/designs/channels.py
--rw-r--r--   0        0        0     3021 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/designs/design.py
--rw-r--r--   0        0        0        0 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/__init__.py
--rw-r--r--   0        0        0     2714 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/abstract.py
--rw-r--r--   0        0        0     7736 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/dummy.py
--rw-r--r--   0        0        0      726 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/dummy_oscillator.py
--rw-r--r--   0        0        0     8021 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/erasynth.py
--rw-r--r--   0        0        0    12572 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/icarusq.py
--rw-r--r--   0        0        0     9126 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/icarusqfpga.py
--rw-r--r--   0        0        0   147723 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/qblox.py
--rw-r--r--   0        0        0    42699 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/qm.py
--rw-r--r--   0        0        0     2144 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/qmsim.py
--rw-r--r--   0        0        0     6466 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/qutech.py
--rw-r--r--   0        0        0    20329 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/rfsoc.py
--rw-r--r--   0        0        0     5034 2023-05-22 11:44:47.529459 qibolab-0.0.3/src/qibolab/instruments/rohde_schwarz.py
--rw-r--r--   0        0        0      272 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/paths.py
--rw-r--r--   0        0        0     9354 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platform.py
--rw-r--r--   0        0        0        0 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/__init__.py
--rw-r--r--   0        0        0    29895 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/abstract.py
--rw-r--r--   0        0        0     6646 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/icplatform.py
--rw-r--r--   0        0        0    26191 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/multiqubit.py
--rw-r--r--   0        0        0     3112 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/platforms/platform.py
--rw-r--r--   0        0        0    68007 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/pulses.py
--rw-r--r--   0        0        0     3020 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/result.py
--rw-r--r--   0        0        0     8260 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/dummy.yml
--rw-r--r--   0        0        0     2057 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/icarusq.yml
--rw-r--r--   0        0        0     4751 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/multiqubit_icarusq.yml
--rw-r--r--   0        0        0     4423 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/multiqubit_icarusqfpga.yml
--rw-r--r--   0        0        0     4033 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/qili1q_os2.yml
--rw-r--r--   0        0        0     8282 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/qw5q_gold.yml
--rw-r--r--   0        0        0    15895 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/qw5q_gold_qblox.yml
--rw-r--r--   0        0        0      946 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/runcards/tii1q_b1.yml
--rw-r--r--   0        0        0     2937 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/sweeper.py
--rw-r--r--   0        0        0    19979 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/symbolic.py
--rw-r--r--   0        0        0      311 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/__init__.py
--rw-r--r--   0        0        0     2019 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/abstract.py
--rw-r--r--   0        0        0      977 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/fusion.py
--rw-r--r--   0        0        0    14368 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/gate_decompositions.py
--rw-r--r--   0        0        0    19396 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/general_connectivity.py
--rw-r--r--   0        0        0     1932 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/pipeline.py
--rw-r--r--   0        0        0     6247 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/star_connectivity.py
--rw-r--r--   0        0        0     8264 2023-05-22 11:44:47.533460 qibolab-0.0.3/src/qibolab/transpilers/unitary_decompositions.py
--rw-r--r--   0        0        0     4174 1970-01-01 00:00:00.000000 qibolab-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      204 2023-05-26 11:08:04.360072 qibolab-0.0.4/.readthedocs.yml
+-rw-r--r--   0        0        0    11357 2023-05-26 11:08:04.360072 qibolab-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3266 2023-05-26 11:08:04.360072 qibolab-0.0.4/README.md
+-rw-r--r--   0        0        0     2281 2023-05-26 11:08:04.416072 qibolab-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2344 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/__init__.py
+-rw-r--r--   0        0        0     7118 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/backends.py
+-rw-r--r--   0        0        0       48 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/compilers/__init__.py
+-rw-r--r--   0        0        0     5348 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/compilers/compiler.py
+-rw-r--r--   0        0        0     1978 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/compilers/default.py
+-rw-r--r--   0        0        0      109 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/designs/__init__.py
+-rw-r--r--   0        0        0     5843 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/designs/channels.py
+-rw-r--r--   0        0        0     3021 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/designs/design.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/__init__.py
+-rw-r--r--   0        0        0     2714 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/abstract.py
+-rw-r--r--   0        0        0     8301 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/dummy.py
+-rw-r--r--   0        0        0      775 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/dummy_oscillator.py
+-rw-r--r--   0        0        0     8021 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/erasynth.py
+-rw-r--r--   0        0        0    12572 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/icarusq.py
+-rw-r--r--   0        0        0     9126 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/icarusqfpga.py
+-rw-r--r--   0        0        0   147723 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/qblox.py
+-rw-r--r--   0        0        0    42681 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/qm.py
+-rw-r--r--   0        0        0     2120 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/qmsim.py
+-rw-r--r--   0        0        0     6466 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/qutech.py
+-rw-r--r--   0        0        0    23144 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/rfsoc.py
+-rw-r--r--   0        0        0     5034 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/rohde_schwarz.py
+-rw-r--r--   0        0        0    43695 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/instruments/zhinst.py
+-rw-r--r--   0        0        0      272 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/paths.py
+-rw-r--r--   0        0        0    14941 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/platform.py
+-rw-r--r--   0        0        0        0 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/platforms/__init__.py
+-rw-r--r--   0        0        0    23996 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/platforms/abstract.py
+-rw-r--r--   0        0        0     6640 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/platforms/icplatform.py
+-rw-r--r--   0        0        0    26096 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/platforms/multiqubit.py
+-rw-r--r--   0        0        0     7234 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/platforms/native.py
+-rw-r--r--   0        0        0     4227 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/platforms/platform.py
+-rw-r--r--   0        0        0    68219 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/pulses.py
+-rw-r--r--   0        0        0     5546 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/result.py
+-rw-r--r--   0        0        0     8162 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/runcards/dummy.yml
+-rw-r--r--   0        0        0     2057 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/runcards/icarusq.yml
+-rw-r--r--   0        0        0     8323 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/runcards/iqm5q.yml
+-rw-r--r--   0        0        0     4745 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/runcards/multiqubit_icarusq.yml
+-rw-r--r--   0        0        0     4417 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/runcards/multiqubit_icarusqfpga.yml
+-rw-r--r--   0        0        0     3994 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/runcards/qili1q_os2.yml
+-rw-r--r--   0        0        0     8160 2023-05-26 11:08:04.416072 qibolab-0.0.4/src/qibolab/runcards/qw5q_gold.yml
+-rw-r--r--   0        0        0    15750 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/runcards/qw5q_gold_qblox.yml
+-rw-r--r--   0        0        0      981 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/runcards/tii1q_b1.yml
+-rw-r--r--   0        0        0     3034 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/sweeper.py
+-rw-r--r--   0        0        0    19979 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/symbolic.py
+-rw-r--r--   0        0        0      311 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/transpilers/__init__.py
+-rw-r--r--   0        0        0     2019 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/transpilers/abstract.py
+-rw-r--r--   0        0        0      977 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/transpilers/fusion.py
+-rw-r--r--   0        0        0    13986 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/transpilers/gate_decompositions.py
+-rw-r--r--   0        0        0    19396 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/transpilers/general_connectivity.py
+-rw-r--r--   0        0        0     1932 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/transpilers/pipeline.py
+-rw-r--r--   0        0        0     6247 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/transpilers/star_connectivity.py
+-rw-r--r--   0        0        0     8264 2023-05-26 11:08:04.420072 qibolab-0.0.4/src/qibolab/transpilers/unitary_decompositions.py
+-rw-r--r--   0        0        0     4581 1970-01-01 00:00:00.000000 qibolab-0.0.4/PKG-INFO
```

### Comparing `qibolab-0.0.3/LICENSE` & `qibolab-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/README.md` & `qibolab-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/pyproject.toml` & `qibolab-0.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "qibolab"
-version = "0.0.3"
+version = "0.0.4"
 description = "Quantum hardware module and drivers for Qibo"
 authors = ["The Qibo team"]
 license = "Apache License 2.0"
 readme = "README.md"
 homepage = "https://qibo.science/"
 repository = "https://github.com/qiboteam/qibolab/"
 documentation = "https://qibo.science/docs/qibolab/stable"
@@ -17,19 +17,26 @@
   "Programming Language :: Python :: 3",
   "Topic :: Scientific/Engineering :: Physics",
 ]
 packages = [{ include = "qibolab", from = "src" }]
 include = ["*.out", "*.yml"]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.12"
+python = ">=3.9,<3.12"
 qibo = "^0.1.12"
 networkx = "^3.0"
 more-itertools = "^9.1.0"
 pyyaml = "^6.0"
+qblox-instruments = {version = "0.9.0", optional = true}
+qcodes = {version ="^0.37.0", optional = true}
+qcodes_contrib_drivers = {version ="0.18.0", optional = true}
+pyvisa-py = {version ="0.5.3", optional = true}
+qm-qua = {version ="==1.1.1", optional = true}
+qualang-tools = {version ="==0.14.0", optional = true}
+laboneq = {version ="==2.4.0", optional = true}
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 sphinx = "^6.1.3"
 furo = "^2023.3.27"
@@ -50,24 +57,19 @@
 
 [tool.poetry.group.analysis]
 optional = true
 
 [tool.poetry.group.analysis.dependencies]
 pylint = ">=2.16.0"
 
-[tool.poetry.group.tiiq]
-optional = true
+[tool.poetry.extras]
+qblox  = ["qblox-instruments", "qcodes", "qcodes_contrib_drivers", "pyvisa-py"]
+qm = ["qm-qua", "qualang-tools"]
+zh = ["laboneq"]
 
-[tool.poetry.group.tiiq.dependencies]
-qblox-instruments = "0.9.0"
-qcodes = "^0.37.0"
-qcodes_contrib_drivers = "0.18.0"
-pyvisa-py = "0.5.3"
-qm-qua = "==1.1.1"
-qualang-tools = "==0.14.0"
 
 [tool.poe.tasks]
 test = "pytest"
 lint = "pylint src --errors-only"
 lint-warnings = "pylint src --exit-zero"
 docs = "make -C doc html"
 docs-clean = "make -C doc clean"
```

### Comparing `qibolab-0.0.3/src/qibolab/backends.py` & `qibolab-0.0.4/src/qibolab/backends.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import numpy as np
 from qibo import __version__ as qibo_version
 from qibo import gates
 from qibo.backends import NumpyBackend
 from qibo.config import log, raise_error
 from qibo.states import CircuitResult
 
+from qibolab import ExecutionParameters
 from qibolab import __version__ as qibolab_version
+from qibolab.compilers import Compiler
 from qibolab.platform import Platform
 from qibolab.platforms.abstract import AbstractPlatform
 from qibolab.transpilers import Pipeline
 
 
 class QibolabBackend(NumpyBackend):
     def __init__(self, platform, runcard=None):
@@ -22,22 +24,42 @@
         else:
             self.platform = Platform(platform, runcard)
         self.versions = {
             "qibo": qibo_version,
             "numpy": self.np.__version__,
             "qibolab": qibolab_version,
         }
-        self.transpiler = Pipeline.default(self.platform.two_qubit_natives)
+        self.compiler = Compiler.default()
+        self.transpiler = Pipeline.default(self.platform.two_qubit_native_types)
 
     def apply_gate(self, gate, state, nqubits):  # pragma: no cover
         raise_error(NotImplementedError, "Qibolab cannot apply gates directly.")
 
     def apply_gate_density_matrix(self, gate, state, nqubits):  # pragma: no cover
         raise_error(NotImplementedError, "Qibolab cannot apply gates directly.")
 
+    def assign_measurements(self, measurement_map, circuit_result):
+        """Assigning measurement outcomes to :class:`qibo.states.MeasurementResult` for each gate.
+
+        This allows properly obtaining the measured shots from the :class:`qibo.states.CircuitResult`
+        object returned by the circuit execution.
+
+        Args:
+            measurement_map (dict): Map from each measurement gate to the sequence of
+                readout pulses implementing it.
+            circuit_result (:class:`qibo.states.CircuitResult`): Circuit result object
+                containing the readout measurement shots. This is created in ``execute_circuit``.
+        """
+        readout = circuit_result.execution_result
+        for gate, sequence in measurement_map.items():
+            _samples = (readout[pulse.serial].samples for pulse in sequence.pulses)
+            samples = list(filter(lambda x: x is not None, _samples))
+            gate.result.backend = self
+            gate.result.register_samples(np.array(samples).T)
+
     def execute_circuit(
         self, circuit, initial_state=None, nshots=None, fuse_one_qubit=False, check_transpiled=False
     ):  # pragma: no cover
         """Executes a quantum circuit.
 
         Args:
             circuit (:class:`qibo.models.circuit.Circuit`): Circuit to execute.
@@ -51,15 +73,15 @@
             check_transpiled (bool): If ``True`` it checks that the transpiled
                 circuit is equivalent to the original using simulation.
 
         Returns:
             CircuitResult object containing the results acquired from the execution.
         """
         if isinstance(initial_state, type(circuit)):
-            self.execute_circuit(
+            return self.execute_circuit(
                 circuit=initial_state + circuit,
                 nshots=nshots,
                 fuse_one_qubit=fuse_one_qubit,
                 check_transpiled=check_transpiled,
             )
         elif initial_state is not None:
             raise_error(
@@ -73,37 +95,29 @@
             # Transform a circuit into proper connectivity and native gates
             native_circuit, qubit_map = self.transpiler.transpile(circuit)
             # TODO: Use the qubit map to properly map measurements
             if check_transpiled:
                 self.transpiler.check_execution(circuit, native_circuit)
 
         # Transpile the native circuit into a sequence of pulses ``PulseSequence``
-        sequence = self.platform.transpile(native_circuit)
+        sequence, measurement_map = self.compiler.compile(native_circuit, self.platform)
 
         if not self.platform.is_connected:
             self.platform.connect()
             self.platform.setup()
 
         # Execute the pulse sequence on the platform
         self.platform.start()
-        readout = self.platform.execute_pulse_sequence(sequence, nshots)
+        readout = self.platform.execute_pulse_sequence(
+            sequence,
+            ExecutionParameters(nshots=nshots),
+        )
         self.platform.stop()
-        result = CircuitResult(self, native_circuit, readout, nshots)
-
-        # Register measurement outcomes
-        if isinstance(readout, dict):
-            for gate in native_circuit.queue:
-                if isinstance(gate, gates.M):
-                    samples = []
-                    for serial in gate.pulses:
-                        shots = readout[serial].shots
-                        if shots is not None:
-                            samples.append(shots)
-                    gate.result.backend = self
-                    gate.result.register_samples(np.array(samples).T)
+        result = CircuitResult(self, circuit, readout, nshots)
+        self.assign_measurements(measurement_map, result)
         return result
 
     def circuit_result_tensor(self, result):
         raise_error(
             NotImplementedError,
             "Qibolab cannot return state vector in tensor representation.",
         )
@@ -119,25 +133,25 @@
             qubits = result.measurement_gate.qubits
 
         # basic classification
         probabilities = []
         for qubit in qubits:
             # execution_result[qubit] provides the latest acquisition data for the corresponding qubit
             qubit_result = result.execution_result[qubit]
-            if qubit_result.shots is None:
+            if qubit_result.samples is None:
                 mean_state0 = complex(self.platform.qubits[qubit].mean_gnd_states)
                 mean_state1 = complex(self.platform.qubits[qubit].mean_exc_states)
                 measurement = complex(qubit_result.I, qubit_result.Q)
                 d0 = abs(measurement - mean_state0)
                 d1 = abs(measurement - mean_state1)
                 d01 = abs(mean_state0 - mean_state1)
                 p = (d1**2 + d01**2 - d0**2) / 2 / d01**2
                 probabilities.append([p, 1 - p])
             else:
-                outcomes, counts = np.unique(qubit_result.shots, return_counts=True)
+                outcomes, counts = np.unique(qubit_result.samples, return_counts=True)
                 probabilities.append([0, 0])
                 for i, c in zip(outcomes.astype(int), counts):
                     probabilities[-1][i] = c / result.nshots
 
         # bring probabilities to the format returned by simulation
         return np.array(
             [
```

### Comparing `qibolab-0.0.3/src/qibolab/designs/channels.py` & `qibolab-0.0.4/src/qibolab/designs/channels.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,15 +28,18 @@
     Used to read the sweetspot and filters for flux channels only. ``None`` for non-flux channels.
     """
     ports: List[tuple] = field(default_factory=list)
     """List of tuples (controller, port) connected to this channel."""
     _local_oscillator: Optional[LocalOscillator] = None
     """Instrument object controlling the local oscillator connected to this channel.
     Not applicable for setups that do not use local oscillators because the controller
-    can send sufficiently high frequencies
+    can send sufficiently high frequencies.
+    """
+    power_range: Optional[float] = None
+    """Channel amplification or attenuation of the selected on the device
     """
     _bias: Optional[float] = None
     """DC offset that should be applied in the channel in order to shift the
     frequency of the qubit, usually to put it in its sweetspot.
     Relevant only for flux channels and flux-tunable transmon qubits.
     """
     _filter: Optional[dict] = None
@@ -51,29 +54,35 @@
     to avoid the operation of being executed in the real instruments.
     """
 
     @property
     def local_oscillator(self):
         """LocalOscillator object connnected to this channel."""
         if self._local_oscillator is None:
-            raise_error(NotImplementedError, f"Channel {self.name} does not have a local oscillator")
+            raise_error(
+                NotImplementedError,
+                f"Channel {self.name} does not have a local oscillator",
+            )
         return self._local_oscillator
 
     @local_oscillator.setter
     def local_oscillator(self, local_oscillator):
         if not isinstance(local_oscillator, LocalOscillator):
             raise_error(TypeError, "Attempting to set LocalOscillator failed.")
         self._local_oscillator = local_oscillator
 
     @property
     def bias(self):
         """Bias offset for flux channels."""
         if self._bias is None:
             if self.qubit.flux is None:
-                raise_error(NotImplementedError, f"Channel {self.name} is not connected to a flux qubit")
+                raise_error(
+                    NotImplementedError,
+                    f"Channel {self.name} is not connected to a flux qubit",
+                )
             # operate qubits at their sweetspot unless otherwise stated
             check_max_bias(self.qubit.sweetspot, self.max_bias)
             return self.qubit.sweetspot
         return self._bias
 
     @bias.setter
     def bias(self, bias):
@@ -91,14 +100,28 @@
 
     @filter.setter
     def filter(self, filter):
         if not isinstance(filter, dict):
             raise_error(TypeError, f"Channel filter must be dict but is {type(filter)}.")
         self._filter = filter
 
+    @property
+    def attenuation(self):
+        """Attenuation for qblox devices."""
+        if self._attenuation is None:
+            raise_error(
+                NotImplementedError,
+                f"Channel {self.name} does not support attenuation.",
+            )
+        return self._attenuation
+
+    @attenuation.setter
+    def attenuation(self, attenuation):
+        self._attenuation = attenuation
+
 
 @dataclass
 class ChannelMap:
     """Collection of :class:`qibolab.designs.channel.Channel` objects identified by name."""
 
     _channels: dict = field(default_factory=dict)
 
@@ -124,9 +147,16 @@
 
     def __or__(self, channel_map):
         channels = self._channels.copy()
         channels.update(channel_map._channels)
         return self.__class__(channels)
 
     def __ior__(self, channel_map):
+        if not isinstance(channel_map, type(self)):
+            try:
+                if isinstance(channel_map, str):
+                    raise TypeError
+                channel_map = type(self).from_names(*channel_map)
+            except TypeError:
+                channel_map = type(self).from_names(channel_map)
         self._channels.update(channel_map._channels)
         return self
```

### Comparing `qibolab-0.0.3/src/qibolab/designs/design.py` & `qibolab-0.0.4/src/qibolab/designs/design.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/instruments/abstract.py` & `qibolab-0.0.4/src/qibolab/instruments/abstract.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/instruments/dummy.py` & `qibolab-0.0.4/src/qibolab/instruments/dummy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import copy
 import time
+from typing import Dict, List, Union
 
 import numpy as np
 from qibo.config import log, raise_error
 
+from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.instruments.abstract import AbstractInstrument
+from qibolab.platforms.abstract import Qubit
 from qibolab.pulses import PulseSequence, PulseType
-from qibolab.result import ExecutionResults
-from qibolab.sweeper import Parameter
+from qibolab.sweeper import Parameter, Sweeper
 
 
 class DummyInstrument(AbstractInstrument):
     """Dummy instrument that returns random voltage values.
 
     Useful for testing code without requiring access to hardware.
 
@@ -34,28 +36,45 @@
 
     def stop(self):
         log.info("Stopping dummy instrument.")
 
     def disconnect(self):
         log.info("Disconnecting dummy instrument.")
 
-    def play(self, qubits, sequence, nshots, relaxation_time, raw_adc=False):
-        time.sleep(relaxation_time * 1e-9)
+    def play(self, qubits: Dict[Union[str, int], Qubit], sequence: PulseSequence, options: ExecutionParameters):
+        nshots = options.nshots
+        time.sleep(options.relaxation_time * 1e-9)
 
         ro_pulses = {pulse.qubit: pulse.serial for pulse in sequence.ro_pulses}
 
         results = {}
         for qubit, serial in ro_pulses.items():
-            i = np.random.rand(nshots)
-            q = np.random.rand(nshots)
-            shots = np.random.rand(nshots)
-            results[qubit] = results[serial] = ExecutionResults.from_components(i, q, shots)
+            if options.acquisition_type is AcquisitionType.DISCRIMINATION:
+                samples = (
+                    np.random.rand(1) if options.averaging_mode is AveragingMode.CYCLIC else np.random.rand(nshots)
+                )
+                results[qubit] = results[serial] = options.results_type(samples)
+
+            else:
+                i = np.random.rand(1) if options.averaging_mode is AveragingMode.CYCLIC else np.random.rand(nshots)
+                q = np.random.rand(1) if options.averaging_mode is AveragingMode.CYCLIC else np.random.rand(nshots)
+                exp_res = i + 1j * q
+                results[qubit] = results[serial] = options.results_type(data=exp_res)
+
+            # results[qubit] = results[serial] = ExecutionResults.from_components(i, q, shots)
+
         return results
 
-    def sweep(self, qubits, sequence, *sweepers, nshots=1024, average=True, relaxation_time=None):
+    def sweep(
+        self,
+        qubits: Dict[Union[str, int], Qubit],
+        sequence: PulseSequence,
+        options: ExecutionParameters,
+        *sweepers: List[Sweeper]
+    ):
         results = {}
         sweeper_pulses = {}
 
         # create copy of the sequence
         copy_sequence = copy.deepcopy(sequence)
         map_original_shifted = {pulse: pulse.serial for pulse in copy.deepcopy(copy_sequence).ro_pulses}
 
@@ -68,33 +87,29 @@
                 }
 
         # perform sweeping recursively
         self._sweep_recursion(
             qubits,
             copy_sequence,
             copy.deepcopy(sequence),
+            options,
             *sweepers,
-            nshots=nshots,
-            average=average,
-            relaxation_time=relaxation_time,
             results=results,
             sweeper_pulses=sweeper_pulses,
             map_original_shifted=map_original_shifted
         )
         return results
 
     def _sweep_recursion(
         self,
         qubits,
         sequence,
         original_sequence,
+        options,
         *sweepers,
-        nshots=1024,
-        average=True,
-        relaxation_time=None,
         results=None,
         sweeper_pulses=None,
         map_original_shifted=None
     ):
         sweeper = sweepers[0]
 
         # store values before starting to sweep
@@ -107,29 +122,27 @@
                 qubits, sweeper, sweeper_pulses, original_sequence, map_original_shifted, value
             )
             if len(sweepers) > 1:
                 self._sweep_recursion(
                     qubits,
                     sequence,
                     original_sequence,
+                    options,
                     *sweepers[1:],
-                    nshots=nshots,
-                    average=average,
-                    relaxation_time=relaxation_time,
                     results=results,
                     sweeper_pulses=sweeper_pulses,
                     map_original_shifted=map_original_shifted
                 )
             else:
                 new_sequence = copy.deepcopy(sequence)
-                result = self.play(qubits, new_sequence, nshots, relaxation_time)
+                result = self.play(qubits, new_sequence, options)
 
                 # colllect result and append to original pulse
                 for original_pulse, new_serial in map_original_shifted.items():
-                    acquisition = result[new_serial].average if average else result[new_serial]
+                    acquisition = result[new_serial]
                     if original_pulse.serial in results:
                         results[original_pulse.serial] += acquisition
                         results[original_pulse.qubit] += acquisition
                     else:
                         results[original_pulse.serial] = acquisition
                         results[original_pulse.qubit] = copy.copy(results[original_pulse.serial])
         # restore initial value of the pulse
```

### Comparing `qibolab-0.0.3/src/qibolab/instruments/erasynth.py` & `qibolab-0.0.4/src/qibolab/instruments/erasynth.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/instruments/icarusq.py` & `qibolab-0.0.4/src/qibolab/instruments/icarusq.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/instruments/icarusqfpga.py` & `qibolab-0.0.4/src/qibolab/instruments/icarusqfpga.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/instruments/qblox.py` & `qibolab-0.0.4/src/qibolab/instruments/qblox.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/instruments/qm.py` & `qibolab-0.0.4/src/qibolab/instruments/qm.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,36 @@
 import collections
 import math
+from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import Dict, List, Optional
 
 import numpy as np
 from qibo.config import log, raise_error
 from qm import qua
-from qm.qua import (
-    align,
-    assign,
-    declare,
-    declare_stream,
-    dual_demod,
-    fixed,
-    for_,
-    frame_rotation_2pi,
-    measure,
-    play,
-    program,
-    reset_frame,
-    reset_phase,
-    stream_processing,
-    wait,
-)
+from qm.qua import declare, declare_stream, fixed, for_
 from qm.qua._dsl import _ResultSource, _Variable  # for type declaration only
 from qm.QuantumMachinesManager import QuantumMachinesManager
+from qualang_tools.addons.variables import assign_variables_to_element
 from qualang_tools.bakery import baking
 from qualang_tools.loops import from_array
 from qualang_tools.units import unit
 
+from qibolab import AcquisitionType, AveragingMode
 from qibolab.designs.channels import check_max_bias
 from qibolab.instruments.abstract import AbstractInstrument
 from qibolab.pulses import Pulse, PulseType, Rectangular
-from qibolab.result import AveragedResults, ExecutionResults
+from qibolab.result import (
+    AveragedIntegratedResults,
+    AveragedRawWaveformResults,
+    AveragedSampleResults,
+    IntegratedResults,
+    RawWaveformResults,
+    SampleResults,
+)
 from qibolab.sweeper import Parameter
 
 
 @dataclass
 class QMConfig:
     """Configuration for communicating with the ``QuantumMachinesManager``."""
 
@@ -336,64 +330,200 @@
                     "sine": [(-np.cos(iq_angle), readout_len)],
                 },
             }
         )
 
 
 @dataclass
-class AcquisitionVariables:
+class Acquisition(ABC):
     """QUA variables used for saving of acquisition results.
+
     This class can be instantiated only within a QUA program scope.
     Each readout pulse is associated with its own set of acquisition variables.
     """
 
+    serial: str
+    """Serial of the readout pulse that generates this acquisition."""
+    average: bool
+
+    @abstractmethod
+    def assign_element(self, element):
+        """Assign acquisition variables to the corresponding QM controlled.
+
+        Proposed to do by QM to avoid crashes.
+
+        Args:
+            element (str): Element (from ``config``) that the pulse will be applied on.
+        """
+
+    @abstractmethod
+    def measure(self, operation, element):
+        """Send measurement pulse and acquire results.
+
+        Args:
+            operation (str): Operation (from ``config``) corresponding to the pulse to be played.
+            element (str): Element (from ``config``) that the pulse will be applied on.
+        """
+
+    @abstractmethod
+    def save(self):
+        """Save acquired results from variables to streams."""
+
+    @abstractmethod
+    def download(self, *dimensions):
+        """Save streams to prepare for fetching from host device.
+
+        Args:
+            dimensions (int): Dimensions to use for buffer of data.
+        """
+
+    @abstractmethod
+    def fetch(self):
+        """Fetch downloaded streams to host device."""
+
+
+@dataclass
+class RawAcquisition(Acquisition):
+    """QUA variables used for raw waveform acquisition."""
+
+    adc_stream: _ResultSource = field(default_factory=lambda: declare_stream(adc_trace=True))
+    """Stream to collect raw ADC data."""
+
+    def assign_element(self, element):
+        pass
+
+    def measure(self, operation, element):
+        qua.measure(operation, element, self.adc_stream)
+
+    def save(self):
+        pass
+
+    def download(self, *dimensions):
+        i_stream = self.adc_stream.input1()
+        q_stream = self.adc_stream.input2()
+        if self.average:
+            i_stream = i_stream.average()
+            q_stream = q_stream.average()
+        i_stream.save(f"{self.serial}_I")
+        q_stream.save(f"{self.serial}_Q")
+
+    def fetch(self, handles):
+        ires = handles.get(f"{self.serial}_I").fetch_all()
+        qres = handles.get(f"{self.serial}_Q").fetch_all()
+        # convert raw ADC signal to volts
+        u = unit()
+        ires = u.raw2volts(ires)
+        qres = u.raw2volts(qres)
+        if self.average:
+            return AveragedRawWaveformResults(ires + 1j * qres)
+        return RawWaveformResults(ires + 1j * qres)
+
+
+@dataclass
+class IntegratedAcquisition(Acquisition):
+    """QUA variables used for integrated acquisition."""
+
     I: _Variable = field(default_factory=lambda: declare(fixed))
     Q: _Variable = field(default_factory=lambda: declare(fixed))
     """Variables to save the (I, Q) values acquired from a single shot."""
     I_stream: _ResultSource = field(default_factory=lambda: declare_stream())
     Q_stream: _ResultSource = field(default_factory=lambda: declare_stream())
     """Streams to collect the results of all shots."""
 
-    raw_adc: bool = False
-    """Flag to select whether we are acquiring raw ADC data."""
-    adc_stream: Optional[_ResultSource] = None
-    """Stream to collect raw ADC data."""
+    def assign_element(self, element):
+        assign_variables_to_element(element, self.I, self.Q)
+
+    def measure(self, operation, element):
+        qua.measure(
+            operation,
+            element,
+            None,
+            qua.dual_demod.full("cos", "out1", "sin", "out2", self.I),
+            qua.dual_demod.full("minus_sin", "out1", "cos", "out2", self.Q),
+        )
+
+    def save(self):
+        qua.save(self.I, self.I_stream)
+        qua.save(self.Q, self.Q_stream)
+
+    def download(self, *dimensions):
+        Istream = self.I_stream
+        Qstream = self.Q_stream
+        for dim in dimensions:
+            Istream = Istream.buffer(dim)
+            Qstream = Qstream.buffer(dim)
+        if self.average:
+            Istream = Istream.average()
+            Qstream = Qstream.average()
+        Istream.save(f"{self.serial}_I")
+        Qstream.save(f"{self.serial}_Q")
+
+    def fetch(self, handles):
+        ires = handles.get(f"{self.serial}_I").fetch_all()
+        qres = handles.get(f"{self.serial}_Q").fetch_all()
+        if self.average:
+            # TODO: calculate std
+            return AveragedIntegratedResults(ires + 1j * qres)
+        return IntegratedResults(ires + 1j * qres)
 
-    threshold: Optional[float] = None
+
+@dataclass
+class ShotsAcquisition(Acquisition):
+    """QUA variables used for shot classification.
+
+    Threshold and angle must be given in order to classify shots.
+    """
+
+    threshold: float
     """Threshold to be used for classification of single shots."""
-    angle: Optional[float] = None
+    angle: float
     """Angle in the IQ plane to be used for classification of single shots."""
-    shot: Optional[_Variable] = None
-    shots: Optional[_ResultSource] = None
-    """Variable and stream to collect the classified shots.
-    Used only if a threshold and angle is given.
-    """
+
+    I: _Variable = field(default_factory=lambda: declare(fixed))
+    Q: _Variable = field(default_factory=lambda: declare(fixed))
+    """Variables to save the (I, Q) values acquired from a single shot."""
+    shot: _Variable = field(default_factory=lambda: declare(bool))
+    """Variable for calculating an individual shots."""
+    shots: _ResultSource = field(default_factory=lambda: declare_stream())
+    """Stream to collect multiple shots."""
 
     def __post_init__(self):
-        """Create QUA variables needed for single shot classification."""
-        if self.raw_adc:
-            self.adc_stream = declare_stream(adc_trace=True)
-
-        if self.threshold is not None and self.angle is not None:
-            self.shot = declare(bool)
-            self.shots = declare_stream()
-            self.cos = np.cos(self.angle)
-            self.sin = np.sin(self.angle)
+        self.cos = np.cos(self.angle)
+        self.sin = np.sin(self.angle)
+
+    def assign_element(self, element):
+        assign_variables_to_element(element, self.I, self.Q, self.shot)
+
+    def measure(self, operation, element):
+        qua.measure(
+            operation,
+            element,
+            None,
+            qua.dual_demod.full("cos", "out1", "sin", "out2", self.I),
+            qua.dual_demod.full("minus_sin", "out1", "cos", "out2", self.Q),
+        )
+        qua.assign(self.shot, self.I * self.cos - self.Q * self.sin > self.threshold)
 
     def save(self):
-        """QUA instruction to save acquired results from variables to streams."""
-        qua.save(self.I, self.I_stream)
-        qua.save(self.Q, self.Q_stream)
-        if self.shot is not None:
-            qua.save(self.shot, self.shots)
+        qua.save(self.shot, self.shots)
 
-    def classify_shots(self):
-        """QUA instruction to classify shots in real time and save the result to a variable."""
-        if self.threshold is not None and self.angle is not None:
-            assign(self.shot, self.I * self.cos - self.Q * self.sin > self.threshold)
+    def download(self, *dimensions):
+        shots = self.shots
+        for dim in dimensions:
+            shots = shots.buffer(dim)
+        if self.average:
+            shots = shots.average()
+        shots.save(f"{self.serial}_shots")
+
+    def fetch(self, handles):
+        shots = handles.get(f"{self.serial}_shots").fetch_all().astype(int)
+        if self.average:
+            # TODO: calculate std
+            return AveragedSampleResults(shots)
+        return SampleResults(shots)
 
 
 class QMPulse:
     """Wrapper around :class:`qibolab.pulses.Pulse` for easier translation to QUA program."""
 
     def __init__(self, pulse: Pulse):
         self.pulse: Pulse = pulse
@@ -408,15 +538,15 @@
         self.duration: int = pulse.duration
         """Duration of the pulse. May be overrident when sweeping duration."""
         self.wait_time: int = 0
         """Time (in clock cycles) to wait before playing this pulse.
         Calculated and assigned by :meth:`qibolab.instruments.qm.Sequence.add`."""
         self.wait_time_variable: Optional[_Variable] = None
         """Time (in clock cycles) to wait before playing this pulse when we are sweeping delay."""
-        self.acquisition: AcquisitionVariables = None
+        self.acquisition: Acquisition = None
         """Data class containing the variables required for data acquisition for the instrument."""
 
         self.next: set = set()
         """Pulses that will be played after the current pulse.
         These pulses need to be re-aligned if we are sweeping the delay or duration."""
 
         self.baked = None
@@ -434,16 +564,30 @@
         if self.wait_time_variable is not None:
             return self.wait_time_variable + self.wait_time
         elif self.wait_time >= 4:
             return self.wait_time
         else:
             return None
 
-    def declare_output(self, threshold=None, angle=None, raw_adc=False):
-        self.acquisition = AcquisitionVariables(threshold=threshold, angle=angle, raw_adc=raw_adc)
+    def declare_output(self, options, threshold=None, angle=None):
+        average = options.averaging_mode is AveragingMode.CYCLIC
+        acquisition_type = options.acquisition_type
+        if acquisition_type is AcquisitionType.RAW:
+            self.acquisition = RawAcquisition(self.pulse.serial, average)
+        elif acquisition_type is AcquisitionType.INTEGRATION:
+            self.acquisition = IntegratedAcquisition(self.pulse.serial, average)
+        elif acquisition_type is AcquisitionType.DISCRIMINATION:
+            if threshold is None or angle is None:
+                raise_error(
+                    ValueError, "Cannot use ``AcquisitionType.DISCRIMINATION`` " "if threshold and angle are not given."
+                )
+            self.acquisition = ShotsAcquisition(self.pulse.serial, average, threshold, angle)
+        else:
+            raise_error(ValueError, f"Invalid acquisition type {acquisition_type}.")
+        self.acquisition.assign_element(self.element)
 
     def bake(self, config: QMConfig):
         if self.baked is not None:
             raise_error(RuntimeError, f"Bake was already called for {self.pulse}.")
         # ! Only works for flux pulses that have zero Q waveform
 
         # Create the different baked sequences, each one corresponding to a different truncated duration
@@ -634,207 +778,71 @@
             else:
                 if pulse.duration % 4 != 0 or pulse.duration < 16:
                     raise_error(NotImplementedError, "1ns resolution is available for flux pulses only.")
                 self.config.register_pulse(qubits[pulse.qubit], pulse, self.time_of_flight, self.smearing)
         return qmsequence
 
     @staticmethod
-    def readout(qmpulse, raw_adc):
-        """Plays a readout pulse and assigns the acquired results in QUA variables.
-
-        Args:
-            qmpulse (:class:`qibolab.instruments.qm.QMPulse`): Readout pulse to play.
-            raw_adc (bool): If ``True`` it captures the raw ADC signal, otherwise it integrates.
-        """
-        acquisition = qmpulse.acquisition
-        if raw_adc:
-            measure(qmpulse.operation, qmpulse.element, acquisition.adc_stream)
-        else:
-            measure(
-                qmpulse.operation,
-                qmpulse.element,
-                None,
-                dual_demod.full("cos", "out1", "sin", "out2", acquisition.I),
-                dual_demod.full("minus_sin", "out1", "cos", "out2", acquisition.Q),
-            )
-            acquisition.classify_shots()
-
-    @staticmethod
-    def play_pulses(qmsequence, relaxation_time=0, raw_adc=False):
+    def play_pulses(qmsequence, relaxation_time=0):
         """Part of QUA program that plays an arbitrary pulse sequence.
 
         Should be used inside a ``program()`` context.
 
         Args:
             qmsequence (list): Pulse sequence containing QM specific pulses (``qmpulse``).
                 These pulses are defined in :meth:`qibolab.instruments.qm.QMOPX.play` and
                 hold attributes for the ``element`` and ``operation`` that corresponds to
                 each pulse, as defined in the QM config.
         """
         needs_reset = False
-        align()
+        qua.align()
         for qmpulse in qmsequence.qmpulses:
             pulse = qmpulse.pulse
             if qmpulse.wait_cycles is not None:
-                wait(qmpulse.wait_cycles, qmpulse.element)
+                qua.wait(qmpulse.wait_cycles, qmpulse.element)
             if pulse.type is PulseType.READOUT:
-                QMOPX.readout(qmpulse, raw_adc)
+                qmpulse.acquisition.measure(qmpulse.operation, qmpulse.element)
             else:
                 if not isinstance(qmpulse.relative_phase, float) or qmpulse.relative_phase != 0:
-                    frame_rotation_2pi(qmpulse.relative_phase, qmpulse.element)
+                    qua.frame_rotation_2pi(qmpulse.relative_phase, qmpulse.element)
                     needs_reset = True
                 if qmpulse.baked is not None:
                     if qmpulse.baked_amplitude is not None:
                         qmpulse.baked.run(amp_array=[(qmpulse.element, qmpulse.baked_amplitude)])
                     else:
                         qmpulse.baked.run()
                 else:
-                    play(qmpulse.operation, qmpulse.element)
+                    qua.play(qmpulse.operation, qmpulse.element)
                 if needs_reset:
-                    reset_frame(qmpulse.element)
+                    qua.reset_frame(qmpulse.element)
                     needs_reset = False
 
         # for Rabi-length?
         if relaxation_time > 0:
-            wait(relaxation_time // 4)
+            qua.wait(relaxation_time // 4)
 
         # Save data to the stream processing
-        if not raw_adc:
-            for qmpulse in qmsequence.ro_pulses:
-                qmpulse.acquisition.save()
+        for qmpulse in qmsequence.ro_pulses:
+            qmpulse.acquisition.save()
 
     @staticmethod
-    def fetch_results(result, ro_pulses, average, raw_adc=False):
+    def fetch_results(result, ro_pulses):
         """Fetches results from an executed experiment."""
         # TODO: Update result asynchronously instead of waiting
         # for all values, in order to allow live plotting
-        # import time
-        # for _ in range(5):
-        #    handles.is_processing()
-        #    time.sleep(1)
+        # using ``handles.is_processing()``
         handles = result.result_handles
         handles.wait_for_all_values()
         results = {}
-        for pulse in ro_pulses:
-            serial = pulse.serial
-            ires = handles.get(f"{serial}_I").fetch_all()
-            qres = handles.get(f"{serial}_Q").fetch_all()
-            if raw_adc:
-                # convert raw ADC signal to volts
-                u = unit()
-                ires = u.raw2volts(ires)
-                qres = u.raw2volts(qres)
-
-            if f"{serial}_shots" in handles:
-                shots = handles.get(f"{serial}_shots").fetch_all().astype(int)
-            else:
-                shots = None
-            results[pulse.qubit] = results[serial] = (
-                AveragedResults.from_components(ires, qres)
-                if average
-                else ExecutionResults.from_components(ires, qres, shots)
-            )
+        for qmpulse in ro_pulses:
+            pulse = qmpulse.pulse
+            results[pulse.qubit] = results[pulse.serial] = qmpulse.acquisition.fetch(handles)
         return results
 
     @staticmethod
-    def save_streams(qmpulse, nshots, raw_adc):
-        """Saves streams acquired from readout."""
-        serial = qmpulse.pulse.serial
-        acquisition = qmpulse.acquisition
-        if raw_adc:
-            acquisition.adc_stream.input1().average().save(f"{serial}_I")
-            acquisition.adc_stream.input2().average().save(f"{serial}_Q")
-        else:
-            acquisition.I_stream.buffer(nshots).save(f"{serial}_I")
-            acquisition.Q_stream.buffer(nshots).save(f"{serial}_Q")
-            if acquisition.threshold is not None:
-                acquisition.shots.buffer(nshots).save(f"{serial}_shots")
-
-    def play(self, qubits, sequence, nshots, relaxation_time, average=False, raw_adc=False):
-        """Plays an arbitrary pulse sequence using QUA program.
-
-        Args:
-            qubits (list): List of :class:`qibolab.platforms.utils.Qubit` objects
-                passed from the platform.
-            sequence (:class:`qibolab.pulses.PulseSequence`). Pulse sequence to play.
-            nshots (int): Number of repetitions (shots) of the experiment.
-            relaxation_time (int): Time to wait for the qubit to relax to its ground state between shots in ns.
-            average (bool): If True the return type is :class:`qibolab.result.AveragedResults` which includes
-                averaged values of i and q. If False the return type is :class:`qibolab.result.ExecutionResults`
-                which includes i, q and shot for each shots.
-        """
-        if not sequence:
-            return {}
-
-        qmsequence = self.create_qmsequence(qubits, sequence)
-        # play pulses using QUA
-        with program() as experiment:
-            n = declare(int)
-            for qmpulse in qmsequence.ro_pulses:
-                threshold = qubits[qmpulse.pulse.qubit].threshold
-                iq_angle = qubits[qmpulse.pulse.qubit].iq_angle
-                qmpulse.declare_output(threshold, iq_angle, raw_adc)
-
-            with for_(n, 0, n < nshots, n + 1):
-                self.play_pulses(qmsequence, relaxation_time, raw_adc)
-
-            with stream_processing():
-                for qmpulse in qmsequence.ro_pulses:
-                    self.save_streams(qmpulse, nshots, raw_adc)
-
-        result = self.execute_program(experiment)
-        return self.fetch_results(result, sequence.ro_pulses, average, raw_adc)
-
-    def sweep(self, qubits, sequence, *sweepers, nshots, relaxation_time, average=True):
-        if not sequence:
-            return {}
-
-        qmsequence = self.create_qmsequence(qubits, sequence)
-        # play pulses using QUA
-        with program() as experiment:
-            n = declare(int)
-            for qmpulse in qmsequence.ro_pulses:
-                if average:
-                    # not calculating single shots when averaging
-                    # during sweep so we do not pass ``threshold`` here
-                    qmpulse.declare_output()
-                else:
-                    threshold = qubits[qmpulse.pulse.qubit].threshold
-                    iq_angle = qubits[qmpulse.pulse.qubit].iq_angle
-                    qmpulse.declare_output(threshold, iq_angle)
-
-            with for_(n, 0, n < nshots, n + 1):
-                self.sweep_recursion(list(sweepers), qubits, qmsequence, relaxation_time)
-
-            with stream_processing():
-                for qmpulse in qmsequence.ro_pulses:
-                    acquisition = qmpulse.acquisition
-                    Ist_temp = acquisition.I_stream
-                    Qst_temp = acquisition.Q_stream
-                    if not average and acquisition.threshold is not None:
-                        shots_temp = acquisition.shots
-                    for sweeper in reversed(sweepers):
-                        Ist_temp = Ist_temp.buffer(len(sweeper.values))
-                        Qst_temp = Qst_temp.buffer(len(sweeper.values))
-                        if not average and acquisition.threshold is not None:
-                            shots_temp = shots_temp.buffer(len(sweeper.values))
-                    serial = qmpulse.pulse.serial
-                    if average:
-                        Ist_temp.average().save(f"{serial}_I")
-                        Qst_temp.average().save(f"{serial}_Q")
-                    else:
-                        Ist_temp.buffer(nshots).save(f"{serial}_I")
-                        Qst_temp.buffer(nshots).save(f"{serial}_Q")
-                        if acquisition.threshold is not None:
-                            shots_temp.buffer(nshots).save(f"{serial}_shots")
-
-        result = self.execute_program(experiment)
-        return self.fetch_results(result, sequence.ro_pulses, average, raw_adc=False)
-
-    @staticmethod
     def maximum_sweep_value(values, value0):
         """Calculates maximum value that is reached during a sweep.
 
         Useful to check whether a sweep exceeds the range of allowed values.
         Note that both the array of values we sweep and the center value can
         be negative, so we need to make sure that the maximum absolute value
         is within range.
@@ -956,7 +964,37 @@
             parameter = sweepers[0].parameter
             if parameter in self.SWEEPERS:
                 self.SWEEPERS[parameter](self, sweepers, qubits, qmsequence, relaxation_time)
             else:
                 raise_error(NotImplementedError, f"Sweeper for {parameter} is not implemented.")
         else:
             self.play_pulses(qmsequence, relaxation_time)
+
+    def play(self, qubits, sequence, options):
+        return self.sweep(qubits, sequence, options)
+
+    def sweep(self, qubits, sequence, options, *sweepers):
+        if not sequence:
+            return {}
+
+        buffer_dims = [len(sweeper.values) for sweeper in reversed(sweepers)]
+        if options.averaging_mode is AveragingMode.SINGLESHOT:
+            buffer_dims.append(options.nshots)
+
+        qmsequence = self.create_qmsequence(qubits, sequence)
+        # play pulses using QUA
+        with qua.program() as experiment:
+            n = declare(int)
+            for qmpulse in qmsequence.ro_pulses:
+                threshold = qubits[qmpulse.pulse.qubit].threshold
+                iq_angle = qubits[qmpulse.pulse.qubit].iq_angle
+                qmpulse.declare_output(options, threshold, iq_angle)
+
+            with for_(n, 0, n < options.nshots, n + 1):
+                self.sweep_recursion(list(sweepers), qubits, qmsequence, options.relaxation_time)
+
+            with qua.stream_processing():
+                for qmpulse in qmsequence.ro_pulses:
+                    qmpulse.acquisition.download(*buffer_dims)
+
+        result = self.execute_program(experiment)
+        return self.fetch_results(result, qmsequence.ro_pulses)
```

### Comparing `qibolab-0.0.3/src/qibolab/instruments/qmsim.py` & `qibolab-0.0.4/src/qibolab/instruments/qmsim.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
             from qm.simulate.credentials import create_credentials
 
             self.manager = QuantumMachinesManager(host, int(port), credentials=create_credentials())
         else:
             self.manager = QuantumMachinesManager(host, int(port))
 
     @staticmethod
-    def fetch_results(result, ro_pulses, average, raw_adc=False):
+    def fetch_results(result, ro_pulses):
         return result
 
     def execute_program(self, program):
         ncontrollers = len(self.config.controllers)
 
         # for debugging only
         from qm import generate_qua_script
```

### Comparing `qibolab-0.0.3/src/qibolab/instruments/qutech.py` & `qibolab-0.0.4/src/qibolab/instruments/qutech.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/instruments/rfsoc.py` & `qibolab-0.0.4/src/qibolab/instruments/rfsoc.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,18 +8,19 @@
 import pickle
 import socket
 from dataclasses import dataclass
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 
+from qibolab import AcquisitionType, AveragingMode, ExecutionParameters
 from qibolab.instruments.abstract import AbstractInstrument
 from qibolab.platforms.abstract import Qubit
 from qibolab.pulses import PulseSequence, PulseType
-from qibolab.result import AveragedResults, ExecutionResults
+from qibolab.result import IntegratedResults, SampleResults
 from qibolab.sweeper import Parameter, Sweeper
 
 
 @dataclass
 class QickProgramConfig:
     sampling_rate: int = 9_830_400_000
     repetition_duration: int = 100_000
@@ -186,112 +187,126 @@
             raise results
         return results["i"], results["q"]
 
     def play(
         self,
         qubits: List[Qubit],
         sequence: PulseSequence,
-        relaxation_time: int = None,
-        nshots: int = None,
-        average: bool = False,
-        raw_adc: bool = False,
-    ) -> Dict[str, ExecutionResults]:
+        execution_parameters: ExecutionParameters,
+    ) -> Dict[str, Union[IntegratedResults, SampleResults]]:
         """Executes the sequence of instructions and retrieves readout results.
            Each readout pulse generates a separate acquisition.
            The relaxation_time and the number of shots have default values.
 
         Args:
             qubits (list): List of `qibolab.platforms.utils.Qubit` objects
                            passed from the platform.
-            sequence (`qibolab.pulses.PulseSequence`). Pulse sequence to play.
-            nshots (int): Number of repetitions (shots) of the experiment.
-            relaxation_time (int): Time to wait for the qubit to relax to its
-                                   ground state between shots in ns.
-            raw_adc (bool): allows to acquire raw adc data
+            execution_parameters (ExecutionParameters): Parameters (nshots,
+                                                        relaxation_time,
+                                                        fast_reset,
+                                                        acquisition_type,
+                                                        averaging_mode)
+            sequence (`qibolab.pulses.PulseSequence`): Pulse sequence to play.
         Returns:
             A dictionary mapping the readout pulses serial and respective qubits to
-            `qibolab.ExecutionResults` objects
+            qibolab results objects
         """
 
-        if raw_adc:
+        if execution_parameters.acquisition_type is AcquisitionType.RAW:
             raise NotImplementedError("Raw data acquisition is not supported")
-
+        if execution_parameters.fast_reset:
+            raise NotImplementedError("Fast reset is not supported")
         # if new value are passed, they are updated in the config obj
-        if nshots is not None:
-            self.cfg.reps = nshots
-        if relaxation_time is not None:
-            self.cfg.repetition_duration = relaxation_time
+        if execution_parameters.nshots is not None:
+            self.cfg.reps = execution_parameters.nshots
+        if execution_parameters.relaxation_time is not None:
+            self.cfg.repetition_duration = execution_parameters.relaxation_time
+
+        if execution_parameters.acquisition_type is AcquisitionType.DISCRIMINATION:
+            average = False
+        else:
+            average = execution_parameters.averaging_mode is AveragingMode.CYCLIC
 
         toti, totq = self._execute_pulse_sequence(self.cfg, sequence, qubits, len(sequence.ro_pulses), average)
 
         results = {}
         adcs = np.unique([qubits[p.qubit].feedback.ports[0][1] for p in sequence.ro_pulses])
         for j in range(len(adcs)):
             for i, ro_pulse in enumerate(sequence.ro_pulses):
                 i_pulse = np.array(toti[j][i])
                 q_pulse = np.array(totq[j][i])
 
                 serial = ro_pulse.serial
 
-                if average:
-                    results[ro_pulse.qubit] = results[serial] = AveragedResults.from_components(i_pulse, q_pulse)
+                if execution_parameters.acquisition_type is AcquisitionType.DISCRIMINATION:
+                    discriminated_shots = self.classify_shots(i_pulse, q_pulse, qubits[ro_pulse.qubit])
+                    if execution_parameters.averaging_mode is AveragingMode.CYCLIC:
+                        discriminated_shots = np.mean(discriminated_shots, axis=0)
+                    result = execution_parameters.results_type(discriminated_shots)
                 else:
-                    shots = self.classify_shots(i_pulse, q_pulse, qubits[ro_pulse.qubit])
-                    results[ro_pulse.qubit] = results[serial] = ExecutionResults.from_components(
-                        i_pulse, q_pulse, shots
-                    )
+                    result = execution_parameters.results_type(i_pulse + 1j * q_pulse)
+                results[ro_pulse.qubit] = results[serial] = result
 
         return results
 
     def classify_shots(self, i_values: List[float], q_values: List[float], qubit: Qubit) -> List[float]:
         """Classify IQ values using qubit threshold and rotation_angle if available in runcard"""
 
         if qubit.iq_angle is None or qubit.threshold is None:
             return None
         angle = qubit.iq_angle
         threshold = qubit.threshold
 
         rotated = np.cos(angle) * np.array(i_values) - np.sin(angle) * np.array(q_values)
         shots = np.heaviside(np.array(rotated) - threshold, 0)
+        if isinstance(shots, float):
+            return [shots]
         return shots
 
     def recursive_python_sweep(
         self,
         qubits: List[Qubit],
         sequence: PulseSequence,
         or_sequence: PulseSequence,
         *sweepers: Sweeper,
         average: bool,
-    ) -> Dict[str, Union[AveragedResults, ExecutionResults]]:
+        execution_parameters: ExecutionParameters,
+    ) -> Dict[str, Union[IntegratedResults, SampleResults]]:
         """Execute a sweep of an arbitrary number of Sweepers via recursion.
 
         Args:
             qubits (list): List of `qibolab.platforms.utils.Qubit` objects
                     passed from the platform.
             sequence (`qibolab.pulses.PulseSequence`): Pulse sequence to play.
                     This object is a deep copy of the original
                     sequence and gets modified.
             or_sequence (`qibolab.pulses.PulseSequence`): Reference to original
                     sequence to not modify.
             *sweepers (`qibolab.Sweeper`): Sweeper objects.
+            average (bool): if True averages on nshots
+            execution_parameters (ExecutionParameters): Parameters (nshots,
+                                                        relaxation_time,
+                                                        fast_reset,
+                                                        acquisition_type,
+                                                        averaging_mode)
         Returns:
             A dictionary mapping the readout pulses serial and respective qubits to
             results objects
         Raises:
             NotImplementedError: if a sweep refers to more than one pulse.
             NotImplementedError: if a sweep refers to a parameter different
                                  from frequency or amplitude.
         """
         # gets a list containing the original sequence output serials
         original_ro = [ro.serial for ro in or_sequence.ro_pulses]
 
         # If there are no sweepers run ExecutePulseSequence acquisition.
         # Last layer for recursion.
         if len(sweepers) == 0:
-            res = self.play(qubits, sequence, average=average)
+            res = self.play(qubits, sequence, execution_parameters)
             newres = {}
             for idx, key in enumerate(res):
                 newres[original_ro[idx // 2]] = res[key]
             return newres
 
         # If sweepers are still in queue
         else:
@@ -306,41 +321,49 @@
 
             # if there is one sweeper supported by qick than use hardware sweep
             if len(sweepers) == 1 and not self.get_if_python_sweep(sequence, qubits, *sweepers):
                 toti, totq = self._execute_single_sweep(
                     self.cfg, sequence, qubits, sweepers[0], len(sequence.ro_pulses), average
                 )
                 # convert results
-                res = self.convert_sweep_results(sweepers[0], original_ro, sequence, qubits, toti, totq, average)
+                res = self.convert_sweep_results(
+                    sweepers[0], original_ro, sequence, qubits, toti, totq, execution_parameters
+                )
                 return res
 
             # if it's not possible to execute qick sweep re-call function
             else:
                 sweep_results = {}
                 idx_pulse = or_sequence.index(sweeper.pulses[0])
                 for val in sweeper.values:
                     if is_freq:
                         sequence[idx_pulse].frequency = val
                     elif is_amp:
                         sequence[idx_pulse].amplitude = val
-                    res = self.recursive_python_sweep(qubits, sequence, or_sequence, *sweepers[1:], average=average)
+                    res = self.recursive_python_sweep(
+                        qubits,
+                        sequence,
+                        or_sequence,
+                        *sweepers[1:],
+                        average=average,
+                        execution_parameters=execution_parameters,
+                    )
                     # merge the dictionary obtained with the one already saved
                     sweep_results = self.merge_sweep_results(sweep_results, res)
 
         return sweep_results
 
     @staticmethod
     def merge_sweep_results(
-        dict_a: Dict[str, Union[AveragedResults, ExecutionResults]],
-        dict_b: Dict[str, Union[AveragedResults, ExecutionResults]],
-    ) -> Dict[str, Union[AveragedResults, ExecutionResults]]:
+        dict_a: Dict[str, Union[IntegratedResults, SampleResults]],
+        dict_b: Dict[str, Union[IntegratedResults, SampleResults]],
+    ) -> Dict[str, Union[IntegratedResults, SampleResults]]:
         """Merge two dictionary mapping pulse serial to Results object.
         If dict_b has a key (serial) that dict_a does not have, simply add it,
-        otherwise sum the two results (`qibolab.result.ExecutionResults`
-        or `qibolab.result.AveragedResults`)
+        otherwise sum the two results
 
         Args:
             dict_a (dict): dict mapping ro pulses serial to qibolab res objects
             dict_b (dict): dict mapping ro pulses serial to qibolab res objects
         Returns:
             A dict mapping the readout pulses serial to qibolab results objects
         """
@@ -398,98 +421,121 @@
         self,
         sweeper: Sweeper,
         original_ro: List[str],
         sequence: PulseSequence,
         qubits: List[Qubit],
         toti: List[float],
         totq: List[float],
-        average: bool,
-    ) -> Dict[str, Union[ExecutionResults, AveragedResults]]:
+        execution_parameters: ExecutionParameters,
+    ) -> Dict[str, Union[IntegratedResults, SampleResults]]:
         """Convert sweep res to qibolab dict res
 
         Args:
             *sweepers (`qibolab.Sweeper`): Sweeper objects.
             original_ro (list): list of ro serials of the original sequence
             sequence (`qibolab.pulses.PulseSequence`). Pulse sequence to play.
             qubits (list): List of `qibolab.platforms.utils.Qubit` objects
                  passed from the platform.
             toti (list): i values
             totq (list): q values
-            average (bool): true if the result is from averaged acquisition
+            results_type: qibolab results object
+            execution_parameters (ExecutionParameters): Parameters (nshots,
+                                                        relaxation_time,
+                                                        fast_reset,
+                                                        acquisition_type,
+                                                        averaging_mode)
         Returns:
             A dict mapping the readout pulses serial to qibolab results objects
         """
-        sweep_results = {}
+        results = {}
 
         adcs = np.unique([qubits[p.qubit].feedback.ports[0][1] for p in sequence.ro_pulses])
         for k in range(len(adcs)):
-            for j in range(len(sweeper.values)):
-                results = {}
-                # add a result for every readouts pulse
-                for i, serial in enumerate(original_ro):
-                    i_pulse = np.array(toti[k][i][j])
-                    q_pulse = np.array(totq[k][i][j])
-
-                    if average:
-                        results[sequence.ro_pulses[i].qubit] = results[serial] = AveragedResults.from_components(
-                            i_pulse, q_pulse
-                        )
-                    else:
-                        qubit = qubits[sequence.ro_pulses[i].qubit]
-                        shots = self.classify_shots(i_pulse, q_pulse, qubit)
-                        results[sequence.ro_pulses[i].qubit] = results[serial] = ExecutionResults.from_components(
-                            i_pulse, q_pulse, shots
-                        )
-                # merge new result with already saved ones
-                sweep_results = self.merge_sweep_results(sweep_results, results)
-        return sweep_results
+            for i, serial in enumerate(original_ro):
+                i_pulse = np.array(toti[k][i])
+                q_pulse = np.array(totq[k][i])
+
+                i_vals = i_pulse
+                q_vals = q_pulse
+
+                if execution_parameters.acquisition_type is AcquisitionType.DISCRIMINATION:
+                    average = False
+                else:
+                    average = execution_parameters.averaging_mode is AveragingMode.CYCLIC
+
+                if not average:
+                    shape = i_vals.shape
+                    i_vals = np.reshape(i_vals, (self.cfg.reps, *shape[:-1]))
+                    q_vals = np.reshape(q_vals, (self.cfg.reps, *shape[:-1]))
+
+                if execution_parameters.acquisition_type is AcquisitionType.DISCRIMINATION:
+                    qubit = qubits[sequence.ro_pulses[i].qubit]
+                    discriminated_shots = self.classify_shots(i_vals, q_vals, qubit)
+                    if execution_parameters.averaging_mode is AveragingMode.CYCLIC:
+                        discriminated_shots = np.mean(discriminated_shots, axis=0)
+                    result = execution_parameters.results_type(discriminated_shots)
+                else:
+                    result = execution_parameters.results_type(i_vals + 1j * q_vals)
+
+                results[sequence.ro_pulses[i].qubit] = results[serial] = result
+        return results
 
     def sweep(
         self,
         qubits: List[Qubit],
         sequence: PulseSequence,
+        execution_parameters: ExecutionParameters,
         *sweepers: Sweeper,
-        relaxation_time: int,
-        nshots: int = 1000,
-        average: bool = True,
-    ) -> Dict[str, Union[AveragedResults, ExecutionResults]]:
+    ) -> Dict[str, Union[IntegratedResults, SampleResults]]:
         """Executes the sweep and retrieves the readout results.
         Each readout pulse generates a separate acquisition.
         The relaxation_time and the number of shots have default values.
 
         Args:
             qubits (list): List of `qibolab.platforms.utils.Qubit` objects
                            passed from the platform.
+            execution_parameters (ExecutionParameters): Parameters (nshots,
+                                                        relaxation_time,
+                                                        fast_reset,
+                                                        acquisition_type,
+                                                        averaging_mode)
             sequence (`qibolab.pulses.PulseSequence`). Pulse sequence to play.
             *sweepers (`qibolab.Sweeper`): Sweeper objects.
-            relaxation_time (int): Time to wait for the qubit to relax to its
-                                   ground state between shots in ns.
-            nshots (int): Number of repetitions (shots) of the experiment.
-            average (bool): if False returns single shot measurements
         Returns:
             A dictionary mapping the readout pulses serial and respective qubits to
             results objects
         """
 
+        if execution_parameters.acquisition_type is AcquisitionType.RAW:
+            raise NotImplementedError("Raw data acquisition is not supported")
+        if execution_parameters.fast_reset:
+            raise NotImplementedError("Fast reset is not supported")
         # if new value are passed, they are updated in the config obj
-        if nshots is not None:
-            self.cfg.reps = nshots
-        if relaxation_time is not None:
-            self.cfg.repetition_duration = relaxation_time
+        if execution_parameters.nshots is not None:
+            self.cfg.reps = execution_parameters.nshots
+        if execution_parameters.relaxation_time is not None:
+            self.cfg.repetition_duration = execution_parameters.relaxation_time
+
+        if execution_parameters.acquisition_type is AcquisitionType.DISCRIMINATION:
+            average = False
+        else:
+            average = execution_parameters.averaging_mode is AveragingMode.CYCLIC
 
         # sweepers.values are modified to reflect actual sweeped values
         for sweeper in sweepers:
             if sweeper.parameter == Parameter.frequency:
                 sweeper.values += sweeper.pulses[0].frequency
             elif sweeper.parameter == Parameter.amplitude:
                 sweeper.values *= sweeper.pulses[0].amplitude
 
         sweepsequence = sequence.copy()
 
-        results = self.recursive_python_sweep(qubits, sweepsequence, sequence, *sweepers, average=average)
+        results = self.recursive_python_sweep(
+            qubits, sweepsequence, sequence, *sweepers, average=average, execution_parameters=execution_parameters
+        )
 
         # sweepers.values are converted back to original relative values
         for sweeper in sweepers:
             if sweeper.parameter == Parameter.frequency:
                 sweeper.values -= sweeper.pulses[0].frequency
             elif sweeper.parameter == Parameter.amplitude:
                 sweeper.values /= sweeper.pulses[0].amplitude
```

### Comparing `qibolab-0.0.3/src/qibolab/instruments/rohde_schwarz.py` & `qibolab-0.0.4/src/qibolab/instruments/rohde_schwarz.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/platforms/abstract.py` & `qibolab-0.0.4/src/qibolab/platforms/abstract.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 import math
 import re
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import Any, List, Optional
+from typing import Dict, List, Optional, Tuple, Union
 
-import numpy as np
+import networkx as nx
 import yaml
 from qibo import gates
 from qibo.config import log, raise_error
 from qibo.models import Circuit
 
 from qibolab.designs.channels import Channel
-from qibolab.pulses import FluxPulse, Pulse, PulseSequence, ReadoutPulse
-from qibolab.transpilers.gate_decompositions import TwoQubitNatives
+from qibolab.platforms.native import NativeType, SingleQubitNatives, TwoQubitNatives
+from qibolab.pulses import PulseSequence
+
+QubitId = Union[str, int]
+"""Type for qubit names."""
 
 
 @dataclass
 class Qubit:
     """Representation of a physical qubit.
 
     Qubit objects are instantiated by :class:`qibolab.platforms.platform.Platform`
@@ -33,15 +36,16 @@
         drive (:class:`qibolab.platforms.utils.Channel`): Channel used to
             send drive pulses to the qubit.
         flux (:class:`qibolab.platforms.utils.Channel`): Channel used to
             send flux pulses to the qubit.
         Other characterization parameters for the qubit, loaded from the runcard.
     """
 
-    name: str
+    name: QubitId
+
     bare_resonator_frequency: int = 0
     readout_frequency: int = 0  # this is the dressed frequency
     drive_frequency: int = 0
     sweetspot: float = 0
     peak_voltage: float = 0
     pi_pulse_amplitude: float = 0
     T1: int = 0
@@ -65,54 +69,79 @@
     mixer_readout_phi: float = 0.0
 
     readout: Optional[Channel] = None
     feedback: Optional[Channel] = None
     twpa: Optional[Channel] = None
     drive: Optional[Channel] = None
     flux: Optional[Channel] = None
+    flux_coupler: Optional[List["Qubit"]] = None
+
+    classifiers_hpars: dict = field(default_factory=dict)
+    native_gates: SingleQubitNatives = field(default_factory=SingleQubitNatives)
 
     def __post_init__(self):
         # register qubit in ``flux`` channel so that we can access
         # ``sweetspot`` and ``filters`` at the channel level
         if self.flux:
             self.flux.qubit = self
 
     @property
     def channels(self):
         for channel in [self.readout, self.feedback, self.drive, self.flux, self.twpa]:
             if channel is not None:
                 yield channel
 
 
+@dataclass
+class QubitPair:
+    """Data structure for holding the native two-qubit gates acting on a pair of qubits.
+
+    This is needed for symmetry to the single-qubit gates which are storred in the
+    :class:`qibolab.platforms.abstract.Qubit`.
+
+    Qubits are sorted according to ``qubit.name`` such that
+    ``qubit1.name < qubit2.name``.
+    """
+
+    qubit1: Qubit
+    qubit2: Qubit
+    native_gates: TwoQubitNatives = field(default_factory=TwoQubitNatives)
+
+
 class AbstractPlatform(ABC):
     """Abstract platform for controlling quantum devices.
 
     Args:
         name (str): name of the platform.
         runcard (str): path to the yaml file containing the platform setup.
     """
 
     def __init__(self, name, runcard):
         log.info(f"Loading platform {name} from runcard {runcard}")
         self.name = name
         self.runcard = runcard
 
-        self.qubits = {}
+        self.qubits: Dict[QubitId, Qubit] = {}
+        self.pairs: Dict[Tuple[QubitId, QubitId], QubitPair] = {}
 
         # Values for the following are set from the runcard in ``reload_settings``
         self.settings = None
         self.is_connected = False
+
         self.nqubits = None
         self.resonator_type = None
         self.topology = None
+
+        self.nshots = None
         self.relaxation_time = None
         self.sampling_rate = None
 
-        self.single_qubit_natives = {}
-        self.two_qubit_natives = TwoQubitNatives(0)
+        # TODO: Remove this (needed for the multiqubit platform)
+        self.native_gates = {}
+        self.two_qubit_native_types = NativeType(0)
         # Load platform settings
         self.reload_settings()
 
     def __repr__(self):
         return self.name
 
     def _check_connected(self):
@@ -131,36 +160,59 @@
 
         self.nqubits = settings["nqubits"]
         if "resonator_type" in self.settings:
             self.resonator_type = self.settings["resonator_type"]
         else:
             self.resonator_type = "3D" if self.nqubits == 1 else "2D"
 
-        self.topology = settings["topology"]
-
         self.relaxation_time = settings["settings"]["relaxation_time"]
+        self.nshots = settings["settings"]["nshots"]
         self.sampling_rate = settings["settings"]["sampling_rate"]
-
-        # Load native gates
         self.native_gates = settings["native_gates"]
-        self.single_qubit_natives = self.native_gates["single_qubit"]
-        if "two_qubit" in self.native_gates:
-            for gate in self.native_gates["two_qubit"].values():
-                self.two_qubit_natives |= TwoQubitNatives[list(gate)[0]]
-        else:
-            # dummy value to avoid transpiler failure for single qubit devices
-            self.two_qubit_natives = TwoQubitNatives.CZ
 
         # Load characterization settings and create ``Qubit`` and ``Channel`` objects
         for q in settings["qubits"]:
             if q in self.qubits:
                 for name, value in settings["characterization"]["single_qubit"][q].items():
                     setattr(self.qubits[q], name, value)
             else:
-                self.qubits[q] = Qubit(q, **settings["characterization"]["single_qubit"][q])
+                self.qubits[q] = qubit = Qubit(q, **settings["characterization"]["single_qubit"][q])
+                # register channels to qubits when we are using the old format
+                # needed for ``NativeGates`` to work
+                if "qubit_channel_map" in self.settings:
+                    ro, qd, qf, _ = self.settings["qubit_channel_map"][q]
+                    if ro is not None:
+                        qubit.readout = Channel(ro)
+                    if qd is not None:
+                        qubit.drive = Channel(qd)
+                    if qf is not None:
+                        qubit.flux = Channel(qf)
+                # register single qubit native gates to Qubit objects
+                if q in self.native_gates["single_qubit"]:
+                    qubit.native_gates = SingleQubitNatives.from_dict(qubit, self.native_gates["single_qubit"][q])
+
+        for pair in settings["topology"]:
+            pair = tuple(sorted(pair))
+            if pair not in self.pairs:
+                self.pairs[pair] = QubitPair(self.qubits[pair[0]], self.qubits[pair[1]])
+
+        # Load native two-qubit gates
+        if "two_qubit" in self.native_gates:
+            for pair, gatedict in self.native_gates["two_qubit"].items():
+                pair = tuple(sorted(int(q) if q.isdigit() else q for q in pair.split("-")))
+                self.pairs[pair].native_gates = TwoQubitNatives.from_dict(self.qubits, gatedict)
+                self.two_qubit_native_types |= self.pairs[pair].native_gates.types
+        else:
+            # dummy value to avoid transpiler failure for single qubit devices
+            self.two_qubit_native_types = NativeType.CZ
+
+        if self.topology is None:
+            self.topology = nx.Graph()
+            self.topology.add_nodes_from(self.qubits.keys())
+            self.topology.add_edges_from([(pair.qubit1.name, pair.qubit2.name) for pair in self.pairs.values()])
 
     def dump(self, path: Path):
         with open(path, "w") as file:
             yaml.dump(self.settings, file, sort_keys=False, indent=4, default_flow_style=None)
 
     def update(self, updates: dict):
         r"""Updates platform common runcard parameters after calibration actions.
@@ -192,72 +244,63 @@
         """
 
         for par, values in updates.items():
             for qubit, value in values.items():
                 # resonator_spectroscopy / resonator_spectroscopy_flux / resonator_punchout_attenuation
                 if par == "readout_frequency":
                     freq = int(value * 1e9)
-                    self.single_qubit_natives[qubit]["MZ"]["frequency"] = freq
                     self.settings["native_gates"]["single_qubit"][qubit]["MZ"]["frequency"] = freq
 
-                    if "if_frequency" in self.single_qubit_natives[qubit]["MZ"]:
-                        self.single_qubit_natives[qubit]["MZ"]["if_frequency"] = freq - self.get_lo_readout_frequency(
-                            qubit
-                        )
-                        self.settings["native_gates"]["single_qubit"][qubit]["MZ"][
-                            "if_frequency"
-                        ] = freq - self.get_lo_readout_frequency(qubit)
+                    mz = self.qubits[qubit].native_gates.MZ
+                    mz.frequency = freq
+                    if mz.if_frequency is not None:
+                        mz.if_frequency = freq - self.get_lo_readout_frequency(qubit)
+                        self.settings["native_gates"]["single_qubit"][qubit]["MZ"]["if_frequency"] = mz.if_frequency
 
                     self.qubits[qubit].readout_frequency = freq
                     self.settings["characterization"]["single_qubit"][qubit]["readout_frequency"] = freq
 
                 # resonator_punchout_attenuation
-                elif par == "readout_attenuation":
-                    # TODO: Are we going to save the attenuation somwhere in the native_gates or characterization
-                    # in all platforms?
-                    True
-
-                # resonator_punchout_attenuation
                 elif par == "bare_resonator_frequency":
                     freq = int(value * 1e9)
                     self.qubits[qubit].bare_resonator_frequency = freq
                     self.settings["characterization"]["single_qubit"][qubit]["bare_resonator_frequency"] = freq
 
                 # resonator_spectroscopy_flux / qubit_spectroscopy_flux
                 elif par == "sweetspot":
                     sweetspot = float(value)
                     self.qubits[qubit].sweetspot = sweetspot
                     self.settings["characterization"]["single_qubit"][qubit]["sweetspot"] = sweetspot
 
                 # qubit_spectroscopy / qubit_spectroscopy_flux / ramsey
                 elif par == "drive_frequency":
                     freq = int(value * 1e9)
-                    self.single_qubit_natives[qubit]["RX"]["frequency"] = freq
                     self.settings["native_gates"]["single_qubit"][qubit]["RX"]["frequency"] = freq
 
+                    self.qubits[qubit].native_gates.RX.frequency = freq
                     self.qubits[qubit].drive_frequency = freq
                     self.settings["characterization"]["single_qubit"][qubit]["drive_frequency"] = freq
 
                 elif "amplitude" in par:
                     amplitude = float(value)
                     # resonator_spectroscopy
                     if par == "readout_amplitude" and not math.isnan(amplitude):
-                        self.single_qubit_natives[qubit]["MZ"]["amplitude"] = amplitude
+                        self.qubits[qubit].native_gates.MZ.amplitude = amplitude
                         self.settings["native_gates"]["single_qubit"][qubit]["MZ"]["amplitude"] = amplitude
 
                     # rabi_amplitude / flipping
                     if par == "drive_amplitude" or par == "amplitudes":
-                        self.single_qubit_natives[qubit]["RX"]["amplitude"] = amplitude
+                        self.qubits[qubit].native_gates.RX.amplitude = amplitude
                         self.settings["native_gates"]["single_qubit"][qubit]["RX"]["amplitude"] = amplitude
                         self.settings["characterization"]["single_qubit"][qubit]["pi_pulse_amplitude"] = amplitude
 
                 # rabi_duration
                 elif par == "drive_length":
                     duration = int(value)
-                    self.single_qubit_natives[qubit]["RX"]["duration"] = duration
+                    self.qubits[qubit].native_gates.RX.duration = duration
                     self.settings["native_gates"]["single_qubit"][qubit]["RX"]["duration"] = duration
 
                 # ramsey
                 elif par == "t2":
                     t2 = float(value)
                     self.qubits[qubit].T2 = t2
                     self.settings["characterization"]["single_qubit"][qubit]["T2"] = t2
@@ -296,21 +339,27 @@
                 elif par == "mean_exc_states":
                     mean_exc_states = str(value)
                     self.qubits[qubit].mean_exc_states = mean_exc_states
                     self.settings["characterization"]["single_qubit"][qubit]["mean_exc_states"] = mean_exc_states
 
                 # drag pulse tunning
                 elif "beta" in par:
-                    shape = self.single_qubit_natives[qubit]["RX"]["shape"]
+                    rx = self.qubits[qubit].native_gates.RX
+                    shape = rx.shape
                     rel_sigma = re.findall(r"[\d]+[.\d]+|[\d]*[.][\d]+|[\d]+", shape)[0]
-                    self.single_qubit_natives[qubit]["RX"]["shape"] = f"Drag({rel_sigma}, {float(value)})"
-                    self.settings["native_gates"]["single_qubit"][qubit]["RX"][
-                        "shape"
-                    ] = f"Drag({rel_sigma}, {float(value)})"
+                    rx.shape = f"Drag({rel_sigma}, {float(value)})"
+                    self.settings["native_gates"]["single_qubit"][qubit]["RX"]["shape"] = rx.shape
 
+                elif "length" in par:  # assume only drive length
+                    self.qubits[qubit].native_gates.RX.duration = int(value)
+                elif par == "classifiers_hpars":
+                    self.qubits[qubit].classifiers_hpars = value
+                    self.settings["characterization"]["single_qubit"][qubit]["classifiers_hpars"] = value
+                elif par == "readout_attenuation":
+                    self.set_attenuation(qubit, value)
                 else:
                     raise_error(ValueError, f"Unknown parameter {par} for qubit {qubit}")
 
         # reload_settings after execute any calibration routine keeping fitted parameters
         self.reload_settings()
 
     @abstractmethod
@@ -329,107 +378,14 @@
     def stop(self):
         """Starts all the instruments."""
 
     @abstractmethod
     def disconnect(self):
         """Disconnects to instruments."""
 
-    def transpile(self, circuit: Circuit):
-        """Transforms a circuit to pulse sequence.
-
-        Args:
-            circuit (qibo.models.Circuit): Qibo circuit that respects the platform's
-                connectivity and native gates.
-
-        Returns:
-            sequence (qibolab.pulses.PulseSequence): Pulse sequence that implements the
-                circuit on the qubit.
-        """
-        sequence = PulseSequence()
-        virtual_z_phases = defaultdict(int)
-
-        # keep track of gates that were already added to avoid adding them twice
-        already_processed = set()
-        # process circuit gates
-        for moment in circuit.queue.moments:
-            moment_start = sequence.finish
-            for gate in moment:
-                if isinstance(gate, gates.I) or gate is None or gate in already_processed:
-                    pass
-
-                elif isinstance(gate, gates.Z):
-                    qubit = gate.target_qubits[0]
-                    virtual_z_phases[qubit] += np.pi
-
-                elif isinstance(gate, gates.RZ):
-                    qubit = gate.target_qubits[0]
-                    virtual_z_phases[qubit] += gate.parameters[0]
-
-                elif isinstance(gate, gates.U3):
-                    qubit = gate.target_qubits[0]
-                    # Transform gate to U3 and add pi/2-pulses
-                    theta, phi, lam = gate.parameters
-                    # apply RZ(lam)
-                    virtual_z_phases[qubit] += lam
-                    # Fetch pi/2 pulse from calibration
-                    RX90_pulse_1 = self.create_RX90_pulse(
-                        qubit,
-                        start=max(sequence.get_qubit_pulses(qubit).finish, moment_start),
-                        relative_phase=virtual_z_phases[qubit],
-                    )
-                    # apply RX(pi/2)
-                    sequence.add(RX90_pulse_1)
-                    # apply RZ(theta)
-                    virtual_z_phases[qubit] += theta
-                    # Fetch pi/2 pulse from calibration
-                    RX90_pulse_2 = self.create_RX90_pulse(
-                        qubit, start=RX90_pulse_1.finish, relative_phase=virtual_z_phases[qubit] - np.pi
-                    )
-                    # apply RX(-pi/2)
-                    sequence.add(RX90_pulse_2)
-                    # apply RZ(phi)
-                    virtual_z_phases[qubit] += phi
-
-                elif isinstance(gate, gates.M):
-                    # Add measurement pulse
-                    measurement_start = max(sequence.get_qubit_pulses(*gate.target_qubits).finish, moment_start)
-                    gate.pulses = ()
-                    for qubit in gate.target_qubits:
-                        MZ_pulse = self.create_MZ_pulse(qubit, start=measurement_start)
-                        sequence.add(MZ_pulse)
-                        gate.pulses = (*gate.pulses, MZ_pulse.serial)
-
-                elif isinstance(gate, gates.CZ):
-                    # create CZ pulse sequence with start time = 0
-                    cz_sequence, cz_virtual_z_phases = self.create_CZ_pulse_sequence(gate.qubits)
-
-                    # determine the right start time based on the availability of the qubits involved
-                    cz_qubits = {*cz_sequence.qubits, *gate.qubits}
-                    cz_start = max(sequence.get_qubit_pulses(*cz_qubits).finish, moment_start)
-
-                    # shift the pulses
-                    for pulse in cz_sequence.pulses:
-                        pulse.start += cz_start
-
-                    # add pulses to the sequence
-                    sequence.add(cz_sequence)
-
-                    # update z_phases registers
-                    for qubit in cz_virtual_z_phases:
-                        virtual_z_phases[qubit] += cz_virtual_z_phases[qubit]
-
-                else:  # pragma: no cover
-                    raise_error(
-                        NotImplementedError,
-                        f"Transpilation of {gate.__class__.__name__} gate has not been implemented yet.",
-                    )
-
-                already_processed.add(gate)
-        return sequence
-
     @abstractmethod
     def execute_pulse_sequence(self, sequence, nshots=1024, relaxation_time=None, raw_adc=False):
         """Executes a pulse sequence.
 
         Args:
             sequence (:class:`qibolab.pulses.PulseSequence`): Pulse sequence to execute.
             nshots (int): Number of shots to sample from the experiment. Default is 1024.
@@ -450,24 +406,26 @@
         Example:
             .. testcode::
 
                 import numpy as np
                 from qibolab.platform import Platform
                 from qibolab.sweeper import Sweeper, Parameter
                 from qibolab.pulses import PulseSequence
+                from qibolab import ExecutionParameters
 
 
                 platform = Platform("dummy")
                 sequence = PulseSequence()
                 parameter = Parameter.frequency
                 pulse = platform.create_qubit_readout_pulse(qubit=0, start=0)
                 sequence.add(pulse)
                 parameter_range = np.random.randint(10, size=10)
                 sweeper = Sweeper(parameter, parameter_range, [pulse])
-                platform.sweep(sequence, sweeper)
+                platform.sweep(sequence, ExecutionParameters(), sweeper)
+
 
 
         Args:
             sequence (:class:`qibolab.pulses.PulseSequence`): Pulse sequence to execute.
             sweepers (:class:`qibolab.sweeper.Sweeper`): Sweeper objects that specify which
                 parameters are being sweeped.
             nshots (int): Number of shots to sample from the experiment. Default is 1024.
@@ -476,134 +434,55 @@
             average (bool): If ``True`` the IQ results of individual shots are averaged on hardware.
 
         Returns:
             Readout results acquired by after execution.
         """
         raise_error(NotImplementedError, f"Platform {self.name} does not support sweeping.")
 
-    def get_qd_channel(self, qubit):
-        if self.qubits[qubit].drive:
-            return self.qubits[qubit].drive.name
-        else:
-            return self.settings["qubit_channel_map"][qubit][1]
-
     def create_RX90_pulse(self, qubit, start=0, relative_phase=0):
-        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
-        qd_duration = pulse_kwargs["duration"]
-        qd_frequency = pulse_kwargs["frequency"]
-        qd_amplitude = pulse_kwargs["amplitude"] / 2.0
-        qd_shape = pulse_kwargs["shape"]
-        qd_channel = self.get_qd_channel(qubit)
-        return Pulse(start, qd_duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
+        return self.qubits[qubit].native_gates.RX90.pulse(start, relative_phase)
 
     def create_RX_pulse(self, qubit, start=0, relative_phase=0):
-        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
-        qd_duration = pulse_kwargs["duration"]
-        qd_frequency = pulse_kwargs["frequency"]
-        qd_amplitude = pulse_kwargs["amplitude"]
-        qd_shape = pulse_kwargs["shape"]
-        qd_channel = self.get_qd_channel(qubit)
-        return Pulse(start, qd_duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
+        return self.qubits[qubit].native_gates.RX.pulse(start, relative_phase)
 
     def create_CZ_pulse_sequence(self, qubits, start=0):
         # Check in the settings if qubits[0]-qubits[1] is a key
-        if f"{qubits[0]}-{qubits[1]}" in self.settings["native_gates"]["two_qubit"]:
-            pulse_sequence_settings = self.settings["native_gates"]["two_qubit"][f"{qubits[0]}-{qubits[1]}"]["CZ"]
-        elif f"{qubits[1]}-{qubits[0]}" in self.settings["native_gates"]["two_qubit"]:
-            pulse_sequence_settings = self.settings["native_gates"]["two_qubit"][f"{qubits[1]}-{qubits[0]}"]["CZ"]
-        else:
+        pair = tuple(sorted(qubits))
+        if pair not in self.pairs or self.pairs[pair].native_gates.CZ is None:
             raise_error(
                 ValueError,
                 f"Calibration for CZ gate between qubits {qubits[0]} and {qubits[1]} not found.",
             )
-
-        # If settings contains only one pulse dictionary, convert it into a list that can be iterated below
-        if isinstance(pulse_sequence_settings, dict):
-            pulse_sequence_settings = [pulse_sequence_settings]
-
-        from qibolab.pulses import FluxPulse, PulseSequence
-
-        sequence = PulseSequence()
-        virtual_z_phases = defaultdict(int)
-
-        for pulse_settings in pulse_sequence_settings:
-            if pulse_settings["type"] == "qf":
-                qf_duration = pulse_settings["duration"]
-                qf_amplitude = pulse_settings["amplitude"]
-                qf_shape = pulse_settings["shape"]
-                qubit = pulse_settings["qubit"]
-                if self.qubits[qubit].flux:
-                    qf_channel = self.qubits[qubit].flux.name
-                else:
-                    qf_channel = self.settings["qubit_channel_map"][qubit][2]
-                sequence.add(
-                    FluxPulse(
-                        start + pulse_settings["relative_start"], qf_duration, qf_amplitude, qf_shape, qf_channel, qubit
-                    )
-                )
-            elif pulse_settings["type"] == "virtual_z":
-                virtual_z_phases[pulse_settings["qubit"]] += pulse_settings["phase"]
-            else:
-                raise NotImplementedError(
-                    "Implementation of CZ gates using pulses of types other than `qf` or `virtual_z` is not supported yet."
-                )
-
-        return sequence, virtual_z_phases
+        return self.pairs[pair].native_gates.CZ.sequence(start)
 
     def create_MZ_pulse(self, qubit, start):
-        pulse_kwargs = self.single_qubit_natives[qubit]["MZ"]
-        ro_duration = pulse_kwargs["duration"]
-        ro_frequency = pulse_kwargs["frequency"]
-        ro_amplitude = pulse_kwargs["amplitude"]
-        ro_shape = pulse_kwargs["shape"]
-        if self.qubits[qubit].readout:
-            ro_channel = self.qubits[qubit].readout.name
-        else:
-            ro_channel = self.settings["qubit_channel_map"][qubit][0]
-        return ReadoutPulse(start, ro_duration, ro_amplitude, ro_frequency, 0, ro_shape, ro_channel, qubit=qubit)
+        return self.qubits[qubit].native_gates.MZ.pulse(start)
 
     def create_qubit_drive_pulse(self, qubit, start, duration, relative_phase=0):
-        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
-        qd_frequency = pulse_kwargs["frequency"]
-        qd_amplitude = pulse_kwargs["amplitude"]
-        qd_shape = pulse_kwargs["shape"]
-        qd_channel = self.get_qd_channel(qubit)
-        return Pulse(start, duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
+        pulse = self.qubits[qubit].native_gates.RX.pulse(start, relative_phase)
+        pulse.duration = duration
+        return pulse
 
     def create_qubit_readout_pulse(self, qubit, start):
         return self.create_MZ_pulse(qubit, start)
 
     # TODO Remove RX90_drag_pulse and RX_drag_pulse, replace them with create_qubit_drive_pulse
     # TODO Add RY90 and RY pulses
 
     def create_RX90_drag_pulse(self, qubit, start, relative_phase=0, beta=None):
-        # create RX pi/2 pulse with drag shape
-        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
-        qd_duration = pulse_kwargs["duration"]
-        qd_frequency = pulse_kwargs["frequency"]
-        qd_amplitude = pulse_kwargs["amplitude"] / 2.0
-        qd_shape = pulse_kwargs["shape"]
-        if beta != None:
-            qd_shape = "Drag(5," + str(beta) + ")"
-
-        qd_channel = self.get_qd_channel(qubit)
-        return Pulse(start, qd_duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
+        pulse = self.qubits[qubit].native_gates.RX90.pulse(start, relative_phase)
+        if beta is not None:
+            pulse.shape = "Drag(5," + str(beta) + ")"
+        return pulse
 
     def create_RX_drag_pulse(self, qubit, start, relative_phase=0, beta=None):
-        # create RX pi pulse with drag shape
-        pulse_kwargs = self.single_qubit_natives[qubit]["RX"]
-        qd_duration = pulse_kwargs["duration"]
-        qd_frequency = pulse_kwargs["frequency"]
-        qd_amplitude = pulse_kwargs["amplitude"]
-        qd_shape = pulse_kwargs["shape"]
-        if beta != None:
-            qd_shape = "Drag(5," + str(beta) + ")"
-
-        qd_channel = self.get_qd_channel(qubit)
-        return Pulse(start, qd_duration, qd_amplitude, qd_frequency, relative_phase, qd_shape, qd_channel, qubit=qubit)
+        pulse = self.qubits[qubit].native_gates.RX.pulse(start, relative_phase)
+        if beta is not None:
+            pulse.shape = "Drag(5," + str(beta) + ")"
+        return pulse
 
     @abstractmethod
     def set_lo_drive_frequency(self, qubit, freq):
         """Set frequency of the qubit drive local oscillator.
 
         Args:
             qubit (int): qubit whose local oscillator will be modified.
```

### Comparing `qibolab-0.0.3/src/qibolab/platforms/icplatform.py` & `qibolab-0.0.4/src/qibolab/platforms/icplatform.py`

 * *Files 0% similar despite different names*

```diff
@@ -89,15 +89,15 @@
             after execution.
         """
         if not self.is_connected:
             from qibo.config import raise_error
 
             raise_error(RuntimeError, "Execution failed because instruments are not connected.")
         if nshots is None:
-            nshots = self.hardware_avg
+            nshots = self.nshots
 
         from qibolab.pulses import ReadoutPulse
 
         qubits_to_measure = []
         measurement_results = []
         pulse_mapping = {}
         seq_serial = {}
```

### Comparing `qibolab-0.0.3/src/qibolab/platforms/multiqubit.py` & `qibolab-0.0.4/src/qibolab/platforms/multiqubit.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 import yaml
 from qibo.config import log, raise_error
 
 from qibolab.platforms.abstract import AbstractPlatform, Qubit
 from qibolab.pulses import PulseSequence, PulseType
-from qibolab.result import ExecutionResults
+from qibolab.result import IntegratedResults
 from qibolab.sweeper import Parameter
 
 
 class MultiqubitPlatform(AbstractPlatform):
     def __init__(self, name, runcard):
         super().__init__(name, runcard)
         self.instruments = {}
@@ -39,15 +39,15 @@
                         if channel in self.qubit_channel_map[qubit]:
                             self.qubit_instrument_map[qubit][self.qubit_channel_map[qubit].index(channel)] = name
 
     def reload_settings(self):
         super().reload_settings()
         self.characterization = self.settings["characterization"]
         self.qubit_channel_map = self.settings["qubit_channel_map"]
-        self.hardware_avg = self.settings["settings"]["hardware_avg"]
+        self.nshots = self.settings["settings"]["nshots"]
         self.relaxation_time = self.settings["settings"]["relaxation_time"]
 
         # FIX: Set attenuation again to the original value after sweep attenuation in punchout
         if hasattr(self, "qubit_instrument_map"):
             for qubit in range(self.nqubits):
                 instrument_name = self.qubit_instrument_map[qubit][0]
                 port = self.qrm[qubit].channel_port_map[self.qubit_channel_map[qubit][0]]
@@ -88,15 +88,15 @@
                 # qubit_spectroscopy / qubit_spectroscopy_flux / ramsey
                 if par == "drive_frequency":
                     freq = int(value * 1e9)
 
                     # update Qblox qubit LO drive frequency config
                     instrument_name = self.qubit_instrument_map[qubit][1]
                     port = self.qdm[qubit].channel_port_map[self.qubit_channel_map[qubit][1]]
-                    drive_if = self.single_qubit_natives[qubit]["RX"]["if_frequency"]
+                    drive_if = self.qubits[qubit].native_gates.RX.if_frequency
                     self.settings["instruments"][instrument_name]["settings"]["ports"][port]["lo_frequency"] = (
                         freq - drive_if
                     )
 
                     # set Qblox qubit LO drive frequency
                     self.qd_port[qubit].lo_frequency = freq - drive_if
 
@@ -167,28 +167,28 @@
 
     def get_lo_twpa_power(self, qubit):
         for instrument in self.instruments:
             if "twpa" in instrument:
                 return self.instruments[instrument].power
         raise_error(NotImplementedError, "No twpa instrument found in the platform. ")
 
-    def set_attenuation(self, qubit: Qubit, att):
-        self.ro_port[qubit.name].attenuation = att
+    def set_attenuation(self, qubit, att):
+        self.ro_port[qubit].attenuation = att
 
     def set_gain(self, qubit, gain):
         self.qd_port[qubit].gain = gain
 
     def set_bias(self, qubit: Qubit, bias):
         if qubit.name in self.qbm:
             self.qb_port[qubit.name].current = bias
         elif qubit.name in self.qfm:
             self.qf_port[qubit.name].offset = bias
 
-    def get_attenuation(self, qubit: Qubit):
-        return self.ro_port[qubit.name].attenuation
+    def get_attenuation(self, qubit):
+        return self.ro_port[qubit].attenuation
 
     def get_bias(self, qubit: Qubit):
         if qubit.name in self.qbm:
             return self.qb_port[qubit.name].current
         elif qubit.name in self.qfm:
             return self.qf_port[qubit.name].offset
 
@@ -277,15 +277,15 @@
                 self.instruments[name].disconnect()
             self.is_connected = False
 
     def execute_pulse_sequence(self, sequence: PulseSequence, nshots=None):
         if not self.is_connected:
             raise_error(RuntimeError, "Execution failed because instruments are not connected.")
         if nshots is None:
-            nshots = self.hardware_avg
+            nshots = self.nshots
 
         instrument_pulses = {}
         changed = {}
 
         readout_instruments = [
             self.instruments[instrument]
             for instrument in self.instruments
@@ -331,17 +331,15 @@
                     else:
                         acquisition_results[key] = value
 
         data = {}
         for serial in acquisition_results:
             for if_pulse, original in changed.items():
                 if serial == if_pulse.serial:
-                    data[original] = data[if_pulse.qubit] = ExecutionResults.from_components(
-                        *acquisition_results[serial]
-                    )
+                    data[original] = data[if_pulse.qubit] = IntegratedResults(acquisition_results[serial])
 
         return data
 
     def sweep(self, sequence, *sweepers, nshots=1024, average=True, relaxation_time=None):
         results = {}
         sweeper_pulses = {}
         # create copy of the sequence
@@ -430,15 +428,15 @@
             pulses = sweeper_pulses[sweeper.parameter]
             for pulse in pulses:
                 original_value[pulse] = getattr(pulses[pulse], sweeper.parameter.name)
 
         if sweeper.qubits is not None:
             for qubit in sweeper.qubits:
                 if sweeper.parameter is Parameter.attenuation:
-                    original_value[qubit.name] = self.get_attenuation(qubit)
+                    original_value[qubit.name] = self.get_attenuation(qubit.name)
                 elif sweeper.parameter is Parameter.gain:
                     original_value[qubit.name] = self.get_gain(qubit)
                 elif sweeper.parameter is Parameter.bias:
                     original_value[qubit.name] = self.get_bias(qubit)
 
         return original_value
 
@@ -448,15 +446,15 @@
             pulses = sweeper_pulses[sweeper.parameter]
             for pulse in pulses:
                 setattr(pulses[pulse], sweeper.parameter.name, original_value[pulse])
 
         if sweeper.qubits is not None:
             for qubit in sweeper.qubits:
                 if sweeper.parameter is Parameter.attenuation:
-                    self.set_attenuation(qubit, original_value[qubit.name])
+                    self.set_attenuation(qubit.name, original_value[qubit.name])
                 elif sweeper.parameter is Parameter.gain:
                     self.set_gain(qubit, original_value[qubit.name])
                 elif sweeper.parameter is Parameter.bias:
                     self.set_bias(qubit, original_value[qubit.name])
 
     def _update_pulse_sequence_parameters(
         self, sweeper, sweeper_pulses, original_sequence, map_original_shifted, value
@@ -484,15 +482,15 @@
                     ]
                     if to_modify:
                         map_original_shifted[to_modify[0]] = pulses[pulse].serial
 
         if sweeper.qubits is not None:
             for qubit in sweeper.qubits:
                 if sweeper.parameter is Parameter.attenuation:
-                    self.set_attenuation(qubit, value)
+                    self.set_attenuation(qubit.name, value)
                 elif sweeper.parameter is Parameter.gain:
                     self.set_gain(qubit, value)
                 elif sweeper.parameter is Parameter.bias:
                     self.set_bias(qubit, value)
 
     def measure_fidelity(self, qubits=None, nshots=None):
         self.reload_settings()
```

### Comparing `qibolab-0.0.3/src/qibolab/pulses.py` & `qibolab-0.0.4/src/qibolab/pulses.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     FLUX pulses are used to shift the frequency of flux tunable qubits and with it implement
         two-qubit gates.
     """
 
     READOUT = "ro"
     DRIVE = "qd"
     FLUX = "qf"
+    FLUX_COUPLER = "cf"
 
 
 class Waveform:
     """A class to save pulse waveforms.
 
     A waveform is a list of samples, or discrete data points, used by the digital to analogue converters (DACs)
     to synthesise pulses.
@@ -1415,14 +1416,22 @@
             plt.savefig(savefig_filename)
         else:
             plt.show()
         plt.close()
         return
 
 
+class PulseConstructor(Enum):
+    """An enumeration to map each ``PulseType`` to the proper pulse constructor."""
+
+    READOUT = ReadoutPulse
+    DRIVE = DrivePulse
+    FLUX = FluxPulse
+
+
 class PulseSequence:
     """A collection of scheduled pulses.
 
     A quantum circuit can be translated into a set of scheduled pulses that implement the circuit gates.
     This class contains many supporting fuctions to facilitate the creation and manipulation of
     these collections of pulses.
     None of the methods of PulseSequence modify any of the properties of its pulses.
```

### Comparing `qibolab-0.0.3/src/qibolab/runcards/dummy.yml` & `qibolab-0.0.4/src/qibolab/runcards/dummy.yml`

 * *Files 6% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 description: QuantWare 5-qubit device.
 
 qubits: [0, 1, 2, 3, 4]
 
 settings:
     sampling_rate: 1000000000
     relaxation_time: 0
+    nshots: 1024
 
 resonator_type: 2D
 
-topology: # qubit - qubit connections
--   [ 1, 0, 1, 0, 0, 0]
--   [ 0, 1, 1, 0, 0, 0]
--   [ 1, 1, 1, 1, 1, 0]
--   [ 0, 0, 1, 1, 0, 0]
--   [ 0, 0, 1, 0, 1, 0]
+topology: [[0, 2], [1, 2], [2, 3], [2, 4]]
 
 native_gates:
     single_qubit:
         0: # qubit number
             RX:
                 duration: 40
                 amplitude: 0.005
```

### Comparing `qibolab-0.0.3/src/qibolab/runcards/icarusq.yml` & `qibolab-0.0.4/src/qibolab/runcards/icarusq.yml`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/runcards/multiqubit_icarusq.yml` & `qibolab-0.0.4/src/qibolab/runcards/multiqubit_icarusq.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 nqubits: 1
 description: 1-qubit device controlled with the IcarusQ AWG system.
 
 settings:
-    hardware_avg: 1024
+    nshots: 1024
     sampling_rate: 1_000_000_000
     repetition_duration: 200_000
     minimum_delay_between_instructions: 0
 
 qubits: [0]
 
 topology: # qubit - qubit connections
```

### Comparing `qibolab-0.0.3/src/qibolab/runcards/multiqubit_icarusqfpga.yml` & `qibolab-0.0.4/src/qibolab/runcards/multiqubit_icarusqfpga.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 nqubits: 1
 description: 1-qubit device controlled with the IcarusQ AWG system.
 
 settings:
-    hardware_avg: 1024
+    nshots: 1024
     sampling_rate: 1_000_000_000
     repetition_duration: 200_000
     minimum_delay_between_instructions: 0
 
 qubits: [0]
 
 topology: # qubit - qubit connections
```

### Comparing `qibolab-0.0.3/src/qibolab/runcards/qili1q_os2.yml` & `qibolab-0.0.4/src/qibolab/runcards/qili1q_os2.yml`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 nqubits: 1
 description: 1-qubit device OS2 in XLD fridge, controlled with qblox cluster rf.
 
 settings:
-    hardware_avg: 1024
+    nshots: 1024
     relaxation_time: 200_000
     sampling_rate: 1_000_000_000
 
 qubits: [0]
 
 resonator_type: 3D
 
-topology: # qubit - qubit connections
--   [1]
+topology: []
 
 channels: ['L3-17_qd', 'L3-17_ro', 'L2-4', null]
 
 qubit_channel_map: # [ReadOut, QubitDrive, QubitFlux, QubitBias]
     0: ['L3-17_ro', 'L3-17_qd', null, null]
 
 instruments:
```

### Comparing `qibolab-0.0.3/src/qibolab/runcards/qw5q_gold.yml` & `qibolab-0.0.4/src/qibolab/runcards/qw5q_gold.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,20 @@
 nqubits: 5
 description: QuantWare 5-qubit device.
 
 qubits: [0, 1, 2, 3, 4, 5]
 
 settings:
+    nshots: 1024
     sampling_rate: 1000000000
     relaxation_time: 50_000
 
 resonator_type: 2D
 
-topology: # qubit - qubit connections
--   [ 1, 0, 1, 0, 0, 0]
--   [ 0, 1, 1, 0, 0, 0]
--   [ 1, 1, 1, 1, 1, 0]
--   [ 0, 0, 1, 1, 0, 0]
--   [ 0, 0, 1, 0, 1, 0]
--   [ 0, 0, 0, 0, 0, 1]
+topology: [[0, 2], [1, 2], [2, 3], [2, 4]]
 
 native_gates:
     single_qubit:
         0: # qubit number
             RX:
                 duration: 40
                 amplitude: 0.005
```

### Comparing `qibolab-0.0.3/src/qibolab/runcards/qw5q_gold_qblox.yml` & `qibolab-0.0.4/src/qibolab/runcards/qw5q_gold_qblox.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,20 @@
 nqubits: 5
 description: 5-qubit device at XLD fridge, controlled with qblox cluster rf.
 
 settings:
-    hardware_avg: 1024
+    nshots: 1024
     relaxation_time: 20_000
     sampling_rate: 1_000_000_000
 
 qubits: [0, 1, 2, 3, 4, 5]
 
 resonator_type: 2D
 
-topology: # qubit - qubit connections
--   [ 1, 0, 1, 0, 0, 0]
--   [ 0, 1, 1, 0, 0, 0]
--   [ 1, 1, 1, 1, 1, 0]
--   [ 0, 0, 1, 1, 0, 0]
--   [ 0, 0, 1, 0, 1, 0]
--   [ 0, 0, 0, 0, 0, 1]
+topology: [[0, 2], [1, 2], [2, 3], [2, 4]]
 
 # Drive:
 # L3-15:mod8-o1 q0
 # L3-11:mod3-o1 q1
 # L3-12:mod3-o2 q2
 # L3-13:mod4-o1 q3
 # L3-14:mod4-o2 q4
```

### Comparing `qibolab-0.0.3/src/qibolab/sweeper.py` & `qibolab-0.0.4/src/qibolab/sweeper.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 
 class Parameter(Enum):
     """Sweeping parameters."""
 
     frequency = auto()
     amplitude = auto()
+    duration = auto()
     relative_phase = auto()
     delay = auto()
 
     attenuation = auto()
     gain = auto()
     bias = auto()
 
@@ -32,24 +33,25 @@
     Example:
         .. testcode::
 
             import numpy as np
             from qibolab.platform import Platform
             from qibolab.sweeper import Sweeper, Parameter
             from qibolab.pulses import PulseSequence
+            from qibolab import ExecutionParameters
 
 
             platform = Platform("dummy")
             sequence = PulseSequence()
             parameter = Parameter.frequency
             pulse = platform.create_qubit_readout_pulse(qubit=0, start=0)
             sequence.add(pulse)
             parameter_range = np.random.randint(10, size=10)
             sweeper = Sweeper(parameter, parameter_range, [pulse])
-            platform.sweep(sequence, sweeper)
+            platform.sweep(sequence, ExecutionParameters(), sweeper)
 
     Args:
         parameter (`qibolab.sweeper.Parameter`): parameter to be swept, possible choices are frequency, attenuation, amplitude, current and gain.
         values (np.ndarray): sweep range. If the parameter is `frequency` the sweep will be a shift around the readout frequency
             in case of a `ReadoutPulse` or around the drive frequency for a generic `Pulse`. If the parameter is `amplitude` the range is
             normalized with the current amplitude of the pulse. For other parameters the sweep will be performed directly over the range specified.
         pulses (list) : list of `qibolab.pulses.Pulse` to be swept (optional).
```

### Comparing `qibolab-0.0.3/src/qibolab/symbolic.py` & `qibolab-0.0.4/src/qibolab/symbolic.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/transpilers/abstract.py` & `qibolab-0.0.4/src/qibolab/transpilers/abstract.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/transpilers/fusion.py` & `qibolab-0.0.4/src/qibolab/transpilers/fusion.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/transpilers/gate_decompositions.py` & `qibolab-0.0.4/src/qibolab/transpilers/gate_decompositions.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,24 @@
 from dataclasses import dataclass
-from enum import Flag, auto
 
 import numpy as np
 from qibo import gates
 from qibo.backends import NumpyBackend
 from qibo.config import log, raise_error
 
+from qibolab.platforms.native import NativeType
 from qibolab.transpilers.abstract import Transpiler
 from qibolab.transpilers.unitary_decompositions import (
     two_qubit_decomposition,
     u3_decomposition,
 )
 
 backend = NumpyBackend()
 
 
-class TwoQubitNatives(Flag):
-    """A class to define the two qubit native gates."""
-
-    CZ = auto()
-    iSWAP = auto()
-
-    @classmethod
-    def from_gate(cls, gate: gates.Gate):
-        try:
-            return getattr(cls, gate.__class__.__name__)
-        except AttributeError:
-            raise_error(ValueError, f"Gate {gate} cannot be used as native.")
-
-
 class GateDecompositions:
     """Abstract data structure that holds decompositions of gates."""
 
     def __init__(self):
         self.decompositions = {}
 
     def add(self, gate, decomposition):
@@ -59,15 +45,15 @@
         """Decompose a gate."""
         decomposition = self.decompositions[gate.__class__]
         if callable(decomposition):
             decomposition = decomposition(gate)
         return [g.on_qubits({i: q for i, q in enumerate(gate.qubits)}) for g in decomposition]
 
 
-def translate_gate(gate, native_gates: TwoQubitNatives):
+def translate_gate(gate, native_gates: NativeType):
     """Maps Qibo gates to a hardware native implementation.
 
     Args:
         gate (qibo.gates.abstract.Gate): gate to be decomposed.
         native_gates (list): List of two qubit native gates
             supported by the quantum hardware ("CZ" and/or "iSWAP").
 
@@ -76,15 +62,15 @@
     """
     if isinstance(gate, gates.M):
         return gate
 
     if len(gate.qubits) == 1:
         return onequbit_dec(gate)
 
-    if native_gates is TwoQubitNatives.CZ | TwoQubitNatives.iSWAP:
+    if native_gates is NativeType.CZ | NativeType.iSWAP:
         # Check for a special optimized decomposition.
         if gate.__class__ in opt_dec.decompositions:
             return opt_dec(gate)
         # Check if the gate has a CZ decomposition
         if not gate.__class__ in iswap_dec.decompositions:
             return cz_dec(gate)
         # Check the decomposition with less 2 qubit gates.
@@ -95,27 +81,27 @@
                 return iswap_dec(gate)
             # If equal check the decomposition with less 1 qubit gates.
             # This is never used for now but may be useful for future generalization
             elif cz_dec.count_1q(gate) < iswap_dec.count_1q(gate):  # pragma: no cover
                 return cz_dec(gate)
             else:  # pragma: no cover
                 return iswap_dec(gate)
-    elif native_gates is TwoQubitNatives.CZ:
+    elif native_gates is NativeType.CZ:
         return cz_dec(gate)
-    elif native_gates is TwoQubitNatives.iSWAP:
+    elif native_gates is NativeType.iSWAP:
         if gate.__class__ in iswap_dec.decompositions:
             return iswap_dec(gate)
         else:
             # First decompose into CZ
             cz_decomposed = cz_dec(gate)
             # Then CZ are decomposed into iSWAP
             iswap_decomposed = []
             for g in cz_decomposed:
                 # Need recursive function as gates.Unitary is not in iswap_dec
-                for g_translated in translate_gate(g, TwoQubitNatives.iSWAP):
+                for g_translated in translate_gate(g, NativeType.iSWAP):
                     iswap_decomposed.append(g_translated)
             return iswap_decomposed
     else:  # pragma: no cover
         raise_error(NotImplementedError, "Use only CZ and/or iSWAP as native gates")
 
 
 onequbit_dec = GateDecompositions()
@@ -384,15 +370,15 @@
         two_qubit_natives (list): List of two qubit native gates
             supported by the quantum hardware ("CZ" and/or "iSWAP").
 
     Returns:
         new (qibo.models.Circuit): Equivalent circuit with native gates.
     """
 
-    two_qubit_natives: TwoQubitNatives
+    two_qubit_natives: NativeType
     translate_single_qubit: bool = True
     verbose: bool = False
 
     def tlog(self, message):
         """Print messages only if ``verbose`` was set to ``True``."""
         # TODO: Move this in ``AbstractTranspiler``
         if self.verbose:
@@ -422,15 +408,15 @@
             if len(gate.qubits) == 1:
                 # TODO: Make setting single-qubit native gates more flexible
                 if not isinstance(gate, (gates.I, gates.Z, gates.RZ, gates.U3)):
                     self.tlog(f"{gate.name} is not a single qubit native gate.")
                     return False
 
             elif len(gate.qubits) == 2:
-                if not (TwoQubitNatives.from_gate(gate) in self.two_qubit_natives):
+                if not (NativeType.from_gate(gate) in self.two_qubit_natives):
                     self.tlog(f"{gate.name} is not a two qubit native gate.")
                     return False
 
             else:
                 self.tlog(f"{gate.name} acts on more than two qubits.")
                 return False
```

### Comparing `qibolab-0.0.3/src/qibolab/transpilers/general_connectivity.py` & `qibolab-0.0.4/src/qibolab/transpilers/general_connectivity.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/transpilers/pipeline.py` & `qibolab-0.0.4/src/qibolab/transpilers/pipeline.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/transpilers/star_connectivity.py` & `qibolab-0.0.4/src/qibolab/transpilers/star_connectivity.py`

 * *Files identical despite different names*

### Comparing `qibolab-0.0.3/src/qibolab/transpilers/unitary_decompositions.py` & `qibolab-0.0.4/src/qibolab/transpilers/unitary_decompositions.py`

 * *Files identical despite different names*

