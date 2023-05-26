# Comparing `tmp/in-dbt-spark-1.2.514.tar.gz` & `tmp/in-dbt-spark-1.2.515.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.2.514.tar", last modified: Mon May 15 09:28:26 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.2.515.tar", last modified: Fri May 26 06:37:21 2023, max compression
```

## Comparing `in-dbt-spark-1.2.514.tar` & `in-dbt-spark-1.2.515.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.292834 in-dbt-spark-1.2.514/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-15 09:28:26.292834 in-dbt-spark-1.2.514/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.284834 in-dbt-spark-1.2.514/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.284834 in-dbt-spark-1.2.514/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.288834 in-dbt-spark-1.2.514/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11220 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.288834 in-dbt-spark-1.2.514/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    24549 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.284834 in-dbt-spark-1.2.514/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.288834 in-dbt-spark-1.2.514/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.288834 in-dbt-spark-1.2.514/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/apply_retention.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.292834 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.292834 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.292834 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 09:28:26.292834 in-dbt-spark-1.2.514/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-15 09:28:26.000000 in-dbt-spark-1.2.514/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-15 09:28:26.000000 in-dbt-spark-1.2.514/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:28:26.000000 in-dbt-spark-1.2.514/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 09:28:26.000000 in-dbt-spark-1.2.514/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-15 09:28:26.000000 in-dbt-spark-1.2.514/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-15 09:28:26.000000 in-dbt-spark-1.2.514/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 09:28:26.292834 in-dbt-spark-1.2.514/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-15 09:28:14.000000 in-dbt-spark-1.2.514/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.196196 in-dbt-spark-1.2.515/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-26 06:37:21.196196 in-dbt-spark-1.2.515/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.188196 in-dbt-spark-1.2.515/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.188196 in-dbt-spark-1.2.515/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.192196 in-dbt-spark-1.2.515/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12119 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.192196 in-dbt-spark-1.2.515/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24626 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.188196 in-dbt-spark-1.2.515/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.192196 in-dbt-spark-1.2.515/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.192196 in-dbt-spark-1.2.515/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.196196 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.196196 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.196196 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:37:21.196196 in-dbt-spark-1.2.515/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-26 06:37:21.000000 in-dbt-spark-1.2.515/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-26 06:37:21.000000 in-dbt-spark-1.2.515/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:37:21.000000 in-dbt-spark-1.2.515/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:37:21.000000 in-dbt-spark-1.2.515/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-26 06:37:21.000000 in-dbt-spark-1.2.515/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-26 06:37:21.000000 in-dbt-spark-1.2.515/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 06:37:21.196196 in-dbt-spark-1.2.515/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-26 06:37:09.000000 in-dbt-spark-1.2.515/setup.py
```

### Comparing `in-dbt-spark-1.2.514/PKG-INFO` & `in-dbt-spark-1.2.515/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.514
+Version: 1.2.515
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.514 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.515 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.514/README.md` & `in-dbt-spark-1.2.515/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/client.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -184,18 +184,17 @@
         session_request = SetuSessionRequest(dependency=dependency, config=config)
         logger.info(f"Session create request body : \n {session_request.to_json()}")
         session_request = SetuSessionRequest(dependency=dependency, config=config)
         logger.info(f"Session create request body : \n {session_request.to_json()}")
         try:
             data = self._client.post("/sessions", data=json.loads(session_request.to_json()))
         except requests.HTTPError as e:
-            logger.exception(
-                f"Failed while creating Spark Interactive session : {session_request.to_json()}",
-                e,
-            )
+            logger.error("Failed while creating Spark Interactive session with error:")
+            logger.error(e.response.text)
+            logger.exception(f"Failed while creating Spark Interactive session with error {e}")
             raise
         return Session.from_json(data)
 
     def get_session(self, session_id: str) -> Optional[Session]:
         """
         Get information about a specific session.
         :param session_id: The ID of the session.
@@ -206,14 +205,36 @@
             logger.exception(f"Failed to get the Setu session with id {session_id}", e)
             if e.response.status_code == 404:
                 return None
             else:
                 raise
         return Session.from_json(data)
 
+    def get_log(self, session_id: str):
+        """
+        Get information about spark-submit yarn logs regarding specific session.
+        :param session_id: The ID of the session.
+        """
+        try:
+            data = self._client.get(f"/sessions/{session_id}/log")
+        except requests.HTTPError as e:
+            logger.error(
+                f"Failed to fetch spark submit logs from Setu with session id {session_id}"
+            )
+            if e.response.status_code == 404:
+                logger.error(f"Session {session_id} not found.")
+            else:
+                # Logging log API response
+                logger.error(f"Setu /log API failed with error: {e}")
+
+            # Not raising an exception at DBT end in case failed to fetch logs
+            return None
+
+        return "\n".join(data["logs"])
+
     def cancel_session(self, session_id: str) -> None:
         """
         Cancels the session (kills the respective spark app). The session resource itself will not be deleted,
         and will be available for a few days so users can access logs and get job info. (internal config).
         :param session_id: The ID of the session.
         """
         try:
```

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/models.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,20 +94,22 @@
     BUSY = "busy"
     SHUTTING_DOWN = "shutting_down"
     ERROR = "error"
     DEAD = "dead"
     KILLED = "killed"
     SUCCESS = "success"
     SUBMITTING = "submitting"
+    SUBMITTED = "submitted"
 
 
 SESSION_STATE_NOT_READY = {
     SessionState.NOT_STARTED,
     SessionState.STARTING,
     SessionState.SUBMITTING,
+    SessionState.SUBMITTED,
 }
 SESSION_INVALID_STATE = {
     SessionState.ERROR,
     SessionState.DEAD,
     SessionState.KILLED,
 }
 SESSION_STATE_FINISHED = {
@@ -133,14 +135,15 @@
     session_id: str
     session_name: str
     session_owner: str
     proxy_user: str
     state: SessionState
     application_id: str
     app_info: Optional[SessionAppInfo]
+    diagnostics: str
 
     @classmethod
     def from_json(cls, data: dict) -> "Session":
         if data["appInfo"] is None:
             output = None
         else:
             output = SessionAppInfo.from_json(data["appInfo"])
@@ -148,14 +151,15 @@
             data["id"],
             data["name"],
             data["owner"],
             data["proxyUser"],
             SessionState(data["state"]),
             data["appId"],
             output,
+            data["diagnostics"],
         )
 
 
 @dataclass
 class SessionInitializationConfig:
     proxy_user: str
     jars: List[str]
```

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/session.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/session.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         session_id: str,
         auth: Auth = None,
         verify: Verify = False,
     ) -> None:
         self.client = SetuClient(url, auth, verify)
         self.session_id = session_id
         self.url = url
+        self.diagnostics = "No diagnostics available."
 
     def __enter__(self) -> "SetuSession":
         self.wait_till_ready()
         return self
 
     def __exit__(self, exc_type, exc_value, traceback) -> None:
         self.close()
@@ -55,25 +56,33 @@
             interval = next(intervals)
             logger.info(
                 f"Waiting to get spark resources for setu session - {self.session_id}, current state - {self.state.value}"
             )
             logger.info(f"Sleeping for {interval} seconds..")
             time.sleep(interval)
         if self.state in SESSION_INVALID_STATE:
+            # Log setu submit error for dead state
+            if self.state == SessionState.DEAD:
+                logger.error(self.client.get_log(self.session_id))
+            logger.error(f"Unable to create setu session with {self.session_id} with error:")
+            logger.error(self.diagnostics)
             raise dbt.exceptions.RuntimeException(
                 f" Setu session state = {self.state} Unable to create setu session with {self.session_id}"
             )
         self.print_session_details()
 
     @property
     def state(self) -> SessionState:
         """The state of the managed SETU session."""
         session = self.client.get_session(self.session_id)
         if session is None:
             raise dbt.exceptions.RuntimeException("session not found - it may have been shut down")
+
+        if session.state in SESSION_INVALID_STATE:
+            self.diagnostics = session.diagnostics
         return session.state
 
     def cursor(self) -> SetuStatementCursor:
         """create new SETU statement"""
         return SetuStatementCursor(session_id=self.session_id, client=self.client)
 
     def close(self):
```

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/session_cursor.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/session_manager.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.2.515/dbt/adapters/setu/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/spark/column.py` & `in-dbt-spark-1.2.515/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.2.515/dbt/adapters/spark/connections.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,14 +499,15 @@
                         creds,
                         ["schema", "session_name", "proxy_user"],
                     )
                     if not creds.url:
                         connection.credentials.url = SetuCluster(
                             connection.credentials.cluster
                         ).get_url()
+
                     setu_session = SetuSessionManager.create_session(
                         url=creds.url,
                         proxy_user=creds.proxy_user,
                         queue=creds.queue,
                         execution_tags=creds.execution_tags,
                         metadata=creds.metadata,
                         enable_ssl=creds.use_ssl,
@@ -558,15 +559,17 @@
                         f"set to true.\n\tRetrying in "
                         f"{creds.connect_timeout} seconds "
                         f"({i} of {creds.connect_retries})"
                     )
                     logger.warning(msg)
                     time.sleep(creds.connect_timeout)
                 else:
-                    raise dbt.exceptions.FailedToConnectException("failed to connect") from e
+                    raise dbt.exceptions.FailedToConnectException(
+                        "Failed to connect with error: {}".format(str(e))
+                    ) from e
         else:
             raise exc
 
         connection.handle = handle
         connection.state = ConnectionState.OPEN
         return connection
```

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.2.515/dbt/adapters/spark/impl.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.2.515/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/adapters/spark/session.py` & `in-dbt-spark-1.2.515/dbt/adapters/spark/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from types import TracebackType
 from typing import Any, List, Optional, Tuple
 
 from dbt.events import AdapterLogger
 from dbt.utils import DECIMALS
 from pyspark.sql import DataFrame, Row, SparkSession
 
-
 logger = AdapterLogger("Spark")
 NUMBERS = DECIMALS + (int, float)
 
 
 class Cursor:
     """
     Mock a pyodbc cursor.
```

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/adapters.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/apply_retention.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/apply_retention.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/seed.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/table.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/materializations/validate.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/materializations/validate.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.2.515/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.2.515/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.2.515/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.514
+Version: 1.2.515
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.514 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.515 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.514/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.2.515/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.514/setup.py` & `in-dbt-spark-1.2.515/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.2.514"
+package_version = "1.2.515"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.16.0",
```

