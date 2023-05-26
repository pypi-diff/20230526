# Comparing `tmp/neumann-1.0.6.tar.gz` & `tmp/neumann-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neumann-1.0.6.tar", last modified: Sun May  7 16:54:48 2023, max compression
+gzip compressed data, was "neumann-1.0.7.tar", last modified: Fri May 26 16:49:56 2023, max compression
```

## Comparing `neumann-1.0.6.tar` & `neumann-1.0.7.tar`

### file list

```diff
@@ -1,80 +1,81 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-05-07 16:54:42.000000 neumann-1.0.6/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-05-07 16:54:42.000000 neumann-1.0.6/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-05-07 16:54:48.153205 neumann-1.0.6/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4789 2023-05-07 16:54:42.000000 neumann-1.0.6/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-05-07 16:54:42.000000 neumann-1.0.6/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-05-07 16:54:42.000000 neumann-1.0.6/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-07 16:54:48.153205 neumann-1.0.6/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2324 2023-05-07 16:54:42.000000 neumann-1.0.6/setup.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.145205 neumann-1.0.6/src/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.145205 neumann-1.0.6/src/neumann/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.149205 neumann-1.0.6/src/neumann/approx/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/approx/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/approx/func.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7210 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/approx/lagrange.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9840 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/approx/mls.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5607 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/arraysetops.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/decorate.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.149205 neumann-1.0.6/src/neumann/function/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2530 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/constraint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9141 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3851 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/metafunction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/relation.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/function/testfunction.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/hist.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.149205 neumann-1.0.6/src/neumann/linalg/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5029 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/abstract.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/exceptions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24717 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frame.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/src/neumann/linalg/frontal/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8015 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/frontal.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2131 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/frutils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7447 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/path.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/postproc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10580 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/proc.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1605 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/frontal/topo.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12875 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/meta.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/solve.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/src/neumann/linalg/sparse/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/sparse/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10045 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/sparse/csr.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10297 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/sparse/jaggedarray.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/sparse/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12663 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/tensor.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3137 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/top.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29691 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6763 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/linalg/vector.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4333 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/logical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3811 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/numint.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/src/neumann/optimize/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/optimize/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/optimize/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14973 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/optimize/ga.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    31396 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/optimize/lp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/src/neumann/topology/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/topology/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5492 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/topology/graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13118 2023-05-07 16:54:42.000000 neumann-1.0.6/src/neumann/utils.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.149205 neumann-1.0.6/src/neumann.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1856 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-05-07 16:54:48.000000 neumann-1.0.6/src/neumann.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-07 16:54:48.153205 neumann-1.0.6/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1185 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_approx.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4268 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_function.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2220 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_ga.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      579 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_graph.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    33834 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_linalg.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3776 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_logical.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7684 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_lpp.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      682 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_numint.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2023-05-07 16:54:42.000000 neumann-1.0.6/tests/test_utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.654960 neumann-1.0.7/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1069 2023-05-26 16:49:50.000000 neumann-1.0.7/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-05-26 16:49:50.000000 neumann-1.0.7/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-05-26 16:49:56.654960 neumann-1.0.7/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4789 2023-05-26 16:49:50.000000 neumann-1.0.7/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      116 2023-05-26 16:49:50.000000 neumann-1.0.7/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2023-05-26 16:49:50.000000 neumann-1.0.7/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-26 16:49:56.654960 neumann-1.0.7/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2203 2023-05-26 16:49:50.000000 neumann-1.0.7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.642960 neumann-1.0.7/src/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.646960 neumann-1.0.7/src/neumann/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      172 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.646960 neumann-1.0.7/src/neumann/approx/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/approx/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/approx/func.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7210 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/approx/lagrange.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9900 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/approx/mls.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5607 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/arraysetops.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1443 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/decorate.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.646960 neumann-1.0.7/src/neumann/function/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       72 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/function/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2530 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/function/constraint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9141 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/function/function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2656 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/function/functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3840 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/function/metafunction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2875 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/function/relation.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/function/testfunction.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/hist.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.650960 neumann-1.0.7/src/neumann/linalg/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      106 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6305 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/abstract.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      443 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/exceptions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25497 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/frame.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.650960 neumann-1.0.7/src/neumann/linalg/frontal/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       47 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/frontal/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8015 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/frontal/frontal.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2131 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/frontal/frutils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7447 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/frontal/path.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1103 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/frontal/postproc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10580 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/frontal/proc.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1605 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/frontal/topo.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      240 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/imap.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14784 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/meta.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7996 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/solve.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.650960 neumann-1.0.7/src/neumann/linalg/sparse/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/sparse/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10045 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/sparse/csr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10297 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/sparse/jaggedarray.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1224 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/sparse/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10418 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/tensor.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      998 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/testing.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6504 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/tr.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29683 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6768 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/linalg/vector.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4333 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3811 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/numint.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.650960 neumann-1.0.7/src/neumann/optimize/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      105 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/optimize/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      473 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/optimize/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14973 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/optimize/ga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    31591 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/optimize/lp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.650960 neumann-1.0.7/src/neumann/topology/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       21 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/topology/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5492 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/topology/graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13116 2023-05-26 16:49:50.000000 neumann-1.0.7/src/neumann/utils.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.646960 neumann-1.0.7/src/neumann.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5753 2023-05-26 16:49:56.000000 neumann-1.0.7/src/neumann.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1891 2023-05-26 16:49:56.000000 neumann-1.0.7/src/neumann.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-26 16:49:56.000000 neumann-1.0.7/src/neumann.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-26 16:49:56.000000 neumann-1.0.7/src/neumann.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      114 2023-05-26 16:49:56.000000 neumann-1.0.7/src/neumann.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        8 2023-05-26 16:49:56.000000 neumann-1.0.7/src/neumann.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-26 16:49:56.654960 neumann-1.0.7/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1163 2023-05-26 16:49:50.000000 neumann-1.0.7/tests/test_approx.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4274 2023-05-26 16:49:50.000000 neumann-1.0.7/tests/test_function.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2146 2023-05-26 16:49:50.000000 neumann-1.0.7/tests/test_ga.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      570 2023-05-26 16:49:50.000000 neumann-1.0.7/tests/test_graph.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3669 2023-05-26 16:49:50.000000 neumann-1.0.7/tests/test_logical.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7591 2023-05-26 16:49:50.000000 neumann-1.0.7/tests/test_lpp.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      649 2023-05-26 16:49:50.000000 neumann-1.0.7/tests/test_numint.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3767 2023-05-26 16:49:50.000000 neumann-1.0.7/tests/test_utils.py
```

### Comparing `neumann-1.0.6/LICENSE` & `neumann-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/PKG-INFO` & `neumann-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neumann
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python Library for Applied Mathematics in Physical Sciences.
 Home-page: https://github.com/dewloosh/Neumann
-Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.6.zip
+Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.7.zip
 Author: Bence Balogh
 Author-email: dewloosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `neumann-1.0.6/README.md` & `neumann-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/approx/func.py` & `neumann-1.0.7/src/neumann/approx/func.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/approx/lagrange.py` & `neumann-1.0.7/src/neumann/approx/lagrange.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/approx/mls.py` & `neumann-1.0.7/src/neumann/approx/mls.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                 def bdyy(x):
                     return np.array([0, 0, 0])
 
                 def bdxy(x):
                     return np.array([0, 0, 0])
 
         else:
-            raise
+            raise NotImplementedError
     elif deg == 2:
         if dim == 1:
 
             def b(x):
                 return np.array([1, x, x**2])
 
             if grad:
@@ -180,17 +180,17 @@
                 def bdyy(x):
                     return np.array([0, 0, 0, 0, 2, 0])
 
                 def bdxy(x):
                     return np.array([0, 0, 0, 0, 0, 1])
 
         else:
-            raise
+            raise NotImplementedError
     else:
-        raise
+        raise NotImplementedError
 
     # moment matrix
     nData = points.shape[0]
     k = int(fact(deg + dim) / fact(deg) / fact(dim))
     A = np.zeros([k, k])
     B = np.zeros([k, nData])
     Adx, Ady, Bdx, Bdy = 4 * (None,)
```

### Comparing `neumann-1.0.6/src/neumann/arraysetops.py` & `neumann-1.0.7/src/neumann/arraysetops.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/decorate.py` & `neumann-1.0.7/src/neumann/decorate.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/function/constraint.py` & `neumann-1.0.7/src/neumann/function/constraint.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/function/function.py` & `neumann-1.0.7/src/neumann/function/function.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/function/functions.py` & `neumann-1.0.7/src/neumann/function/functions.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/function/metafunction.py` & `neumann-1.0.7/src/neumann/function/metafunction.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 
 
 class ABCMeta_MetaFunction(ABCMeta_Weak):
     """
     Metaclass for defining ABCs for algebraic structures.
     """
 
-    def __new__(metaclass, name, bases, namespace, *args, **kwargs):
-        cls = super().__new__(metaclass, name, bases, namespace, *args, **kwargs)
+    def __new__(metaclass, name, bases, namespace, /, **kwargs):
+        cls = super().__new__(metaclass, name, bases, namespace, **kwargs)
         if "value" in namespace:
             cls.f = namespace["value"]
 
         if "gradient" in namespace:
             cls.g = namespace["gradient"]
 
         if "Hessian" in namespace:
```

### Comparing `neumann-1.0.6/src/neumann/function/relation.py` & `neumann-1.0.7/src/neumann/function/relation.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/function/testfunction.py` & `neumann-1.0.7/src/neumann/function/testfunction.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/hist.py` & `neumann-1.0.7/src/neumann/hist.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/abstract.py` & `neumann-1.0.7/src/neumann/linalg/abstract.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import numbers
-
+from copy import deepcopy
 import numpy as np
 from numpy import array_repr, array_str
 
 from .meta import TensorLike
 from .exceptions import (
     LinalgInvalidTensorOperationError,
     TensorShapeMismatchError,
@@ -61,14 +61,48 @@
             self.array += other
         elif isinstance(other, TensorLike):
             if not self.array.shape == other.array.shape:
                 raise TensorShapeMismatchError
             self.array += other.show(self.frame)
         return self
 
+    def __add__(self, other) -> TensorLike:
+        if other.__class__ == self.__class__:
+            if not self.array.shape == other.array.shape:
+                raise TensorShapeMismatchError
+            cls = self.__class__
+            fcls = cls._frame_cls_
+            frame = fcls(deepcopy(self.frame.axes))
+            arr = self.array + other.show(self.frame)
+            return cls(arr, frame=frame)
+        else:
+            raise TypeError(
+                (
+                    "Tensor addition is only supported between instances "
+                    "of the same class."
+                )
+            )
+
+    def __sub__(self, other) -> TensorLike:
+        if other.__class__ == self.__class__:
+            if not self.array.shape == other.array.shape:
+                raise TensorShapeMismatchError
+            cls = self.__class__
+            fcls = cls._frame_cls_
+            frame = fcls(deepcopy(self.frame.axes))
+            arr = self.array - other.show(self.frame)
+            return cls(arr, frame=frame)
+        else:
+            raise TypeError(
+                (
+                    "Tensor subtraction is only supported between instances "
+                    "of the same class."
+                )
+            )
+
     def __isub__(self, other) -> TensorLike:
         if isinstance(other, numbers.Number):
             self.array += other
         elif isinstance(other, TensorLike):
             if not self.array.shape == other.array.shape:
                 raise TensorShapeMismatchError
             self.array -= other.show(self.frame)
@@ -101,15 +135,15 @@
         else:
             return HANDLED_FUNCTIONS[func](*args, **kwargs)
 
     def __array_ufunc__(self, ufunc, method, *inputs, **kwargs):
         if ufunc in HANDLED_UNIVERSAL_FUNCTIONS:
             return HANDLED_UNIVERSAL_FUNCTIONS[ufunc](method, *inputs, **kwargs)
         msg = """
-        NumPy universal functions are not supported by tensors. Try calling 
+        Not all NumPy universal functions are not supported by tensors. Try calling 
         this method using the arrays of the tensorial inputs.
         """
         raise LinalgInvalidTensorOperationError(msg)
 
 
 @implements(np.negative, ufunc=True)
 def negative_implementation(method, *args, **kwargs):
```

### Comparing `neumann-1.0.6/src/neumann/linalg/frame.py` & `neumann-1.0.7/src/neumann/linalg/frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,24 +11,26 @@
     is_orthonormal_frame,
     is_normal_frame,
     normalize_frame,
     Gram,
     dual_frame,
     transpose_axes,
     show_frame,
-    rotation_matrix
+    rotation_matrix,
 )
 from ..utils import repeat
 from .meta import FrameLike, TensorLike, ArrayWrapper
 
 
 __all__ = ["ReferenceFrame", "RectangularFrame", "CartesianFrame"]
 
 
-def inplace_binary(obj: FrameLike, other, bop: Callable, rtype: FrameLike = None) -> FrameLike:
+def inplace_binary(
+    obj: FrameLike, other, bop: Callable, rtype: FrameLike = None
+) -> FrameLike:
     """
     Performs a binary operation inplace. Components of registered tensorial entities
     are transformed accordingly and registered to the output frame.
     """
     axes = np.copy(obj.show())
     bop(axes, other, out=(axes,))
     if rtype:
@@ -167,26 +169,29 @@
                 elif isinstance(dim, int):
                     axes = np.eye(dim)
         except Exception as e:  # pragma: no cover
             raise e
         super().__init__(axes, *args)
         self._name = name
 
+    @property
     def is_rectangular(self):
         """
         Returns True if the frame is a rectangular one.
         """
         return is_rectangular_frame(self.axes)
 
+    @property
     def is_cartesian(self):
         """
         Returns True if the frame is a cartesian (orthonormal) one.
         """
         return is_orthonormal_frame(self.axes)
 
+    @property
     def is_independent(self) -> bool:
         """
         Returns True if the base vectors that make up the frame are linearly
         independent.
         """
         return np.linalg.det(self.Gram()) > 0
 
@@ -288,15 +293,14 @@
         If the target is None, the componants are returned in the ambient frame.
 
         Returns
         -------
         numpy.ndarray
         """
         return self.dcm(source=target)
-        #return show_frame(self.dcm(target=target), eye_like(self.axes))
 
     def dcm(
         self, *, target: "ReferenceFrame" = None, source: "ReferenceFrame" = None
     ) -> ndarray:
         """
         Returns the direction cosine matrix (DCM) of a transformation
         from a source (S) to a target (T) frame. The current frame can be
@@ -346,18 +350,40 @@
                     " source shape {} and target shape {}"
                 )
                 raise NotImplementedError(msg.format(S.shape, T.shape))
         # We only get here if the function is called without arguments.
         # The DCM from the ambient frame to the current frame is returned.
         return self.axes
 
+    def transpose(self, inplace: bool = False) -> "ReferenceFrame":
+        """
+        Either transposes the array of the frame, or returns a copy
+        of it with the components transposed.
+
+        Parameters
+        ----------
+        inplace: bool, Optional
+            If ``True``, the operation is performed on the instance the call
+            is made upon. Default is False.
+
+        Note
+        ----
+        The rule of transposition differs from the one implemented in NumPy, as
+        only tensorial axes are being transposed.
+        """
+        if inplace:
+            self.axes = transpose_axes(self.axes)
+            return self
+        else:
+            return self.__class__(transpose_axes(self.axes))
+
     def orient(self, *args, **kwargs) -> "ReferenceFrame":
         """
         Orients the current frame inplace. All arguments are forwarded
-        to :func:`~neumann.linalg.utils.rotation_matrix`, see there for the 
+        to :func:`~neumann.linalg.utils.rotation_matrix`, see there for the
         details.
 
         Returns
         -------
         ReferenceFrame
 
         Example
@@ -373,29 +399,29 @@
 
         See Also
         --------
         :func:`orient_new`
         :func:`~neumann.linalg.utils.rotation_matrix`
         """
         dcm = rotation_matrix(*args, **kwargs)
-        self._array = show_frame(dcm.T, self.axes)
+        self._array = show_frame(transpose_axes(dcm), self.axes)
         return self
 
     def orient_new(self, *args, name="", **kwargs) -> "ReferenceFrame":
         """
         Returns a new frame, oriented relative to the called object.
-        All extra positional and keyword arguments are forwarded to 
-        :func:`~neumann.linalg.utils.rotation_matrix`, see there for the 
+        All extra positional and keyword arguments are forwarded to
+        :func:`~neumann.linalg.utils.rotation_matrix`, see there for the
         details.
 
         Parameters
         ----------
         name: str
             Name for the new reference frame.
-        
+
         Returns
         -------
         ReferenceFrame
             A new ReferenceFrame object.
 
         See Also
         --------
@@ -604,27 +630,29 @@
 
     See also
     --------
     :class:`~neumann.linalg.ReferenceFrame`
     :class:`~neumann.linalg.CartesianFrame`
     """
 
-    def __init__(self, *args, assume_rectangular:bool=False, **kwargs):
+    def __init__(self, *args, assume_rectangular: bool = False, **kwargs):
         super().__init__(*args, **kwargs)
         if not assume_rectangular:
             assert is_rectangular_frame(
                 self.axes
             ), "This frame is not rectangular, check your input!"
 
+    @property
     def is_rectangular(self):
         """
         Returns True if the frame is a rectangular one.
         """
         return True
 
+    @property
     def is_independent(self) -> bool:
         """
         Returns True if the base vectors that make up the frame are linearly
         independent.
         """
         return True
 
@@ -684,30 +712,34 @@
 
     See also
     --------
     :class:`~neumann.linalg.ReferenceFrame`
     :class:`~neumann.linalg.RectangularFrame`
     """
 
-    def __init__(self, *args, normalize: bool = False, assume_cartesian:bool=False, **kwargs):
+    def __init__(
+        self, *args, normalize: bool = False, assume_cartesian: bool = False, **kwargs
+    ):
         super().__init__(*args, assume_rectangular=assume_cartesian, **kwargs)
         if normalize:
             self.axes = normalize_frame(self.axes)
         else:
             if not assume_cartesian:
                 assert is_normal_frame(
                     self.axes
                 ), "This frame is not cartesian, check your input!"
 
+    @property
     def is_rectangular(self):
         """
         Returns True if the frame is a rectangular one.
         """
         return True
 
+    @property
     def is_cartesian(self):
         """
         Returns True if the frame is a cartesian (orthonormal) one.
         """
         return True
 
     def Gram(self) -> ndarray:
```

### Comparing `neumann-1.0.6/src/neumann/linalg/frontal/frontal.py` & `neumann-1.0.7/src/neumann/linalg/frontal/frontal.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/frontal/frutils.py` & `neumann-1.0.7/src/neumann/linalg/frontal/frutils.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/frontal/path.py` & `neumann-1.0.7/src/neumann/linalg/frontal/path.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/frontal/postproc.py` & `neumann-1.0.7/src/neumann/linalg/frontal/postproc.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/frontal/proc.py` & `neumann-1.0.7/src/neumann/linalg/frontal/proc.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/frontal/topo.py` & `neumann-1.0.7/src/neumann/linalg/frontal/topo.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/meta.py` & `neumann-1.0.7/src/neumann/linalg/meta.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 from abc import abstractmethod
 import weakref
 from typing import Tuple, Union
 import numbers
+from functools import partial
+from copy import copy, deepcopy
 
 import numpy as np
 from numpy import array_repr, array_str, ndarray
 from numpy.lib.mixins import NDArrayOperatorsMixin
 
 from dewloosh.core import Wrapper
 from dewloosh.core.abc import ABC_Safe
@@ -139,27 +141,27 @@
 
     @property
     def minmax(self) -> Tuple[float]:
         """
         Returns the minimum and maximum values of the array.
         """
         return minmax(self._array)
-    
-    def chop(self, tol:float=1e-12) -> "ArrayWrapper":
+
+    def chop(self, tol: float = 1e-12) -> "ArrayWrapper":
         """
         Sets very small values (in an absolute sense) to zero.
 
         .. versionadded:: 1.0.5
-        
+
         Parameters
         ----------
         tol: float, Optional
             The values whose absolute value is less than this limit are
             set to zero. Default is 1e-12.
-        
+
         Returns
         -------
         ~`neumann.linalg.meta.ArrayWrapper`
             The object the call was made upon.
         """
         self._array[np.where(np.abs(self._array) < tol)] = 0.0
         return self
@@ -248,14 +250,25 @@
     def Gram(self) -> ndarray:
         ...
 
     @abstractmethod
     def dual(self) -> "FrameLike":
         ...
 
+    @abstractmethod
+    def transpose(self, inplace: bool = False) -> "FrameLike":
+        ...
+
+    @property
+    def T(self) -> "FrameLike":
+        """
+        Returns the transpose.
+        """
+        return self.transpose(inplace=False)
+
     def _register_tensorial_(self, v: "TensorLike"):
         """
         Registers tensorial objects by appending a weak reference to the set
         of weak references. Registered objects change their components upon
         changes of their supporting frame.
         """
         self._weakrefs[id(v)] = v
@@ -303,37 +316,60 @@
             if not (len(args) > 0 and isinstance(args[0], np.ndarray)):
                 raise LinalgMissingInputError(
                     "A frame or an array of components is required."
                 )
 
             arr = args[0]
             if bulk:
-                frame = self._frame_cls_(dim=arr.shape[1])
+                frame = self.__class__._frame_cls_(dim=arr.shape[1])
             else:
-                frame = self._frame_cls_(dim=arr.shape[0])
+                frame = self.__class__._frame_cls_(dim=arr.shape[0])
             cls_params["frame"] = frame
 
         kwargs["cls_params"] = cls_params
         super().__init__(*args, **kwargs)
 
         if self._array._frame is None:
-            self._array._frame = self._frame_cls_(dim=self._array.shape)
+            self._array._frame = self.__class__._frame_cls_(dim=self._array.shape)
 
         self.frame._register_tensorial_(self)
 
         self._bulk = bulk
 
         if rank is not None:
             if self.__class__._rank_ is not None:
                 raise ValueError("Rank is already defined on the class level.")
             else:
                 self._rank = rank
         else:
             self._rank = None
 
+    def __deepcopy__(self, memo):
+        return self.__copy__(memo)
+
+    def __copy__(self, memo=None):
+        cls = type(self)
+        copy_function = copy if (memo is None) else partial(deepcopy, memo=memo)
+        is_deep = memo is not None
+        frame_cls = cls._frame_cls_
+
+        f = self.frame
+        if is_deep:
+            ax = deepcopy(f.axes)
+            memo[id(f.axes)] = ax
+            frame = frame_cls(ax)
+        else:
+            frame = f
+
+        arr = copy_function(self.array)
+        if is_deep:
+            memo[id(self.array)] = arr
+
+        return cls(arr, frame=frame)
+
     @classmethod
     def _from_any_input(cls, *args, **kwargs) -> "TensorLike":
         raise NotImplementedError
 
     @classmethod
     def _verify_input(cls, arr: ndarray, *_, **kwargs) -> bool:
         raise NotImplementedError
@@ -399,17 +435,45 @@
         f._register_tensorial_(self)
 
     @property
     def T(self) -> "TensorLike":
         """
         Returns the transpose.
         """
-        f = self.frame
-        frame = f.__class__(np.copy(f.axes))
-        return self.__class__(self.array.T, frame=frame)
+        return self.transpose(inplace=False)
+
+    def transpose(self, inplace: bool = False) -> "TensorLike":
+        """
+        Either transposes the array of the tensor, or returns a copy
+        of it with the components transposed.
+
+        Parameters
+        ----------
+        inplace: bool, Optional
+            If ``True``, the operation is performed on the instance the call
+            is made upon. Default is False.
+
+        Note
+        ----
+        The rule of transposition differs from the one implemented in NumPy, as
+        only tensorial axes are being transposed.
+        """
+        r = self.rank
+        shape = self.array.shape
+        indices = tuple(range(len(shape)))
+        data_indices = indices[:-r]
+        tensor_indices = indices[len(shape) - r :]
+        indices = data_indices + tensor_indices[::-1]
+        if inplace:
+            self._array = np.transpose(self.array, indices)
+            return self
+        else:
+            f = self.frame
+            frame = f.__class__(np.copy(f.axes))
+            return self.__class__(np.transpose(self.array, indices), frame=frame)
 
     @abstractmethod
     def show(self) -> Array:
         ...
 
     @abstractmethod
     def orient(self) -> "TensorLike":
```

### Comparing `neumann-1.0.6/src/neumann/linalg/solve.py` & `neumann-1.0.7/src/neumann/linalg/solve.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/sparse/csr.py` & `neumann-1.0.7/src/neumann/linalg/sparse/csr.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/sparse/jaggedarray.py` & `neumann-1.0.7/src/neumann/linalg/sparse/jaggedarray.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/sparse/utils.py` & `neumann-1.0.7/src/neumann/linalg/sparse/utils.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/linalg/tensor.py` & `neumann-1.0.7/src/neumann/linalg/tensor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,35 +1,40 @@
-from typing import Iterable
 from copy import deepcopy as dcopy
 
 import numpy as np
 from numpy import ndarray
-import sympy as sy
 
 from dewloosh.core.tools.alphabet import latinrange
+
 from .frame import ReferenceFrame as Frame
 from .abstract import AbstractTensor
-from .top import tr_3333, tr_3333_jit
-from .utils import is_hermitian, _transform_tensors2_multi
-
-
-__all__ = ["Tensor", "Tensor2", "Tensor4", "Tensor2x3", "Tensor4x3"]
+from .tr import _tr_tensors2, _tr_tensors4x3
+from .exceptions import TensorShapeMismatchError
+from .utils import is_hermitian, transpose_axes
+
+__all__ = [
+    "Tensor",
+    "Tensor2",
+    "Tensor4",
+    "Tensor2x3",
+    "Tensor4x3",
+]
 
 
 class Tensor(AbstractTensor):
     """
     A class to handle tensors.
 
     Parameters
     ----------
-    args : tuple, Optional
+    args: tuple, Optional
         Positional arguments forwarded to `numpy.ndarray`.
-    frame : numpy.ndarray, Optional
+    frame: numpy.ndarray, Optional
         The reference frame the vector is represented by its coordinates.
-    kwargs : dict, Optional
+    kwargs: dict, Optional
         Keyword arguments forwarded to `numpy.ndarray`.
 
     Examples
     --------
     Import the necessary classes:
 
     >>> from neumann.linalg import Tensor, ReferenceFrame
@@ -107,28 +112,28 @@
         Returns the components in a target frame. If the target is
         `None`, the components are returned in the ambient frame.
 
         The transformation can also be specified with a proper DCM matrix.
 
         Parameters
         ----------
-        target : numpy.ndarray, Optional
+        target: numpy.ndarray, Optional
             Target frame.
-        dcm : numpy.ndarray, Optional
+        dcm: numpy.ndarray, Optional
             The DCM matrix of the transformation.
 
         Returns
         -------
         numpy.ndarray
             The components of the tensor in a specified frame, or
             the ambient frame, depending on the arguments.
         """
         if not isinstance(dcm, ndarray):
             if target is None:
-                target = Frame(dim=self._array.shape[-1])
+                target = Frame(dim=self.frame.axes.shape[-1])
             dcm = self.frame.dcm(target=target)
         return self.transform_components(dcm)
 
     def orient(self, *args, **kwargs) -> "Tensor":
         """
         Orients the vector inplace. All arguments are forwarded to
         `orient_new`.
@@ -138,17 +143,17 @@
         Vector
             The same vector the function is called upon.
 
         See Also
         --------
         :func:`orient_new`
         """
-        fcls = self.__class__._frame_cls_
-        dcm = fcls.eye(dim=len(self)).orient_new(*args, **kwargs).dcm()
-        self.array = self.transform_components(dcm.T)
+        fcls: Frame = self.__class__._frame_cls_
+        dcm = fcls.eye(dim=self.frame.shape[-1]).orient_new(*args, **kwargs).dcm()
+        self.array = self.transform_components(transpose_axes(dcm))
         return self
 
     def orient_new(self, *args, **kwargs) -> "Tensor":
         """
         Returns a transformed version of the instance.
 
         Returns
@@ -156,16 +161,16 @@
         Vector
             A new vector.
 
         See Also
         --------
         :func:`orient`
         """
-        fcls = self.__class__._frame_cls_
-        dcm = fcls.eye(dim=len(self)).orient_new(*args, **kwargs).dcm()
+        fcls: Frame = self.__class__._frame_cls_
+        dcm = fcls.eye(dim=self.frame.shape[-1]).orient_new(*args, **kwargs).dcm()
         array = self.transform_components(dcm.T)
         return self.__class__(array, frame=self.frame)
 
     def copy(self, deep: bool = False, name: str = None) -> "Tensor":
         """
         Returns a shallow or deep copy of this object, depending of the
         argument `deepcopy` (default is False).
@@ -180,208 +185,132 @@
         Returns a deep copy of the frame.
         """
         return self.copy(deep=True, name=name)
 
 
 class Tensor2(Tensor):
     """
-    A class to handle 2nd-order tensors. Some operations have dedicated implementations
-    that provide higher performence utilizing implicit parallelization. Examples include
-    the metric tensor, or the stress and strain tensors of elasticity.
+    A class to handle second-order tensors. Some operations have dedicated implementations
+    that provide higher performence utilizing implicit parallelization. Examples
+    for tensors of this class include the metric tensor, or the stress and strain tensors
+    of elasticity.
+
+    See also
+    --------
+    :class:"~neumann.linalg.tensor.Tensor2x3"
     """
 
     _rank_ = 2
 
     @classmethod
     def _verify_input(cls, arr: ndarray, *_, bulk: bool = False, **kwargs) -> bool:
         if bulk:
-            return len(arr.shape) == 3 and is_hermitian(arr[0])
+            return len(arr.shape) == 3 and arr.shape[-1] == arr.shape[-2]
         else:
-            return len(arr.shape) == 2 and is_hermitian(arr)
+            return len(arr.shape) == 2 and arr.shape[-1] == arr.shape[-2]
 
     def transform_components(self, Q: ndarray) -> ndarray:
-        if len(Q.shape) == 3 and len(self.array.shape) == 3:
-            return _transform_tensors2_multi(self.array, Q)
-        else:
-            return Q @ self.array @ Q.T
+        return _tr_tensors2(self.array, Q)
 
 
 class Tensor2x3(Tensor2):
-    ...
-
-
-class Tensor4(Tensor):
     """
-    A class to handle 4th-order tensors. Some operations have dedicated implementations
-    that provide higher performence utilizing implicit parallelization. Examples include
-    the piezo-optical tensor, the elasto-optical tensor, the flexoelectric tensor or the
-    elasticity tensor.
+    Dedicated class for second-order tensors, with 3 indices per axis.
+    Since the shape of the tensor is known, instances are able to automatically detect
+    if the provided components resemble a single item or a collection.
     """
 
-    _rank_ = 4
+    def __init__(self, *args, **kwargs):
+        if len(args) > 0 and isinstance(args[0], ndarray):
+            arr = args[0]
+            shape = arr.shape
+            if shape[-2:] == (3, 3):
+                if len(shape) >= 3:
+                    is_bulk = kwargs.get("bulk", True)
+                    if not is_bulk:
+                        raise ValueError("Incorrect input!")
+                    kwargs["bulk"] = is_bulk
+                else:
+                    if not len(shape) == 2:
+                        raise TensorShapeMismatchError("Invalid shape!")
+                    is_bulk = kwargs.get("bulk", False)
+                    if is_bulk:
+                        raise ValueError("Incorrect input!")
+            else:
+                raise TensorShapeMismatchError("Invalid shape!")
+
+        super().__init__(*args, **kwargs)
 
     @classmethod
     def _verify_input(cls, arr: ndarray, *_, bulk: bool = False, **kwargs) -> bool:
         if bulk:
-            return len(arr.shape) == 5 and is_hermitian(arr[0])
+            return len(arr.shape) >= 3 and arr.shape[-2:] == (3, 3)
         else:
-            return len(arr.shape) == 4 and is_hermitian(arr)
+            return len(arr.shape) == 2 and arr.shape[-2:] == (3, 3)
 
 
-class Tensor4x3(Tensor):
+class Tensor4(Tensor):
     """
-    A class for fourth-order tensors, where each index ranges from 1 to 3.
+    A class to handle fourth-order tensors. Some operations have dedicated implementations
+    that provide higher performence utilizing implicit parallelization. Examples of this class
+    include the piezo-optical tensor, the elasto-optical tensor, the flexoelectric tensor or the
+    elasticity tensor.
 
-    Parameters
-    ----------
-    imap : dict, Optional
-        An invertible index map for second-order tensors that assigns to each pair
-        of indices a single index. The index map used to switch between 4d and 2d
-        representation is inferred from this input. The default is the Voigt indicial map:
-            0 : (0, 0)
-            1 : (1, 1)
-            2 : (2, 2)
-            3 : (1, 2)
-            4 : (0, 2)
-            5 : (0, 1)
-    symbolic : bool, Optional
-        If True, the tensor is stored in symbolic form, and the components are stored as
-        a `SymPy` matrix. Default is False.
+    See also
+    --------
+    :class:"~neumann.linalg.tensor.Tensor4x3"
     """
 
-    __imap__ = {0: (0, 0), 1: (1, 1), 2: (2, 2), 3: (1, 2), 4: (0, 2), 5: (0, 1)}
-
-    def __init__(self, *args, symbolic: bool = False, imap: dict = None, **kwargs):
-        super().__init__(*args, **kwargs)
-
-        if isinstance(imap, dict):
-            self.__imap__ = imap
+    _rank_ = 4
 
-        if symbolic:
-            self.transform_components = self._transform_sym_
-            self.dtype = object
-
-    @property
-    def collapsed(self):
-        if self._array is not None:
-            return self._array.shape[-1] == 6
+    @classmethod
+    def _verify_input(cls, arr: ndarray, *_, bulk: bool = False, **kwargs) -> bool:
+        shape = arr.shape
+        is_hermitian = (shape[-1],) * 4 == shape[-4:]
+        if bulk:
+            return len(shape) == 5 and is_hermitian
         else:
-            raise ValueError("There is no data.")
+            return len(shape) == 4 and is_hermitian
 
-    def expand(self) -> "Tensor4x3":
+    def transform_components(self, dcm: ndarray) -> ndarray:
         """
-        Changes the representation of the tensor to 4d.
+        Returns the components of the transformed numerical tensor, based on
+        the provided direction cosine matrix.
         """
-        if not self.collapsed:
-            return self
-        T = np.zeros((3, 3, 3, 3), dtype=self._array.dtype)
-        m = self._array
-        imap = self.imap()
-        for ij, ijkl in imap.items():
-            T[ijkl] = m[ij]
-        self._array = T
-        return self
+        return _tr_tensors4x3(self._array, dcm)
 
-    def collapse(self) -> "Tensor4x3":
-        """
-        Changes the representation of the tensor to 2d.
-        """
-        if self.collapsed:
-            return self
-        m = np.zeros((6, 6), dtype=self._array.dtype)
-        T = self._array
-        imap = self.imap()
-        for ij, ijkl in imap.items():
-            m[ij] = T[ijkl]
-        self._array = m
-        return self
 
-    @classmethod
-    def imap(cls, imap1d: dict = None) -> dict:
-        """
-        Returns a 2d-to-4d index map used to collapse or expand a tensor,
-        based on the 1d-to-2d mapping of the class the function is called on,
-        or on the first argument, if it is a suitable candidate for an
-        index map.
-        """
-        if imap1d is None:
-            imap1d = cls.__imap__
-        indices = np.indices((6, 6))
-        it = np.nditer([*indices], ["multi_index"])
-        imap2d = dict()
-        for _ in it:
-            i, j = it.multi_index
-            imap2d[(i, j)] = imap1d[i] + imap1d[j]
-        return imap2d
+class Tensor4x3(Tensor4):
+    """
+    Dedicated class for fourth order tensors, with 3 indices per axis.
+    Since the shape of the tensor is known, instances are able to automatically detect
+    if the provided components resemble a single item or a collection.
+    """
 
-    @classmethod
-    def symbolic(
-        cls, *args, base: str = "C_", as_matrix: bool = False, imap: dict = None
-    ) -> Iterable:
-        """
-        Returns a symbolic representation of a 4th order 3x3x3x3 tensor.
-        If the argument 'as_matrix' is True, the function returns a 6x6 matrix,
-        that unfolds according to the argument 'imap', or if it's not provided,
-        the index map of the class the function is called on. If 'imap' is
-        provided, it must be a dictionary including exactly 6 keys and
-        values. The keys must be integers in the integer range (0, 6), the
-        values must be tuples on the integer range (0, 3).
-        The default mapping is the Voigt indicial map:
-            0 : (0, 0)
-            1 : (1, 1)
-            2 : (2, 2)
-            3 : (1, 2)
-            4 : (0, 2)
-            5 : (0, 1)
-        """
-        res = np.zeros((3, 3, 3, 3), dtype=object)
-        indices = np.indices((3, 3, 3, 3))
-        it = np.nditer([*indices], ["multi_index"])
-        for _ in it:
-            p, q, r, s = it.multi_index
-            if q >= p and s >= r:
-                sinds = np.array([p, q, r, s], dtype=np.int16) + 1
-                sym = sy.symbols(base + "_".join(sinds.astype(str)))
-                res[p, q, r, s] = sym
-                res[q, p, r, s] = sym
-                res[p, q, s, r] = sym
-                res[q, p, s, r] = sym
-                res[r, s, p, q] = sym
-                res[r, s, q, p] = sym
-                res[s, r, p, q] = sym
-                res[s, r, q, p] = sym
-        if as_matrix:
-            mat = np.zeros((6, 6), dtype=object)
-            imap = cls.imap(imap) if imap is None else imap
-            for ij, ijkl in imap.items():
-                mat[ij] = res[ijkl]
-            if "sympy" in args:
-                res = sy.Matrix(mat)
+    def __init__(self, *args, **kwargs):
+        if len(args) > 0 and isinstance(args[0], ndarray):
+            arr = args[0]
+            shape = arr.shape
+            if shape[-4:] == (3, 3, 3, 3):
+                if len(shape) >= 5:
+                    is_bulk = kwargs.get("bulk", True)
+                    if not is_bulk:
+                        raise ValueError("Incorrect input!")
+                    kwargs["bulk"] = is_bulk
+                else:
+                    if not len(shape) == 4:
+                        raise TensorShapeMismatchError("Invalid shape!")
+                    is_bulk = kwargs.get("bulk", False)
+                    if is_bulk:
+                        raise ValueError("Incorrect input!")
             else:
-                res = mat
-        return res
+                raise TensorShapeMismatchError("Invalid shape!")
 
-    def transform_components(self, dcm: np.ndarray) -> ndarray:
-        """
-        Returns the components of the transformed numerical tensor, based on
-        the provided direction cosine matrix.
-        """
-        if self.collapsed:
-            self.expand()
-            array = tr_3333_jit(self._array, dcm)
-            self.collapse()
-        else:
-            array = tr_3333_jit(self._array, dcm)
-        return array
+        super().__init__(*args, **kwargs)
 
-    def _transform_sym_(self, dcm: np.ndarray) -> ndarray:
-        """
-        Returns the components of the transformed symbolic tensor, based on
-        the provided direction cosine matrix.
-        """
-        if self.collapsed:
-            self.expand()
-            array = tr_3333(self._array, dcm, dtype=object)
-            self.collapse()
+    @classmethod
+    def _verify_input(cls, arr: ndarray, *_, bulk: bool = False, **kwargs) -> bool:
+        is_hermitian = arr.shape[-4:] == (3, 3, 3, 3)
+        if bulk:
+            return len(arr.shape) >= 5 and is_hermitian
         else:
-            array = tr_3333(self._array, dcm, dtype=object)
-        return array
+            return len(arr.shape) == 4 and is_hermitian
```

### Comparing `neumann-1.0.6/src/neumann/linalg/utils.py` & `neumann-1.0.7/src/neumann/linalg/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,22 +49,20 @@
     "norm",
     "norm2d",
     "linspace",
     "linspace1d",
     "inv",
     "show_vector",
     "show_frame",
-    "rotation_matrix"
+    "rotation_matrix",
 ]
 
 
 def rotation_matrix(
-    rot_type: str,
-    amounts: Iterable,
-    rot_order: Union[str, int] = ''
+    rot_type: str, amounts: Iterable, rot_order: Union[str, int] = ""
 ) -> ndarray:
     """
     Returns a rotation matrix using the mechanism provided by
     `sympy.physics.vector.ReferenceFrame.orientnew`.
 
     Parameters
     ----------
@@ -76,27 +74,27 @@
         - ``'DCM'``: for setting the direction cosine matrix directly
         - ``'Body'``: three successive rotations about new intermediate
             axes, also called "Euler and Tait-Bryan angles"
         - ``'Space'``: three successive rotations about the parent
             frames' unit vectors
         - ``'Quaternion'``: rotations defined by four parameters which
             result in a singularity free direction cosine matrix
-            
+
     amounts: Iterable
         Expressions defining the rotation angles or direction cosine
         matrix. These must match the ``rot_type``. See examples below for
         details. The input types are:
 
         - ``'Axis'``: 2-tuple (expr/sym/func, Vector)
         - ``'DCM'``: Matrix, shape(3, 3)
         - ``'Body'``: 3-tuple of expressions, symbols, or functions
         - ``'Space'``: 3-tuple of expressions, symbols, or functions
         - ``'Quaternion'``: 4-tuple of expressions, symbols, or
             functions
-            
+
     rot_order: str or int, Optional
         If applicable, the order of the successive of rotations. The string
         ``'123'`` and integer ``123`` are equivalent, for example. Required
         for ``'Body'`` and ``'Space'``.
 
     Returns
     -------
@@ -482,16 +480,16 @@
 
     Returns
     -------
     numpy.ndarray
         The new coordinates of the frame with the same shape as `arr`.
     """
     res = np.zeros_like(arr)
-    for i in prange(arr.shape[-1]): 
-        res[i, :] = dcm @ arr[i, :] 
+    for i in prange(arr.shape[-1]):
+        res[i, :] = dcm @ arr[i, :]
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def _show_frames(dcm: ndarray, arr: ndarray) -> ndarray:
     """
     Returns the coordinates of multiple frames in a target frame specified
@@ -507,15 +505,15 @@
     Returns
     -------
     numpy.ndarray
         The new coordinates of the frames with the same shape as `arr`.
     """
     res = np.zeros_like(arr)
     for i in prange(arr.shape[0]):
-        for j in prange(arr.shape[-1]): 
+        for j in prange(arr.shape[-1]):
             res[i, j, :] = dcm @ arr[i, j, :]
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def _show_frames_multi(dcm: ndarray, arr: ndarray) -> ndarray:
     """
@@ -531,35 +529,41 @@
     Returns
     -------
     numpy.ndarray
         The new coordinates of the frames with the same shape as `arr`.
     """
     res = np.zeros_like(arr)
     for i in prange(arr.shape[0]):
-        for j in prange(arr.shape[-1]): 
+        for j in prange(arr.shape[-1]):
             res[i, j, :] = dcm[i] @ arr[i, j, :]
     return res
 
 
 @njit(nogil=True, parallel=True, cache=__cache)
 def _transpose_multi(dcm: ndarray) -> ndarray:
     N = dcm.shape[0]
     res = np.zeros_like(dcm)
     for i in prange(N):
-        res[i] = dcm[i].T
+        res[i, :, :] = dcm[i].T
     return res
 
 
-def transpose_axes(a: ndarray, axes=None) -> ndarray:
-    if len(a.shape) == 2:
-        return a.T
-    elif len(a.shape) == 3:
-        return _transpose_multi(a)
+def transpose_axes(arr: ndarray) -> ndarray:
+    if len(arr.shape) == 2:
+        return arr.T
+    elif len(arr.shape) == 3:
+        # FIXME this might be unnecessary
+        return _transpose_multi(arr)
     else:
-        return np.transpose(a, axes)
+        shape = arr.shape
+        indices = tuple(range(len(shape)))
+        data_indices = indices[:-2]
+        tensor_indices = indices[len(shape) - 2 :]
+        indices = data_indices + tensor_indices[::-1]
+        return np.transpose(arr, indices)
 
 
 def is_rectangular_frame(axes: ndarray) -> bool:
     """
     Returns True if a frame is Cartesian.
 
     Parameters
@@ -636,15 +640,15 @@
     Returns the Gram matrix of a frame.
 
     Parameters
     ----------
     axes: numpy.ndarray
         A matrix where the i-th row is the i-th basis vector.
     """
-    return axes @ axes.T
+    return axes @ transpose_axes(axes)
 
 
 def dual_frame(axes: ndarray) -> ndarray:
     """
     Returns the dual frame of the input.
 
     Parameters
@@ -946,16 +950,7 @@
 @njit(nogil=True, parallel=True, cache=__cache)
 def linspace1d(start, stop, N) -> ndarray:
     res = np.zeros(N)
     di = (stop - start) / (N - 1)
     for i in prange(N):
         res[i] = start + i * di
     return res
-
-
-@njit(nogil=True, parallel=True, cache=__cache)
-def _transform_tensors2_multi(arr: ndarray, Q: ndarray):
-    nE = arr.shape[0]
-    res = np.zeros_like(arr)
-    for iE in prange(nE):
-        res[iE, :, :] = Q[iE] @ arr[iE] @ Q[iE].T
-    return res
```

### Comparing `neumann-1.0.6/src/neumann/linalg/vector.py` & `neumann-1.0.7/src/neumann/linalg/vector.py`

 * *Files 0% similar despite different names*

```diff
@@ -152,25 +152,25 @@
         See Also
         --------
         :func:`orient_new`
         """
         if not isinstance(dcm, ndarray):
             fcls = self.__class__._frame_cls_
             dcm = fcls.eye(dim=len(self)).orient_new(*args, **kwargs).dcm()
-            #self.array = dcm.T @ self._array
+            # self.array = dcm.T @ self._array
             self.array = show_vector(dcm.T, self.array)
-            #self.array = np.linalg.inv(dcm) @ self._array
+            # self.array = np.linalg.inv(dcm) @ self._array
             # FIXME check this
         else:
             self.array = show_vector(dcm.T, self.array)
-            #self.array = dcm.T @ self._array
+            # self.array = dcm.T @ self._array
             # FIXME check if inversion is necessary here
             # inversion might be necessary here because it is uncertain if the
             # dcm matrix was fabricated properly.
-            #self.array = np.linalg.inv(dcm) @ self._array
+            # self.array = np.linalg.inv(dcm) @ self._array
         return self
 
     def orient_new(self, *args, **kwargs) -> "Vector":
         """
         Returns a transformed version of the instance.
 
         Returns
@@ -182,15 +182,15 @@
         --------
         :func:`orient`
         """
         fcls = self.__class__._frame_cls_
         dcm = fcls.eye(dim=len(self)).orient_new(*args, **kwargs).dcm()
         array = dcm.T @ self._array
         # FIXME check if inversion is necessary or not
-        #array = np.linalg.inv(dcm) @ self._array
+        # array = np.linalg.inv(dcm) @ self._array
         return Vector(array, frame=self.frame)
 
     def copy(self, deep: bool = False, name: str = None) -> "Vector":
         """
         Returns a shallow or deep copy of this object, depending of the
         argument `deepcopy` (default is False).
         """
```

### Comparing `neumann-1.0.6/src/neumann/logical.py` & `neumann-1.0.7/src/neumann/logical.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/numint.py` & `neumann-1.0.7/src/neumann/numint.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/optimize/ga.py` & `neumann-1.0.7/src/neumann/optimize/ga.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/optimize/lp.py` & `neumann-1.0.7/src/neumann/optimize/lp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import numpy as np
 from numpy import ndarray
 from numpy.linalg import LinAlgError
 import sympy as sy
 from sympy.utilities.iterables import multiset_permutations
 from copy import copy, deepcopy
+from contextlib import suppress
 
 try:
     from collections.abc import Iterable
 except ImportError:  # pragma: no cover
     from collections import Iterable
 from collections import defaultdict
 from typing import Tuple
@@ -500,46 +501,47 @@
         """
         m, n = A.shape
         r = n - m
         assert r > 0
 
         stop = False
         try:
-            if order is not None:
-                if isinstance(order, Iterable):
-                    permutations = iter([order])
-            else:
-                order = [i for i in range(n)]
-                permutations = multiset_permutations(order)
-            while not stop:
-                order = next(permutations)
-                A_ = A[:, order]
-                B_ = A_[:, :m]
-                try:
-                    B_inv = np.linalg.inv(B_)
-                    xB = np.matmul(B_inv, b)
-                    stop = all(xB >= 0)
-                except LinAlgError:
-                    """
-                    If there is no error, it means that calculation
-                    of xB was succesful, which is only possible if the
-                    current permutation defines a positive definite submatrix.
-                    Note that this is cheaper than checking the eigenvalues,
-                    since it only requires the eigenvalues to be all positive,
-                    and does not involve calculating their actual values.
-                    """
-                    pass
-        except StopIteration:
-            """
-            There is no permutation of columns that would produce a regular
-            mxm submatrix
-                -> there is no feasible basic solution
-                    -> there is no feasible solution
-            """
-            pass
+            with suppress(StopIteration):
+                """
+                StopIteration:
+
+                There is no permutation of columns that would produce a regular
+                mxm submatrix
+                    -> there is no feasible basic solution
+                        -> there is no feasible solution
+                """
+                if order is not None:
+                    if isinstance(order, Iterable):
+                        permutations = iter([order])
+                else:
+                    order = [i for i in range(n)]
+                    permutations = multiset_permutations(order)
+                while not stop:
+                    order = next(permutations)
+                    A_ = A[:, order]
+                    B_ = A_[:, :m]
+                    with suppress(LinAlgError):
+                        B_inv = np.linalg.inv(B_)
+                        xB = np.matmul(B_inv, b)
+                        stop = all(xB >= 0)
+                        """
+                        LinAlgError:
+                        
+                        If there is no error, it means that calculation
+                        of xB was succesful, which is only possible if the
+                        current permutation defines a positive definite submatrix.
+                        Note that this is cheaper than checking the eigenvalues,
+                        since it only requires the eigenvalues to be all positive,
+                        and does not involve calculating their actual values.
+                        """
         finally:
             if stop:
                 N_ = A_[:, m:]
                 xN = np.zeros(r, dtype=float)
                 return B_, B_inv, N_, xB, xN, order
             else:
                 return None
```

### Comparing `neumann-1.0.6/src/neumann/topology/graph.py` & `neumann-1.0.7/src/neumann/topology/graph.py`

 * *Files identical despite different names*

### Comparing `neumann-1.0.6/src/neumann/utils.py` & `neumann-1.0.7/src/neumann/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -276,17 +276,17 @@
 @njit(nogil=True, parallel=True, cache=__cache)
 def repeat(a: ndarray, N: int = 1) -> ndarray:
     """
     Repeats an array N-times.
 
     Parameters
     ----------
-    a : numpy.ndarray
+    a: numpy.ndarray
         Input array.
-    N : int, Optional
+    N: int, Optional
         Number of repetitions. Default is 1.
 
     Returns
     -------
     numpy.ndarray
         A NumPy array with shape (N, a.shape[0], a.shape[1]).
```

### Comparing `neumann-1.0.6/src/neumann.egg-info/PKG-INFO` & `neumann-1.0.7/src/neumann.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: neumann
-Version: 1.0.6
+Version: 1.0.7
 Summary: A Python Library for Applied Mathematics in Physical Sciences.
 Home-page: https://github.com/dewloosh/Neumann
-Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.6.zip
+Download-URL: https://github.com/dewloosh/Neumann/archive/refs/tags/1.0.7.zip
 Author: Bence Balogh
 Author-email: dewloosh@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `neumann-1.0.6/src/neumann.egg-info/SOURCES.txt` & `neumann-1.0.7/src/neumann.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -28,18 +28,20 @@
 src/neumann/function/metafunction.py
 src/neumann/function/relation.py
 src/neumann/function/testfunction.py
 src/neumann/linalg/__init__.py
 src/neumann/linalg/abstract.py
 src/neumann/linalg/exceptions.py
 src/neumann/linalg/frame.py
+src/neumann/linalg/imap.py
 src/neumann/linalg/meta.py
 src/neumann/linalg/solve.py
 src/neumann/linalg/tensor.py
-src/neumann/linalg/top.py
+src/neumann/linalg/testing.py
+src/neumann/linalg/tr.py
 src/neumann/linalg/utils.py
 src/neumann/linalg/vector.py
 src/neumann/linalg/frontal/__init__.py
 src/neumann/linalg/frontal/frontal.py
 src/neumann/linalg/frontal/frutils.py
 src/neumann/linalg/frontal/path.py
 src/neumann/linalg/frontal/postproc.py
@@ -55,12 +57,11 @@
 src/neumann/optimize/lp.py
 src/neumann/topology/__init__.py
 src/neumann/topology/graph.py
 tests/test_approx.py
 tests/test_function.py
 tests/test_ga.py
 tests/test_graph.py
-tests/test_linalg.py
 tests/test_logical.py
 tests/test_lpp.py
 tests/test_numint.py
 tests/test_utils.py
```

### Comparing `neumann-1.0.6/tests/test_approx.py` & `neumann-1.0.7/tests/test_approx.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,35 +3,33 @@
 import numpy as np
 import sympy as sy
 
 from neumann.approx.lagrange import gen_Lagrange_1d, approx_Lagrange_1d
 
 
 class TestLagrange(unittest.TestCase):
-
     def test_1d(self):
         gen_Lagrange_1d(x=[-1, 0, 1])
         gen_Lagrange_1d(i=[1, 2], sym=True)
         gen_Lagrange_1d(i=[1, 2], sym=False, lambdify=True)
         gen_Lagrange_1d(i=[1, 2, 3], sym=False)
         gen_Lagrange_1d(N=3)
         approx_Lagrange_1d([-1, 1], [0, 10], lambdify=True)
         approx_Lagrange_1d([-1, 1], [0, 10], lambdify=False)
-        
+
     def test_approx_Lagrange_1d(self):
         source, target = [-1, 1], [0, 10]
         approx = approx_Lagrange_1d(source, target, lambdify=True)
         for s, t in zip(source, target):
             self.assertTrue(np.isclose(approx(s), t))
-            
-        L = sy.symbols('L', real=True, positive=True)
+
+        L = sy.symbols("L", real=True, positive=True)
         source, target = [-1, 1], [0, L]
         approx = approx_Lagrange_1d(source, target)
-        v = float(approx.subs([('x', -1), (L, 10)]))
+        v = float(approx.subs([("x", -1), (L, 10)]))
         self.assertTrue(np.isclose(v, 0))
-        v = float(approx.subs([('x', 1), (L, 10)]))
+        v = float(approx.subs([("x", 1), (L, 10)]))
         self.assertTrue(np.isclose(v, 10))
 
 
 if __name__ == "__main__":
-
     unittest.main()
```

### Comparing `neumann-1.0.6/tests/test_function.py` & `neumann-1.0.7/tests/test_function.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,118 +14,128 @@
 def load_tests(loader, tests, ignore):  # pragma: no cover
     tests.addTests(doctest.DocTestSuite(fnc.function))
     tests.addTests(doctest.DocTestSuite(fnc.relation))
     return tests
 
 
 class TestFunction(unittest.TestCase):
-    
     def assertFailsProperly(self, exc, fnc, *args, **kwargs):
         failed_properly = False
         try:
             fnc(*args, **kwargs)
         except exc:
             failed_properly = True
         finally:
             self.assertTrue(failed_properly)
-        
+
     def test_bulk(self):
-        def f0(x, y): return x**2 + y  # pragma: no cover
-        def f1(x, y): return np.array([2*x, 1])  # pragma: no cover
-        
+        def f0(x, y):
+            return x**2 + y  # pragma: no cover
+
+        def f1(x, y):
+            return np.array([2 * x, 1])  # pragma: no cover
+
         f = Function(f0, f1, d=2)
         self.assertFalse(f.symbolic)
-        #f.to_latex()
+        # f.to_latex()
         f.coefficients()
         f.linear_coefficients()
-        
+
         Function(value=f0, gradient=f1, Hessian=None, d=2)
-        
+
         class MyFunction(Function):  # pragma: no cover
-            def value(x, y): return f0(x, y)
-            def gradient(x, y): return f1(x, y)
-            def Hessian(x, y): ...
-            
+            def value(x, y):
+                return f0(x, y)
+
+            def gradient(x, y):
+                return f1(x, y)
+
+            def Hessian(x, y):
+                ...
+
         f = Function()
         self.assertFailsProperly(TypeError, f, [0, 0])
-        self.assertFailsProperly(TypeError, lambda x : x.to_latex(), f)
-        self.assertFailsProperly(TypeError, lambda x : x.subs([0, 0]), f)
+        self.assertFailsProperly(TypeError, lambda x: x.to_latex(), f)
+        self.assertFailsProperly(TypeError, lambda x: x.subs([0, 0]), f)
         self.assertFailsProperly(TypeError, f.g, [0, 0])
         self.assertFailsProperly(TypeError, f.G, [0, 0])
-        
+
         str_expr = "x*y + y**2 + 6*b + 2"
         decode(str_expr=str_expr)
         self.assertFailsProperly(Exception, decode, expr=[])
-        
-        g = Function('3*x + 4*y - 2', variables=['x', 'y', 'z'])
-        g.subs([0, 0, 0], ['x', 'y', 'z'], inplace=True)
-        
+
+        g = Function("3*x + 4*y - 2", variables=["x", "y", "z"])
+        g.subs([0, 0, 0], ["x", "y", "z"], inplace=True)
+
         coefficients(g.expr)
-        substitute(g.expr, [0,0])
-            
+        substitute(g.expr, [0, 0])
+
     def test_linearity(self):
-        def f0(x=None, y=None): return x**2 + y  # pragma: no cover
-        def f1(x=None, y=None): return np.array([2*x, 1])  # pragma: no cover
-        
+        def f0(x=None, y=None):
+            return x**2 + y  # pragma: no cover
+
+        def f1(x=None, y=None):
+            return np.array([2 * x, 1])  # pragma: no cover
+
         f = Function(f0, f1, d=2)
         self.assertFalse(f.symbolic)
         self.assertTrue(f.linear)
-        
+
     def test_sym(self):
         f = gen_Lagrange_1d(N=2)
         f1 = Function(f[1][0], f[1][1], f[1][2])
         f2 = Function(f[2][0], f[2][1], f[2][2])
-        assert (f1.linear and f2.linear)
+        assert f1.linear and f2.linear
         assert f1.dimension == 1
         assert f2.dimension == 1
         assert np.isclose(f1([-1]), 1.0)
         assert np.isclose(f1([1]), 0.0)
         assert np.isclose(f2([-1]), 0.0)
         assert np.isclose(f2([1]), 1.0)
         f1.coefficients()
         f1.linear_coefficients()
         f1.to_latex()
         f1.f([-1]), f1.g([-1]), f1.G([-1])
         f1.subs([1], variables=f1.variables)
 
 
 class TestRelations(unittest.TestCase):
-
     def test_Relation(self):
-        variables = ['x1', 'x2', 'x3', 'x4'] 
-        x1, _, x3, x4 = syms = sy.symbols(variables, positive=True) 
-        r = Relation(x1 + 2*x3 + x4 - 4, variables=syms)
+        variables = ["x1", "x2", "x3", "x4"]
+        x1, _, x3, x4 = syms = sy.symbols(variables, positive=True)
+        r = Relation(x1 + 2 * x3 + x4 - 4, variables=syms)
         r.operator
-        r = Relation(x1 + 2*x3 + x4 - 4, variables=syms, op=lambda x, y: x <= y)  # pragma: no cover
-    
+        r = Relation(
+            x1 + 2 * x3 + x4 - 4, variables=syms, op=lambda x, y: x <= y
+        )  # pragma: no cover
+
     def test_Equality(self):
-        variables = ['x1', 'x2', 'x3', 'x4'] 
-        x1, _, x3, x4 = syms = sy.symbols(variables, positive=True) 
-        eq1 = Equality(x1 + 2*x3 + x4 - 4, variables=syms)
-        eq1.to_eq() 
+        variables = ["x1", "x2", "x3", "x4"]
+        x1, _, x3, x4 = syms = sy.symbols(variables, positive=True)
+        eq1 = Equality(x1 + 2 * x3 + x4 - 4, variables=syms)
+        eq1.to_eq()
         eq1.operator
-    
+
     def test_InEquality(self):
-        gt = InEquality('x + y', op='>')
+        gt = InEquality("x + y", op=">")
         assert not gt.relate([0.0, 0.0])
 
-        ge = InEquality('x + y', op='>=')
+        ge = InEquality("x + y", op=">=")
         assert ge.relate([0.0, 0.0])
 
-        le = InEquality('x + y', op=lambda x, y: x <= y)
+        le = InEquality("x + y", op=lambda x, y: x <= y)
         assert le.relate([0.0, 0.0])
 
-        lt = InEquality('x + y', op=lambda x, y: x < y)
+        lt = InEquality("x + y", op=lambda x, y: x < y)
         assert not lt.relate([0.0, 0.0])
-        
+
         failed_properly = False
         try:
-            InEquality('x + y')
+            InEquality("x + y")
         except ValueError:
             failed_properly = True
         finally:
             self.assertTrue(failed_properly)
 
 
 if __name__ == "__main__":
-
     unittest.main()
```

### Comparing `neumann-1.0.6/tests/test_ga.py` & `neumann-1.0.7/tests/test_ga.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,71 +7,74 @@
 
 def load_tests(loader, tests, ignore):  # pragma: no cover
     tests.addTests(doctest.DocTestSuite(optimize.ga))
     return tests
 
 
 def Rosenbrock(a, b, x, y):
-    return (a-x)**2 + b*(y-x**2)**2
+    return (a - x) ** 2 + b * (y - x**2) ** 2
 
 
 class TestBGA(unittest.TestCase):
-
     def test_BGA(self):
         def f(x):
             return Rosenbrock(1, 100, x[0], x[1])
+
         f.dimension = 2
         ranges = [[-10, 10], [-10, 10]]
-        BGA = BinaryGeneticAlgorithm(f, ranges, length=12, nPop=200)        
+        BGA = BinaryGeneticAlgorithm(f, ranges, length=12, nPop=200)
         BGA.evolver()
         BGA.evolve()
         BGA.genotypes = BGA.genotypes
         BGA.fittness()
         BGA.fittness(BGA.phenotypes)
         BGA.best_phenotype(lastknown=False)
         BGA.best_phenotype(lastknown=True)
         BGA.random_parents_generator(BGA.genotypes)
         BGA.reset()
-        
+
     def test_BGA_elitism_eq_1(self):
         def f(x):
             return Rosenbrock(1, 100, x[0], x[1])
+
         f.dimension = 2
         ranges = [[-10, 10], [-10, 10]]
-        BGA = BinaryGeneticAlgorithm(f, ranges, length=6, nPop=100, elitism=1)        
+        BGA = BinaryGeneticAlgorithm(f, ranges, length=6, nPop=100, elitism=1)
         BGA.evolve()
         BGA.divide()
-    
+
     def test_BGA_elitism_gt_1(self):
         def f(x):
             return Rosenbrock(1, 100, x[0], x[1])
+
         f.dimension = 2
         ranges = [[-10, 10], [-10, 10]]
-        BGA = BinaryGeneticAlgorithm(f, ranges, length=6, nPop=100, elitism=2)        
+        BGA = BinaryGeneticAlgorithm(f, ranges, length=6, nPop=100, elitism=2)
         BGA.evolve()
         BGA.divide()
-        
+
     def test_BGA_elitism_lt_1(self):
         def f(x):
             return Rosenbrock(1, 100, x[0], x[1])
+
         f.dimension = 2
         ranges = [[-10, 10], [-10, 10]]
-        BGA = BinaryGeneticAlgorithm(f, ranges, length=6, nPop=100, elitism=0.5)        
+        BGA = BinaryGeneticAlgorithm(f, ranges, length=6, nPop=100, elitism=0.5)
         BGA.evolve()
         BGA.divide()
-    
+
     def test_Rosenbrock(self):
         def f(x):
             return Rosenbrock(1, 100, x[0], x[1])
+
         f.dimension = 2
         ranges = [[-10, 10], [-10, 10]]
         BGA = BinaryGeneticAlgorithm(f, ranges, length=12, nPop=200)
         BGA.solve()
-        
+
         BGA.genotypes = BGA.genotypes
         BGA.evolver()
         BGA.evolve()
-        
-        
+
+
 if __name__ == "__main__":
-        
-    unittest.main()
+    unittest.main()
```

### Comparing `neumann-1.0.6/tests/test_graph.py` & `neumann-1.0.7/tests/test_graph.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import unittest
 from neumann.topology import Graph
 import networkx as nx
 
 
 class TestGraph(unittest.TestCase):
-
     def test_Graph(self):
         grid = nx.grid_2d_graph(5, 5)  # 5x5 grid
         G = Graph(grid)
         G.adjacency_matrix()
         G.pseudo_peripheral_nodes()
         G.rooted_level_structure()
-        
+
         seed = 13648  # Seed random number generators for reproducibility
         G = Graph(nx.random_k_out_graph(10, 3, 0.5, seed=seed))
         G.pseudo_peripheral_nodes()
         G.rooted_level_structure()
 
 
 if __name__ == "__main__":
```

### Comparing `neumann-1.0.6/tests/test_logical.py` & `neumann-1.0.7/tests/test_logical.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 import unittest
 import doctest
 
 import neumann.logical as logical
-from neumann.logical import (isclose, allclose, 
-                             isintarray, is1dintarray,
-                             isfloatarray, is1dfloatarray,
-                             isboolarray,
-                             issymmetric, is_none_or_false)
+from neumann.logical import (
+    isclose,
+    allclose,
+    isintarray,
+    is1dintarray,
+    isfloatarray,
+    is1dfloatarray,
+    isboolarray,
+    issymmetric,
+    is_none_or_false,
+)
 from neumann.linalg.utils import random_posdef_matrix
 import numpy as np
 
 
 def load_tests(loader, tests, ignore):  # pragma: no cover
     tests.addTests(doctest.DocTestSuite(logical))
     return tests
 
 
 class TestLogical(unittest.TestCase):
-    
     def test_istype(self):
         # 0d
         self.assertTrue(is_none_or_false(False))
         self.assertTrue(is_none_or_false(None))
         self.assertFalse(is_none_or_false(True))
-        self.assertFalse(is_none_or_false('a'))
+        self.assertFalse(is_none_or_false("a"))
         # 1d
         arr = np.zeros(2, dtype=int)
         self.assertTrue(isintarray(arr))
         self.assertTrue(is1dintarray(arr))
         self.assertTrue(not isfloatarray(arr))
         self.assertTrue(not isboolarray(arr))
         self.assertTrue(not is1dfloatarray(arr))
@@ -58,32 +63,33 @@
         self.assertTrue(not isboolarray(arr))
         arr = arr.astype(bool)
         self.assertTrue(not isintarray(arr))
         self.assertTrue(not is1dintarray(arr))
         self.assertTrue(not isfloatarray(arr))
         self.assertTrue(not is1dfloatarray(arr))
         self.assertTrue(isboolarray(arr))
-        
+
     def test_issymmetric(self):
         self.assertTrue(issymmetric(random_posdef_matrix(2)))
         a = np.zeros((2, 2))
         a[0, 0] = 1.0
         self.assertTrue(issymmetric(a))
         a[0, 1] = 1.0
         self.assertFalse(issymmetric(a))
         a[1, 0] = 1.0
         self.assertTrue(issymmetric(a))
-        
+
     def test_isclose(self):
         def assertAssert(fnc, *args, **kwargs):
             try:
                 fnc(*args, **kwargs)
                 self.assertTrue(False)
             except AssertionError as e:
                 pass
+
         # 0d
         self.assertTrue(isclose(0, 0))
         self.assertTrue(not isclose(0, 1))
         self.assertTrue(not isclose(1, 0))
         # 1d
         x1 = np.zeros(10, dtype=float)
         x2 = x1 + 0.01
@@ -96,13 +102,11 @@
         self.assertTrue(allclose(x1, x1))
         self.assertTrue(not allclose(x1, x2))
         self.assertTrue(not allclose(x2, x1))
         # purposeful assertion errors
         assertAssert(isclose, 0, 0, atol=None, rtol=None)
         assertAssert(isclose, 0, 0, atol=-1)
         assertAssert(isclose, 0, 0, rtol=-1)
-        
 
 
 if __name__ == "__main__":
-
-    unittest.main()
+    unittest.main()
```

### Comparing `neumann-1.0.6/tests/test_lpp.py` & `neumann-1.0.7/tests/test_lpp.py`

 * *Files 21% similar despite different names*

```diff
@@ -10,175 +10,173 @@
 from neumann import optimize
 
 
 def load_tests(loader, tests, ignore):  # pragma: no cover
     tests.addTests(doctest.DocTestSuite(optimize.lp))
     return tests
 
-       
+
 class TestLPP(unittest.TestCase):
-    
     def assertFailsProperly(self, exc, fnc, *args, **kwargs):
         failed_properly = False
         try:
             fnc(*args, **kwargs)
         except exc:
             failed_properly = True
         finally:
             self.assertTrue(failed_properly)
-    
+
     def test_coverage(self):
         P = LPP.example_unique()
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
-        P.add_constraint(InEquality(x1 - 1, op='>=', variables=syms))
-        P.add_constraint(x1 - 1, op='>=', variables=syms)
+        P.add_constraint(InEquality(x1 - 1, op=">=", variables=syms))
+        P.add_constraint(x1 - 1, op=">=", variables=syms)
         P.simplify(inplace=True)
-        
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
         f = Function(x1 + x2, variables=syms)
-        ieq1 = InEquality(x1 - 1, op='>=', variables=syms)
-        ieq2 = InEquality(x2 - 1, op='>=', variables=syms)
-        ieq3 = InEquality(x1 + x2 - 4, op='<=', variables=syms)
+        ieq1 = InEquality(x1 - 1, op=">=", variables=syms)
+        ieq2 = InEquality(x2 - 1, op=">=", variables=syms)
+        ieq3 = InEquality(x1 + x2 - 4, op="<=", variables=syms)
         lpp = LPP(cost=f, constraints=[ieq1, ieq2, ieq3], variables=syms)
         lpp.feasible([0, 0])
-        
+
     def test_lpp_create(self):
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
         f = Function(x1 + x2, variables=syms)
-        ieq1 = InEquality(x1 - 1, op='>=', variables=syms)
-        ieq2 = InEquality(x2 - 1, op='>=', variables=syms)
-        ieq3 = InEquality(x1 + x2 - 4, op='<=', variables=syms)
+        ieq1 = InEquality(x1 - 1, op=">=", variables=syms)
+        ieq2 = InEquality(x2 - 1, op=">=", variables=syms)
+        ieq3 = InEquality(x1 + x2 - 4, op="<=", variables=syms)
         lpp = LPP(f, variables=syms)
         lpp.add_constraint(ieq1)
         lpp.add_constraint(ieq2)
         lpp.add_constraint(ieq3)
         lpp.simplify(inplace=True)
-       
+
     def test_unique_solution(self):
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
         f = Function(x1 + x2, variables=syms)
-        ieq1 = InEquality(x1 - 1, op='>=', variables=syms)
-        ieq2 = InEquality(x2 - 1, op='>=', variables=syms)
-        ieq3 = InEquality(x1 + x2 - 4, op='<=', variables=syms)
+        ieq1 = InEquality(x1 - 1, op=">=", variables=syms)
+        ieq2 = InEquality(x2 - 1, op=">=", variables=syms)
+        ieq3 = InEquality(x1 + x2 - 4, op="<=", variables=syms)
         lpp = LPP(cost=f, constraints=[ieq1, ieq2, ieq3], variables=syms)
-        x = lpp.solve()['x']
+        x = lpp.solve()["x"]
         _x = np.array([1.0, 1.0])
         self.assertTrue(np.all(np.isclose(_x, x)))
         self.assertTrue(lpp.feasible(x))
-            
+
     def test_degenerate_solution(self):
-        variables = ['x1', 'x2', 'x3', 'x4']
+        variables = ["x1", "x2", "x3", "x4"]
         x1, x2, x3, x4 = syms = sy.symbols(variables, positive=True)
-        obj2 = Function(3*x1 + x2 - 6*x3 + x4, variables=syms)
-        eq21 = Equality(x1 + 2*x3 + x4, variables=syms)
+        obj2 = Function(3 * x1 + x2 - 6 * x3 + x4, variables=syms)
+        eq21 = Equality(x1 + 2 * x3 + x4, variables=syms)
         eq22 = Equality(x2 + x3 - x4 - 2, variables=syms)
         P2 = LPP(cost=obj2, constraints=[eq21, eq22], variables=syms)
         P2.solve(raise_errors=False)
-            
+
     def test_no_solution(self):
         """
         Example for no solution.
         """
-        variables = ['x1', 'x2', 'x3', 'x4']
+        variables = ["x1", "x2", "x3", "x4"]
         x1, x2, x3, x4 = syms = sy.symbols(variables, positive=True)
-        obj3 = Function(-3*x1 + x2 + 9*x3 + x4, variables=syms)
-        eq31 = Equality(x1 - 2*x3 - x4 + 2, variables=syms)
+        obj3 = Function(-3 * x1 + x2 + 9 * x3 + x4, variables=syms)
+        eq31 = Equality(x1 - 2 * x3 - x4 + 2, variables=syms)
         eq32 = Equality(x2 + x3 - x4 - 2, variables=syms)
         P3 = LPP(cost=obj3, constraints=[eq31, eq32], variables=syms)
         self.assertFailsProperly(NoSolutionError, P3.solve, raise_errors=True)
-        
+
     def test_multiple_solution(self):
         """
         Example for multiple solutions.
         (0, 1, 1, 0)
         (0, 4, 0, 2)
         """
-        variables = ['x1', 'x2', 'x3', 'x4']
+        variables = ["x1", "x2", "x3", "x4"]
         x1, x2, x3, x4 = syms = sy.symbols(variables, positive=True)
-        obj4 = Function(3*x1 + 2*x2 + 8*x3 + x4, variables=syms)
-        eq41 = Equality(x1 - 2*x3 - x4 + 2, variables=syms)
+        obj4 = Function(3 * x1 + 2 * x2 + 8 * x3 + x4, variables=syms)
+        eq41 = Equality(x1 - 2 * x3 - x4 + 2, variables=syms)
         eq42 = Equality(x2 + x3 - x4 - 2, variables=syms)
         P4 = LPP(cost=obj4, constraints=[eq41, eq42], variables=syms)
-        x = P4.solve(return_all=True, raise_errors=True)['x']
+        x = P4.solve(return_all=True, raise_errors=True)["x"]
         assert len(x.shape) == 2
         assert x.shape[0] == 2
-        x = P4.solve(return_all=False, raise_errors=True)['x']
+        x = P4.solve(return_all=False, raise_errors=True)["x"]
         assert len(x.shape) == 1
-        
+
     def test_maximize_solution(self):
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
         f = Function(-x1 - x2, variables=syms)
-        ieq1 = InEquality(x1 - 1, op='>=', variables=syms)
-        ieq2 = InEquality(x2 - 1, op='>=', variables=syms)
-        ieq3 = InEquality(x1 + x2 - 4, op='<=', variables=syms)
+        ieq1 = InEquality(x1 - 1, op=">=", variables=syms)
+        ieq2 = InEquality(x2 - 1, op=">=", variables=syms)
+        ieq3 = InEquality(x1 + x2 - 4, op="<=", variables=syms)
         lpp = LPP(cost=f, constraints=[ieq1, ieq2, ieq3], variables=syms)
-        x = atleast2d(lpp.maximize()['x'])
+        x = atleast2d(lpp.maximize()["x"])
         _x = np.array([1.0, 1.0])
         assert np.all(np.isclose(_x, x))
-    
+
     def test_standardform(self):
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
         f = Function(-x1 - x2, variables=syms)
-        ieq1 = InEquality(x1 - 1, op='>=', variables=syms)
-        ieq2 = InEquality(x2 - 1, op='>=', variables=syms)
-        ieq3 = InEquality(x1 + x2 - 4, op='<=', variables=syms)
+        ieq1 = InEquality(x1 - 1, op=">=", variables=syms)
+        ieq2 = InEquality(x2 - 1, op=">=", variables=syms)
+        ieq3 = InEquality(x1 + x2 - 4, op="<=", variables=syms)
         lpp = LPP(cost=f, constraints=[ieq1, ieq2, ieq3], variables=syms)
         lpp.to_numpy()
-        
+
     def test_feasible(self):
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
         f = Function(-x1 - x2, variables=syms)
-        ieq1 = InEquality(x1 - 1, op='>=', variables=syms)
-        ieq2 = InEquality(x2 - 1, op='>=', variables=syms)
-        ieq3 = InEquality(x1 + x2 - 4, op='<=', variables=syms)
+        ieq1 = InEquality(x1 - 1, op=">=", variables=syms)
+        ieq2 = InEquality(x2 - 1, op=">=", variables=syms)
+        ieq3 = InEquality(x1 + x2 - 4, op="<=", variables=syms)
         lpp = LPP(cost=f, constraints=[ieq1, ieq2, ieq3], variables=syms)
         self.assertTrue(lpp.feasible([1, 1]))
         self.assertFalse(lpp.feasible([0, 1]))
         self.assertFalse(lpp.feasible([1, 0]))
-    
+
     def test_1(self):
-        variables = ['x1', 'x2']
+        variables = ["x1", "x2"]
         x1, x2 = syms = sy.symbols(variables, positive=True)
         f = Function(x1 + x2, variables=syms)
         eq = Equality(x1 - 2, variables=syms)
         lpp = LPP(cost=f, constraints=[eq], variables=syms)
-        x = lpp.solve(return_all=True, raise_errors=True)['x']
-        assert np.all(np.isclose(x, np.array([2., 0.])))
-        variables = ['x1', 'x2']
+        x = lpp.solve(return_all=True, raise_errors=True)["x"]
+        assert np.all(np.isclose(x, np.array([2.0, 0.0])))
+        variables = ["x1", "x2"]
         x1, x2 = syms = sy.symbols(variables, positive=True)
         f = Function(x1 + x2, variables=syms)
         eq = Equality(x2 - 2, variables=syms)
         lpp = LPP(cost=f, constraints=[eq], variables=syms)
-        x = lpp.solve(return_all=True, raise_errors=True)['x']
-        assert np.all(np.isclose(x, np.array([0., 2.])))
-        
+        x = lpp.solve(return_all=True, raise_errors=True)["x"]
+        assert np.all(np.isclose(x, np.array([0.0, 2.0])))
+
     def test_2(self):
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
         f = Function(x1 + x2, variables=syms)
-        ieq1 = InEquality(x1 - 1, op='>=', variables=syms)
-        ieq2 = InEquality(x2 - 1, op='>=', variables=syms)
-        ieq3 = InEquality(x1 + x2 - 4, op='<=', variables=syms)
+        ieq1 = InEquality(x1 - 1, op=">=", variables=syms)
+        ieq2 = InEquality(x2 - 1, op=">=", variables=syms)
+        ieq3 = InEquality(x1 + x2 - 4, op="<=", variables=syms)
         lpp = LPP(cost=f, constraints=[ieq1, ieq2, ieq3], variables=syms)
-        x = lpp.solve(return_all=True, raise_errors=True)['x']
-        assert np.all(np.isclose(x, np.array([1., 1.])))
-        x1, x2 = sy.symbols(['x1', 'x2'], positive=True)
+        x = lpp.solve(return_all=True, raise_errors=True)["x"]
+        assert np.all(np.isclose(x, np.array([1.0, 1.0])))
+        x1, x2 = sy.symbols(["x1", "x2"], positive=True)
         syms = [x1, x2]
         f = Function(x1 + x2, variables=syms)
-        ieq1 = InEquality(x1 - 1, op='>=', variables=syms)
-        ieq2 = InEquality(x2 - 1, op='>=', variables=syms)
-        ieq3 = InEquality(x1 + x2 - 4, op='>=', variables=syms)
+        ieq1 = InEquality(x1 - 1, op=">=", variables=syms)
+        ieq2 = InEquality(x2 - 1, op=">=", variables=syms)
+        ieq3 = InEquality(x1 + x2 - 4, op=">=", variables=syms)
         lpp = LPP(cost=f, constraints=[ieq1, ieq2, ieq3], variables=syms)
-        e = lpp.solve(return_all=True, raise_errors=True, as_dict=True)['e']
+        e = lpp.solve(return_all=True, raise_errors=True, as_dict=True)["e"]
         assert len(e) == 0
-    
-    
+
+
 if __name__ == "__main__":
-        
-    unittest.main()
+    unittest.main()
```

### Comparing `neumann-1.0.6/tests/test_numint.py` & `neumann-1.0.7/tests/test_numint.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,25 +7,23 @@
 
 def load_tests(loader, tests, ignore):  # pragma: no cover
     tests.addTests(doctest.DocTestSuite(numint))
     return tests
 
 
 class TestGaussNumInt(unittest.TestCase):
-
     def test_gauss_numint(self):
         gauss_points(2)
         gauss_points(2, 2)
         gauss_points(2, 2, 2)
-        
+
         failed_properly = False
         try:
             gauss_points(2, 2, 2, 2)
         except NotImplementedError:
             failed_properly = True
         finally:
             self.assertTrue(failed_properly)
-            
-            
-if __name__ == "__main__":
 
-    unittest.main()
+
+if __name__ == "__main__":
+    unittest.main()
```

### Comparing `neumann-1.0.6/tests/test_utils.py` & `neumann-1.0.7/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,101 +16,98 @@
     tests.addTests(doctest.DocTestSuite(neumann.decorate))
     tests.addTests(doctest.DocTestSuite(arraysetops))
     tests.addTests(doctest.DocTestSuite(neumann.utils))
     return tests
 
 
 class TestUtils(unittest.TestCase):
-    
     def test_arraysetops(self):
         arr = np.array([[1, 2, 3], [1, 2, 4]], dtype=int)
         arraysetops.unique2d(arr)
         arraysetops.unique2d(arr, return_index=True)
         arraysetops.unique2d(arr, return_inverse=True)
         arraysetops.unique2d(arr, return_counts=True)
-        
+
         arr = ak.Array([[1, 2], [1, 2, 3]])
         arraysetops.unique2d(arr)
         arraysetops.unique2d(arr, return_index=True)
         arraysetops.unique2d(arr, return_inverse=True)
         arraysetops.unique2d(arr, return_counts=True)
-                
+
         data = np.array([1, 2, 1, 2, 3])
         arr = JaggedArray(data, cuts=[2, 3])
         arraysetops.unique2d(arr)
         arraysetops.unique2d(arr, return_index=True)
         arraysetops.unique2d(arr, return_inverse=True)
         arraysetops.unique2d(arr, return_counts=True)
-        
+
         data = np.array([1, 2, 1, 2, 3, 5])
         arr = JaggedArray(data, cuts=[3, 3], force_numpy=True)
         arraysetops.unique2d(arr)
-        
+
         failed_properly = False
         try:
-            arraysetops.unique2d('aaa')
+            arraysetops.unique2d("aaa")
         except TypeError:
             failed_properly = True
         finally:
             self.assertTrue(failed_properly)
-        
+
     def test_decorators(self):
-        
         @squeeze(default=True)
-        def foo(arr) -> np.ndarray:
+        def foo1(arr) -> np.ndarray:
             return arr
-        
-        self.assertTrue(len(foo(np.array([[1, 2]])).shape), 1)
-        self.assertTrue(len(foo(np.array([[1, 2]]), squeeze=False).shape), 2)
-        
+
+        self.assertTrue(len(foo1(np.array([[1, 2]])).shape), 1)
+        self.assertTrue(len(foo1(np.array([[1, 2]]), squeeze=False).shape), 2)
+
         @squeeze(default=True)
-        def foo(arr) -> np.ndarray:
+        def foo2(arr) -> np.ndarray:
             return arr, arr
-        
+
         arr = np.array([[1, 2]])
-        foo(arr)
-        foo(arr, squeeze=False)
-        
+        foo2(arr)
+        foo2(arr, squeeze=False)
+
         @squeeze(default=True)
-        def foo(arr) -> np.ndarray:
-            return {'1' : arr, '2' : arr}
-        
-        foo(arr)
-        foo(arr, squeeze=False)
-        
+        def foo3(arr) -> np.ndarray:
+            return {"1": arr, "2": arr}
+
+        foo3(arr)
+        foo3(arr, squeeze=False)
+
     def test_utils(self):
         self.assertEqual(nu.itype_of_ftype(np.float32), np.int32)
         self.assertEqual(nu.itype_of_ftype(np.float64), np.int64)
-        
+
         nu.atleastnd(1, 2, front=True)
-        nu.atleastnd(1, 2, back=True) 
+        nu.atleastnd(1, 2, back=True)
         nu.atleast1d(1)
         nu.atleast2d(1)
         nu.atleast3d(1)
-        nu.atleast4d(1) 
+        nu.atleast4d(1)
         nu.matrixform(1)
-        nu.flatten2d(np.eye(3), order='C')
-        nu.flatten2d(np.eye(3), order='F')
+        nu.flatten2d(np.eye(3), order="C")
+        nu.flatten2d(np.eye(3), order="F")
         nu.bool_to_float([True, False])
         nu.choice([False, True], (2, 2), [0.2, 0.8])
         nu.choice([False, True], (2, 2))
-        nu.indices_of_equal_rows(np.eye(3), np.eye(3)) 
+        nu.indices_of_equal_rows(np.eye(3), np.eye(3))
         nu.indices_of_equal_rows(np.eye(3, dtype=int), np.eye(3, dtype=int))
         arr = np.array([[1, 2, 3], [4, 5, 6]])
         nu.indices_of_equal_rows(arr, arr)
         arr = np.array([[1, 2, 3], [4, 5, 6]], dtype=float)
         nu.indices_of_equal_rows(arr, arr)
         x = np.array([[1, 2, 3], [4, 5, 6]])
         y = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]])
         nu.indices_of_equal_rows(x, y)
         x = np.array([[1, 2, 3], [4, 5, 6]], dtype=float)
         y = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9]], dtype=float)
         nu.indices_of_equal_rows(x, y)
         nu.to_range_1d([0.3, 0.5], source=[0, 1], target=[-1, 1])
-        
-        histogram([1, 2, 1], bins=[0, 1, 2, 3])   
-        histogram([1, 2, 1], bins=[0, 1, 2, 3], return_edges=True)           
-        
-        
+
+        histogram([1, 2, 1], bins=[0, 1, 2, 3])
+        histogram([1, 2, 1], bins=[0, 1, 2, 3], return_edges=True)
+
+
 if __name__ == "__main__":
-            
     unittest.main()
```

