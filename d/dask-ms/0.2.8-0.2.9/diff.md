# Comparing `tmp/dask-ms-0.2.8.tar.gz` & `tmp/dask-ms-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/dask-ms-0.2.8.tar", last modified: Wed Apr  6 09:43:14 2022, max compression
+gzip compressed data, was "dist/dask-ms-0.2.9.tar", last modified: Tue Jun 28 13:25:25 2022, max compression
```

## Comparing `dask-ms-0.2.8.tar` & `dask-ms-0.2.9.tar`

### file list

```diff
@@ -1,97 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-04-06 09:43:14.000000 dask-ms-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     5840 2022-04-06 09:43:14.000000 dask-ms-0.2.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-04-06 09:43:14.000000 dask-ms-0.2.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-04-06 09:43:14.000000 dask-ms-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/
--rw-r--r--   0 runner    (1001) docker     (121)      632 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/testing.py
--rw-r--r--   0 runner    (1001) docker     (121)    13134 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/table_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)      126 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    25271 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/writes.py
--rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/example_data.py
--rw-r--r--   0 runner    (1001) docker     (121)      785 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/table.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     7169 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_ordering.py
--rw-r--r--   0 runner    (1001) docker     (121)      836 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_dataset_keywords.py
--rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_optimisation.py
--rw-r--r--   0 runner    (1001) docker     (121)     3325 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_patterns.py
--rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_columns.py
--rw-r--r--   0 runner    (1001) docker     (121)     6579 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_table_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)      846 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_stress.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_table.py
--rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_dataset_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     9862 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_ms_read_and_update.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20515 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_fsspec_store.py
--rw-r--r--   0 runner    (1001) docker     (121)    12130 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_ms_creation.py
--rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_table_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_expression.py
--rw-r--r--   0 runner    (1001) docker     (121)     2366 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    12601 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/tests/test_optional.py
--rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/table_executor.py
--rw-r--r--   0 runner    (1001) docker     (121)     8426 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/columns.py
--rw-r--r--   0 runner    (1001) docker     (121)    12300 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/dask_ms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/descriptors/
--rw-r--r--   0 runner    (1001) docker     (121)     9398 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/descriptors/ms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/descriptors/ms_subtable.py
--rw-r--r--   0 runner    (1001) docker     (121)      150 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/descriptors/register_default_builders.py
--rw-r--r--   0 runner    (1001) docker     (121)     5498 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/descriptors/builder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/descriptors/builder_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/descriptors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      747 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/descriptors/ratt_ms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3704 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/fsspec_store.py
--rw-r--r--   0 runner    (1001) docker     (121)     5788 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/optimisation.py
--rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/table_schemas.py
--rw-r--r--   0 runner    (1001) docker     (121)    13169 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/apps/
--rw-r--r--   0 runner    (1001) docker     (121)    12632 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/apps/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)      315 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/apps/application.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/apps/conf/
--rw-r--r--   0 runner    (1001) docker     (121)      322 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/apps/conf/logging.ini
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/apps/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (121)    16917 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/reads.py
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7446 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/ordering.py
--rw-r--r--   0 runner    (1001) docker     (121)     2685 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/expressions.py
--rw-r--r--   0 runner    (1001) docker     (121)     9699 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/dataset_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/
--rw-r--r--   0 runner    (1001) docker     (121)     7335 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/extension_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     5568 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/arrow_schema.py
--rw-r--r--   0 runner    (1001) docker     (121)     5768 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/writes.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     5624 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/tests/test_parquet.py
--rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/tests/test_extensions.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9653 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/reads.py
--rw-r--r--   0 runner    (1001) docker     (121)      149 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/arrow/require_arrow.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/zarr/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/zarr/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     7878 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/zarr/tests/test_zarr.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/zarr/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/zarr/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    12715 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/zarr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3153 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/experimental/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     9682 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)     5840 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    16341 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      714 2022-04-06 09:43:14.000000 dask-ms-0.2.8/daskms/query.py
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-04-06 09:43:14.000000 dask-ms-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-04-06 09:43:14.000000 dask-ms-0.2.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5886 2022-04-06 09:43:14.000000 dask-ms-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3853 2022-04-06 09:43:14.000000 dask-ms-0.2.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5031 2022-04-06 09:43:14.000000 dask-ms-0.2.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-06 09:43:14.000000 dask-ms-0.2.8/dask_ms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2343 2022-04-06 09:43:14.000000 dask-ms-0.2.8/dask_ms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)       57 2022-04-06 09:43:14.000000 dask-ms-0.2.8/dask_ms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5886 2022-04-06 09:43:14.000000 dask-ms-0.2.8/dask_ms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      238 2022-04-06 09:43:14.000000 dask-ms-0.2.8/dask_ms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-06 09:43:14.000000 dask-ms-0.2.8/dask_ms.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 09:43:14.000000 dask-ms-0.2.8/dask_ms.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-06 09:43:14.000000 dask-ms-0.2.8/dask_ms.egg-info/dependency_links.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/
+-rw-r--r--   0 runner    (1001) docker     (121)      126 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16917 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/reads.py
+-rw-r--r--   0 runner    (1001) docker     (121)      785 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2685 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/expressions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/experimental/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/experimental/zarr/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/experimental/zarr/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     9274 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/zarr/tests/test_zarr.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1818 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/zarr/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/zarr/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14301 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/zarr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3292 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/experimental/arrow/
+-rw-r--r--   0 runner    (1001) docker     (121)     5568 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/arrow_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7335 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/extension_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10977 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/reads.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/experimental/arrow/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     1951 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/tests/test_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6488 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/tests/test_parquet.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/require_arrow.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5763 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/writes.py
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/experimental/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/testing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16707 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      714 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/query.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9699 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/dataset_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13310 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/dask_ms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4486 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/example_data.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)      315 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/apps/application.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/apps/conf/
+-rw-r--r--   0 runner    (1001) docker     (121)      322 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/apps/conf/logging.ini
+-rw-r--r--   0 runner    (1001) docker     (121)     1867 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/apps/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13506 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/apps/convert.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8426 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/columns.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6375 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7446 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13169 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)     6579 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_table_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9862 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_ms_read_and_update.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2652 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_fsspec_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20515 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (121)      846 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_stress.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1801 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_storage.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4364 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1716 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2664 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      479 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1605 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_dataset_schema.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1958 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_columns.py
+-rw-r--r--   0 runner    (1001) docker     (121)      836 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1305 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_table_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3322 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_patterns.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12601 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_optional.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3327 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_dataset_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12130 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_ms_creation.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7169 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_ordering.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/tests/test_expression.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/daskms/descriptors/
+-rw-r--r--   0 runner    (1001) docker     (121)     1346 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/descriptors/ms_subtable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9674 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/descriptors/ms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      747 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/descriptors/ratt_ms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4201 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/descriptors/builder_factory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5518 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/descriptors/builder.py
+-rw-r--r--   0 runner    (1001) docker     (121)      150 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/descriptors/register_default_builders.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/descriptors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4031 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/fsspec_store.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25261 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/writes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4876 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/table_schemas.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9727 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1574 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/table_executor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5790 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/optimisation.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13134 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/table_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      632 2022-06-28 13:25:24.000000 dask-ms-0.2.9/daskms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6777 2022-06-28 13:25:24.000000 dask-ms-0.2.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1819 2022-06-28 13:25:24.000000 dask-ms-0.2.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5930 2022-06-28 13:25:25.000000 dask-ms-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3853 2022-06-28 13:25:24.000000 dask-ms-0.2.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-06-28 13:25:24.000000 dask-ms-0.2.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     1565 2022-06-28 13:25:24.000000 dask-ms-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     5075 2022-06-28 13:25:24.000000 dask-ms-0.2.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-06-28 13:25:25.000000 dask-ms-0.2.9/dask_ms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-06-28 13:25:25.000000 dask-ms-0.2.9/dask_ms.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 13:25:25.000000 dask-ms-0.2.9/dask_ms.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)     5930 2022-06-28 13:25:25.000000 dask-ms-0.2.9/dask_ms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-06-28 13:25:25.000000 dask-ms-0.2.9/dask_ms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      238 2022-06-28 13:25:25.000000 dask-ms-0.2.9/dask_ms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2372 2022-06-28 13:25:25.000000 dask-ms-0.2.9/dask_ms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-06-28 13:25:25.000000 dask-ms-0.2.9/dask_ms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-06-28 13:25:25.000000 dask-ms-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-06-28 13:25:24.000000 dask-ms-0.2.9/MANIFEST.in
```

### Comparing `dask-ms-0.2.8/setup.cfg` & `dask-ms-0.2.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 0.2.8
+current_version = 0.2.9
 commit = True
 tag = True
 tag_name = {new_version}
 parse = (?P<major>\d+)\.(?P<minor>\d+)\.(?P<patch>\d+)(\-(?P<release>[a-z]+)(?P<build>\d+))?
 serialize = 
 	{major}.{minor}.{patch}-{release}{build}
 	{major}.{minor}.{patch}
```

### Comparing `dask-ms-0.2.8/HISTORY.rst` & `dask-ms-0.2.9/HISTORY.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,34 @@
 =======
 History
 =======
 
-X.Y.Z (YYYY-MM-DD)
+0.2.9 (2022-06-28)
 ------------------
-*
+* Recreate Grouping Columns when writing to CASA format in dask-ms convert (:pr:`222`)
+* Ignore SOURCE subtable in dask-ms convert (:pr:`221`)
+* Fix cached_array implementation. (:pr:`220`)
+* Use DaskMSStore throughout dask-ms convert (:pr:`218`)
+* Upgrade from deprecated ``visit_Num`` to ``visit_Constant`` (:pr:`217`)
+* Ensure url and table consistency in DaskMSStore (:pr:`216`)
+* Wait for minio to start with greater precision (:pr:`215`)
+* Chunk correctly when reading from parquet. (:pr:`210`)
+* Fix minor bugs in zarr and conversion functionality. (:pr:`208`)
+* Add xds_to_storage_table. (:pr:`207`)
+* Add option to rechunk automatically on writes. (:pr:`204`)
+* Raise more informative error. (:pr:`203`)
+* Improve tiling. (:pr:`202`)
+* Do not create spurious fields in zarr writes. (:pr:`200`)
+* Error out when missing datavars should be written. (:pr:`197`, :pr:`198`)
+* Allow non-standard columns to be tiled. (:pr:`196`)
 
 0.2.8 (2022-04-06)
 ------------------
-* Fix #176. Fix roundtripping of boolean tensor arrays. (:pr:`194`)
-* Fix #175 for xds_from_storage_* functions. (:pr:`192`)
+* Fix roundtripping of boolean tensor arrays. (:pr:`194`)
+* Ignore unsupported kwargs in xds_from_storage_* functions. (:pr:`192`)
 * Improve handling of subtables with variably sized rows in daskms-convert. (:pr:`191`)
 * Ensure that `xds_from_zarr` sorts groups as integers and not strings (:pr:`188`)
 * Ensure Natural Ordering for parquet files (:pr:`183)
 * Fix xds_from_zarr and xds_from_parquet chunking behaviour (:pr:`182`)
 * Add LazyProxy and LazyProxyMultiton patterns to dask-ms (:pr:`177`)
 * Support cloud native storage formats via fsspec (:pr:`174`)
```

### Comparing `dask-ms-0.2.8/setup.py` & `dask-ms-0.2.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 def readme():
     with open("README.rst") as f:
         return f.read()
 
 
 setup(
     name="dask-ms",
-    version="0.2.8",
+    version="0.2.9",
     description="xarray Datasets from CASA Tables.",
     long_description=readme(),
     url="http://github.com/ska-sa/dask-ms",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
```

### Comparing `dask-ms-0.2.8/daskms/testing.py` & `dask-ms-0.2.9/daskms/testing.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/table_proxy.py` & `dask-ms-0.2.9/daskms/table_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/writes.py` & `dask-ms-0.2.9/daskms/writes.py`

 * *Files 1% similar despite different names*

```diff
@@ -306,29 +306,27 @@
         #    discarding any that currently exist on the table
 
         schemas = [DatasetSchema.from_dataset(ds, missing) for ds in datasets]
         builder = descriptor_builder(table, descriptor)
         variables = builder.dataset_variables(schemas)
         default_desc = builder.default_descriptor()
         table_desc = builder.descriptor(variables, default_desc)
-        table_desc = {m: table_desc[m] for m in missing}
 
         # Original Data Manager Groups
         odminfo = {g['NAME'] for g in table_proxy.getdminfo()
                                                  .result()
                                                  .values()}
 
-        # Construct a dminfo object with Data Manager Groups not present
-        # on the original dminfo object
-        dminfo = {f"*{i + 1}": v for i, v
-                  in enumerate(builder.dminfo(table_desc).values())
-                  if v['NAME'] not in odminfo}
-
-        # Add the columns
-        table_proxy.addcols(table_desc, dminfo=dminfo).result()
+        # NOTE(JSKenyon): Add columns one at a time - this avoids issues when
+        # adding multiple columns with different managers.
+        for col in missing:
+            _table_desc = {col: table_desc[col]}
+            _dminfo = builder.dminfo(_table_desc)
+            _dminfo = {} if _dminfo['*1']['NAME'] in odminfo else _dminfo
+            table_proxy.addcols(_table_desc, dminfo=_dminfo).result()
 
     return table_proxy
 
 
 def _add_row_wrapper(table, rows, checkrow=-1):
     startrow = table.nrows()
```

### Comparing `dask-ms-0.2.8/daskms/example_data.py` & `dask-ms-0.2.9/daskms/example_data.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/table.py` & `dask-ms-0.2.9/daskms/table.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_ordering.py` & `dask-ms-0.2.9/daskms/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_github.py` & `dask-ms-0.2.9/daskms/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_dataset_keywords.py` & `dask-ms-0.2.9/daskms/tests/test_dataset_keywords.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_optimisation.py` & `dask-ms-0.2.9/daskms/tests/test_optimisation.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_patterns.py` & `dask-ms-0.2.9/daskms/tests/test_patterns.py`

 * *Files 2% similar despite different names*

```diff
@@ -98,15 +98,15 @@
         out = pool_proxy.apply(int, args=("123456",))  # noqa
         return np.array(list(map(int, values))) + other + out
 
     values = da.blockwise(reader, "r",
                           file_proxy, None,
                           pool_proxy, None,
                           da.arange(100, chunks=10), "r",
-                          meta=np.empty((0,), np.object))
+                          meta=np.empty((0,), object))
     values.compute(scheduler="processes")
 
 
 def test_multiton():
     class A(metaclass=Multiton):
         def __init__(self, *args, **kwargs):
             self.args = args
```

### Comparing `dask-ms-0.2.8/daskms/tests/test_columns.py` & `dask-ms-0.2.9/daskms/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_table_proxy.py` & `dask-ms-0.2.9/daskms/tests/test_table_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_stress.py` & `dask-ms-0.2.9/daskms/tests/test_stress.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_dataset_schema.py` & `dask-ms-0.2.9/daskms/tests/test_dataset_schema.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_executor.py` & `dask-ms-0.2.9/daskms/tests/test_executor.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_ms_read_and_update.py` & `dask-ms-0.2.9/daskms/tests/test_ms_read_and_update.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_dataset.py` & `dask-ms-0.2.9/daskms/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_ms_creation.py` & `dask-ms-0.2.9/daskms/tests/test_ms_creation.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_table_schemas.py` & `dask-ms-0.2.9/daskms/tests/test_table_schemas.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_expression.py` & `dask-ms-0.2.9/daskms/tests/test_expression.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/tests/test_utils.py` & `dask-ms-0.2.9/daskms/tests/test_utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import platform
 
 import pytest
 
 from daskms.utils import (promote_columns,
                           natural_order,
                           table_path_split,
-                          requires)
+                          requires,
+                          filter_kwargs)
 
 
 def test_natural_order():
     data = [f"{i}.parquet" for i in reversed(range(20))]
     expected = [f"{i}.parquet" for i in range(20)]
     assert sorted(data, key=natural_order) == expected
     assert sorted(data) != expected
@@ -74,7 +75,20 @@
 
     assert "1. foo" in e.value.msg
     assert "2. bar" in e.value.msg
     assert "need foo" in e.value.msg
     assert "need bar" in e.value.msg
 
     assert requires("need foo", 1, None)(fn)() == 1
+
+
+def test_filter_kwargs():
+
+    def f(arg0, arg1=None, arg2=None):
+        return
+
+    kwargs = {"arg0": None, "arg1": None, "arg2": None, "arg3": None}
+
+    with pytest.warns(UserWarning):
+        filter_kwargs(f, kwargs)
+
+    assert "arg3" not in kwargs
```

### Comparing `dask-ms-0.2.8/daskms/tests/test_optional.py` & `dask-ms-0.2.9/daskms/tests/test_optional.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/table_executor.py` & `dask-ms-0.2.9/daskms/table_executor.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/columns.py` & `dask-ms-0.2.9/daskms/columns.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/dask_ms.py` & `dask-ms-0.2.9/daskms/dask_ms.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import logging
 
 from daskms.fsspec_store import DaskMSStore
 from daskms.table_proxy import TableProxy
 from daskms.reads import DatasetFactory
 from daskms.writes import write_datasets
-from daskms.utils import promote_columns
+from daskms.utils import promote_columns, filter_kwargs
 
 _DEFAULT_INDEX_COLUMNS = []
 _DEFAULT_GROUP_COLUMNS = ["FIELD_ID", "DATA_DESC_ID"]
 
 log = logging.getLogger(__name__)
 
 
@@ -68,22 +68,30 @@
     write_datasets : list of :class:`xarray.Dataset`
         Datasets containing arrays representing write operations
         into a CASA Table
     table_proxy : :class:`daskms.TableProxy`, optional
         The Table Proxy associated with the datasets
     """
     if isinstance(table_name, DaskMSStore):
-        table_name = table_name.casa_path()
+        store = table_name
     else:
-        table_name = DaskMSStore(table_name).casa_path()
+        store = DaskMSStore(table_name)
+
+    table_name = store.casa_path()
 
     # Promote dataset to a list
     if not isinstance(xds, (tuple, list)):
         xds = [xds]
 
+    # Not writing to an existing dataset so we drop ROWID to ensure that rows
+    # get added correctly. TODO: This may be a little brittle - we could
+    # consider altering the functionality in writes.py.
+    if not store.exists():
+        xds = [ds.drop_vars("ROWID", errors="ignore") for ds in xds]
+
     if not isinstance(columns, (tuple, list)):
         if columns != "ALL":
             columns = [columns]
 
     # Write the datasets
     out_ds = write_datasets(table_name, xds, columns,
                             descriptor=descriptor,
@@ -346,14 +354,35 @@
     elif typ == "parquet":
         from daskms.experimental.arrow import xds_from_parquet
         return xds_from_parquet(store, **kwargs)
     else:
         raise TypeError(f"Unknown dataset {typ}")
 
 
+def xds_to_storage_table(xds, store, **kwargs):
+    if not isinstance(store, DaskMSStore):
+        store = DaskMSStore(store)
+
+    typ = store.type()
+
+    if typ == "casa":
+        filter_kwargs(xds_to_table, kwargs)
+        return xds_to_table(xds, store,  **kwargs)
+    elif typ == "zarr":
+        from daskms.experimental.zarr import xds_to_zarr
+        filter_kwargs(xds_to_zarr, kwargs)
+        return xds_to_zarr(xds, store, **kwargs)
+    elif typ == "parquet":
+        from daskms.experimental.arrow import xds_to_parquet
+        filter_kwargs(xds_to_parquet, kwargs)
+        return xds_to_parquet(xds, store, **kwargs)
+    else:
+        raise TypeError(f"Unknown dataset {typ}")
+
+
 # Set docstring variables in try/except
 # ``__doc__`` may not be present as
 # ``python -OO`` strips docstrings
 try:
     xds_from_ms.__doc__ %= {
         'indices': _DEFAULT_INDEX_COLUMNS,
         'groups': _DEFAULT_GROUP_COLUMNS}
```

### Comparing `dask-ms-0.2.8/daskms/descriptors/ms.py` & `dask-ms-0.2.9/daskms/descriptors/ms.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 # -*- coding: utf-8 -*-
-
-from functools import reduce
 import logging
-from operator import mul
 
 import numpy as np
 import pyrap.tables as pt
 
 from daskms.columns import infer_dtype
 from daskms.descriptors.builder import (register_descriptor_builder,
                                         AbstractDescriptorBuilder)
@@ -160,82 +157,86 @@
         col_desc['option'] |= 4
         col_desc['dataManagerGroup'] = f"{column}_GROUP"
         col_desc['dataManagerType'] = "TiledColumnStMan"
 
     def fix_columns(self, variables, desc, dim_sizes):
         """ Set large columns to fixed columns """
 
-        # We need channel and correlation
-        try:
-            chan = dim_sizes['chan']
-        except KeyError:
-            log.warning("Unable to infer 'chan' dimension from variables. "
-                        "Columns won't be FixedShape.")
-            return desc
-        else:
-            if np.isnan(chan):
-                log.warning("'nan' chan dimension. "
-                            "Columns won't be FixedShape.")
-                return desc
+        # NOTE(JSKenyon): Attempt to make custom (non-standard) columns fixed
+        # shape when possible. Only chan and corr dimensions are handled at
+        # the moment.
+        for col_name, schemas in variables.items():
+            # Don't attempt to fix columns with object type.
+            if schemas[0].dtype == np.dtype('O'):
+                continue
+
+            schema_dims = schemas[0].dims
+            # First dim must be row (for now).
+            if schema_dims[0] != "row":
+                continue
+            # Don't bother fixing row-only columns.
+            if len(schema_dims) == 1:
+                continue
 
-            # We can fix IMAGING_WEIGHT at least
-            self._maybe_fix_column('IMAGING_WEIGHT', desc, (chan,))
-
-        try:
-            corr = dim_sizes['corr']
-        except KeyError:
-            log.warning("Unable to infer 'corr' dimension from variables. "
-                        "Columns won't be FixedShape.")
-            return desc
-        else:
-            if np.isnan(corr):
-                log.warning("'nan' corr dimension. "
-                            "Columns won't be FixedShape.")
-
-        self._maybe_fix_column('FLAG', desc, (chan, corr))
-        self._maybe_fix_column('DATA', desc, (chan, corr))
-        self._maybe_fix_column('MODEL_DATA', desc, (chan, corr))
-        self._maybe_fix_column('CORRECTED_DATA', desc, (chan, corr))
-        self._maybe_fix_column('WEIGHT_SPECTRUM', desc, (chan, corr))
-        self._maybe_fix_column('SIGMA_SPECTRUM', desc, (chan, corr))
+            try:
+                shape = tuple([dim_sizes[d] for d in schema_dims[1:]])
+            except KeyError:  # We don't understand the dims.
+                log.warning(f"Could not fix shape for column {col_name} "
+                            f"with dimensions {schema_dims}.")
+                continue
+
+            if np.nan in shape:
+                log.warning(f"Could not fix shape for column {col_name} "
+                            f"with np.nan in shape.")
+                continue
 
-        try:
-            flagcat = dim_sizes['flagcat']
-        except KeyError:
-            log.warning("Unable to infer 'flagcat' dimension "
-                        "from input variables")
-        else:
-            self._maybe_fix_column("FLAG_CATEGORY", desc,
-                                   (flagcat, chan, corr))
+            self._maybe_fix_column(col_name, desc, shape)
 
         return desc
 
     def _fit_tile_shape(self, desc):
         """ Infer a tile shape """
         try:
             shape = desc['shape']
         except KeyError:
             raise ValueError(f"No shape in descriptor {desc}")
-        else:
-            rev_shape = tuple(reversed(shape))
 
         try:
             casa_type = desc['valueType']
         except KeyError:
             raise ValueError(f"No valueType in descriptor {desc}")
         else:
             dtype = infer_dtype(casa_type, desc)
             nbytes = np.dtype(dtype).itemsize
 
-        rows = 1
+        # NOTE(JSKenyon): The following is entirely heuristic and may require
+        # adjustments if chunks grow unwieldy.
+
+        min_tile_dims = [512]  # Approx sensible starting number of rows.
+        max_tile_dims = [np.inf]
 
-        while reduce(mul, rev_shape + (2*rows,), 1)*nbytes < 4*1024*1024:
-            rows *= 2
+        for dim in shape:
+            min_tile = min(dim, 4)  # Don't tile <=4 elements.
+            # For dims which are not exact powers of two, treat them as though
+            # they are floored to the nearest power of two.
+            max_tile = int(min(2 ** int(np.log2(dim)) / 8, 64))
+            max_tile = min_tile if max_tile < min_tile else max_tile
+            min_tile_dims.append(min_tile)
+            max_tile_dims.append(max_tile)
+
+        tile_shape = min_tile_dims.copy()
+        growth_axis = 0
+
+        while np.prod(tile_shape)*nbytes < 1024**2:  # 1MB tiles.
+            if tile_shape[growth_axis] < max_tile_dims[growth_axis]:
+                tile_shape[growth_axis] *= 2
+            growth_axis += 1
+            growth_axis %= len(tile_shape)
 
-        return {"DEFAULTTILESHAPE": np.int32(rev_shape + (2*rows,))}
+        return {"DEFAULTTILESHAPE": np.int32(tile_shape[::-1])}
 
     def dminfo(self, table_desc):
         """
         Create Data Manager Info for the MS, adding Tiled Shapes to
         all TiledColumnStMan groups.
         """
```

### Comparing `dask-ms-0.2.8/daskms/descriptors/ms_subtable.py` & `dask-ms-0.2.9/daskms/descriptors/ms_subtable.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/descriptors/builder.py` & `dask-ms-0.2.9/daskms/descriptors/builder.py`

 * *Files 8% similar despite different names*

```diff
@@ -133,18 +133,17 @@
         dtypes.add(v.dtype)
 
         if v.ndim == 0:
             # Scalar array, ndim == 0 in numpy and CASA
             ndims.append(0)
         else:
             if not v.dims[0] == "row":
-                log.warning(f"Column {column} doesn't start with "
-                            f"with a 'row' dimension: {v.dims} "
-                            f"and will be ignored")
-                continue
+                raise ValueError(f"'row' is not the first dimension in the "
+                                 f"dimensions {v.dims} of column {column}. "
+                                 f"Column cannot be added to MAIN table.")
 
             # Row only, so ndim must be removed from the descriptor
             # Add a marker to distinguish in case of multiple
             # shapes
             if v.ndim == 1:
                 ndims.add('row')
             # Other dims, add dimension data, excluding the row
```

### Comparing `dask-ms-0.2.8/daskms/descriptors/builder_factory.py` & `dask-ms-0.2.9/daskms/descriptors/builder_factory.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/descriptors/ratt_ms.py` & `dask-ms-0.2.9/daskms/descriptors/ratt_ms.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/fsspec_store.py` & `dask-ms-0.2.9/daskms/fsspec_store.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 from pathlib import Path, PurePath
 
 import fsspec
 
-from daskms.patterns import Multiton
 
-
-class DaskMSStore(metaclass=Multiton):
+class DaskMSStore:
     def __init__(self, url, **storage_options):
         if isinstance(url, PurePath):
             url = str(url)
 
-        self.url = url
-        self.map = fsspec.get_mapper(url, **storage_options)
-        self.fs = self.map.fs
-        self.storage_options = storage_options
-        protocol = fsspec.core.split_protocol(url)[0]
-        self.protocol = "file" if protocol is None else protocol
-
-        path = fsspec.core.strip_protocol(url)
-        bits = path.split("::", 1)
+        bits = url.split("::", 1)
 
         if len(bits) == 1:
-            path = bits[0]
-            table = "MAIN"
+            url = bits[0]
+            table = ""
         elif len(bits) == 2:
-            path, table = bits
+            url, table = bits
 
             if table == "MAIN":
                 raise ValueError("MAIN is a reserved table name")
         else:
             raise RuntimeError(f"len(bits): {len(bits)} not in (1, 2)")
 
-        self.path = path
-        self.table = table
+        self.map = fsspec.get_mapper(url, **storage_options)
+        self.fs = self.map.fs
+        self.storage_options = storage_options
+        protocol, path = fsspec.core.split_protocol(url)
+        self.protocol = "file" if protocol is None else protocol
+
+        if table:
+            self.canonical_path = f"{path}::{table}"
+            self.full_path = f"{path}{self.fs.sep}{table}"
+            self.table = table
+        else:
+            self.canonical_path = path
+            self.full_path = path
+            self.table = "MAIN"
 
     def type(self):
         """
         Returns
         -------
         type : {"casa", "zarr", "parquet"}
             Type of table at the specified path
@@ -46,75 +48,83 @@
         TypeError
             If it was not possible to infer the type of dataset
         """
         # From shallowest to deepest recursion
         if self.exists("table.dat"):
             return "casa"
         else:
-            for _, _, files in self.fs.walk(self.path):
+            for _, _, files in self.fs.walk(self.full_path):
                 for f in files:
                     if f == ".zgroup":
                         return "zarr"
                     elif f.endswith(".parquet"):
                         return "parquet"
 
-        raise TypeError(f"Unknown table type at {self.url}")
+        raise ValueError(f"Unable to infer table type at {self.full_path}")
+
+    @property
+    def url(self):
+        return f"{self.fs.unstrip_protocol(self.canonical_path)}"
 
     def subdirectories(self):
         return [d["name"] for d
-                in self.fs.listdir(self.path, detail=True)
+                in self.fs.listdir(self.full_path, detail=True)
                 if d["type"] == "directory"]
 
     def casa_path(self):
         if self.protocol != "file":
-            raise ValueError(f"CASA Tables don't work with the "
+            raise ValueError(f"CASA Tables are incompatible with the "
                              f"{self.protocol} protocol")
 
-        return (self.path if self.table == "MAIN"
-                else f"{self.path}::{self.table}")
+        return self.canonical_path
 
     @staticmethod
     def from_url_storage_options(url, storage_options):
         return DaskMSStore(url, **storage_options)
 
     def __reduce__(self):
         return (DaskMSStore.from_url_storage_options,
                 (self.url, self.storage_options))
 
     def __getitem__(self, key):
         return self.map[key]
 
-    def exists(self, path):
-        fullpath = "".join((self.path, self.fs.sep, path))
-        return self.fs.exists(fullpath)
+    def _extend_path(self, path=""):
+        return (f"{self.full_path}{self.fs.sep}{path}"
+                if self.full_path
+                else self.full_path)
+
+    def exists(self, path=""):
+        return self.fs.exists(self._extend_path(path))
 
-    def ls(self, path=None):
-        path = path or self.path
+    def ls(self, path=""):
+        path = self._extend_path(path)
         return list(map(Path, self.fs.ls(path, detail=False)))
 
     @staticmethod
     def _remove_prefix(s, prefix):
         return s[len(prefix):] if s.startswith(prefix) else s
 
     def rglob(self, pattern, **kwargs):
         sep = self.fs.sep
-        fullpath = "".join(
-            (self.path, sep, self.table, sep, "**", sep, pattern)
-        )
-        paths = self.fs.glob(fullpath, **kwargs)
-        prefix = "".join((self.path, sep))
+        globpath = f"{self.full_path}{sep}**{sep}{pattern}"
+        paths = self.fs.glob(globpath, **kwargs)
+        prefix = f"{self.full_path}{sep}"
         return (self._remove_prefix(p, prefix) for p in paths)
 
-    def open_file(self, key, *args, **kwargs):
-        fullpath = f"{self.path}{self.fs.sep}{key}"
-        return self.fs.open(fullpath, *args, **kwargs)
+    def open(self, key, *args, **kwargs):
+        path = self._extend_path(key)
+        return self.fs.open(path, *args, **kwargs)
 
     def makedirs(self, key, *args, **kwargs):
-        fullpath = f"{self.path}{self.fs.sep}{key}"
-        return self.fs.makedirs(fullpath, *args, **kwargs)
+        path = self._extend_path(key)
+        return self.fs.makedirs(path, *args, **kwargs)
+
+    def rm(self, path="", recursive=False, maxdepth=None):
+        path = self._extend_path(path)
+        self.fs.rm(path, recursive=recursive, maxdepth=maxdepth)
 
     def subtable_store(self, subtable):
         if subtable == "MAIN":
             return self
 
-        fullpath = f"{self.url}{self.fs.sep}{subtable}"
-        return DaskMSStore(fullpath, **self.storage_options)
+        return DaskMSStore(f"{self.url}::{subtable}", **self.storage_options)
```

### Comparing `dask-ms-0.2.8/daskms/optimisation.py` & `dask-ms-0.2.9/daskms/optimisation.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
     def __reduce__(self):
         return (Key, (self.key,))
 
     __str__ = __repr__
 
 
-def cache_entry(cache, key, task):
+def cache_entry(cache, key, *task):
     with cache.lock:
         try:
             return cache.cache[key]
         except KeyError:
             cache.cache[key] = value = _execute_task(task, {})
             return value
 
@@ -140,15 +140,15 @@
 
     # Create a cache used to store array values
     cache = ArrayCache(token)
 
     assert len(dsk3) == len(keys)
 
     for k in keys:
-        dsk3[k] = (cache_entry, cache, Key(k), dsk3.pop(k))
+        dsk3[k] = (cache_entry, cache, Key(k), *dsk3.pop(k))
 
     graph = HighLevelGraph.from_collections(array.name, dsk3, [])
 
     return da.Array(graph, array.name, array.chunks, array.dtype)
 
 
 def inlined_array(a, inline_arrays=None):
```

### Comparing `dask-ms-0.2.8/daskms/table_schemas.py` & `dask-ms-0.2.9/daskms/table_schemas.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/patterns.py` & `dask-ms-0.2.9/daskms/patterns.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/apps/convert.py` & `dask-ms-0.2.9/daskms/apps/convert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import abc
 import ast
 from argparse import ArgumentTypeError
 from functools import partial
 import logging
 from pathlib import Path
-import shutil
+
+import dask.array as da
 
 from daskms.apps.application import Application
 from daskms.fsspec_store import DaskMSStore
 
 log = logging.getLogger(__name__)
 
 
@@ -31,15 +32,15 @@
 
     def visit_Name(self, node):
         return node.id
 
     def visit_Tuple(self, node):
         return tuple(self.visit(v) for v in node.elts)
 
-    def visit_Num(self, node):
+    def visit_Constant(self, node):
         return node.n
 
 
 class TableFormat(abc.ABC):
     @abc.abstractproperty
     def version(self):
         raise NotImplementedError
@@ -54,15 +55,15 @@
 
     @abc.abstractclassmethod
     def writer(self):
         raise NotImplementedError
 
     @staticmethod
     def from_path(path):
-        store = DaskMSStore(path)
+        store = path if isinstance(path, DaskMSStore) else DaskMSStore(path)
         typ = store.type()
 
         if typ == "casa":
             from daskms.table_proxy import TableProxy
             import pyrap.tables as pt
             table_proxy = TableProxy(pt.table, str(store.casa_path()),
                                      readonly=True, ack=False)
@@ -85,14 +86,16 @@
             subtables = ParquetFormat.find_subtables(store)
             return ParquetFormat("0.1", subtables)
         else:
             raise ValueError(f"Unexpected table type {typ}")
 
     @staticmethod
     def from_type(typ):
+        if typ == "ms":
+            return CasaFormat("2.0", [], "measurementset")
         if typ == "casa":
             return CasaFormat("<unspecified>", [], "plain")
         elif typ == "zarr":
             return ZarrFormat("0.1", [])
         elif typ == "parquet":
             return ParquetFormat("0.1", [])
         else:
@@ -264,80 +267,27 @@
     def __str__(self):
         return "parquet"
 
 
 NONUNIFORM_SUBTABLES = ["SPECTRAL_WINDOW", "POLARIZATION", "FEED", "SOURCE"]
 
 
-def convert_table(args):
-    in_fmt = TableFormat.from_path(args.input)
-    out_fmt = TableFormat.from_type(args.format)
-
-    reader = in_fmt.reader(
-        group_columns=args.group_columns,
-        index_columns=args.index_columns
-    )
-    writer = out_fmt.writer()
-
-    datasets = reader(args.input, chunks=args.chunks)
-
-    if isinstance(in_fmt, CasaFormat):
-        # Drop any ROWID columns
-        datasets = [ds.drop_vars("ROWID", errors="ignore")
-                    for ds in datasets]
-
-    log.info("Input: '%s' %s", in_fmt, str(args.input))
-    log.info("Output: '%s' %s", out_fmt, str(args.output))
-
-    writes = [writer(datasets, str(args.output))]
-
-    # Now do the subtables
-    for table in list(in_fmt.subtables):
-        if table == "SORTED_TABLE":
-            log.warning(f"Ignoring {table}")
-            continue
-
-        in_path = args.input.parent / "::".join((args.input.name, table))
-        in_fmt = TableFormat.from_path(in_path)
-        out_path = args.output.parent / "::".join((args.output.name, table))
-        out_fmt = TableFormat.from_type(args.format)
-
-        reader = in_fmt.reader()
-        writer = out_fmt.writer()
-
-        if isinstance(in_fmt, CasaFormat) and table in NONUNIFORM_SUBTABLES:
-            # Drop any ROWID columns
-            datasets = [ds.drop_vars("ROWID", errors="ignore")
-                        for ds in reader(in_path, group_cols="__row__")]
-        else:
-            datasets = reader(in_path)
-
-        writes.append(writer(datasets, str(out_path)))
-
-    return writes
-
-
 def _check_input_path(input: str):
-    input_path = Path(input)
-
-    parts = input_path.name.split("::", 1)
-
-    if len(parts) == 1:
-        check_path = input_path
-    elif len(parts) == 2:
-        check_path = input_path.parent / parts[0]
-    else:
-        raise RuntimeError("len(parts) not in (1, 2)")
+    input_path = DaskMSStore(input)
 
-    if not check_path.exists():
+    if not input_path.exists():
         raise ArgumentTypeError(f"{input} is an invalid path.")
 
     return input_path
 
 
+def _check_output_path(output: str):
+    return DaskMSStore(output)
+
+
 def parse_chunks(chunks: str):
     return ChunkTransformer().visit(ast.parse(chunks))
 
 
 class Convert(Application):
     TABLE_KEYWORD_PREFIX = "Table: "
 
@@ -351,15 +301,15 @@
             return None
 
         return [c.strip() for c in columns.split(",")]
 
     @classmethod
     def setup_parser(cls, parser):
         parser.add_argument("input", type=_check_input_path)
-        parser.add_argument("-o", "--output", type=Path)
+        parser.add_argument("-o", "--output", type=_check_output_path)
         parser.add_argument("-g", "--group-columns",
                             type=Convert.col_converter,
                             default="",
                             help="Columns to group or partition "
                                  "the input dataset by. "
                                  "This defaults to the default "
                                  "for the underlying storage mechanism."
@@ -371,15 +321,15 @@
                             help="Columns to sort "
                                  "the input dataset by. "
                                  "This defaults to the default "
                                  "for the underlying storage mechanism."
                                  "This is only supported when converting "
                                  "from casa format.")
         parser.add_argument("-f", "--format",
-                            choices=["casa", "zarr", "parquet"],
+                            choices=["ms", "casa", "zarr", "parquet"],
                             default="zarr",
                             help="Output format")
         parser.add_argument("--force",
                             action="store_true",
                             default=False,
                             help="Force overwrite of output")
         parser.add_argument("-c", "--chunks",
@@ -389,15 +339,85 @@
                             type=parse_chunks)
 
     def execute(self):
         import dask
 
         if self.args.output.exists():
             if self.args.force:
-                shutil.rmtree(self.args.output)
+                self.args.output.rm(recursive=True)
             else:
                 raise ValueError(f"{self.args.output} exists. "
                                  f"Use --force to overwrite.")
 
-        writes = convert_table(self.args)
+        writes = self.convert_table(self.args)
 
         dask.compute(writes)
+
+    def _convert_casa_datasets(self, datasets, args):
+        new_datasets = []
+        group_columns = args.group_columns or []
+
+        for ds in datasets:
+            # Drop any ROWID columns
+            new_ds = ds.drop_vars("ROWID", errors="ignore")
+
+            # Remove grouping attribute and recreate grouping columns
+            new_group_vars = {}
+            row_chunks = new_ds.chunks["row"]
+            row_dims = new_ds.dims["row"]
+
+            for column in group_columns:
+                value = new_ds.attrs.pop(column)
+                group_column = da.full(row_dims, value, chunks=row_chunks)
+                new_group_vars[column] = (("row",), group_column)
+
+            new_datasets.append(new_ds.assign(**new_group_vars))
+
+        return new_datasets
+
+    def convert_table(self, args):
+        in_fmt = TableFormat.from_path(args.input)
+        out_fmt = TableFormat.from_type(args.format)
+
+        reader = in_fmt.reader(
+            group_columns=args.group_columns,
+            index_columns=args.index_columns
+        )
+        writer = out_fmt.writer()
+
+        datasets = reader(args.input, chunks=args.chunks)
+
+        if isinstance(in_fmt, CasaFormat):
+            datasets = self._convert_casa_datasets(datasets, args)
+
+        log.info("Input: '%s' %s", in_fmt, str(args.input))
+        log.info("Output: '%s' %s", out_fmt, str(args.output))
+
+        writes = [writer(datasets, args.output)]
+
+        # Now do the subtables
+        for table in list(in_fmt.subtables):
+            if table in {"SORTED_TABLE", "SOURCE"}:
+                log.warning(f"Ignoring {table}")
+                continue
+
+            in_store = args.input.subtable_store(table)
+            in_fmt = TableFormat.from_path(in_store)
+            out_store = args.output.subtable_store(table)
+            out_fmt = TableFormat.from_type(args.format)
+
+            reader = in_fmt.reader()
+            writer = out_fmt.writer()
+
+            if (isinstance(in_fmt, CasaFormat) and
+                    table in NONUNIFORM_SUBTABLES):
+                datasets = reader(in_store, group_cols="__row__")
+            else:
+                datasets = reader(in_store)
+
+            if isinstance(in_fmt, CasaFormat):
+                datasets = [ds.drop_vars("ROWID", errors="ignore")
+                            for ds in datasets]
+
+            writes.append(writer(datasets, out_store))
+
+        return writes
```

### Comparing `dask-ms-0.2.8/daskms/apps/entrypoint.py` & `dask-ms-0.2.9/daskms/apps/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/reads.py` & `dask-ms-0.2.9/daskms/reads.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/__init__.py` & `dask-ms-0.2.9/daskms/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 
 import logging
 
 __author__ = """Simon Perkins"""
 __email__ = "sperkins@ska.ac.za"
-__version__ = "0.2.8"
+__version__ = "0.2.9"
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
-from daskms.dask_ms import (xds_from_storage_ms, xds_from_table,      # noqa
-                                xds_to_table,    # noqa
-                                xds_from_ms,     # noqa
-                                xds_from_storage_ms,     # noqa
-                                xds_from_storage_table)  # noqa
+from daskms.dask_ms import (xds_from_table,  # noqa
+                            xds_from_ms,  # noqa
+                            xds_from_storage_ms,  # noqa
+                            xds_from_storage_table,  # noqa
+                            xds_to_table,  # noqa
+                            xds_to_storage_table)  # noqa
 
 from daskms.dataset import Dataset, Variable     # noqa
 from daskms.table_proxy import TableProxy        # noqa
```

### Comparing `dask-ms-0.2.8/daskms/ordering.py` & `dask-ms-0.2.9/daskms/ordering.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/expressions.py` & `dask-ms-0.2.9/daskms/expressions.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/dataset_schema.py` & `dask-ms-0.2.9/daskms/dataset_schema.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/experimental/arrow/extension_types.py` & `dask-ms-0.2.9/daskms/experimental/arrow/extension_types.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/experimental/arrow/arrow_schema.py` & `dask-ms-0.2.9/daskms/experimental/arrow/arrow_schema.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/experimental/arrow/writes.py` & `dask-ms-0.2.9/daskms/experimental/arrow/writes.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 raise NotImplementedError("Scalar array writing "
                                           "not implemented")
 
             table_data[column] = pa_data
 
         table = pa.table(table_data, schema=self.schema.to_arrow_schema())
         parquet_filename = self.key / f"{chunk.item()}.parquet"
-        sf = self.store.open_file(parquet_filename, "wb")
+        sf = self.store.open(parquet_filename, "wb")
         pq.write_table(table, sf)
 
         return np.array([True], bool)
 
 
 @requires_arrow(pyarrow_import_error)
 def xds_to_parquet(xds, store, columns=None):
```

### Comparing `dask-ms-0.2.8/daskms/experimental/arrow/tests/test_parquet.py` & `dask-ms-0.2.9/daskms/experimental/arrow/tests/test_parquet.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import random
+from itertools import chain
 
 import dask
 import dask.array as da
 import numpy as np
 from numpy.testing import assert_array_equal
 import pytest
 
 from daskms import xds_from_storage_ms
+from daskms.dask_ms import xds_from_ms
 from daskms.dataset import Dataset
 from daskms.fsspec_store import DaskMSStore
 from daskms.experimental.arrow.extension_types import TensorArray
 from daskms.experimental.arrow.reads import xds_from_parquet
 from daskms.experimental.arrow.reads import partition_chunking
 from daskms.experimental.arrow.writes import xds_to_parquet
 from daskms.constants import DASKMS_PARTITION_KEY
@@ -70,15 +72,19 @@
 @pytest.mark.parametrize("row_chunks", [[2, 3, 4]])
 @pytest.mark.parametrize("user_chunks", [{"row": 2, "chan": 4}])
 def test_partition_chunks(row_chunks, user_chunks):
     expected = [(0, (0, 2)),
                 (1, (0, 2)), (1, (2, 3)),
                 (2, (0, 1)), (2, (1, 3)), (2, (3, 4))]
 
-    assert partition_chunking(0, row_chunks, [user_chunks]) == expected
+    partition_chunks = partition_chunking(0, row_chunks, [user_chunks])
+
+    obtained = chain.from_iterable([c for c in partition_chunks.values()])
+
+    assert list(obtained) == expected
 
 
 def test_xds_to_parquet_string(tmp_path_factory):
     store = tmp_path_factory.mktemp("parquet_store") / "string-dataset.parquet"
 
     datasets = []
 
@@ -153,17 +159,42 @@
 
     py_minio_client.make_bucket(s3_bucket_name)
 
     store = DaskMSStore(f"s3://{s3_bucket_name}/measurementset.MS",
                         key=minio_user_key,
                         secret=minio_user_key,
                         client_kwargs={
-                          "endpoint_url": minio_url.geturl(),
-                          "region_name": "af-cpt",
+                            "endpoint_url": minio_url.geturl(),
+                            "region_name": "af-cpt",
                         })
 
     # NOTE(sjperkins)
     # Review this interface
     # spw_store = store.subtable_store("SPECTRAL_WINDOW")
     # ant_store = store.subtable_store("ANTENNA")
 
     return parquet_tester(ms, store)
+
+
+@pytest.fixture(params=[1, 2, 3, 4])
+def parquet_ms(ms, tmp_path_factory, request):
+
+    parquet_store = tmp_path_factory.mktemp("parquet") / "test.parquet"
+
+    # Chunk in row so we can probe chunk behaviour on reads.
+    xdsl = xds_from_ms(ms, chunks={"row": request.param})
+
+    writes = xds_to_parquet(xdsl, parquet_store)
+
+    dask.compute(writes)  # Write to parquet.
+
+    return parquet_store
+
+
+@pytest.mark.parametrize("rc", [1, 2, 3, 4])
+def test_xds_from_parquet_chunks(ms, parquet_ms, rc):
+
+    xdsl = xds_from_parquet(parquet_ms, chunks={'row': rc})
+
+    chunks = chain.from_iterable([xds.chunks['row'] for xds in xdsl])
+
+    assert all([c <= rc for c in chunks])
```

### Comparing `dask-ms-0.2.8/daskms/experimental/arrow/tests/test_extensions.py` & `dask-ms-0.2.9/daskms/experimental/arrow/tests/test_extensions.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/experimental/arrow/reads.py` & `dask-ms-0.2.9/daskms/experimental/arrow/reads.py`

 * *Files 10% similar despite different names*

```diff
@@ -72,15 +72,15 @@
 
         with self.lock:
             try:
                 return self._file
             except AttributeError:
                 pass
 
-            sf = self.store.open_file(self.key, "rb")
+            sf = self.store.open(self.key, "rb")
             self._file = file_ = pq.ParquetFile(sf)
             return file_
 
     @property
     def metadata(self):
         return self.file.metadata
 
@@ -110,15 +110,18 @@
         field, value = (s.strip() for s in ps.split("="))
 
         if field != pf:
             raise ValueError(f"Column name {field} in partition string "
                              f"{partition_strings} does not match "
                              f"metadata column name {pf}")
 
-        partitions.append((field, np.dtype(dt).type(value)))
+        # NOTE(JSKenyon): Use item to get a python type. Coercing to numpy
+        # type is not used for the other formats and causes serialization
+        # woes.
+        partitions.append((field, np.dtype(dt).type(value).item()))
 
     return tuple(partitions)
 
 
 def partition_chunking(partition, fragment_rows, chunks):
     partition_rows = sum(fragment_rows)
 
@@ -146,18 +149,19 @@
         if isinstance(row_chunks, list):
             row_chunks = tuple(row_chunks)
 
         row_chunks = normalize_chunks(row_chunks, (partition_rows,))[0]
 
     intervals = np.cumsum([0] + fragment_rows)
     chunk_intervals = np.cumsum((0,) + row_chunks)
-    ranges = []
+    ranges = defaultdict(list)
     it = zip(chunk_intervals, chunk_intervals[1:])
 
     for c, (lower, upper) in enumerate(it):
+
         si = np.searchsorted(intervals, lower, side='right') - 1
         ei = np.searchsorted(intervals, upper, side='left')
 
         if si == ei:
             raise ValueError("si == ei, arrays may have zero chunks")
 
         for s in range(si, ei):
@@ -169,19 +173,36 @@
                 start = lower - intervals[s]
 
             if upper >= intervals[e]:
                 end = intervals[e] - intervals[s]
             else:
                 end = upper - intervals[s]
 
-            ranges.append((s, (start, end)))
+            ranges[c].append((s, (start, end)))
 
     return ranges
 
 
+def fragment_reader(fragments, ranges, column, shape, dtype):
+
+    if len(fragments) > 1:  # Reading over multiple row_groups.
+        arr = np.empty(shape, dtype=dtype)
+        offset = 0
+        for fragment, (start, end) in zip(fragments, ranges):
+            sel = slice(offset, offset + (end - start))
+            arr[sel] = fragment.read_column(column, start, end)
+            offset += (end - start)
+    else:
+        fragment = fragments[0]
+        start, end = ranges[0]
+        arr = fragment.read_column(column, start, end)
+
+    return arr
+
+
 @requires_arrow(pyarrow_import_error)
 def xds_from_parquet(store, columns=None, chunks=None, **kwargs):
 
     # If any kwargs are added, they should be popped prior to this check.
     if len(kwargs) > 0:
         warnings.warn(
             f"The following unsupported kwargs were ignored in "
@@ -240,41 +261,54 @@
 
     # Now create a dataset per partition
     for p, (partition, fragments) in enumerate(sorted(ds_cfg.items())):
         fragments = list(sorted(fragments))
         column_arrays = defaultdict(list)
         fragment_rows = [f.metadata.num_rows for f in fragments]
 
-        for (f, (start, end)) in partition_chunking(p, fragment_rows, chunks):
-            fragment = fragments[f]
-            fragment_meta = fragment.metadata
-            rows = fragment_meta.num_rows
-            schema = fragment_meta.schema.to_arrow_schema()
-            fields = {n: schema.field(n) for n in schema.names}
+        # Returns a dictionary of lists mapping fragments to partitions.
+        partition_chunks = partition_chunking(p, fragment_rows, chunks)
+
+        for pieces in partition_chunks.values():
+
+            chunk_fragments = [fragments[i] for i, _ in pieces]
+            chunk_ranges = [r for _, r in pieces]
+            chunk_metas = [f.metadata for f in chunk_fragments]
+
+            rows = sum(end - start for start, end in chunk_ranges)
+
+            # NOTE(JSKenyon): This assumes that the schema/fields are
+            # consistent between fragments. This should be ok.
+            exemplar_schema = chunk_metas[0].schema.to_arrow_schema()
+            exemplar_fields = {n: exemplar_schema.field(n)
+                               for n in exemplar_schema.names}
 
-            for column, field in column_iterator(fields, columns):
+            for column, field in column_iterator(exemplar_fields, columns):
                 field_metadata = field.metadata[DASKMS_METADATA.encode()]
                 field_metadata = json.loads(field_metadata)
                 dims = tuple(field_metadata["dims"])
 
                 if isinstance(field.type, TensorType):
                     shape = (rows,) + field.type.shape
                 else:
                     shape = (rows,)
 
                 assert len(shape) == len(dims)
 
-                meta = np.empty((0,)*len(dims), field.type.to_pandas_dtype())
+                dtype = field.type.to_pandas_dtype()
+                meta = np.empty((0,)*len(dims), dtype)
                 new_axes = {d: s for d, s in zip(dims, shape)}
 
-                read = da.blockwise(fragment.read_column, dims,
+                read = da.blockwise(fragment_reader, dims,
+                                    chunk_fragments, None,
+                                    chunk_ranges, None,
                                     column, None,
-                                    start, None,
-                                    end, None,
-                                    adjust_chunks={"row": end - start},
+                                    shape, None,
+                                    dtype, None,
+                                    adjust_chunks={"row": rows},
                                     new_axes=new_axes,
                                     meta=meta)
 
                 column_arrays[column].append((read, dims))
 
         data_vars = {}
```

### Comparing `dask-ms-0.2.8/daskms/experimental/zarr/tests/test_zarr.py` & `dask-ms-0.2.9/daskms/experimental/zarr/tests/test_zarr.py`

 * *Files 14% similar despite different names*

```diff
@@ -246,7 +246,43 @@
 
     # We need >10 datasets to be sure roundtripping is consistent.
     xdsl = [Dataset({'x': (('y',), da.ones(i))}) for i in range(1, 12)]
     dask.compute(xds_to_zarr(xdsl, path))
 
     xdsl = xds_from_zarr(path)
     dask.compute(xds_to_zarr(xdsl, path))
+
+
+@pytest.mark.skipif(xarray is None, reason="depends on xarray")
+@pytest.mark.parametrize("prechunking", [{"row": -1, "chan": -1},
+                                         {"row": 1, "chan": 1},
+                                         {"row": 2, "chan": 7}])
+@pytest.mark.parametrize("postchunking", [{"row": -1, "chan": -1},
+                                          {"row": 1, "chan": 1},
+                                          {"row": 2, "chan": 7}])
+def test_rechunking(ms, tmp_path_factory, prechunking, postchunking):
+    store = tmp_path_factory.mktemp("zarr_store")
+    ref_datasets = xds_from_ms(ms)
+
+    for i, ds in enumerate(ref_datasets):
+        chunks = ds.chunks
+        row = sum(chunks["row"])
+        chan = sum(chunks["chan"])
+        corr = sum(chunks["corr"])
+
+        ref_datasets[i] = ds.assign_coords(
+            row=np.arange(row),
+            chan=np.arange(chan),
+            corr=np.arange(corr)
+        )
+
+    chunked_datasets = [ds.chunk(prechunking) for ds in ref_datasets]
+    dask.compute(xds_to_zarr(chunked_datasets, store))
+
+    rechunked_datasets = [ds.chunk(postchunking)
+                          for ds in xds_from_zarr(store)]
+    dask.compute(xds_to_zarr(rechunked_datasets, store, rechunk=True))
+
+    rechunked_datasets = xds_from_zarr(store)
+
+    assert all([ds.equals(rds)
+                for ds, rds in zip(rechunked_datasets, ref_datasets)])
```

### Comparing `dask-ms-0.2.8/daskms/experimental/zarr/tests/conftest.py` & `dask-ms-0.2.9/daskms/experimental/zarr/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/daskms/experimental/zarr/__init__.py` & `dask-ms-0.2.9/daskms/experimental/zarr/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     promote_columns)
 from daskms.optimisation import inlined_array
 from daskms.utils import requires
 from daskms.fsspec_store import DaskMSStore
 
 try:
     import zarr
+    import zarr.convenience as zc
 except ImportError as e:
     zarr_import_error = e
 else:
     zarr_import_error = None
 
 
 DASKMS_ATTR_KEY = "__daskms_zarr_attr__"
@@ -83,27 +84,14 @@
 
     array = ds_group.require_dataset(column, column_schema.shape,
                                      chunks=zchunks,
                                      dtype=column_schema.dtype,
                                      object_codec=codec,
                                      exact=True)
 
-    if zchunks is not None:
-        # Expand zarr chunks to full dask resolution
-        # For comparison purposes
-        zchunks = normalize_chunks(array.chunks, column_schema.shape)
-
-        if zchunks != chunks:
-            raise ValueError(
-                f"zarr chunks {zchunks} "
-                f"don't match dask chunks {column_schema.chunks}. "
-                f"This can cause data corruption as described in "
-                f"https://zarr.readthedocs.io/en/stable/tutorial.html"
-                f"#parallel-computing-and-synchronization")
-
     array.attrs[DASKMS_ATTR_KEY] = {
         "dims": column_schema.dims,
         "coordinate": coordinate,
         "array_type": encode_type(column_schema.type),
     }
 
 
@@ -131,14 +119,49 @@
         **schema.attrs,
         DASKMS_ATTR_KEY: {"chunks": dict(dataset.chunks)}
     })
 
     return ds_group
 
 
+def maybe_rechunk(dataset, group, rechunk=False):
+
+    for field in (*dataset.data_vars.keys(), *dataset.coords.keys()):
+        zarr_array = group.get(field)
+        shape = zarr_array.shape
+        disk_chunks = normalize_chunks(zarr_array.chunks, shape)
+        dask_chunks = dataset[field].chunks
+
+        if dask_chunks and (dask_chunks != disk_chunks):
+            if rechunk:
+                dataset = dataset.assign(
+                    {field: dataset[field].chunk(disk_chunks)}
+                )
+            else:
+                raise ValueError(
+                    f"On disk (zarr) chunks: {disk_chunks} - don't match in "
+                    f"memory (dask) chunks: {dask_chunks}. This can cause "
+                    f"data corruption as described in "
+                    f"https://zarr.readthedocs.io/en/stable/tutorial.html"
+                    f"#parallel-computing-and-synchronization. Consider "
+                    f"setting 'rechunk=True' in 'xds_to_zarr'.")
+
+    try:
+        dataset.chunks
+    except ValueError as e:
+        raise e
+
+    # This makes the attributes consistent with the final chunking.
+    group.attrs.update({
+        DASKMS_ATTR_KEY: {"chunks": dict(dataset.chunks)}
+    })
+
+    return dataset, group
+
+
 def zarr_setter(data, name, group, *extents):
     try:
         zarray = getattr(group, name)
     except AttributeError:
         raise ValueError(f"{name} is not a variable of {group}")
 
     selection = tuple(slice(start, end) for start, end in extents)
@@ -184,28 +207,32 @@
         dims = [f"_{d}_" for d in var.dims] if indirect_dims else var.dims
 
         yield name, (dims, write, var.attrs)
 
 
 @requires("pip install dask-ms[zarr] for zarr support",
           zarr_import_error)
-def xds_to_zarr(xds, store, columns=None):
+def xds_to_zarr(xds, store, columns=None, rechunk=False):
     """
     Stores a dataset of list of datasets defined by `xds` in
     file location `store`.
 
     Parameters
     ----------
     xds : Dataset or list of Datasets
         Data
     store : str or Path
         Path to store the data
     columns : list of str or str or None
         Columns to store. `None` or `"ALL"` stores all columns on each dataset.
-        Otherwise, a list of columns should be supplied.
+        Otherwise, a list of columns should be supplied. All coordinates
+        associated with a specified column will be written automatically.
+    rechunk : bool
+        Controls whether dask arrays should be automatically rechunked to be
+        consistent with existing on-disk zarr arrays while writing to disk.
 
     Returns
     -------
     writes : Dataset
         A Dataset representing the write operations
     """
     if isinstance(store, DaskMSStore):
@@ -227,20 +254,27 @@
             raise TypeError("xds must be a Dataset or list of Datasets")
     else:
         raise TypeError("xds must be a Dataset or list of Datasets")
 
     write_datasets = []
 
     for di, ds in enumerate(xds):
-        group = prepare_zarr_group(di, ds, store)
 
         data_vars, coords = select_vars_and_coords(ds, columns)
-        data_vars = dict(_gen_writes(data_vars, ds.chunks, group))
+
+        # Create a new ds which is consistent with what we want to write.
+        ds = Dataset(data_vars, coords=coords, attrs=ds.attrs)
+
+        group = prepare_zarr_group(di, ds, store)
+
+        ds, group = maybe_rechunk(ds, group, rechunk=rechunk)
+
+        data_vars = dict(_gen_writes(ds.data_vars, ds.chunks, group))
         # Include coords in the write dataset so they're reified
-        data_vars.update(dict(_gen_writes(coords, ds.chunks, group,
+        data_vars.update(dict(_gen_writes(ds.coords, ds.chunks, group,
                                           indirect_dims=True)))
 
         # Transfer any partition information over to the write dataset
         partition = ds.attrs.get(DASKMS_PARTITION_KEY, False)
 
         if not partition:
             attrs = None
@@ -250,15 +284,19 @@
 
         write_datasets.append(Dataset(data_vars, attrs=attrs))
 
     return write_datasets
 
 
 def zarr_getter(zarray, *extents):
-    return zarray[tuple(slice(start, end) for start, end in extents)]
+    if any([start == end for start, end in extents]):  # Empty slice.
+        shape = [start - end for start, end in extents]
+        return np.empty(shape, dtype=zarray.dtype)
+    else:
+        return zarray[tuple(slice(start, end) for start, end in extents)]
 
 
 def group_sortkey(element):
     return int(element[0].split('_')[-1])
 
 
 @requires("pip install dask-ms[zarr] for zarr support",
@@ -314,15 +352,18 @@
         chunks = [chunks]
     else:
         raise TypeError("chunks must be None, a dict or a list of dicts")
 
     datasets = []
     numpy_vars = []
 
-    table_group = zarr.open(store.map)[store.table]
+    # NOTE(JSKenyon): Iterating over all the zarr groups/arrays is VERY
+    # expensive if the metadata has not been consolidated.
+    zc.consolidate_metadata(store.map)
+    table_group = zarr.open_consolidated(store.map)[store.table]
 
     for g, (group_name, group) in enumerate(sorted(table_group.groups(),
                                                    key=group_sortkey)):
         group_attrs = decode_attr(dict(group.attrs))
         dask_ms_attrs = group_attrs.pop(DASKMS_ATTR_KEY)
         natural_chunks = dask_ms_attrs["chunks"]
         group_chunks = {d: tuple(dc) for d, dc in natural_chunks.items()}
```

### Comparing `dask-ms-0.2.8/daskms/conftest.py` & `dask-ms-0.2.9/daskms/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -265,19 +265,21 @@
 
     data_dir = tmp_path_factory.mktemp("data")
     args = [str(server_path), "server",
             str(data_dir), f"--address={MINIO_URL.netloc}"]
 
     # Start the server process and read a line from stdout so that we know
     # it's started
-    ctx = multiprocessing.get_context("spawn")  # noqa
     server_process = Popen(args, shell=False, stdout=PIPE, stderr=PIPE)
-    server_process.stdout.readline()
 
     try:
+        while line := server_process.stdout.readline():
+            if "Documentation: ".encode("utf-8") in line:
+                break
+
         retcode = server_process.poll()
 
         if retcode is not None:
             raise ValueError(f"Server failed to start "
                              f"with return code {retcode}")
 
         yield server_process
```

### Comparing `dask-ms-0.2.8/daskms/utils.py` & `dask-ms-0.2.9/daskms/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 
 from collections import OrderedDict
 import logging
 from pathlib import PurePath, Path
 import re
 import time
+import inspect
+import warnings
 
 from dask.utils import funcname
 # The numpy module may disappear during interpreter shutdown
 # so explicitly import ndarray
 from numpy import ndarray
 
 from daskms.testing import in_pytest
@@ -206,7 +208,25 @@
             return wrapper
     else:
         # Return original function as is
         def decorator(fn):
             return fn
 
     return decorator
+
+
+def filter_kwargs(func, kwargs):
+    """Filters unhandled kwargs and raises appropriate warnings."""
+
+    known_args = inspect.getfullargspec(func).args
+
+    unhandled_kwargs = [k for k in kwargs.keys() if k not in known_args]
+
+    for unhandled_kwarg in unhandled_kwargs:
+        kwargs.pop(unhandled_kwarg)
+
+    if unhandled_kwargs:
+        warnings.warn(
+            f"The following kwargs will be ignored in {func.__name__}: "
+            f"{unhandled_kwargs}.",
+            UserWarning,
+        )
```

### Comparing `dask-ms-0.2.8/daskms/dataset.py` & `dask-ms-0.2.9/daskms/dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -261,15 +261,15 @@
                 self._coords = {}
 
             self._attrs = attrs or {}
 
         @property
         def attrs(self):
             """ Dataset attributes """
-            return Frozen(self._attrs)
+            return self._attrs
 
         @property
         def dims(self):
             """ A :code:`{dim: size}` dictionary """
             return data_var_dims(self._data_vars)
 
         sizes = dims
@@ -327,17 +327,15 @@
             Returns
             -------
             :class:`~daskms.dataset.Dataset`
                 Dataset containing existing variables combined with
                 those in \*\*kwargs.
             """
             data_vars = self._data_vars.copy()
-
-            for k, v in kwargs.items():
-                data_vars[k] = v
+            data_vars.update(**kwargs)
 
             return Dataset(data_vars,
                            attrs=self._attrs.copy(),
                            coords=self._coords)
 
         def assign_coords(self, **kwargs):
             r"""
@@ -407,14 +405,30 @@
             dataset : Dataset
                 New dataset without the specified variables
             """
             data_vars = self._drop_internal(self.data_vars, names, errors)
             coords = self._drop_internal(self.coords, names, errors)
             return Dataset(data_vars, coords=coords, attrs=self.attrs.copy())
 
+        def __getitem__(self, name):
+            try:
+                return self._data_vars[name]
+            except KeyError:
+                pass
+
+            try:
+                return self._coords[name]
+            except KeyError:
+                pass
+
+            try:
+                return self._attrs[name]
+            except KeyError:
+                raise AttributeError(f"Invalid item {name}")
+
         def __getattr__(self, name):
             try:
                 return self._data_vars[name]
             except KeyError:
                 pass
 
             try:
```

### Comparing `dask-ms-0.2.8/daskms/query.py` & `dask-ms-0.2.9/daskms/query.py`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/LICENSE` & `dask-ms-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/PKG-INFO` & `dask-ms-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-ms
-Version: 0.2.8
+Version: 0.2.9
 Summary: xarray Datasets from CASA Tables.
 Home-page: http://github.com/ska-sa/dask-ms
 Author: Simon Perkins
 Author-email: sperkins@ska.ac.za
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,16 +28,16 @@
 ================================
 xarray Datasets from CASA Tables
 ================================
 
 .. image:: https://img.shields.io/pypi/v/dask-ms.svg
         :target: https://pypi.python.org/pypi/dask-ms
 
-.. image:: https://img.shields.io/travis/ska-sa/dask-ms.svg
-        :target: https://travis-ci.org/ska-sa/dask-ms
+.. image:: https://github.com/ratt-ru/dask-ms/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ratt-ru/dask-ms/actions/workflows/ci.yml
 
 .. image:: https://readthedocs.org/projects/dask-ms/badge/?version=latest
         :target: https://dask-ms.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 Constructs xarray_ ``Datasets`` from CASA Tables via python-casacore_.
 The ``Variables`` contained in the ``Dataset`` are dask_ arrays backed by
```

### Comparing `dask-ms-0.2.8/CONTRIBUTING.rst` & `dask-ms-0.2.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dask-ms-0.2.8/README.rst` & `dask-ms-0.2.9/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 ================================
 xarray Datasets from CASA Tables
 ================================
 
 .. image:: https://img.shields.io/pypi/v/dask-ms.svg
         :target: https://pypi.python.org/pypi/dask-ms
 
-.. image:: https://img.shields.io/travis/ska-sa/dask-ms.svg
-        :target: https://travis-ci.org/ska-sa/dask-ms
+.. image:: https://github.com/ratt-ru/dask-ms/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ratt-ru/dask-ms/actions/workflows/ci.yml
 
 .. image:: https://readthedocs.org/projects/dask-ms/badge/?version=latest
         :target: https://dask-ms.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 Constructs xarray_ ``Datasets`` from CASA Tables via python-casacore_.
 The ``Variables`` contained in the ``Dataset`` are dask_ arrays backed by
```

### Comparing `dask-ms-0.2.8/dask_ms.egg-info/SOURCES.txt` & `dask-ms-0.2.9/dask_ms.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -73,12 +73,13 @@
 daskms/tests/test_github.py
 daskms/tests/test_ms_creation.py
 daskms/tests/test_ms_read_and_update.py
 daskms/tests/test_optimisation.py
 daskms/tests/test_optional.py
 daskms/tests/test_ordering.py
 daskms/tests/test_patterns.py
+daskms/tests/test_storage.py
 daskms/tests/test_stress.py
 daskms/tests/test_table.py
 daskms/tests/test_table_proxy.py
 daskms/tests/test_table_schemas.py
 daskms/tests/test_utils.py
```

### Comparing `dask-ms-0.2.8/dask_ms.egg-info/PKG-INFO` & `dask-ms-0.2.9/dask_ms.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-ms
-Version: 0.2.8
+Version: 0.2.9
 Summary: xarray Datasets from CASA Tables.
 Home-page: http://github.com/ska-sa/dask-ms
 Author: Simon Perkins
 Author-email: sperkins@ska.ac.za
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -28,16 +28,16 @@
 ================================
 xarray Datasets from CASA Tables
 ================================
 
 .. image:: https://img.shields.io/pypi/v/dask-ms.svg
         :target: https://pypi.python.org/pypi/dask-ms
 
-.. image:: https://img.shields.io/travis/ska-sa/dask-ms.svg
-        :target: https://travis-ci.org/ska-sa/dask-ms
+.. image:: https://github.com/ratt-ru/dask-ms/actions/workflows/ci.yml/badge.svg
+        :target: https://github.com/ratt-ru/dask-ms/actions/workflows/ci.yml
 
 .. image:: https://readthedocs.org/projects/dask-ms/badge/?version=latest
         :target: https://dask-ms.readthedocs.io/en/latest/?badge=latest
         :alt: Documentation Status
 
 Constructs xarray_ ``Datasets`` from CASA Tables via python-casacore_.
 The ``Variables`` contained in the ``Dataset`` are dask_ arrays backed by
```

