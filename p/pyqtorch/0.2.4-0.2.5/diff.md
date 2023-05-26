# Comparing `tmp/pyqtorch-0.2.4.tar.gz` & `tmp/pyqtorch-0.2.5.tar.gz`

## Comparing `pyqtorch-0.2.4.tar` & `pyqtorch-0.2.5.tar`

### file list

```diff
@@ -1,76 +1,135 @@
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/README.md
--rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/mkdocs.yml
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/readthedocs.yml
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/setup.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.github/workflows/run-tests-and-mypy.yml
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/21836652c37a637f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/2602555962d0fc4c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/30645ad5f1f1dcfe
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/317d2f17a1075099
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/41d845d0f90a6417
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/617ac8c861e982f1
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/68cc7f39a1692629
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/71de32d0dc4ef210
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/7ab8961a5fd3e34a
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/7b50e93d7b401d37
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/7e9bc91eb0e4bec7
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/8446b77184378e13
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/8c22cf14dc3075f3
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/8f831c3208d022cd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/963472f7f566f99d
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/9b70b475da072d2b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/a3b4cbbb65fe8420
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/aaa2c54c6449792b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/af9c8e117f709f43
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/c73abac16d830acc
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/ce5cb2c96a07a572
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/ce5dade58b1ccd69
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/d49ef2d71d47c091
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/df86f5c8bc05afc4
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/e69f22aa2552f985
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/f6f6f60064e20f97
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.ruff_cache/content/f78c2e380fc669b7
--rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/QAOA.ipynb
--rw-r--r--   0        0        0   154586 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/fit_function.ipynb
--rw-r--r--   0        0        0    74094 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/getting_started.ipynb
--rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/index.ipynb
--rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/deprecated/QAOA.ipynb
--rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/deprecated/bench.py
--rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/deprecated/fit_function.ipynb
--rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/deprecated/ham_evol_comparison.ipynb
--rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/docs/deprecated/state_evolution.ipynb
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/__init__.py
--rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/ansatz.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/embedding.py
--rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/matrices.py
--rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/matrices_sparse.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/converters/__init__.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/converters/store_ops.py
--rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/converters/to_qiskit.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/core/__init__.py
--rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/core/batched_operation.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/core/circuit.py
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/core/measurement.py
--rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/core/operation.py
--rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/core/utils.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/modules/__init__.py
--rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/modules/circuit.py
--rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/modules/hamevo.py
--rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/modules/parametric.py
--rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/modules/primitive.py
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyqtorch/modules/utils.py
--rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/tests/conftest.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/tests/test_batched_operations.py
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/tests/test_converters.py
--rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/tests/test_module_hamevo.py
--rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/tests/test_modules.py
--rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/tests/test_operations.py
--rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/tests/test_operations_hamevo.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/LICENSE
--rw-r--r--   0        0        0     2634 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pyqtorch-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     2318 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/CONTRIBUTING.md
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/README.md
+-rw-r--r--   0        0        0     1555 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/mkdocs.yml
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/publish.sh
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/readthedocs.yml
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/setup.py
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.github/workflows/run-tests-and-mypy.yml
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/21836652c37a637f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/2602555962d0fc4c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/30645ad5f1f1dcfe
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/317d2f17a1075099
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/41d845d0f90a6417
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/617ac8c861e982f1
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/68cc7f39a1692629
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/71de32d0dc4ef210
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/7ab8961a5fd3e34a
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/7b50e93d7b401d37
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/7e9bc91eb0e4bec7
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/8446b77184378e13
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/8c22cf14dc3075f3
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/8f831c3208d022cd
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/963472f7f566f99d
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/9b70b475da072d2b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/a3b4cbbb65fe8420
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/aaa2c54c6449792b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/af9c8e117f709f43
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/c73abac16d830acc
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/ce5cb2c96a07a572
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/ce5dade58b1ccd69
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/d49ef2d71d47c091
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/df86f5c8bc05afc4
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/e69f22aa2552f985
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/f6f6f60064e20f97
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.ruff_cache/content/f78c2e380fc669b7
+-rw-r--r--   0        0        0    57645 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/QAOA.ipynb
+-rw-r--r--   0        0        0   154586 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/fit_function.ipynb
+-rw-r--r--   0        0        0    74094 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/getting_started.ipynb
+-rw-r--r--   0        0        0    14131 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/index.ipynb
+-rw-r--r--   0        0        0    46162 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/deprecated/QAOA.ipynb
+-rw-r--r--   0        0        0    19339 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/deprecated/bench.py
+-rw-r--r--   0        0        0    74042 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/deprecated/fit_function.ipynb
+-rw-r--r--   0        0        0   121176 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/deprecated/ham_evol_comparison.ipynb
+-rw-r--r--   0        0        0     6459 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/docs/deprecated/state_evolution.ipynb
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/__init__.py
+-rw-r--r--   0        0        0     3544 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/ansatz.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/embedding.py
+-rw-r--r--   0        0        0     3479 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/matrices.py
+-rw-r--r--   0        0        0     6255 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/matrices_sparse.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/converters/__init__.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/converters/store_ops.py
+-rw-r--r--   0        0        0     2701 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/converters/to_qiskit.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/core/__init__.py
+-rw-r--r--   0        0        0    24532 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/core/batched_operation.py
+-rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/core/circuit.py
+-rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/core/measurement.py
+-rw-r--r--   0        0        0    22213 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/core/operation.py
+-rw-r--r--   0        0        0     5940 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/core/utils.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/modules/__init__.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/modules/circuit.py
+-rw-r--r--   0        0        0     7686 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/modules/hamevo.py
+-rw-r--r--   0        0        0     7730 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/modules/parametric.py
+-rw-r--r--   0        0        0     3417 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/modules/primitive.py
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyqtorch/modules/utils.py
+-rw-r--r--   0        0        0    15118 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/404.html
+-rw-r--r--   0        0        0   618774 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/index.html
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/sitemap.xml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/sitemap.xml.gz
+-rw-r--r--   0        0        0   654874 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/QAOA/index.html
+-rw-r--r--   0        0        0     5657 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/_markdown_exec_ansi.css
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/_mkdocstrings.css
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/images/favicon.png
+-rw-r--r--   0        0        0   113489 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/bundle.b4d07000.min.js
+-rw-r--r--   0        0        0   954781 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/bundle.b4d07000.min.js.map
+-rw-r--r--   0        0        0    22878 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/tinyseg.js
+-rw-r--r--   0        0        0   677463 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/wordcut.js
+-rw-r--r--   0        0        0    17074 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.ar.min.js
+-rw-r--r--   0        0        0     4654 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.da.min.js
+-rw-r--r--   0        0        0     6119 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.de.min.js
+-rw-r--r--   0        0        0     6208 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.du.min.js
+-rw-r--r--   0        0        0    11499 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.es.min.js
+-rw-r--r--   0        0        0     9342 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.fi.min.js
+-rw-r--r--   0        0        0    10669 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.fr.min.js
+-rw-r--r--   0        0        0     3383 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.hi.min.js
+-rw-r--r--   0        0        0     9437 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.hu.min.js
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.hy.min.js
+-rw-r--r--   0        0        0    11232 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.it.min.js
+-rw-r--r--   0        0        0     2313 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.ja.min.js
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.jp.min.js
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.kn.min.js
+-rw-r--r--   0        0        0     7972 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.ko.min.js
+-rw-r--r--   0        0        0      817 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.multi.min.js
+-rw-r--r--   0        0        0     6026 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.nl.min.js
+-rw-r--r--   0        0        0     4754 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.no.min.js
+-rw-r--r--   0        0        0    10171 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.pt.min.js
+-rw-r--r--   0        0        0    10958 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.ro.min.js
+-rw-r--r--   0        0        0    10331 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.ru.min.js
+-rw-r--r--   0        0        0     4901 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.sa.min.js
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.stemmer.support.min.js
+-rw-r--r--   0        0        0     4523 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.sv.min.js
+-rw-r--r--   0        0        0     2406 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.ta.min.js
+-rw-r--r--   0        0        0     2330 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.te.min.js
+-rw-r--r--   0        0        0     1031 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.th.min.js
+-rw-r--r--   0        0        0    15009 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.tr.min.js
+-rw-r--r--   0        0        0      784 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.vi.min.js
+-rw-r--r--   0        0        0     2158 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/lunr/min/lunr.zh.min.js
+-rw-r--r--   0        0        0    38916 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/workers/search.208ed371.min.js
+-rw-r--r--   0        0        0   209901 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/javascripts/workers/search.208ed371.min.js.map
+-rw-r--r--   0        0        0   113455 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/stylesheets/main.85bb2934.min.css
+-rw-r--r--   0        0        0    38958 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/stylesheets/main.85bb2934.min.css.map
+-rw-r--r--   0        0        0    12227 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/stylesheets/palette.a6bdf11c.min.css
+-rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/assets/stylesheets/palette.a6bdf11c.min.css.map
+-rw-r--r--   0        0        0   645434 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/deprecated/QAOA/index.html
+-rw-r--r--   0        0        0   748442 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/deprecated/bench/index.html
+-rw-r--r--   0        0        0   673688 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/deprecated/fit_function/index.html
+-rw-r--r--   0        0        0   757086 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/deprecated/ham_evol_comparison/index.html
+-rw-r--r--   0        0        0   606372 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/deprecated/state_evolution/index.html
+-rw-r--r--   0        0        0   752067 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/fit_function/index.html
+-rw-r--r--   0        0        0   674916 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/getting_started/index.html
+-rw-r--r--   0        0        0   121228 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/site/search/search_index.json
+-rw-r--r--   0        0        0     3046 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/tests/conftest.py
+-rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/tests/test_batched_operations.py
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/tests/test_converters.py
+-rw-r--r--   0        0        0     5104 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/tests/test_module_hamevo.py
+-rw-r--r--   0        0        0     3281 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/tests/test_modules.py
+-rw-r--r--   0        0        0     4872 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/tests/test_operations.py
+-rw-r--r--   0        0        0     6496 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/tests/test_operations_hamevo.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/LICENSE
+-rw-r--r--   0        0        0     2685 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     1460 2020-02-02 00:00:00.000000 pyqtorch-0.2.5/PKG-INFO
```

### Comparing `pyqtorch-0.2.4/.pre-commit-config.yaml` & `pyqtorch-0.2.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/mkdocs.yml` & `pyqtorch-0.2.5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/.github/workflows/run-tests-and-mypy.yml` & `pyqtorch-0.2.5/.github/workflows/run-tests-and-mypy.yml`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/QAOA.ipynb` & `pyqtorch-0.2.5/docs/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/fit_function.ipynb` & `pyqtorch-0.2.5/docs/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/getting_started.ipynb` & `pyqtorch-0.2.5/docs/getting_started.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/index.ipynb` & `pyqtorch-0.2.5/docs/index.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/deprecated/QAOA.ipynb` & `pyqtorch-0.2.5/docs/deprecated/QAOA.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/deprecated/bench.py` & `pyqtorch-0.2.5/docs/deprecated/bench.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/deprecated/fit_function.ipynb` & `pyqtorch-0.2.5/docs/deprecated/fit_function.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/deprecated/ham_evol_comparison.ipynb` & `pyqtorch-0.2.5/docs/deprecated/ham_evol_comparison.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/docs/deprecated/state_evolution.ipynb` & `pyqtorch-0.2.5/docs/deprecated/state_evolution.ipynb`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/__init__.py` & `pyqtorch-0.2.5/pyqtorch/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/ansatz.py` & `pyqtorch-0.2.5/pyqtorch/ansatz.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/embedding.py` & `pyqtorch-0.2.5/pyqtorch/embedding.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/matrices.py` & `pyqtorch-0.2.5/pyqtorch/matrices.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/matrices_sparse.py` & `pyqtorch-0.2.5/pyqtorch/matrices_sparse.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/converters/store_ops.py` & `pyqtorch-0.2.5/pyqtorch/converters/store_ops.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/converters/to_qiskit.py` & `pyqtorch-0.2.5/pyqtorch/converters/to_qiskit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/core/__init__.py` & `pyqtorch-0.2.5/pyqtorch/core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/core/batched_operation.py` & `pyqtorch-0.2.5/pyqtorch/core/batched_operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/core/circuit.py` & `pyqtorch-0.2.5/pyqtorch/core/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/core/measurement.py` & `pyqtorch-0.2.5/pyqtorch/core/measurement.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/core/operation.py` & `pyqtorch-0.2.5/pyqtorch/core/operation.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/core/utils.py` & `pyqtorch-0.2.5/pyqtorch/core/utils.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/modules/circuit.py` & `pyqtorch-0.2.5/pyqtorch/modules/circuit.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/modules/hamevo.py` & `pyqtorch-0.2.5/pyqtorch/modules/hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/modules/parametric.py` & `pyqtorch-0.2.5/pyqtorch/modules/parametric.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyqtorch/modules/primitive.py` & `pyqtorch-0.2.5/pyqtorch/modules/primitive.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/tests/conftest.py` & `pyqtorch-0.2.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/tests/test_batched_operations.py` & `pyqtorch-0.2.5/tests/test_batched_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/tests/test_converters.py` & `pyqtorch-0.2.5/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/tests/test_module_hamevo.py` & `pyqtorch-0.2.5/tests/test_module_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/tests/test_modules.py` & `pyqtorch-0.2.5/tests/test_modules.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/tests/test_operations.py` & `pyqtorch-0.2.5/tests/test_operations.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/tests/test_operations_hamevo.py` & `pyqtorch-0.2.5/tests/test_operations_hamevo.py`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/LICENSE` & `pyqtorch-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqtorch-0.2.4/pyproject.toml` & `pyqtorch-0.2.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     { name = "Aleksander Wennersteen", email = "aleksander.wennersteen@pasqal.com" },
     { name = "Mario Dagrada", email = "mario.dagrada@pasqal.com" },
     { name = "Dominik Seitz", email = "dominik.seitz@pasqal.com" },
     { name = "Niklas Heim", email = "niklas.heim@pasqal.com" },
 ]
 requires-python = ">=3.8.1,<3.11"
 license = {text = "Proprietary"}
-version = "0.2.4"
+version = "0.2.5"
 classifiers=[
     "License :: Other/Proprietary License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
@@ -37,15 +37,15 @@
 [tool.hatch.envs.tests]
 features = [
   "dev",
   "converters",
 ]
 
 [tool.hatch.envs.tests.scripts]
-test = "pytest {args}"
+test = "pytest {args} && hatch -e docs run mkdocs build --clean --strict"
 
 [tool.hatch.envs.docs]
 dependencies = [
   "mkdocs",
   "mkdocs-material",
   "mkdocstrings",
   "mkdocstrings-python",
```

### Comparing `pyqtorch-0.2.4/PKG-INFO` & `pyqtorch-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyqtorch
-Version: 0.2.4
+Version: 0.2.5
 Summary: An efficient, large-scale emulator designed for quantum machine learning, seamlessly integrated with a PyTorch backend. Please refer to https://pyqtorch.readthedocs.io/en/latest/ for setup and usage info, along with the full documentation.
 Author-email: Slimane Thabet <slimane.thabet@pasqal.com>, Aleksander Wennersteen <aleksander.wennersteen@pasqal.com>, Mario Dagrada <mario.dagrada@pasqal.com>, Dominik Seitz <dominik.seitz@pasqal.com>, Niklas Heim <niklas.heim@pasqal.com>
 License: Proprietary
 License-File: LICENSE
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

