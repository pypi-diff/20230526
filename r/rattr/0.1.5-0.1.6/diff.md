# Comparing `tmp/rattr-0.1.5.tar.gz` & `tmp/rattr-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rattr-0.1.5.tar", last modified: Wed May 24 13:49:36 2023, max compression
+gzip compressed data, was "rattr-0.1.6.tar", last modified: Fri May 26 08:32:07 2023, max compression
```

## Comparing `rattr-0.1.5.tar` & `rattr-0.1.6.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.581004 rattr-0.1.5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.565003 rattr-0.1.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.569003 rattr-0.1.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-24 13:49:14.000000 rattr-0.1.5/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-24 13:49:14.000000 rattr-0.1.5/.github/workflows/staticanalysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-24 13:49:14.000000 rattr-0.1.5/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-24 13:49:14.000000 rattr-0.1.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-24 13:49:14.000000 rattr-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-24 13:49:14.000000 rattr-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-24 13:49:36.581004 rattr-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-24 13:49:14.000000 rattr-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.569003 rattr-0.1.5/rattr/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/analyser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/cls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/analyser/context/
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20909 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/context/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/context/symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/context/symbol_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/file.py
--rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/function.py
--rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/ir_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/results.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    33184 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/analyser/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)    22526 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/toml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/cli/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/config/
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/config/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/error/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/error/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/error/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/rattr/plugins/analysers/
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/analysers/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/analysers/collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/rattr/plugins/assertors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/assertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-24 13:49:14.000000 rattr-0.1.5/rattr/plugins/assertors/import_clobbering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.573003 rattr-0.1.5/rattr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1980 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 13:49:36.000000 rattr-0.1.5/rattr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 13:49:14.000000 rattr-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-24 13:49:36.581004 rattr-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-24 13:49:14.000000 rattr-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20806 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/tests/context/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/context/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28992 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/context/test_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/context/test_symbol.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/context/test_symbol_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.577004 rattr-0.1.5/tests/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.581004 rattr-0.1.5/tests/plugins/analysers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/analysers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/analysers/test_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/analysers/test_collections.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.581004 rattr-0.1.5/tests/plugins/assertors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/assertors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/plugins/assertors/test_import_clobbering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:36.581004 rattr-0.1.5/tests/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/snippets/not_a_py.file
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/snippets/rattr_full_one.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/snippets/rattr_results_one.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/snippets/rattr_results_two.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_analysers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_bin.py
--rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_function.py
--rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_ir_dag.py
--rw-r--r--   0 runner    (1001) docker     (123)     8456 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_rattr.py
--rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_regressions.py
--rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_results.py
--rw-r--r--   0 runner    (1001) docker     (123)    43225 2023-05-24 13:49:14.000000 rattr-0.1.5/tests/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.718930 rattr-0.1.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.722930 rattr-0.1.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-26 08:31:47.000000 rattr-0.1.6/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-26 08:31:47.000000 rattr-0.1.6/.github/workflows/staticanalysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-05-26 08:31:47.000000 rattr-0.1.6/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-26 08:31:47.000000 rattr-0.1.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-26 08:31:47.000000 rattr-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 08:31:47.000000 rattr-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-26 08:32:07.730930 rattr-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13848 2023-05-26 08:31:47.000000 rattr-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.722930 rattr-0.1.6/rattr/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5703 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6930 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/cls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/analyser/context/
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20909 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/context/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5084 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/context/symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/context/symbol_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17963 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10901 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/ir_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33184 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/analyser/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23959 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2467 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/toml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/cli/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/config/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/error/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/error/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/error/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/plugins/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/analysers/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/analysers/collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.726930 rattr-0.1.6/rattr/plugins/assertors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/assertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4740 2023-05-26 08:31:47.000000 rattr-0.1.6/rattr/plugins/assertors/import_clobbering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.722930 rattr-0.1.6/rattr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14789 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2005 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 08:32:07.000000 rattr-0.1.6/rattr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 08:31:47.000000 rattr-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-26 08:32:07.730930 rattr-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-26 08:31:47.000000 rattr-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21080 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/context/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/context/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28992 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/context/test_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6744 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/context/test_symbol.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/context/test_symbol_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/data/config_1.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/plugins/analysers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/analysers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4795 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/analysers/test_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/analysers/test_collections.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/plugins/assertors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/assertors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15049 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/plugins/assertors/test_import_clobbering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 08:32:07.730930 rattr-0.1.6/tests/snippets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/snippets/not_a_py.file
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/snippets/rattr_full_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/snippets/rattr_results_one.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/snippets/rattr_results_two.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_analysers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_bin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13583 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5299 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23253 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17199 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_ir_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9440 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4311 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_rattr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14967 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_regressions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43225 2023-05-26 08:31:47.000000 rattr-0.1.6/tests/test_util.py
```

### Comparing `rattr-0.1.5/.github/workflows/publish.yml` & `rattr-0.1.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/.github/workflows/staticanalysis.yml` & `rattr-0.1.6/.github/workflows/staticanalysis.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/.github/workflows/tests.yml` & `rattr-0.1.6/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/.gitignore` & `rattr-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/LICENSE` & `rattr-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/PKG-INFO` & `rattr-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Rattr rats on your attrs.
 Home-page: https://github.com/SuadeLabs/ratter
 Author: Suade Labs
 License: MIT
 Keywords: automation linting type-checking attributes rats
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rattr-0.1.5/README.md` & `rattr-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/__main__.py` & `rattr-0.1.6/rattr/__main__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/annotations.py` & `rattr-0.1.6/rattr/analyser/annotations.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/base.py` & `rattr-0.1.6/rattr/analyser/base.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/cls.py` & `rattr-0.1.6/rattr/analyser/cls.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/context/context.py` & `rattr-0.1.6/rattr/analyser/context/context.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/context/symbol.py` & `rattr-0.1.6/rattr/analyser/context/symbol.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/context/symbol_table.py` & `rattr-0.1.6/rattr/analyser/context/symbol_table.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/file.py` & `rattr-0.1.6/rattr/analyser/file.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/function.py` & `rattr-0.1.6/rattr/analyser/function.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/ir_dag.py` & `rattr-0.1.6/rattr/analyser/ir_dag.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/results.py` & `rattr-0.1.6/rattr/analyser/results.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/types.py` & `rattr-0.1.6/rattr/analyser/types.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/analyser/util.py` & `rattr-0.1.6/rattr/analyser/util.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/cli/argparse.py` & `rattr-0.1.6/rattr/cli/argparse.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/cli/parser.py` & `rattr-0.1.6/rattr/cli/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from abc import ABC, abstractstaticmethod
 from argparse import ArgumentError, Namespace, RawTextHelpFormatter
 from os.path import isfile, splitext
+from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple
 
 from tomli import TOMLDecodeError
 
 from rattr import _version, error
 from rattr.cli.argparse import _ArgumentParser as ArgumentParser
 from rattr.cli.toml_parser import find_project_toml, load_cfg_from_project_toml
@@ -54,14 +55,30 @@
                     )
                     raise ArgumentError(None, message)
             except KeyError:
                 pass
     return toml_cfg
 
 
+def get_toml_override(
+    cli_parser: ArgumentParser,
+    sys_args: Optional[List[str]] = None,
+) -> Optional[Path]:
+    """Return the toml config override from the CLI if given, otherwise `None`."""
+    # Parse a throwaway copy of the cli arguments to see if the user specified a toml
+    # override, if he did and it is an extant file we ought to return it.
+    cli_arguments = cli_parser.parse_args(namespace=Namespace(), args=sys_args)
+    config: Optional[Path] = cli_arguments.config
+
+    if config is not None and not config.is_file():
+        return None
+
+    return config
+
+
 def parse_arguments(
     sys_args: Optional[List[str]] = None,
     project_toml_cfg: Optional[Dict[str, Any]] = None,
     exit_on_error: bool = True,
 ) -> Namespace:
     """Return the parsed and validated CLI arguments.
 
@@ -77,15 +94,14 @@
     If there is invalidity within the arguments, then the method should raise
     and `argparse.ArgumentError` with an appropriate message.
 
     On error the program usage and the error message will be shown before
     exiting.
 
     """
-
     cli_parser: ArgumentParser = ArgumentParser(
         prog="rattr",
         description=multi_paragraph_wrap(
             """\
             Parse a given Python 3 file to find the attributes used in each
             function.
 
@@ -128,15 +144,20 @@
         ShowWarnings,
         ShowPath,
         StrictOrPermissive,
         Output,
         Cache,
     )
 
-    CLI_ARG_GROUP_PARSERS = TOML_ARG_GROUP_PARSERS + (FilterString, File)
+    CLI_ARG_GROUP_PARSERS = (
+        TomlConfigPath,
+        *TOML_ARG_GROUP_PARSERS,
+        FilterString,
+        File,
+    )
 
     for argument_group_parser in CLI_ARG_GROUP_PARSERS:
         cli_parser = argument_group_parser.register(cli_parser)
         if argument_group_parser in TOML_ARG_GROUP_PARSERS:
             toml_parser = argument_group_parser.register(toml_parser)
 
     # TODO
@@ -147,15 +168,20 @@
     # extracting .toml expected field lists from 'TOML_ARG_GROUP_PARSERS'
     toml_expected_fields: Tuple[str] = ()
     for arg_group_parser in TOML_ARG_GROUP_PARSERS:
         toml_expected_fields += tuple(
             arg_group_parser.TOML_ARG_NAME_ARG_TYPE_MAP.keys()
         )
 
-    if not project_toml_cfg:
+    toml_config_override = get_toml_override(cli_parser, sys_args)
+
+    if toml_config_override is not None:
+        project_toml_cfg = load_cfg_from_project_toml(toml_config_override)
+
+    if project_toml_cfg is None:
         try:
             toml_cfg_path = find_project_toml()
             project_toml_cfg = load_cfg_from_project_toml(toml_cfg_path=toml_cfg_path)
         except TOMLDecodeError as e:
             if exit_on_error:
                 error.fatal(
                     f"Error decoding pyproject.toml file: {toml_cfg_path}. Error: {e}."
@@ -242,14 +268,36 @@
         return parser
 
     @abstractstaticmethod
     def validate(parser: ArgumentParser, arguments: Namespace) -> Namespace:
         return arguments
 
 
+class TomlConfigPath(ArgumentGroupParser):
+    def register(parser: ArgumentParser) -> ArgumentParser:
+        parser.add_argument(
+            "-c",
+            "--config",
+            default=None,
+            type=Path,
+            required=False,
+            help=multi_paragraph_wrap(
+                """\
+                >override the default toml config
+                >can't be specified in .toml
+                """
+            ),
+        )
+
+        return parser
+
+    def validate(parser: ArgumentParser, arguments: Namespace) -> Namespace:
+        return arguments
+
+
 class FollowImports(ArgumentGroupParser):
 
     ARG_LONG_NAME = "follow-imports"
 
     TOML_ARG_NAME_ARG_TYPE_MAP = {ARG_LONG_NAME: int}
 
     def register(parser: ArgumentParser) -> ArgumentParser:
```

### Comparing `rattr-0.1.5/rattr/cli/toml_parser.py` & `rattr-0.1.6/rattr/cli/toml_parser.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/cli/util.py` & `rattr-0.1.6/rattr/cli/util.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/config/__init__.py` & `rattr-0.1.6/rattr/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/error/error.py` & `rattr-0.1.6/rattr/error/error.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/plugins/__init__.py` & `rattr-0.1.6/rattr/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/plugins/analysers/builtins.py` & `rattr-0.1.6/rattr/plugins/analysers/builtins.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/plugins/analysers/collections.py` & `rattr-0.1.6/rattr/plugins/analysers/collections.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr/plugins/assertors/import_clobbering.py` & `rattr-0.1.6/rattr/plugins/assertors/import_clobbering.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/rattr.egg-info/PKG-INFO` & `rattr-0.1.6/rattr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rattr
-Version: 0.1.5
+Version: 0.1.6
 Summary: Rattr rats on your attrs.
 Home-page: https://github.com/SuadeLabs/ratter
 Author: Suade Labs
 License: MIT
 Keywords: automation linting type-checking attributes rats
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `rattr-0.1.5/rattr.egg-info/SOURCES.txt` & `rattr-0.1.6/rattr.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -60,14 +60,15 @@
 tests/test_regressions.py
 tests/test_results.py
 tests/test_util.py
 tests/context/__init__.py
 tests/context/test_context.py
 tests/context/test_symbol.py
 tests/context/test_symbol_table.py
+tests/data/config_1.toml
 tests/plugins/__init__.py
 tests/plugins/analysers/__init__.py
 tests/plugins/analysers/test_builtins.py
 tests/plugins/analysers/test_collections.py
 tests/plugins/assertors/__init__.py
 tests/plugins/assertors/test_import_clobbering.py
 tests/snippets/not_a_py.file
```

### Comparing `rattr-0.1.5/setup.py` & `rattr-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/conftest.py` & `rattr-0.1.6/tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import ast
 import sys
 from contextlib import contextmanager
 from os.path import dirname, join
+from pathlib import Path
 from typing import Iterable
 
 import pytest
 
 import rattr
 from rattr.analyser.base import CustomFunctionAnalyser, CustomFunctionHandler
 from rattr.analyser.context import Context, RootContext
@@ -843,14 +844,28 @@
 
 @pytest.fixture
 def sys_args5():
     return ["rattr", "rattr/cli/parser.py", "--permissive", "3"]
 
 
 @pytest.fixture
+def sys_args6():
+    here = Path(__file__).resolve().parent / "data" / "config_1.toml"
+
+    return [
+        "rattr",
+        "rattr/cli/parser.py",
+        "--permissive",
+        "3",
+        "--config",
+        str(here),
+    ]
+
+
+@pytest.fixture
 def walrus():
     def parse(expr: str):
         return ast.parse(f"a = ({expr})").body[0].value
 
     def _inner(*exprs):
         if len(exprs) == 0:
             raise ValueError
```

### Comparing `rattr-0.1.5/tests/context/test_context.py` & `rattr-0.1.6/tests/context/test_context.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/context/test_symbol.py` & `rattr-0.1.6/tests/context/test_symbol.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/context/test_symbol_table.py` & `rattr-0.1.6/tests/context/test_symbol_table.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/plugins/analysers/test_builtins.py` & `rattr-0.1.6/tests/plugins/analysers/test_builtins.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/plugins/analysers/test_collections.py` & `rattr-0.1.6/tests/plugins/analysers/test_collections.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/plugins/assertors/test_import_clobbering.py` & `rattr-0.1.6/tests/plugins/assertors/test_import_clobbering.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/snippets/rattr_full_one.py` & `rattr-0.1.6/tests/snippets/rattr_full_one.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_analysers.py` & `rattr-0.1.6/tests/test_analysers.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_base.py` & `rattr-0.1.6/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_cls.py` & `rattr-0.1.6/tests/test_cls.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_error.py` & `rattr-0.1.6/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_file.py` & `rattr-0.1.6/tests/test_file.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_function.py` & `rattr-0.1.6/tests/test_function.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_ir_dag.py` & `rattr-0.1.6/tests/test_ir_dag.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_parser.py` & `rattr-0.1.6/tests/test_parser.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from argparse import ArgumentError, Namespace
+from pathlib import Path
 
 import pytest
 
 from rattr.cli.parser import parse_arguments
 
 
 class TestParser:
@@ -51,14 +52,15 @@
         args = parse_arguments(
             sys_args=sys_args1[1:],
             project_toml_cfg=correct_toml_dict1,
             exit_on_error=False,
         )
 
         exp_args = Namespace(
+            config=None,
             follow_imports=3,
             exclude_import=["a\\.a\\.a", "b\\.b.*", "c\\.c\\.c\\.c", "d\\d\\.d.*"],
             exclude=["a_.*", "b_.*", "c_.*"],
             show_warnings="all",
             show_path="short",
             strict=True,
             permissive=False,
@@ -80,14 +82,15 @@
         args = parse_arguments(
             sys_args=sys_args1[1:],
             project_toml_cfg=correct_toml_dict2,
             exit_on_error=False,
         )
 
         exp_args = Namespace(
+            config=None,
             follow_imports=3,
             exclude_import=["a\\.a\\.a", "b\\.b.*", "c\\.c\\.c\\.c", "d\\d\\.d.*"],
             exclude=["a_.*", "b_.*", "c_.*"],
             show_warnings="all",
             show_path="full",
             strict=False,
             permissive=True,
@@ -109,14 +112,15 @@
         args = parse_arguments(
             sys_args=sys_args2[1:],
             project_toml_cfg=correct_toml_dict1,
             exit_on_error=False,
         )
 
         exp_args = Namespace(
+            config=None,
             follow_imports=2,
             exclude_import=["a\\.a\\.a", "b\\.b.*", "c\\.c\\.c\\.c", "d\\d\\.d.*"],
             exclude=["a_.*", "b_.*", "c_.*"],
             show_warnings="file",
             show_path="short",
             strict=True,
             permissive=False,
@@ -138,14 +142,15 @@
         args = parse_arguments(
             sys_args=sys_args3[1:],
             project_toml_cfg=correct_toml_dict1,
             exit_on_error=False,
         )
 
         exp_args = Namespace(
+            config=None,
             follow_imports=2,
             exclude_import=[
                 "a\\.a\\.a",
                 "b\\.b.*",
                 "c\\.c\\.c\\.c",
                 "d\\d\\.d.*",
                 "*exclude-import*",
@@ -173,14 +178,15 @@
         args = parse_arguments(
             sys_args=sys_args2[1:],
             project_toml_cfg=correct_toml_dict2,
             exit_on_error=False,
         )
 
         exp_args = Namespace(
+            config=None,
             follow_imports=2,
             exclude_import=["a\\.a\\.a", "b\\.b.*", "c\\.c\\.c\\.c", "d\\d\\.d.*"],
             exclude=["a_.*", "b_.*", "c_.*"],
             show_warnings="file",
             show_path="short",
             strict=True,
             permissive=False,
@@ -215,14 +221,15 @@
             # empty 'sys_args' imply no file specified in cli call
             sys_args=sys_args4[1:],
             project_toml_cfg={},
             exit_on_error=False,
         )
 
         exp_args = Namespace(
+            config=None,
             follow_imports=1,
             exclude_import=[],
             exclude=[],
             show_warnings="all",
             show_path="short",
             strict=False,
             permissive=True,
@@ -242,14 +249,15 @@
         args = parse_arguments(
             sys_args=sys_args5[1:],
             project_toml_cfg=correct_toml_dict2,
             exit_on_error=False,
         )
 
         exp_args = Namespace(
+            config=None,
             follow_imports=3,
             exclude_import=["a\\.a\\.a", "b\\.b.*", "c\\.c\\.c\\.c", "d\\d\\.d.*"],
             exclude=["a_.*", "b_.*", "c_.*"],
             show_warnings="all",
             show_path="full",
             strict=False,
             permissive=True,
@@ -260,7 +268,35 @@
             cache="cache.json",
             threshold=3,
             filter_string="",
             file="rattr/cli/parser.py",
         )
 
         assert args == exp_args
+
+    def test_toml_config_override(self, sys_args6):
+        args = parse_arguments(
+            sys_args=sys_args6[1:],
+            project_toml_cfg={},
+            exit_on_error=False,
+        )
+
+        exp_args = Namespace(
+            config=Path(__file__).resolve().parent / "data" / "config_1.toml",
+            follow_imports=1,
+            exclude_import=[],
+            exclude=[],
+            show_warnings="all",
+            show_path="full",
+            strict=False,
+            permissive=True,
+            show_ir=True,
+            show_results=False,
+            show_stats=False,
+            silent=False,
+            cache="",
+            threshold=3,
+            filter_string="",
+            file="rattr/cli/parser.py",
+        )
+
+        assert args == exp_args
```

### Comparing `rattr-0.1.5/tests/test_rattr.py` & `rattr-0.1.6/tests/test_rattr.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_regressions.py` & `rattr-0.1.6/tests/test_regressions.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_results.py` & `rattr-0.1.6/tests/test_results.py`

 * *Files identical despite different names*

### Comparing `rattr-0.1.5/tests/test_util.py` & `rattr-0.1.6/tests/test_util.py`

 * *Files identical despite different names*

