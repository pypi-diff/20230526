# Comparing `tmp/dbt-bigquery-1.6.0b1.tar.gz` & `tmp/dbt-bigquery-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-bigquery-1.6.0b1.tar", last modified: Fri May 12 20:06:21 2023, max compression
+gzip compressed data, was "dbt-bigquery-1.6.0b2.tar", last modified: Thu May 25 22:00:10 2023, max compression
```

## Comparing `dbt-bigquery-1.6.0b1.tar` & `dbt-bigquery-1.6.0b2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.518346 dbt-bigquery-1.6.0b1/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.518346 dbt-bigquery-1.6.0b1/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    26002 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/gcloud.py
--rw-r--r--   0 runner    (1001) docker     (123)    37860 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/python_submissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/relation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.518346 dbt-bigquery-1.6.0b1/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters/
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/catalog.sql
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/etc.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/copy.sql
--rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.522347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/python_model/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/python_model/python.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/array_append.sql
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/array_concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/array_construct.sql
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/date_trunc.sql
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/except.sql
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/hash.sql
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/intersect.sql
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/position.sql
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/right.sql
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/safe_cast.sql
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/utils/timestamps.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/dbt/include/bigquery/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-12 20:06:21.000000 dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-12 20:06:21.526347 dbt-bigquery-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-12 20:06:04.000000 dbt-bigquery-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.350865 dbt-bigquery-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-25 22:00:10.350865 dbt-bigquery-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.338866 dbt-bigquery-1.6.0b2/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.338866 dbt-bigquery-1.6.0b2/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.342866 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26002 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/gcloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37860 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7624 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/python_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4025 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/relation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.338866 dbt-bigquery-1.6.0b2/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.342866 dbt-bigquery-1.6.0b2/dbt/include/bigquery/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.342866 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.342866 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/adapters/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     8440 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7751 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/catalog.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/etc.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.346866 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/copy.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     7735 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.346866 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/common.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.346866 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/python_model/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/python_model/python.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.350865 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/array_append.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/array_concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/array_construct.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/date_trunc.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/escape_single_quotes.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/except.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/get_columns_spec_ddl.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/hash.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/intersect.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/position.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/right.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/safe_cast.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/utils/timestamps.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/dbt/include/bigquery/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-25 22:00:10.350865 dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-25 22:00:10.000000 dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-05-25 22:00:10.000000 dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 22:00:10.000000 dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-25 22:00:10.000000 dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-25 22:00:10.000000 dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-25 22:00:10.000000 dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-25 22:00:10.350865 dbt-bigquery-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3307 2023-05-25 21:59:58.000000 dbt-bigquery-1.6.0b2/setup.py
```

### Comparing `dbt-bigquery-1.6.0b1/LICENSE.md` & `dbt-bigquery-1.6.0b2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/PKG-INFO` & `dbt-bigquery-1.6.0b2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b1 Summary: The Bigquery
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b2 Summary: The Bigquery
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-bigquery-1.6.0b1/README.md` & `dbt-bigquery-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/__init__.py` & `dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/column.py` & `dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/column.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/connections.py` & `dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/dataset.py` & `dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/dataset.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/gcloud.py` & `dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/gcloud.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/impl.py` & `dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/impl.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/python_submissions.py` & `dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/python_submissions.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/adapters/bigquery/relation.py` & `dbt-bigquery-1.6.0b2/dbt/adapters/bigquery/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters/apply_grants.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/adapters/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/adapters.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/catalog.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/copy.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/copy.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/insert_overwrite.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/merge.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/incremental_strategy/time_ingestion_tables.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/seed.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/table.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/macros/materializations/view.sql` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/macros/materializations/view.sql`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt/include/bigquery/profile_template.yml` & `dbt-bigquery-1.6.0b2/dbt/include/bigquery/profile_template.yml`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/PKG-INFO` & `dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-bigquery
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: The Bigquery adapter plugin for dbt
 Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs
 Author-email: info@dbtlabs.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b1 Summary: The Bigquery
+Metadata-Version: 2.1 Name: dbt-bigquery Version: 1.6.0b2 Summary: The Bigquery
 adapter plugin for dbt Home-page: https://github.com/dbt-labs/dbt-bigquery
 Author: dbt Labs Author-email: info@dbtlabs.com Classifier: Development Status
 :: 5 - Production/Stable Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: Microsoft :: Windows Classifier:
 Operating System :: MacOS :: MacOS X Classifier: Operating System :: POSIX ::
 Linux Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dbt-bigquery-1.6.0b1/dbt_bigquery.egg-info/SOURCES.txt` & `dbt-bigquery-1.6.0b2/dbt_bigquery.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-bigquery-1.6.0b1/setup.py` & `dbt-bigquery-1.6.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     else:
         core_patch = "0"
 
     return f"{major}.{minor}.{core_patch}"
 
 
 package_name = "dbt-bigquery"
-package_version = "1.6.0b1"
+package_version = "1.6.0b2"
 dbt_core_version = _dbt_core_version(_dbt_bigquery_version())
 description = """The BigQuery adapter plugin for dbt"""
 
 setup(
     name="dbt-bigquery",
     version=_dbt_bigquery_version(),
     description="The Bigquery adapter plugin for dbt",
```

