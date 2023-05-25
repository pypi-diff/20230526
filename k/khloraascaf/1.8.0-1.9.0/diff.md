# Comparing `tmp/khloraascaf-1.8.0.tar.gz` & `tmp/khloraascaf-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khloraascaf-1.8.0.tar", last modified: Tue May  9 12:11:22 2023, max compression
+gzip compressed data, was "khloraascaf-1.9.0.tar", last modified: Thu May 25 22:49:15 2023, max compression
```

## Comparing `khloraascaf-1.8.0.tar` & `khloraascaf-1.9.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.363547 khloraascaf-1.8.0/
--rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/LICENCE
--rw-r--r--   0 root         (0) root         (0)    46344 2023-05-09 12:11:22.362547 khloraascaf-1.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     4964 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-09 12:11:22.363547 khloraascaf-1.8.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.346546 khloraascaf-1.8.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.354547 khloraascaf-1.8.0/src/khloraascaf/
--rw-rw-rw-   0 root         (0) root         (0)     1579 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/__main__.py
--rw-rw-rw-   0 root         (0) root         (0)    13402 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/cli.py
--rw-rw-rw-   0 root         (0) root         (0)     5600 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.360547 khloraascaf-1.8.0/src/khloraascaf/ilp/
--rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/dirf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/invf_sets.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_circuit.py
--rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_dirf.py
--rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_invf.py
--rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_presscore.py
--rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_repeated_fragments.py
--rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_to_solver.py
--rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_var_db.py
--rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/lib.py
--rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/multiplied_doubled_contig_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     8323 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/py.typed
--rw-rw-rw-   0 root         (0) root         (0)    21582 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/result.py
--rw-rw-rw-   0 root         (0) root         (0)    28593 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/run_metadata.py
--rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/scaffolding_methods.py
--rw-rw-rw-   0 root         (0) root         (0)     7160 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/src/khloraascaf/utils_debug.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.356547 khloraascaf-1.8.0/src/khloraascaf.egg-info/
--rw-r--r--   0 root         (0) root         (0)    46344 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1174 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       77 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-05-09 12:11:22.000000 khloraascaf-1.8.0/src/khloraascaf.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-09 12:11:22.362547 khloraascaf-1.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    13219 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_assembly_graph.py
--rw-rw-rw-   0 root         (0) root         (0)     3186 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)    15226 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_run_metdata.py
--rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_toy_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     2989 2023-05-09 12:10:59.000000 khloraascaf-1.8.0/tests/test_utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 22:49:15.244953 khloraascaf-1.9.0/
+-rw-rw-rw-   0 root         (0) root         (0)    34916 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/LICENCE
+-rw-r--r--   0 root         (0) root         (0)    46317 2023-05-25 22:49:15.243954 khloraascaf-1.9.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4937 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1339 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 22:49:15.244953 khloraascaf-1.9.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 22:49:15.231954 khloraascaf-1.9.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 22:49:15.237954 khloraascaf-1.9.0/src/khloraascaf/
+-rw-rw-rw-   0 root         (0) root         (0)     1981 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1760 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/__main__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13402 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     5619 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/cli.py
+-rw-rw-rw-   0 root         (0) root         (0)     6571 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 22:49:15.241954 khloraascaf-1.9.0/src/khloraascaf/ilp/
+-rw-rw-rw-   0 root         (0) root         (0)      372 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    11068 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/dirf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)    10725 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/invf_sets.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3418 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_max_dirf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3402 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_max_invf.py
+-rw-rw-rw-   0 root         (0) root         (0)     3738 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_max_presscore.py
+-rw-rw-rw-   0 root         (0) root         (0)    12009 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_repeated_fragments.py
+-rw-rw-rw-   0 root         (0) root         (0)     3027 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_to_solver.py
+-rw-rw-rw-   0 root         (0) root         (0)    10512 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_var_db.py
+-rw-rw-rw-   0 root         (0) root         (0)     4402 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1124 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12867 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/multiplied_doubled_contig_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     8323 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/py.typed
+-rw-rw-rw-   0 root         (0) root         (0)    21582 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/result.py
+-rw-rw-rw-   0 root         (0) root         (0)    28593 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/run_metadata.py
+-rw-rw-rw-   0 root         (0) root         (0)    21539 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/scaffolding_methods.py
+-rw-rw-rw-   0 root         (0) root         (0)     7160 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/src/khloraascaf/utils_debug.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 22:49:15.238954 khloraascaf-1.9.0/src/khloraascaf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    46317 2023-05-25 22:49:15.000000 khloraascaf-1.9.0/src/khloraascaf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1174 2023-05-25 22:49:15.000000 khloraascaf-1.9.0/src/khloraascaf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 22:49:15.000000 khloraascaf-1.9.0/src/khloraascaf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       77 2023-05-25 22:49:15.000000 khloraascaf-1.9.0/src/khloraascaf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-05-25 22:49:15.000000 khloraascaf-1.9.0/src/khloraascaf.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 22:49:15.243954 khloraascaf-1.9.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    13219 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/tests/test_assembly_graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     3745 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/tests/test_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       63 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/tests/test_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)    15226 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/tests/test_run_metdata.py
+-rw-rw-rw-   0 root         (0) root         (0)    22601 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/tests/test_toy_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     2989 2023-05-25 22:48:59.000000 khloraascaf-1.9.0/tests/test_utils_debug.py
```

### Comparing `khloraascaf-1.8.0/LICENCE` & `khloraascaf-1.9.0/LICENCE`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/PKG-INFO` & `khloraascaf-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.8.0
+Version: 1.9.0
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -677,16 +677,16 @@
         library, you may consider it more useful to permit linking proprietary
         applications with the library. If this is what you want to do, use the
         GNU Lesser General Public License instead of this License. But first,
         please read <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding
 Project-URL: Repository, https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding
-Project-URL: Documentation, https://khloraa_scaffolding.readthedocs.io
-Project-URL: Changelog, https://khloraa_scaffolding.readthedocs.io/en/latest/changelog.html
+Project-URL: Documentation, https://khloraa-scaffolding.readthedocs.io
+Project-URL: Changelog, https://khloraa-scaffolding.readthedocs.io/en/latest/changelog.html
 Keywords: Scaffolding,Chloroplast,Assembly,DNA repeats
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -698,24 +698,24 @@
 
 [![Latest release](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/badges/release.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/releases)
 [![PyPI version](https://badge.fury.io/py/khloraascaf.svg)](https://badge.fury.io/py/khloraascaf)
 [![Coverage report](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/badges/main/coverage.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Pylint score](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/jobs/artifacts/main/raw/pylint/pylint.svg?job=pylint)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Mypy](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/jobs/artifacts/main/raw/mypy/mypy.svg?job=mypy)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Pipeline status](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/badges/main/pipeline.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
-[![Documentation Status](https://readthedocs.org/projects/khloraa_scaffolding/badge/?version=latest)](https://khloraa_scaffolding.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/khloraa_scaffolding/badge/?version=latest)](https://khloraa-scaffolding.readthedocs.io/en/latest)
 
  <img src="docs/img/logo_transp.png" alt="khloraascaf logo"
 width="200" height="200">
 
 `khloraascaf` is a Python3 package that implements a dedicated scaffolding method for chloroplast genomes.
 
 From input data files, it computes combinations of Integer Linear Programming (ILP) programs and write the result of the best one in output files.
 
-Please have a look to the [documentation website](https://khloraa_scaffolding.readthedocs.io) for more details.
+Please have a look to the [documentation website](https://khloraa-scaffolding.readthedocs.io) for more details.
 
 
 ## Quick installation
 
 To install the `khloraascaf` package from the [PyPI repository](https://pypi.org/project/khloraascaf/), run the `pip` command :
 ```sh
 pip install khloraascaf
@@ -725,20 +725,20 @@
 
 
 ## Quick usage example
 
 ```python
 from pathlib import Path
 
-from khloraascaf import IOConfig, MetadataAllSolutions, scaffolding
-from khloraascaf.inputs import SOLVER_CBC
+from khloraascaf import SOLVER_CBC, IOConfig, MetadataAllSolutions, scaffolding
 
-# ------------------------------------------------------------------------ #
+
+# ---------------------------------------------------------------------------- #
 # Run the example
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
 # Compute the scaffolding using the assembly data
@@ -753,17 +753,17 @@
 #
 # khloraascaf creates a directory with a unique name
 #   to put all the files it has created
 #
 assert outdir_gen in outdir.glob('*')
 print(outdir_gen)
 
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 # Dive into the results
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 #
 # Use metadata class to easily dive into the results
 # (you can also see by hand the solutions.yaml file that has been produced)
 #
 all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
 #
 # * How many solutions the scaffolding has produced?
```

### Comparing `khloraascaf-1.8.0/README.md` & `khloraascaf-1.9.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 [![Latest release](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/badges/release.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/releases)
 [![PyPI version](https://badge.fury.io/py/khloraascaf.svg)](https://badge.fury.io/py/khloraascaf)
 [![Coverage report](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/badges/main/coverage.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Pylint score](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/jobs/artifacts/main/raw/pylint/pylint.svg?job=pylint)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Mypy](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/jobs/artifacts/main/raw/mypy/mypy.svg?job=mypy)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Pipeline status](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/badges/main/pipeline.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
-[![Documentation Status](https://readthedocs.org/projects/khloraa_scaffolding/badge/?version=latest)](https://khloraa_scaffolding.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/khloraa_scaffolding/badge/?version=latest)](https://khloraa-scaffolding.readthedocs.io/en/latest)
 
  <img src="docs/img/logo_transp.png" alt="khloraascaf logo"
 width="200" height="200">
 
 `khloraascaf` is a Python3 package that implements a dedicated scaffolding method for chloroplast genomes.
 
 From input data files, it computes combinations of Integer Linear Programming (ILP) programs and write the result of the best one in output files.
 
-Please have a look to the [documentation website](https://khloraa_scaffolding.readthedocs.io) for more details.
+Please have a look to the [documentation website](https://khloraa-scaffolding.readthedocs.io) for more details.
 
 
 ## Quick installation
 
 To install the `khloraascaf` package from the [PyPI repository](https://pypi.org/project/khloraascaf/), run the `pip` command :
 ```sh
 pip install khloraascaf
@@ -29,20 +29,20 @@
 
 
 ## Quick usage example
 
 ```python
 from pathlib import Path
 
-from khloraascaf import IOConfig, MetadataAllSolutions, scaffolding
-from khloraascaf.inputs import SOLVER_CBC
+from khloraascaf import SOLVER_CBC, IOConfig, MetadataAllSolutions, scaffolding
 
-# ------------------------------------------------------------------------ #
+
+# ---------------------------------------------------------------------------- #
 # Run the example
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
 # Compute the scaffolding using the assembly data
@@ -57,17 +57,17 @@
 #
 # khloraascaf creates a directory with a unique name
 #   to put all the files it has created
 #
 assert outdir_gen in outdir.glob('*')
 print(outdir_gen)
 
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 # Dive into the results
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 #
 # Use metadata class to easily dive into the results
 # (you can also see by hand the solutions.yaml file that has been produced)
 #
 all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
 #
 # * How many solutions the scaffolding has produced?
```

### Comparing `khloraascaf-1.8.0/pyproject.toml` & `khloraascaf-1.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 
 name = "khloraascaf"
-version = "1.8.0"
+version = "1.9.0"
 authors = [{ name = "vepain", email = "victor.epain@laposte.net" }]
 description = "A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage."
 keywords = ["Scaffolding", "Chloroplast", "Assembly", "DNA repeats"]
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -27,13 +27,13 @@
     "PyYAML >=6.0, < 6.1",
 ]
 
 [project.urls]
 
 Homepage = "https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding"
 Repository = "https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding"
-Documentation = "https://khloraa_scaffolding.readthedocs.io"
-Changelog = "https://khloraa_scaffolding.readthedocs.io/en/latest/changelog.html"
+Documentation = "https://khloraa-scaffolding.readthedocs.io"
+Changelog = "https://khloraa-scaffolding.readthedocs.io/en/latest/changelog.html"
 
 [tool.setuptools.package-data]
 
 khloraascaf = ["py.typed"]
```

### Comparing `khloraascaf-1.8.0/src/khloraascaf/__init__.py` & `khloraascaf-1.9.0/src/khloraascaf/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 # -*- coding=utf-8 -*-
 
 """Init file for module path shortcuts."""
 
 # flake8: noqa
 
+# REFACTOR import precisely, not with '*'
 # ============================================================================ #
 #                                ASSEMBLY GRAPH                                #
 # ============================================================================ #
 from khloraascaf.assembly_graph import *  # DOCU be sure it's described
 # ============================================================================ #
 #                                  EXCEPTIONS                                  #
 # ============================================================================ #
 from khloraascaf.exceptions import *  # DOCU be sure to describe
 # ============================================================================ #
+#                                     INPUT                                    #
+# ============================================================================ #
+from khloraascaf.inputs import *  # DOCU be sure to describe
+# ============================================================================ #
 #                                    LIBRARY                                   #
 # ============================================================================ #
-from khloraascaf.lib import *
+from khloraascaf.lib import *  # DOCU be sure to describe
 # ============================================================================ #
 #                                 RUN METADATA                                 #
 # ============================================================================ #
 from khloraascaf.run_metadata import *  # DOCU be sure to describe
 # ============================================================================ #
 #                              SCAFFOLDING METHODS                             #
 # ============================================================================ #
-from khloraascaf.scaffolding_methods import *
+from khloraascaf.scaffolding_methods import *  # DOCU be sure to describe
```

### Comparing `khloraascaf-1.8.0/src/khloraascaf/__main__.py` & `khloraascaf-1.9.0/src/khloraascaf/__main__.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/assembly_graph.py` & `khloraascaf-1.9.0/src/khloraascaf/assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/cli.py` & `khloraascaf-1.9.0/src/khloraascaf/cli.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/exceptions.py` & `khloraascaf-1.9.0/src/khloraascaf/exceptions.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,14 +18,24 @@
     """Scaffolding error exception."""
 
     def __init__(self, outdir: Path):
         """The Initialiser."""
         super().__init__()
         self.__outdir: Path = outdir
 
+    def outdir_gen(self) -> Path:
+        """Unique identifier output directory path.
+
+        Returns
+        -------
+        Path
+            Unique identifier output directory path
+        """
+        return self.__outdir
+
     def __str__(self) -> str:
         """Exception message."""
         return (
             'Scaffolding fails\n'
             f'\tSee output directory: {self.__outdir}'
         )
 
@@ -67,14 +77,24 @@
     """Wrong region identifier exception."""
 
     def __init__(self, region_id: str):
         """The Initializer."""
         super().__init__()
         self.__region_id = region_id
 
+    def region_id(self) -> str:
+        """Wrong region identifier.
+
+        Returns
+        -------
+        str
+            Wrong region identifier
+        """
+        return self.__region_id
+
     def __str__(self) -> str:
         """Print the exception message.
 
         Returns
         -------
         str
             Exception message
@@ -89,14 +109,24 @@
     """Wrong solver name exception."""
 
     def __init__(self, solver: str):
         """The Initializer."""
         super().__init__()
         self.__solver = solver
 
+    def solver(self) -> str:
+        """Wrong solver name.
+
+        Returns
+        -------
+        str
+            Wrong solver name
+        """
+        return self.__solver
+
     def __str__(self) -> str:
         """Print the exception message.
 
         Returns
         -------
         str
             Exception message
@@ -113,14 +143,34 @@
     _PROBLEM_ID = 'THE PROBLEM'
 
     def __init__(self, status: str, ilp_combi: Iterable[RegionIDT]):
         super().__init__()
         self.__status: str = status
         self.__ilp_combi: tuple[RegionIDT, ...] = tuple(ilp_combi)
 
+    def status(self) -> str:
+        """Status.
+
+        Returns
+        -------
+        str
+            Status
+        """
+        return self.__status
+
+    def ilp_combi(self) -> tuple[RegionIDT, ...]:
+        """ILP code combination.
+
+        Returns
+        -------
+        tuple of RegionIDT
+            ILP code combination
+        """
+        return self.__ilp_combi
+
     def __str__(self) -> str:
         """Print the exception message.
 
         Returns
         -------
         str
             Exception message
```

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/dirf_sets.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/dirf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/invf_sets.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/invf_sets.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_circuit.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_circuit.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_dirf.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_max_dirf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_invf.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_max_invf.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_max_presscore.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_max_presscore.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_repeated_fragments.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_repeated_fragments.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_to_solver.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_to_solver.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/ilp/pulp_var_db.py` & `khloraascaf-1.9.0/src/khloraascaf/ilp/pulp_var_db.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/inputs.py` & `khloraascaf-1.9.0/src/khloraascaf/inputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/lib.py` & `khloraascaf-1.9.0/src/khloraascaf/lib.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/multiplied_doubled_contig_graph.py` & `khloraascaf-1.9.0/src/khloraascaf/multiplied_doubled_contig_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/outputs.py` & `khloraascaf-1.9.0/src/khloraascaf/outputs.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/result.py` & `khloraascaf-1.9.0/src/khloraascaf/result.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/run_metadata.py` & `khloraascaf-1.9.0/src/khloraascaf/run_metadata.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/scaffolding_methods.py` & `khloraascaf-1.9.0/src/khloraascaf/scaffolding_methods.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf/utils_debug.py` & `khloraascaf-1.9.0/src/khloraascaf/utils_debug.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/src/khloraascaf.egg-info/PKG-INFO` & `khloraascaf-1.9.0/src/khloraascaf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khloraascaf
-Version: 1.8.0
+Version: 1.9.0
 Summary: A python package that takes an assembly result of a chloroplast genome and continues it by computing the scaffolding stage.
 Author-email: vepain <victor.epain@laposte.net>
 License: ### GNU GENERAL PUBLIC LICENSE
         
         Version 3, 29 June 2007
         
         Copyright (C) 2007 Free Software Foundation, Inc.
@@ -677,16 +677,16 @@
         library, you may consider it more useful to permit linking proprietary
         applications with the library. If this is what you want to do, use the
         GNU Lesser General Public License instead of this License. But first,
         please read <https://www.gnu.org/licenses/why-not-lgpl.html>.
         
 Project-URL: Homepage, https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding
 Project-URL: Repository, https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding
-Project-URL: Documentation, https://khloraa_scaffolding.readthedocs.io
-Project-URL: Changelog, https://khloraa_scaffolding.readthedocs.io/en/latest/changelog.html
+Project-URL: Documentation, https://khloraa-scaffolding.readthedocs.io
+Project-URL: Changelog, https://khloraa-scaffolding.readthedocs.io/en/latest/changelog.html
 Keywords: Scaffolding,Chloroplast,Assembly,DNA repeats
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
@@ -698,24 +698,24 @@
 
 [![Latest release](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/badges/release.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/releases)
 [![PyPI version](https://badge.fury.io/py/khloraascaf.svg)](https://badge.fury.io/py/khloraascaf)
 [![Coverage report](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/badges/main/coverage.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Pylint score](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/jobs/artifacts/main/raw/pylint/pylint.svg?job=pylint)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Mypy](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/jobs/artifacts/main/raw/mypy/mypy.svg?job=mypy)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
 [![Pipeline status](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/badges/main/pipeline.svg)](https://gitlab.com/khloraa_scaffolding/khloraa_scaffolding/-/commits/main)
-[![Documentation Status](https://readthedocs.org/projects/khloraa_scaffolding/badge/?version=latest)](https://khloraa_scaffolding.readthedocs.io/en/latest/?badge=latest)
+[![Documentation Status](https://readthedocs.org/projects/khloraa_scaffolding/badge/?version=latest)](https://khloraa-scaffolding.readthedocs.io/en/latest)
 
  <img src="docs/img/logo_transp.png" alt="khloraascaf logo"
 width="200" height="200">
 
 `khloraascaf` is a Python3 package that implements a dedicated scaffolding method for chloroplast genomes.
 
 From input data files, it computes combinations of Integer Linear Programming (ILP) programs and write the result of the best one in output files.
 
-Please have a look to the [documentation website](https://khloraa_scaffolding.readthedocs.io) for more details.
+Please have a look to the [documentation website](https://khloraa-scaffolding.readthedocs.io) for more details.
 
 
 ## Quick installation
 
 To install the `khloraascaf` package from the [PyPI repository](https://pypi.org/project/khloraascaf/), run the `pip` command :
 ```sh
 pip install khloraascaf
@@ -725,20 +725,20 @@
 
 
 ## Quick usage example
 
 ```python
 from pathlib import Path
 
-from khloraascaf import IOConfig, MetadataAllSolutions, scaffolding
-from khloraascaf.inputs import SOLVER_CBC
+from khloraascaf import SOLVER_CBC, IOConfig, MetadataAllSolutions, scaffolding
 
-# ------------------------------------------------------------------------ #
+
+# ---------------------------------------------------------------------------- #
 # Run the example
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 #
 # Prepare the scaffolding result directory
 #
 outdir = Path('scaffolding_result')
 outdir.mkdir(exist_ok=True)
 #
 # Compute the scaffolding using the assembly data
@@ -753,17 +753,17 @@
 #
 # khloraascaf creates a directory with a unique name
 #   to put all the files it has created
 #
 assert outdir_gen in outdir.glob('*')
 print(outdir_gen)
 
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 # Dive into the results
-# ------------------------------------------------------------------------ #
+# ---------------------------------------------------------------------------- #
 #
 # Use metadata class to easily dive into the results
 # (you can also see by hand the solutions.yaml file that has been produced)
 #
 all_solutions_metadata = MetadataAllSolutions.from_run_directory(outdir_gen)
 #
 # * How many solutions the scaffolding has produced?
```

### Comparing `khloraascaf-1.8.0/src/khloraascaf.egg-info/SOURCES.txt` & `khloraascaf-1.9.0/src/khloraascaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/tests/test_assembly_graph.py` & `khloraascaf-1.9.0/tests/test_assembly_graph.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/tests/test_exceptions.py` & `khloraascaf-1.9.0/tests/test_exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 
 
 # ============================================================================ #
 #                                TEST FUNCTIONS                                #
 # ============================================================================ #
 def test_scaffolding_error():
     """Test ScaffoldingError exception."""
-    exc = ScaffoldingError(Path('./jaaj'))
+    outdir_gen = Path('./jaaj')
+    exc = ScaffoldingError(outdir_gen)
+    assert exc.outdir_gen() == outdir_gen
     assert str(exc) == (
         'Scaffolding fails\n'
         '\tSee output directory: jaaj'
     )
 
 
 def test_repeat_scaffolding_error():
@@ -53,52 +55,61 @@
     exc = CombineScaffoldingError()
     assert str(exc) == 'The scaffolding combination has failed'
 
 
 def test_wrong_region_code():
     """Test WrongRegionID exception."""
     exc = WrongRegionID(IR_REGION_ID)
+    assert exc.region_id() == IR_REGION_ID
     assert str(exc) == "The region identifier 'ir' is not correct"
 
 
 def test_wrong_solver_name():
     """Test WrongSolverName exception."""
-    exc = WrongSolverName('wrong_solver')
-    assert str(exc) == 'The solver name wrong_solver is not correct'
+    wrong_solver_name = 'un_oracle_ma_dit'
+    exc = WrongSolverName(wrong_solver_name)
+    assert exc.solver() == wrong_solver_name
+    assert str(exc) == 'The solver name un_oracle_ma_dit is not correct'
 
 
 def test_unfeasible_ir():
     """Test UnfeasibleIR exception."""
-    exc = UnfeasibleIR(
-        LpStatus[LpStatusInfeasible], (IR_REGION_ID, SC_REGION_ID),
-    )
+    bad_status = LpStatus[LpStatusInfeasible]
+    ilp_combi = (IR_REGION_ID, SC_REGION_ID)
+    exc = UnfeasibleIR(bad_status, ilp_combi)
+    assert exc.status() == bad_status
+    assert exc.ilp_combi() == ilp_combi
     assert str(exc) == (
         'The Find the best inverted repeats problem is unfeasible:\n'
         '\t* ILP codes: ir-sc\n'
         '\t* Status: Infeasible'
     )
 
 
 def test_unfeasible_dr():
     """Test UnfeasibleDR exception."""
-    exc = UnfeasibleDR(
-        LpStatus[LpStatusInfeasible], (IR_REGION_ID, SC_REGION_ID),
-    )
+    bad_status = LpStatus[LpStatusInfeasible]
+    ilp_combi = (IR_REGION_ID, SC_REGION_ID)
+    exc = UnfeasibleDR(bad_status, ilp_combi)
+    assert exc.status() == bad_status
+    assert exc.ilp_combi() == ilp_combi
     assert str(exc) == (
         'The Find the best direct repeats problem is unfeasible:\n'
         '\t* ILP codes: ir-sc\n'
         '\t* Status: Infeasible'
     )
 
 
 def test_unfeasible_sc():
     """Test UnfeasibleSC exception."""
-    exc = UnfeasibleSC(
-        LpStatus[LpStatusInfeasible], (IR_REGION_ID, SC_REGION_ID),
-    )
+    bad_status = LpStatus[LpStatusInfeasible]
+    ilp_combi = (IR_REGION_ID, SC_REGION_ID)
+    exc = UnfeasibleSC(bad_status, ilp_combi)
+    assert exc.status() == bad_status
+    assert exc.ilp_combi() == ilp_combi
     assert str(exc) == (
         'The Find the best single copy regions problem is unfeasible:\n'
         '\t* ILP codes: ir-sc\n'
         '\t* Status: Infeasible'
     )
```

### Comparing `khloraascaf-1.8.0/tests/test_run_metdata.py` & `khloraascaf-1.9.0/tests/test_run_metdata.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/tests/test_toy_examples.py` & `khloraascaf-1.9.0/tests/test_toy_examples.py`

 * *Files identical despite different names*

### Comparing `khloraascaf-1.8.0/tests/test_utils_debug.py` & `khloraascaf-1.9.0/tests/test_utils_debug.py`

 * *Files identical despite different names*

