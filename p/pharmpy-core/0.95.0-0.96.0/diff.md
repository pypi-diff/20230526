# Comparing `tmp/pharmpy-core-0.95.0.tar.gz` & `tmp/pharmpy-core-0.96.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pharmpy-core-0.95.0.tar", last modified: Mon May 22 08:31:02 2023, max compression
+gzip compressed data, was "pharmpy-core-0.96.0.tar", last modified: Fri May 26 09:46:09 2023, max compression
```

## Comparing `pharmpy-core-0.95.0.tar` & `pharmpy-core-0.96.0.tar`

### file list

```diff
@@ -1,1185 +1,1195 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    45578 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/LICENSE.LESSER
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    47493 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/NONMEM.rst
--rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/Pharmpy_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/Pharmpy_logo_dark.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/_ext/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/_ext/pharmpy_snippet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/allometry.rst
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/amd.rst
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api_model.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api_modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/api_workflows.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/bootstrap.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/cdd.rst
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/citation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/cli.rst
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/code_of_conduct.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/contribute.rst
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/contributors.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/covsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/crossval.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/custom.css
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/data.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/design.rst
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/developers.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/estmethod.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/frem.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/getting_started.rst
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/iivsearch.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/images/Pharmpy_symbol.svg
--rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/images/tools.png
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/iovsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/linearize.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/model.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2968 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/modelfit.rst
--rw-r--r--   0 runner    (1001) docker     (123)    28177 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/modeling.rst
--rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/modelsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/nonmem_plugin.rst
--rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/pharmr_logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/plots.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/projects.rst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/psn_resmod.rst
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/psn_tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/qa.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/ruvsearch.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/scm.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/simeval.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/tools.rst
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/user_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/docs/using_r.rst
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.348744 pharmpy-core-0.95.0/src/pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    80455 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.352744 pharmpy-core-0.95.0/src/pharmpy/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/altair.py
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/rich.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/scipy.py
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/deps/sympy_printing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.352744 pharmpy-core-0.95.0/src/pharmpy/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/code_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/df.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.352744 pharmpy-core-0.95.0/src/pharmpy/internals/ds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/ds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/ds/ordered_set.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.352744 pharmpy-core-0.95.0/src/pharmpy/internals/expr/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/assumptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/eval.py
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/leaves.py
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/ode.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/parse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/subs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/expr/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/fn/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fn/signature.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fn/type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/cwd.py
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/fs/tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.320743 pharmpy-core-0.95.0/src/pharmpy/internals/graph/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/connected_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/inverse.py
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/reachability.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/immutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/math.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/module/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/module/lazy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/parse/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/ignored.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/missing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/prettyprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/parse/treeprint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/sequence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/sequence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/sequence/lcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.356744 pharmpy-core-0.95.0/src/pharmpy/internals/set/
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/set/partitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/set/subsets.py
--rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/internals/unicode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.360744 pharmpy-core-0.95.0/src/pharmpy/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    30729 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/datainfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.360744 pharmpy-core-0.95.0/src/pharmpy/model/distributions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/distributions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/distributions/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/distributions/symbolic.py
--rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)    18415 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    72906 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/model/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.364744 pharmpy-core-0.95.0/src/pharmpy/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     6460 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/block_rvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     6655 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/blq.py
--rw-r--r--   0 runner    (1001) docker     (123)    18497 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    49857 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    34265 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/eta_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/eta_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)    14677 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/evaluation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.368744 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/
--rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/moxo.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/moxo.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.tab
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.lst
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.phi
--rw-r--r--   0 runner    (1001) docker     (123)    45326 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)    19401 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/math.py
--rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)    70916 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/odes.py
--rw-r--r--   0 runner    (1001) docker     (123)    11770 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/plots.py
--rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/remove_iiv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/remove_iov.py
--rw-r--r--   0 runner    (1001) docker     (123)    25078 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/update_inits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/modeling/write_csv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.368744 pharmpy-core-0.95.0/src/pharmpy/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.368744 pharmpy-core-0.95.0/src/pharmpy/plugins/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/fcon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/fcon/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.368744 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/error_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/ini.py
--rw-r--r--   0 runner    (1001) docker     (123)    28145 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/model_block.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/name_mangle.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/sanity_checks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.376744 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22581 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/advan.py
--rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/detect.py
--rw-r--r--   0 runner    (1001) docker     (123)    14704 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/nmtran_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    28819 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/parsing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.380744 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    25142 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/code_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/data_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/etas_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.380744 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
--rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/omega_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/parsers.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/problem_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/raw_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/record.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/simulation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/sizes_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/table_record.py
--rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/theta_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    21224 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/results_file.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7135 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/run.py
--rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/table.py
--rw-r--r--   0 runner    (1001) docker     (123)    64435 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/update.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.380744 pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13589 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/plugins/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/reporting/altairplot.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/reporting/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/reporting/custom.css
--rwxr-xr-x   0 runner    (1001) docker     (123)     5634 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/reporting/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     8786 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/allometry/
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/allometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/allometry/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/amd/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/amd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/amd/funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/amd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16039 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/amd/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/cdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/cdd/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.384744 pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    19893 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/crossval/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/crossval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/crossval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6908 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/evaldesign/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/evaldesign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/evaldesign/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/frem/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/report.rst
--rw-r--r--   0 runner    (1001) docker     (123)    38454 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/frem/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/
--rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
--rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
--rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/funcs/summarize_individuals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.388744 pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/iovsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iovsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12303 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/iovsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/linearize/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/linearize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/linearize/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/linearize/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/parse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.392744 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/definition.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/transits.py
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/mfl/stringify.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/tool.py
--rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/psn_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/qa/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/qa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18713 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/qa/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    32362 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    16607 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/tool.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/scm/
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/scm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/scm/psn_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/scm/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.396745 pharmpy-core-0.95.0/src/pharmpy/tools/simeval/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/simeval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2742 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/simeval/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.404744 pharmpy-core-0.95.0/src/pharmpy/tools/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/simfit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/simfit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/tools/wrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/visualization.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.404744 pharmpy-core-0.95.0/src/pharmpy/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/args.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/call.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/context.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.408745 pharmpy-core-0.95.0/src/pharmpy/workflows/dispatchers/
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/dispatchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/dispatchers/local_dask.py
--rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/execute.py
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.408745 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    12168 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/optimize.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.408745 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/baseclass.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/local_directory.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/null_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/src/pharmpy/workflows/workflow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    47493 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    46762 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-22 08:24:01.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-22 08:31:02.000000 pharmpy-core-0.95.0/src/pharmpy_core.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/cli/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/tests/config/
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.412745 pharmpy-core-0.95.0/tests/deps/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/deps/test_deps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.416745 pharmpy-core-0.95.0/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      663 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_evaldesign.py
--rw-r--r--   0 runner    (1001) docker     (123)     4016 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_resume.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/integration/test_ruvsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.416745 pharmpy-core-0.95.0/tests/internals/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.416745 pharmpy-core-0.95.0/tests/internals/fs/
--rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/fs/test_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/fs/test_tmp.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.416745 pharmpy-core-0.95.0/tests/internals/module/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/module/test_lazy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/test_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/internals/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/lib.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.420745 pharmpy-core-0.95.0/tests/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_datainfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_estimation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_random_variables.py
--rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/model/test_statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.424745 pharmpy-core-0.95.0/tests/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_add_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_basic_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_block_rvs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4573 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_blq.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_compartments.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_data_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_estimation_steps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_eta_additions.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_eta_transformations.py
--rw-r--r--   0 runner    (1001) docker     (123)     4036 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_expressions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_has_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_help_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_lrt.py
--rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_metabolite.py
--rw-r--r--   0 runner    (1001) docker     (123)   100500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_modeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2950 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_parameter_sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_plots.py
--rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_remove_covariate_effect.py
--rw-r--r--   0 runner    (1001) docker     (123)     7257 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_tmdd.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/modeling/test_units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.428745 pharmpy-core-0.95.0/tests/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.428745 pharmpy-core-0.95.0/tests/nonmem/output/
--rw-r--r--   0 runner    (1001) docker     (123)    13661 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/output/test_nonmem_results_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.428745 pharmpy-core-0.95.0/tests/nonmem/records/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_abbreviated.py
--rw-r--r--   0 runner    (1001) docker     (123)    28301 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_estimation_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_etas.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_model_record.py
--rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_omega.py
--rw-r--r--   0 runner    (1001) docker     (123)     7703 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_option_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_sizes.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_subroutines.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/records/test_theta.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_advan.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_des.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_fcon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_input.py
--rw-r--r--   0 runner    (1001) docker     (123)     9966 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_modelfit_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    35087 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_nonmem_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_nonmem_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/nonmem/test_read.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.428745 pharmpy-core-0.95.0/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     2313 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/plugins/test_nlmixr.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/plugins/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/plugins/test_rxode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.432745 pharmpy-core-0.95.0/tests/testdata/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.432745 pharmpy-core-0.95.0/tests/testdata/frem/
--rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/frem/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.436745 pharmpy-core-0.95.0/tests/testdata/nonmem/
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/DDMODEL00000130
--rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.440745 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.440745 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.452745 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
--rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.456745 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/control_stream_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/est_step_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/failed_run.ext
--rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/no_header_error.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/no_header_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/rounding_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/run_interrupted.ext
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/run_interrupted.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.456745 pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/FCON
--rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/FDATA
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/file.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.456745 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/
--rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/
--rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/minimal.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.332744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.460745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.464745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
--rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
--rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
--rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
--rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.464745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.328744 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.472746 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
--rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
--rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
--rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
--rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
--rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
--rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
--rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
--rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
--rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.472746 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
--rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
--rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.476745 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/
--rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.476745 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
--rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
--rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
--rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.488746 pharmpy-core-0.95.0/tests/testdata/nonmem/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.mod
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.prn
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.lst
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.phi
--rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_log.csv
--rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pef.csv
--rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pef.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_conc.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_dvid.csv
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_dvid.mod
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.coi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.cov
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.lst
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.phi
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_abbr.mod
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_abbr_comments.mod
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_block.mod
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_etas.mod
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_nm750.mod
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_rate.dta
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.coi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.cor
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.cov
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.lst
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.phi
--rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.tab
--rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.xml
--rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.tab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.492746 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/
--rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.lst
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.lst
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.phi
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.lst
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.mod
--rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.phi
--rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/resmod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/scm_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/simeval_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.phi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.phi
--rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
--rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mytab
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/gofofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/localmin.logf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.496746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/meta.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.500746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.500746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.500746 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scmplus_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
--rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/sdtab1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.500746 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/pheno_data.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.332744 pharmpy-core-0.95.0/tests/testdata/psn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.504746 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data3.dta
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.512746 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
--rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/xv_result.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.516746 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/command.txt
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.516746 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/frem_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.524746 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
--rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
--rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/meta.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/proposal_density.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/command.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/
--rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
--rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
--rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
--rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
--rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
--rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/results_summary.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir1/
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir2/
--rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.528746 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.540746 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/
--rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.cor
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.cov
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.ext
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.phi
--rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
--rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
--rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
--rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
--rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
--rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
--rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/
--rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/allometry_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/amd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/bootstrap_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/cdd_results.json
--rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/covsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/estmethod_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/iivsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/iovsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/linearize_results.json
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/modelsearch_results.json
--rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/qa_results.json
--rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/ruvsearch_results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.332744 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.332744 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:26:00.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.548746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.552746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.552746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.552746 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
--rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.556747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.556747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.556747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.556747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.560747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.560747 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
--rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
--rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
--rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
--rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/results.csv
--rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/results.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/tests/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_allometry.py
--rw-r--r--   0 runner    (1001) docker     (123)     7560 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_amd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     7896 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_cdd.py
--rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_covsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_crossval.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_estmethod.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)    27775 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_frem.py
--rw-r--r--   0 runner    (1001) docker     (123)     7840 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_iivsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_iovsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_linearize.py
--rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_mfl.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_modelfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_modelsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8112 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_qa.py
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_rankfuncs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16975 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_runtool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4806 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_ruvsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_scm.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_simeval.py
--rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_start_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_summarize_individuals.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/tools/test_wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-22 08:31:02.568747 pharmpy-core-0.95.0/tests/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_call.py
--rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_execute.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_model_database.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_task.py
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_tool_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tests/workflows/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-22 08:22:32.000000 pharmpy-core-0.95.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.042861 pharmpy-core-0.96.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    45995 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    35196 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7652 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/LICENSE.LESSER
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    47910 2023-05-26 09:46:09.042861 pharmpy-core-0.96.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2933 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.942861 pharmpy-core-0.96.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10512 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/NONMEM.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    14367 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/Pharmpy_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/Pharmpy_logo_dark.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.942861 pharmpy-core-0.96.0/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (123)     7108 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/_ext/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/_ext/pharmpy_snippet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5230 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/allometry.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/amd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/api_model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/api_modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/api_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/api_workflows.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4317 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/bootstrap.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/cdd.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/citation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/code_of_conduct.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6059 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/contribute.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/contributors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10790 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/covsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/crossval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/custom.css
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/data.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/design.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/developers.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10499 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/estmethod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/frem.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/getting_started.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12790 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/iivsearch.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.942861 pharmpy-core-0.96.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5937 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/images/Pharmpy_symbol.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   179150 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/images/tools.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11603 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/iovsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/linearize.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/model.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/modelfit.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    28238 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/modeling.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    16031 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/modelsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4434 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/nonmem_plugin.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12416 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/pharmr_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/plots.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/projects.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/psn_resmod.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/psn_tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/qa.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/ruvsearch.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2697 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/scm.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/simeval.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    15103 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/tools.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/user_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/docs/using_r.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2406 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-26 09:46:09.046861 pharmpy-core-0.96.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3180 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.942861 pharmpy-core-0.96.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80648 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3593 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/deps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/deps/altair.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/deps/rich.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/deps/scipy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/deps/sympy_printing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/code_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      909 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/df.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/internals/ds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/ds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/ds/ordered_set.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/internals/expr/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/assumptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/eval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/leaves.py
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/ode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/subs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/expr/units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/internals/fn/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/fn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/fn/signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/fn/type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/fs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/fs/cwd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/fs/lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/fs/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/fs/tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.930861 pharmpy-core-0.96.0/src/pharmpy/internals/graph/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/internals/graph/directed/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/graph/directed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/graph/directed/connected_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/graph/directed/inverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/graph/directed/reachability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/immutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/math.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.946861 pharmpy-core-0.96.0/src/pharmpy/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/module/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/module/lazy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/internals/parse/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/parse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15783 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/parse/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3050 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/parse/ignored.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/parse/missing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2519 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/parse/prettyprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/parse/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4340 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/parse/treeprint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/internals/sequence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/sequence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2114 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/sequence/lcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/internals/set/
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/set/partitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/set/subsets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6365 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/internals/unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30729 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/datainfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/model/distributions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/distributions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/distributions/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19145 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/distributions/symbolic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14790 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/estimation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/model/external/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/model/external/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/fcon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2117 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/fcon/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10036 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/error_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/ini.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9061 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/model_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/name_mangle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10780 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/sanity_checks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.950861 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22581 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11551 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/detect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14131 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6712 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/nmtran_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28896 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/parsing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.954861 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/abbreviated_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25158 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/code_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/data_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/etas_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.954861 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/definitions.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/option_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/problem_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1397 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     1692 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17000 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/omega_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/problem_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/raw_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/simulation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/sizes_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/subroutine_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2803 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/table_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5335 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/theta_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11765 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64737 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/update.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.954861 pharmpy-core-0.96.0/src/pharmpy/model/external/rxode/
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7199 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/rxode/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/external/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21361 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13285 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34378 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8281 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72906 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/model/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.958861 pharmpy-core-0.96.0/src/pharmpy/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)    10619 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6536 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/block_rvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6721 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18481 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21363 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49871 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36044 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5087 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9043 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16283 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/eta_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7964 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/eta_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/evaluation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.958861 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    50310 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/moxo.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/moxo.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.tab
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14564 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    45278 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11217 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2671 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70916 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/odes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12116 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15780 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4939 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/remove_iiv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/remove_iov.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25760 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6314 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4920 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4242 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/update_inits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/modeling/write_csv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)    11165 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/reporting/altairplot.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/reporting/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/reporting/custom.css
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5634 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/reporting/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)     3744 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/allometry/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/allometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/allometry/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/amd/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/amd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4902 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/amd/funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/amd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16119 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/amd/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/bootstrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      540 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/bootstrap/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     8800 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/bootstrap/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/bootstrap/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/cdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8393 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/cdd/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4863 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/covsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/covsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/covsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19965 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/covsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/crossval/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/crossval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1449 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/crossval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/estmethod/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/estmethod/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5527 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/estmethod/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/estmethod/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/estmethod/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/evaldesign/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/evaldesign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/evaldesign/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/external/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/external/nlmixr/
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/nlmixr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19032 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/nlmixr/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      635 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21360 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18254 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/results_file.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7225 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.962861 pharmpy-core-0.96.0/src/pharmpy/tools/external/rxode/
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/rxode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6598 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/external/rxode/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/frem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/frem/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/frem/report.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    39039 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/frem/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/frem/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/funcs/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/funcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9605 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/funcs/ml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/funcs/ml_models/
+-rw-r--r--   0 runner    (1001) docker     (123)    91484 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)    93596 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite
+-rw-r--r--   0 runner    (1001) docker     (123)     9949 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/funcs/summarize_individuals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/iivsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/iivsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5147 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/iivsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9843 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/iivsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/iovsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/iovsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/iovsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/linearize/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/linearize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/linearize/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/linearize/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1405 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2619 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2166 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/parse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.966861 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/definition.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/absorption.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/covariate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/elimination.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/lagtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      444 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/peripherals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/symbols.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/transits.py
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/mfl/stringify.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/tools/modelfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/modelfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4086 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/modelfit/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/tools/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/modelsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11394 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/modelsearch/algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/modelsearch/tool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6174 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/psn_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/tools/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/qa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19639 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/qa/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33617 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/tools/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/ruvsearch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4507 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/ruvsearch/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16708 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/ruvsearch/tool.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/tools/scm/
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/scm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/scm/psn_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27585 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/scm/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/tools/simeval/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/simeval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/simeval/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/tools/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/simfit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/simfit/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/tools/wrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5676 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/visualization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/args.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/call.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/workflows/dispatchers/
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/dispatchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4460 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/dispatchers/local_dask.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/workflows/model_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/model_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9287 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/model_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12311 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/model_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/model_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/optimize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.970861 pharmpy-core-0.96.0/src/pharmpy/workflows/tool_database/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/tool_database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/tool_database/baseclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/tool_database/local_directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/tool_database/null_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5880 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/src/pharmpy/workflows/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/src/pharmpy_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    47910 2023-05-26 09:46:08.000000 pharmpy-core-0.96.0/src/pharmpy_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    47414 2023-05-26 09:46:08.000000 pharmpy-core-0.96.0/src/pharmpy_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:46:08.000000 pharmpy-core-0.96.0/src/pharmpy_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-26 09:46:08.000000 pharmpy-core-0.96.0/src/pharmpy_core.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 09:40:32.000000 pharmpy-core-0.96.0/src/pharmpy_core.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-26 09:46:08.000000 pharmpy-core-0.96.0/src/pharmpy_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-26 09:46:08.000000 pharmpy-core-0.96.0/src/pharmpy_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/cli/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/deps/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/deps/test_deps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/external/test_external.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/external/test_nlmixr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1721 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/external/test_rxode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_evaldesign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7463 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8845 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_resume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/integration/test_ruvsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/internals/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/internals/fs/
+-rw-r--r--   0 runner    (1001) docker     (123)    15348 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/internals/fs/test_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/internals/fs/test_tmp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/internals/module/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/internals/module/test_lazy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5505 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/internals/test_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/internals/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/lib.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.974861 pharmpy-core-0.96.0/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10091 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/model/test_datainfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5537 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/model/test_estimation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/model/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8855 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/model/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29709 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/model/test_random_variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15860 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/model/test_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.978861 pharmpy-core-0.96.0/tests/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_add_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4437 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_basic_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3861 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_block_rvs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_blq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_compartments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10292 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_data_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17022 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27570 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4447 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_estimation_steps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_eta_additions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_eta_transformations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20673 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_expressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_has_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_help_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_lrt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_metabolite.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100513 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_modeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_parameter_sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4968 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16483 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_remove_covariate_effect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7765 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_tmdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/modeling/test_units.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.978861 pharmpy-core-0.96.0/tests/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.978861 pharmpy-core-0.96.0/tests/nonmem/output/
+-rw-r--r--   0 runner    (1001) docker     (123)    13614 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/output/test_nonmem_results_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.982861 pharmpy-core-0.96.0/tests/nonmem/records/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_abbreviated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_estimation_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_etas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_model_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10795 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_omega.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7717 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_option_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_sizes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_subroutines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/records/test_theta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8486 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_advan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_des.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_fcon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_input.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8868 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_modelfit_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35139 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_nonmem_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3822 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_nonmem_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5595 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/nonmem/test_read.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.982861 pharmpy-core-0.96.0/tests/testdata/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.982861 pharmpy-core-0.96.0/tests/testdata/frem/
+-rw-r--r--   0 runner    (1001) docker     (123)    52275 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/frem/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.986861 pharmpy-core-0.96.0/tests/testdata/nonmem/
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/DDMODEL00000130
+-rw-r--r--   0 runner    (1001) docker     (123)    59142 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.986861 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.986861 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.990861 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21670 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21677 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21680 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22454 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    22067 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/skipped_individuals1.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.990861 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/control_stream_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    10369 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/est_step_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     9105 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/failed_run.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/failed_run.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    23702 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/no_header_error.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19648 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/no_header_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/rounding_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/run_interrupted.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/run_interrupted.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10316 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/errors/zero_gradient_error.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.990861 pharmpy-core-0.96.0/tests/testdata/nonmem/fcon/
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/fcon/FCON
+-rw-r--r--   0 runner    (1001) docker     (123)    39432 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/fcon/FDATA
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/file.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.934861 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.994861 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/
+-rw-r--r--   0 runner    (1001) docker     (123)    22896 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1277 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11250 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1623 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26246 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.994861 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/
+-rw-r--r--   0 runner    (1001) docker     (123)    24625 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4861 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    26183 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1599 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.934861 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.994861 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14234 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.994861 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9547 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/minimal.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.934861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.994861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17620 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.934861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/multPROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.934861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.994861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91887 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.934861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.934861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.994861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    36515 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16505 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13947 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    59168 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    37889 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov
+-rw-r--r--   0 runner    (1001) docker     (123)   115118 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    82511 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    75841 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.998861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.934861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.998861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)    15883 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    18122 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    15469 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    26695 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     8760 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17548 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6956 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13203 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14451 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     2492 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11801 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1393 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5460 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17299 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16143 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    14090 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    54699 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    19741 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    31702 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.998861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/
+-rw-r--r--   0 runner    (1001) docker     (123)   178666 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext
+-rw-r--r--   0 runner    (1001) docker     (123)  1091059 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.002861 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4152 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    38485 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    41718 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.002861 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_1transit.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_2transits.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan11.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan12.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      719 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    18812 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.006861 pharmpy-core-0.96.0/tests/testdata/nonmem/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/fviii6.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/fviii6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/fviii6.prn
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    19098 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    90456 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21336 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   175384 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_simulated_log.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   185992 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_simulated_normal.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)   105888 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pef.csv
+-rwxr-xr-x   0 runner    (1001) docker     (123)      189 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pef.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12218 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_advan3_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    10093 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_conc.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_dvid.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_dvid.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10527 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_trans1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10693 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_trans1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_trans1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_trans1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10540 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      470 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_abbr.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_abbr_comments.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_block.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_clashing_symbols.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_etas.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_nm750.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36053 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_rate.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.coi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    90151 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.tab
+-rw-r--r--   0 runner    (1001) docker     (123)    22114 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   298562 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    28308 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6933 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    17010 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.tab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.010861 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/
+-rw-r--r--   0 runner    (1001) docker     (123)   370034 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/add_etas_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/add_etas_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16579 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/add_etas_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/add_etas_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/boxcox.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14595 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/boxcox.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/boxcox.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/boxcox.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2824 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/fullblock.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17210 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/fullblock.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/fullblock.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/fullblock.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/iov.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12617 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/iov.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/iov.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    24133 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/iov.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   262826 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15014 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     3943 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/resmod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/scm_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   392990 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/simeval_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3262 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/tdist.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17544 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/tdist.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/tdist.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/qa/tdist.phi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.010861 pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mox3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13182 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mox3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      672 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mox3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12417 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mox3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   276902 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   180553 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mytab
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/backward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/backward_dir1/config_fake.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3068 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/gofofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10037 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     5383 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/localmin.logf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/backward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/backward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3813 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2723 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_pval_4.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir1/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    38957 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir2/config_havebaserun.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    20500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/meta.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/onlyforward_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/onlyforward_dir1/config_normal.scm
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/scmplus_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)   108031 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/sdtab1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.014861 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.cov
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1454 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17071 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    16730 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/pheno_data.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.938861 pharmpy-core-0.96.0/tests/testdata/psn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.018861 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13424 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/est_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/est_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13336 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/est_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    13843 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/est_data3.dta
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.022861 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    17040 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11625 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11637 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    11623 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    15116 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4615 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/pred_data0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/pred_data1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/pred_data2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     4196 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/pred_data3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/xv_result.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.022861 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/command.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/covariates_summary.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.022861 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14761 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13993 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    19440 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/frem_dataset.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/frem_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.026861 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9040 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6946 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    93135 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    16221 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.cor
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    21654 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    13826 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10472 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    14006 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/proposal_density.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.026861 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/command.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.026861 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/
+-rw-r--r--   0 runner    (1001) docker     (123)     5485 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.026861 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    12131 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi
+-rw-r--r--   0 runner    (1001) docker     (123)   137744 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table
+-rw-r--r--   0 runner    (1001) docker     (123)   316422 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      700 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    11536 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/results_summary.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.026861 pharmpy-core-0.96.0/tests/testdata/psn/resmod_dir1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/resmod_dir1/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.026861 pharmpy-core-0.96.0/tests/testdata/psn/resmod_dir2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11647 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/resmod_dir2/resmod_results.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.026861 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.030861 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/
+-rw-r--r--   0 runner    (1001) docker     (123)    63331 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.cor
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.cov
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.ext
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6973 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    54391 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    38720 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    14039 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    13972 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-5.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-6.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-7.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext
+-rw-r--r--   0 runner    (1001) docker     (123)     9500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-8.mod
+-rw-r--r--   0 runner    (1001) docker     (123)     6986 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    73024 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    36512 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta
+-rw-r--r--   0 runner    (1001) docker     (123)    21489 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.034861 pharmpy-core-0.96.0/tests/testdata/results/
+-rw-r--r--   0 runner    (1001) docker     (123)    24788 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/allometry_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    50648 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/amd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   130598 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/bootstrap_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12291 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/cdd_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1360720 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/covsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/estmethod_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   205797 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/iivsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)   197228 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/iovsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12639 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/linearize_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)   105603 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/modelsearch_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7841 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/qa_results.json
+-rw-r--r--   0 runner    (1001) docker     (123)    57352 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/ruvsearch_results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.938861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.034861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/metadata.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.034861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.034861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:08.938861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/.hash/-7907770233072098756/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   183701 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:41:55.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7120 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91188 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    12377 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1761 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91119 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.038861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    53630 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91754 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.042861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.042861 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/metadata.json
+-rw-r--r--   0 runner    (1001) docker     (123)    54979 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext
+-rw-r--r--   0 runner    (1001) docker     (123)    91879 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi
+-rw-r--r--   0 runner    (1001) docker     (123)    70155 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/nonmem.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stderr
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout
+-rw-r--r--   0 runner    (1001) docker     (123)    47403 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/results.csv
+-rw-r--r--   0 runner    (1001) docker     (123)   105597 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/results.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.042861 pharmpy-core-0.96.0/tests/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_allometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7559 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_amd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8607 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_cdd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3914 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_covsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_crossval.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_estmethod.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_frem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_iivsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_iovsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4328 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_linearize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11786 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_mfl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10258 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_modelsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10900 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_qa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_rankfuncs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15964 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_runtool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_ruvsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19845 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_scm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_simeval.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_start_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_summarize_individuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/tools/test_wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 09:46:09.042861 pharmpy-core-0.96.0/tests/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/workflows/test_call.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6586 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/workflows/test_execute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/workflows/test_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/workflows/test_model_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/workflows/test_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/workflows/test_tool_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4125 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tests/workflows/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-05-26 09:39:32.000000 pharmpy-core-0.96.0/tox.ini
```

### Comparing `pharmpy-core-0.95.0/AUTHORS.rst` & `pharmpy-core-0.96.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/CHANGELOG.rst` & `pharmpy-core-0.96.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,27 @@
+0.96.0 (2023-05-26)
+-------------------
+
+Changes
+=======
+
+* Rename functions handling the precision matrix (was previously referring to information matrix which was an error)
+* Remove saddle reset for default AMD model
+* Let LLQ column takes precedence over BLQ column
+
+New features
+============
+
+* Add tools.load_example_modelfit_results
+
+Bugfixes
+========
+
+* Fix bug where if-statements were reordered incorrectly
+
 0.95.0 (2023-05-22)
 -------------------
 
 Changes
 =======
 
 * ``ModelfitResults.ofv_iterations`` and ``ModelfitResults.parameter_estimates_iterations`` have NaN rows in failed runs
```

### Comparing `pharmpy-core-0.95.0/CODE_OF_CONDUCT.rst` & `pharmpy-core-0.96.0/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/LICENSE` & `pharmpy-core-0.96.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/LICENSE.LESSER` & `pharmpy-core-0.96.0/LICENSE.LESSER`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/MANIFEST.in` & `pharmpy-core-0.96.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/PKG-INFO` & `pharmpy-core-0.96.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.95.0
+Version: 0.96.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -40,14 +40,34 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.96.0 (2023-05-26)
+-------------------
+
+Changes
+=======
+
+* Rename functions handling the precision matrix (was previously referring to information matrix which was an error)
+* Remove saddle reset for default AMD model
+* Let LLQ column takes precedence over BLQ column
+
+New features
+============
+
+* Add tools.load_example_modelfit_results
+
+Bugfixes
+========
+
+* Fix bug where if-statements were reordered incorrectly
+
 0.95.0 (2023-05-22)
 -------------------
 
 Changes
 =======
 
 * ``ModelfitResults.ofv_iterations`` and ``ModelfitResults.parameter_estimates_iterations`` have NaN rows in failed runs
```

### Comparing `pharmpy-core-0.95.0/README.rst` & `pharmpy-core-0.96.0/README.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/NONMEM.rst` & `pharmpy-core-0.96.0/docs/NONMEM.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/Pharmpy_logo.svg` & `pharmpy-core-0.96.0/docs/Pharmpy_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/Pharmpy_logo_dark.svg` & `pharmpy-core-0.96.0/docs/Pharmpy_logo_dark.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/_ext/conversion.py` & `pharmpy-core-0.96.0/docs/_ext/conversion.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/_ext/pharmpy_snippet.py` & `pharmpy-core-0.96.0/docs/_ext/pharmpy_snippet.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/allometry.rst` & `pharmpy-core-0.96.0/docs/allometry.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/amd.rst` & `pharmpy-core-0.96.0/docs/amd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/api.rst` & `pharmpy-core-0.96.0/docs/api.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/bootstrap.rst` & `pharmpy-core-0.96.0/docs/bootstrap.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/cdd.rst` & `pharmpy-core-0.96.0/docs/cdd.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/cli.rst` & `pharmpy-core-0.96.0/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/conf.py` & `pharmpy-core-0.96.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 source_suffix = '.rst'
 master_doc = 'index'
 project = 'Pharmpy'
 year = '2018-2023'
 authors = ['the Pharmpy development team']
 copyright = '{0}; {1}'.format(year, ', '.join(authors))
-version = release = '0.95.0'
+version = release = '0.96.0'
 html_show_sourcelink = False
 
 pygments_style = 'trac'
 templates_path = ['.']
 
 html_static_path = ['.']
 html_theme = "pydata_sphinx_theme"
```

### Comparing `pharmpy-core-0.95.0/docs/configuration.rst` & `pharmpy-core-0.96.0/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/contribute.rst` & `pharmpy-core-0.96.0/docs/contribute.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/covsearch.rst` & `pharmpy-core-0.96.0/docs/covsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/crossval.rst` & `pharmpy-core-0.96.0/docs/crossval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/custom.css` & `pharmpy-core-0.96.0/docs/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/data.rst` & `pharmpy-core-0.96.0/docs/data.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/design.rst` & `pharmpy-core-0.96.0/docs/design.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/estmethod.rst` & `pharmpy-core-0.96.0/docs/estmethod.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/frem.rst` & `pharmpy-core-0.96.0/docs/frem.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/getting_started.rst` & `pharmpy-core-0.96.0/docs/getting_started.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/help_functions.py` & `pharmpy-core-0.96.0/docs/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/iivsearch.rst` & `pharmpy-core-0.96.0/docs/iivsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/images/Pharmpy_symbol.svg` & `pharmpy-core-0.96.0/docs/images/Pharmpy_symbol.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/images/tools.png` & `pharmpy-core-0.96.0/docs/images/tools.png`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/index.rst` & `pharmpy-core-0.96.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/iovsearch.rst` & `pharmpy-core-0.96.0/docs/iovsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/license.rst` & `pharmpy-core-0.96.0/docs/license.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/linearize.rst` & `pharmpy-core-0.96.0/docs/linearize.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/model.rst` & `pharmpy-core-0.96.0/docs/model.rst`

 * *Files 4% similar despite different names*

```diff
@@ -133,15 +133,19 @@
 
    eta1 = rvs['ETA_1']
 
 Joint distributions are also supported
 
 .. pharmpy-execute::
 
-   frem_model = read_model(path / "frem" / "pheno" / "model_4.mod")
+   from pharmpy.tools import read_modelfit_results
+
+   frem_path = path / "frem" / "pheno" / "model_4.mod"
+   frem_model = read_model(frem_path)
+   frem_model_results = read_modelfit_results(frem_path)
 
    rvs = frem_model.random_variables
    rvs
 
 .. pharmpy-execute::
 
    omega = rvs['ETA_1'].variance
@@ -153,15 +157,15 @@
 
    omega.subs(frem_model.parameters.inits)
 
 or from estimated values
 
 .. pharmpy-execute::
 
-   omega_est = omega.subs(dict(frem_model.modelfit_results.parameter_estimates))
+   omega_est = omega.subs(dict(frem_model_results.parameter_estimates))
    omega_est
 
 Operations on this parameter matrix can be done either by using SymPy
 
 .. pharmpy-execute::
 
    omega_est.cholesky()
@@ -216,39 +220,7 @@
 ~~~~~~~~~~~~~~~~~~~
 
 A model can describe one or more dependent variables (output variables). Each dependent variable is defined in the ``dependent_variables`` attribute. This is a dictionary of each dependent variable symbol to the corresponding ``DVID``. If there is only one dependent variable the ``DVID`` column in the dataset is not needed and its value in this definition is unimportant. The expressions of the dependent variables are all found in the statements.
 
 .. pharmpy-execute::
 
     model.dependent_variables
-
-~~~~~~~~~~~~~~~~
-Modelfit results
-~~~~~~~~~~~~~~~~
-
-If a model has been fit the results can be retrieved directly from the model object. Here are some examples of the results that can be available:
-
-.. pharmpy-execute::
-
-   model.modelfit_results.parameter_estimates
-
-
-.. pharmpy-execute::
-
-   model.modelfit_results.covariance_matrix
-
-.. pharmpy-execute::
-
-   model.modelfit_results.standard_errors
-
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-Updating initial estimates
-~~~~~~~~~~~~~~~~~~~~~~~~~~
-
-Updating all initial estimates of a model from its own results can be done by:
-
-.. pharmpy-execute::
-
-    from pharmpy.modeling import update_inits
-    update_inits(model, model.modelfit_results.parameter_estimates)
-
-
```

### Comparing `pharmpy-core-0.95.0/docs/modelfit.rst` & `pharmpy-core-0.96.0/docs/modelfit.rst`

 * *Files 24% similar despite different names*

```diff
@@ -13,125 +13,125 @@
 Final OFV
 ~~~~~~~~~
 
 The final OFV is available in `ofv`:
 
 .. pharmpy-execute::
 
-    from pharmpy.modeling import read_model
+    from pharmpy.tools import read_modelfit_results
 
-    model = read_model('tests/testdata/nonmem/pheno_real.mod')
-    model.modelfit_results.ofv
+    results = read_modelfit_results('tests/testdata/nonmem/pheno_real.mod')
+    results.ofv
 
 
 Parameter estimates
 ~~~~~~~~~~~~~~~~~~~
 
 The `parameter_estimates` series contains the final estimates of all estimated parameters.
 
 .. pharmpy-execute::
 
-    model.modelfit_results.parameter_estimates
+    results.parameter_estimates
 
 It is also possible to get the parameters with all variability parameters as standard deviations or correlations.
 
 .. pharmpy-execute::
 
-   model.modelfit_results.parameter_estimates_sdcorr
+   results.parameter_estimates_sdcorr
 
 Standard errors of parameter estimates
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The standard errors of the parameter estimates are in the `standard_errors` series.
 
 .. pharmpy-execute::
 
-    model.modelfit_results.standard_errors
+   results.standard_errors
 
 Or in `standard_errors_sdcorr` with variability parameters as standard deviations or correlations.
 
 .. pharmpy-execute::
 
-    model.modelfit_results.standard_errors_sdcorr
+   results.standard_errors_sdcorr
 
 Relative standard errors of parameter estimates
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The relative standard errors of the parameter estimates
 
 
 .. pharmpy-execute::
 
-    model.modelfit_results.relative_standard_errors
+    results.relative_standard_errors
 
 Covariance matrix
 ~~~~~~~~~~~~~~~~~
 
 The covariance matrix for all estimated parameters
 
 .. pharmpy-execute::
 
-    model.modelfit_results.covariance_matrix
+    results.covariance_matrix
 
 Correlation Matrix
 ~~~~~~~~~~~~~~~~~~
 
 The correlation matrix for all estimated parameters.
 
 .. note::
     Note to NONMEM users. This is a proper correlation matrix meaning that diagonal elements are 1.
     Standard errors can be retrieved from `standard_errors`.
 
 .. pharmpy-execute::
 
-    model.modelfit_results.correlation_matrix
+    results.correlation_matrix
 
-Information Matrix
-~~~~~~~~~~~~~~~~~~
+Precision Matrix
+~~~~~~~~~~~~~~~~
 
-The information matrix for all estimated parameters. This is the inverse of the covariance matrix.
+The precision matrix for all estimated parameters. This is the inverse of the covariance matrix.
 
 .. pharmpy-execute::
 
-    model.modelfit_results.information_matrix
+    results.precision_matrix
 
 Indiviudal OFV
 ~~~~~~~~~~~~~~
 
 The OFV for each individual or `iOFV` is in the `individual_ofv` series.
 
 .. pharmpy-execute::
 
-    model.modelfit_results.individual_ofv
+    results.individual_ofv
 
 Predictions
 ~~~~~~~~~~~
 
 Different predictions can be found in `predictions`
 
 .. pharmpy-execute::
 
-    model.modelfit_results.predictions
+    results.predictions
 
 Residuals
 ~~~~~~~~~
 
 Different residual metrics can be found in `residuals`
 
 .. pharmpy-execute::
 
-    model.modelfit_results.residuals
+    results.residuals
 
 Individual estimates
 ~~~~~~~~~~~~~~~~~~~~
 
 Individual estimates (or EBEs)
 
 .. pharmpy-execute::
 
-    model.modelfit_results.individual_estimates
+    results.individual_estimates
 
 Uncertainty for the individual estimates can be found in `individual_estimates_covariance`, which is a series of covariance matrices for each individual.
 
 .. pharmpy-execute::
 
-    model.modelfit_results.individual_estimates_covariance[1]
+    results.individual_estimates_covariance[1]
```

### Comparing `pharmpy-core-0.95.0/docs/modeling.rst` & `pharmpy-core-0.96.0/docs/modeling.rst`

 * *Files 0% similar despite different names*

```diff
@@ -985,18 +985,20 @@
 
 If there are results from a previous run, those can be used for initial estimates in your
 pharmpy model. See :py:func:`pharmpy.modeling.update_inits`.
 
 .. pharmpy-execute::
 
    from pharmpy.modeling import read_model, update_inits
+   from pharmpy.tools import read_modelfit_results
 
    model = read_model(path / "pheno.mod")
+   results = read_modelfit_results(path / "pheno.mod")
 
-   update_inits(model, model.modelfit_results.parameter_estimates)
+   update_inits(model, results.parameter_estimates)
 
 
 ~~~~~~~~~~~~~~~
 Fitting a model
 ~~~~~~~~~~~~~~~
 
 Pharmpy is designed to be able to do fitting of models to data using different external tools. Currently only NONMEM is supported.
@@ -1026,16 +1028,16 @@
 
 Eta shrinkage can be calculated either on the standard deviation scale or on the variance scale
 
 .. pharmpy-execute::
 
     from pharmpy.modeling import calculate_eta_shrinkage
 
-    pe = model.modelfit_results.parameter_estimates
-    ie = model.modelfit_results.individual_estimates
+    pe = results.parameter_estimates
+    ie = results.individual_estimates
     calculate_eta_shrinkage(model, pe, ie)
 
 
 .. pharmpy-execute::
 
     calculate_eta_shrinkage(model, pe, ie, sd=True)
```

### Comparing `pharmpy-core-0.95.0/docs/modelsearch.rst` & `pharmpy-core-0.96.0/docs/modelsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/nonmem_plugin.rst` & `pharmpy-core-0.96.0/docs/nonmem_plugin.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/pharmr_logo.svg` & `pharmpy-core-0.96.0/docs/pharmr_logo.svg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/plots.rst` & `pharmpy-core-0.96.0/docs/plots.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/plugins.rst` & `pharmpy-core-0.96.0/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/projects.rst` & `pharmpy-core-0.96.0/docs/projects.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/qa.rst` & `pharmpy-core-0.96.0/docs/qa.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/ruvsearch.rst` & `pharmpy-core-0.96.0/docs/ruvsearch.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/scm.rst` & `pharmpy-core-0.96.0/docs/scm.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/simeval.rst` & `pharmpy-core-0.96.0/docs/simeval.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/tools.rst` & `pharmpy-core-0.96.0/docs/tools.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/docs/using_r.rst` & `pharmpy-core-0.96.0/docs/using_r.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/requirements.txt` & `pharmpy-core-0.96.0/requirements.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 debugpy==1.6.7
 decorator==5.1.1
 defusedxml==0.7.1
 distributed==2023.5.0
 docutils==0.20.1
 entrypoints==0.4
 executing==1.2.0
-fastjsonschema==2.17.0
+fastjsonschema==2.17.1
 fsspec==2023.5.0
 HeapDict==1.0.1
 idna==3.4
 imagesize==1.4.1
 importlib_metadata==6.6.0
 ipykernel==6.23.1
 ipython==8.13.2
@@ -43,15 +43,15 @@
 locket==1.0.0
 lxml==4.9.2
 MarkupSafe==2.1.2
 matplotlib-inline==0.1.6
 mistune==2.0.5
 mpmath==1.3.0
 msgpack==1.0.5
-nbclient==0.7.4
+nbclient==0.8.0
 nbconvert==7.4.0
 nbformat==5.8.0
 nest-asyncio==1.5.6
 networkx==3.1
 numexpr==2.8.4
 numpy==1.24.3
 packaging==23.1
@@ -69,15 +69,15 @@
 Pygments==2.15.1
 pyreadr==0.4.7
 pyrsistent==0.19.3
 python-dateutil==2.8.2
 pytz==2023.3
 pywin32>=302,!=304; sys_platform == 'win32' and platform_python_implementation != 'PyPy'
 PyYAML==6.0
-requests==2.30.0
+requests==2.31.0
 pyzmq==25.0.2
 rich==13.3.5
 scipy==1.10.1
 six==1.16.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 soupsieve==2.4.1
```

### Comparing `pharmpy-core-0.95.0/setup.cfg` & `pharmpy-core-0.96.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/setup.py` & `pharmpy-core-0.96.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     txt = re.compile(pat, re.MULTILINE | re.DOTALL).findall(text_str)
     txt = [dedent(block).strip() for block in txt]
     return '\n\n'.join(txt)
 
 
 setup(
     name='pharmpy-core',
-    version='0.95.0',
+    version='0.96.0',
     license='GNU Lesser General Public License v3 (LGPLv3)',
     description='Pharmacometric modeling',
     long_description='%s\n\n%s'
     % (strip_refs(longdesc(read('README.rst'))), strip_refs(read('CHANGELOG.rst'))),
     author='Rikard Nordgren',
     author_email='rikard.nordgren@farmaci.uu.se',
     url='https://pharmpy.github.io',
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/cli.py` & `pharmpy-core-0.96.0/src/pharmpy/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -888,16 +888,20 @@
 def input_model(path):
     """Returns :class:`~pharmpy.model.Model` from *path*.
 
     Raises if not found or is dir, without tracebacks (see :func:`error_exit`).
     """
     path = check_input_path(path)
     from pharmpy.model import Model
+    from pharmpy.tools import read_modelfit_results
 
-    model = Model.create_model(path)
+    model = Model.parse_model(path)
+    res = read_modelfit_results(path)
+    # FIXME: Should use tuple or something else instead
+    model = model.replace(modelfit_results=res)
     return model
 
 
 def input_model_or_dataset(path):
     """Returns :class:`~pharmpy.model.Model` or pd.DataFrame from *path*"""
     path = check_input_path(path)
     from pharmpy.plugins.utils import PluginError
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/config.py` & `pharmpy-core-0.96.0/src/pharmpy/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/deps/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/deps/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/deps/altair.py` & `pharmpy-core-0.96.0/src/pharmpy/deps/altair.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/df.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/df.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/ds/ordered_set.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/ds/ordered_set.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/expr/eval.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/expr/eval.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/expr/funcs.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/expr/funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/expr/leaves.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/expr/leaves.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/expr/ode.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/expr/ode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/expr/subs.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/expr/subs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/expr/tree.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/expr/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/expr/units.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/expr/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/fn/signature.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/fn/signature.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/fn/type.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/fn/type.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/fs/lock.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/fs/lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/fs/path.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/fs/path.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/fs/tmp.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/fs/tmp.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/graph/directed/connected_components.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/graph/directed/connected_components.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/immutable.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/immutable.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/math.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/module/lazy.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/module/lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/parse/generic.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/parse/generic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/parse/ignored.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/parse/ignored.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/parse/missing.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/parse/missing.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/parse/prettyprint.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/parse/prettyprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/parse/tree.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/parse/tree.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/parse/treeprint.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/parse/treeprint.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/sequence/lcs.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/sequence/lcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/set/partitions.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/set/partitions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/set/subsets.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/set/subsets.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/internals/unicode.py` & `pharmpy-core-0.96.0/src/pharmpy/internals/unicode.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/model/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/data.py` & `pharmpy-core-0.96.0/src/pharmpy/model/data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/datainfo.py` & `pharmpy-core-0.96.0/src/pharmpy/model/datainfo.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/distributions/numeric.py` & `pharmpy-core-0.96.0/src/pharmpy/model/distributions/numeric.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/distributions/symbolic.py` & `pharmpy-core-0.96.0/src/pharmpy/model/distributions/symbolic.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/estimation.py` & `pharmpy-core-0.96.0/src/pharmpy/model/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/model.py` & `pharmpy-core-0.96.0/src/pharmpy/model/model.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 
 Definitions
 -----------
 """
 from __future__ import annotations
 
 import warnings
-from io import IOBase
 from pathlib import Path
 
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
 from pharmpy.internals.immutable import Immutable, frozenmapping
-from pharmpy.plugins.utils import detect_model
+from pharmpy.model.external import detect_model
 
 from .datainfo import ColumnInfo, DataInfo
 from .estimation import EstimationSteps
 from .parameters import Parameters
 from .random_variables import RandomVariables
 from .statements import ODESystem, Statements
 
@@ -54,52 +53,101 @@
         self,
         name='',
         parameters=Parameters(),
         random_variables=RandomVariables.create(()),
         statements=Statements(),
         dataset=None,
         datainfo=DataInfo(),
-        dependent_variables=None,
+        dependent_variables=frozenmapping({sympy.Symbol('y'): 1}),
         observation_transformation=None,
         estimation_steps=EstimationSteps(),
         modelfit_results=None,
         parent_model=None,
         initial_individual_estimates=None,
         filename_extension='',
         value_type='PREDICTION',
         description='',
         internals=None,
     ):
-        actual_dependent_variables = (
-            {sympy.Symbol('y'): 1} if dependent_variables is None else dependent_variables
-        )
         self._name = name
         self._datainfo = datainfo
         self._dataset = dataset
         self._random_variables = random_variables
         self._parameters = parameters
         self._statements = statements
-        # FIXME: Only do this conversion in the future Model.create
-        self._dependent_variables = frozenmapping(actual_dependent_variables)
+        self._dependent_variables = dependent_variables
         if observation_transformation is None:
-            self._observation_transformation = frozenmapping(
-                {dv: dv for dv in actual_dependent_variables.keys()}
+            observation_transformation = frozenmapping(
+                {dv: dv for dv in dependent_variables.keys()}
             )
-        else:
-            # FIXME: Only do this conversion in the future Model.create
-            self._observation_transformation = frozenmapping(observation_transformation)
+        self._observation_transformation = observation_transformation
         self._estimation_steps = estimation_steps
         self._modelfit_results = modelfit_results
         self._parent_model = parent_model
         self._initial_individual_estimates = initial_individual_estimates
         self._filename_extension = filename_extension
         self._value_type = value_type
         self._description = description
         self._internals = internals
 
+    @classmethod
+    def create(
+        cls,
+        name,
+        parameters=None,
+        random_variables=None,
+        statements=None,
+        dataset=None,
+        datainfo=None,
+        dependent_variables=None,
+        observation_transformation=None,
+        estimation_steps=None,
+        modelfit_results=None,
+        parent_model=None,
+        initial_individual_estimates=None,
+        filename_extension='',
+        value_type='PREDICTION',
+        description='',
+        internals=None,
+    ):
+        Model._canonicalize_name(name)
+        dependent_variables = Model._canonicalize_dependent_variables(dependent_variables)
+        observation_transformation = Model._canonicalize_observation_transformation(
+            observation_transformation, dependent_variables
+        )
+        parameters = Model._canonicalize_parameters(parameters)
+        random_variables = Model._canonicalize_random_variables(random_variables)
+        parameters = Model._canonicalize_parameter_estimates(parameters, random_variables)
+        estimation_steps = Model._canonicalize_estimation_steps(estimation_steps)
+        value_type = Model._canonicalize_value_type(value_type)
+        if not isinstance(datainfo, DataInfo):
+            raise TypeError("model.datainfo must be of DataInfo type")
+
+        if dataset is not None:
+            datainfo = update_datainfo(datainfo, dataset)
+
+        statements = Model._canonicalize_statements(
+            statements, parameters, random_variables, datainfo
+        )
+        return cls(
+            name=name,
+            dependent_variables=dependent_variables,
+            observation_transformation=observation_transformation,
+            parameters=parameters,
+            random_variables=random_variables,
+            estimation_steps=estimation_steps,
+            statements=statements,
+            modelfit_results=modelfit_results,
+            description=description,
+            parent_model=parent_model,
+            filename_extension=filename_extension,
+            internals=internals,
+            initial_individual_estimates=initial_individual_estimates,
+        )
+
     def _canonicalize_value_type(self, value):
         allowed_strings = ('PREDICTION', 'LIKELIHOOD', '-2LL')
         if isinstance(value, str):
             if value.upper() not in allowed_strings:
                 raise ValueError(
                     f"Cannot set value_type to {value}. Must be one of {allowed_strings} "
                     f"or a symbol"
@@ -123,17 +171,23 @@
             params = params.set_initial_estimates(nearest)
         return params
 
     @staticmethod
     def _canonicalize_random_variables(rvs):
         if not isinstance(rvs, RandomVariables):
             raise TypeError("model.random_variables must be of RandomVariables type")
+        if rvs is None:
+            return RandomVariables.create()
+        else:
+            return rvs
 
     @staticmethod
     def _canonicalize_statements(statements, params, rvs, datainfo):
+        if statements is None:
+            return Statements()
         if not isinstance(statements, Statements):
             raise TypeError("model.statements must be of Statements type")
         colnames = {sympy.Symbol(colname) for colname in datainfo.names}
         symbs_all = rvs.free_symbols.union(params.symbols).union(colnames)
         sset_prev = []
         for i, statement in enumerate(statements):
             if isinstance(statement, ODESystem):
@@ -155,35 +209,76 @@
                         if statements.ode_system and symb in statements.ode_system.amounts:
                             continue
                         raise ValueError(f'Symbol {symb} is not defined')
                     if Statements(sset_prev).find_assignment_index(symb) is None:
                         raise ValueError(f'Symbol {symb} defined after being used')
 
             sset_prev += statement
+        return statements
 
-    def replace(self, **kwargs):
-        name = kwargs.get('name', self.name)
+    @staticmethod
+    def _canonicalize_name(name):
         if not isinstance(name, str):
             raise TypeError("Name of a model has to be of string type")
 
+    @staticmethod
+    def _canonicalize_dependent_variables(dvs):
+        if dvs is None:
+            dvs = {sympy.Symbol('y'): 1}
+        return frozenmapping(dvs)
+
+    @staticmethod
+    def _canonicalize_observation_transformation(obs, dvs):
+        if obs is None:
+            obs = {dv: dv for dv in dvs.keys()}
+        return frozenmapping(obs)
+
+    @staticmethod
+    def _canonicalize_parameters(params):
+        if params is None:
+            return Parameters()
+        else:
+            if not isinstance(params, Parameters):
+                raise TypeError("parameters must be of Parameters type")
+            return params
+
+    @staticmethod
+    def _canonicalize_estimation_steps(steps):
+        if steps is None:
+            return EstimationSteps()
+        else:
+            if not isinstance(steps, EstimationSteps):
+                raise TypeError("model.estimation_steps must be of EstimationSteps type")
+            return steps
+
+    def replace(self, **kwargs):
+        name = kwargs.get('name', self.name)
+        Model._canonicalize_name(name)
+
         if 'dependent_variables' in kwargs:
-            dependent_variables = frozenmapping(kwargs['dependent_variables'])
+            dependent_variables = Model._canonicalize_dependent_variables(
+                kwargs['dependent_variables']
+            )
         else:
             dependent_variables = self.dependent_variables
 
         if 'observation_transformation' in kwargs:
-            observation_transformation = frozenmapping(kwargs['observation_transformation'])
+            observation_transformation = Model._canonicalize_observation_transformation(
+                kwargs['observation_transformation'], dependent_variables
+            )
         else:
             observation_transformation = self.observation_transformation
 
-        parameters = kwargs.get('parameters', self.parameters)
+        if 'parameters' in kwargs:
+            parameters = Model._canonicalize_parameters(kwargs['parameters'])
+        else:
+            parameters = self.parameters
 
         if 'random_variables' in kwargs:
-            random_variables = kwargs['random_variables']
-            Model._canonicalize_random_variables(random_variables)
+            random_variables = Model._canonicalize_random_variables(kwargs['random_variables'])
         else:
             random_variables = self.random_variables
 
         parameters = Model._canonicalize_parameter_estimates(parameters, random_variables)
 
         if 'dataset' in kwargs:
             dataset = kwargs['dataset']
@@ -200,22 +295,25 @@
             datainfo = self._datainfo
 
         if new_dataset:
             datainfo = update_datainfo(datainfo, dataset)
 
         # Has to be checked after datainfo is updated since it looks for symbols in datainfo as well
         if 'statements' in kwargs:
-            statements = kwargs['statements']
-            Model._canonicalize_statements(statements, parameters, random_variables, datainfo)
+            statements = Model._canonicalize_statements(
+                kwargs['statements'], parameters, random_variables, datainfo
+            )
         else:
             statements = self.statements
 
-        estimation_steps = kwargs.get('estimation_steps', self.estimation_steps)
-        if not isinstance(estimation_steps, EstimationSteps):
-            raise TypeError("model.estimation_steps must be of EstimationSteps type")
+        if 'estimation_steps' in kwargs:
+            estimation_steps = Model._canonicalize_estimation_steps(kwargs['estimation_steps'])
+        else:
+            estimation_steps = self.estimation_steps
+
         modelfit_results = kwargs.get('modelfit_results', self.modelfit_results)
         parent_model = kwargs.get('parent_model', self.parent_model)
         initial_individual_estimates = kwargs.get(
             'initial_individual_estimates', self.initial_individual_estimates
         )
         filename_extension = kwargs.get('filename_extension', self.filename_extension)
         if not isinstance(filename_extension, str):
@@ -458,47 +556,51 @@
 
     @property
     def description(self):
         """A free text discription of the model"""
         return self._description
 
     @staticmethod
-    def create_model(obj=None, **kwargs):
-        """Factory for creating a :class:`pharmpy.model` object from an object representing the model
-
-        .. _path-like object: https://docs.python.org/3/glossary.html#term-path-like-object
+    def parse_model(path):
+        """Create a model object by parsing a model file of any supported type
 
         Parameters
         ----------
-        obj
-            `path-like object`_ pointing to the model file or an IO object.
+        path : Path or str
+            Path to a model file
 
         Returns
         -------
         Model
-            Generic :class:`~pharmpy.generic.Model` if obj is None, otherwise appropriate
-            implementation is invoked (e.g. NONMEM7 :class:`~pharmpy.plugins.nonmem.Model`).
+            A model object
         """
-        if obj is None:
-            return Model()
-        elif isinstance(obj, IOBase):
-            path = None
-            code = obj.read()
-        elif isinstance(obj, (str, Path)):
-            path = Path(obj)
-            with open(path, 'r', encoding='latin-1') as fp:
-                code = fp.read()
-        else:
-            raise ValueError("Unknown input type to Model constructor")
+        path = Path(path)
+        with open(path, 'r', encoding='latin-1') as fp:
+            code = fp.read()
+
+        model_module = detect_model(code)
+        model = model_module.parse_model(code, path)
+        return model
 
+    @staticmethod
+    def parse_model_from_string(code):
+        """Create a model object by parsing a string with model code of any supported type
+
+        Parameters
+        ----------
+        code : str
+            Model code
+
+        Returns
+        -------
+        Model
+            A model object
+        """
         model_module = detect_model(code)
-        model = model_module.parse_code(code, path, **kwargs)
-        # Setup model database here
-        # Read in model results here?
-        # Set filename extension?
+        model = model_module.parse_model(code, None)
         return model
 
     def update_source(self):
         """Update source code of the model. If any paths need to be changed or added (e.g. for a
         NONMEM model with an updated dataset) they will be replaced with DUMMYPATH"""
         return self
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/parameters.py` & `pharmpy-core-0.96.0/src/pharmpy/model/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/random_variables.py` & `pharmpy-core-0.96.0/src/pharmpy/model/random_variables.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/results.py` & `pharmpy-core-0.96.0/src/pharmpy/model/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/model/statements.py` & `pharmpy-core-0.96.0/src/pharmpy/model/statements.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -108,21 +108,21 @@
     make_declarative,
     mu_reference_model,
     simplify_expression,
 )
 from .iterators import omit_data, resample_data
 from .math import (
     calculate_corr_from_cov,
-    calculate_corr_from_inf,
+    calculate_corr_from_prec,
     calculate_cov_from_corrse,
-    calculate_cov_from_inf,
-    calculate_inf_from_corrse,
-    calculate_inf_from_cov,
+    calculate_cov_from_prec,
+    calculate_prec_from_corrse,
+    calculate_prec_from_cov,
     calculate_se_from_cov,
-    calculate_se_from_inf,
+    calculate_se_from_prec,
 )
 from .metabolite import add_metabolite
 from .odes import (
     add_individual_parameter,
     add_lag_time,
     add_peripheral_compartment,
     display_odes,
@@ -214,28 +214,28 @@
     'add_population_parameter',
     'add_time_after_dose',
     'append_estimation_step_options',
     'bump_model_number',
     'calculate_aic',
     'calculate_bic',
     'calculate_corr_from_cov',
-    'calculate_corr_from_inf',
+    'calculate_corr_from_prec',
     'calculate_cov_from_corrse',
-    'calculate_cov_from_inf',
+    'calculate_cov_from_prec',
     'calculate_epsilon_gradient_expression',
     'calculate_eta_gradient_expression',
     'calculate_eta_shrinkage',
     'calculate_individual_parameter_statistics',
     'calculate_individual_shrinkage',
-    'calculate_inf_from_corrse',
-    'calculate_inf_from_cov',
+    'calculate_prec_from_corrse',
+    'calculate_prec_from_cov',
     'calculate_parameters_from_ucp',
     'calculate_pk_parameters_statistics',
     'calculate_se_from_cov',
-    'calculate_se_from_inf',
+    'calculate_se_from_prec',
     'calculate_ucp_scale',
     'check_dataset',
     'check_high_correlations',
     'check_parameters_near_bounds',
     'cleanup_model',
     'convert_model',
     'create_basic_pk_model',
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/allometry.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/basic_models.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/basic_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,15 +107,14 @@
 
     est = EstimationStep.create(
         "FOCE",
         interaction=True,
         maximum_evaluations=99999,
         predictions=['CIPREDI'],
         residuals=['CWRES'],
-        tool_options={'SADDLE_RESET': 1},
     )
     eststeps = EstimationSteps.create([est])
 
     model = Model(
         name='start',
         statements=stats,
         estimation_steps=eststeps,
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/block_rvs.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/block_rvs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/blq.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/blq.py`

 * *Files 4% similar despite different names*

```diff
@@ -131,16 +131,18 @@
     y_idx = sset.find_assignment_index(y.symbol)
     sset_new = sset[:y_idx] + assignments + sset[y_idx + 1 :]
     model = model.replace(statements=sset_new)
 
     return model.update_source()
 
 
-def has_blq_transformation(model: Model, y_expr):
+def has_blq_transformation(model: Model):
     # FIXME: make more general
+    y = list(model.dependent_variables.keys())[0]
+    y_expr = model.statements.error.find_assignment(y).expression
     if not isinstance(y_expr, sympy.Piecewise):
         return False
     for statement, cond in y_expr.args:
         blq_symb, _ = get_blq_symb_and_type(model)
         if blq_symb in cond.free_symbols:
             break
     else:
@@ -151,20 +153,20 @@
     return _has_all_expected_symbs(model.statements.error, expected_m3) or _has_all_expected_symbs(
         model.statements.error, expected_m4
     )
 
 
 def get_blq_symb_and_type(model: Model):
     try:
-        blq_datainfo = model.datainfo.typeix['blq']
-        return sympy.Symbol(blq_datainfo[0].name), 'blq'
+        blq_datainfo = model.datainfo.typeix['lloq']
+        return sympy.Symbol(blq_datainfo[0].name), 'lloq'
     except IndexError:
         try:
-            blq_datainfo = model.datainfo.typeix['lloq']
-            return sympy.Symbol(blq_datainfo[0].name), 'lloq'
+            blq_datainfo = model.datainfo.typeix['blq']
+            return sympy.Symbol(blq_datainfo[0].name), 'blq'
         except IndexError:
             return sympy.Symbol('LLOQ'), 'lloq'
 
 
 def _has_all_expected_symbs(sset, expected_symbs):
     symb_names = [s.symbol.name for s in sset]
     return all(symb in symb_names for symb in expected_symbs)
@@ -176,26 +178,26 @@
         raise ValueError(
             f'Invalid input model: covariance between epsilons not supported in `method` {method}'
         )
 
 
 def _get_sd(model, y):
     y_expr = model.statements.find_assignment(y.symbol).expression
-    rvs = model.random_variables.epsilons
+    sd_expr = get_sd_expr(y_expr, model.random_variables)
+    symb_sd = create_symbol(model, 'SD')
+    return Assignment(symb_sd, simplify_expression(model, sd_expr))
+
 
+def get_sd_expr(y_expr, rvs):
     rv_terms = [arg for arg in y_expr.args if arg.free_symbols.intersection(rvs.free_symbols)]
     sd_expr = []
     for i, term in enumerate(rv_terms, 1):
-        rvs_in_term = model.random_variables.free_symbols.intersection(term.free_symbols)
+        rvs_in_term = rvs.free_symbols.intersection(term.free_symbols)
         if len(rvs_in_term) > 1:
             raise ValueError(
                 'Invalid input model: error model not supported, terms in error model cannot contain '
                 'more than one random variable'
             )
         expr = rvs.replace_with_sympy_rvs(term)
-        std_term = simplify_expression(model, sympy.stats.std(expr))
-        sd_expr.append(std_term)
-
-    symb_sd = create_symbol(model, 'SD')
-    sd_expr_full = sympy.sqrt(sympy.Add(*[expr**2 for expr in sd_expr]))
+        sd_expr.append(sympy.stats.std(expr))
 
-    return Assignment(symb_sd, simplify_expression(model, sd_expr_full))
+    return sympy.sqrt(sympy.Add(*[expr**2 for expr in sd_expr]))
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/common.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Common modeling pipeline elements
 :meta private:
 """
 
 import re
 import warnings
-from io import StringIO
 from pathlib import Path
 from typing import Dict, Union
 
 import pharmpy.config as config
 from pharmpy.deps import sympy
 from pharmpy.internals.fs.path import normalize_user_given_path
 from pharmpy.model import (
@@ -44,15 +43,15 @@
     See also
     --------
     read_model_from_database : Read model from database
     read_model_from_string : Read model from string
 
     """
     path = normalize_user_given_path(path)
-    model = Model.create_model(path)
+    model = Model.parse_model(path)
     return model
 
 
 def read_model_from_string(code: str):
     """Read model from the model code in a string
 
     Parameters
@@ -82,15 +81,15 @@
 
     See also
     --------
     read_model : Read model from file
     read_model_from_database : Read model from database
 
     """
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     return model
 
 
 def write_model(model: Model, path: Union[str, Path] = '', force: bool = True):
     """Write model code to file
 
     Parameters
@@ -165,15 +164,15 @@
 
     """
     supported = ['generic', 'nlmixr', 'nonmem', 'rxode']
     if to_format not in supported:
         raise ValueError(f"Unknown format {to_format}: supported formats are f{supported}")
     # FIXME: Use code that can discover plugins below
     if to_format == 'generic':
-        new = Model.create_model()
+        new = Model()
         new = new.replace(
             dataset=model.dataset,
             datainfo=model.datainfo,
             name=model.name,
             parameters=model.parameters,
             statements=model.statements,
             random_variables=model.random_variables,
@@ -183,23 +182,23 @@
             description=model.description,
             parent_model=model.name,
             filename_extension=model.filename_extension,
             initial_individual_estimates=model.initial_individual_estimates,
         )
         return new
     elif to_format == 'nlmixr':
-        import pharmpy.plugins.nlmixr.model as nlmixr
+        import pharmpy.model.external.nlmixr.model as nlmixr
 
         new = nlmixr.convert_model(model)
     elif to_format == 'rxode':
-        import pharmpy.plugins.rxode.model as rxode
+        import pharmpy.model.external.rxode.model as rxode
 
         new = rxode.convert_model(model)
     else:
-        import pharmpy.plugins.nonmem.model as nonmem
+        import pharmpy.model.external.nonmem.model as nonmem
 
         new = nonmem.convert_model(model)
     return new
 
 
 def get_model_code(model: Model):
     """Get the model code of the underlying model language
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/compartments.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/compartments.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/covariate_effect.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/data.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1632,16 +1632,16 @@
         The dataset
     """
     if not isinstance(datainfo, DataInfo):
         datainfo = DataInfo.read_json(datainfo)
 
     if datainfo.path is None:
         raise ValueError('datainfo.path is None')
-    from pharmpy.plugins.nonmem.dataset import read_nonmem_dataset
-    from pharmpy.plugins.nonmem.parsing import filter_observations
+    from pharmpy.model.external.nonmem.dataset import read_nonmem_dataset
+    from pharmpy.model.external.nonmem.parsing import filter_observations
 
     if datatype == 'nonmem':
         drop = [col.drop for col in datainfo]
         df = read_nonmem_dataset(
             datainfo.path,
             ignore_character='@',
             drop=drop,
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/error.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/error.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,17 +6,18 @@
 from typing import List, Optional, Union
 
 from pharmpy.deps import sympy
 from pharmpy.internals.expr.parse import parse as parse_expr
 from pharmpy.internals.expr.subs import subs
 from pharmpy.model import Assignment, Model, NormalDistribution, Parameter, Parameters, Statements
 
+from .blq import get_blq_symb_and_type, get_sd_expr, has_blq_transformation
 from .common import _get_unused_parameters_and_rvs, remove_unused_parameters_and_rvs
 from .data import get_observations
-from .expressions import _create_symbol, create_symbol, get_dv_symbol
+from .expressions import _create_symbol, create_symbol, get_dv_symbol, simplify_expression
 from .help_functions import _format_input_list, _get_epsilons
 from .parameters import add_population_parameter, fix_parameters, set_initial_estimates
 
 
 def _preparations(model, y=None):
     stats = model.statements
     # FIXME: handle other DVs?
@@ -263,44 +264,71 @@
 
     stats, y, f = _preparations(model, dv)
     ruv = create_symbol(model, 'epsilon_p')
 
     data_trans = _canonicalize_data_transformation(model, data_trans, dv)
     ipred = create_symbol(model, 'IPREDADJ') if zero_protection else f
 
+    sigma = create_symbol(model, 'sigma')
+    model = add_population_parameter(model, sigma.name, 0.09)
+
+    eps = NormalDistribution.create(ruv.name, 'RUV', 0, sigma)
+
+    f_dummy = sympy.Dummy('x')
     if data_trans == sympy.log(dv):
-        expr = sympy.log(ipred) + ruv
+        error_expr = sympy.log(ipred) + ruv if zero_protection else sympy.log(f_dummy) + ruv
     elif data_trans == dv:
-        expr = f + ipred * ruv
+        error_expr = f_dummy + ipred * ruv if zero_protection else f_dummy + f_dummy * ruv
     else:
         raise ValueError(f"Not supported data transformation {data_trans}")
 
-    statements = model.statements
+    if has_blq_transformation(model):
+        f, stats_new = _get_updated_blq_statements(model, error_expr, y, f, f_dummy, eps)
+    else:
+        expr = error_expr.subs({f_dummy: f})
+        stats_new = stats.reassign(y, expr)
+
     if zero_protection:
         guard_expr = sympy.Piecewise((2.225e-16, sympy.Eq(f, 0)), (f, True))
         guard_assignment = Assignment(ipred, guard_expr)
-        ind = stats.find_assignment_index(y)
-        statements = statements[0:ind] + guard_assignment + statements[ind:]
-
-    sigma = create_symbol(model, 'sigma')
-    model = add_population_parameter(model, sigma.name, 0.09)
-
-    eps = NormalDistribution.create(ruv.name, 'RUV', 0, sigma)
+        ind = 0
+        # Find first occurrence of IPREDADJ
+        for i, s in enumerate(stats_new):
+            if ipred in s.free_symbols:
+                ind = i
+                break
+        stats_new = stats_new[0:ind] + guard_assignment + stats_new[ind:]
 
     rvs_new, params_new = _get_unused_parameters_and_rvs(
-        stats.reassign(y, expr), model.parameters, model.random_variables + eps
+        stats_new, model.parameters, model.random_variables + eps
     )
 
-    model = model.replace(
-        statements=statements.reassign(y, expr), random_variables=rvs_new, parameters=params_new
-    )
+    model = model.replace(statements=stats_new, random_variables=rvs_new, parameters=params_new)
 
     return model.update_source()
 
 
+def _get_updated_blq_statements(model, expr_dummy, y, f, f_dummy, eps_new):
+    blq_symb, _ = get_blq_symb_and_type(model)
+    for expr, cond in f.args:
+        if blq_symb in cond.free_symbols:
+            f_above_lloq = expr
+            break
+    else:
+        raise AssertionError('BLQ symbol not found')
+    expr_above_lloq = expr_dummy.subs({f_dummy: f_above_lloq})
+    expr = f.subs({f_above_lloq: expr_above_lloq})
+    # FIXME: make more general
+    sd = model.statements.find_assignment('SD')
+    sd_new = get_sd_expr(expr_above_lloq, model.random_variables + eps_new)
+    stats_new = model.statements.reassign(sd.symbol, simplify_expression(model, sd_new))
+    stats_new = stats_new.reassign(y, expr)
+    return f_above_lloq, stats_new
+
+
 def set_combined_error_model(
     model: Model,
     dv: Union[sympy.Symbol, str, int, None] = None,
     data_trans: Optional[Union[str, sympy.Expr]] = None,
 ):
     r"""Set a combined error model. Initial estimates for new sigmas are :math:`(min(DV)/2)²` for
     proportional and 0.09 for additive.
@@ -363,62 +391,74 @@
     ruv_add = create_symbol(model, 'epsilon_a')
 
     eta_ruv = sympy.Symbol('ETA_RV1')
     theta_time = sympy.Symbol('time_varying')
 
     data_trans = _canonicalize_data_transformation(model, data_trans, dv)
 
+    sigma_prop = create_symbol(model, 'sigma_prop')
+    model = add_population_parameter(model, sigma_prop.name, 0.09)
+    sigma_add = create_symbol(model, 'sigma_add')
+    model = add_population_parameter(model, sigma_add.name, _get_prop_init(model))
+
+    eps_prop = NormalDistribution.create(ruv_prop.name, 'RUV', 0, sigma_prop)
+    eps_add = NormalDistribution.create(ruv_add.name, 'RUV', 0, sigma_add)
+
     # FIXME: handle other DVs
     dv = list(model.dependent_variables.keys())[0]
+    f_dummy = sympy.Dummy('x')
     if data_trans == sympy.log(dv):
-        expr_combined = sympy.log(f) + ruv_prop + ruv_add / f
+        error_expr = sympy.log(f_dummy) + ruv_prop + ruv_add / f_dummy
     elif data_trans == dv:
-        if isinstance(expr, sympy.Piecewise):
+        # Time varying
+        if isinstance(expr, sympy.Piecewise) and not has_blq_transformation(model):
             expr_0 = expr.args[0][0]
             expr_1 = expr.args[1][0]
             cond_0 = expr.args[0][1]
-            expr_combined = None
+            error_expr = None
             for eps in model.random_variables.epsilons.names:
                 expr_0 = subs(expr_0, {sympy.Symbol(eps): ruv_prop}, simultaneous=True)
                 expr_1 = subs(expr_1, {sympy.Symbol(eps): ruv_prop}, simultaneous=True)
                 if (
                     eta_ruv in model.random_variables.free_symbols
                     and theta_time in model.parameters.symbols
                 ):
-                    expr_combined = sympy.Piecewise(
+                    error_expr = sympy.Piecewise(
                         (expr_0 + ruv_add * theta_time * sympy.exp(eta_ruv), cond_0),
                         (expr_1 + ruv_add * sympy.exp(eta_ruv), True),
                     )
                 elif (
                     eta_ruv not in model.random_variables.free_symbols
                     and theta_time in model.parameters.symbols
                 ):
-                    expr_combined = sympy.Piecewise(
+                    error_expr = sympy.Piecewise(
                         (expr_0 + ruv_add * theta_time, cond_0), (expr_1 + ruv_add, True)
                     )
-            assert expr_combined is not None
+            assert error_expr is not None
         elif (
             eta_ruv in model.random_variables.free_symbols
             and theta_time not in model.parameters.symbols
         ):
-            expr_combined = f + f * ruv_prop * sympy.exp(eta_ruv) + ruv_add * sympy.exp(eta_ruv)
+            if has_blq_transformation(model):
+                raise ValueError('Currently not supported to change from IIV on RUV model with BLQ')
+            error_expr = (
+                f_dummy + f_dummy * ruv_prop * sympy.exp(eta_ruv) + ruv_add * sympy.exp(eta_ruv)
+            )
         else:
-            expr_combined = f + f * ruv_prop + ruv_add
+            error_expr = f_dummy + f_dummy * ruv_prop + ruv_add
     else:
         raise ValueError(f"Not supported data transformation {data_trans}")
 
-    stats_new = stats.reassign(y, expr_combined)
-
-    sigma_prop = create_symbol(model, 'sigma_prop')
-    model = add_population_parameter(model, sigma_prop.name, 0.09)
-    sigma_add = create_symbol(model, 'sigma_add')
-    model = add_population_parameter(model, sigma_add.name, _get_prop_init(model))
-
-    eps_prop = NormalDistribution.create(ruv_prop.name, 'RUV', 0, sigma_prop)
-    eps_add = NormalDistribution.create(ruv_add.name, 'RUV', 0, sigma_add)
+    if has_blq_transformation(model):
+        _, stats_new = _get_updated_blq_statements(
+            model, error_expr, y, f, f_dummy, [eps_prop, eps_add]
+        )
+    else:
+        expr = error_expr.subs({f_dummy: f})
+        stats_new = stats.reassign(y, expr)
 
     rvs_new, params_new = _get_unused_parameters_and_rvs(
         stats_new, model.parameters, model.random_variables + [eps_prop, eps_add]
     )
     model = model.replace(statements=stats_new, random_variables=rvs_new, parameters=params_new)
 
     return model.update_source()
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/estimation.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/estimation_steps.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/eta_additions.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/eta_additions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/eta_transformations.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/eta_transformations.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/evaluation.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/evaluation.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,16 +60,18 @@
     -------
     pd.Series
         A series of one evaluated value for each data record
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, evaluate_expression
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> pe = model.modelfit_results.parameter_estimates
+    >>> results = load_example_modelfit_results("pheno")
+    >>> pe = results.parameter_estimates
     >>> evaluate_expression(model, "TVCL*1000", parameter_estimates=pe)
     0      6.573770
     1      6.573770
     2      6.573770
     3      6.573770
     4      6.573770
              ...
@@ -118,16 +120,18 @@
     -------
     pd.Series
         Population predictions
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, evaluate_population_prediction
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno_linear")
-    >>> pe = model.modelfit_results.parameter_estimates
+    >>> results = load_example_modelfit_results("pheno_linear")
+    >>> pe = results.parameter_estimates
     >>> evaluate_population_prediction(model, parameters=dict(pe))
     0      17.529739
     1      28.179910
     2       9.688648
     3      17.798916
     4      25.023225
              ...
@@ -184,16 +188,18 @@
     -------
     pd.Series
         Individual predictions
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, evaluate_individual_prediction
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno_linear")
-    >>> etas = model.modelfit_results.individual_estimates
+    >>> results = load_example_modelfit_results("pheno_linear")
+    >>> etas = results.individual_estimates
     >>> evaluate_individual_prediction(model, etas=etas)
     0      17.771084
     1      28.881859
     2      11.441728
     3      21.113050
     4      29.783055
              ...
@@ -270,16 +276,18 @@
     -------
     pd.DataFrame
         Gradient
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, evaluate_eta_gradient
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno_linear")
-    >>> etas = model.modelfit_results.individual_estimates
+    >>> results = load_example_modelfit_results("pheno_linear")
+    >>> etas = results.individual_estimates
     >>> evaluate_eta_gradient(model, etas=etas)
          dF/dETA_1  dF/dETA_2
     0     -0.159537 -17.609116
     1     -9.325893 -19.562289
     2     -0.104417 -11.346161
     3     -4.452951 -16.682310
     4    -10.838840 -18.981836
@@ -358,16 +366,18 @@
     -------
     pd.DataFrame
         Gradient
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, evaluate_epsilon_gradient
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno_linear")
-    >>> etas = model.modelfit_results.individual_estimates
+    >>> results = load_example_modelfit_results("pheno_linear")
+    >>> etas = results.individual_estimates
     >>> evaluate_epsilon_gradient(model, etas=etas)
          dY/dEPS_1
     0     17.771084
     1     28.881859
     2     11.441728
     3     21.113050
     4     29.783055
@@ -444,16 +454,18 @@
     -------
     pd.Series
         WRES
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, evaluate_weighted_residuals
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno_linear")
-    >>> parameters = model.modelfit_results.parameter_estimates
+    >>> results = load_example_modelfit_results("pheno_linear")
+    >>> parameters = results.parameter_estimates
     >>> evaluate_weighted_residuals(model, parameters=dict(parameters))
     0     -0.313859
     1      0.675721
     2     -1.544240
     3      1.921720
     4      1.517677
             ...
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/moxo.csv` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/moxo.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/moxo.mod` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/moxo.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.cov` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.datainfo` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.dta` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.ext` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.lst` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.mod` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.phi` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno.tab` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.dta` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.ext` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.lst` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.mod` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/example_models/pheno_linear.phi` & `pharmpy-core-0.96.0/src/pharmpy/modeling/example_models/pheno_linear.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/expressions.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/expressions.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,14 @@
     Returns
     -------
     Expression
         Simplified expression
 
     Example
     -------
-    >>> from pharmpy.plugins.nonmem import conf
     >>> from pharmpy.modeling import load_example_model, simplify_expression
     >>> model = load_example_model("pheno")
     >>> simplify_expression(model, "Abs(PTVCL)")
     PTVCL
     """
     expr = parse_expr(expr)
     d = {}
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/help_functions.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/iterators.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/lrt.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/math.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/math.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,17 +14,18 @@
     Return
     ------
     pd.Series
         Standard errors
 
     Examples
     --------
-    >>> from pharmpy.modeling import load_example_model, calculate_se_from_cov
-    >>> model = load_example_model("pheno")
-    >>> cov = model.modelfit_results.covariance_matrix
+    >>> from pharmpy.modeling import calculate_se_from_cov
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> cov = results.covariance_matrix
     >>> cov
                       PTVCL          PTVV   THETA_3      IVCL           IVV     SIGMA_1_1
     PTVCL      4.411510e-08  4.010000e-08 -0.000002 -0.000001  1.538630e-07  8.178090e-08
     PTVV       4.010000e-08  7.233530e-04 -0.000804  0.000050  7.171840e-05  1.461760e-05
     THETA_3   -1.665010e-06 -8.040250e-04  0.007016 -0.000108 -3.944800e-05  2.932950e-05
     IVCL      -1.093430e-06  4.981380e-05 -0.000108  0.000180 -1.856650e-05  4.867230e-06
     IVV        1.538630e-07  7.171840e-05 -0.000039 -0.000019  5.589820e-05 -4.685650e-07
@@ -36,73 +37,74 @@
     IVCL         0.013415
     IVV          0.007477
     SIGMA_1_1    0.002279
     dtype: float64
 
     See also
     --------
-    calculate_se_from_inf : Standard errors from information matrix
+    calculate_se_from_prec : Standard errors from precision matrix
     calculate_corr_from_cov : Correlation matrix from covariance matrix
-    calculate_cov_from_inf : Covariance matrix from information matrix
+    calculate_cov_from_prec : Covariance matrix from precision matrix
     calculate_cov_from_corrse : Covariance matrix from correlation matrix and standard errors
-    calculate_inf_from_cov : Information matrix from covariance matrix
-    calculate_inf_from_corrse : Information matrix from correlation matrix and standard errors
-    calculate_corr_from_inf : Correlation matrix from information matrix
+    calculate_prec_from_cov : Precision matrix from covariance matrix
+    calculate_prec_from_corrse : Precision matrix from correlation matrix and standard errors
+    calculate_corr_from_prec : Correlation matrix from precision matrix
     """
     se = pd.Series(np.sqrt(np.diag(cov.values)), index=cov.index)
     return se
 
 
-def calculate_se_from_inf(information_matrix: pd.DataFrame):
-    """Calculate standard errors from an information matrix
+def calculate_se_from_prec(precision_matrix: pd.DataFrame):
+    """Calculate standard errors from a precision matrix
 
     Parameters
     ----------
-    information_matrix : pd.DataFrame
-        Input information matrix
+    precision_matrix : pd.DataFrame
+        Input precision matrix
 
     Return
     ------
     pd.Series
         Standard errors
 
     Examples
     --------
-    >>> from pharmpy.modeling import load_example_model, calculate_se_from_inf
-    >>> model = load_example_model("pheno")
-    >>> inf = model.modelfit_results.information_matrix
-    >>> inf
+    >>> from pharmpy.modeling import calculate_se_from_prec
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> prec = results.precision_matrix
+    >>> prec
                       PTVCL          PTVV       THETA_3           IVCL           IVV      SIGMA_1_1
     PTVCL      2.995567e+07  22660.028196  16057.855248  203511.614428 -39474.250514 -820118.299536
     PTVV       2.266003e+04   2129.904642    260.176234    -375.266233  -2800.816246   -7718.769557
     THETA_3    1.605786e+04    260.176234    187.038903     177.207683   -205.808480   -2225.150449
     IVCL       2.035116e+05   -375.266233    177.207683    7527.530027   2462.974821   -9977.488860
     IVV       -3.947425e+04  -2800.816246   -205.808480    2462.974821  22343.198618    9370.758371
     SIGMA_1_1 -8.201183e+05  -7718.769557  -2225.150449   -9977.488860   9370.758371  249847.177845
-    >>> calculate_se_from_inf(inf)
+    >>> calculate_se_from_prec(prec)
     PTVCL        0.000210
     PTVV         0.026895
     THETA_3      0.083762
     IVCL         0.013415
     IVV          0.007477
     SIGMA_1_1    0.002279
     dtype: float64
 
     See also
     --------
     calculate_se_from_cov : Standard errors from covariance matrix
     calculate_corr_from_cov : Correlation matrix from covariance matrix
-    calculate_cov_from_inf : Covariance matrix from information matrix
+    calculate_cov_from_prec : Covariance matrix from precision matrix
     calculate_cov_from_corrse : Covariance matrix from correlation matrix and standard errors
-    calculate_inf_from_cov : Information matrix from covariance matrix
-    calculate_inf_from_corrse : Information matrix from correlation matrix and standard errors
-    calculate_corr_from_inf : Correlation matrix from information matrix
+    calculate_prec_from_cov : Precision matrix from covariance matrix
+    calculate_prec_from_corrse : Precision matrix from correlation matrix and standard errors
+    calculate_corr_from_prec : Correlation matrix from precision matrix
     """
     se = pd.Series(
-        np.sqrt(np.diag(np.linalg.inv(information_matrix.values))), index=information_matrix.index
+        np.sqrt(np.diag(np.linalg.inv(precision_matrix.values))), index=precision_matrix.index
     )
     return se
 
 
 def calculate_corr_from_cov(cov: pd.DataFrame):
     """Calculate correlation matrix from a covariance matrix
 
@@ -114,17 +116,18 @@
     Return
     ------
     pd.DataFrame
         Correlation matrix
 
     Examples
     --------
-    >>> from pharmpy.modeling import load_example_model, calculate_corr_from_cov
-    >>> model = load_example_model("pheno")
-    >>> cov = model.modelfit_results.covariance_matrix
+    >>> from pharmpy.modeling import calculate_corr_from_cov
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> cov = results.covariance_matrix
     >>> cov
                       PTVCL          PTVV   THETA_3      IVCL           IVV     SIGMA_1_1
     PTVCL      4.411510e-08  4.010000e-08 -0.000002 -0.000001  1.538630e-07  8.178090e-08
     PTVV       4.010000e-08  7.233530e-04 -0.000804  0.000050  7.171840e-05  1.461760e-05
     THETA_3   -1.665010e-06 -8.040250e-04  0.007016 -0.000108 -3.944800e-05  2.932950e-05
     IVCL      -1.093430e-06  4.981380e-05 -0.000108  0.000180 -1.856650e-05  4.867230e-06
     IVV        1.538630e-07  7.171840e-05 -0.000039 -0.000019  5.589820e-05 -4.685650e-07
@@ -137,76 +140,77 @@
     IVCL      -0.388059  0.138062 -0.096515  1.000000 -0.185111   0.159170
     IVV        0.097981  0.356662 -0.062991 -0.185111  1.000000  -0.027495
     SIGMA_1_1  0.170820  0.238441  0.153616  0.159170 -0.027495   1.000000
 
     See also
     --------
     calculate_se_from_cov : Standard errors from covariance matrix
-    calculate_se_from_inf : Standard errors from information matrix
-    calculate_cov_from_inf : Covariance matrix from information matrix
+    calculate_se_from_prec : Standard errors from precision matrix
+    calculate_cov_from_prec : Covariance matrix from precision matrix
     calculate_cov_from_corrse : Covariance matrix from correlation matrix and standard errors
-    calculate_inf_from_cov : Information matrix from covariance matrix
-    calculate_inf_from_corrse : Information matrix from correlation matrix and standard errors
-    calculate_corr_from_inf : Correlation matrix from information matrix
+    calculate_prec_from_cov : Precision matrix from covariance matrix
+    calculate_prec_from_corrse : Precision matrix from correlation matrix and standard errors
+    calculate_corr_from_prec : Correlation matrix from precision matrix
     """
 
     corr = pd.DataFrame(cov2corr(cov.values), index=cov.index, columns=cov.columns)
     return corr
 
 
-def calculate_cov_from_inf(information_matrix: pd.DataFrame):
-    """Calculate covariance matrix from an information matrix
+def calculate_cov_from_prec(precision_matrix: pd.DataFrame):
+    """Calculate covariance matrix from a precision matrix
 
     Parameters
     ----------
-    information_matrix : pd.DataFrame
-        Information matrix
+    precision_matrix : pd.DataFrame
+        Precision matrix
 
     Return
     ------
     pd.DataFrame
         Covariance matrix
 
     Examples
     --------
-    >>> from pharmpy.modeling import load_example_model, calculate_cov_from_inf
-    >>> model = load_example_model("pheno")
-    >>> inf = model.modelfit_results.information_matrix
-    >>> inf
+    >>> from pharmpy.modeling import calculate_cov_from_prec
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> prec = results.precision_matrix
+    >>> prec
                       PTVCL          PTVV       THETA_3           IVCL           IVV      SIGMA_1_1
     PTVCL      2.995567e+07  22660.028196  16057.855248  203511.614428 -39474.250514 -820118.299536
     PTVV       2.266003e+04   2129.904642    260.176234    -375.266233  -2800.816246   -7718.769557
     THETA_3    1.605786e+04    260.176234    187.038903     177.207683   -205.808480   -2225.150449
     IVCL       2.035116e+05   -375.266233    177.207683    7527.530027   2462.974821   -9977.488860
     IVV       -3.947425e+04  -2800.816246   -205.808480    2462.974821  22343.198618    9370.758371
     SIGMA_1_1 -8.201183e+05  -7718.769557  -2225.150449   -9977.488860   9370.758371  249847.177845
-    >>> calculate_cov_from_inf(inf)
+    >>> calculate_cov_from_prec(prec)
                       PTVCL          PTVV   THETA_3      IVCL           IVV     SIGMA_1_1
     PTVCL      4.411510e-08  4.010000e-08 -0.000002 -0.000001  1.538630e-07  8.178090e-08
     PTVV       4.010000e-08  7.233530e-04 -0.000804  0.000050  7.171840e-05  1.461760e-05
     THETA_3   -1.665010e-06 -8.040250e-04  0.007016 -0.000108 -3.944800e-05  2.932950e-05
     IVCL      -1.093430e-06  4.981380e-05 -0.000108  0.000180 -1.856650e-05  4.867230e-06
     IVV        1.538630e-07  7.171840e-05 -0.000039 -0.000019  5.589820e-05 -4.685650e-07
     SIGMA_1_1  8.178090e-08  1.461760e-05  0.000029  0.000005 -4.685650e-07  5.195640e-06
 
     See also
     --------
     calculate_se_from_cov : Standard errors from covariance matrix
-    calculate_se_from_inf : Standard errors from information matrix
+    calculate_se_from_prec : Standard errors from precision matrix
     calculate_corr_from_cov : Correlation matrix from covariance matrix
     calculate_cov_from_corrse : Covariance matrix from correlation matrix and standard errors
-    calculate_inf_from_cov : Information matrix from covariance matrix
-    calculate_inf_from_corrse : Information matrix from correlation matrix and standard errors
-    calculate_corr_from_inf : Correlation matrix from information matrix
+    calculate_prec_from_cov : Precision matrix from covariance matrix
+    calculate_prec_from_corrse : Precision matrix from correlation matrix and standard errors
+    calculate_corr_from_prec : Correlation matrix from precision matrix
     """
 
     cov = pd.DataFrame(
-        np.linalg.inv(information_matrix.values),
-        index=information_matrix.index,
-        columns=information_matrix.columns,
+        np.linalg.inv(precision_matrix.values),
+        index=precision_matrix.index,
+        columns=precision_matrix.columns,
     )
     return cov
 
 
 def calculate_cov_from_corrse(corr: pd.DataFrame, se: pd.Series):
     """Calculate covariance matrix from a correlation matrix and standard errors
 
@@ -220,18 +224,19 @@
     Return
     ------
     pd.DataFrame
         Covariance matrix
 
     Examples
     --------
-    >>> from pharmpy.modeling import load_example_model, calculate_cov_from_corrse
-    >>> model = load_example_model("pheno")
-    >>> corr = model.modelfit_results.correlation_matrix
-    >>> se = model.modelfit_results.standard_errors
+    >>> from pharmpy.modeling import calculate_cov_from_corrse
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> corr = results.correlation_matrix
+    >>> se = results.standard_errors
     >>> corr
                   PTVCL      PTVV   THETA_3      IVCL       IVV  SIGMA_1_1
     PTVCL      1.000000  0.007099 -0.094640 -0.388059  0.097981   0.170820
     PTVV       0.007099  1.000000 -0.356899  0.138062  0.356662   0.238441
     THETA_3   -0.094640 -0.356899  1.000000 -0.096515 -0.062991   0.153616
     IVCL      -0.388059  0.138062 -0.096515  1.000000 -0.185111   0.159170
     IVV        0.097981  0.356662 -0.062991 -0.185111  1.000000  -0.027495
@@ -244,178 +249,181 @@
     IVCL      -1.093431e-06  4.981380e-05 -0.000108  0.000180 -1.856651e-05  4.867245e-06
     IVV        1.538630e-07  7.171834e-05 -0.000039 -0.000019  5.589820e-05 -4.685661e-07
     SIGMA_1_1  8.178111e-08  1.461762e-05  0.000029  0.000005 -4.685661e-07  5.195664e-06
 
     See also
     --------
     calculate_se_from_cov : Standard errors from covariance matrix
-    calculate_se_from_inf : Standard errors from information matrix
+    calculate_se_from_prec : Standard errors from precision matrix
     calculate_corr_from_cov : Correlation matrix from covariance matrix
-    calculate_cov_from_inf : Covariance matrix from information matrix
-    calculate_inf_from_cov : Information matrix from covariance matrix
-    calculate_inf_from_corrse : Information matrix from correlation matrix and standard errors
-    calculate_corr_from_inf : Correlation matrix from information matrix
+    calculate_cov_from_prec : Covariance matrix from precision matrix
+    calculate_prec_from_cov : Precision matrix from covariance matrix
+    calculate_prec_from_corrse : Precision matrix from correlation matrix and standard errors
+    calculate_corr_from_prec : Correlation matrix from precision matrix
     """
 
     sd_matrix = np.diag(se.values)
     cov = sd_matrix @ corr.values @ sd_matrix
     cov_df = pd.DataFrame(cov, index=corr.index, columns=corr.columns)
     return cov_df
 
 
-def calculate_inf_from_cov(cov: pd.DataFrame):
-    """Calculate information matrix from a covariance matrix
+def calculate_prec_from_cov(cov: pd.DataFrame):
+    """Calculate precision matrix from a covariance matrix
 
     Parameters
     ----------
     cov : pd.DataFrame
         Covariance matrix
 
     Return
     ------
     pd.DataFrame
-        Information matrix
+        Precision matrix
 
     Examples
     --------
-    >>> from pharmpy.modeling import load_example_model, calculate_inf_from_cov
-    >>> model = load_example_model("pheno")
-    >>> cov = model.modelfit_results.covariance_matrix
+    >>> from pharmpy.modeling import calculate_prec_from_cov
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> cov = results.covariance_matrix
     >>> cov
                       PTVCL          PTVV   THETA_3      IVCL           IVV     SIGMA_1_1
     PTVCL      4.411510e-08  4.010000e-08 -0.000002 -0.000001  1.538630e-07  8.178090e-08
     PTVV       4.010000e-08  7.233530e-04 -0.000804  0.000050  7.171840e-05  1.461760e-05
     THETA_3   -1.665010e-06 -8.040250e-04  0.007016 -0.000108 -3.944800e-05  2.932950e-05
     IVCL      -1.093430e-06  4.981380e-05 -0.000108  0.000180 -1.856650e-05  4.867230e-06
     IVV        1.538630e-07  7.171840e-05 -0.000039 -0.000019  5.589820e-05 -4.685650e-07
     SIGMA_1_1  8.178090e-08  1.461760e-05  0.000029  0.000005 -4.685650e-07  5.195640e-06
-    >>> calculate_inf_from_cov(cov)
+    >>> calculate_prec_from_cov(cov)
                       PTVCL          PTVV       THETA_3           IVCL           IVV      SIGMA_1_1
     PTVCL      2.995567e+07  22660.028196  16057.855248  203511.614428 -39474.250514 -820118.299536
     PTVV       2.266003e+04   2129.904642    260.176234    -375.266233  -2800.816246   -7718.769557
     THETA_3    1.605786e+04    260.176234    187.038903     177.207683   -205.808480   -2225.150449
     IVCL       2.035116e+05   -375.266233    177.207683    7527.530027   2462.974821   -9977.488860
     IVV       -3.947425e+04  -2800.816246   -205.808480    2462.974821  22343.198618    9370.758371
     SIGMA_1_1 -8.201183e+05  -7718.769557  -2225.150449   -9977.488860   9370.758371  249847.177845
 
     See also
     --------
     calculate_se_from_cov : Standard errors from covariance matrix
-    calculate_se_from_inf : Standard errors from information matrix
+    calculate_se_from_prec : Standard errors from precision matrix
     calculate_corr_from_cov : Correlation matrix from covariance matrix
-    calculate_cov_from_inf : Covariance matrix from information matrix
+    calculate_cov_from_prec : Covariance matrix from precision matrix
     calculate_cov_from_corrse : Covariance matrix from correlation matrix and standard errors
-    calculate_inf_from_corrse : Information matrix from correlation matrix and standard errors
-    calculate_corr_from_inf : Correlation matrix from information matrix
+    calculate_prec_from_corrse : Precision matrix from correlation matrix and standard errors
+    calculate_corr_from_prec : Correlation matrix from precision matrix
     """
 
-    Im = pd.DataFrame(np.linalg.inv(cov.values), index=cov.index, columns=cov.columns)
-    return Im
+    Pm = pd.DataFrame(np.linalg.inv(cov.values), index=cov.index, columns=cov.columns)
+    return Pm
 
 
-def calculate_inf_from_corrse(corr: pd.DataFrame, se: pd.Series):
-    """Calculate information matrix from a correlation matrix and standard errors
+def calculate_prec_from_corrse(corr: pd.DataFrame, se: pd.Series):
+    """Calculate precision matrix from a correlation matrix and standard errors
 
     Parameters
     ----------
     corr : pd.DataFrame
         Correlation matrix
     se : pd.Series
         Standard errors
 
     Return
     ------
     pd.DataFrame
-        Information matrix
+        Precision matrix
 
     Examples
     --------
-    >>> from pharmpy.modeling import load_example_model, calculate_inf_from_corrse
-    >>> model = load_example_model("pheno")
-    >>> corr = model.modelfit_results.correlation_matrix
-    >>> se = model.modelfit_results.standard_errors
+    >>> from pharmpy.modeling import calculate_prec_from_corrse
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> corr = results.correlation_matrix
+    >>> se = results.standard_errors
     >>> corr
                   PTVCL      PTVV   THETA_3      IVCL       IVV  SIGMA_1_1
     PTVCL      1.000000  0.007099 -0.094640 -0.388059  0.097981   0.170820
     PTVV       0.007099  1.000000 -0.356899  0.138062  0.356662   0.238441
     THETA_3   -0.094640 -0.356899  1.000000 -0.096515 -0.062991   0.153616
     IVCL      -0.388059  0.138062 -0.096515  1.000000 -0.185111   0.159170
     IVV        0.097981  0.356662 -0.062991 -0.185111  1.000000  -0.027495
     SIGMA_1_1  0.170820  0.238441  0.153616  0.159170 -0.027495   1.000000
-    >>> calculate_inf_from_corrse(corr, se)
+    >>> calculate_prec_from_corrse(corr, se)
                       PTVCL          PTVV       THETA_3           IVCL           IVV      SIGMA_1_1
     PTVCL      2.995565e+07  22660.041788  16057.848052  203511.410335 -39474.240358 -820116.179011
     PTVV       2.266004e+04   2129.908225    260.176399    -375.266263  -2800.818557   -7718.757955
     THETA_3    1.605785e+04    260.176399    187.038825     177.207512   -205.808434   -2225.144772
     IVCL       2.035114e+05   -375.266263    177.207512    7527.518562   2462.972906   -9977.457873
     IVV       -3.947424e+04  -2800.818557   -205.808434    2462.972906  22343.197906    9370.736254
     SIGMA_1_1 -8.201162e+05  -7718.757955  -2225.144772   -9977.457873   9370.736254  249846.006431
 
     See also
     --------
     calculate_se_from_cov : Standard errors from covariance matrix
-    calculate_se_from_inf : Standard errors from information matrix
+    calculate_se_from_prec : Standard errors from precision matrix
     calculate_corr_from_cov : Correlation matrix from covariance matrix
-    calculate_cov_from_inf : Covariance matrix from information matrix
+    calculate_cov_from_prec : Covariance matrix from precision matrix
     calculate_cov_from_corrse : Covariance matrix from correlation matrix and standard errors
-    calculate_inf_from_cov : Information matrix from covariance matrix
-    calculate_corr_from_inf : Correlation matrix from information matrix
+    calculate_prec_from_cov : Precision matrix from covariance matrix
+    calculate_corr_from_prec : Correlation matrix from precision matrix
     """
 
     sd_matrix = np.diag(se.values)
     cov = sd_matrix @ corr.values @ sd_matrix
-    Im = pd.DataFrame(np.linalg.inv(cov), index=corr.index, columns=corr.columns)
-    return Im
+    Pm = pd.DataFrame(np.linalg.inv(cov), index=corr.index, columns=corr.columns)
+    return Pm
 
 
-def calculate_corr_from_inf(information_matrix: pd.DataFrame):
-    """Calculate correlation matrix from an information matrix
+def calculate_corr_from_prec(precision_matrix: pd.DataFrame):
+    """Calculate correlation matrix from a precision matrix
 
     Parameters
     ----------
-    information_matrix : pd.DataFrame
-        Information matrix
+    precision_matrix : pd.DataFrame
+        Precision matrix
 
     Return
     ------
     pd.DataFrame
         Correlation matrix
 
     Examples
     --------
-    >>> from pharmpy.modeling import load_example_model, calculate_corr_from_inf
-    >>> model = load_example_model("pheno")
-    >>> inf = model.modelfit_results.information_matrix
-    >>> inf
+    >>> from pharmpy.modeling import calculate_corr_from_prec
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> prec = results.precision_matrix
+    >>> prec
                       PTVCL          PTVV       THETA_3           IVCL           IVV      SIGMA_1_1
     PTVCL      2.995567e+07  22660.028196  16057.855248  203511.614428 -39474.250514 -820118.299536
     PTVV       2.266003e+04   2129.904642    260.176234    -375.266233  -2800.816246   -7718.769557
     THETA_3    1.605786e+04    260.176234    187.038903     177.207683   -205.808480   -2225.150449
     IVCL       2.035116e+05   -375.266233    177.207683    7527.530027   2462.974821   -9977.488860
     IVV       -3.947425e+04  -2800.816246   -205.808480    2462.974821  22343.198618    9370.758371
     SIGMA_1_1 -8.201183e+05  -7718.769557  -2225.150449   -9977.488860   9370.758371  249847.177845
-    >>> calculate_corr_from_inf(inf)
+    >>> calculate_corr_from_prec(prec)
                   PTVCL      PTVV   THETA_3      IVCL       IVV  SIGMA_1_1
     PTVCL      1.000000  0.007099 -0.094640 -0.388059  0.097981   0.170820
     PTVV       0.007099  1.000000 -0.356899  0.138062  0.356662   0.238441
     THETA_3   -0.094640 -0.356899  1.000000 -0.096515 -0.062991   0.153616
     IVCL      -0.388059  0.138062 -0.096515  1.000000 -0.185111   0.159170
     IVV        0.097981  0.356662 -0.062991 -0.185111  1.000000  -0.027495
     SIGMA_1_1  0.170820  0.238441  0.153616  0.159170 -0.027495   1.000000
 
     See also
     --------
     calculate_se_from_cov : Standard errors from covariance matrix
-    calculate_se_from_inf : Standard errors from information matrix
+    calculate_se_from_prec : Standard errors from precision matrix
     calculate_corr_from_cov : Correlation matrix from covariance matrix
-    calculate_cov_from_inf : Covariance matrix from information matrix
+    calculate_cov_from_prec : Covariance matrix from precision matrix
     calculate_cov_from_corrse : Covariance matrix from correlation matrix and standard errors
-    calculate_inf_from_cov : Information matrix from covariance matrix
-    calculate_inf_from_corrse : Information matrix from correlation matrix and standard errors
+    calculate_prec_from_cov : Precision matrix from covariance matrix
+    calculate_prec_from_corrse : Precision matrix from correlation matrix and standard errors
     """
 
     corr = pd.DataFrame(
-        cov2corr(np.linalg.inv(information_matrix.values)),
-        index=information_matrix.index,
-        columns=information_matrix.columns,
+        cov2corr(np.linalg.inv(precision_matrix.values)),
+        index=precision_matrix.index,
+        columns=precision_matrix.columns,
     )
     return corr
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/metabolite.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/metabolite.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/odes.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/odes.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/parameter_sampling.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/parameter_sampling.py`

 * *Files 6% similar despite different names*

```diff
@@ -147,17 +147,19 @@
     -------
     pd.DataFrame
         samples
 
     Example
     -------
     >>> from pharmpy.modeling import create_rng, sample_parameters_uniformly, load_example_model
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
+    >>> results = load_example_modelfit_results("pheno")
     >>> rng = create_rng(23)
-    >>> pe = model.modelfit_results.parameter_estimates
+    >>> pe = results.parameter_estimates
     >>> sample_parameters_uniformly(model, pe, n=3, rng=rng)
           PTVCL      PTVV   THETA_3      IVCL       IVV  SIGMA_1_1
     0  0.004878  0.908216  0.149441  0.029179  0.025472   0.012947
     1  0.004828  1.014444  0.149958  0.028853  0.027653   0.013348
     2  0.004347  1.053837  0.165804  0.028465  0.026798   0.013727
 
     See also
@@ -217,18 +219,20 @@
     -------
     pd.DataFrame
         A dataframe with one sample per row
 
     Example
     -------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
+    >>> results = load_example_modelfit_results("pheno")
     >>> rng = create_rng(23)
-    >>> cov = model.modelfit_results.covariance_matrix
-    >>> pe = model.modelfit_results.parameter_estimates
+    >>> cov = results.covariance_matrix
+    >>> pe = results.parameter_estimates
     >>> sample_parameters_from_covariance_matrix(model, pe, cov, n=3, rng=rng)
           PTVCL      PTVV   THETA_3      IVCL       IVV  SIGMA_1_1
     0  0.005069  0.974989  0.204629  0.024756  0.012088   0.012943
     1  0.004690  0.958431  0.233231  0.038866  0.029000   0.012516
     2  0.004902  0.950778  0.128388  0.019020  0.023866   0.013413
 
     See also
@@ -287,19 +291,21 @@
     Returns
     -------
     pd.DataFrame
         Pool of samples in a DataFrame
 
     Example
     -------
-    >>> from pharmpy.modeling import *
+    >>> from pharmpy.modeling import create_rng, load_example_model, sample_individual_estimates
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
+    >>> results = load_example_modelfit_results("pheno")
     >>> rng = create_rng(23)
-    >>> ie = model.modelfit_results.individual_estimates
-    >>> iec = model.modelfit_results.individual_estimates_covariance
+    >>> ie = results.individual_estimates
+    >>> iec = results.individual_estimates_covariance
     >>> sample_individual_estimates(model, ie, iec, samples_per_id=2, rng=rng)
                   ETA_1     ETA_2
     ID sample
     1  0      -0.127941  0.037273
        1      -0.065492 -0.182851
     2  0      -0.263323 -0.265849
        1      -0.295883 -0.060346
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/parameters.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/plots.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/plots.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/remove_iiv.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/remove_iiv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/remove_iov.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/remove_iov.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/results.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/results.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,17 +50,19 @@
     ------
     Series
         Shrinkage for each eta
 
     Examples
     --------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> pe = model.modelfit_results.parameter_estimates
-    >>> ie = model.modelfit_results.individual_estimates
+    >>> results = load_example_modelfit_results("pheno")
+    >>> pe = results.parameter_estimates
+    >>> ie = results.individual_estimates
     >>> calculate_eta_shrinkage(model, pe, ie)
     ETA_1    0.720481
     ETA_2    0.240295
     dtype: float64
     >>> calculate_eta_shrinkage(model, pe, ie, sd=True)
     ETA_1    0.471305
     ETA_2    0.128389
@@ -105,17 +107,19 @@
     ------
     DataFrame
         Shrinkage for each eta and individual
 
     Examples
     --------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> pe = model.modelfit_results.parameter_estimates
-    >>> covs = model.modelfit_results.individual_estimates_covariance
+    >>> results = load_example_modelfit_results("pheno")
+    >>> pe = results.parameter_estimates
+    >>> covs = results.individual_estimates_covariance
     >>> calculate_individual_shrinkage(model, pe, covs)
            ETA_1     ETA_2
     ID
     1   0.847789  0.256473
     2   0.796643  0.210669
     3   0.755025  0.226957
     4   0.764541  0.216405
@@ -242,18 +246,20 @@
     pd.DataFrame
         A DataFrame of statistics indexed on parameter and covariate value.
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, create_rng
     >>> from pharmpy.modeling import calculate_individual_parameter_statistics
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
+    >>> results = load_example_modelfit_results("pheno")
     >>> rng = create_rng(23)
-    >>> pe = model.modelfit_results.parameter_estimates
-    >>> cov = model.modelfit_results.covariance_matrix
+    >>> pe = results.parameter_estimates
+    >>> cov = results.covariance_matrix
     >>> calculate_individual_parameter_statistics(model, "K=CL/V", pe, cov, rng=rng)
                               mean  variance    stderr
     parameter covariates
     K         p5          0.004234  0.000001  0.001138
               median      0.004907  0.000001  0.001247
               p95         0.004907  0.000001  0.001247
     """
@@ -414,18 +420,20 @@
     pd.DataFrame
         A DataFrame of statistics indexed on parameter and covariate value.
 
     Examples
     --------
     >>> from pharmpy.modeling import load_example_model, create_rng
     >>> from pharmpy.modeling import calculate_pk_parameters_statistics
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
+    >>> results = load_example_modelfit_results("pheno")
     >>> rng = create_rng(23)
-    >>> pe = model.modelfit_results.parameter_estimates
-    >>> cov = model.modelfit_results.covariance_matrix
+    >>> pe = results.parameter_estimates
+    >>> cov = results.covariance_matrix
     >>> calculate_pk_parameters_statistics(model, pe, cov, rng=rng)
                                   mean     variance     stderr
     parameter   covariates
     t_half_elim p5          173.337164  1769.493756  42.843398
                 median      149.567842  1317.474199  36.233070
                 p95         149.567842  1317.474199  36.233070
     k_e         p5            0.004234     0.000001   0.001138
@@ -591,16 +599,18 @@
     -------
     float
         BIC of model fit
 
     Examples
     --------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> ofv = model.modelfit_results.ofv
+    >>> results = load_example_modelfit_results("pheno")
+    >>> ofv = results.ofv
     >>> calculate_bic(model, ofv)
     611.7071686183284
     >>> calculate_bic(model, ofv, type='fixed')
     616.536606983396
     >>> calculate_bic(model, ofv, type='random')
     610.7412809453149
     >>> calculate_bic(model, ofv, type='iiv')
@@ -670,16 +680,18 @@
     -------
     pd.Series
         Correlation values indexed on pairs of parameters for (absolute) correlations above limit
 
     Example
     -------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> cor = model.modelfit_results.correlation_matrix
+    >>> results = load_example_modelfit_results("pheno")
+    >>> cor = results.correlation_matrix
     >>> check_high_correlations(model, cor, limit=0.3)
     PTVCL  IVCL      -0.388059
     PTVV   THETA_3   -0.356899
            IVV        0.356662
     dtype: float64
     """
     high_and_below_diagonal = cor.abs().ge(limit) & np.triu(np.ones(cor.shape), k=1).astype(bool)
@@ -706,16 +718,18 @@
     -------
     pd.Series
         Logical Series with same index as values
 
     Example
     -------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> check_parameters_near_bounds(model, model.modelfit_results.parameter_estimates)
+    >>> results = load_example_modelfit_results("pheno")
+    >>> check_parameters_near_bounds(model, results.parameter_estimates)
     PTVCL        False
     PTVV         False
     THETA_3      False
     IVCL         False
     IVV          False
     SIGMA_1_1    False
     dtype: bool
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/tmdd.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/tmdd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/units.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/units.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/update_inits.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/update_inits.py`

 * *Files 20% similar despite different names*

```diff
@@ -28,18 +28,20 @@
     -------
     Model
         Pharmpy model object
 
     Example
     -------
     >>> from pharmpy.modeling import load_example_model, update_inits
-    >>> model = load_example_model("pheno")   # This model was previously fitted to its data
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> model = load_example_model("pheno")
+    >>> results = load_example_modelfit_results("pheno")
     >>> model.parameters.inits  # doctest:+ELLIPSIS
     {'PTVCL': 0.00469307, 'PTVV': 1.00916, 'THETA_3': 0.1, 'IVCL': 0.0309626, 'IVV': 0.031128, 'SIGMA_1_1': 0.013241}
-    >>> model = update_inits(model, model.modelfit_results.parameter_estimates)
+    >>> model = update_inits(model, results.parameter_estimates)
     >>> model.parameters.inits  # doctest:+ELLIPSIS
     {'PTVCL': 0.00469555, 'PTVV': 0.984258, 'THETA_3': 0.15892, 'IVCL': 0.0293508, 'IVV': 0.027906, ...}
 
     """
     if move_est_close_to_bounds:
         parameter_estimates = _move_est_close_to_bounds(model, parameter_estimates)
 
@@ -101,16 +103,18 @@
     -------
     Model
         Pharmpy model object
 
     Example
     -------
     >>> from pharmpy.modeling import load_example_model, update_initial_individual_estimates
+    >>> from pharmpy.tools import load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> ie = model.modelfit_results.individual_estimates
+    >>> results = load_example_modelfit_results("pheno")
+    >>> ie = results.individual_estimates
     >>> model = update_initial_individual_estimates(model, ie)
     """
     if not force and model.initial_individual_estimates is None:
         return model
 
     model = model.replace(initial_individual_estimates=individual_estimates)
     return model.update_source()
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/modeling/write_csv.py` & `pharmpy-core-0.96.0/src/pharmpy/modeling/write_csv.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/fcon/model.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/fcon/model.py`

 * *Files 20% similar despite different names*

```diff
@@ -24,52 +24,51 @@
 class FCONInternals:
     code: str = None
     path: Path = None
 
 
 class Model(BaseModel):
     def __init__(self, **kwargs):
-        super().__init__(
-            **kwargs,
-        )
-
-    def _parse_labels_and_formats(self):
-        in_labl = False
-        labels = []
-        lines = iter(self.internals.code.split('\n'))
-        for line in lines:
-            if line.startswith('LABL'):
-                in_labl = True
-            if in_labl:
-                stripped = line[4:].replace(' ', '')
-                if stripped.startswith(','):
-                    in_labl = False
-                else:
-                    a = stripped.split(',')
-                    labels.extend(a)
-            if line.startswith('FORM'):
-                next_line = next(lines)
-                formats = next_line.strip()[1:-1].split(',')
-                break
-        else:
-            raise ModelSyntaxError("Problems parsing the FORM record in FCONS")
-
-        return labels, formats
-
-    @property
-    def dataset(self):
-        labels, formats = self._parse_labels_and_formats()
-        widths = []
-        for fmt in formats:
-            m = re.match(r'(\d+)\w(\d+)', fmt)
-            if not m:
-                raise ModelSyntaxError(f"Unrecognized Data format in FORM: {fmt}")
-            widths += [int(m.group(2))] * int(m.group(1))
-        df = pd.read_fwf(
-            self.internals.path.parent / 'FDATA', widths=widths, header=None, names=labels
-        )
-        return df
+        self._internals = kwargs['internals']
+        self._dataset = kwargs['dataset']
 
 
-def parse_code(code: str, path: Path, **kwargs):
+def _parse_labels_and_formats(code):
+    in_labl = False
+    labels = []
+    lines = iter(code.split('\n'))
+    for line in lines:
+        if line.startswith('LABL'):
+            in_labl = True
+        if in_labl:
+            stripped = line[4:].replace(' ', '')
+            if stripped.startswith(','):
+                in_labl = False
+            else:
+                a = stripped.split(',')
+                labels.extend(a)
+        if line.startswith('FORM'):
+            next_line = next(lines)
+            formats = next_line.strip()[1:-1].split(',')
+            break
+    else:
+        raise ModelSyntaxError("Problems parsing the FORM record in FCONS")
+
+    return labels, formats
+
+
+def parse_dataset(code, path):
+    labels, formats = _parse_labels_and_formats(code)
+    widths = []
+    for fmt in formats:
+        m = re.match(r'(\d+)\w(\d+)', fmt)
+        if not m:
+            raise ModelSyntaxError(f"Unrecognized Data format in FORM: {fmt}")
+        widths += [int(m.group(2))] * int(m.group(1))
+    df = pd.read_fwf(path.parent / 'FDATA', widths=widths, header=None, names=labels)
+    return df
+
+
+def parse_model(code: str, path: Path):
     internals = FCONInternals(code=code, path=path)
-    return Model(internals=internals, **kwargs)
+    dataset = parse_dataset(code, path)
+    return Model(internals=internals, dataset=dataset)
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/external/nlmixr/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pathlib
 
 import pharmpy.config as config
+from pharmpy.model.external.nlmixr import Model, convert_model
 
-from .model import Model, convert_model, execute_model, parse_modelfit_results, verification
+from .run import execute_model, parse_modelfit_results, verification
 
 r"""
 .. list-table:: Options for the nlmixr plugin
    :widths: 25 25 50 150
    :header-rows: 1
 
    * - Option name
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/error_model.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/error_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/ini.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/ini.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/model.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/external/nlmixr/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,416 +1,32 @@
 import json
 import os
 import subprocess
 import uuid
 import warnings
-from dataclasses import dataclass, replace
-from pathlib import Path, PosixPath
-from typing import Optional, Union
+from pathlib import Path
+from typing import Union
 
 import pharmpy.model
 from pharmpy.deps import pandas as pd
 from pharmpy.internals.code_generator import CodeGenerator
+from pharmpy.model.external.nlmixr import convert_model
+from pharmpy.model.external.nlmixr.model import add_evid
 from pharmpy.modeling import (
     append_estimation_step_options,
-    drop_columns,
-    get_evid,
     get_sigmas,
     get_thetas,
     set_evaluation_step,
-    translate_nmtran_time,
     update_inits,
     write_csv,
 )
 from pharmpy.results import ModelfitResults
 from pharmpy.tools import fit
 from pharmpy.workflows.log import Log
 
-from .error_model import res_error_term
-from .ini import add_eta, add_sigma, add_theta
-from .model_block import add_bioavailability, add_lag_times, add_ode, add_statements
-from .sanity_checks import check_model
-
-
-def convert_model(
-    model: pharmpy.model.Model,
-    keep_etas: bool = False,
-    skip_check: bool = False,
-    updated_estimates: bool = False,
-) -> pharmpy.model.Model:
-    """
-    Convert a NONMEM model into an nlmixr model
-
-    Parameters
-    ----------
-    model : pharmpy.model.Model
-        A NONMEM pharmpy model object
-    keep_etas : bool, optional
-        Decide if NONMEM estimated thetas are to be used. The default is False.
-    skip_check : bool, optional
-        Skip determination of error model type. Could speed up conversion. The default is False.
-
-    Returns
-    -------
-    pharmpy.model.Model
-        A model converted to nlmixr format.
-
-    """
-
-    if isinstance(model, Model):
-        return model
-
-    if updated_estimates:
-        model = update_inits(model, model.modelfit_results.parameter_estimates)
-
-    nlmixr_model = Model(
-        internals=NLMIXRModelInternals(),
-        parameters=model.parameters,
-        random_variables=model.random_variables,
-        statements=model.statements,
-        dependent_variables=model.dependent_variables,
-        estimation_steps=model.estimation_steps,
-        filename_extension='.R',
-        datainfo=model.datainfo,
-        dataset=model.dataset,
-        name=model.name,
-        description=model.description,
-    )
-
-    # Update dataset
-    if model.dataset is not None:
-        if keep_etas is True:
-            nlmixr_model = nlmixr_model.replace(
-                modelfit_results=ModelfitResults(
-                    individual_estimates=model.modelfit_results.individual_estimates
-                )
-            )
-            nlmixr_model = fixate_eta(nlmixr_model)
-
-        nlmixr_model = translate_nmtran_time(nlmixr_model)
-        # FIXME: dropping columns runs update source which becomes redundant.
-        # drop_dropped_columns(nlmixr_model)
-        if all(x in nlmixr_model.dataset.columns for x in ["RATE", "DUR"]):
-            nlmixr_model = drop_columns(nlmixr_model, ["DUR"])
-        nlmixr_model = nlmixr_model.replace(
-            datainfo=nlmixr_model.datainfo.replace(path=None),
-            dataset=nlmixr_model.dataset.reset_index(drop=True),
-        )
-
-        # Add evid
-        nlmixr_model = add_evid(nlmixr_model)
-
-    # Check model for warnings regarding data structure or model contents
-    nlmixr_model = check_model(nlmixr_model, skip_error_model_check=skip_check)
-
-    nlmixr_model.update_source()
-
-    return nlmixr_model
-
-
-def create_dataset(cg: CodeGenerator, model: pharmpy.model.Model, path=None) -> None:
-    """
-    Create dataset for nlmixr
-
-    Parameters
-    ----------
-    cg : CodeGenerator
-        A code object associated with the model.
-    model : pharmpy.model.Model
-        A pharmpy.model object.
-    path : TYPE, optional
-        Path to add file to. The default is None.
-
-    """
-    dataname = f'{model.name}.csv'
-    if path is None:
-        path = ""
-    path = Path(path) / dataname
-    cg.add(f'dataset <- read.csv("{path}")')
-
-
-def create_ini(cg: CodeGenerator, model: pharmpy.model.Model) -> None:
-    """
-    Create the nlmixr ini block code
-
-    Parameters
-    ----------
-    cg : CodeGenerator
-        A code object associated with the model.
-    model : pharmpy.model.Model
-        A pharmpy.model object.
-
-    """
-    cg.add('ini({')
-    cg.indent()
-
-    add_theta(model, cg)
-
-    add_eta(model, cg)
-
-    add_sigma(model, cg)
-
-    cg.dedent()
-    cg.add('})')
-
-
-def create_model(cg: CodeGenerator, model: pharmpy.model.Model) -> None:
-    """
-    Create the nlmixr model block code
-
-    Parameters
-    ----------
-    cg : CodeGenerator
-        A code object associated with the model.
-    model : pharmpy.model.Model
-        A pharmpy.model object.
-
-    """
-
-    cg.add('model({')
-
-    # Add statements before ODEs
-    cg.indent()
-    if len(model.statements.after_odes) != 0:
-        add_statements(model, cg, model.statements.before_odes)
-
-    # Add the ODEs
-    cg.add("")
-    cg.add("# --- DIFF EQUATIONS ---")
-    if model.statements.ode_system:
-        add_ode(model, cg)
-    cg.add("")
-
-    # Find what kind of error model we are looking at
-    dv = list(model.dependent_variables.keys())[0]
-    dv_statement = model.statements.find_assignment(dv)
-
-    only_piecewise = False
-    if dv_statement.expression.is_Piecewise:
-        only_piecewise = True
-        dependencies = set()
-        res_alias = set()
-        for s in model.statements.after_odes:
-            if s.symbol == dv:
-                if s.expression.is_Piecewise:
-                    for value, cond in s.expression.args:
-                        if value != dv:
-                            dv_term = res_error_term(model, value)
-                            dependencies.update(dv_term.dependencies())
-
-                            dv_term.create_res_alias()
-                            res_alias.update(dv_term.res_alias)
-                else:
-                    dv_term = res_error_term(model, s.expression)
-                    dependencies.update(dv_term.dependencies())
-
-                    dv_term.create_res_alias()
-                    res_alias.update(dv_term.res_alias)
-    else:
-        dv_term = res_error_term(model, dv_statement.expression)
-        dependencies = dv_term.dependencies()
-        dv_term.create_res_alias()
-        res_alias = dv_term.res_alias
-
-    # Add bioavailability statements
-    if model.statements.ode_system is not None:
-        add_bioavailability(model, cg)
-        add_lag_times(model, cg)
-
-    # Add statements after ODEs
-    if len(model.statements.after_odes) == 0:
-        statements = model.statements
-    else:
-        statements = model.statements.after_odes
-    add_statements(
-        model, cg, statements, only_piecewise, dependencies=dependencies, res_alias=res_alias
-    )
-
-    cg.dedent()
-    cg.add('})')
-
-
-def create_fit(cg: CodeGenerator, model: pharmpy.model.Model) -> None:
-    """
-    Create the call to fit for the nlmixr model with appropriate methods and datasets
-
-    Parameters
-    ----------
-    cg : CodeGenerator
-        A code object associated with the model.
-    model : pharmpy.model
-        A pharmpy.model.Model object.
-
-    """
-    # FIXME : rasie error if the method does not match when evaluating
-    estimation_steps = model.estimation_steps[0]
-    if "fix_eta" in estimation_steps.tool_options:
-        fix_eta = True
-    else:
-        fix_eta = False
-
-    if [s.evaluation for s in model.estimation_steps._steps][0] is True:
-        max_eval = 0
-    else:
-        max_eval = estimation_steps.maximum_evaluations
-
-    method = estimation_steps.method
-    interaction = estimation_steps.interaction
-
-    nonmem_method_to_nlmixr = {"FOCE": "foce", "FO": "fo", "SAEM": "saem"}
-
-    if method not in nonmem_method_to_nlmixr.keys():
-        nlmixr_method = "focei"
-    else:
-        nlmixr_method = nonmem_method_to_nlmixr[method]
-
-    if interaction and nlmixr_method != "saem":
-        nlmixr_method += "i"
-
-    if max_eval is not None:
-        if max_eval == 0 and nlmixr_method not in ["fo", "foi", "foce", "focei"]:
-            nlmixr_method = "posthoc"
-            cg.add(f'fit <- nlmixr2({model.name}, dataset, est = "{nlmixr_method}"')
-        else:
-            f = f'fit <- nlmixr2({model.name}, dataset, est = "{nlmixr_method}", '
-            if fix_eta:
-                f += f'control=foceiControl(maxOuterIterations={max_eval}, maxInnerIterations=0, etaMat = etas))'
-            else:
-                f += f'control=foceiControl(maxOuterIterations={max_eval}))'
-            cg.add(f)
-    else:
-        cg.add(f'fit <- nlmixr2({model.name}, dataset, est = "{nlmixr_method}")')
-
-
-def add_evid(model: pharmpy.model.Model) -> pharmpy.model.Model:
-    temp_model = model
-    if "EVID" not in temp_model.dataset.columns:
-        temp_model.dataset["EVID"] = get_evid(temp_model)
-    return temp_model
-
-
-@dataclass
-class NLMIXRModelInternals:
-    src: Optional[str] = None
-    path: Optional[Path] = None
-
-
-class Model(pharmpy.model.Model):
-    def __init__(self, **kwargs):
-        super().__init__(
-            **kwargs,
-        )
-
-    def update_source(self):
-        cg = CodeGenerator()
-        cg.add(f'{self.name} <- function() {{')
-        cg.indent()
-        create_ini(cg, self)
-        create_model(cg, self)
-        cg.dedent()
-        cg.add('}')
-        cg.empty_line()
-        create_fit(cg, self)
-        # Create lowercase id, time and amount symbols for nlmixr to be able
-        # to run
-        self.internals.src = str(cg).replace("AMT", "amt").replace("TIME", "time")
-        self.internals.path = None
-        code = str(cg).replace("AMT", "amt").replace("TIME", "time")
-        internals = replace(self.internals, src=code)
-        model = self.replace(internals=internals)
-        return model
-
-    @property
-    def model_code(self):
-        model = self.update_source()
-        code = model.internals.src
-        assert code is not None
-        return code
-
-
-def parse_modelfit_results(
-    model: pharmpy.model.Model, path: PosixPath
-) -> Union[None, ModelfitResults]:
-    """
-    Create ModelfitResults object for given model object taken from values saved in executed Rdata file
-
-    Parameters
-    ----------
-    model : pharmpy.model.Model
-        An nlmixr pharmpy model object.
-    path : PosixPath
-        A path to folder with model and data files.
-
-    Returns
-    -------
-    Union[None, ModelfitResults]
-        Either return ModelfitResult object or None if Rdata file not found.
-
-    """
-    rdata_path = path / (model.name + '.RDATA')
-    with warnings.catch_warnings():
-        # Supress a numpy deprecation warning
-        warnings.simplefilter("ignore")
-        import pyreadr
-    try:
-        rdata = pyreadr.read_r(rdata_path)
-    except (FileNotFoundError, OSError):
-        return None
-
-    rdata["thetas"] = rdata["thetas"].loc[get_thetas(model).names]
-    s = []
-    for sigma in get_sigmas(model):
-        if sigma.init != 1 and not sigma.fix:
-            s.append(sigma.name)
-    rdata["sigma"] = rdata["sigma"].loc[s]
-
-    ofv = rdata['ofv']['ofv'][0]
-    omegas_sigmas = {}
-    omega = model.random_variables.etas.covariance_matrix
-    for i in range(0, omega.rows):
-        for j in range(0, omega.cols):
-            symb = omega.row(i)[j]
-            if symb != 0:
-                omegas_sigmas[symb.name] = rdata['omega'].values[i, j]
-    sigma = model.random_variables.epsilons.covariance_matrix
-    for i in range(len(sigma)):
-        if sigma[i] != 0:
-            s = sigma[i]
-            if model.parameters[s].init != 1 and not model.parameters[s].fix:
-                omegas_sigmas[sigma[i].name] = rdata['sigma']['fit$theta'][sigma[i].name]
-    thetas_index = 0
-    pe = {}
-    for param in model.parameters:
-        if param.fix:
-            continue
-        elif param.name in omegas_sigmas:
-            pe[param.name] = omegas_sigmas[param.name]
-        else:
-            pe[param.name] = rdata['thetas']['fit$theta'][param.name]
-            thetas_index += 1
-
-    name = model.name
-    description = model.description
-    pe = pd.Series(pe)
-    predictions = rdata['pred'].set_index(["ID", "TIME"])
-    predictions.index = predictions.index.set_levels(
-        predictions.index.levels[0].astype("float64"), level=0
-    )
-
-    res = ModelfitResults(
-        name=name,
-        description=description,
-        ofv=ofv,
-        minimization_successful=True,  # FIXME: parse minimization status
-        parameter_estimates=pe,
-        predictions=predictions,
-        log=Log(),
-    )
-    return res
-
 
 def execute_model(model: pharmpy.model.Model, db: str, evaluate=False) -> pharmpy.model.Model:
     """
     Executes a model using nlmixr2 estimation.
 
     Parameters
     ----------
@@ -462,15 +78,15 @@
     cg.add(
         f'save(file="{path}/{model.name}.RDATA",ofv, thetas, omega, sigma, log_likelihood, runtime_total, pred)'
     )
     code += f'\n{str(cg)}'
     with open(path / f'{model.name}.R', 'w') as fh:
         fh.write(code)
 
-    from pharmpy.plugins.nlmixr import conf
+    from pharmpy.tools.external.nlmixr import conf
 
     rpath = conf.rpath / 'bin' / 'Rscript'
 
     newenv = os.environ
     # Reset environment variables incase started from R
     # and calling other R version.
     newenv['R_LIBS_USERS'] = ''
@@ -879,7 +495,86 @@
                 p2 = param2[p1.name]
                 diff = p1.init - p2.init
                 if abs(diff) > tol:
                     failed.append((p1.name, diff))
                 else:
                     passed.append((p1.name, diff))
     return passed, failed
+
+
+def parse_modelfit_results(model: pharmpy.model.Model, path: Path) -> Union[None, ModelfitResults]:
+    """
+    Create ModelfitResults object for given model object taken from values saved in executed Rdata file
+
+    Parameters
+    ----------
+    model : pharmpy.model.Model
+        An nlmixr pharmpy model object.
+    path : Path
+        A path to folder with model and data files.
+
+    Returns
+    -------
+    Union[None, ModelfitResults]
+        Either return ModelfitResult object or None if Rdata file not found.
+
+    """
+    rdata_path = path / (model.name + '.RDATA')
+    with warnings.catch_warnings():
+        # Supress a numpy deprecation warning
+        warnings.simplefilter("ignore")
+        import pyreadr
+    try:
+        rdata = pyreadr.read_r(rdata_path)
+    except (FileNotFoundError, OSError):
+        return None
+
+    rdata["thetas"] = rdata["thetas"].loc[get_thetas(model).names]
+    s = []
+    for sigma in get_sigmas(model):
+        if sigma.init != 1 and not sigma.fix:
+            s.append(sigma.name)
+    rdata["sigma"] = rdata["sigma"].loc[s]
+
+    ofv = rdata['ofv']['ofv'][0]
+    omegas_sigmas = {}
+    omega = model.random_variables.etas.covariance_matrix
+    for i in range(0, omega.rows):
+        for j in range(0, omega.cols):
+            symb = omega.row(i)[j]
+            if symb != 0:
+                omegas_sigmas[symb.name] = rdata['omega'].values[i, j]
+    sigma = model.random_variables.epsilons.covariance_matrix
+    for i in range(len(sigma)):
+        if sigma[i] != 0:
+            s = sigma[i]
+            if model.parameters[s].init != 1 and not model.parameters[s].fix:
+                omegas_sigmas[sigma[i].name] = rdata['sigma']['fit$theta'][sigma[i].name]
+    thetas_index = 0
+    pe = {}
+    for param in model.parameters:
+        if param.fix:
+            continue
+        elif param.name in omegas_sigmas:
+            pe[param.name] = omegas_sigmas[param.name]
+        else:
+            pe[param.name] = rdata['thetas']['fit$theta'][param.name]
+            thetas_index += 1
+
+    name = model.name
+    description = model.description
+    pe = pd.Series(pe)
+    predictions = rdata['pred'].set_index(["ID", "TIME"])
+    predictions.index = predictions.index.set_levels(
+        predictions.index.levels[0].astype("float64"), level=0
+    )
+
+    res = ModelfitResults(
+        name=name,
+        description=description,
+        ofv=ofv,
+        minimization_successful=True,  # FIXME: parse minimization status
+        parameter_estimates=pe,
+        predictions=predictions,
+        log=Log(),
+    )
+    return res
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/model_block.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/model_block.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nlmixr/sanity_checks.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nlmixr/sanity_checks.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 from .config import NONMEMConfiguration, conf
-from .detect import detect_model
-from .model import Model, convert_model, parse_code
 from .results import parse_modelfit_results
 
 r"""
 .. list-table:: Options for the nonmem plugin
    :widths: 25 25 50 150
    :header-rows: 1
 
@@ -24,15 +22,11 @@
    * - ``write_etas_in_abbr``
      - ``False``
      - bool
      - Whether to write etas as $ABBR records
 """
 
 __all__ = (
-    'parse_code',
-    'detect_model',
-    'convert_model',
     'parse_modelfit_results',
-    'Model',
     'conf',
     'NONMEMConfiguration',
 )
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/advan.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/advan.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/config.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/config.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/dataset.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/dataset.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/model.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/model.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     parse_description,
     parse_estimation_steps,
     parse_initial_individual_estimates,
     parse_parameters,
     parse_statements,
     parse_value_type,
 )
-from .results import _parse_modelfit_results
 from .update import (
     abbr_translation,
     create_name_map,
     update_ccontra,
     update_description,
     update_estimation,
     update_initial_individual_estimates,
@@ -82,15 +81,15 @@
     code += '$DATA file.csv IGNORE=@\n'
     if model.statements.ode_system is None:
         code += '$PRED\nY=X\n'
     else:
         code += '$SUBROUTINES ADVAN1 TRANS2\n'
         code += '$PK\nY=X\n'
         code += '$ERROR\nA=B\n'
-    nm_model = parse_code(code, dataset=model.dataset)
+    nm_model = parse_model(code, dataset=model.dataset)
     assert isinstance(nm_model, Model)
     nm_model._datainfo = model.datainfo
     nm_model._parameters = model.parameters
     nm_model._dataset = model.dataset
     nm_model._estimation_steps = model.estimation_steps
     nm_model._initial_individual_estimates = model.initial_individual_estimates
     # FIXME: This is handled equivalently to dependent variables, should handle multiple DVs
@@ -296,15 +295,17 @@
 
     def read_raw_dataset(self, parse_columns: Tuple[str, ...] = ()):
         return parse_dataset(
             self.datainfo, self.internals.control_stream, raw=True, parse_columns=parse_columns
         )
 
 
-def parse_code(code: str, path: Optional[Path] = None, dataset: Optional[pd.DataFrame] = None, **_):
+def parse_model(
+    code: str, path: Optional[Path] = None, dataset: Optional[pd.DataFrame] = None, **_
+):
     parser = NMTranParser()
     if path is None:
         name = 'run1'
         filename_extension = '.ctl'
     else:
         name = path.stem
         filename_extension = path.suffix
@@ -348,30 +349,14 @@
 
     init_etas = parse_initial_individual_estimates(
         control_stream, name_map, None if path is None else path.parent
     )
 
     value_type = parse_value_type(control_stream, statements)
 
-    modelfit_results = _parse_modelfit_results(
-        path,
-        control_stream,
-        name_map,
-        BaseModel(  # FIXME This should not be necessary
-            name=name,
-            description=description,
-            parameters=parameters,
-            random_variables=rvs,
-            statements=statements,
-            dependent_variables=dependent_variables,
-            observation_transformation=obs_trans,
-            estimation_steps=estimation_steps,
-        ),
-    )
-
     internals = NONMEMModelInternals(
         control_stream=control_stream,
         old_name=name,
         old_description=description,
         old_estimation_steps=estimation_steps,
         old_observation_transformation=obs_trans,
         old_parameters=parameters,
@@ -389,15 +374,14 @@
         parameters=parameters,
         random_variables=rvs,
         statements=statements,
         dataset=dataset,
         datainfo=di,
         dependent_variables=dependent_variables,
         estimation_steps=estimation_steps,
-        modelfit_results=modelfit_results,
         parent_model=None,
         initial_individual_estimates=init_etas,
         filename_extension=filename_extension,
         value_type=value_type,
         description=description,
         internals=internals,
     )
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/nmtran_parser.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/nmtran_parser.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/parsing.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/parsing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import warnings
 from pathlib import Path
 from typing import Callable, Dict, Optional, Tuple
 
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
 from pharmpy.internals.fs.path import path_absolute
+from pharmpy.internals.immutable import frozenmapping
 from pharmpy.internals.math import triangular_root
 from pharmpy.model import (
     Assignment,
     ColumnInfo,
     DataInfo,
     DatasetError,
     EstimationStep,
@@ -20,19 +21,19 @@
     NormalDistribution,
     ODESystem,
     Parameter,
     Parameters,
     RandomVariables,
     Statements,
 )
-from pharmpy.plugins.nonmem.table import NONMEMTableFile, PhiTable
 
 from .advan import _compartmental_model, des_assign_statements
 from .dataset import read_nonmem_dataset
 from .nmtran_parser import NMTranControlStream
+from .table import NONMEMTableFile, PhiTable
 
 
 def parse_thetas(control_stream):
     names = []
     bounds = []
     inits = []
     fixs = []
@@ -264,31 +265,31 @@
 
 
 def convert_dvs(statements, control_stream):
     # Conversion of IF (DVID.EQ.n) THEN to non-piecewise
     # could partly be done in code_record
     after = statements.error
     kept = []
-    dvs = {sympy.Symbol('Y'): 1}
-    obs_trans = {sympy.Symbol('Y'): sympy.Symbol('Y')}
+    dvs = frozenmapping({sympy.Symbol('Y'): 1})
+    obs_trans = frozenmapping({sympy.Symbol('Y'): sympy.Symbol('Y')})
     change = False
     yind = after.find_assignment_index('Y')
     if yind is None:
         return statements, dvs, obs_trans
     yind = yind - 1
     for s in after:
         expr = s.expression
         if isinstance(expr, sympy.Piecewise) and sympy.Symbol("DVID") in expr.free_symbols:
             cond = expr.args[0][1]
             if cond.lhs == sympy.Symbol("DVID") and cond.rhs == 1:
                 ass1 = s.replace(symbol=sympy.Symbol('Y_1'), expression=expr.args[0][0])
                 ass2 = s.replace(symbol=sympy.Symbol('Y_2'), expression=expr.args[1][0])
                 kept.append(ass1)
                 kept.append(ass2)
-                dvs = {sympy.Symbol('Y_1'): 1, sympy.Symbol('Y_2'): 2}
+                dvs = frozenmapping({sympy.Symbol('Y_1'): 1, sympy.Symbol('Y_2'): 2})
                 obs_trans = {sympy.Symbol('Y_1'): sympy.Symbol('Y_1')}
                 change = True
                 continue
         kept.append(s)
     after = Statements(tuple(kept))
     if statements.ode_system is not None:
         statements = statements.before_odes + statements.ode_system + after
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/abbreviated_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/abbreviated_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/code_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/code_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     PZR,
 )
 from pharmpy.internals.expr.subs import subs
 from pharmpy.internals.parse import AttrTree, NoSuchRuleException
 from pharmpy.internals.parse.tree import Interpreter
 from pharmpy.internals.sequence.lcs import diff
 from pharmpy.model import Assignment, Statement, Statements
-from pharmpy.plugins.nonmem.records.parsers import CodeRecordParser
 
+from .parsers import CodeRecordParser
 from .record import Record
 
 
 class NMTranPrinter(sympy_printing.str.StrPrinter):
     _operators = {
         'not': '.NOT. ',
     }
@@ -721,15 +721,15 @@
                             )
                             symbols.add(symbol)
                     piecewise_logic = True
                     if len(blocks) == 1 and len(blocks[0][1]) == 0:
                         # Special case for empty if
                         piecewise_logic = sympy.Not(blocks[0][0])
                     blocks.append((piecewise_logic, else_symb_exprs))
-
+                s_block = []
                 for symbol in symbols:
                     pairs = []
                     for block in blocks:
                         logic = block[0]
                         for cursymb, expr in block[1]:
                             if cursymb == symbol:
                                 pairs.append((expr, logic))
@@ -744,17 +744,17 @@
 
                     if len(pairs) == 1:
                         expr = pairs[0][0]
                         ass = Assignment(symbol, expr)
                     else:
                         pw = sympy.Piecewise(*pairs)
                         ass = Assignment(symbol, pw)
-                    s.append(ass)
+                    s_block.append(ass)
 
-                s = _reorder_block_statements(s)
+                s.extend(_reorder_block_statements(s_block))
                 curind = (child_index, child_index + 1, len(s) - len(symbols), len(s))
                 new_index.append(curind)
 
     return new_index, Statements(s)
 
 
 def _reorder_block_statements(s):
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/data_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/data_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/factory.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/code_record.lark` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/code_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/data_record.lark` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/data_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/model_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/omega_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/omega_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/option_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/option_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/parsers.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/parsers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/problem_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/problem_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/sizes_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/sizes_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/subroutine_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/subroutine_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/table_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/table_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/records/theta_record.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/records/theta_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 from pathlib import Path
 from typing import Dict, Optional, Union
 
 import pharmpy.modeling as modeling
 from pharmpy.deps import numpy as np
 from pharmpy.deps import pandas as pd
 from pharmpy.model import EstimationSteps, Model, Parameters, RandomVariables
+from pharmpy.model.external.nonmem.nmtran_parser import NMTranControlStream
+from pharmpy.model.external.nonmem.parsing import parse_table_columns
+from pharmpy.model.external.nonmem.table import ExtTable, NONMEMTableFile, PhiTable
+from pharmpy.model.external.nonmem.update import create_name_map
 from pharmpy.results import ModelfitResults
 from pharmpy.workflows.log import Log
 
-from .nmtran_parser import NMTranControlStream
-from .parsing import parse_table_columns
 from .results_file import NONMEMResultsFile
-from .table import ExtTable, NONMEMTableFile, PhiTable
-from .update import create_name_map
 
 
 def _parse_modelfit_results(
     path: Optional[Union[str, Path]],
     control_stream: NMTranControlStream,
     name_map,
     model: Model,
@@ -125,15 +125,15 @@
         relative_standard_errors=rse,
         individual_estimates=ie,
         individual_estimates_covariance=iec,
         runtime_total=runtime_total,
         log_likelihood=log_likelihood,
         covariance_matrix=cov,
         correlation_matrix=cor,
-        information_matrix=coi,
+        precision_matrix=coi,
         standard_errors=ses,
         standard_errors_sdcorr=ses_sdcorr,
         individual_ofv=iofv,
         parameter_estimates=final_pe,
         parameter_estimates_sdcorr=sdcorr,
         parameter_estimates_iterations=pe_iterations,
         ofv=final_ofv,
@@ -147,30 +147,30 @@
 
 
 def calculate_cov_cor_coi_ses(cov, cor, coi, ses):
     if cov is None:
         if cor is not None:
             cov = modeling.calculate_cov_from_corrse(cor, ses)
         elif coi is not None:
-            cov = modeling.calculate_cov_from_inf(coi)
+            cov = modeling.calculate_cov_from_prec(coi)
     if cor is None:
         if cov is not None:
             cor = modeling.calculate_corr_from_cov(cov)
         elif coi is not None:
-            cor = modeling.calculate_corr_from_inf(coi)
+            cor = modeling.calculate_corr_from_prec(coi)
     if coi is None:
         if cov is not None:
-            coi = modeling.calculate_inf_from_cov(cov)
+            coi = modeling.calculate_prec_from_cov(cov)
         elif cor is not None:
-            coi = modeling.calculate_inf_from_corrse(cor, ses)
+            coi = modeling.calculate_prec_from_corrse(cor, ses)
     if ses is None:
         if cov is not None:
             ses = modeling.calculate_se_from_cov(cov)
         elif coi is not None:
-            ses = modeling.calculate_se_from_inf(coi)
+            ses = modeling.calculate_se_from_prec(coi)
     return cov, cor, coi, ses
 
 
 def _parse_matrix(
     path: Path,
     control_stream: NMTranControlStream,
     name_map,
@@ -583,15 +583,15 @@
     sdcorr_ses = sdcorr_ses.rename(index=name_map)
     return ses, sdcorr_ses
 
 
 def _parse_evaluation(estimation_steps: EstimationSteps):
     index = list(range(1, len(estimation_steps) + 1))
     evaluation = [est.evaluation for est in estimation_steps]
-    return pd.Series(evaluation, index=index, name='evaluation')
+    return pd.Series(evaluation, index=index, name='evaluation', dtype='float64')
 
 
 def _get_fixed_parameters(table: ExtTable, parameters: Parameters, pe_translation: Dict):
     try:
         return table.fixed
     except KeyError:
         # NM 7.2 does not have row -1000000006 indicating FIXED status
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/results_file.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/results_file.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/run.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/external/nonmem/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,18 @@
 import time
 import uuid
 import warnings
 from itertools import repeat
 from pathlib import Path
 
 from pharmpy.model import EstimationSteps
+from pharmpy.model.external.nonmem import convert_model
+from pharmpy.model.external.nonmem.records.factory import create_record
 from pharmpy.modeling import write_csv, write_model
-from pharmpy.plugins.nonmem import conf, convert_model, parse_modelfit_results
-
-from .records.factory import create_record
+from pharmpy.tools.external.nonmem import conf, parse_modelfit_results
 
 PARENT_DIR = f'..{os.path.sep}'
 
 
 def execute_model(model, db):
     database = db.model_database
     parent_model = model.parent_model
@@ -131,15 +131,15 @@
         plugin_path = model_path / 'nonmem.json'
         with open(plugin_path, 'w') as f:
             json.dump(plugin, f, indent=2)
 
         txn.store_local_file(plugin_path)
 
         txn.store_metadata(metadata)
-        if len(model.estimation_steps) > 0:
+        if len(model.estimation_steps) > 0 or True:
             txn.store_modelfit_results()
 
             # Read in results for the server side
             model = model.replace(
                 modelfit_results=parse_modelfit_results(model, model_path / basename)
             )
 
@@ -196,18 +196,18 @@
 
     design_code = '$DESIGN APPROX=FOCEI MODE=1 NELDER FIMDIAG=0 DATASIM=1 GROUPSIZE=32 OFVTYPE=0'
     design_record = create_record(design_code)
     stream = stream.insert_record(design_record)
     internals = model.internals.replace(control_stream=stream)
     model = model.replace(internals=internals)
 
-    execute_model(model, context)
+    model = execute_model(model, context)
 
     from pharmpy.tools.evaldesign import EvalDesignResults
 
     mfr = model.modelfit_results
     res = EvalDesignResults(
         ofv=mfr.ofv,
         individual_ofv=mfr.individual_ofv,
-        information_matrix=mfr.information_matrix,
+        information_matrix=mfr.precision_matrix,
     )
     return res
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/table.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/table.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/nonmem/update.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/nonmem/update.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     Parameters,
     RandomVariables,
     Statements,
     data,
     output,
 )
 from pharmpy.modeling import get_ids, simplify_expression
-from pharmpy.plugins.nonmem.records.parsers import CodeRecordParser
+
+from .records.parsers import CodeRecordParser
 
 if TYPE_CHECKING:
     from .model import Model
 
 from .nmtran_parser import NMTranControlStream
 from .parsing import parse_column_info
 from .records import code_record
@@ -900,24 +901,34 @@
     return model
 
 
 def match_advan1(odes):
     return len(odes) == 1
 
 
-def match_advan2(odes):
+def match_advan2(statements):
+    odes = statements.ode_system
     if len(odes) != 2:
         return False
     dosing = odes.dosing_compartment
     outflows = odes.get_compartment_outflows(dosing)
     if len(outflows) != 1:
         return False
     central = outflows[0][0]
     central_rate = outflows[0][1]
-    if {sympy.Symbol('CL'), sympy.Symbol('V')} & central_rate.free_symbols:
+
+    # Check if rate is depending on CL or V assignments
+    dep_assigns = set()
+    expr = central_rate
+    for s in reversed(statements.before_odes):
+        if s.symbol in expr.free_symbols:
+            dep_assigns.add(s.symbol)
+            expr = expr.subs(s.symbol, s.expression)
+
+    if {sympy.Symbol('CL'), sympy.Symbol('V')} & dep_assigns:
         # Cannot use reserved symbols
         return False
     central_outflows = odes.get_compartment_outflows(central)
     if len(central_outflows) != 1:
         return False
     return True
 
@@ -997,15 +1008,15 @@
     odes = model.statements.ode_system
     nonlin = is_nonlinear_odes(model)
     has_zo = has_zero_order_inputs(model)
     if nonlin or has_zo:
         advan = 'ADVAN13'
     elif match_advan1(odes):
         advan = 'ADVAN1'
-    elif match_advan2(odes):
+    elif match_advan2(model.statements):
         advan = 'ADVAN2'
     elif match_advan3(odes):
         advan = 'ADVAN3'
     elif match_advan4(odes):
         advan = 'ADVAN4'
     elif match_advan11(odes):
         advan = 'ADVAN11'
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/external/rxode/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import pathlib
 
 import pharmpy.config as config
+from pharmpy.model.external.rxode import Model, convert_model
 
-from .model import Model, convert_model, execute_model, parse_modelfit_results, verification
+from .run import execute_model, parse_modelfit_results, verification
 
 r"""
 .. list-table:: Options for the nlmixr plugin
    :widths: 25 25 50 150
    :header-rows: 1
 
    * - Option name
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/rxode/model.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/model_database/local_directory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,443 +1,331 @@
 import json
-import os
-import subprocess
-import uuid
-import warnings
-from dataclasses import dataclass, replace
-from pathlib import Path, PosixPath
-from typing import Optional, Union
-
-import pharmpy.model
-from pharmpy.deps import pandas as pd
-from pharmpy.deps import sympy
-from pharmpy.internals.code_generator import CodeGenerator
-from pharmpy.modeling import (
-    drop_columns,
-    get_bioavailability,
-    get_lag_times,
-    get_omegas,
-    get_sigmas,
-    get_thetas,
-    translate_nmtran_time,
-    write_csv,
+import shutil
+from contextlib import contextmanager
+from os import stat
+from pathlib import Path
+from typing import Union
+
+from pharmpy.internals.df import hash_df_fs
+from pharmpy.internals.fs.lock import path_lock
+from pharmpy.internals.fs.path import path_absolute
+from pharmpy.model import DataInfo, Model
+from pharmpy.results import read_results
+
+from .baseclass import (
+    ModelSnapshot,
+    ModelTransaction,
+    NonTransactionalModelDatabase,
+    PendingTransactionError,
+    TransactionalModelDatabase,
 )
-from pharmpy.plugins.nlmixr.error_model import convert_eps_to_sigma
-from pharmpy.plugins.nlmixr.model import add_evid
-from pharmpy.plugins.nlmixr.model_block import (
-    add_bioavailability,
-    add_lag_times,
-    add_ode,
-    convert_eq,
-)
-from pharmpy.results import ModelfitResults
 
+DIRECTORY_PHARMPY_METADATA = '.pharmpy'
+DIRECTORY_DATASETS = '.datasets'
+DIRECTORY_INDEX = '.hash'
+FILE_METADATA = 'metadata.json'
+FILE_MODELFIT_RESULTS = 'results.json'
+FILE_PENDING = 'PENDING'
+FILE_LOCK = '.lock'
+
+
+def get_modelfit_results(model, path):
+    # FIXME: This is a workaround. The proper solution is to only read the results.json from
+    # the database. For this to work roundtrip of DataFrames in json is needed.
+    # This is currently broken because of rounding issue in pandas
+    # Also the modelfit_results attribute will soon be removed from model objects.
+    import pharmpy.model.external.nonmem as nonmem_model
+    import pharmpy.tools.external.nonmem as nonmem
 
-@dataclass
-class RxODEModelInternals:
-    src: Optional[str] = None
-    path: Optional[Path] = None
-
-
-class Model(pharmpy.model.Model):
-    def __init__(self, **kwargs):
-        super().__init__(
-            **kwargs,
-        )
-
-    def update_source(self):
-        cg = CodeGenerator()
-        cg.add(f'{self.name} <- rxode2({{')
-        cg.indent()
-        create_model(cg, self)
-        cg.dedent()
-        cg.add('})')
-        cg.empty_line()
-        create_theta(cg, self)
-        cg.empty_line()
-        create_eta(cg, self)
-        cg.empty_line()
-        create_sigma(cg, self)
-        cg.empty_line()
-        create_fit(cg, self)
-        self.internals.src = str(cg).replace("AMT", "amt").replace("TIME", "time")
-        self.internals.path = None
-        code = str(cg)
-        internals = replace(self.internals, src=code)
-        model = self.replace(internals=internals)
-        return model
+    if isinstance(model, nonmem_model.Model):
+        res = nonmem.parse_modelfit_results(model, path)
+    else:
+        import pharmpy.model.external.nlmixr as nlmixr_model
+        import pharmpy.tools.external.nlmixr as nlmixr
 
-    @property
-    def model_code(self):
-        model = self.update_source()
-        code = model.internals.src
-        assert code is not None
-        return code
+        assert isinstance(model, nlmixr_model.Model)
+        res = nlmixr.parse_modelfit_results(model, path)
 
+    model = model.replace(modelfit_results=res)
+    return model
 
-def execute_model(model: pharmpy.model.Model, db: str) -> pharmpy.model.Model:
-    """
-    Executes a model using rxode2.
+
+class LocalDirectoryDatabase(NonTransactionalModelDatabase):
+    """ModelDatabase implementation for single local directory
+
+    All files will be stored in the same directory. It is assumed that
+    all files connected to a model are named modelname + extension. This means that
+    care must be taken to keep filenames unique. Clashing filenames will
+    be overwritten. It is recommended to use the LocalModelDirectoryDatabase
+    instead.
 
     Parameters
     ----------
-    model : pharmpy.model.Model
-        An pharmpy model object.
-    db : str
-        Name of folder in home directory to store resulting files in.
-
-    Returns
-    -------
-    model : pharmpy.model.Model
-        Model with accompanied results.
-
+    path : str or Path
+        Path to the database directory. Will be created if it does not exist.
+    file_extension : str
+        File extension to use for model files.
     """
-    db = pharmpy.workflows.LocalDirectoryToolDatabase(db)
-    database = db.model_database
-    model = convert_model(model)
-    path = Path.cwd() / f'rxode_run_{model.name}-{uuid.uuid1()}'
-    model.internals.path = path
-    meta = path / '.pharmpy'
-    meta.mkdir(parents=True, exist_ok=True)
-    if model.datainfo.path is not None:
-        model = model.replace(datainfo=model.datainfo.replace(path=None))
-    write_csv(model, path=path)
-    model = model.replace(datainfo=model.datainfo.replace(path=path))
-
-    dataname = f'{model.name}.csv'
-    pre = f'library(rxode2)\n\nev <- read.csv("{path / dataname}")\n'
-
-    pre += "\n"
-
-    code = pre + model.model_code
-    cg = CodeGenerator()
-
-    dv = list(model.dependent_variables.keys())[0]
-    cg.add(f"res <- as.data.frame(fit[c('id', 'time', '{dv}')])")
-    cg.add("sigma <- as.data.frame(sigmas)")
-    cg.add("omegas <- as.data.frame(omegas)")
-    cg.add("params <- as.data.frame(fit$params)")
-
-    cg.add(f'save(file="{path}/{model.name}.RDATA", res, params)')
-
-    code += f'\n{str(cg)}'
-
-    with open(path / f'{model.name}.R', 'w') as fh:
-        fh.write(code)
-
-    from pharmpy.plugins.nlmixr import conf
-
-    rpath = conf.rpath / 'bin' / 'Rscript'
-
-    newenv = os.environ
-    # Reset environment variables incase started from R
-    # and calling other R version.
-    newenv['R_LIBS_USERS'] = ''
-    newenv['R_LIBS_SITE'] = ''
-
-    stdout = path / 'stdout'
-    stderr = path / 'stderr'
-
-    args = [str(rpath), str(path / (model.name + '.R'))]
 
-    with open(stdout, "wb") as out, open(stderr, "wb") as err:
-        result = subprocess.run(args, stdin=subprocess.DEVNULL, stderr=err, stdout=out, env=newenv)
-
-    rdata_path = path / f'{model.name}.RDATA'
-
-    metadata = {
-        'plugin': 'nlmixr',
-        'path': str(path),
-    }
+    def __init__(self, path='.', file_extension='.mod'):
+        path = Path(path)
+        path.mkdir(parents=True, exist_ok=True)
+        self.path = path_absolute(path)
+        self.file_extension = file_extension
+        self.ignored_names = frozenset(('stdout', 'stderr', 'nonmem.json', 'nlmixr.json'))
+
+    def store_model(self, model):
+        pass
+
+    def store_local_file(self, model, path, new_filename=None):
+        path_object = Path(path)
+        if path_object.name not in self.ignored_names and path_object.is_file():
+            dest_path = self.path
+            if new_filename:
+                dest_path = self.path / new_filename
+            shutil.copy2(path, dest_path)
+
+    def retrieve_local_files(self, name, destination_path):
+        # Retrieve all files stored for one model
+        files = self.path.glob(f'{name}.*')
+        for f in files:
+            shutil.copy2(f, destination_path)
+
+    def retrieve_file(self, name, filename):
+        # Return path to file
+        path = self.path / filename
+        if path.is_file() and stat(path).st_size > 0:
+            return path
+        else:
+            raise FileNotFoundError(f"Cannot retrieve {filename} for {name}")
 
-    plugin = {
-        'rpath': str(rpath),
-        'commands': [
-            {
-                'args': args,
-                'returncode': result.returncode,
-                'stdout': 'stdout',
-                'stderr': 'stderr',
-            }
-        ],
-    }
+    def retrieve_model(self, name):
+        filename = name + self.file_extension
+        path = self.path / filename
+        from pharmpy.model import Model
+
+        try:
+            model = Model.create_model(path)
+        except FileNotFoundError:
+            raise KeyError('Model cannot be found in database')
+        model = get_modelfit_results(model, self.path)
+        return model
 
-    with database.transaction(model) as txn:
-        txn.store_local_file(path / f'{model.name}.R')
-        txn.store_local_file(rdata_path)
+    def retrieve_modelfit_results(self, name):
+        return self.retrieve_model(name).modelfit_results
 
-        txn.store_local_file(stdout)
-        txn.store_local_file(stderr)
-        txn.store_local_file(path / f'{model.name}.csv')
+    def store_metadata(self, model, metadata):
+        pass
 
-        txn.store_local_file(model.datainfo.path)
+    def store_modelfit_results(self, model):
+        pass
 
-        plugin_path = path / 'nlmixr.json'
-        with open(plugin_path, 'w') as f:
-            json.dump(plugin, f, indent=2)
+    def __repr__(self):
+        return f"LocalDirectoryDatabase({self.path})"
 
-        txn.store_local_file(plugin_path)
 
-        txn.store_metadata(metadata)
-        txn.store_modelfit_results()
+class LocalModelDirectoryDatabase(TransactionalModelDatabase):
+    """ModelDatabase implementation for a local directory structure
 
-    res = parse_modelfit_results(model, path)
-    model = model.replace(modelfit_results=res)
-    return model
+    Files will be stored in separate subdirectories named after each model.
+    There are no restrictions on names of the files so models can have the same
+    name of some connected file without creating a name clash.
 
+    Parameters
+    ----------
+    path : str or Path
+        Path to the base database directory. Will be created if it does not exist.
+    file_extension : str
+        File extension to use for model files.
+    """
 
-def parse_modelfit_results(
-    model: pharmpy.model.Model, path: PosixPath
-) -> Union[None, ModelfitResults]:
-    rdata_path = path / (model.name + '.RDATA')
-    with warnings.catch_warnings():
-        # Supress a numpy deprecation warning
-        warnings.simplefilter("ignore")
-        import pyreadr
-    try:
-        rdata = pyreadr.read_r(rdata_path)
-    except (FileNotFoundError, OSError):
-        return None
-
-    dv = list(model.dependent_variables.keys())[0]
-    pred = rdata["res"][["id", "time", f"{dv}"]]
-    pred.rename(columns={f"{dv}": 'PRED', "id": "ID", "time": "TIME"}, inplace=True)
-    pred = pred.set_index(["ID", "TIME"])
-
-    # TODO : extract thetas, omegas and sigmas
-
-    predictions = pred
-    predictions.index = predictions.index.set_levels(
-        predictions.index.levels[0].astype("float64"), level=0
-    )
-
-    # TODO : Add more variables such as name and description and parameter estimates
-    res = ModelfitResults(predictions=predictions)
-    return res
-
-
-def verification(
-    model: pharmpy.model.Model,
-    db_name: str,
-    error: float = 10**-3,
-    return_comp: bool = False,
-    ignore_print=False,
-) -> Union[bool, pd.DataFrame]:
-    nonmem_model = model
-
-    from pharmpy.modeling import update_inits
-    from pharmpy.plugins.nlmixr.model import print_step
-    from pharmpy.tools import fit
-
-    # Save results from the nonmem model
-    if nonmem_model.modelfit_results is None:
-        if not ignore_print:
-            print_step("Calculating NONMEM predictions... (this might take a while)")
-        nonmem_model = nonmem_model.replace(modelfit_results=fit(nonmem_model))
-    else:
-        if nonmem_model.modelfit_results.predictions is None:
-            if not ignore_print:
-                print_step("Calculating NONMEM predictions... (this might take a while)")
-            nonmem_model = nonmem_model.replace(modelfit_results=fit(nonmem_model))
-
-    param_estimates = nonmem_model.modelfit_results.parameter_estimates
-
-    omega_names = get_omegas(nonmem_model).names
-    for name in omega_names:
-        param_estimates[name] = 0
-
-    sigma_names = get_sigmas(model).names
-    for name in sigma_names:
-        param_estimates[name] = 0
-
-    # Update the nonmem model with new estimates
-    # and convert to nlmixr
-    if not ignore_print:
-        print_step("Converting NONMEM model to RxODE...")
-    rxode_model = convert_model(update_inits(nonmem_model, param_estimates))
-
-    # Execute the nlmixr model
-    if not ignore_print:
-        print_step("Executing RxODE model... (this might take a while)")
-
-    rxode_model = execute_model(rxode_model, db_name)
-
-    from pharmpy.plugins.nlmixr.model import compare_models
-
-    combined_result = compare_models(
-        nonmem_model, rxode_model, error=error, force_pred=True, ignore_print=ignore_print
-    )
-
-    if not ignore_print:
-        print_step("DONE")
-    if return_comp is True:
-        return combined_result
-    else:
-        if all(combined_result["PASS/FAIL"] == "PASS"):
-            return True
+    def __init__(self, path: Union[str, Path] = '.', file_extension='.mod'):
+        path = Path(path)
+        path.mkdir(parents=True, exist_ok=True)
+        self.path = path_absolute(path)
+        self.file_extension = file_extension
+
+    def _read_lock(self):
+        # NOTE Obtain shared (blocking) lock on the entire database
+        path = self.path / FILE_LOCK
+        path.touch(exist_ok=True)
+        return path_lock(str(path), shared=True)
+
+    def _write_lock(self):
+        # NOTE Obtain exclusive (blocking) lock on the entire database
+        path = self.path / FILE_LOCK
+        path.touch(exist_ok=True)
+        return path_lock(str(path), shared=False)
+
+    @contextmanager
+    def snapshot(self, model_name: str):
+        model_path = self.path / model_name
+        destination = model_path / DIRECTORY_PHARMPY_METADATA
+        destination.mkdir(parents=True, exist_ok=True)
+        with self._read_lock():
+            # NOTE Check that no pending transaction exists
+            path = destination / FILE_PENDING
+            if path.exists():
+                # TODO finish pending transaction from journal if possible
+                raise PendingTransactionError()
+
+            yield LocalModelDirectoryDatabaseSnapshot(self, model_name)
+
+    @contextmanager
+    def transaction(self, model: Model):
+        model_path = self.path / model.name
+        destination = model_path / DIRECTORY_PHARMPY_METADATA
+        destination.mkdir(parents=True, exist_ok=True)
+        with self._write_lock():
+            # NOTE Mark state as pending
+            path = destination / FILE_PENDING
+            try:
+                path.touch(exist_ok=False)
+            except FileExistsError:
+                # TODO finish pending transaction from journal if possible
+                raise PendingTransactionError()
+
+            yield LocalModelDirectoryDatabaseTransaction(self, model)
+
+            # NOTE Commit transaction (only if no exception was raised)
+            path.unlink()
+
+    def list_models(self):
+        model_dir_names = [p.name for p in self.path.glob('*') if not p.name.startswith('.')]
+        return sorted(model_dir_names)
+
+    def __repr__(self):
+        return f"LocalModelDirectoryDatabase({self.path})"
+
+
+class LocalModelDirectoryDatabaseTransaction(ModelTransaction):
+    def __init__(self, database: LocalModelDirectoryDatabase, model: Model):
+        self.db = database
+        self.model = model
+
+    def store_model(self):
+        from pharmpy.modeling import read_dataset_from_datainfo, write_csv, write_model
+
+        model = self.model
+        datasets_path = self.db.path / DIRECTORY_DATASETS
+
+        # NOTE Get the hash of the dataset and list filenames with contents
+        # matching this hash only
+        h = hash_df_fs(model.dataset)
+        h_dir = datasets_path / DIRECTORY_INDEX / h
+        h_dir.mkdir(parents=True, exist_ok=True)
+        for hpath in h_dir.iterdir():
+            # NOTE This variable holds a string similar to "run1.csv"
+            matching_model_filename = hpath.name
+            data_path = datasets_path / matching_model_filename
+            dipath = data_path.with_suffix('.datainfo')
+            # TODO Maybe catch FileNotFoundError and similar here (pass)
+            curdi = DataInfo.read_json(dipath)
+            # NOTE paths are not compared here
+            if curdi == model.datainfo:
+                df = read_dataset_from_datainfo(curdi)
+                if df.equals(model.dataset):
+                    # NOTE Update datainfo path
+                    datainfo = model.datainfo.replace(path=curdi.path)
+                    model = model.replace(datainfo=datainfo)
+                    break
         else:
-            return False
+            model_filename = model.name + '.csv'
 
-
-def convert_model(model, skip_check=False):
-    if isinstance(model, Model):
+            # NOTE Create the index file at .datasets/.hash/<hash>/<model_filename>
+            index_path = h_dir / model_filename
+            index_path.touch()
+
+            data_path = path_absolute(datasets_path / model_filename)
+            datainfo = model.datainfo.replace(path=data_path)
+            model = model.replace(datainfo=datainfo)
+            model = write_csv(model, path=data_path, force=True)
+
+            # NOTE Write datainfo last so that we are "sure" dataset is there
+            # if datainfo is there
+            model.datainfo.to_json(datasets_path / (model.name + '.datainfo'))
+
+        # NOTE Write the model
+        model_path = self.db.path / model.name
+        model_path.mkdir(exist_ok=True)
+        write_model(model, str(model_path / (model.name + model.filename_extension)), force=True)
         return model
 
-    rxode_model = Model(
-        internals=RxODEModelInternals(),
-        parameters=model.parameters,
-        random_variables=model.random_variables,
-        statements=model.statements,
-        dependent_variables=model.dependent_variables,
-        estimation_steps=model.estimation_steps,
-        filename_extension='.R',
-        datainfo=model.datainfo,
-        dataset=model.dataset,
-        name=model.name,
-        description=model.description,
-    )
-
-    # Update dataset
-    if model.dataset is not None:
-        rxode_model = translate_nmtran_time(rxode_model)
-
-        if all(x in rxode_model.dataset.columns for x in ["RATE", "DUR"]):
-            rxode_model = drop_columns(rxode_model, ["DUR"])
-        rxode_model = rxode_model.replace(
-            datainfo=rxode_model.datainfo.replace(path=None),
-            dataset=rxode_model.dataset.reset_index(drop=True),
-        )
-
-        # Add evid
-        rxode_model = add_evid(rxode_model)
-
-    # Check model for warnings regarding data structure or model contents
-    from pharmpy.plugins.nlmixr.sanity_checks import check_model
-
-    rxode_model = check_model(rxode_model, skip_error_model_check=skip_check)
-
-    rxode_model.update_source()
-
-    return rxode_model
-
-
-def create_model(cg, model):
-    add_true_statements(model, cg, model.statements.before_odes)
-
-    if model.statements.ode_system:
-        add_ode(model, cg)
-
-    # Add bioavailability statements
-    if model.statements.ode_system is not None:
-        add_bioavailability(model, cg)
-        add_lag_times(model, cg)
-
-    # Add statements after ODE
-    add_true_statements(model, cg, model.statements.after_odes)
-
-
-def add_true_statements(model, cg, statements):
-    for s in statements:
-        if model.statements.ode_system is not None and (
-            s.symbol in get_bioavailability(model).values()
-            or s.symbol in get_lag_times(model).values()
-        ):
-            pass
-        else:
-            expr = s.expression
-            expr = convert_eps_to_sigma(expr, model)
-            if expr.is_Piecewise:
-                add_piecewise(model, cg, s)
+    def store_local_file(self, path, new_filename=None):
+        if Path(path).is_file():
+            destination = self.db.path / self.model.name
+            destination.mkdir(parents=True, exist_ok=True)
+            if new_filename:
+                destination = destination / new_filename
+            shutil.copy2(path, destination)
+
+    def store_metadata(self, metadata):
+        destination = self.db.path / self.model.name / DIRECTORY_PHARMPY_METADATA
+        destination.mkdir(parents=True, exist_ok=True)
+        with open(destination / FILE_METADATA, 'w') as f:
+            json.dump(metadata, f, indent=2)
+
+    def store_modelfit_results(self):
+        destination = self.db.path / self.model.name / DIRECTORY_PHARMPY_METADATA
+        destination.mkdir(parents=True, exist_ok=True)
+
+        if self.model.modelfit_results:
+            self.model.modelfit_results.to_json(destination / FILE_MODELFIT_RESULTS)
+
+
+class LocalModelDirectoryDatabaseSnapshot(ModelSnapshot):
+    def __init__(self, database: LocalModelDirectoryDatabase, model_name: str):
+        self.db = database
+        self.name = model_name
+
+    def retrieve_local_files(self, destination_path):
+        path = self.db.path / self.name
+        files = path.glob('*')
+        for f in files:
+            if f.is_file():
+                shutil.copy2(f, destination_path)
             else:
-                cg.add(f'{s.symbol.name} <- {expr}')
-
+                shutil.copytree(f, Path(destination_path) / f.stem)
 
-def add_piecewise(model: pharmpy.model.Model, cg: CodeGenerator, s):
-    expr = s.expression
-    first = True
-    for value, cond in expr.args:
-        if cond is not sympy.S.true:
-            if cond.atoms(sympy.Eq):
-                cond = convert_eq(cond)
-            if first:
-                cg.add(f'if ({cond}) {{')
-                first = False
-            else:
-                cg.add(f'}} else if ({cond}) {{')
-        else:
-            cg.add('} else {')
-            if "NEWIND" in [t.name for t in expr.free_symbols] and value == 0:
-                largest_value = expr.args[0].expr
-                largest_cond = expr.args[0].cond
-                for value, cond in expr.args[1:]:
-                    if cond is not sympy.S.true:
-                        if cond.rhs > largest_cond.rhs:
-                            largest_value = value
-                            largest_cond = cond
-                        elif cond.rhs == largest_cond.rhs:
-                            if not isinstance(cond, sympy.LessThan) and isinstance(
-                                largest_cond, sympy.LessThan
-                            ):
-                                largest_value = value
-                                largest_cond = cond
-                value = largest_value
-        cg.indent()
-        value = convert_eps_to_sigma(value, model)
-        cg.add(f'{s.symbol.name} <- {value}')
-        cg.dedent()
-    cg.add('}')
-
-
-def create_theta(cg, model):
-    cg.add("thetas <-")
-    cg.add("c(")
-    thetas = get_thetas(model)
-    for n, theta in enumerate(thetas):
-        if n != len(thetas) - 1:
-            cg.add(f'{theta.name} = {theta.init}, ')
+    def retrieve_file(self, filename):
+        # Return path to file
+        path = self.db.path / self.name / filename
+        if path.is_file() and stat(path).st_size > 0:
+            return path
         else:
-            cg.add(f'{theta.name} = {theta.init}')
-    cg.add(")")
+            raise FileNotFoundError(f"Cannot retrieve {filename} for {self.name}")
 
-
-def create_eta(cg, model):
-    from pharmpy.plugins.nlmixr.ini import add_eta
-
-    cg.add("omegas = lotri(")
-    add_eta(model, cg, as_list=True)
-    cg.add(")")
-
-
-def create_sigma(cg, model):
-    cg.add("sigmas <-")
-    cg.add("lotri(")
-    all_eps = model.random_variables.epsilons
-    for n, eps in enumerate(all_eps):
-        sigma = eps.variance
-        if len(eps.names) == 1:
-            name = model.parameters[sigma].name
-            init = model.parameters[sigma].init
-            if n != len(all_eps) - 1:
-                cg.add(f'{name} ~ {init},')
-            else:
-                cg.add(f'{name} ~ {init}')
+    def retrieve_model(self):
+        extensions = ['.mod', '.ctl']
+        from pharmpy.model import Model
+
+        errors = []
+        root = self.db.path / self.name
+        for extension in extensions:
+            filename = self.name + extension
+            path = root / filename
+            try:
+                # NOTE this will guess the model type
+                model = Model.parse_model(path)
+                break
+            except FileNotFoundError as e:
+                errors.append(e)
+                pass
         else:
-            cg.add(f'{" + ".join([name for name in eps.names])} ~ c(')
-            inits = []
-            for row in range(sigma.rows):
-                for col in range(row + 1):
-                    if col == 0 and row != 0:
-                        cg.add(f'{", ".join([str(x) for x in inits])},')
-                        inits = []
-                        inits.append(f'{model.parameters[sigma[row, col].name].init}')
-                    else:
-                        inits.append(model.parameters[sigma[row, col].name].init)
-            cg.add(f'{", ".join([str(x) for x in inits])}')
-            if eps != model.random_variables.epsilons[-1]:
-                cg.add("),")
-            else:
-                cg.add(")")
-    cg.add(")")
+            raise KeyError(
+                f'Could not find {self.name} in {self.db}.'
+                f' Looked up {", ".join(map(lambda e: f"`{e.filename}`", errors))}.'
+            )
 
+        model = get_modelfit_results(model, path)
+        return model
 
-def create_fit(cg, model):
-    cg.add(f'fit <- {model.name} %>% rxSolve(thetas, ev, omega = omegas, sigma = sigmas)')
+    def retrieve_modelfit_results(self):
+        res = self.retrieve_model().modelfit_results
+        if res is not None:
+            return res
+
+        # FIXME The following does not work because deserialization of modelfit
+        # results is not generic enough. We only use it to make the resume_tool
+        # test pass.
+        path = self.db.path / self.name / DIRECTORY_PHARMPY_METADATA / FILE_MODELFIT_RESULTS
+        return read_results(path)
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/plugins/utils.py` & `pharmpy-core-0.96.0/src/pharmpy/model/external/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,40 @@
-"""Utils for managing plugins."""
+"""Utils for managing detecting and parsing of external model types."""
 
 from importlib import import_module
 from pathlib import Path
 from pkgutil import iter_modules
 
 
-class PluginError(Exception):
-    pass
-
-
 def detect_model(src):
     """Detects appropriate implementation from a source object
-    Return a plugin module
+    Return an external model module
     """
 
-    plugins = load_plugins()
-    detected_plugins = []
+    plugins = _load_external_modules()
+    detected_modules = []
     for module in plugins:
         if hasattr(module, 'detect_model'):
-            is_plugin = module.detect_model(src)
-            if is_plugin:
-                detected_plugins.append(module)
-
-    if len(detected_plugins) == 0:
-        raise PluginError(f"No support for model {src}")
-    elif len(detected_plugins) > 1:
-        raise PluginError(f"More than one model plugin supports model {src}")
+            is_module = module.detect_model(src)
+            if is_module:
+                detected_modules.append(module)
+
+    if len(detected_modules) == 0:
+        raise TypeError(f"No support for model {src}")
+    elif len(detected_modules) > 1:
+        raise TypeError(f"More than one external model module supports model {src}")
     else:
-        return detected_plugins[0]
+        return detected_modules[0]
 
 
-def load_plugins():
-    """Find and import all available plugins"""
-    plugin_path = Path(__file__).resolve().parent
+def _load_external_modules():
+    """Find and import all available external modules"""
+    path = Path(__file__).resolve().parent
 
     # str on path to workaround https://bugs.python.org/issue44061
-    plugin_path = str(plugin_path)
+    path = str(path)
 
     return [
         import_module(modname)
-        for _, modname, ispkg in iter_modules([plugin_path], 'pharmpy.plugins.')
+        for _, modname, ispkg in iter_modules([path], 'pharmpy.model.external.')
         if ispkg
     ]
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/reporting/altairplot.py` & `pharmpy-core-0.96.0/src/pharmpy/reporting/altairplot.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/reporting/custom.css` & `pharmpy-core-0.96.0/src/pharmpy/reporting/custom.css`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/reporting/reporting.py` & `pharmpy-core-0.96.0/src/pharmpy/reporting/reporting.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/results.py` & `pharmpy-core-0.96.0/src/pharmpy/results.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,16 +150,16 @@
         Name of model
     description : str
         Description of model
     correlation_matrix : pd.DataFrame
         Correlation matrix of the population parameter estimates
     covariance_matrix : pd.DataFrame
         Covariance matrix of the population parameter estimates
-    information_matrix : pd.DataFrame
-        Fischer information matrix of the population parameter estimates
+    precision_matrix : pd.DataFrame
+        Precision matrix of the population parameter estimates
     evaluation_ofv : float
         The objective function value as if the model was evaluated. Currently
         workfs for classical estimation methods by taking the OFV of the first
         iteration.
     individual_ofv : pd.Series
         OFV for each individual
     individual_estimates : pd.DataFrame
@@ -201,15 +201,15 @@
     ofv: Optional[float] = None
     ofv_iterations: Optional[pd.Series] = None
     parameter_estimates: Optional[pd.Series] = None
     parameter_estimates_sdcorr: Optional[pd.Series] = None
     parameter_estimates_iterations: Optional[pd.DataFrame] = None
     covariance_matrix: Optional[pd.DataFrame] = None
     correlation_matrix: Optional[pd.DataFrame] = None
-    information_matrix: Optional[pd.DataFrame] = None
+    precision_matrix: Optional[pd.DataFrame] = None
     standard_errors: Optional[pd.Series] = None
     standard_errors_sdcorr: Optional[pd.Series] = None
     relative_standard_errors: Optional[pd.Series] = None
     minimization_successful: Optional[bool] = None
     minimization_successful_iterations: Optional[pd.DataFrame] = None
     estimation_runtime: Optional[float] = None
     estimation_runtime_iterations: Optional[pd.DataFrame] = None
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from threading import Lock
 
 __all__ = (
     'create_report',  # pyright: ignore [reportUnsupportedDunderAll]
     'create_results',  # pyright: ignore [reportUnsupportedDunderAll]
     'fit',  # pyright: ignore [reportUnsupportedDunderAll]
+    'load_example_modelfit_results',  # pyright: ignore [reportUnsupportedDunderAll]
     'predict_influential_individuals',  # pyright: ignore [reportUnsupportedDunderAll]
     'predict_influential_outliers',  # pyright: ignore [reportUnsupportedDunderAll]
     'predict_outliers',  # pyright: ignore [reportUnsupportedDunderAll]
     'print_fit_summary',  # pyright: ignore [reportUnsupportedDunderAll]
     'rank_models',  # pyright: ignore [reportUnsupportedDunderAll]
     'read_results',  # pyright: ignore [reportUnsupportedDunderAll]
     'read_modelfit_results',  # pyright: ignore [reportUnsupportedDunderAll]
@@ -37,14 +38,15 @@
 
 _not_wrapped = {
     '.amd.run': ('run_amd',),
     '.reporting': ('create_report',),
     '.run': (
         'create_results',
         'fit',
+        'load_example_modelfit_results',
         'print_fit_summary',
         'rank_models',
         'read_modelfit_results',
         'read_results',
         'resume_tool',
         'retrieve_final_model',
         'retrieve_models',
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/allometry/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/allometry/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,17 +61,18 @@
     -------
     AllometryResults
         Allometry tool result object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import run_allometry, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> from pharmpy.tools import run_allometry # doctest: +SKIP
-    >>> run_allometry(model=model, results=model.modelfit_results, allometric_variable='WGT') # doctest: +SKIP
+    >>> results = load_example_modelfit_results("pheno")
+    >>> run_allometry(model=model, results=results, allometric_variable='WGT') # doctest: +SKIP
 
     """
 
     wf = Workflow()
     wf.name = "allometry"
     if model is not None:
         start_task = Task('start_allometry', start, model)
@@ -168,15 +169,15 @@
     best_model = start_model if allometry_model_failed else allometry_model
 
     summod_start = summarize_modelfit_results(start_model.modelfit_results)
     summod_allometry = summarize_modelfit_results(allometry_model.modelfit_results)
     summods = pd.concat([summod_start, summod_allometry], keys=[0, 1], names=['step'])
     suminds = summarize_individuals([start_model, allometry_model])
     sumcount = summarize_individuals_count_table(df=suminds)
-    sumerrs = summarize_errors([start_model, allometry_model])
+    sumerrs = summarize_errors([start_model.modelfit_results, allometry_model.modelfit_results])
 
     return AllometryResults(
         summary_models=summods,
         summary_individuals=suminds,
         summary_individuals_count=sumcount,
         summary_errors=sumerrs,
         final_model_name=best_model.name,
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/amd/funcs.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/amd/funcs.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,23 +16,25 @@
     NormalDistribution,
     Parameter,
     Parameters,
     RandomVariables,
     Statements,
     output,
 )
+
+# FIXME: This shouldn't be used here
+from pharmpy.model.external.nonmem.advan import dosing
 from pharmpy.modeling import (
     add_iiv,
     create_joint_distribution,
     set_first_order_absorption,
     set_initial_estimates,
     set_proportional_error_model,
 )
 from pharmpy.modeling.data import read_dataset_from_datainfo
-from pharmpy.plugins.nonmem.advan import dosing
 
 
 def create_start_model(dataset_path, modeltype='pk_oral', cl_init=0.01, vc_init=1.0, mat_init=0.1):
     dataset_path = Path(dataset_path)
     di = _create_default_datainfo(dataset_path)
     df = read_dataset_from_datainfo(di, datatype='nonmem')
 
@@ -66,15 +68,14 @@
 
     est = EstimationStep.create(
         "FOCE",
         interaction=True,
         maximum_evaluations=99999,
         predictions=['CIPREDI'],
         residuals=['CWRES'],
-        tool_options={'SADDLE_RESET': 1},
     )
     eststeps = EstimationSteps.create([est])
 
     model = Model(
         name='start',
         statements=stats,
         estimation_steps=eststeps,
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/amd/run.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/amd/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,25 +86,26 @@
     -------
     Model
         Reference to the same model object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import run_amd, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> from pharmpy.tools import run_amd # doctest: +SKIP
-    >>> run_amd(model, results=model.modelfit_results)      # doctest: +SKIP
+    >>> results = load_example_modelfit_results("pheno")
+    >>> run_amd(model, results=results)      # doctest: +SKIP
 
     See also
     --------
     run_iiv
     run_tool
 
     """
-    from pharmpy.plugins import nonmem  # FIXME We should not depend on NONMEM
+    from pharmpy.model.external import nonmem  # FIXME We should not depend on NONMEM
 
     if type(input) is str:
         from pharmpy.tools.amd.funcs import create_start_model
 
         model = create_start_model(
             input, modeltype=modeltype, cl_init=cl_init, vc_init=vc_init, mat_init=mat_init
         )
@@ -244,15 +245,15 @@
 
     if summary_individuals_count is None:
         warnings.warn(
             'AMDResults.summary_individuals_count is None because none of the tools yielded '
             'a summary.'
         )
 
-    summary_errors = summarize_errors(next_model)
+    summary_errors = summarize_errors(next_model.modelfit_results)
     res = AMDResults(
         final_model=next_model.name,
         summary_tool=summary_tool,
         summary_models=summary_models,
         summary_individuals_count=summary_individuals_count,
         summary_errors=summary_errors,
     )
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/report.rst` & `pharmpy-core-0.96.0/src/pharmpy/tools/bootstrap/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/bootstrap/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/bootstrap/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/bootstrap/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,18 +23,18 @@
     Returns
     -------
     BootstrapResults
         Bootstrap tool result object
 
     Examples
     --------
-    >>> from pharmpy.modeling import *
+    >>> from pharmpy.modeling import load_example_model
+    >>> from pharmpy.tools import run_bootstrap, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> from pharmpy.tools import run_bootstrap # doctest: +SKIP
-    >>> res = model.modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
     >>> run_bootstrap(model, res, resamples=500) # doctest: +SKIP
     """
 
     wf = Workflow()
     wf.name = 'bootstrap'
 
     for i in range(resamples):
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/cdd/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/cdd/results.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing import Any, Dict, List, Optional, Union
 
 from pharmpy.deps import numpy as np
 from pharmpy.deps import pandas as pd
 from pharmpy.deps.scipy import linalg
 from pharmpy.model import Model, Results
 from pharmpy.modeling import plot_individual_predictions
-from pharmpy.results import mfr
+from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.psn_helpers import model_paths, options_from_command
 
 
 @dataclass(frozen=True)
 class CDDResults(Results):
     """CDD Results class"""
 
@@ -38,22 +38,20 @@
         delta_matrix = cdd_estimates - base_estimate
         x = linalg.solve_triangular(chol, delta_matrix.transpose(), lower=islow, trans=1)
         return list(map(np.linalg.norm, x.transpose()))
     except Exception:
         return None
 
 
-def compute_delta_ofv(base_model: Model, cdd_models: List[Model], skipped_individuals):
-    iofv = mfr(base_model).individual_ofv
+def compute_delta_ofv(base_model_results, cdd_model_results, skipped_individuals):
+    iofv = base_model_results.individual_ofv
     if iofv is None:
-        return [np.nan] * len(cdd_models)
+        return [np.nan] * len(cdd_model_results)
 
-    cdd_ofvs = [
-        m.modelfit_results.ofv if m.modelfit_results is not None else np.nan for m in cdd_models
-    ]
+    cdd_ofvs = [res.ofv if res is not None else np.nan for res in cdd_model_results]
 
     # need to set dtype for index.difference to work
     skipped_indices = [
         pd.Index(np.array(skipped, dtype=iofv.index.dtype)) for skipped in skipped_individuals
     ]
 
     return [
@@ -64,103 +62,109 @@
 
 def compute_jackknife_covariance_matrix(cdd_estimates):
     bigN = len(cdd_estimates.index)
     delta_est = cdd_estimates - cdd_estimates.mean()
     return delta_est.transpose() @ delta_est * (bigN - 1) / bigN
 
 
-def compute_covariance_ratios(cdd_models, covariance_matrix):
+def compute_covariance_ratios(cdd_model_results, covariance_matrix):
     try:
         orig_det = np.linalg.det(covariance_matrix)
         return [
-            sqrt(np.linalg.det(m.modelfit_results.covariance_matrix) / orig_det)
-            if m.modelfit_results is not None and m.modelfit_results.covariance_matrix is not None
+            sqrt(np.linalg.det(res.covariance_matrix) / orig_det)
+            if res is not None and res.covariance_matrix is not None
             else np.nan
-            for m in cdd_models
+            for res in cdd_model_results
         ]
     except Exception:
         return None
 
 
 def calculate_results(
-    base_model: Model, cdd_models: List[Model], case_column, skipped_individuals, **_
+    base_model: Model,
+    base_model_results,
+    cdd_models: List[Model],
+    cdd_model_results,
+    case_column,
+    skipped_individuals,
+    **_,
 ):
     """Calculate CDD results"""
 
-    if base_model.modelfit_results is None:
+    if base_model_results is None:
         raise ValueError('cdd base model has no results')
 
     cdd_estimates = pd.DataFrame(
         data=[
-            pd.Series(m.modelfit_results.parameter_estimates, name=m.name)
-            for m in cdd_models
-            if m.modelfit_results is not None
+            pd.Series(res.parameter_estimates, name=m.name)
+            for m, res in zip(cdd_models, cdd_model_results)
+            if res is not None
         ]
     )
 
     cdd_model_names = [m.name for m in cdd_models]
 
     # create Series of NaN values and then replace any computable results
     cook_temp = pd.Series(np.nan, index=cdd_model_names)
     try:
-        base_model.modelfit_results.covariance_matrix
+        base_model_results.covariance_matrix
     except Exception:
         pass
     else:
         cook_temp.update(
             pd.Series(
                 compute_cook_scores(
-                    base_model.modelfit_results.parameter_estimates,
+                    base_model_results.parameter_estimates,
                     cdd_estimates,
-                    base_model.modelfit_results.covariance_matrix,
+                    base_model_results.covariance_matrix,
                 ),
                 index=cdd_estimates.index,
                 dtype=np.float64,
             )
         )
 
     jack_cook_score = None
     if len(cdd_model_names) == cdd_estimates.shape[0]:
         # all models have results
         jackkknife_covariance_matrix = compute_jackknife_covariance_matrix(cdd_estimates)
         jack_cook_score = pd.Series(
             compute_cook_scores(
-                base_model.modelfit_results.parameter_estimates,
+                base_model_results.parameter_estimates,
                 cdd_estimates,
                 jackkknife_covariance_matrix,
             ),
             index=cdd_model_names,
         )
 
-    dofv = compute_delta_ofv(base_model, cdd_models, skipped_individuals)
+    dofv = compute_delta_ofv(base_model_results, cdd_model_results, skipped_individuals)
     dofv_influential = [elt > 3.86 for elt in dofv]
     infl_list = [
         skipped[0]
         for skipped, infl in zip(skipped_individuals, dofv_influential)
         if infl and len(skipped) == 1
     ]
 
     if infl_list:
         try:
             iplot = plot_individual_predictions(
                 base_model,
-                base_model.modelfit_results.predictions[['PRED', 'CIPREDI']],
+                base_model_results.predictions[['PRED', 'CIPREDI']],
                 individuals=infl_list,
             )
         except Exception:
             iplot = None
     else:
         iplot = None
 
     try:
-        covmatrix = base_model.modelfit_results.covariance_matrix
+        covmatrix = base_model_results.covariance_matrix
     except Exception:
         covratios = np.nan
     else:
-        covratios = compute_covariance_ratios(cdd_models, covmatrix)
+        covratios = compute_covariance_ratios(cdd_model_results, covmatrix)
 
     case_results = pd.DataFrame(
         {
             'cook_score': cook_temp,
             'jackknife_cook_score': jack_cook_score,
             'delta_ofv': dofv,
             'dofv_influential': dofv_influential,
@@ -226,13 +230,23 @@
         raise IOError(f'Could not find cdd folder: {str(path)}')
 
     options = psn_cdd_options(path)
 
     if base_model_path is None:
         base_model_path = Path(options['model_path'])
     base_model = Model.create_model(base_model_path)
+    base_model_results = read_modelfit_results(base_model_path)
 
-    cdd_models = list(map(Model.create_model, model_paths(path, 'cdd_*.mod')))
+    paths = model_paths(path, 'cdd_*.mod')
+    cdd_models = list(map(Model.parse_model, paths))
+    cdd_results = list(map(read_modelfit_results, paths))
     skipped_individuals = psn_cdd_skipped_individuals(path)
 
-    res = calculate_results(base_model, cdd_models, options['case_column'], skipped_individuals)
+    res = calculate_results(
+        base_model,
+        base_model_results,
+        cdd_models,
+        cdd_results,
+        options['case_column'],
+        skipped_individuals,
+    )
     return res
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/common.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/common.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,17 @@
 ) -> T:
     summary_tool = summarize_tool(res_models, base_model, rank_type, cutoff, bic_type)
     summary_individuals, summary_individuals_count = summarize_tool_individuals(
         [base_model] + res_models,
         summary_tool['description'],
         summary_tool[f'd{"ofv" if rank_type == "lrt" else rank_type}'],
     )
-    summary_errors = summarize_errors([base_model] + res_models)
+    summary_errors = summarize_errors(
+        [base_model.modelfit_results] + [m.modelfit_results for m in res_models]
+    )
 
     best_model_name = summary_tool['rank'].idxmin()
     best_model = next(filter(lambda model: model.name == best_model_name, res_models), base_model)
 
     if base_model.name != input_model.name:
         models = [base_model] + res_models
     else:
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/covsearch/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/covsearch/tool.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,19 +130,20 @@
     Returns
     -------
     COVSearchResults
         COVsearch tool result object
 
     Examples
     --------
-    >>> from pharmpy.modeling import *
+    >>> from pharmpy.modeling import load_example_model
+    >>> from pharmpy.tools import run_covsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> from pharmpy.tools import run_covsearch  # doctest: +SKIP
+    >>> results = load_example_modelfit_results("pheno")
     >>> effects = 'COVARIATE([CL, V], [AGE, WT], EXP)'
-    >>> res = run_covsearch(effects, model=model, results=model.modelfit_results)      # doctest: +SKIP
+    >>> res = run_covsearch(effects, model=model, results=results)      # doctest: +SKIP
     """
 
     wf = Workflow()
     wf.name = NAME_WF
 
     init_task = init(model)
     wf.add_task(init_task)
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/crossval/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/crossval/results.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from __future__ import annotations
 
 import re
 from dataclasses import dataclass
 from typing import Any, Optional
 
 from pharmpy.deps import pandas as pd
-from pharmpy.model import Model, Results
+from pharmpy.model import Results
+from pharmpy.tools import read_modelfit_results
 
 
 @dataclass(frozen=True)
 class CrossvalResults(Results):
     """Crossval results class"""
 
     runs: Optional[Any] = None
     prediction_ofv_sum: Optional[Any] = None
 
 
-def calculate_results(estimation_models, prediction_models):
+def calculate_results(estimation_results, prediction_results):
     """Calculate crossval results"""
-    est_ofvs = [model.modelfit_results.ofv for model in estimation_models]
-    pred_ofvs = [model.modelfit_results.ofv for model in prediction_models]
+    est_ofvs = [res.ofv for res in estimation_results]
+    pred_ofvs = [res.ofv for res in prediction_results]
     runs = pd.DataFrame(
         {'estimation_ofv': est_ofvs, 'prediction_ofv': pred_ofvs},
         index=pd.RangeIndex(start=1, stop=len(est_ofvs) + 1),
     )
 
     return CrossvalResults(runs=runs, prediction_ofv_sum=sum(pred_ofvs))
 
@@ -35,12 +36,12 @@
     def natural_keys(text):
         return [atoi(c) for c in re.split(r'(\d+)', text)]
 
     est_paths = [str(p) for p in (path / 'm1').glob('est_model*.mod')]
     est_paths.sort(key=natural_keys)
     pred_paths = [str(p) for p in (path / 'm1').glob('pred_model*.mod')]
     pred_paths.sort(key=natural_keys)
-    ests = [Model.create_model(path) for path in est_paths]
-    preds = [Model.create_model(path) for path in pred_paths]
+    ests = [read_modelfit_results(path) for path in est_paths]
+    preds = [read_modelfit_results(path) for path in pred_paths]
 
     res = calculate_results(ests, preds)
     return res
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/algorithms.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/estmethod/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/report.rst` & `pharmpy-core-0.96.0/src/pharmpy/tools/estmethod/report.rst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/estmethod/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/estmethod/tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     -------
     EstMethodResults
         Estmethod tool result object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import run_estmethod, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> from pharmpy.tools import run_estmethod # doctest: +SKIP
-    >>> res = model.modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
     >>> methods = ['imp', 'saem']
-    >>> run_estmethod('reduced', methods=methods, solvers='all', results=res, model=model) # doctest: +SKIP
+    >>> run_estmethod('reduced', methods=methods, solvers='all', results=results, model=model) # doctest: +SKIP
 
     """
     wf = Workflow()
     wf.name = "estmethod"
 
     algorithm_func = getattr(algorithms, algorithm)
 
@@ -114,15 +114,15 @@
             res_models.append(model)
 
     summary_tool = summarize_tool(models)
     summary_models = summarize_modelfit_results(
         [base_model.modelfit_results] + [model.modelfit_results for model in res_models],
         include_all_estimation_steps=True,
     )
-    summary_errors = summarize_errors(models)
+    summary_errors = summarize_errors(m.modelfit_results for m in models)
     summary_settings = summarize_estimation_steps([base_model] + res_models)
 
     if base_model.name == input_model.name:
         models = res_models
     else:
         models = [base_model] + res_models
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/evaldesign/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/evaldesign/tool.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from pharmpy.workflows import Task, Workflow
 
 
 def create_workflow(model: Model):
     wf = Workflow()
     wf.name = 'evaldesign'
 
-    from pharmpy.plugins.nonmem.run import evaluate_design
+    from pharmpy.tools.external.nonmem.run import evaluate_design
 
     task = Task('run', evaluate_design, model)
     wf.add_task(task)
 
     task_result = Task('results', post_process_results)
     wf.add_task(task_result, predecessors=[task])
     return wf
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/frem/models.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/frem/models.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import itertools
 
 from pharmpy.deps import numpy as np
 from pharmpy.internals.math import corr2cov, nearest_postive_semidefinite
 from pharmpy.modeling import fix_or_unfix_parameters, set_initial_estimates
 
 
-def calculate_parcov_inits(model, ncovs):
+def calculate_parcov_inits(model, ie, ncovs):
     """Get dict of new updated inits for parcov block
 
     model already has a FREM block
     Initial estimates for the parcov block is calculated given correlations of individual etas
     """
     dist = model.random_variables.iiv[-1]
     rvs = list(dist.names)
-    ie = model.modelfit_results.individual_estimates
     eta_corr = ie[rvs].corr()
     eta_corr.fillna(value=1.0, inplace=True)  # Identical etas will get NaN as both diag and corr
 
     sigma = dist.variance
     inits = sigma.subs(model.parameters.inits)
     inits = np.array(inits).astype(np.float64)
     sd = np.sqrt(inits.diagonal())
@@ -33,26 +32,25 @@
     param_inits = {
         parcov_symb[i, j].name: parcov_inits[i, j]
         for i, j in itertools.product(range(ncovs), range(npars))
     }
     return param_inits
 
 
-def create_model3b(model1b, model3, ncovs):
+def create_model3b(model1b, model3, model3_res, ncovs):
     """Create model 3b from model 3
 
     * Update parcov omega block
     * Set FIX pattern back from model1b
     * Use initial etas from model3
     """
     model3b = model3.replace(name='model_3b')
-    parcov_inits = calculate_parcov_inits(model3, ncovs)
+    ie = model3_res.individual_estimates
+    parcov_inits = calculate_parcov_inits(model3, ie, ncovs)
     model3b = set_initial_estimates(model3b, parcov_inits)
     model3b = set_initial_estimates(
         model3b, model3b.random_variables.nearest_valid_parameters(model3b.parameters.inits)
     )
     model3b = fix_or_unfix_parameters(model3b, model1b.parameters.fix)
 
-    model3b = model3b.replace(
-        initial_individual_estimates=model3.modelfit_results.individual_estimates
-    )
+    model3b = model3b.replace(initial_individual_estimates=ie)
     return model3b
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/frem/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/frem/results.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     get_baselines,
     get_covariate_baselines,
     is_linearized,
     sample_individual_estimates,
     sample_parameters_from_covariance_matrix,
     set_covariates,
 )
+from pharmpy.tools import read_modelfit_results
 from pharmpy.workflows import ToolDatabase
 
 
 @dataclass(frozen=True)
 class FREMResults(Results):
     """FREM Results class
 
@@ -389,114 +390,133 @@
         plots.append(plot)
 
     v = alt.vconcat(*plots).resolve_scale(x='shared')
     return v
 
 
 def calculate_results(
-    frem_model, continuous, categorical, method=None, intermediate_models=None, rng=None, **kwargs
+    frem_model,
+    frem_model_results,
+    continuous,
+    categorical,
+    method=None,
+    intermediate_models=None,
+    intermediate_models_res=None,
+    rng=None,
+    **kwargs,
 ):
     """Calculate FREM results
 
     :param method: Either 'cov_sampling' or 'bipp'
     """
     if intermediate_models is None:
         intermediate_models = []
+        intermediate_models_res = []
 
     if method is None or method == 'cov_sampling':
         try:
             res = calculate_results_using_cov_sampling(
-                frem_model, continuous, categorical, rng=rng, **kwargs
+                frem_model, frem_model_results, continuous, categorical, rng=rng, **kwargs
             )
         except AttributeError:
             # Fallback to bipp
-            res = calculate_results_using_bipp(frem_model, continuous, categorical, rng=rng)
+            res = calculate_results_using_bipp(
+                frem_model, frem_model_results, continuous, categorical, rng=rng
+            )
     elif method == 'bipp':
-        res = calculate_results_using_bipp(frem_model, continuous, categorical, rng=rng)
+        res = calculate_results_using_bipp(
+            frem_model, frem_model_results, continuous, categorical, rng=rng
+        )
     else:
         raise ValueError(f'Unknown frem postprocessing method {method}')
     mod_names = []
     mod_ofvs = []
     if intermediate_models:
-        for intmod in intermediate_models:
-            intmod_res = intmod.modelfit_results
+        for intmod, intmod_res in zip(intermediate_models, intermediate_models_res):
             if intmod_res is not None:
                 mod_ofvs.append(intmod_res.ofv)
                 mod_names.append(intmod.name)
-    mod_ofvs.append(frem_model.modelfit_results.ofv)
+    mod_ofvs.append(frem_model_results.ofv)
     mod_names.append(frem_model.name)
     ofv = pd.DataFrame({'ofv': mod_ofvs}, index=mod_names)
     ofv.index.name = 'model_name'
-    estimates = parameter_inits_and_estimates(frem_model, intermediate_models)
+    estimates = parameter_inits_and_estimates(
+        frem_model, frem_model_results, intermediate_models, intermediate_models_res
+    )
     res = replace(res, ofv=ofv, parameter_inits_and_estimates=estimates)
 
     if intermediate_models:
-        ser = base_vs_frem_model(frem_model, intermediate_models[0])
+        ser = base_vs_frem_model(frem_model_results, intermediate_models_res[0])
         res = replace(res, base_parameter_change=ser)
 
-    estimated_covbase = _calculate_covariate_baselines(frem_model, continuous + categorical)
+    estimated_covbase = _calculate_covariate_baselines(
+        frem_model, frem_model_results, continuous + categorical
+    )
     mean = estimated_covbase.mean()
     stdev = estimated_covbase.std()
     estcovs = pd.DataFrame({'mean': mean, 'stdev': stdev})
 
     res = replace(res, estimated_covariates=estcovs)
 
     return replace(
         res,
         covariate_effects_plot=plot_covariate_effects(res),
         individual_effects_plot=plot_individual_effects(res),
         unexplained_variability_plot=plot_unexplained_variability(res),
     )
 
 
-def base_vs_frem_model(frem_model, model_1):
-    base_ests = model_1.modelfit_results.parameter_estimates
-    final_ests = frem_model.modelfit_results.parameter_estimates
+def base_vs_frem_model(frem_model_res, model_1_res):
+    base_ests = model_1_res.parameter_estimates
+    final_ests = frem_model_res.parameter_estimates
     ser = pd.Series(dtype=np.float64, name='relative_change')
     for param in base_ests.keys():
         if param in final_ests:
             ser[param] = (final_ests[param] - base_ests[param]) / abs(base_ests[param]) * 100
     return ser
 
 
-def parameter_inits_and_estimates(frem_model, intermediate_models) -> pd.DataFrame:
+def parameter_inits_and_estimates(
+    frem_model, frem_model_results, intermediate_models, intermediate_models_res
+) -> pd.DataFrame:
     model_names = []
     df = pd.DataFrame()
 
-    for model in intermediate_models:
+    for model, res in zip(intermediate_models, intermediate_models_res):
         df = pd.concat(
             [
                 df,
                 pd.Series(model.parameters.nonfixed.inits),
-                model.modelfit_results.parameter_estimates,
+                res.parameter_estimates,
             ],
             ignore_index=True,
             axis=1,
         )
         model_names.append(model.name)
 
     df = pd.concat(
         [
             df,
             pd.Series(frem_model.parameters.nonfixed.inits),
-            frem_model.modelfit_results.parameter_estimates,
+            frem_model_results.parameter_estimates,
         ],
         ignore_index=True,
         axis=1,
     )
     df = df.T
     df = df.reindex(columns=frem_model.parameters.nonfixed.inits.keys())
     model_names.append(frem_model.name)
     index = pd.MultiIndex.from_product([model_names, ['init', 'estimate']], names=['model', 'type'])
     df.index = index
     return df
 
 
 def calculate_results_using_cov_sampling(
     frem_model,
+    frem_model_results,
     continuous,
     categorical,
     cov_model=None,
     force_posdef_samples=500,
     force_posdef_covmatrix=False,
     samples=1000,
     rescale=True,
@@ -514,51 +534,53 @@
                                    the cov model to be positive definite. Default is to raise
                                    in this case.
     :param samples: The number of parameter vector samples to use.
     """
     if cov_model is not None:
         uncertainty_results = cov_model.modelfit_results
     else:
-        uncertainty_results = frem_model.modelfit_results
+        uncertainty_results = frem_model_results
 
     dist = frem_model.random_variables.iiv[-1]
     sigma_symb = dist.variance
 
     parameters = [
         s
-        for s in frem_model.modelfit_results.parameter_estimates.index
+        for s in frem_model_results.parameter_estimates.index
         if sympy.Symbol(s) in sigma_symb.free_symbols
     ]
     parvecs = sample_parameters_from_covariance_matrix(
         frem_model,
         uncertainty_results.parameter_estimates[parameters],
         uncertainty_results.covariance_matrix,
         force_posdef_samples=force_posdef_samples,
         force_posdef_covmatrix=force_posdef_covmatrix,
         n=samples,
         rng=rng,
     )
     res = calculate_results_from_samples(
-        frem_model, continuous, categorical, parvecs, rescale=rescale
+        frem_model, frem_model_results, continuous, categorical, parvecs, rescale=rescale
     )
     return res
 
 
-def calculate_results_from_samples(frem_model, continuous, categorical, parvecs, rescale=True):
+def calculate_results_from_samples(
+    frem_model, frem_model_results, continuous, categorical, parvecs, rescale=True
+):
     """Calculate the FREM results given samples of parameter estimates"""
     n = len(parvecs)
     dist = frem_model.random_variables.iiv[-1]
     rvs = list(dist.names)
     sigma_symb = dist.variance
     parameters = [
         s
-        for s in frem_model.modelfit_results.parameter_estimates.index
+        for s in frem_model_results.parameter_estimates.index
         if sympy.Symbol(s) in sigma_symb.free_symbols
     ]
-    parvecs.loc['estimates'] = frem_model.modelfit_results.parameter_estimates.loc[parameters]
+    parvecs.loc['estimates'] = frem_model_results.parameter_estimates.loc[parameters]
 
     covariates = continuous + categorical
     frem_model = set_covariates(frem_model, covariates)
     covariate_baselines = get_covariate_baselines(frem_model)
     covariate_baselines = covariate_baselines[covariates]
     cov_means = covariate_baselines.mean()
     cov_modes = covariate_baselines.mode().iloc[0]  # Select first mode if more than one
@@ -611,15 +633,15 @@
     parameter_variability = []
 
     # Switch to symengine for speed
     # Could also assume order of parameters, but not much gain
     sigma_symb = symengine.sympify(sigma_symb)
     parvecs.columns = [symengine.Symbol(colname) for colname in parvecs.columns]
 
-    estimated_covbase = _calculate_covariate_baselines(frem_model, covariates)
+    estimated_covbase = _calculate_covariate_baselines(frem_model, frem_model_results, covariates)
     covbase = estimated_covbase.to_numpy()
 
     parameter_variability_all = None
 
     for sample_no, params in parvecs.iterrows():
         sigma = sigma_symb.subs(dict(params))
         sigma = np.array(sigma).astype(np.float64)
@@ -845,23 +867,23 @@
     while True:
         candidate = f'{stem}({i})'
         if candidate not in params:
             return candidate
         i += 1
 
 
-def _calculate_covariate_baselines(model, covariates):
+def _calculate_covariate_baselines(model, res, covariates):
     exprs = [
         ass.expression.args[0][0]
         for ass in model.statements
         if sympy.Symbol('FREMTYPE') in ass.free_symbols and ass.symbol.name == 'IPRED'
     ]
     exprs = [
         subs(
-            subs(expr, dict(model.modelfit_results.parameter_estimates), simultaneous=True),
+            subs(expr, dict(res.parameter_estimates), simultaneous=True),
             model.parameters.inits,
             simultaneous=True,
         )
         for expr in exprs
     ]
     new = []
     for expr in exprs:
@@ -871,45 +893,45 @@
                 expr = subs(expr, {symb: stat.expression}, simultaneous=True)
         new.append(expr)
     exprs = new
 
     def fn(row):
         return [np.float64(subs(expr, dict(row))) for expr in exprs]
 
-    df = model.modelfit_results.individual_estimates.apply(fn, axis=1, result_type='expand')
+    df = res.individual_estimates.apply(fn, axis=1, result_type='expand')
     df.columns = covariates
     return df
 
 
 def calculate_results_using_bipp(
-    frem_model, continuous, categorical, rescale=True, samples=2000, rng=None
+    frem_model, frem_model_results, continuous, categorical, rescale=True, samples=2000, rng=None
 ):
     """Estimate a covariance matrix for the frem model using the BIPP method
 
     Bootstrap on the individual parameter posteriors
     Only the individual estimates, individual unvertainties and the parameter estimates
     are needed.
 
     """
     rng = create_rng(rng)
     assert rng is not None
     dist = frem_model.random_variables.iiv[-1]
     etas = list(dist.names)
     pool = sample_individual_estimates(
         frem_model,
-        frem_model.modelfit_results.individual_estimates,
-        frem_model.modelfit_results.individual_estimates_covariance,
+        frem_model_results.individual_estimates,
+        frem_model_results.individual_estimates_covariance,
         parameters=etas,
         rng=rng,
     ).droplevel('sample')
     ninds = len(pool.index.unique())
     ishr = calculate_individual_shrinkage(
         frem_model,
-        frem_model.modelfit_results.parameter_estimates,
-        frem_model.modelfit_results.individual_estimates_covariance,
+        frem_model_results.parameter_estimates,
+        frem_model_results.individual_estimates_covariance,
     )
     ishr = ishr[pool.columns]
     lower_indices = np.tril_indices(len(etas))
     pop_params = np.array(dist.variance).astype(str)[lower_indices]
     parameter_samples = np.empty((samples, len(pop_params)))
     remaining_samples = samples
     k = 0
@@ -922,18 +944,18 @@
         bootstrap_cov = np.cov(np.transpose(corrected_bootstrap))
         if not is_posdef(bootstrap_cov):
             continue
         parameter_samples[k, :] = bootstrap_cov[lower_indices]
         k += 1
     frame = pd.DataFrame(parameter_samples, columns=pop_params)
     # Shift to the mean of the parameter estimate
-    shift = frem_model.modelfit_results.parameter_estimates[pop_params] - frame.mean()
+    shift = frem_model_results.parameter_estimates[pop_params] - frame.mean()
     frame = frame + shift
     res = calculate_results_from_samples(
-        frem_model, continuous, categorical, frame, rescale=rescale
+        frem_model, frem_model_results, continuous, categorical, frame, rescale=rescale
     )
     return res
 
 
 def psn_reorder_base_model_inits(model, path):
     """Reorder omega inits from base model in PsN
 
@@ -982,27 +1004,28 @@
 
     """
     path = Path(path)
 
     model_4_path = path / 'final_models' / 'model_4.mod'
     if not model_4_path.is_file():
         raise IOError(f'Could not find FREM model 4: {str(model_4_path)}')
-    model_4 = Model.create_model(model_4_path)
+    model_4 = Model.parse_model(model_4_path)
+    model_4_results = read_modelfit_results(model_4_path)
     with warnings.catch_warnings():
         warnings.filterwarnings("ignore", message="Adjusting initial estimates")
-        if model_4.modelfit_results is None:
+        if model_4_results is None:
             raise ValueError('Model 4 has no results')
     cov_model = None
     if method == 'cov_sampling':
         try:
-            model_4.modelfit_results.covariance_matrix
+            model_4_results.covariance_matrix
         except Exception:
             model_4b_path = path / 'final_models' / 'model_4b.mod'
             try:
-                model_4b = Model.create_model(model_4b_path)
+                model_4b = Model.parse_model(model_4b_path)
             except FileNotFoundError:
                 pass
             else:
                 cov_model = model_4b
 
     with open(path / 'covariates_summary.csv') as covsum:
         covsum.readline()
@@ -1034,35 +1057,40 @@
 
     nunique = get_baselines(model_4)[all_covariates].nunique()
     continuous = list(nunique.index[nunique != 2])
     categorical = list(nunique.index[nunique == 2])
 
     intmod_names = ['model_1.mod', 'model_2.mod', 'model_3.mod', 'model_3b.mod']
     intmods = []
+    intmodres = []
     for m in intmod_names:
         intmod_path = path / 'm1' / m
         if intmod_path.is_file():
-            intmod = Model.create_model(intmod_path)
+            intmod = Model.parse_model(intmod_path)
             intmods.append(intmod)
+            res = read_modelfit_results(intmod_path)
+            intmodres.append(res)
 
-    model1b = Model.create_model(path / 'm1' / 'model_1b.mod')
+    model1b = Model.parse_model(path / 'm1' / 'model_1b.mod')
     model1 = intmods[0]
-    modelfit_results = replace(
-        model1.modelfit_results, parameter_estimates=pd.Series(model1b.parameters.nonfixed.inits)
+    model1_res = replace(
+        intmodres[0], parameter_estimates=pd.Series(model1b.parameters.nonfixed.inits)
     )
-    model1 = model1.replace(modelfit_results=modelfit_results)
     model1 = psn_reorder_base_model_inits(model1, path)
     intmods[0] = model1
+    intmodres[0] = model1_res
 
     res = calculate_results(
         model_4,
+        model_4_results,
         continuous,
         categorical,
         method=method,
         force_posdef_covmatrix=force_posdef_covmatrix,
         force_posdef_samples=force_posdef_samples,
         cov_model=cov_model,
         rescale=rescale,
         intermediate_models=intmods,
+        intermediate_models_res=intmodres,
         rng=np.random.default_rng(9843),
     )
     return res
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/frem/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/frem/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from pharmpy.model import Model
 from pharmpy.modeling import (
     get_covariate_baselines,
     list_time_varying_covariates,
     set_covariates,
     write_model,
 )
+from pharmpy.tools import read_modelfit_results
 
 from .models import create_model3b
 
 
 def setup(model_path, covariates):
     input_model = Model.create_model(model_path)
     covariates = check_covariates(input_model, covariates)
@@ -74,11 +75,12 @@
 def update_model3b_for_psn(rundir, ncovs):
     """Function to update model3b from psn
 
     NOTE: This function lets pharmpy tie in to the PsN workflow
           and is a temporary solution
     """
     model_path = Path(rundir) / 'm1'
-    model1b = Model.create_model(model_path / 'model_1b.mod')
-    model3 = Model.create_model(model_path / 'model_3.mod')
-    model3b = create_model3b(model1b, model3, int(ncovs))
+    model1b = Model.parse_model(model_path / 'model_1b.mod')
+    model3 = Model.parse_model(model_path / 'model_3.mod')
+    model3_res = read_modelfit_results(model_path / 'model_3.mod')
+    model3b = create_model3b(model1b, model3, model3_res, int(ncovs))
     write_model(model3b, model_path, force=True)
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/funcs/ml.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite` & `pharmpy-core-0.96.0/src/pharmpy/tools/funcs/ml_models/infinds.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite` & `pharmpy-core-0.96.0/src/pharmpy/tools/funcs/ml_models/outliers.tflite`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/funcs/summarize_individuals.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/funcs/summarize_individuals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/algorithms.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/iivsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/iivsearch/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/iivsearch/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,17 +59,18 @@
     -------
     IIVSearchResults
         IIVsearch tool result object
 
     Examples
     --------
     >>> from pharmpy.modeling import *
+    >>> from pharmpy.tools import run_iivsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> from pharmpy.tools import run_iivsearch     # doctest: +SKIP
-    >>> run_iivsearch('brute_force', results=model.modelfit_results, model=model)   # doctest: +SKIP
+    >>> results = load_example_modelfit_results("pheno")
+    >>> run_iivsearch('brute_force', results=results, model=model)   # doctest: +SKIP
     """
 
     wf = Workflow()
     wf.name = 'iivsearch'
     start_task = Task('start_iiv', start, model, algorithm, iiv_strategy, rank_type, cutoff)
     wf.add_task(start_task)
     task_results = Task('results', _results)
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/iovsearch/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/iovsearch/tool.py`

 * *Files 6% similar despite different names*

```diff
@@ -61,17 +61,19 @@
     Returns
     -------
     IOVSearchResults
         IOVSearch tool result object
 
     Examples
     --------
-    >>> from pharmpy.modeling import *
+    >>> from pharmpy.modeling import load_example_model
+    >>> from pharmpy.tools import run_iovsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> run_iovsearch('OCC', results=model.modelfit_results, model=model)      # doctest: +SKIP
+    >>> results = load_example_modelfit_results("pheno")
+    >>> run_iovsearch('OCC', results=results, model=model)      # doctest: +SKIP
     """
 
     wf = Workflow()
     wf.name = NAME_WF
 
     init_task = init(model)
     wf.add_task(init_task)
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/linearize/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/linearize/tool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/absorption.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/covariate.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/elimination.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/peripherals.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/peripherals.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/feature/transits.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/filter.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/filter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/grammar.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/grammar.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/helpers.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/interpreter.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/parse.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/definition.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/definition.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/absorption.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/absorption.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/count_interpreter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/covariate.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/covariate.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/elimination.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/elimination.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/statement/feature/transits.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/statement/feature/transits.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/mfl/stringify.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/mfl/stringify.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/modelfit/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/modelfit/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/modelfit/tool.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,14 +111,14 @@
 def get_execute_model(tool: Optional[SupportedPlugin]):
     from pharmpy.tools.modelfit import conf
 
     if tool is None:
         tool = conf.default_tool
 
     if tool == 'nonmem':
-        from pharmpy.plugins.nonmem.run import execute_model
+        from pharmpy.tools.external.nonmem.run import execute_model
     elif tool == 'nlmixr':
-        from pharmpy.plugins.nlmixr.run import execute_model
+        from pharmpy.tools.external.nlmixr.run import execute_model
     else:
         raise ValueError(f"Unknown estimation tool {tool}")
 
     return execute_model
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/algorithms.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/modelsearch/algorithms.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/modelsearch/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/modelsearch/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,19 +49,19 @@
     Returns
     -------
     ModelSearchResults
         Modelsearch tool result object
 
     Examples
     --------
-    >>> from pharmpy.modeling import *
+    >>> from pharmpy.modeling import load_example_model
+    >>> from pharmpy.tools import run_modelsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> from pharmpy.tools import run_modelsearch # doctest: +SKIP
-    >>> res = model.modelfit_results
-    >>> run_modelsearch('ABSORPTION(ZO);PERIPHERALS(1)', 'exhaustive', results=res, model=model) # doctest: +SKIP
+    >>> results = load_example_modelfit_results("pheno")
+    >>> run_modelsearch('ABSORPTION(ZO);PERIPHERALS(1)', 'exhaustive', results=results, model=model) # doctest: +SKIP
 
     """
 
     wf = Workflow()
     wf.name = 'modelsearch'
 
     if model:
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/psn_helpers.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/psn_helpers.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/qa/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/qa/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 import pharmpy.tools.psn_helpers as psn_helpers
 from pharmpy.deps import numpy as np
 from pharmpy.deps import pandas as pd
 from pharmpy.deps import sympy
 from pharmpy.model import Model, Results
 from pharmpy.results import read_results
+from pharmpy.tools import read_modelfit_results
 
 
 @dataclass(frozen=True)
 class QAResults(Results):
     dofv: Optional[Any] = None
     fullblock_parameters: Optional[Any] = None
     boxcox_parameters: Optional[Any] = None
@@ -490,40 +491,60 @@
     """Create qa results from a PsN qa run
 
     :param path: Path to PsN qa run directory
     :return: A :class:`QAResults` object
     """
     path = Path(path)
 
-    original_model = Model.create_model(path / 'linearize_run' / 'scm_dir1' / 'derivatives.mod')
+    original_model = Model.parse_model(path / 'linearize_run' / 'scm_dir1' / 'derivatives.mod')
+    orig_res = read_modelfit_results(path / 'linearize_run' / 'scm_dir1' / 'derivatives.mod')
+    original_model = original_model.replace(modelfit_results=orig_res)
+
     base_path = list(path.glob('*_linbase.mod'))[0]
-    base_model = Model.create_model(base_path)
+    base_model = Model.parse_model(base_path)
+    base_res = Model.parse_model(base_path)
+    base_model = base_model.replace(modelfit_results=base_res)
+
     fullblock_path = path / 'modelfit_run' / 'fullblock.mod'
     if fullblock_path.is_file():
-        fullblock_model = Model.create_model(fullblock_path)
+        fullblock_model = Model.parse_model(fullblock_path)
+        fb_res = read_modelfit_results(fullblock_path)
+        fullblock_model = fullblock_model.replace(modelfit_results=fb_res)
     else:
         fullblock_model = None
+
     boxcox_path = path / 'modelfit_run' / 'boxcox.mod'
     if boxcox_path.is_file():
-        boxcox_model = Model.create_model(boxcox_path)
+        boxcox_model = Model.parse_model(boxcox_path)
+        bc_res = read_modelfit_results(boxcox_path)
+        boxcox_model = boxcox_model.replace(modelfit_results=bc_res)
     else:
         boxcox_model = None
+
     tdist_path = path / 'modelfit_run' / 'tdist.mod'
     if tdist_path.is_file():
-        tdist_model = Model.create_model(tdist_path)
+        tdist_model = Model.parse_model(tdist_path)
+        td_res = read_modelfit_results(tdist_path)
+        tdist_model = tdist_model.replace(modelfit_results=td_res)
     else:
         tdist_model = None
+
     addetas_path = path / 'add_etas_run' / 'add_etas_linbase.mod'
     if addetas_path.is_file():
-        addetas_model = Model.create_model(addetas_path)
+        addetas_model = Model.parse_model(addetas_path)
+        ae_res = read_modelfit_results(addetas_path)
+        addetas_model = addetas_model.replace(modelfit_results=ae_res)
     else:
         addetas_model = None
+
     iov_path = path / 'modelfit_run' / 'iov.mod'
     if iov_path.is_file():
-        iov_model = Model.create_model(iov_path)
+        iov_model = Model.parse_model(iov_path)
+        iov_res = read_modelfit_results(iov_path)
+        iov_model = iov_model.replace(modelfit_results=iov_res)
     else:
         iov_model = None
 
     frem_path = path / 'frem_run' / 'results.json'
     if frem_path.is_file():
         frem_res = read_results(frem_path)
     else:
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/rankfuncs.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/reporting.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/reporting.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/run.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/run.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 from pharmpy.modeling.lrt import test as lrt_test
 from pharmpy.results import ModelfitResults, mfr
 from pharmpy.tools.psn_helpers import create_results as psn_create_results
 from pharmpy.workflows import Workflow, execute_workflow, split_common_options
 from pharmpy.workflows.model_database import LocalModelDirectoryDatabase, ModelDatabase
 from pharmpy.workflows.tool_database import ToolDatabase
 
+from .external import parse_modelfit_results
+
 
 def fit(
     model_or_models: Union[Model, List[Model]], tool: Optional[str] = None
 ) -> Union[ModelfitResults, List[ModelfitResults]]:
     """Fit models.
 
     Parameters
@@ -176,15 +178,15 @@
 
 
 def run_tool_with_name(
     name: str, tool, args: Sequence, kwargs: Mapping[str, Any]
 ) -> Union[Model, List[Model], Tuple[Model], Results]:
     # FIXME: workaround until ModelfitResults is disentangled with
     #  Model object
-    if 'model' in kwargs.keys() and 'results' in kwargs.keys():
+    if 'model' in kwargs and 'results' in kwargs:
         model = kwargs['model']
         res = kwargs['results']
         if isinstance(model, Model) and isinstance(res, ModelfitResults):
             model = model.replace(modelfit_results=res)
             kwargs['model'] = model
 
     common_options, tool_options = split_common_options(kwargs)
@@ -672,23 +674,23 @@
     path = normalize_user_given_path(path)
     if csv:
         results.to_csv(path)
     else:
         results.to_json(path, lzma=lzma)
 
 
-def summarize_errors(models: Union[Model, List[Model]]) -> pd.DataFrame:
+def summarize_errors(results: Union[ModelfitResults, List[ModelfitResults]]) -> pd.DataFrame:
     """Summarize errors and warnings from one or multiple model runs.
 
     Summarize the errors and warnings found after running the model/models.
 
     Parameters
     ----------
-    models : list, Model
-        List of models or single model
+    results : list, ModelfitResults
+        List of ModelfitResults or single ModelfitResults
 
     Return
     ------
     pd.DataFrame
         A DataFrame of errors with model name, category (error or warning), and an int as index,
         an empty DataFrame if there were no errors or warnings found.
 
@@ -696,24 +698,23 @@
     --------
     >>> from pharmpy.modeling import load_example_model
     >>> from pharmpy.tools import summarize_errors
     >>> model = load_example_model("pheno")
     >>> summarize_errors(model)      # doctest: +SKIP
     """
     # FIXME: have example with errors
-    if isinstance(models, Model):
-        models = [models]
+    if isinstance(results, ModelfitResults):
+        results = [results]
 
     idcs, rows = [], []
 
-    for model in models:
-        res = model.modelfit_results
+    for res in results:
         if res is not None and len(res.log.log) > 0:
             for i, entry in enumerate(res.log.log):
-                idcs.append((model.name, entry.category, i))
+                idcs.append((res.name, entry.category, i))
                 rows.append([entry.time, entry.message])
 
     index_names = ['model', 'category', 'error_no']
     col_names = ['time', 'message']
     index = pd.MultiIndex.from_tuples(idcs, names=index_names)
 
     if rows:
@@ -906,14 +907,17 @@
     >>> summarize_modelfit_results(model.modelfit_results) # doctest: +SKIP
                      description  minimization_successful ...        ofv  ... runtime_total  ...
     pheno PHENOBARB SIMPLE MODEL                     True ... 586.276056  ...           4.0  ...
     """
     if isinstance(results, ModelfitResults):
         results = [results]
 
+    if all(res is None for res in results):
+        raise ValueError('All input results are empty')
+
     summaries = []
 
     for res in results:
         if res is not None:
             summary = _get_model_result_summary(res, include_all_estimation_steps)
             summary.insert(0, 'description', res.description)
             summaries.append(summary)
@@ -1018,17 +1022,17 @@
 
     Return
     ------
     ModelfitResults
         Results object
     """
     path = Path(path)
-    # FIXME: Quick and dirty solution
     model = read_model(path)
-    return mfr(model)
+    res = parse_modelfit_results(model, path)
+    return res
 
 
 def _get_run_setup_from_metadata(path):
     import pharmpy.workflows as workflows
 
     tool_database = workflows.default_tool_database(toolname=None, path=path, exist_ok=True)
 
@@ -1040,7 +1044,44 @@
     dispatcher = getattr(workflows, common_options['dispatcher'].split('.')[-1])
 
     # TODO be more general
     assert common_options['database']['class'] == 'LocalDirectoryToolDatabase'
     assert common_options['database']['toolname'] == tool_name
 
     return dispatcher, tool_database
+
+
+def load_example_modelfit_results(name: str):
+    """Load the modelfit results of an example model
+
+    Load the modelfit results of an example model built into Pharmpy
+
+    Parameters
+    ----------
+    name : str
+        Name of the model. Currently available models are "pheno" and "pheno_linear"
+
+    Returns
+    -------
+    ModelfitResults
+        Loaded modelfit results object
+
+    Example
+    -------
+    >>> from pharmpy.tools import load_example_modelfit_results
+    >>> results = load_example_modelfit_results("pheno")
+    >>> results.parameter_estimates
+        PTVCL        0.004696
+    PTVV         0.984258
+    THETA_3      0.158920
+    IVCL         0.029351
+    IVV          0.027906
+    SIGMA_1_1    0.013241
+    Name: estimates, dtype: float64
+
+    """
+    available = ('moxo', 'pheno', 'pheno_linear')
+    if name not in available:
+        raise ValueError(f'Unknown example model {name}. Available examples: {available}')
+    path = Path(__file__).resolve().parent.parent / 'modeling' / 'example_models' / (name + '.mod')
+    res = read_modelfit_results(path)
+    return res
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/ruvsearch/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/ruvsearch/tool.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/ruvsearch/tool.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,18 +69,19 @@
     Returns
     -------
     RUVSearchResults
         Ruvsearch tool result object
 
     Examples
     --------
-    >>> from pharmpy.modeling import *
+    >>> from pharmpy.modeling import load_example_model
+    >>> from pharmpy.tools import run_ruvsearch, load_example_modelfit_results
     >>> model = load_example_model("pheno")
-    >>> from pharmpy.tools import run_ruvsearch # doctest: +SKIP
-    >>> run_ruvsearch(model=model, results=model.modelfit_results)      # doctest: +SKIP
+    >>> results = load_example_modelfit_results("pheno")
+    >>> run_ruvsearch(model=model, results=results)      # doctest: +SKIP
 
     """
 
     wf = Workflow()
     wf.name = "ruvsearch"
     start_task = Task('start_ruvsearch', start, model, groups, p_value, skip)
     wf.add_task(start_task)
@@ -175,15 +176,15 @@
         else:
             skip.append(selected_model_name)
 
     sumind = summarize_individuals(selected_models)
     sumcount = summarize_individuals_count_table(df=sumind)
     summf = pd.concat(sum_models, keys=list(range(last_iteration)), names=['step'])
     summary_tool = _create_summary_tool(selected_models, cutoff)
-    summary_errors = summarize_errors(selected_models)
+    summary_errors = summarize_errors(m.modelfit_results for m in selected_models)
 
     res = RUVSearchResults(
         cwres_models=pd.concat(cwres_models),
         summary_individuals=sumind,
         summary_individuals_count=sumcount,
         final_model_name=model.name,
         summary_models=summf,
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/scm/psn_wrapper.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/scm/psn_wrapper.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/scm/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/scm/results.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/simeval/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/simeval/results.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,34 +3,35 @@
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Optional
 
 from pharmpy.deps import pandas as pd
 from pharmpy.model import Model, Results
 from pharmpy.modeling import plot_individual_predictions
+from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.simfit.results import psn_simfit_results
 
 
 @dataclass(frozen=True)
 class SimevalResults(Results):
     """Simeval results class"""
 
     sampled_iofv: Optional[Any] = None
     iofv_summary: Optional[Any] = None
     individual_predictions_plot: Optional[Any] = None
 
 
-def calculate_results(original_model, simfit_results):
+def calculate_results(original_model, original_results, simfit_results):
     """Calculate simeval results"""
     sampled_iofv = pd.concat(
         [res.individual_ofv for res in simfit_results.modelfit_results],
         axis=1,
         keys=range(1, len(simfit_results.modelfit_results) + 1),
     )
-    origiofv = original_model.modelfit_results.individual_ofv
+    origiofv = original_results.individual_ofv
     iofv_summary = pd.DataFrame(
         {
             'original': origiofv,
             'sampled_mean': sampled_iofv.T.mean(),
             'sampled_stdev': sampled_iofv.T.std(),
         }
     )
@@ -47,15 +48,15 @@
 
     ids = iofv_summary.index[iofv_summary['residual_outlier']].tolist()
     id_plot = None
     if ids:
         try:
             id_plot = plot_individual_predictions(
                 original_model,
-                original_model.modelfit_results.predictions[['IPRED', 'PRED']],
+                original_results.predictions[['IPRED', 'PRED']],
                 individuals=ids,
             )
         except Exception:
             pass
 
     res = SimevalResults(
         sampled_iofv=sampled_iofv,
@@ -65,16 +66,17 @@
     return res
 
 
 def psn_simeval_results(path):
     path = Path(path)
     simfit_paths = (path / 'm1').glob('sim-*.mod')
     simfit_results = psn_simfit_results(simfit_paths)
-    original = Model.create_model(path / 'm1' / 'original.mod')
-    res = calculate_results(original, simfit_results)
+    original = Model.parse_model(path / 'm1' / 'original.mod')
+    original_results = read_modelfit_results(path / 'm1' / 'original.mod')
+    res = calculate_results(original, original_results, simfit_results)
 
     # Add CWRES outliers as 2 in data_flag
     # Reading PsN results for now
     # df = pd.read_csv(path / 'summary_cwres.csv')
     # outliers = df['OUTLIER'].fillna(0).astype(int)
     # outliers.replace({1.0: 2}, inplace=True)
     # outliers = outliers + res.data_flag
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/simfit/results.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/simfit/results.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass
 from typing import Any, Optional
 
 from pharmpy.model import Model, Results
-from pharmpy.plugins.nonmem.results import simfit_results
+from pharmpy.tools.external.nonmem.results import simfit_results
 
 
 @dataclass(frozen=True)
 class SimfitResults(Results):
     """Simfit results class"""
 
     modelfit_results: Optional[Any] = None
@@ -16,11 +16,11 @@
     """Calculate simfit results"""
     return SimfitResults(modelfit_results=modelfit_results)
 
 
 def psn_simfit_results(paths):
     modelfit_results = []
     for path in paths:
-        model = Model.create_model(path)
+        model = Model.parse_model(path)
         modelfit_results.extend(simfit_results(model, path))
     res = calculate_results(modelfit_results)
     return res
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy/tools/wrap.py` & `pharmpy-core-0.96.0/src/pharmpy/tools/wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/visualization.py` & `pharmpy-core-0.96.0/src/pharmpy/visualization.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/__init__.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/args.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/args.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/call.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/dispatchers/local_dask.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/dispatchers/local_dask.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/execute.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/execute.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/log.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/log.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/baseclass.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/model_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/model_database/null_database.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/model_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/optimize.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/optimize.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/baseclass.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/tool_database/baseclass.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/local_directory.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/tool_database/local_directory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/tool_database/null_database.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/tool_database/null_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy/workflows/workflow.py` & `pharmpy-core-0.96.0/src/pharmpy/workflows/workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/src/pharmpy_core.egg-info/PKG-INFO` & `pharmpy-core-0.96.0/src/pharmpy_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pharmpy-core
-Version: 0.95.0
+Version: 0.96.0
 Summary: Pharmacometric modeling
 Home-page: https://pharmpy.github.io
 Author: Rikard Nordgren
 Author-email: rikard.nordgren@farmaci.uu.se
 License: GNU Lesser General Public License v3 (LGPLv3)
 Project-URL: Bug Tracker, https://github.com/pharmpy/pharmpy/issues
 Project-URL: Source Code, https://github.com/pharmpy/pharmpy
@@ -40,14 +40,34 @@
 * A model abstraction as a foundation for higher level operations on models
 * Functions for manipulation of models, e.g. changing model components like elimination or absorption
 * Reading NONMEM models and results
 * Running models and complex workflows (with NONMEM or to some extent nlmixr)
 
 This is the `team behind Pharmpy <https://pharmpy.github.io/latest/contributors.html>`_
 
+0.96.0 (2023-05-26)
+-------------------
+
+Changes
+=======
+
+* Rename functions handling the precision matrix (was previously referring to information matrix which was an error)
+* Remove saddle reset for default AMD model
+* Let LLQ column takes precedence over BLQ column
+
+New features
+============
+
+* Add tools.load_example_modelfit_results
+
+Bugfixes
+========
+
+* Fix bug where if-statements were reordered incorrectly
+
 0.95.0 (2023-05-22)
 -------------------
 
 Changes
 =======
 
 * ``ModelfitResults.ofv_iterations`` and ``ModelfitResults.parameter_estimates_iterations`` have NaN rows in failed runs
```

### Comparing `pharmpy-core-0.95.0/src/pharmpy_core.egg-info/SOURCES.txt` & `pharmpy-core-0.96.0/src/pharmpy_core.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -134,14 +134,64 @@
 src/pharmpy/model/parameters.py
 src/pharmpy/model/random_variables.py
 src/pharmpy/model/results.py
 src/pharmpy/model/statements.py
 src/pharmpy/model/distributions/__init__.py
 src/pharmpy/model/distributions/numeric.py
 src/pharmpy/model/distributions/symbolic.py
+src/pharmpy/model/external/__init__.py
+src/pharmpy/model/external/utils.py
+src/pharmpy/model/external/fcon/__init__.py
+src/pharmpy/model/external/fcon/model.py
+src/pharmpy/model/external/nlmixr/__init__.py
+src/pharmpy/model/external/nlmixr/error_model.py
+src/pharmpy/model/external/nlmixr/ini.py
+src/pharmpy/model/external/nlmixr/model.py
+src/pharmpy/model/external/nlmixr/model_block.py
+src/pharmpy/model/external/nlmixr/name_mangle.py
+src/pharmpy/model/external/nlmixr/sanity_checks.py
+src/pharmpy/model/external/nonmem/__init__.py
+src/pharmpy/model/external/nonmem/advan.py
+src/pharmpy/model/external/nonmem/dataset.py
+src/pharmpy/model/external/nonmem/detect.py
+src/pharmpy/model/external/nonmem/model.py
+src/pharmpy/model/external/nonmem/nmtran_parser.py
+src/pharmpy/model/external/nonmem/parsing.py
+src/pharmpy/model/external/nonmem/table.py
+src/pharmpy/model/external/nonmem/update.py
+src/pharmpy/model/external/nonmem/records/__init__.py
+src/pharmpy/model/external/nonmem/records/abbreviated_record.py
+src/pharmpy/model/external/nonmem/records/code_record.py
+src/pharmpy/model/external/nonmem/records/data_record.py
+src/pharmpy/model/external/nonmem/records/estimation_record.py
+src/pharmpy/model/external/nonmem/records/etas_record.py
+src/pharmpy/model/external/nonmem/records/factory.py
+src/pharmpy/model/external/nonmem/records/model_record.py
+src/pharmpy/model/external/nonmem/records/omega_record.py
+src/pharmpy/model/external/nonmem/records/option_record.py
+src/pharmpy/model/external/nonmem/records/parsers.py
+src/pharmpy/model/external/nonmem/records/problem_record.py
+src/pharmpy/model/external/nonmem/records/raw_record.py
+src/pharmpy/model/external/nonmem/records/record.py
+src/pharmpy/model/external/nonmem/records/simulation_record.py
+src/pharmpy/model/external/nonmem/records/sizes_record.py
+src/pharmpy/model/external/nonmem/records/subroutine_record.py
+src/pharmpy/model/external/nonmem/records/table_record.py
+src/pharmpy/model/external/nonmem/records/theta_record.py
+src/pharmpy/model/external/nonmem/records/grammars/abbreviated_record.lark
+src/pharmpy/model/external/nonmem/records/grammars/code_record.lark
+src/pharmpy/model/external/nonmem/records/grammars/data_record.lark
+src/pharmpy/model/external/nonmem/records/grammars/definitions.lark
+src/pharmpy/model/external/nonmem/records/grammars/omega_record.lark
+src/pharmpy/model/external/nonmem/records/grammars/option_record.lark
+src/pharmpy/model/external/nonmem/records/grammars/problem_record.lark
+src/pharmpy/model/external/nonmem/records/grammars/simulation_record.lark
+src/pharmpy/model/external/nonmem/records/grammars/theta_record.lark
+src/pharmpy/model/external/rxode/__init__.py
+src/pharmpy/model/external/rxode/model.py
 src/pharmpy/modeling/__init__.py
 src/pharmpy/modeling/allometry.py
 src/pharmpy/modeling/basic_models.py
 src/pharmpy/modeling/block_rvs.py
 src/pharmpy/modeling/blq.py
 src/pharmpy/modeling/common.py
 src/pharmpy/modeling/compartments.py
@@ -181,68 +231,14 @@
 src/pharmpy/modeling/example_models/pheno.phi
 src/pharmpy/modeling/example_models/pheno.tab
 src/pharmpy/modeling/example_models/pheno_linear.dta
 src/pharmpy/modeling/example_models/pheno_linear.ext
 src/pharmpy/modeling/example_models/pheno_linear.lst
 src/pharmpy/modeling/example_models/pheno_linear.mod
 src/pharmpy/modeling/example_models/pheno_linear.phi
-src/pharmpy/plugins/utils.py
-src/pharmpy/plugins/fcon/__init__.py
-src/pharmpy/plugins/fcon/model.py
-src/pharmpy/plugins/nlmixr/__init__.py
-src/pharmpy/plugins/nlmixr/error_model.py
-src/pharmpy/plugins/nlmixr/ini.py
-src/pharmpy/plugins/nlmixr/model.py
-src/pharmpy/plugins/nlmixr/model_block.py
-src/pharmpy/plugins/nlmixr/name_mangle.py
-src/pharmpy/plugins/nlmixr/run.py
-src/pharmpy/plugins/nlmixr/sanity_checks.py
-src/pharmpy/plugins/nonmem/__init__.py
-src/pharmpy/plugins/nonmem/advan.py
-src/pharmpy/plugins/nonmem/config.py
-src/pharmpy/plugins/nonmem/dataset.py
-src/pharmpy/plugins/nonmem/detect.py
-src/pharmpy/plugins/nonmem/model.py
-src/pharmpy/plugins/nonmem/nmtran_parser.py
-src/pharmpy/plugins/nonmem/parsing.py
-src/pharmpy/plugins/nonmem/results.py
-src/pharmpy/plugins/nonmem/results_file.py
-src/pharmpy/plugins/nonmem/run.py
-src/pharmpy/plugins/nonmem/table.py
-src/pharmpy/plugins/nonmem/update.py
-src/pharmpy/plugins/nonmem/records/__init__.py
-src/pharmpy/plugins/nonmem/records/abbreviated_record.py
-src/pharmpy/plugins/nonmem/records/code_record.py
-src/pharmpy/plugins/nonmem/records/data_record.py
-src/pharmpy/plugins/nonmem/records/estimation_record.py
-src/pharmpy/plugins/nonmem/records/etas_record.py
-src/pharmpy/plugins/nonmem/records/factory.py
-src/pharmpy/plugins/nonmem/records/model_record.py
-src/pharmpy/plugins/nonmem/records/omega_record.py
-src/pharmpy/plugins/nonmem/records/option_record.py
-src/pharmpy/plugins/nonmem/records/parsers.py
-src/pharmpy/plugins/nonmem/records/problem_record.py
-src/pharmpy/plugins/nonmem/records/raw_record.py
-src/pharmpy/plugins/nonmem/records/record.py
-src/pharmpy/plugins/nonmem/records/simulation_record.py
-src/pharmpy/plugins/nonmem/records/sizes_record.py
-src/pharmpy/plugins/nonmem/records/subroutine_record.py
-src/pharmpy/plugins/nonmem/records/table_record.py
-src/pharmpy/plugins/nonmem/records/theta_record.py
-src/pharmpy/plugins/nonmem/records/grammars/abbreviated_record.lark
-src/pharmpy/plugins/nonmem/records/grammars/code_record.lark
-src/pharmpy/plugins/nonmem/records/grammars/data_record.lark
-src/pharmpy/plugins/nonmem/records/grammars/definitions.lark
-src/pharmpy/plugins/nonmem/records/grammars/omega_record.lark
-src/pharmpy/plugins/nonmem/records/grammars/option_record.lark
-src/pharmpy/plugins/nonmem/records/grammars/problem_record.lark
-src/pharmpy/plugins/nonmem/records/grammars/simulation_record.lark
-src/pharmpy/plugins/nonmem/records/grammars/theta_record.lark
-src/pharmpy/plugins/rxode/__init__.py
-src/pharmpy/plugins/rxode/model.py
 src/pharmpy/reporting/altairplot.py
 src/pharmpy/reporting/conf.py
 src/pharmpy/reporting/custom.css
 src/pharmpy/reporting/reporting.py
 src/pharmpy/tools/__init__.py
 src/pharmpy/tools/common.py
 src/pharmpy/tools/psn_helpers.py
@@ -269,14 +265,25 @@
 src/pharmpy/tools/crossval/results.py
 src/pharmpy/tools/estmethod/__init__.py
 src/pharmpy/tools/estmethod/algorithms.py
 src/pharmpy/tools/estmethod/report.rst
 src/pharmpy/tools/estmethod/tool.py
 src/pharmpy/tools/evaldesign/__init__.py
 src/pharmpy/tools/evaldesign/tool.py
+src/pharmpy/tools/external/__init__.py
+src/pharmpy/tools/external/results.py
+src/pharmpy/tools/external/nlmixr/__init__.py
+src/pharmpy/tools/external/nlmixr/run.py
+src/pharmpy/tools/external/nonmem/__init__.py
+src/pharmpy/tools/external/nonmem/config.py
+src/pharmpy/tools/external/nonmem/results.py
+src/pharmpy/tools/external/nonmem/results_file.py
+src/pharmpy/tools/external/nonmem/run.py
+src/pharmpy/tools/external/rxode/__init__.py
+src/pharmpy/tools/external/rxode/run.py
 src/pharmpy/tools/frem/__init__.py
 src/pharmpy/tools/frem/models.py
 src/pharmpy/tools/frem/report.rst
 src/pharmpy/tools/frem/results.py
 src/pharmpy/tools/frem/tool.py
 src/pharmpy/tools/funcs/__init__.py
 src/pharmpy/tools/funcs/ml.py
@@ -316,15 +323,14 @@
 src/pharmpy/tools/mfl/statement/feature/elimination.py
 src/pharmpy/tools/mfl/statement/feature/feature.py
 src/pharmpy/tools/mfl/statement/feature/lagtime.py
 src/pharmpy/tools/mfl/statement/feature/peripherals.py
 src/pharmpy/tools/mfl/statement/feature/symbols.py
 src/pharmpy/tools/mfl/statement/feature/transits.py
 src/pharmpy/tools/modelfit/__init__.py
-src/pharmpy/tools/modelfit/results.py
 src/pharmpy/tools/modelfit/tool.py
 src/pharmpy/tools/modelsearch/__init__.py
 src/pharmpy/tools/modelsearch/algorithms.py
 src/pharmpy/tools/modelsearch/tool.py
 src/pharmpy/tools/qa/__init__.py
 src/pharmpy/tools/qa/results.py
 src/pharmpy/tools/ruvsearch/__init__.py
@@ -365,14 +371,17 @@
 src/pharmpy_core.egg-info/top_level.txt
 tests/__init__.py
 tests/conftest.py
 tests/lib.py
 tests/cli/test_cli.py
 tests/config/test_config.py
 tests/deps/test_deps.py
+tests/external/test_external.py
+tests/external/test_nlmixr.py
+tests/external/test_rxode.py
 tests/integration/conftest.py
 tests/integration/test_allometry.py
 tests/integration/test_amd.py
 tests/integration/test_bootstrap.py
 tests/integration/test_common.py
 tests/integration/test_covsearch.py
 tests/integration/test_estmethod.py
@@ -447,17 +456,14 @@
 tests/nonmem/records/test_omega.py
 tests/nonmem/records/test_option_record.py
 tests/nonmem/records/test_problem.py
 tests/nonmem/records/test_simulation.py
 tests/nonmem/records/test_sizes.py
 tests/nonmem/records/test_subroutines.py
 tests/nonmem/records/test_theta.py
-tests/plugins/test_nlmixr.py
-tests/plugins/test_plugins.py
-tests/plugins/test_rxode.py
 tests/testdata/pheno_data.csv
 tests/testdata/frem/results.json
 tests/testdata/nonmem/DDMODEL00000130
 tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv
 tests/testdata/nonmem/file.csv
 tests/testdata/nonmem/minimal.mod
 tests/testdata/nonmem/pheno.datainfo
@@ -548,14 +554,15 @@
 tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod
 tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod
 tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod
 tests/testdata/nonmem/errors/control_stream_error.lst
 tests/testdata/nonmem/errors/est_step_warning.lst
 tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst
 tests/testdata/nonmem/errors/failed_run.ext
+tests/testdata/nonmem/errors/failed_run.mod
 tests/testdata/nonmem/errors/no_header_error.ext
 tests/testdata/nonmem/errors/no_header_error.lst
 tests/testdata/nonmem/errors/rounding_error.lst
 tests/testdata/nonmem/errors/run_interrupted.ext
 tests/testdata/nonmem/errors/run_interrupted.mod
 tests/testdata/nonmem/errors/zero_gradient_error.lst
 tests/testdata/nonmem/fcon/FCON
@@ -1011,15 +1018,14 @@
 tests/tools/test_exports.py
 tests/tools/test_frem.py
 tests/tools/test_iivsearch.py
 tests/tools/test_iovsearch.py
 tests/tools/test_linearize.py
 tests/tools/test_mfl.py
 tests/tools/test_ml.py
-tests/tools/test_modelfit.py
 tests/tools/test_modelsearch.py
 tests/tools/test_qa.py
 tests/tools/test_rankfuncs.py
 tests/tools/test_run.py
 tests/tools/test_runtool.py
 tests/tools/test_ruvsearch.py
 tests/tools/test_scm.py
```

### Comparing `pharmpy-core-0.95.0/tests/cli/test_cli.py` & `pharmpy-core-0.96.0/tests/cli/test_cli.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/conftest.py` & `pharmpy-core-0.96.0/tests/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
     _cache: Dict[Hashable, Model] = {}
 
     def _load(given_path: Union[str, Path]) -> Model:
         # TODO Cache based on file contents instead.
 
         def _parse_model():
-            model = Model.create_model(given_path)
+            model = Model.parse_model(given_path)
             try:
                 model.dataset  # NOTE Force parsing of dataset
             except FileNotFoundError:
                 pass  # NOTE The error will resurface later if needed
             return model
 
         basetemp = tmp_path_factory.getbasetemp().resolve()
@@ -52,15 +52,15 @@
             resolved_path.relative_to(basetemp)
             return _parse_model()
         except ValueError:
             # NOTE This is raised when resolved_path is not descendant of
             # basetemp. With Python >= 3.9 we could use is_relative_to instead.
             pass
 
-        from pharmpy.plugins.nonmem import conf
+        from pharmpy.tools.external.nonmem import conf
 
         key = (str(conf), str(resolved_path))
 
         if key not in _cache:
             _cache[key] = _parse_model()
 
         return _cache[key]
@@ -75,34 +75,32 @@
 
     _cache: Dict[Hashable, Model] = {}
 
     def _load(given_name: str) -> Model:
         def _parse_model():
             return load_example_model(given_name)
 
-        from pharmpy.plugins.nonmem import conf
+        from pharmpy.tools.external.nonmem import conf
 
         key = (str(conf), given_name)
 
         if key not in _cache:
             _cache[key] = _parse_model()
 
         return _cache[key]
 
     return _load
 
 
 @pytest.fixture(scope='session')
 def create_model_for_test(load_example_model_for_test):
-    from io import StringIO
-
     from pharmpy.model import Model
 
     def _create(code: str, dataset: Optional[str] = None) -> Model:
-        model = Model.create_model(StringIO(code))
+        model = Model.parse_model_from_string(code)
         datapath = model.datainfo.path
         if dataset is not None:
             # NOTE This yields a copy of the dataset through Model#copy
             model = model.replace(
                 dataset=load_example_model_for_test(dataset).dataset,
                 datainfo=model.datainfo.replace(path=datapath),
             )
```

### Comparing `pharmpy-core-0.95.0/tests/integration/conftest.py` & `pharmpy-core-0.96.0/tests/integration/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @pytest.fixture(scope='session')
 def start_model(testdata):
     tempdir = Path(tempfile.mkdtemp())
     with chdir(tempdir):
         shutil.copy2(testdata / 'nonmem' / 'models' / 'mox2.mod', tempdir)
         shutil.copy2(testdata / 'nonmem' / 'models' / 'mox_simulated_normal.csv', tempdir)
-        model_start = Model.create_model('mox2.mod')
+        model_start = Model.parse_model('mox2.mod')
         model_start = model_start.replace(
             datainfo=model_start.datainfo.replace(path=tempdir / 'mox_simulated_normal.csv')
         )
         modelfit_results = fit(model_start)
         # FIXME: Remove
         model_start = model_start.replace(modelfit_results=modelfit_results)
     return model_start
```

### Comparing `pharmpy-core-0.95.0/tests/integration/test_allometry.py` & `pharmpy-core-0.96.0/tests/integration/test_allometry.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 import os.path
 import shutil
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Model
-from pharmpy.tools import run_tool
+from pharmpy.tools import read_modelfit_results, run_tool
 from pharmpy.workflows import ModelDatabase
 
 
 def test_allometry(tmp_path, testdata):
     with chdir(tmp_path):
         for path in (testdata / 'nonmem').glob('pheno_real.*'):
             shutil.copy2(path, tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'sdtab1', tmp_path)
 
-        model = Model.create_model('pheno_real.mod')
+        model = Model.parse_model('pheno_real.mod')
+        results = read_modelfit_results('pheno_real.mod')
         datainfo = model.datainfo.replace(path=tmp_path / 'pheno.dta')
         model = model.replace(datainfo=datainfo)
-        res = run_tool(
-            'allometry', model, results=model.modelfit_results, allometric_variable='WGT'
-        )
+        res = run_tool('allometry', model=model, results=results, allometric_variable='WGT')
         assert len(res.summary_models) == 2
 
         db: ModelDatabase = res.tool_database.model_database
         sep = os.path.sep
         model_name = 'scaled_model'
         assert str(db.retrieve_model(model_name).datainfo.path).endswith(
             f'{sep}allometry_dir1{sep}models{sep}.datasets{sep}input_model.csv'
```

### Comparing `pharmpy-core-0.95.0/tests/integration/test_amd.py` & `pharmpy-core-0.96.0/tests/integration/test_amd.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/integration/test_bootstrap.py` & `pharmpy-core-0.96.0/tests/integration/test_evaldesign.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import shutil
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Model
 from pharmpy.tools import run_tool
 
 
-def test_bootstrap(tmp_path, testdata):
+def test_evaldesign(tmp_path, testdata):
     with chdir(tmp_path):
-        shutil.copy2(testdata / 'nonmem' / 'pheno.mod', tmp_path)
+        for path in (testdata / 'nonmem').glob('pheno_real.*'):
+            shutil.copy2(path, tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path)
-        shutil.copy2(testdata / 'nonmem' / 'pheno.ext', tmp_path)
-        shutil.copy2(testdata / 'nonmem' / 'pheno.lst', tmp_path)
-        model = Model.create_model('pheno.mod')
+        shutil.copy2(testdata / 'nonmem' / 'sdtab1', tmp_path)
+
+        model = Model.parse_model('pheno_real.mod')
         model = model.replace(datainfo=model.datainfo.replace(path=tmp_path / 'pheno.dta'))
-        res = run_tool('bootstrap', model, resamples=3)
-        assert len(res.parameter_estimates) == 3
+        res = run_tool('evaldesign', model)
+        assert len(res.individual_ofv) == 59
```

### Comparing `pharmpy-core-0.95.0/tests/integration/test_common.py` & `pharmpy-core-0.96.0/tests/integration/test_common.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/integration/test_covsearch.py` & `pharmpy-core-0.96.0/tests/integration/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/integration/test_fit.py` & `pharmpy-core-0.96.0/tests/integration/test_fit.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,30 +3,30 @@
 import pandas as pd
 import pytest
 
 import pharmpy.modeling as modeling
 from pharmpy.config import site_config_path, user_config_path
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Model
-from pharmpy.plugins.nonmem import conf
 from pharmpy.tools import fit
+from pharmpy.tools.external.nonmem import conf
 
 
 def test_configuration():
     print("User config dir:", user_config_path())
     print("Site config dir:", site_config_path())
     print("Default NONMEM path:", conf.default_nonmem_path)
     assert (conf.default_nonmem_path / 'license' / 'nonmem.lic').is_file()
 
 
 def test_fit_single(tmp_path, model_count, testdata):
     with chdir(tmp_path):
         shutil.copy2(testdata / 'nonmem' / 'pheno.mod', tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path)
-        model = Model.create_model('pheno.mod')
+        model = Model.parse_model('pheno.mod')
         model = model.replace(datainfo=model.datainfo.replace(path=tmp_path / 'pheno.dta'))
         res = fit(model)
         rundir = tmp_path / 'modelfit_dir1'
         assert res.ofv == pytest.approx(730.8947268137308)
         assert rundir.is_dir()
         assert model_count(rundir) == 1
         assert (rundir / 'models' / 'pheno' / '.pharmpy').exists()
@@ -35,22 +35,22 @@
         ]
 
 
 def test_fit_multiple(tmp_path, model_count, testdata):
     with chdir(tmp_path):
         shutil.copy2(testdata / 'nonmem' / 'pheno.mod', tmp_path / 'pheno_1.mod')
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path / 'pheno_1.dta')
-        model_1 = Model.create_model('pheno_1.mod')
+        model_1 = Model.parse_model('pheno_1.mod')
         df = pd.read_table(tmp_path / 'pheno_1.dta', sep=r'\s+', header=0)
         model_1 = model_1.replace(
             dataset=df, datainfo=model_1.datainfo.replace(path=tmp_path / 'pheno_1.dta')
         )
         shutil.copy2(testdata / 'nonmem' / 'pheno.mod', tmp_path / 'pheno_2.mod')
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path / 'pheno_2.dta')
-        model_2 = Model.create_model('pheno_2.mod')
+        model_2 = Model.parse_model('pheno_2.mod')
         model_2 = model_2.replace(
             dataset=df, datainfo=model_2.datainfo.replace(path=tmp_path / 'pheno_2.dta')
         )
         res1, res2 = fit([model_1, model_2])
         rundir = tmp_path / 'modelfit_dir1'
         assert res1.ofv == pytest.approx(730.8947268137308)
         assert res2.ofv == pytest.approx(730.8947268137308)
@@ -59,15 +59,15 @@
 
 
 def test_fit_copy(tmp_path, model_count, testdata):
     with chdir(tmp_path):
         shutil.copy2(testdata / 'nonmem' / 'pheno.mod', tmp_path / 'pheno.mod')
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path / 'pheno.dta')
 
-        model_1 = Model.create_model('pheno.mod')
+        model_1 = Model.parse_model('pheno.mod')
         model_1 = model_1.replace(datainfo=model_1.datainfo.replace(path=tmp_path / 'pheno.dta'))
         res1 = fit(model_1)
 
         rundir_1 = tmp_path / 'modelfit_dir1'
         assert rundir_1.is_dir()
         assert model_count(rundir_1) == 1
 
@@ -79,20 +79,20 @@
         assert rundir_2.is_dir()
         assert model_count(rundir_2) == 1
 
         assert res1.ofv != res2.ofv
 
 
 def test_fit_nlmixr(tmp_path, testdata):
-    from pharmpy.plugins.nlmixr import conf
+    from pharmpy.tools.external.nlmixr import conf
 
     if str(conf.rpath) == '.':
         pytest.skip("No R selected in conf. Skipping nlmixr tests")
     with chdir(tmp_path):
         shutil.copy2(testdata / 'nonmem' / 'pheno.mod', tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path)
-        model = Model.create_model('pheno.mod')
+        model = Model.parse_model('pheno.mod')
         model = model.replace(datainfo=model.datainfo.replace(path=tmp_path / 'pheno.dta'))
         model = modeling.convert_model(model, 'nlmixr')
         res = fit(model, tool='nlmixr')
-        assert res.ofv == pytest.approx(732.58928)
-        assert res.parameter_estimates['TVCL'] == pytest.approx(0.0058614, abs=1e-6)
+        assert res.ofv == pytest.approx(732.58813)
+        assert res.parameter_estimates['TVCL'] == pytest.approx(0.0058686, abs=1e-6)
```

### Comparing `pharmpy-core-0.95.0/tests/integration/test_iivsearch.py` & `pharmpy-core-0.96.0/tests/integration/test_iivsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/integration/test_iovsearch.py` & `pharmpy-core-0.96.0/tests/integration/test_iovsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         assert res.final_model_name == 'iovsearch_run7'
 
 
 def test_default_mox1(tmp_path, model_count, testdata):
     shutil.copy2(testdata / 'nonmem' / 'models' / 'mox1.mod', tmp_path)
     shutil.copy2(testdata / 'nonmem' / 'models' / 'mox_simulated_log.csv', tmp_path)
     with chdir(tmp_path):
-        start_model = Model.create_model('mox1.mod')
+        start_model = Model.parse_model('mox1.mod')
         start_res = fit(start_model)
         start_model = start_model.replace(modelfit_results=start_res)
         res = run_iovsearch('VISI', results=start_res, model=start_model)
         rundir = tmp_path / 'iovsearch_dir1'
         assert model_count(rundir) == 7
 
         assert res.final_model_name == start_model.name
```

### Comparing `pharmpy-core-0.95.0/tests/integration/test_modelsearch.py` & `pharmpy-core-0.96.0/tests/integration/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/integration/test_resume.py` & `pharmpy-core-0.96.0/tests/integration/test_resume.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,34 +2,36 @@
 
 import pytest
 from pandas.testing import assert_frame_equal
 
 from pharmpy.config import ConfigurationContext
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Model
-from pharmpy.plugins.nonmem import conf
-from pharmpy.tools import fit, resume_tool, run_tool
+from pharmpy.tools import fit, read_modelfit_results, resume_tool, run_tool
+from pharmpy.tools.external.nonmem import conf
 
 
 def test_run_tool_ruvsearch_resume_flag(tmp_path, testdata):
     with chdir(tmp_path):
         for path in (testdata / 'nonmem').glob('pheno_real.*'):
             shutil.copy2(path, tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'sdtab1', tmp_path)
         # FIXME: temporary workaround so that read in parameter estimates use the Pharmpy name
         with ConfigurationContext(conf, parameter_names=['comment', 'basic']):
-            model = Model.create_model('pheno_real.mod')
+            model = Model.parse_model('pheno_real.mod')
+            results = read_modelfit_results('pheno_real.mod')
             model = model.replace(datainfo=model.datainfo.replace(path=tmp_path / 'pheno.dta'))
             path = 'x'
             for i, resume in enumerate([False, False, True]):
                 try:
                     res = run_tool(
                         'ruvsearch',
-                        model,
+                        model=model,
+                        results=results,
                         groups=4,
                         p_value=0.05,
                         skip=[],
                         path=path,
                         resume=resume,
                     )
                     if i != 0 and not resume:
@@ -44,15 +46,15 @@
 
 def test_run_tool_iivsearch_resume_flag(tmp_path, testdata, model_count):
     with chdir(tmp_path):
         shutil.copy2(testdata / 'nonmem' / 'models' / 'mox2.mod', tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'models' / 'mox_simulated_normal.csv', tmp_path)
         # FIXME: temporary workaround so that read in parameter estimates use the Pharmpy name
         with ConfigurationContext(conf, parameter_names=['comment', 'basic']):
-            model_start = Model.create_model('mox2.mod')
+            model_start = Model.parse_model('mox2.mod')
             model_start = model_start.replace(
                 datainfo=model_start.datainfo.replace(path=tmp_path / 'mox_simulated_normal.csv')
             )
             start_res = fit(model_start)
             # FIXME: Remove
             model_start = model_start.replace(modelfit_results=start_res)
 
@@ -98,15 +100,15 @@
     tmp_path, testdata, model_count, search_space, no_of_models, last_model_parent_name
 ):
     shutil.copy2(testdata / 'nonmem' / 'models' / 'mox2.mod', tmp_path)
     shutil.copy2(testdata / 'nonmem' / 'models' / 'mox_simulated_normal.csv', tmp_path)
     # FIXME: temporary workaround so that read in parameter estimates use the Pharmpy name
     with chdir(tmp_path):
         with ConfigurationContext(conf, parameter_names=['comment', 'basic']):
-            model_start = Model.create_model('mox2.mod')
+            model_start = Model.parse_model('mox2.mod')
             model_start = model_start.replace(
                 datainfo=model_start.datainfo.replace(path=tmp_path / 'mox_simulated_normal.csv')
             )
 
             start_res = fit(model_start)
             model_start = model_start.replace(modelfit_results=start_res)
 
@@ -160,21 +162,22 @@
 def test_resume_tool_ruvsearch(tmp_path, testdata):
     with chdir(tmp_path):
         for path in (testdata / 'nonmem').glob('pheno_real.*'):
             shutil.copy2(path, tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'pheno.dta', tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'sdtab1', tmp_path)
 
-        model = Model.create_model('pheno_real.mod')
+        model = Model.parse_model('pheno_real.mod')
+        results = read_modelfit_results('pheno_real.mod')
         model = model.replace(datainfo=model.datainfo.replace(path=tmp_path / 'pheno.dta'))
         path = 'x'
         run_tool_res = run_tool(
             'ruvsearch',
-            model,
-            results=model.modelfit_results,
+            model=model,
+            results=results,
             groups=4,
             p_value=0.05,
             skip=[],
             path=path,
         )
         assert run_tool_res
```

### Comparing `pharmpy-core-0.95.0/tests/integration/test_ruvsearch.py` & `pharmpy-core-0.96.0/tests/integration/test_ruvsearch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import shutil
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import Model
 from pharmpy.modeling import remove_covariance_step
-from pharmpy.tools import retrieve_final_model, run_tool
+from pharmpy.tools import read_modelfit_results, retrieve_final_model, run_tool
 
 
 def test_ruvsearch(tmp_path, testdata):
     with chdir(tmp_path):
         for path in (testdata / 'nonmem' / 'ruvsearch').glob('mox3.*'):
             shutil.copy2(path, tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'ruvsearch' / 'moxo_simulated_resmod.csv', tmp_path)
         shutil.copy2(testdata / 'nonmem' / 'ruvsearch' / 'mytab', tmp_path)
 
-        model = Model.create_model('mox3.mod')
+        model = Model.parse_model('mox3.mod')
+        results = read_modelfit_results('mox3.mod')
         model = remove_covariance_step(model)
         model = model.replace(
             datainfo=model.datainfo.replace(path=tmp_path / 'moxo_simulated_resmod.csv')
         )
-        res = run_tool(
-            'ruvsearch', model, results=model.modelfit_results, groups=4, p_value=0.05, skip=[]
-        )
+        res = run_tool('ruvsearch', model=model, results=results, groups=4, p_value=0.05, skip=[])
         iteration = [1, 1, 1, 1, 1, 1, 2, 2, 2, 2, 2, 3, 3]
         best_model = retrieve_final_model(res)
         assert (res.cwres_models.index.get_level_values('iteration') == iteration).all()
         assert best_model.model_code.split('\n')[12] == 'IF (TAD.LT.6.08) THEN'
         assert (
             best_model.model_code.split('\n')[13]
             == '    Y = A(2)/VC + A(2)*EPS(1)*THETA(4)*EXP(ETA_RV1)/VC'
```

### Comparing `pharmpy-core-0.95.0/tests/internals/fs/test_lock.py` & `pharmpy-core-0.96.0/tests/internals/fs/test_lock.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/internals/module/test_lazy.py` & `pharmpy-core-0.96.0/tests/internals/module/test_lazy.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/internals/test_math.py` & `pharmpy-core-0.96.0/tests/internals/test_math.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/internals/test_parse.py` & `pharmpy-core-0.96.0/tests/internals/test_parse.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/model/test_datainfo.py` & `pharmpy-core-0.96.0/tests/model/test_datainfo.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/model/test_estimation.py` & `pharmpy-core-0.96.0/tests/model/test_estimation.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/model/test_model.py` & `pharmpy-core-0.96.0/tests/model/test_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import pytest
 
 from pharmpy.deps import sympy
 from pharmpy.model import Assignment, Model
+from pharmpy.model.external.nonmem.dataset import read_nonmem_dataset
 from pharmpy.modeling import convert_model, create_symbol, load_example_model
-from pharmpy.plugins.nonmem.dataset import read_nonmem_dataset
 
 tabpath = Path(__file__).resolve().parent.parent / 'testdata' / 'nonmem' / 'pheno_real_linbase.tab'
 lincorrect = read_nonmem_dataset(
     tabpath,
     ignore_character='@',
     colnames=['ID', 'G11', 'G21', 'H11', 'CIPREDI', 'DV', 'PRED', 'RES', 'WRES'],
 )
```

### Comparing `pharmpy-core-0.95.0/tests/model/test_parameter.py` & `pharmpy-core-0.96.0/tests/model/test_parameter.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/model/test_random_variables.py` & `pharmpy-core-0.96.0/tests/model/test_random_variables.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/model/test_statements.py` & `pharmpy-core-0.96.0/tests/model/test_statements.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_add_covariate_effect.py` & `pharmpy-core-0.96.0/tests/modeling/test_add_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_allometry.py` & `pharmpy-core-0.96.0/tests/modeling/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_block_rvs.py` & `pharmpy-core-0.96.0/tests/modeling/test_block_rvs.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pytest
 from sympy import Symbol as S
 
 from pharmpy.model import NormalDistribution
 from pharmpy.modeling import add_iiv, create_joint_distribution
 from pharmpy.modeling.block_rvs import _choose_param_init
-from pharmpy.results import ModelfitResults
+from pharmpy.tools import read_modelfit_results
 
 
 @pytest.mark.parametrize(
     'rvs, exception_msg',
     [
         (['ETA_3', 'NON_EXISTENT_RV'], r'.*non-existing.*'),
         (['ETA_3', 'ETA_6'], r'.*ETA_6.*'),
@@ -17,65 +17,53 @@
 )
 def test_incorrect_params(load_model_for_test, testdata, rvs, exception_msg):
     model = load_model_for_test(
         testdata / 'nonmem' / 'modelfit_results' / 'onePROB' / 'multEST' / 'noSIM' / 'withBayes.mod'
     )
 
     with pytest.raises(Exception, match=exception_msg):
-        create_joint_distribution(
-            model, rvs, individual_estimates=model.modelfit_results.individual_estimates
-        )
+        create_joint_distribution(model, rvs, individual_estimates=None)
 
 
 def test_choose_param_init(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
+    res = read_modelfit_results(pheno_path)
     params = (model.parameters['IVCL'], model.parameters['IVV'])
     rvs = model.random_variables.etas
-    init = _choose_param_init(model, model.modelfit_results.individual_estimates, rvs, *params)
+    init = _choose_param_init(model, res.individual_estimates, rvs, *params)
     assert init == 0.0118179
 
     model = load_model_for_test(pheno_path)
-    model = model.replace(modelfit_results=None)
     init = _choose_param_init(model, None, rvs, *params)
     assert init == 0.0031045
 
     model = load_model_for_test(pheno_path)
     rv_new = NormalDistribution.create('ETA_3', 'IIV', 0, S('OMEGA_3_3'))
     rvs += rv_new
-    res = model.modelfit_results
     ie = res.individual_estimates.copy()
     ie['ETA_3'] = ie['ETA_1']
-    modelfit_results = ModelfitResults(
-        parameter_estimates=res.parameter_estimates, individual_estimates=ie
-    )
-    model = model.replace(modelfit_results=modelfit_results)
     init = _choose_param_init(model, res.individual_estimates, rvs, *params)
     assert init == 0.0118179
 
     # If one eta doesn't have individual estimates
     model = load_model_for_test(pheno_path)
     model = add_iiv(model, 'S1', 'add')
     params = (model.parameters['IVCL'], model.parameters['IIV_S1'])
     rvs = model.random_variables[('ETA_1', 'ETA_S1')]
-    init = _choose_param_init(model, model.modelfit_results.individual_estimates, rvs, *params)
+    init = _choose_param_init(model, res.individual_estimates, rvs, *params)
     assert init == 0.0052789
 
     # If the standard deviation in individual estimates of one eta is 0
     model = load_model_for_test(pheno_path)
-    res = model.modelfit_results
     ie = res.individual_estimates.copy()
     ie['ETA_1'] = 0
-    modelfit_results = ModelfitResults(
-        parameter_estimates=res.parameter_estimates, individual_estimates=ie
-    )
-    model = model.replace(modelfit_results=modelfit_results)
     params = (model.parameters['IVCL'], model.parameters['IVV'])
     rvs = model.random_variables[('ETA_1', 'ETA_2')]
     with pytest.warns(UserWarning, match='Correlation of individual estimates'):
-        init = _choose_param_init(model, model.modelfit_results.individual_estimates, rvs, *params)
+        init = _choose_param_init(model, ie, rvs, *params)
         assert init == 0.0031045
 
 
 def test_choose_param_init_fo(create_model_for_test):
     model = create_model_for_test(
         '''$PROBLEM PHENOBARB SIMPLE MODEL
 $DATA pheno.dta IGNORE=@
```

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_common.py` & `pharmpy-core-0.96.0/tests/modeling/test_common.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import os.path
 from pathlib import Path
 
 import pytest
 import sympy
 
 from pharmpy.model import Model as BaseModel
+from pharmpy.model.external.nlmixr.model import Model as nlmixrModel
+from pharmpy.model.external.nonmem import Model as NMModel
 from pharmpy.modeling import (
     convert_model,
     create_basic_pk_model,
     create_joint_distribution,
     fix_parameters,
     get_config_path,
     get_model_code,
@@ -16,16 +18,15 @@
     load_example_model,
     read_model,
     read_model_from_string,
     remove_unused_parameters_and_rvs,
     set_name,
     write_model,
 )
-from pharmpy.plugins.nlmixr.model import Model as nlmixrModel
-from pharmpy.plugins.nonmem.model import Model as NMModel
+from pharmpy.tools import read_modelfit_results
 
 
 def test_get_config_path():
     with pytest.warns(UserWarning):
         assert get_config_path() is None
 
 
@@ -84,15 +85,14 @@
     model = fix_parameters(model, ['THETA_1'])
     assert get_model_code(model).split('\n')[7] == '$THETA 0.1 FIX'
 
 
 def test_load_example_model():
     model = load_example_model("pheno")
     assert len(model.parameters) == 6
-    assert len(model.modelfit_results.parameter_estimates) == 6
 
     model = load_example_model("moxo")
     assert len(model.parameters) == 11
 
     with pytest.raises(ValueError):
         load_example_model("grekztalb23=")
 
@@ -131,17 +131,17 @@
 
     assert base.name == run3.name
     # Only checking parameters due to NONMEM parametrizations
     assert base.parameters == run3.parameters
     assert isinstance(run3, NMModel)
 
 
-def test_remove_unused_parameters_and_rvs(pheno):
+def test_remove_unused_parameters_and_rvs(load_model_for_test, pheno_path):
+    pheno = load_model_for_test(pheno_path)
+    res = read_modelfit_results(pheno_path)
     model = remove_unused_parameters_and_rvs(pheno)
-    model = create_joint_distribution(
-        model, individual_estimates=model.modelfit_results.individual_estimates
-    )
+    model = create_joint_distribution(model, individual_estimates=res.individual_estimates)
     statements = model.statements
     i = statements.index(statements.find_assignment('CL'))
     model = model.replace(statements=model.statements[0:i] + model.statements[i + 1 :])
     model = remove_unused_parameters_and_rvs(model)
     assert len(model.random_variables['ETA_2'].names) == 1
```

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_covariate_effect.py` & `pharmpy-core-0.96.0/tests/modeling/test_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_data_funcs.py` & `pharmpy-core-0.96.0/tests/modeling/test_data_funcs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_distribution.py` & `pharmpy-core-0.96.0/tests/modeling/test_distribution.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_error.py` & `pharmpy-core-0.96.0/tests/modeling/test_error.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_estimation_steps.py` & `pharmpy-core-0.96.0/tests/modeling/test_estimation_steps.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_eta_additions.py` & `pharmpy-core-0.96.0/tests/modeling/test_eta_additions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_eta_transformations.py` & `pharmpy-core-0.96.0/tests/modeling/test_eta_transformations.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_evaluate.py` & `pharmpy-core-0.96.0/tests/modeling/test_evaluate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from io import StringIO
 from pathlib import Path
 
 import pandas as pd
 import pytest
 
+from pharmpy.model.external.nonmem.dataset import read_nonmem_dataset
 from pharmpy.modeling import (
     evaluate_epsilon_gradient,
     evaluate_eta_gradient,
     evaluate_expression,
     evaluate_individual_prediction,
     evaluate_population_prediction,
     evaluate_weighted_residuals,
 )
-from pharmpy.plugins.nonmem.dataset import read_nonmem_dataset
+from pharmpy.tools import read_modelfit_results
 
 tabpath = Path(__file__).resolve().parent.parent / 'testdata' / 'nonmem' / 'pheno_real_linbase.tab'
 lincorrect = read_nonmem_dataset(
     tabpath,
     ignore_character='@',
     colnames=['ID', 'G11', 'G21', 'H11', 'CIPREDI', 'DV', 'PRED', 'RES', 'WRES'],
 )
 
 
 def test_evaluate_expression(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'pheno_noifs.mod')
-    ser = evaluate_expression(model, 'TVV', model.modelfit_results.parameter_estimates)
+    res = read_modelfit_results(testdata / 'nonmem' / 'models' / 'pheno_noifs.mod')
+    ser = evaluate_expression(model, 'TVV', res.parameter_estimates)
     assert ser[0] == pytest.approx(1.413062)
     assert ser[743] == pytest.approx(1.110262)
 
 
 def test_evaluate_population_prediction(load_model_for_test, testdata):
     path = testdata / 'nonmem' / 'minimal.mod'
     model = load_model_for_test(path)
@@ -52,17 +54,16 @@
     dataset = read_nonmem_dataset(StringIO('1 0 3\n2 0 4\n'), colnames=['ID', 'TIME', 'DV'])
     pred = evaluate_individual_prediction(model, dataset=dataset)
 
     assert list(pred) == [0.1, 0.1]
 
     linpath = testdata / 'nonmem' / 'pheno_real_linbase.mod'
     linmod = load_model_for_test(linpath)
-    pred = evaluate_individual_prediction(
-        model=linmod, etas=linmod.modelfit_results.individual_estimates
-    )
+    res = read_modelfit_results(linpath)
+    pred = evaluate_individual_prediction(model=linmod, etas=res.individual_estimates)
 
     pd.testing.assert_series_equal(lincorrect['CIPREDI'], pred, rtol=1e-4, check_names=False)
 
 
 def test_evaluate_eta_gradient(load_model_for_test, testdata):
     path = testdata / 'nonmem' / 'minimal.mod'
     model = load_model_for_test(path)
@@ -84,18 +85,18 @@
 
     dataset = read_nonmem_dataset(StringIO('1 0 3\n2 0 4\n'), colnames=['ID', 'TIME', 'DV'])
     grad = evaluate_epsilon_gradient(model, dataset=dataset)
     pd.testing.assert_frame_equal(grad, pd.DataFrame([1.0, 1.0], columns=['dY/dEPS_1']))
 
     linpath = testdata / 'nonmem' / 'pheno_real_linbase.mod'
     linmod = load_model_for_test(linpath)
-    grad = evaluate_epsilon_gradient(linmod, etas=linmod.modelfit_results.individual_estimates)
+    res = read_modelfit_results(linpath)
+    grad = evaluate_epsilon_gradient(linmod, etas=res.individual_estimates)
     pd.testing.assert_series_equal(lincorrect['H11'], grad.iloc[:, 0], rtol=1e-4, check_names=False)
 
 
 def test_evaluate_weighted_residuals(load_model_for_test, testdata):
     linpath = testdata / 'nonmem' / 'pheno_real_linbase.mod'
     linmod = load_model_for_test(linpath)
-    wres = evaluate_weighted_residuals(
-        linmod, parameters=dict(linmod.modelfit_results.parameter_estimates)
-    )
+    res = read_modelfit_results(linpath)
+    wres = evaluate_weighted_residuals(linmod, parameters=dict(res.parameter_estimates))
     pd.testing.assert_series_equal(lincorrect['WRES'], wres, rtol=1e-4, check_names=False)
```

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_expressions.py` & `pharmpy-core-0.96.0/tests/modeling/test_expressions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_has_covariate_effect.py` & `pharmpy-core-0.96.0/tests/modeling/test_has_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_help_functions.py` & `pharmpy-core-0.96.0/tests/modeling/test_help_functions.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_iterators.py` & `pharmpy-core-0.96.0/tests/modeling/test_iterators.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_lrt.py` & `pharmpy-core-0.96.0/tests/modeling/test_lrt.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_metabolite.py` & `pharmpy-core-0.96.0/tests/modeling/test_metabolite.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_modeling.py` & `pharmpy-core-0.96.0/tests/modeling/test_modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     transform_etas_boxcox,
     transform_etas_john_draper,
     transform_etas_tdist,
     update_initial_individual_estimates,
     update_inits,
 )
 from pharmpy.modeling.odes import find_clearance_parameters, find_volume_parameters
+from pharmpy.tools import read_modelfit_results
 
 
 def test_set_first_order_elimination(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
     correct = model.model_code
     model = set_first_order_elimination(model)
     assert model.model_code == correct
@@ -2580,26 +2581,25 @@
     shutil.copy(testdata / 'nonmem/pheno.dta', tmp_path / 'pheno.dta')
 
     with chdir(tmp_path):
         with open('run1.mod', 'a') as f:
             f.write(etas_file)
 
         model = load_model_for_test('run1.mod')
-        model = update_initial_individual_estimates(
-            model, model.modelfit_results.individual_estimates, force=force
-        )
+        res = read_modelfit_results('run1.mod')
+        model = update_initial_individual_estimates(model, res.individual_estimates, force=force)
         model = model.write_files()
 
         assert ('$ETAS FILE=run1_input.phi' in model.model_code) is file_exists
         assert (os.path.isfile('run1_input.phi')) is file_exists
 
 
 def test_update_inits_move_est(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
-    res = model.modelfit_results
+    res = read_modelfit_results(pheno_path)
 
     model = create_joint_distribution(model, individual_estimates=res.individual_estimates)
     model = add_iiv(model, 'S1', 'add')
 
     param_est = res.parameter_estimates.copy()
     param_est['IIV_CL_IIV_V'] = 0.0285  # Correlation > 0.99
     param_est['IIV_S1'] = 0.0005
@@ -2611,24 +2611,23 @@
     assert round(model.parameters['IIV_CL_IIV_V'].init, 6) == 0.025757
 
 
 def test_update_inits_zero_fix(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
     d = {name: 0 for name in model.random_variables.iiv.parameter_names}
     model = fix_parameters_to(model, d)
-    res = model.modelfit_results
+    res = read_modelfit_results(pheno_path)
     param_est = res.parameter_estimates.drop(index=['IVCL'])
     model = update_inits(model, param_est)
     assert model.parameters['IVCL'].init == 0
     assert model.parameters['IVCL'].fix
 
     model = load_model_for_test(pheno_path)
     d = {name: 0 for name in model.random_variables.iiv.parameter_names}
     model = fix_parameters_to(model, d)
-    res = model.modelfit_results
     param_est = res.parameter_estimates.drop(index=['IVCL'])
     model = update_inits(model, param_est, move_est_close_to_bounds=True)
     assert model.parameters['IVCL'].init == 0
     assert model.parameters['IVCL'].fix
 
 
 def test_update_inits_no_res(load_model_for_test, testdata, tmp_path):
@@ -2636,33 +2635,32 @@
     shutil.copy(testdata / 'nonmem/pheno.dta', tmp_path / 'pheno.dta')
 
     with chdir(tmp_path):
         shutil.copy(testdata / 'nonmem/pheno.ext', tmp_path / 'run1.ext')
         shutil.copy(testdata / 'nonmem/pheno.lst', tmp_path / 'run1.lst')
 
         model = load_model_for_test('run1.mod')
+        res = read_modelfit_results('run1.mod')
 
         modelfit_results = replace(
-            model.modelfit_results,
+            res,
             parameter_estimates=pd.Series(
                 np.nan, name='estimates', index=list(model.parameters.nonfixed.inits.keys())
             ),
         )
-        model = model.replace(modelfit_results=modelfit_results)
 
         with pytest.raises(ValueError):
-            update_inits(model, model.modelfit_results.parameter_estimates)
+            update_inits(model, modelfit_results.parameter_estimates)
 
 
 def test_nested_update_source(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
+    res = read_modelfit_results(pheno_path)
 
-    model = create_joint_distribution(
-        model, individual_estimates=model.modelfit_results.individual_estimates
-    )
+    model = create_joint_distribution(model, individual_estimates=res.individual_estimates)
     model = model.update_source()
 
     assert 'IIV_CL_IIV_V' in model.model_code
 
     model = load_model_for_test(pheno_path)
 
     model = remove_iiv(model, 'CL')
```

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_parameter_sampling.py` & `pharmpy-core-0.96.0/tests/modeling/test_parameter_sampling.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 from pharmpy.modeling import (
     create_rng,
-    load_example_model,
     sample_individual_estimates,
     sample_parameters_from_covariance_matrix,
     sample_parameters_uniformly,
 )
+from pharmpy.tools import read_modelfit_results
 
 
 def test_create_rng():
     rng = create_rng(23)
     assert rng.standard_normal() == 0.5532605888887387
 
     rng = create_rng(23.0)
     assert rng.standard_normal() == 0.5532605888887387
 
 
-def test_sample_parameters_uniformly():
-    model = load_example_model("pheno")
+def test_sample_parameters_uniformly(load_model_for_test, testdata):
+    model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
+    res = read_modelfit_results(testdata / 'nonmem' / 'pheno_real.mod')
     rng = create_rng(23)
-    df = sample_parameters_uniformly(
-        model, model.modelfit_results.parameter_estimates, n=3, rng=rng
-    )
+    df = sample_parameters_uniformly(model, res.parameter_estimates, n=3, rng=rng)
     assert df['PTVCL'][0] == 0.004877674495376137
 
 
 def test_sample_parameter_from_covariance_matrix(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
+    res = read_modelfit_results(testdata / 'nonmem' / 'pheno_real.mod')
     rng = np.random.default_rng(318)
-    pe = model.modelfit_results.parameter_estimates
-    cm = model.modelfit_results.covariance_matrix
+    pe = res.parameter_estimates
+    cm = res.covariance_matrix
     samples = sample_parameters_from_covariance_matrix(
         model,
         pe,
         cm,
         n=3,
         rng=rng,
     )
@@ -62,17 +62,18 @@
             n=1,
             force_posdef_covmatrix=True,
         )
 
 
 def test_sample_individual_estimates(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
+    res = read_modelfit_results(testdata / 'nonmem' / 'pheno_real.mod')
     rng = np.random.default_rng(86)
-    ie = model.modelfit_results.individual_estimates
-    iec = model.modelfit_results.individual_estimates_covariance
+    ie = res.individual_estimates
+    iec = res.individual_estimates_covariance
     samples = sample_individual_estimates(model, ie, iec, rng=rng)
     assert len(samples) == 59 * 100
     assert list(samples.columns) == ['ETA_1', 'ETA_2']
     assert pytest.approx(samples.iloc[0]['ETA_1'], 1e-5) == 0.21179186940672637
     assert pytest.approx(samples.iloc[0]['ETA_2'], 1e-5) == -0.05771736555248238
 
     restricted = sample_individual_estimates(
```

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_parameters.py` & `pharmpy-core-0.96.0/tests/modeling/test_parameters.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_plots.py` & `pharmpy-core-0.96.0/tests/modeling/test_plots.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 from pharmpy.modeling import (
     plot_individual_predictions,
     plot_iofv_vs_iofv,
     plot_transformed_eta_distributions,
 )
+from pharmpy.tools import read_modelfit_results
 
 
-def test_plot_iofv_vs_iofv(load_example_model_for_test):
-    model = load_example_model_for_test('pheno')
-    iofv = model.modelfit_results.individual_ofv
+def test_plot_iofv_vs_iofv(testdata):
+    res = read_modelfit_results(testdata / 'nonmem' / 'pheno_real.mod')
+    iofv = res.individual_ofv
     assert plot_iofv_vs_iofv(iofv, iofv, "run1", "run1")
 
 
 def test_plot_individual_predictions(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
-    plot = plot_individual_predictions(model, model.modelfit_results.predictions)
+    res = read_modelfit_results(testdata / 'nonmem' / 'pheno_real.mod')
+    plot = plot_individual_predictions(model, res.predictions)
     assert plot
-    plot = plot_individual_predictions(
-        model, model.modelfit_results.predictions[['PRED']], individuals=[1, 2, 5]
-    )
+    plot = plot_individual_predictions(model, res.predictions[['PRED']], individuals=[1, 2, 5])
     assert plot
 
 
 def test_plot_transformed_eta_distributions(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'qa' / 'boxcox.mod')
-    pe = model.modelfit_results.parameter_estimates
-    ie = model.modelfit_results.individual_estimates
+    res = read_modelfit_results(testdata / 'nonmem' / 'qa' / 'boxcox.mod')
+    pe = res.parameter_estimates
+    ie = res.individual_estimates
     plot = plot_transformed_eta_distributions(model, pe, ie)
     assert plot
```

### Comparing `pharmpy-core-0.95.0/tests/modeling/test_remove_covariate_effect.py` & `pharmpy-core-0.96.0/tests/modeling/test_remove_covariate_effect.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/output/test_nonmem_results_file.py` & `pharmpy-core-0.96.0/tests/nonmem/output/test_nonmem_results_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from pathlib import Path
 
 import pytest
 from numpy import nan
 
-import pharmpy.plugins.nonmem.results_file as rf
-import pharmpy.plugins.nonmem.table as table
-from pharmpy.modeling import read_model
+import pharmpy.model.external.nonmem.table as table
+import pharmpy.tools.external.nonmem.results_file as rf
+from pharmpy.tools import read_modelfit_results
 from pharmpy.workflows.log import Log
 
 
 def test_supported_version():
     assert rf.NONMEMResultsFile.supported_version(None) is False
     assert rf.NONMEMResultsFile.supported_version('7.1.0') is False
     assert rf.NONMEMResultsFile.supported_version('7.2.0') is True
@@ -425,14 +425,14 @@
 def test_warnings(testdata, file_name, ref, idx):
     lst = rf.NONMEMResultsFile(testdata / 'nonmem' / 'errors' / file_name, log=Log())
     message = lst.log.to_dataframe()['message'].iloc[idx]
     assert message == ref
 
 
 def test_covariance_status(testdata):
-    model = read_model(
+    res = read_modelfit_results(
         testdata / 'nonmem' / 'modelfit_results' / 'covariance' / 'pheno_nocovariance.mod'
     )
-    assert model.modelfit_results.standard_errors is None
-    assert model.modelfit_results.covariance_matrix is None
-    assert model.modelfit_results.correlation_matrix is None
-    assert model.modelfit_results.information_matrix is None
+    assert res.standard_errors is None
+    assert res.covariance_matrix is None
+    assert res.correlation_matrix is None
+    assert res.precision_matrix is None
```

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_abbreviated.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_abbreviated.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_code.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import sympy
 
 from pharmpy.internals.expr.funcs import PHI
 from pharmpy.model import Assignment
-from pharmpy.plugins.nonmem.records.code_record import CodeRecord
+from pharmpy.model.external.nonmem.records.code_record import CodeRecord
 
 
 def _ensure_trailing_newline(buf):
     # FIXME This should not be necessary
     return buf if buf[-1] == '\n' else buf + '\n'
```

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_data.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_data.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_estimation_record.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_estimation_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_factory.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_factory.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_model_record.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_model_record.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_omega.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_omega.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_option_record.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_option_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
-from pharmpy.plugins.nonmem.records.option_record import OptionRecord, StrOpt, WildOpt
-from pharmpy.plugins.nonmem.records.table_record import table_options
+from pharmpy.model.external.nonmem.records.option_record import OptionRecord, StrOpt, WildOpt
+from pharmpy.model.external.nonmem.records.table_record import table_options
 
 
 def test_create_record(parser):
     recs = parser.parse('$INPUT ID TIME DV WGT=DROP')
     rec = recs.records[0]
     pairs = rec.option_pairs
     assert list(pairs.items()) == [('ID', None), ('TIME', None), ('DV', None), ('WGT', 'DROP')]
```

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_problem.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_problem.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_sizes.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_sizes.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/records/test_theta.py` & `pharmpy-core-0.96.0/tests/nonmem/records/test_theta.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/test_advan.py` & `pharmpy-core-0.96.0/tests/nonmem/test_advan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import pytest
 import sympy
 
 from pharmpy.model import output
+from pharmpy.model.external.nonmem.advan import compartmental_model
 from pharmpy.modeling import get_initial_conditions
-from pharmpy.plugins.nonmem.advan import compartmental_model
 
 
 def S(x):
     return sympy.Symbol(x)
 
 
 @pytest.mark.parametrize(
```

### Comparing `pharmpy-core-0.95.0/tests/nonmem/test_des.py` & `pharmpy-core-0.96.0/tests/nonmem/test_des.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/test_input.py` & `pharmpy-core-0.96.0/tests/nonmem/test_input.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/nonmem/test_nonmem_model.py` & `pharmpy-core-0.96.0/tests/nonmem/test_nonmem_model.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import shutil
-from io import StringIO
 
 import pytest
 import sympy
 from sympy import Symbol as symbol
 
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.model import (
@@ -14,29 +13,30 @@
     ModelSyntaxError,
     NormalDistribution,
     ODESystem,
     Parameter,
     Parameters,
     Statements,
 )
+from pharmpy.model.external.nonmem import convert_model
+from pharmpy.model.external.nonmem.nmtran_parser import NMTranParser
+from pharmpy.model.external.nonmem.records.factory import create_record
 from pharmpy.modeling import (
     add_iiv,
     add_population_parameter,
     create_joint_distribution,
     remove_iiv,
     set_estimation_step,
     set_initial_condition,
     set_initial_estimates,
     set_zero_order_absorption,
     set_zero_order_elimination,
     set_zero_order_input,
 )
-from pharmpy.plugins.nonmem import convert_model
-from pharmpy.plugins.nonmem.nmtran_parser import NMTranParser
-from pharmpy.plugins.nonmem.records.factory import create_record
+from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.amd.funcs import create_start_model
 
 
 def _ensure_trailing_newline(buf):
     # FIXME This should not be necessary
     return buf if buf[-1] == '\n' else buf + '\n'
 
@@ -45,40 +45,39 @@
     return symbol(x)
 
 
 def test_source(pheno):
     assert pheno.model_code.startswith('$PROBLEM PHENOBARB')
 
 
-def test_update_inits(load_model_for_test, pheno, pheno_path):
+def test_update_inits(load_model_for_test, pheno_path):
     from pharmpy.modeling import update_inits
 
-    model = update_inits(pheno, pheno.modelfit_results.parameter_estimates)
-
     model = load_model_for_test(pheno_path)
-    model = update_inits(model, model.modelfit_results.parameter_estimates)
+    res = read_modelfit_results(pheno_path)
+    model = update_inits(model, res.parameter_estimates)
 
 
-def test_empty_ext_file(load_model_for_test, testdata):
+def test_empty_ext_file(testdata):
     # assert existing but empty ext-file does not give modelfit_results
-    model = load_model_for_test(
+    res = read_modelfit_results(
         testdata / 'nonmem' / 'modelfit_results' / 'onePROB' / 'noESTwithSIM' / 'onlysim.mod'
     )
-    assert model.modelfit_results is None
+    assert res is None
 
 
 def test_detection():
-    Model.create_model(StringIO("$PROBLEM this\n$PRED\n"))
-    Model.create_model(StringIO("   \t$PROBLEM skld fjl\n$PRED\n"))
-    Model.create_model(StringIO(" $PRO l907\n$PRED\n"))
+    Model.parse_model_from_string("$PROBLEM this\n$PRED\n")
+    Model.parse_model_from_string("   \t$PROBLEM skld fjl\n$PRED\n")
+    Model.parse_model_from_string(" $PRO l907\n$PRED\n")
 
 
-def test_validate(pheno):
+def test_validate():
     with pytest.raises(ModelSyntaxError):
-        Model.create_model(StringIO("$PROBLEM this\n$SIZES LIM1=3000\n$PRED\n"))
+        Model.parse_model_from_string("$PROBLEM this\n$SIZES LIM1=3000\n$PRED\n")
 
 
 def test_parameters(pheno):
     params = pheno.parameters
     assert len(params) == 6
     assert pheno.parameters['PTVCL'] == Parameter('PTVCL', 0.00469307, lower=0, upper=1000000)
     assert pheno.parameters['PTVV'] == Parameter('PTVV', 1.00916, lower=0, upper=1000000)
@@ -86,15 +85,17 @@
     assert pheno.parameters['IVCL'] == Parameter('IVCL', 0.0309626, lower=0, upper=sympy.oo)
     assert pheno.parameters['IVV'] == Parameter('IVV', 0.031128, lower=0, upper=sympy.oo)
     assert pheno.parameters['SIGMA_1_1'] == Parameter(
         'SIGMA_1_1', 0.013241, lower=0, upper=sympy.oo
     )
 
 
-def test_set_parameters(pheno):
+def test_set_parameters(pheno_path, load_model_for_test):
+    pheno = load_model_for_test(pheno_path)
+    res = read_modelfit_results(pheno_path)
     params = {
         'PTVCL': 0.75,
         'PTVV': 0.5,
         'THETA_3': 0.25,
         'IVCL': 0.1,
         'IVV': 0.2,
         'SIGMA_1_1': 0.3,
@@ -116,17 +117,15 @@
     sigmas = model.internals.control_stream.get_records('SIGMA')
     assert str(sigmas[0]) == '$SIGMA 0.3\n'
 
     model = set_initial_estimates(pheno, {'PTVCL': 18})
     assert model.parameters['PTVCL'] == Parameter('PTVCL', 18, lower=0, upper=1000000)
     assert model.parameters['PTVV'] == Parameter('PTVV', 1.00916, lower=0, upper=1000000)
 
-    model = create_joint_distribution(
-        pheno, individual_estimates=model.modelfit_results.individual_estimates
-    )
+    model = create_joint_distribution(pheno, individual_estimates=res.individual_estimates)
     with pytest.raises(UserWarning, match='Adjusting initial'):
         set_initial_estimates(model, {'IVV': 0.000001})
 
 
 def test_adjust_iovs(load_model_for_test, testdata):
     model = load_model_for_test(
         testdata / 'nonmem' / 'modelfit_results' / 'onePROB' / 'multEST' / 'noSIM' / 'withBayes.mod'
@@ -385,15 +384,15 @@
 
 $THETA 0.1  ; TV
 $OMEGA 0.01
 $SIGMA 1
 $ESTIMATION METHOD=1 INTER MAXEVALS=9990 PRINT=2 POSTHOC
 """
     with pytest.warns(UserWarning):
-        model = Model.create_model(StringIO(code))
+        model = Model.parse_model_from_string(code)
         assert model.parameters.names == ['THETA_1', 'OMEGA_1_1', 'SIGMA_1_1']
 
 
 def test_symbol_names_in_abbr(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno_abbr.mod')
     pset, rvs = model.parameters, model.random_variables
 
@@ -415,30 +414,30 @@
 
 $THETA 0.1  ; TV
 $OMEGA 0.01 ; TV
 $SIGMA 1 ; TV
 $ESTIMATION METHOD=1 INTER MAXEVALS=9990 PRINT=2 POSTHOC
 """
     with pytest.warns(UserWarning):
-        model = Model.create_model(StringIO(code))
+        model = Model.parse_model_from_string(code)
         assert model.parameters.names == ['TV', 'OMEGA_1_1', 'SIGMA_1_1']
 
     code = """$PROBLEM base model
 $INPUT ID DV TIME
 $DATA file.csv IGNORE=@
 
 $PRED
 Y = THETA(1) + THETA(2)
 
 $THETA 0.1  ; TV
 $THETA 0.1  ; TV
 $ESTIMATION METHOD=1 INTER MAXEVALS=9990 PRINT=2 POSTHOC
 """
     with pytest.warns(UserWarning):
-        model = Model.create_model(StringIO(code))
+        model = Model.parse_model_from_string(code)
         assert model.parameters.names == ['TV', 'THETA_2']
 
 
 def test_abbr_write(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
     model = add_iiv(model, 'S1', 'add')
 
@@ -446,15 +445,15 @@
     assert 'ETA_S1' in model.random_variables.names
     assert S('ETA_S1') in model.statements.free_symbols
 
 
 def test_abbr_read_write(load_model_for_test, pheno_path):
     model_write = load_model_for_test(pheno_path)
     model_write = add_iiv(model_write, 'S1', 'add')
-    model_read = Model.create_model(StringIO(model_write.model_code))
+    model_read = Model.parse_model_from_string(model_write.model_code)
     assert model_read.model_code == model_write.model_code
     assert model_read.statements == model_write.statements
     assert not (
         set(model_read.random_variables.names) - set(model_write.random_variables.names)
     )  # Different order due to renaming in read
 
 
@@ -545,39 +544,39 @@
 $THETA  (0,0.0818029) ; POP_LAG
 $THETA  65.1756756757 FIX ; TV_AGE
  1.2027027027 FIX ; TV_SEX
 $SIGMA  0.112373
 $SIGMA  0.0000001  FIX  ;     EPSCOV
 $ESTIMATION METHOD=1 MAXEVAL=9999 NONINFETA=1 MCETA=1
 """
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     rvs = model.random_variables
     assert len(rvs.names) == 11
 
 
 @pytest.mark.parametrize(
     'model_path, transformation',
     [
         ('nonmem/pheno.mod', set_zero_order_elimination),
     ],
 )
 def test_des(load_model_for_test, testdata, model_path, transformation):
     model_ref = load_model_for_test(testdata / model_path)
     model_ref = transformation(model_ref)
 
-    model_des = Model.create_model(StringIO(model_ref.model_code))
+    model_des = Model.parse_model_from_string(model_ref.model_code)
 
     assert model_ref.statements.ode_system == model_des.statements.ode_system
 
 
 def test_cmt_warning(load_model_for_test, testdata):
     model_original = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox1.mod')
 
     model_str = model_original.model_code.replace('CMT=DROP', 'CMT')
-    model = Model.create_model(StringIO(model_str))
+    model = Model.parse_model_from_string(model_str)
     model = model.replace(datainfo=model.datainfo.replace(path=model_original.datainfo.path))
 
     with pytest.raises(UserWarning, match='Compartment structure has been updated'):
         set_zero_order_absorption(model)
 
 
 @pytest.mark.parametrize(
@@ -625,15 +624,15 @@
 $PRED
 Y = THETA(1) + ETA(1) + ERR(1)
 $THETA 0.1
 $OMEGA 0.01
 $SIGMA 1
 '''
     code += estcode
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     correct = EstimationSteps.create(steps=est_steps)
     assert model.estimation_steps == correct
 
 
 def test_estimation_steps_getter_options():
     code = '''$PROBLEM base model
 $INPUT ID DV TIME
@@ -641,15 +640,15 @@
 $PRED
 Y = THETA(1) + ETA(1) + ERR(1)
 $THETA 0.1
 $OMEGA 0.01
 $SIGMA 1
 $ESTIMATION METHOD=1 SADDLE_RESET=1
 '''
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     assert model.estimation_steps[0].method == 'FOCE'
     assert model.estimation_steps[0].tool_options['SADDLE_RESET'] == '1'
 
 
 @pytest.mark.parametrize(
     'estcode,kwargs,rec_ref',
     [
@@ -687,15 +686,15 @@
 $PRED
 Y = THETA(1) + ETA(1) + ERR(1)
 $THETA 0.1
 $OMEGA 0.01
 $SIGMA 1
 '''
     code += estcode
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     steps = model.estimation_steps
     newstep = steps[0].replace(**kwargs)
     model = model.replace(estimation_steps=newstep + steps[1:])
     model = model.update_source()
     assert model.model_code.split('\n')[-2] == rec_ref
 
 
@@ -721,15 +720,15 @@
 $PRED
 Y = THETA(1) + ETA(1) + ERR(1)
 $THETA 0.1
 $OMEGA 0.01
 $SIGMA 1
 '''
     code += estcode
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
 
     steps = model.estimation_steps
     newstep = steps[0].replace(**kwargs)
     newsteps = newstep + steps[1:]
     model = model.replace(estimation_steps=newsteps)
 
     with pytest.raises(ValueError) as excinfo:
@@ -744,15 +743,15 @@
 $PRED
 Y = THETA(1) + ETA(1) + ERR(1)
 $THETA 0.1
 $OMEGA 0.01
 $SIGMA 1
 $EST METH=COND INTER
 '''
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     est_new = EstimationStep.create('IMP', interaction=True, tool_options={'saddle_reset': 1})
     model = model.replace(estimation_steps=model.estimation_steps + est_new)
     model = model.update_source()
     assert model.model_code.split('\n')[-2] == '$ESTIMATION METHOD=IMP INTER SADDLE_RESET=1'
     est_new = EstimationStep.create('SAEM', interaction=True)
     model = model.replace(estimation_steps=est_new + model.estimation_steps)
     model = model.update_source()
@@ -774,15 +773,15 @@
 $PRED
 Y = THETA(1) + ETA(1) + ERR(1)
 $THETA 0.1
 $OMEGA 0.01
 $SIGMA 1
 $EST METH=COND INTER
 '''
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     model = model.replace(estimation_steps=model.estimation_steps[1:])
     assert not model.estimation_steps
     model = model.update_source()
     assert model.model_code.split('\n')[-2] == '$SIGMA 1'
 
 
 def test_update_source_comments():
@@ -820,15 +819,15 @@
 $SIGMA  0.013241
 $ESTIMATION METHOD=1 INTERACTION MAXEVALS=9999
 $COVARIANCE UNCONDITIONAL
 $TABLE      ID TIME AMT WGT APGR IPRED PRED TAD CWRES NPDE NOAPPEND
             NOPRINT ONEHEADER FILE=mytab3
 """
     with pytest.warns(UserWarning):
-        model = Model.create_model(StringIO(code))
+        model = Model.parse_model_from_string(code)
         model.update_source()
 
 
 def test_convert_model(testdata):
     code = """$PROBLEM base model
 $INPUT ID DV TIME
 $DATA file.csv IGNORE=@
@@ -837,15 +836,15 @@
 Y = THETA(1) + ETA(1) + EPS(1)
 
 $THETA 1  ; TH1
 $OMEGA 2 ; OM1
 $SIGMA 3 ; SI1
 $ESTIMATION METHOD=1 INTER
 """
-    base = Model.create_model(StringIO(code))
+    base = Model.parse_model_from_string(code)
     base.dataset_path = testdata / 'nonmem' / 'file.csv'
     model = convert_model(base)
     model.dataset_path = "file.csv"  # Otherwise we get full path
     correct = """$PROBLEM base model
 $INPUT ID DV TIME
 $DATA file.csv IGNORE=@
 
@@ -869,15 +868,15 @@
     Y = THETA(1) + ETA(1) + EPS(1)
 
     $THETA 1  ; TH1
     $OMEGA 2 ; OM1
     $SIGMA 3 ; SI1
     $ESTIMATION METHOD=1 INTER
     """
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     dataset_new = model.dataset.copy()
     dataset_new['ID'] = dataset_new['ID'] * 10000
     model = model.replace(dataset=dataset_new)
     model = set_estimation_step(model, 'FO', residuals=['CWRES'])
     assert 'FORMAT=' in model.model_code
 
 
@@ -912,15 +911,15 @@
 Y = THETA(1) + ETA(1) + EPS(1)
 
 $THETA 1  ; TH1
 $OMEGA 0 FIX ; OM1
 $SIGMA 3 ; SI1
 $ESTIMATION METHOD=1 INTER
 """
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     assert len(model.random_variables.etas) == 1
 
 
 def test_solver():
     code = """
 $PROBLEM
 $DATA ../../pheno.dta IGNORE=@
@@ -938,15 +937,15 @@
 $THETA (0,0.00469555)
 $THETA (0,0.984258)
 $THETA (0.15892)
 $OMEGA 0.0293508 0.027906
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION MAXEVALS=9999
 """
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     assert len(model.estimation_steps) == 1
     step = model.estimation_steps[0]
     assert step.solver == 'DVERK'
     assert step.solver_rtol == 5
     assert step.solver_atol == 1e-12
 
     code = """
@@ -966,15 +965,15 @@
 $THETA (0,0.00469555)
 $THETA (0,0.984258)
 $THETA (0.15892)
 $OMEGA 0.0293508 0.027906
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION MAXEVALS=9999
 """
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     assert len(model.estimation_steps) == 1
     step = model.estimation_steps[0]
     assert step.solver == 'LSODA'
     assert step.solver_rtol == 5
     assert step.solver_atol == 1.5
 
 
@@ -1002,15 +1001,15 @@
 $THETA (0,0.00469555)
 $THETA (0,0.984258)
 $THETA (0.15892)
 $OMEGA 0.0293508 0.027906
 $SIGMA 0.013241
 $ESTIMATION METHOD=1 INTERACTION MAXEVALS=9999
 """
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     assert type(model.statements.ode_system.eqs[0].rhs) == sympy.Piecewise
     assert model.statements[3].symbol == sympy.Function("A_CENTRAL")(0)
     assert model.statements[3].expression == sympy.Integer(2)
 
 
 @pytest.mark.parametrize(
     'estline,likelihood',
@@ -1027,15 +1026,15 @@
 $PRED
 Y = THETA(1) + ETA(1) + EPS(1)
 
 $THETA 1  ; TH1
 $OMEGA 0 FIX ; OM1
 $SIGMA 3 ; SI1
 """
-    model = Model.create_model(StringIO(code + estline))
+    model = Model.parse_model_from_string(code + estline)
     assert model.value_type == likelihood
 
 
 def test_f_flag():
     code = """$PROBLEM base model
 $INPUT ID DV TIME
 $DATA file.csv IGNORE=@
@@ -1045,15 +1044,15 @@
 Y = THETA(1) + ETA(1) + EPS(1)
 
 $THETA 1  ; TH1
 $OMEGA 0 FIX ; OM1
 $SIGMA 3 ; SI1
 $ESTIMATION METHOD=1 INTER
 """
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     assert model.value_type == sympy.Symbol('F_FLAG')
 
 
 def test_datainfo_model_drop_clash(testdata):
     datapath = testdata / 'nonmem' / 'pheno.dta'
     code = f"""$PROBLEM
 $DATA {datapath} IGNORE=@
@@ -1070,15 +1069,15 @@
 $SIGMA 0.013241
 
 $ESTIMATION METHOD=1 INTERACTION
 """
     with pytest.warns(
         UserWarning, match='NONMEM .mod and dataset .datainfo disagree on DROP for columns WGT'
     ):
-        model = Model.create_model(StringIO(code))
+        model = Model.parse_model_from_string(code)
 
     assert model.datainfo['WGT'].drop
 
 
 def test_abbr_etas():
     code = '''$PROBLEM
 $INPUT ID DV TIME
@@ -1087,15 +1086,15 @@
 $PRED
 VAR = ETA_MY
 Y = THETA(1) + VAR + ERR(1)
 $THETA 0.1
 $OMEGA 0.01
 $SIGMA 1
 '''
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     assert model.random_variables.etas.names == ['ETA_MY']
 
     model = add_iiv(model, ['Y'], 'exp', '+', eta_names=['ETA_DUMMY'])
     model = remove_iiv(model, ['ETA_MY'])
     model = add_iiv(model, ['VAR'], 'exp', '+', eta_names=['ETA_MY'])
     assert model.model_code.split('\n')[3] == '$ABBR REPLACE ETA_DUMMY=ETA(1)'
     assert model.model_code.split('\n')[4] == '$ABBR REPLACE ETA_MY=ETA(2)'
@@ -1115,15 +1114,15 @@
 $PRED
 VAR = ETA(1)
 Y = THETA(1) + VAR + ERR(1)
 $THETA 0.1
 $OMEGA 0.01
 $SIGMA 1
 '''
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
     model = add_iiv(model, ['Y'], 'exp', '+', eta_names=['ETA_DUMMY'])
     assert model.model_code.split('\n')[3] == '$ABBR PROTECT DERIV2=NO'
 
 
 def test_parse_dvid(testdata, load_model_for_test):
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'pheno_dvid.mod')
     assert model.statements[-1] == Assignment.create("Y_2", "EPS_1 * F + EPS_2 + F")
@@ -1145,15 +1144,15 @@
     $DATA file.csv IGNORE=@
     $PRED
     Y = THETA(1) + ETA(1) + ERR(1)
     $THETA 0.1
     $OMEGA 0.01
     $SIGMA 1
     '''
-    model = Model.create_model(StringIO(code))
+    model = Model.parse_model_from_string(code)
 
     with pytest.raises(ValueError, match='NONMEM does not allow etas named `eta`'):
         add_iiv(model, ['Y'], 'exp', '+', eta_names=['eta'])
 
 
 def test_ics(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
```

### Comparing `pharmpy-core-0.95.0/tests/nonmem/test_nonmem_table.py` & `pharmpy-core-0.96.0/tests/nonmem/test_nonmem_table.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import pytest
 
 from pharmpy.internals.fs.cwd import chdir
-from pharmpy.plugins.nonmem.table import CovTable, ExtTable, NONMEMTableFile, PhiTable
+from pharmpy.model.external.nonmem.table import CovTable, ExtTable, NONMEMTableFile, PhiTable
 
 
 def test_nonmem_table(pheno_ext):
     ext_table_file = NONMEMTableFile(pheno_ext)
     ext_table = ext_table_file.table
     assert isinstance(ext_table, ExtTable)
     assert list(ext_table.data_frame.columns) == [
```

### Comparing `pharmpy-core-0.95.0/tests/nonmem/test_parser.py` & `pharmpy-core-0.96.0/tests/nonmem/test_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pytest
 
-from pharmpy.plugins.nonmem.nmtran_parser import NMTranParser
-from pharmpy.plugins.nonmem.parsing import parse_table_columns
+from pharmpy.model.external.nonmem.nmtran_parser import NMTranParser
+from pharmpy.model.external.nonmem.parsing import parse_table_columns
 
 
 def test_simple_parse():
     parser = NMTranParser()
 
     model = parser.parse('$PROBLEM MYPROB\n')
```

### Comparing `pharmpy-core-0.95.0/tests/nonmem/test_read.py` & `pharmpy-core-0.96.0/tests/nonmem/test_read.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 from io import StringIO
 
 import pandas as pd
 import pytest
 
 from pharmpy.model import DatasetError, DatasetWarning
-from pharmpy.plugins.nonmem.dataset import NMTRANDataIO, convert_fortran_number, read_nonmem_dataset
+from pharmpy.model.external.nonmem.dataset import (
+    NMTRANDataIO,
+    convert_fortran_number,
+    read_nonmem_dataset,
+)
 
 
 def test_read_nonmem_dataset(testdata):
     path = testdata / 'nonmem' / 'pheno.dta'
     colnames = ['ID', 'TIME', 'AMT', 'WGT', 'APGR', 'DV', 'FA1', 'FA2']
     df = read_nonmem_dataset(path, colnames=colnames, ignore_character='@')
     assert list(df.columns) == colnames
```

### Comparing `pharmpy-core-0.95.0/tests/plugins/test_nlmixr.py` & `pharmpy-core-0.96.0/tests/external/test_nlmixr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pharmpy.plugins.nlmixr import convert_model
+from pharmpy.model.external.nlmixr import convert_model
 
 
 def test_model(testdata, load_model_for_test):
     nmmodel = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
     model = convert_model(nmmodel)
     assert 'ini' in model.model_code
     assert 'model' in model.model_code
```

### Comparing `pharmpy-core-0.95.0/tests/plugins/test_rxode.py` & `pharmpy-core-0.96.0/tests/external/test_rxode.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from pharmpy.plugins.rxode import convert_model
+from pharmpy.model.external.rxode import convert_model
 
 
 def test_model(testdata, load_model_for_test):
     nmmodel = load_model_for_test(testdata / 'nonmem' / 'pheno.mod')
     model = convert_model(nmmodel)
     assert 'rxode2' in model.model_code
     assert 'thetas' in model.model_code
```

### Comparing `pharmpy-core-0.95.0/tests/testdata/frem/results.json` & `pharmpy-core-0.96.0/tests/testdata/frem/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/DDMODEL00000130` & `pharmpy-core-0.96.0/tests/testdata/nonmem/DDMODEL00000130`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv` & `pharmpy-core-0.96.0/tests/testdata/nonmem/Simulated_CMS_colistin_PK_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/cdd_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_10.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_5.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_7.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_8.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/m1/rem_9.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml` & `pharmpy-core-0.96.0/tests/testdata/nonmem/cdd/pheno_real_bin10/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/control_stream_error.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/control_stream_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/est_step_warning.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/est_step_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/estimate_near_boundary_warning.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/failed_run.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/failed_run.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/no_header_error.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/no_header_error.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/no_header_error.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/no_header_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/rounding_error.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/rounding_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/run_interrupted.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/run_interrupted.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/errors/zero_gradient_error.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/errors/zero_gradient_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/FCON` & `pharmpy-core-0.96.0/tests/testdata/nonmem/fcon/FCON`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/fcon/FDATA` & `pharmpy-core-0.96.0/tests/testdata/nonmem/fcon/FDATA`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/frem/pheno_cat/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/linearize/linearize_dir1/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/covariance/pheno_nocovariance.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/multPROB/multEST/withSIM/multprobmix_nm730.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/anneal2_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/pheno_multEST.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/superid2_6_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/multEST/noSIM/withBayes.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/noESTwithSIM/onlysim.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/UseCase7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/example6b_V7_30_beta.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/hessian_error.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/large_s_matrix_cov_fail.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval0.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/maxeval3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_fail_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/mox_nocov_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/near_bounds.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/nm710_fail_negV.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/pheno_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/phenocorr.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/sparse_matrix_with_msfi.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_nonp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/theo_withcov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/noSIM/warfarin_ddmore.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/onePROB/oneEST/withSIM/control3boot.res`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modelfit_results/simfit/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_1transit.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_1transit.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_2transits.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_2transits.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan1.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan11.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan11.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan12.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan12.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan1_zero_order.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan2.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan2_seq.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan3.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan4.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan5_depot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_advan5_nodepot.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/pheno_zero_order.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/modeling/transit_indirect_reabsorption.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.datainfo` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/fviii6.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/fviii6.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/fviii6.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox1.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox2.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_2comp.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_2comp.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_log.csv` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_simulated_log.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_normal.csv` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_simulated_normal.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mox_simulated_normal.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/moxo_simulated_amd.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/moxo_simulated_amd.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/mytab_mox2` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pef.csv` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pef.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_advan3_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_advan3_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_advan3_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_dvid.csv` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_dvid.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_dvid.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_dvid.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.coi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.cor` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_noifs.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_noifs.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_trans1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_trans1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/models/pheno_trans1.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/models/pheno_trans1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.datainfo` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_block.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_block.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_etas.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_etas.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_multivariate_piecewise.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_no_obs_1stID.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_rate.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_rate.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.coi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.coi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.cor` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.tab` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real.xml` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real.xml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/pheno_real_linbase.tab` & `pharmpy-core-0.96.0/tests/testdata/nonmem/pheno_real_linbase.tab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/add_etas_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/add_etas_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/add_etas_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/add_etas_linbase.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/add_etas_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/boxcox.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/boxcox.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/boxcox.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/boxcox.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/boxcox.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/cdd_results.json` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/fullblock.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/fullblock.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/fullblock.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/fullblock.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/fullblock.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/iov.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/iov.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/iov.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/iov.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/iov.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/pheno_linbase.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/pheno_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/resmod_results.json` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/resmod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/scm_results.json` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/scm_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/simeval_results.json` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/simeval_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/tdist.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/tdist.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/tdist.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/qa/tdist.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/qa/tdist.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mox3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mox3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.mod` & `pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mox3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mox3.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mox3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv` & `pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/moxo_simulated_resmod.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/ruvsearch/mytab` & `pharmpy-core-0.96.0/tests/testdata/nonmem/ruvsearch/mytab`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/backward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/backward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/gofofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/localmin.logf` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/localmin.logf`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/backward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_ofv_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_pval_1.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_pval_2.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/log_steps/forward_pval_3.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir2/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/mergeofv_dir2/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/meta.yaml` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/onlyforward_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/onlyforward_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/scm_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt` & `pharmpy-core-0.96.0/tests/testdata/nonmem/scm/scmplus_dir1/scmlog.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/sdtab1` & `pharmpy-core-0.96.0/tests/testdata/nonmem/sdtab1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.dta` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/pheno.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/pheno.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run1.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.cov` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.ext` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.lst` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/nonmem/secondary_parameters/run2.phi` & `pharmpy-core-0.96.0/tests/testdata/nonmem/secondary_parameters/run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/pheno_data.csv` & `pharmpy-core-0.96.0/tests/testdata/pheno_data.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data0.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/est_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data1.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/est_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data2.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/est_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/est_data3.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/est_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/est_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model0.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/m1/pred_model3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/meta.yaml` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data0.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/pred_data0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data1.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/pred_data1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data2.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/pred_data2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/pred_data3.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/pred_data3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt` & `pharmpy-core-0.96.0/tests/testdata/psn/crossval_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/final_models/model_4_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/frem_dataset.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/frem_dataset.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/frem_results.csv` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/frem_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filter_data_model.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/filtered_plus_type0.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_1b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.cor` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.mod` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_2_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.mod` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/m1/model_3b_input.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/meta.yaml` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/meta.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/proposal_density.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/proposal_density.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt` & `pharmpy-core-0.96.0/tests/testdata/psn/frem_dir1/version_and_option_info.txt`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/results.json` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/derivatives.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/linearize_run/scm_dir1/extra_table`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/pheno_real_linbase.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/qa_dir1/results_summary.yaml` & `pharmpy-core-0.96.0/tests/testdata/psn/qa_dir1/results_summary.yaml`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir1/resmod_results.csv` & `pharmpy-core-0.96.0/tests/testdata/psn/resmod_dir1/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/resmod_dir2/resmod_results.csv` & `pharmpy-core-0.96.0/tests/testdata/psn/resmod_dir2/resmod_results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/orig_pred.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.cor` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.cor`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.cov` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.cov`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.mod` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/original_res_table.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/pheno.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-5.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-5.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-5.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-6.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-6.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-6.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-7.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-7.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-7.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-8.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-8.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim-8.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-1.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-2.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-3.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-4.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-5.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-6.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-7.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/m1/sim_res_table-8.dta`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv` & `pharmpy-core-0.96.0/tests/testdata/psn/simeval_dir1/summary_cwres.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/allometry_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/allometry_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/amd_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/amd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/bootstrap_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/bootstrap_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/cdd_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/cdd_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/covsearch_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/covsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/estmethod_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/estmethod_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/iivsearch_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/iivsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/iovsearch_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/iovsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/linearize_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/linearize_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/metadata.json` & `pharmpy-core-0.96.0/tests/testdata/results/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/modelsearch_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/modelsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/qa_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/qa_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/ruvsearch_results.json` & `pharmpy-core-0.96.0/tests/testdata/results/ruvsearch_results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/metadata.json` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/metadata.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/.datasets/input_model.datainfo`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/input_model/input_model.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/modelsearch_run1.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/mytab_mox1`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run1/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/modelsearch_run2.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/mytab_mox2`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run2/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/modelsearch_run3.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/mytab_mox3`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run3/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/.pharmpy/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.ext`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.lst`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.mod`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/modelsearch_run4.phi`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/mytab_mox4`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/models/modelsearch_run4/stdout`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/results.csv` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/results.csv`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/testdata/results/tool_databases/modelsearch/results.json` & `pharmpy-core-0.96.0/tests/testdata/results/tool_databases/modelsearch/results.json`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_allometry.py` & `pharmpy-core-0.96.0/tests/tools/test_allometry.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_amd.py` & `pharmpy-core-0.96.0/tests/tools/test_amd.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,15 @@
     if with_datainfo:
         shutil.copy2(models / 'mox_simulated_normal.datainfo', '.')
     shutil.copy2(models / 'mox2.mod', '.')
     shutil.copy2(models / 'mox2.ext', '.')
     shutil.copy2(models / 'mox2.lst', '.')
     shutil.copy2(models / 'mox2.phi', '.')
 
-    model = Model.create_model('mox2.mod')
+    model = Model.parse_model('mox2.mod')
     model = model.replace(name='start')
 
     # NOTE Load results directly in DB to skip fitting
     db_tool = default_tool_database(toolname='amd', path='amd_dir1')
     db_fit = default_tool_database(toolname='modelfit', path=db_tool.path / 'modelfit')
 
     with db_fit.model_database.transaction(model) as txn:
```

### Comparing `pharmpy-core-0.95.0/tests/tools/test_bootstrap.py` & `pharmpy-core-0.96.0/tests/tools/test_bootstrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_cdd.py` & `pharmpy-core-0.96.0/tests/tools/test_cdd.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 from pytest import approx
 
 import pharmpy.tools.cdd.results as cdd
+from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.psn_helpers import model_paths, options_from_command
 
 
 def test_psn_cdd_options(testdata):
     opts = cdd.psn_cdd_options(testdata / 'nonmem' / 'cdd' / 'pheno_real_bin10')
     assert opts['case_column'] == 'ID'
     assert (
@@ -25,19 +26,22 @@
         'dir': 'caseWGTbin10',
     }
 
 
 def test_cdd_psn(load_model_for_test, testdata):
     path = testdata / 'nonmem' / 'cdd' / 'pheno_real_bin10'
     base_model = load_model_for_test(testdata / 'nonmem' / 'cdd' / 'pheno_real.mod')
+    base_model_results = read_modelfit_results(testdata / 'nonmem' / 'cdd' / 'pheno_real.mod')
     cdd_models = [load_model_for_test(p) for p in model_paths(path, 'cdd_*.mod')]
+    cdd_model_results = [read_modelfit_results(p) for p in model_paths(path, 'cdd_*.mod')]
     skipped_individuals = cdd.psn_cdd_skipped_individuals(path)
 
-    cdd_bin_id = cdd.calculate_results(base_model, cdd_models, 'ID', skipped_individuals)
-    print(cdd_bin_id)
+    cdd_bin_id = cdd.calculate_results(
+        base_model, base_model_results, cdd_models, cdd_model_results, 'ID', skipped_individuals
+    )
 
     correct = pd.DataFrame(
         {
             'cook_score': [
                 0.6002247,
                 0.7681936,
                 1.054763,
@@ -126,31 +130,33 @@
     pd.testing.assert_frame_equal(cdd_bin_id.case_results, correct, rtol=1e-4)
 
 
 def test_cdd_calculate_results(load_model_for_test, testdata):
     path = testdata / 'nonmem' / 'cdd' / 'pheno_real_bin10'
     skipped_individuals = cdd.psn_cdd_skipped_individuals(path)
     base_model = load_model_for_test(testdata / 'nonmem' / 'cdd' / 'pheno_real.mod')
+    base_model_results = read_modelfit_results(testdata / 'nonmem' / 'cdd' / 'pheno_real.mod')
     cdd_model_paths = model_paths(path, 'cdd_*.mod')
 
     cdd_models = [load_model_for_test(p) for p in cdd_model_paths]
+    cdd_model_results = [read_modelfit_results(p) for p in cdd_model_paths]
 
     # Results for plain PsN run
-    delta_ofv = cdd.compute_delta_ofv(base_model, cdd_models, skipped_individuals)
+    delta_ofv = cdd.compute_delta_ofv(base_model_results, cdd_model_results, skipped_individuals)
 
     assert delta_ofv == approx(
         [0.27067, 0.35146, 0.79115, 0.84426, 0.86966, 0.37618, 0.69805, 0.49343, 0.31184, 0.31729],
         abs=1e-5,
     )
 
     cdd_estimates = pd.DataFrame(
         data=[
-            pd.Series(m.modelfit_results.parameter_estimates, name=m.name)
-            for m in cdd_models
-            if m.modelfit_results is not None
+            pd.Series(res.parameter_estimates, name=m.name)
+            for m, res in zip(cdd_models, cdd_model_results)
+            if res is not None
         ]
     )
 
     jackknife = cdd.compute_jackknife_covariance_matrix(cdd_estimates)
     jackpsnvalues = [
         3.30415232e-08,
         -1.02486433e-06,
@@ -189,17 +195,17 @@
         -2.00496073e-06,
         2.62509124e-06,
     ]
 
     assert jackknife.values.flatten() == approx(jackpsnvalues, rel=1e-6)
 
     cook_scores = cdd.compute_cook_scores(
-        base_model.modelfit_results.parameter_estimates,
+        base_model_results.parameter_estimates,
         cdd_estimates,
-        base_model.modelfit_results.covariance_matrix,
+        base_model_results.covariance_matrix,
     )
 
     assert cook_scores == approx(
         [
             0.6002247,
             0.7681936,
             1.054763,
@@ -211,15 +217,15 @@
             0.7535628,
             0.5651823,
         ],
         abs=1e-5,
     )
 
     cov_ratios = cdd.compute_covariance_ratios(
-        cdd_models, base_model.modelfit_results.covariance_matrix
+        cdd_model_results, base_model_results.covariance_matrix
     )
 
     assert cov_ratios == approx(
         [
             1.218597,
             1.389662,
             0.906991,
@@ -233,18 +239,23 @@
         ],
         abs=1e-5,
     )
 
     # Replace three estimated cdd_models with fake models without estimates
     # and recompute results to verify handling of missing output
     cdd_models[0] = load_model_for_test(path / 'm1' / 'rem_1.mod')
+    cdd_model_results[0] = read_modelfit_results(path / 'm1' / 'rem_1.mod')
     cdd_models[1] = load_model_for_test(path / 'm1' / 'rem_2.mod')
+    cdd_model_results[1] = read_modelfit_results(path / 'm1' / 'rem_2.mod')
     cdd_models[3] = load_model_for_test(path / 'm1' / 'rem_4.mod')
+    cdd_model_results[3] = read_modelfit_results(path / 'm1' / 'rem_4.mod')
 
-    res = cdd.calculate_results(base_model, cdd_models, 'ID', skipped_individuals)
+    res = cdd.calculate_results(
+        base_model, base_model_results, cdd_models, cdd_model_results, 'ID', skipped_individuals
+    )
 
     assert res.case_results.delta_ofv.values == approx(
         [np.nan, np.nan, 0.79115, np.nan, 0.86966, 0.37618, 0.69805, 0.49343, 0.31184, 0.31729],
         abs=1e-5,
         nan_ok=True,
     )
```

### Comparing `pharmpy-core-0.95.0/tests/tools/test_covsearch.py` & `pharmpy-core-0.96.0/tests/tools/test_covsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_estmethod.py` & `pharmpy-core-0.96.0/tests/tools/test_estmethod.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_exports.py` & `pharmpy-core-0.96.0/tests/tools/test_exports.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_frem.py` & `pharmpy-core-0.96.0/tests/tools/test_frem.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 from pytest import approx
 
 import pharmpy.tools as tools
+from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.frem.models import calculate_parcov_inits, create_model3b
 from pharmpy.tools.frem.results import (
     calculate_results,
     calculate_results_using_bipp,
     get_params,
     psn_frem_results,
 )
@@ -43,45 +44,53 @@
     model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
     newcov = check_covariates(model, ['FA1', 'FA2'])
     assert newcov == []
 
 
 def test_parcov_inits(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'frem' / 'pheno' / 'model_3.mod')
-    params = calculate_parcov_inits(model, 2)
+    res = read_modelfit_results(testdata / 'nonmem' / 'frem' / 'pheno' / 'model_3.mod')
+    params = calculate_parcov_inits(model, res.individual_estimates, 2)
     assert params == approx(
         {
             'OMEGA_3_1': 0.02560327,
             'OMEGA_3_2': -0.001618381,
             'OMEGA_4_1': -0.06764814,
             'OMEGA_4_2': 0.02350935,
         }
     )
 
 
 def test_create_model3b(load_model_for_test, testdata):
     model3 = load_model_for_test(testdata / 'nonmem' / 'frem' / 'pheno' / 'model_3.mod')
+    model3_res = read_modelfit_results(testdata / 'nonmem' / 'frem' / 'pheno' / 'model_3.mod')
     model1b = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
-    model3b = create_model3b(model1b, model3, 2)
+    model3b = create_model3b(model1b, model3, model3_res, 2)
     pset = model3b.parameters
     assert pset['OMEGA_3_1'].init == approx(0.02560327)
     assert pset['POP_CL'].init == 0.00469555
     assert model3b.name == 'model_3b'
 
 
 def test_bipp_covariance(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'frem' / 'pheno' / 'model_4.mod')
-    res = calculate_results_using_bipp(model, continuous=['APGR', 'WGT'], categorical=[], rng=9532)
+    res = read_modelfit_results(testdata / 'nonmem' / 'frem' / 'pheno' / 'model_4.mod')
+    res = calculate_results_using_bipp(
+        model, res, continuous=['APGR', 'WGT'], categorical=[], rng=9532
+    )
     assert res
 
 
 def test_frem_results_pheno(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'frem' / 'pheno' / 'model_4.mod')
+    res = read_modelfit_results(testdata / 'nonmem' / 'frem' / 'pheno' / 'model_4.mod')
     rng = np.random.default_rng(39)
-    res = calculate_results(model, continuous=['APGR', 'WGT'], categorical=[], samples=10, rng=rng)
+    res = calculate_results(
+        model, res, continuous=['APGR', 'WGT'], categorical=[], samples=10, rng=rng
+    )
 
     correct = """parameter,covariate,condition,p5,mean,p95
 CL,APGR,5th,0.972200,1.099294,1.242870
 CL,APGR,95th,0.901919,0.958505,1.013679
 CL,WGT,5th,0.864055,0.941833,1.003508
 CL,WGT,95th,0.993823,1.138392,1.346290
 V,APGR,5th,0.818275,0.900856,0.980333
@@ -246,16 +255,19 @@
     )
     correct.index.name = 'covariate'
     pd.testing.assert_frame_equal(res.covariate_statistics, correct)
 
 
 def test_frem_results_pheno_categorical(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'frem' / 'pheno_cat' / 'model_4.mod')
+    res = read_modelfit_results(testdata / 'nonmem' / 'frem' / 'pheno_cat' / 'model_4.mod')
     rng = np.random.default_rng(8978)
-    res = calculate_results(model, continuous=['WGT'], categorical=['APGRX'], samples=10, rng=rng)
+    res = calculate_results(
+        model, res, continuous=['WGT'], categorical=['APGRX'], samples=10, rng=rng
+    )
 
     correct = """parameter,covariate,condition,p5,mean,p95
 CL,WGT,5th,0.8888806479928386,0.9344068474824363,1.0429216842428766
 CL,WGT,95th,0.9275380047890988,1.1598301793623595,1.2703988351195366
 CL,APGRX,other,0.9915508260440394,1.0837646491987887,1.2173634348518769
 V,WGT,5th,0.9765936229688581,1.0120003772784190,1.0739756346907814
 V,WGT,95th,0.8694233922131289,0.9798663683220742,1.0494977661151397
```

### Comparing `pharmpy-core-0.95.0/tests/tools/test_iivsearch.py` & `pharmpy-core-0.96.0/tests/tools/test_iivsearch.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from pharmpy.modeling import (
     add_iiv,
     add_peripheral_compartment,
     add_pk_iiv,
     create_joint_distribution,
 )
+from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.iivsearch.algorithms import (
     _create_param_dict,
     _is_rv_block_structure,
     _rv_block_structures,
     brute_force_block_structure,
     brute_force_no_of_etas,
     create_eta_blocks,
@@ -36,19 +37,20 @@
     'list_of_parameters, block_structure, no_of_models',
     [([], [], 4), (['QP1'], [], 14), ([], ['ETA_1', 'ETA_2'], 4)],
 )
 def test_brute_force_block_structure(
     load_model_for_test, testdata, list_of_parameters, block_structure, no_of_models
 ):
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox2.mod')
+    res = read_modelfit_results(testdata / 'nonmem' / 'models' / 'mox2.mod')
     model = add_peripheral_compartment(model)
     model = add_iiv(model, list_of_parameters, 'add')
     if block_structure:
         model = create_joint_distribution(
-            model, block_structure, individual_estimates=model.modelfit_results.individual_estimates
+            model, block_structure, individual_estimates=res.individual_estimates
         )
 
     wf = brute_force_block_structure(model)
     fit_tasks = [task.name for task in wf.tasks if task.name.startswith('run')]
 
     assert len(fit_tasks) == no_of_models
 
@@ -88,54 +90,58 @@
     assert block_structures_integer_partitions.count((1, 2, 2)) == 15
     assert block_structures_integer_partitions.count((1, 1, 1, 2)) == 10
     assert block_structures_integer_partitions.count((1, 1, 1, 1, 1)) == 1
 
 
 def test_is_rv_block_structure(load_model_for_test, pheno_path):
     model = load_model_for_test(pheno_path)
+    res = read_modelfit_results(pheno_path)
     model = add_iiv(model, ['TAD', 'S1'], 'exp')
 
     etas_block_structure = (('ETA_1', 'ETA_2'), ('ETA_TAD',), ('ETA_S1',))
     model = create_joint_distribution(
         model,
         list(etas_block_structure[0]),
-        individual_estimates=model.modelfit_results.individual_estimates,
+        individual_estimates=res.individual_estimates,
     )
     etas = model.random_variables.iiv
     assert _is_rv_block_structure(etas, etas_block_structure)
 
     etas_block_structure = (('ETA_1',), ('ETA_2',), ('ETA_TAD', 'ETA_S1'))
     assert not _is_rv_block_structure(etas, etas_block_structure)
 
     etas_block_structure = (('ETA_1',), ('ETA_2', 'ETA_TAD'), ('ETA_S1',))
     assert not _is_rv_block_structure(etas, etas_block_structure)
 
-    model = create_joint_distribution(
-        model, individual_estimates=model.modelfit_results.individual_estimates
-    )
+    model = create_joint_distribution(model, individual_estimates=res.individual_estimates)
     etas_block_structure = (('ETA_1', 'ETA_2', 'ETA_TAD', 'ETA_S1'),)
     etas = model.random_variables.iiv
     assert _is_rv_block_structure(etas, etas_block_structure)
 
 
 def test_create_joint_dist(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox2.mod')
+    res = read_modelfit_results(testdata / 'nonmem' / 'models' / 'mox2.mod')
+    # FIXME!!
+    model = model.replace(modelfit_results=res)
+
     model = add_peripheral_compartment(model)
     model = add_pk_iiv(model)
     etas_block_structure = (('ETA_1', 'ETA_2'), ('ETA_QP1',), ('ETA_VP1',))
     model = create_eta_blocks(etas_block_structure, model)
     assert len(model.random_variables.iiv) == 4
 
     model = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox2.mod')
+    model = model.replace(modelfit_results=res)
     model = add_peripheral_compartment(model)
     model = add_pk_iiv(model)
     model = create_joint_distribution(
         model,
         ['ETA_1', 'ETA_2'],
-        individual_estimates=model.modelfit_results.individual_estimates,
+        individual_estimates=res.individual_estimates,
     )
     etas_block_structure = (('ETA_1',), ('ETA_2',), ('ETA_3', 'ETA_VP1', 'ETA_QP1'))
     model = create_eta_blocks(etas_block_structure, model)
     assert len(model.random_variables.iiv) == 3
 
 
 def test_get_param_names(create_model_for_test, load_model_for_test, testdata):
```

### Comparing `pharmpy-core-0.95.0/tests/tools/test_iovsearch.py` & `pharmpy-core-0.96.0/tests/tools/test_iovsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_mfl.py` & `pharmpy-core-0.96.0/tests/tools/test_mfl.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_ml.py` & `pharmpy-core-0.96.0/tests/tools/test_ml.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import sys
 
 import pytest
 
 from pharmpy.modeling import load_example_model
-from pharmpy.tools import predict_influential_individuals, predict_outliers
+from pharmpy.tools import (
+    load_example_modelfit_results,
+    predict_influential_individuals,
+    predict_outliers,
+)
 
 tflite_condition = (
     sys.version_info >= (3, 10)
     and sys.platform != 'linux'
     or sys.version_info >= (3, 11)
     and sys.platform == 'linux'
 )
 
 
 @pytest.mark.skipif(tflite_condition, reason="Skipping tests requiring tflite for Python 3.10")
 def test_predict_outliers():
     model = load_example_model('pheno')
-    res = predict_outliers(model, model.modelfit_results)
+    results = load_example_modelfit_results('pheno')
+    res = predict_outliers(model, results)
     assert len(res) == 59
     assert res['residual'][1] == pytest.approx(-0.28144291043281555)
 
 
 @pytest.mark.skipif(tflite_condition, reason="Skipping tests requiring tflite for Python 3.10")
 def test_predict_influential_individuals():
     model = load_example_model('pheno')
-    res = predict_influential_individuals(model, model.modelfit_results)
+    results = load_example_modelfit_results('pheno')
+    res = predict_influential_individuals(model, results)
     assert len(res) == 59
     assert res['dofv'][59] == pytest.approx(0.08806940913200378)
```

### Comparing `pharmpy-core-0.95.0/tests/tools/test_modelsearch.py` & `pharmpy-core-0.96.0/tests/tools/test_modelsearch.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_rankfuncs.py` & `pharmpy-core-0.96.0/tests/tools/test_rankfuncs.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_run.py` & `pharmpy-core-0.96.0/tests/tools/test_run.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from pharmpy.internals.fs.cwd import chdir
 from pharmpy.results import read_results
 from pharmpy.tools.run import (
     _create_metadata_common,
     _create_metadata_tool,
     _get_run_setup,
     import_tool,
+    load_example_modelfit_results,
     rank_models,
     read_modelfit_results,
     retrieve_final_model,
     retrieve_models,
     summarize_errors,
     summarize_modelfit_results,
 )
@@ -213,34 +214,28 @@
     res = read_results(results_json_none)
     with pytest.raises(ValueError, match='Attribute \'final_model_name\' is None'):
         retrieve_final_model(res)
 
 
 def test_summarize_errors(load_model_for_test, testdata, tmp_path, pheno_path):
     with chdir(tmp_path):
-        model = load_model_for_test(pheno_path)
+        model = read_modelfit_results(pheno_path)
         shutil.copy2(testdata / 'pheno_data.csv', tmp_path)
 
         error_path = testdata / 'nonmem' / 'errors'
 
         shutil.copy2(testdata / 'nonmem' / 'pheno_real.mod', tmp_path / 'pheno_no_header.mod')
         shutil.copy2(error_path / 'no_header_error.lst', tmp_path / 'pheno_no_header.lst')
         shutil.copy2(testdata / 'nonmem' / 'pheno_real.ext', tmp_path / 'pheno_no_header.ext')
-        model_no_header = load_model_for_test('pheno_no_header.mod')
-        model_no_header = model_no_header.replace(
-            datainfo=model_no_header.datainfo.replace(path=tmp_path / 'pheno_data.csv')
-        )
+        model_no_header = read_modelfit_results('pheno_no_header.mod')
 
         shutil.copy2(testdata / 'nonmem' / 'pheno_real.mod', tmp_path / 'pheno_rounding_error.mod')
         shutil.copy2(error_path / 'rounding_error.lst', tmp_path / 'pheno_rounding_error.lst')
         shutil.copy2(testdata / 'nonmem' / 'pheno_real.ext', tmp_path / 'pheno_rounding_error.ext')
-        model_rounding_error = load_model_for_test('pheno_rounding_error.mod')
-        model_rounding_error = model_rounding_error.replace(
-            datainfo=model_rounding_error.datainfo.replace(path=tmp_path / 'pheno_data.csv')
-        )
+        model_rounding_error = read_modelfit_results('pheno_rounding_error.mod')
 
         models = [model, model_no_header, model_rounding_error]
         summary = summarize_errors(models)
 
         assert 'pheno_real' not in summary.index.get_level_values('model')
         assert len(summary.loc[('pheno_no_header', 'WARNING')]) == 1
         assert len(summary.loc[('pheno_no_header', 'ERROR')]) == 2
@@ -332,116 +327,105 @@
     df = rank_models(base_nan, models, errors_allowed=['rounding_errors'], rank_type='ofv')
     assert df.iloc[0].name == 'm1'
 
 
 def test_summarize_modelfit_results(
     load_model_for_test, create_model_for_test, testdata, pheno_path
 ):
-    pheno = load_model_for_test(pheno_path)
+    pheno = read_modelfit_results(pheno_path)
 
-    summary_single = summarize_modelfit_results(pheno.modelfit_results)
+    summary_single = summarize_modelfit_results(pheno)
 
     assert summary_single.loc['pheno_real']['ofv'] == 586.2760562818805
     assert summary_single['IVCL_estimate'].mean() == 0.0293508
 
     assert len(summary_single.index) == 1
 
-    mox = load_model_for_test(testdata / 'nonmem' / 'models' / 'mox1.mod')
+    mox = read_modelfit_results(testdata / 'nonmem' / 'models' / 'mox1.mod')
 
-    summary_multiple = summarize_modelfit_results([pheno.modelfit_results, mox.modelfit_results])
+    summary_multiple = summarize_modelfit_results([pheno, mox])
 
     assert summary_multiple.loc['mox1']['ofv'] == -624.5229577248352
     assert summary_multiple['IIV_CL_estimate'].mean() == 0.41791
     assert summary_multiple['IIV_CL_V_estimate'].mean() == 0.395647  # One is NaN
 
     assert len(summary_multiple.index) == 2
     assert list(summary_multiple.index) == ['pheno_real', 'mox1']
 
-    pheno_no_res = create_model_for_test(pheno.model_code)
-    pheno_no_res = pheno_no_res.replace(name='pheno_no_res')
-
-    summary_no_res = summarize_modelfit_results(
-        [pheno.modelfit_results, pheno_no_res.modelfit_results]
-    )
+    summary_no_res = summarize_modelfit_results([pheno, None])
 
     assert summary_no_res.loc['pheno_real']['ofv'] == 586.2760562818805
 
-    pheno_multest = load_model_for_test(
+    pheno_multest = read_modelfit_results(
         testdata
         / 'nonmem'
         / 'modelfit_results'
         / 'onePROB'
         / 'multEST'
         / 'noSIM'
         / 'pheno_multEST.mod'
     )
 
-    summary_multest = summarize_modelfit_results(
-        [pheno_multest.modelfit_results, mox.modelfit_results]
-    )
+    summary_multest = summarize_modelfit_results([pheno_multest, mox])
 
     assert len(summary_multest.index) == 2
 
     assert not summary_multest.loc['pheno_multEST']['minimization_successful']
     summary_multest_full = summarize_modelfit_results(
-        [pheno_multest.modelfit_results, mox.modelfit_results], include_all_estimation_steps=True
+        [pheno_multest, mox], include_all_estimation_steps=True
     )
 
     assert len(summary_multest_full.index) == 3
     assert len(set(summary_multest_full.index.get_level_values('model'))) == 2
     assert summary_multest_full.loc['pheno_multEST', 1]['run_type'] == 'estimation'
     assert summary_multest_full.loc['pheno_multEST', 2]['run_type'] == 'evaluation'
 
     assert not summary_multest_full.loc['pheno_multEST', 1]['minimization_successful']
 
-    pheno_multest_no_res = create_model_for_test(pheno_multest.model_code)
-    pheno_multest_no_res = pheno_multest_no_res.replace(name='pheno_multest_no_res')
-
     summary_multest_full_no_res = summarize_modelfit_results(
-        [pheno_multest_no_res.modelfit_results, mox.modelfit_results],
+        [None, mox],
         include_all_estimation_steps=True,
     )
 
     assert summary_multest_full_no_res.loc['mox1', 1]['ofv'] == -624.5229577248352
 
 
 def test_summarize_modelfit_results_errors(load_model_for_test, testdata, tmp_path, pheno_path):
     with chdir(tmp_path):
-        model = load_model_for_test(pheno_path)
+        model = read_modelfit_results(pheno_path)
         shutil.copy2(testdata / 'pheno_data.csv', tmp_path)
 
         error_path = testdata / 'nonmem' / 'errors'
 
         shutil.copy2(testdata / 'nonmem' / 'pheno_real.mod', tmp_path / 'pheno_no_header.mod')
         shutil.copy2(error_path / 'no_header_error.lst', tmp_path / 'pheno_no_header.lst')
         shutil.copy2(testdata / 'nonmem' / 'pheno_real.ext', tmp_path / 'pheno_no_header.ext')
-        model_no_header = load_model_for_test('pheno_no_header.mod')
-        model_no_header = model_no_header.replace(
-            datainfo=model_no_header.datainfo.replace(path=tmp_path / 'pheno_data.csv')
-        )
+        model_no_header = read_modelfit_results('pheno_no_header.mod')
 
         shutil.copy2(testdata / 'nonmem' / 'pheno_real.mod', tmp_path / 'pheno_rounding_error.mod')
         shutil.copy2(error_path / 'rounding_error.lst', tmp_path / 'pheno_rounding_error.lst')
         shutil.copy2(testdata / 'nonmem' / 'pheno_real.ext', tmp_path / 'pheno_rounding_error.ext')
-        model_rounding_error = load_model_for_test('pheno_rounding_error.mod')
-        model_rounding_error = model_rounding_error.replace(
-            datainfo=model_rounding_error.datainfo.replace(path=tmp_path / 'pheno_data.csv')
-        )
+        model_rounding_error = read_modelfit_results('pheno_rounding_error.mod')
 
         results = [
-            model.modelfit_results,
-            model_no_header.modelfit_results,
-            model_rounding_error.modelfit_results,
+            model,
+            model_no_header,
+            model_rounding_error,
         ]
         summary = summarize_modelfit_results(results)
 
         assert summary.loc['pheno_real']['errors_found'] == 0
         assert summary.loc['pheno_real']['warnings_found'] == 0
         assert summary.loc['pheno_no_header']['errors_found'] == 2
         assert summary.loc['pheno_no_header']['warnings_found'] == 1
         assert summary.loc['pheno_rounding_error']['errors_found'] == 2
         assert summary.loc['pheno_rounding_error']['warnings_found'] == 0
 
 
 def test_read_modelfit_results(testdata):
     res = read_modelfit_results(testdata / 'nonmem' / 'pheno_real.mod')
     assert res.ofv == 586.27605628188053
+
+
+def test_load_example_modelfit_results():
+    res = load_example_modelfit_results("pheno")
+    assert res.ofv == 586.27605628188053
```

### Comparing `pharmpy-core-0.95.0/tests/tools/test_runtool.py` & `pharmpy-core-0.96.0/tests/tools/test_runtool.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_ruvsearch.py` & `pharmpy-core-0.96.0/tests/tools/test_ruvsearch.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import replace
 
 import pytest
 
 from pharmpy.modeling import remove_covariance_step
+from pharmpy.tools import read_modelfit_results
 from pharmpy.tools.ruvsearch.results import psn_resmod_results
 from pharmpy.tools.ruvsearch.tool import create_workflow, validate_input
 from pharmpy.workflows import Workflow
 
 
 def test_resmod_results(testdata):
     res = psn_resmod_results(testdata / 'psn' / 'resmod_dir1')
@@ -50,15 +51,17 @@
 
 def test_validate_input():
     validate_input()
 
 
 def test_validate_input_with_model(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'ruvsearch' / 'mox3.mod')
-    remove_covariance_step(model)
+    res = read_modelfit_results(testdata / 'nonmem' / 'ruvsearch' / 'mox3.mod')
+    model = model.replace(modelfit_results=res)
+    model = remove_covariance_step(model)
     validate_input(model=model)
 
 
 @pytest.mark.parametrize(
     ('model_path', 'arguments', 'exception', 'match'),
     [
         (
@@ -139,36 +142,36 @@
 
     with pytest.raises(ValueError, match="missing modelfit results"):
         validate_input(model=model)
 
 
 def test_validate_input_raises_cwres(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'ruvsearch' / 'mox3.mod')
-    remove_covariance_step(model)
-    mfr = model.modelfit_results
-    modelfit_results = replace(mfr, residuals=mfr.residuals.drop(columns=['CWRES']))
+    res = read_modelfit_results(testdata / 'nonmem' / 'ruvsearch' / 'mox3.mod')
+    model = remove_covariance_step(model)
+    modelfit_results = replace(res, residuals=res.residuals.drop(columns=['CWRES']))
     model = model.replace(modelfit_results=modelfit_results)
 
     with pytest.raises(ValueError, match="CWRES"):
         validate_input(model=model)
 
 
 def test_validate_input_raises_cipredi(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'ruvsearch' / 'mox3.mod')
-    remove_covariance_step(model)
-    mfr = model.modelfit_results
-    modelfit_results = replace(mfr, predictions=mfr.predictions.drop(columns=['CIPREDI']))
+    res = read_modelfit_results(testdata / 'nonmem' / 'ruvsearch' / 'mox3.mod')
+    model = remove_covariance_step(model)
+    modelfit_results = replace(res, predictions=res.predictions.drop(columns=['CIPREDI']))
     model = model.replace(modelfit_results=modelfit_results)
 
     with pytest.raises(ValueError, match="IPRED"):
         validate_input(model=model)
 
 
 def test_validate_input_raises_ipred(load_model_for_test, testdata):
     model = load_model_for_test(testdata / 'nonmem' / 'pheno_real.mod')
+    res = read_modelfit_results(testdata / 'nonmem' / 'pheno_real.mod')
     model = remove_covariance_step(model)
-    mfr = model.modelfit_results
-    modelfit_results = replace(mfr, predictions=mfr.predictions.drop(columns=['IPRED']))
+    modelfit_results = replace(res, predictions=res.predictions.drop(columns=['IPRED']))
     model = model.replace(modelfit_results=modelfit_results)
 
     with pytest.raises(ValueError, match="IPRED"):
         validate_input(model=model)
```

### Comparing `pharmpy-core-0.95.0/tests/tools/test_scm.py` & `pharmpy-core-0.96.0/tests/tools/test_scm.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_start_model.py` & `pharmpy-core-0.96.0/tests/tools/test_start_model.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/tools/test_summarize_individuals.py` & `pharmpy-core-0.96.0/tests/tools/test_summarize_individuals.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,19 @@
 
 import numpy as np
 import pandas as pd
 import pytest
 
 from pharmpy.modeling import read_model
 from pharmpy.results import ModelfitResults
-from pharmpy.tools import summarize_individuals, summarize_individuals_count_table
+from pharmpy.tools import (
+    read_modelfit_results,
+    summarize_individuals,
+    summarize_individuals_count_table,
+)
 from pharmpy.tools.funcs.summarize_individuals import dofv
 
 
 def test_summarize_individuals_count_table():
     df = pd.DataFrame(
         {
             'model': ['start_model'] * 3 + ['candidate1'] * 3 + ['candidate2'] * 3,
@@ -40,14 +44,17 @@
     and sys.platform == 'linux'
 )
 
 
 @pytest.mark.skipif(tflite_condition, reason="Skipping tests requiring tflite for Python 3.10")
 def test_tflite_not_installed(pheno_path, monkeypatch):
     model = read_model(pheno_path)
+    results = read_modelfit_results(pheno_path)
+    # FIXME
+    model = model.replace(modelfit_results=results)
 
     df = summarize_individuals([model])
     assert not df['predicted_dofv'].isnull().any().any()
 
     with pytest.warns(UserWarning, match='tflite is not installed'):
         monkeypatch.setitem(sys.modules, 'tflite_runtime', None)
         df = summarize_individuals([model])
@@ -58,17 +65,21 @@
     candidate_model = read_model(pheno_path)
     res = dofv(None, candidate_model)
     assert np.isnan(res)
 
 
 def test_dofv_modelfit_results_is_none(pheno_path):
     parent_model = read_model(pheno_path)
+    res = read_modelfit_results(pheno_path)
+    parent_model = parent_model.replace(modelfit_results=res)
     candidate_model = parent_model.replace(modelfit_results=None)
     res = dofv(parent_model, candidate_model)
     assert res.isna().all()
 
 
 def test_dofv_individual_ofv_is_none(pheno_path):
     parent_model = read_model(pheno_path)
+    res = read_modelfit_results(pheno_path)
+    parent_model = parent_model.replace(modelfit_results=res)
     candidate_model = parent_model.replace(modelfit_results=ModelfitResults())
     res = dofv(parent_model, candidate_model)
     assert res.isna().all()
```

### Comparing `pharmpy-core-0.95.0/tests/tools/test_wrap.py` & `pharmpy-core-0.96.0/tests/tools/test_wrap.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/workflows/test_call.py` & `pharmpy-core-0.96.0/tests/workflows/test_call.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/workflows/test_execute.py` & `pharmpy-core-0.96.0/tests/workflows/test_execute.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/workflows/test_model_database.py` & `pharmpy-core-0.96.0/tests/workflows/test_model_database.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tests/workflows/test_workflow.py` & `pharmpy-core-0.96.0/tests/workflows/test_workflow.py`

 * *Files identical despite different names*

### Comparing `pharmpy-core-0.95.0/tox.ini` & `pharmpy-core-0.96.0/tox.ini`

 * *Files identical despite different names*

