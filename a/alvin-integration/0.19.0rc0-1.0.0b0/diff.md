# Comparing `tmp/alvin_integration-0.19.0rc0.tar.gz` & `tmp/alvin_integration-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alvin_integration-0.19.0rc0.tar", last modified: Fri May 26 20:49:18 2023, max compression
+gzip compressed data, was "alvin_integration-1.0.0b0.tar", last modified: Thu Apr 28 09:57:34 2022, max compression
```

## Comparing `alvin_integration-0.19.0rc0.tar` & `alvin_integration-1.0.0b0.tar`

### file list

```diff
@@ -1,66 +1,86 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/
--rw-r--r--   0 runner    (1001) docker     (123)    34522 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.560430 alvin_integration-0.19.0rc0/alvin_integration/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/adapter.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.560430 alvin_integration-0.19.0rc0/alvin_integration/installer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/installer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4933 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/installer/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.560430 alvin_integration-0.19.0rc0/alvin_integration/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/interfaces/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.560430 alvin_integration-0.19.0rc0/alvin_integration/producers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.560430 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10168 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.560430 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/alvin_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     8854 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/extractors/bigquery.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/extractors/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4111 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/extractors/snowflake.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/patch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17652 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/patch/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/patch/functions_214.py
--rw-r--r--   0 runner    (1001) docker     (123)     4249 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/patch/functions_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/pipeline/dag_metadata_current.py
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/pipeline/dag_metadata_legacy.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/pipeline/extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2614 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/installer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/lineage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/lineage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/lineage/alvin_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/lineage/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/lineage/extractors/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/lineage/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/lineage/extractors/bigquery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/patch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/patch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9801 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/patch/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3035 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/patch/functions_144.py
--rw-r--r--   0 runner    (1001) docker     (123)     2915 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/alvin_integration/producers/dbt/patch/functions_legacy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 20:49:18.560430 alvin_integration-0.19.0rc0/alvin_integration.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-26 20:49:18.000000 alvin_integration-0.19.0rc0/alvin_integration.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-26 20:49:18.000000 alvin_integration-0.19.0rc0/alvin_integration.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 20:49:18.000000 alvin_integration-0.19.0rc0/alvin_integration.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-26 20:49:18.000000 alvin_integration-0.19.0rc0/alvin_integration.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-26 20:49:18.000000 alvin_integration-0.19.0rc0/alvin_integration.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-26 20:48:52.000000 alvin_integration-0.19.0rc0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 20:49:18.564431 alvin_integration-0.19.0rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-26 20:49:17.000000 alvin_integration-0.19.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.516459 alvin_integration-1.0.0b0/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.508458 alvin_integration-1.0.0b0/.git-hooks/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      312 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/.git-hooks/commit-msg
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.508458 alvin_integration-1.0.0b0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.508458 alvin_integration-1.0.0b0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/.github/workflows/on_push_feature_branch.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1902 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1253 2022-04-28 09:57:33.000000 alvin_integration-1.0.0b0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     1440 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-04-28 09:57:34.516459 alvin_integration-1.0.0b0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      484 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/installer/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/installer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4292 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/installer/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      424 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/interfaces/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2207 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/producers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6357 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)      344 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/installer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/alvin_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3330 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/extractors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4246 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/extractors/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1971 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/extractors/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4080 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/extractors/snowflake.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/patch/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/patch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    15189 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/patch/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4042 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/patch/functions_legacy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)     1383 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/pipeline/dag_metadata_current.py
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/pipeline/dag_metadata_legacy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1433 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/alvin_integration/producers/airflow/pipeline/extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/alvin_integration.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-04-28 09:57:34.000000 alvin_integration-1.0.0b0/alvin_integration.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-04-28 09:57:34.000000 alvin_integration-1.0.0b0/alvin_integration.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-28 09:57:34.000000 alvin_integration-1.0.0b0/alvin_integration.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       42 2022-04-28 09:57:34.000000 alvin_integration-1.0.0b0/alvin_integration.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-04-28 09:57:34.000000 alvin_integration-1.0.0b0/alvin_integration.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      286 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/client-commit-validation.sh
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.508458 alvin_integration-1.0.0b0/docker/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/docker/airflow/
+-rw-r--r--   0 runner    (1001) docker     (121)     1019 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/docker/airflow/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/docker/airflow/Dockerfile.legacy
+-rw-r--r--   0 runner    (1001) docker     (121)     3325 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/docker/airflow/docker-compose.legacy.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)    10806 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/docker/airflow/docker-compose.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)      972 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/git-conventional-commits.json
+-rw-r--r--   0 runner    (1001) docker     (121)    33769 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/poetry.lock
+-rw-r--r--   0 runner    (1001) docker     (121)      823 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-04-28 09:57:34.516459 alvin_integration-1.0.0b0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      466 2022-04-28 09:57:32.000000 alvin_integration-1.0.0b0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.508458 alvin_integration-1.0.0b0/tests/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/tests/http_server/
+-rw-r--r--   0 runner    (1001) docker     (121)      250 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/http_server/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)     1283 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/http_server/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/http_server/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.508458 alvin_integration-1.0.0b0/tests/resources/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.508458 alvin_integration-1.0.0b0/tests/resources/airflow/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.508458 alvin_integration-1.0.0b0/tests/resources/airflow/dags/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/tests/resources/airflow/dags/airflow/
+-rw-r--r--   0 runner    (1001) docker     (121)     1903 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/airflow/bigq_demo.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1629 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/airflow/bigquery_dag_airflow_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3480 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/airflow/dag_alvin_patches.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/airflow/dag_task_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/airflow/snowflake_dag_airflow_v2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1232 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/airflow/snowflake_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/tests/resources/airflow/dags/legacy/
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/legacy/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3505 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/legacy/dag_alvin_patches.py
+-rw-r--r--   0 runner    (1001) docker     (121)      607 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/resources/airflow/dags/legacy/snowflake_dag.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.512459 alvin_integration-1.0.0b0/tests/unit/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-28 09:57:34.516459 alvin_integration-1.0.0b0/tests/unit/airflow/
+-rw-r--r--   0 runner    (1001) docker     (121)      558 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/unit/airflow/test_installer.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-04-28 09:56:43.000000 alvin_integration-1.0.0b0/tests/unit/conftest.py
```

### Comparing `alvin_integration-0.19.0rc0/LICENSE` & `alvin_integration-1.0.0b0/LICENSE`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -654,8 +654,8 @@
 of the code.  There are many ways you could offer source, and different
 solutions will be better for different programs; see section 13 for the
 specific requirements.
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU AGPL, see
-<https://www.gnu.org/licenses/>.
+<https://www.gnu.org/licenses/>.
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/installer/base.py` & `alvin_integration-1.0.0b0/alvin_integration/installer/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,131 +1,115 @@
-import logging
-import traceback
-from typing import List
-
+from alvin_integration.interfaces.config import AbstractProducerConfig
 import gorilla
+import logging
 import pkg_resources
+import traceback
 
-from alvin_integration.helper import AlvinLoggerAdapter, log_verbose
-from alvin_integration.interfaces.config import AbstractProducerConfig
-from alvin_integration.models import AlvinPatch
-
-log = AlvinLoggerAdapter(logging.getLogger(__name__), {})
+log = logging.getLogger(__name__)
 
 
 class AlvinBaseInstaller:
     """
     Class responsible to manage the installation of Alvin
     components in the Producer host environment.
     """
-
     def __init__(self, provider_config: AbstractProducerConfig):
         self.provider_config = provider_config
         self.host_package_map = dict()
 
-    def _load_supported_patches(self) -> List[AlvinPatch]:
-        log.info("Start load_supported_patches")
+    def _load_supported_patches(self):
         """Load patches compatible with host environment."""
-        supported_patches: List[AlvinPatch] = []
+        supported_patches = []
         for patch in self.provider_config.get_patching_list():
-            try:
-                log_verbose(f"Looking at patch: {patch}")
 
-                host_package = self.host_package_map.get(patch.package_name)
+            log.info(f"Looking at patch: {patch}")
 
-                log_verbose(f"Found this package: {host_package}")
+            host_package = self.host_package_map.get(patch.package_name)
+
+            log.info(f"Found this package: {host_package}")
+
+            if host_package.version in patch.supported_versions:
+                supported_patches.append(patch)
+                log.info(f"Adding patch: {patch}")
 
-                if host_package.version in patch.supported_versions:
-                    supported_patches.append(patch)
-                    log_verbose(f"Adding patch: {patch}")
-            except ModuleNotFoundError as err:
-                log_verbose(
-                    f"Error loading patch for destination: {patch.destination_path}: {err}"
-                )
         return supported_patches
 
     def install_patches(self):
         """
         Install patches for compatible with the target
         packages of the host environment
         """
         supported_patches = self._load_supported_patches()
 
-        log.info(f"Installing {len(supported_patches)} patches")
+        log.info(f'Installing {len(supported_patches)} patches')
 
         settings = gorilla.Settings(allow_hit=True)
 
         for patch_config in supported_patches:
             patch = gorilla.Patch(
                 patch_config.destination,
                 patch_config.function.__name__,
                 patch_config.function,
                 settings=settings,
             )
 
-            log_verbose(f"Installing: {patch}")
+            log.info(f'Installing: {patch}')
 
             gorilla.apply(patch)
 
-            log_verbose(
+            log.info(
                 f"Patched {patch.destination.__module__} "
                 f"{patch.destination.__name__} {patch.name}"
             )
 
     def load_host_packages(self):
         """Load host environment packages based on the Producer config"""
         target_packages = self.provider_config.get_target_packages()
-        log_verbose(
-            f"Matching host packages {target_packages} for {self.provider_config.producer_name}"
-        )
+        log.info(f'Matching host packages {target_packages} for {self.provider_config.producer_name}')
         for target_package in target_packages:
             host_package = pkg_resources.get_distribution(target_package)
-            log_verbose(f"Host package match: {host_package}")
+            log.info(f'Host package match: {host_package}')
             if host_package:
                 self.host_package_map[target_package] = host_package
 
     def install_pipelines(self):
         """Install pipelines based on teh Producer config."""
         target_pipelines = self.provider_config.get_target_pipelines()
         for target_pipeline in target_pipelines:
             host_package = self.host_package_map.get(target_pipeline.package_name)
-            log_verbose(f"Host Package {host_package}")
-            log_verbose(f"Target Pipeline {target_pipeline}")
+            log.info(f'Host Package {host_package}')
+            log.info(f'Target Pipeline {target_pipeline}')
             if host_package.version in target_pipeline.supported_versions:
-                log_verbose(f"Installing dag {target_pipeline}")
+                log.info(f'Installing dag {target_pipeline}')
                 pipeline = target_pipeline.function
                 pipeline()
-                log_verbose(f"Pipeline {pipeline} creation executed.")
+                log.info(f'Pipeline {pipeline} creation executed.')
 
     def install_lineage(self):
         """Install lineage components based on the Producer config."""
         lineage_config = self.provider_config.get_lineage_config()
         for config in lineage_config:
             host_package = self.host_package_map.get(config.package_name)
-            log_verbose(f"Lineage: {config}")
-            log_verbose(f"Host Package: {host_package}")
+            log.info(f'Lineage: {config}')
+            log.info(f'Host Package: {host_package}')
             if host_package.version in config.supported_versions:
-                log_verbose(
-                    f"Installing lineage: {config.env_name} - {config.env_value}"
-                )
+                log.info(f'Installing lineage: {config.env_name} - {config.env_value}')
                 config.set_lineage()
-                log_verbose(f"Lineage {config} installed successfully.")
+                log.info(f'Lineage {config} installed successfully.')
 
     def install(self):
         """Install Alvin components in the Producer environment."""
         try:
-            log_verbose("Starting Alvin Integration Package installation.", True)
+            log.info('Starting Alvin Integration Package installation.')
 
             self.load_host_packages()
 
             self.install_patches()
 
             self.install_lineage()
 
             self.install_pipelines()
 
-            log_verbose("Alvin Integration Package completed successfully.", True)
+            log.info('Alvin Integration Package completed successfully.')
 
         except Exception:
-            log_verbose(
-                f"Installation failed with error: {traceback.format_exc()}", True
-            )
+            log.error(f'Installation failed with error: {traceback.format_exc()}')
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/models.py` & `alvin_integration-1.0.0b0/alvin_integration/models.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 This module contains the data models that will be produced
 and sent to the Alvin Backend.
 """
-import importlib
-import os
 from dataclasses import dataclass
 from typing import List
+import importlib
+import os
 
 
 @dataclass
 class AlvinAirflowTaskExecution:
     task_id: str
     dag_id: str
     run_id: str
@@ -95,8 +95,8 @@
     function: any
     supported_versions: List[str]
 
     def __repr__(self):
         return (
             f"function: {self.function}, "
             f"supported_versions: {self.supported_versions}"
-        )
+        )
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/config.py` & `alvin_integration-1.0.0b0/alvin_integration/producers/airflow/config.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,86 +1,56 @@
 import os
-from typing import List
-
-from alvin_integration.interfaces.config import AbstractProducerConfig
-from alvin_integration.models import (
-    AlvinLineageConfig,
-    AlvinPatch,
-    AlvinPipelineCreator,
-)
 from alvin_integration.producers.airflow.patch.functions import (
-    _add_auth,
     _run_finished_callback,
-    get_all_dagmodels,
-    get_client,
-    get_hook,
-    get_or_create_openlineage_client,
-    handle_callback,
     handle_failure,
+    handle_callback,
     pre_execute,
+    get_client,
     run,
-    update_state,
-)
-from alvin_integration.producers.airflow.patch.functions_214 import (
-    update_state as update_state_214,
-)
-from alvin_integration.producers.airflow.patch.functions_legacy import (
-    update_state as update_state_legacy,
-)
-from alvin_integration.producers.airflow.pipeline import (
-    create_alvin_dag_current,
-    create_alvin_dag_google_composer,
-    create_alvin_dag_legacy,
+    get_hook,
+    _add_auth,
+    get_or_create_openlineage_client,
+    update_state
 )
+from alvin_integration.producers.airflow.patch.functions_legacy import update_state as update_state_legacy
+from alvin_integration.producers.airflow.pipeline import create_alvin_dag_current, create_alvin_dag_google_composer, create_alvin_dag_legacy
+from alvin_integration.interfaces.config import AbstractProducerConfig
+from alvin_integration.models import AlvinPatch, AlvinLineageConfig, AlvinPipelineCreator
 
-ALVIN_BACKEND_API_URL = os.getenv("ALVIN_URL")
+ALVIN_BACKEND_API_URL = os.getenv('ALVIN_URL')
 
-ALVIN_BACKEND_API_KEY = os.getenv("ALVIN_API_KEY")
+ALVIN_BACKEND_API_KEY = os.getenv('ALVIN_API_KEY')
 
-GOOGLE_COMPOSER_BUCKET = os.getenv("GCS_BUCKET")
+GOOGLE_COMPOSER_BUCKET = os.getenv('GCS_BUCKET')
 
 
 class AirflowProducerConfig(AbstractProducerConfig):
+
     @property
     def producer_name(self):
-        return "Airflow"
+        return 'Airflow'
 
-    def get_patching_list(self) -> List[AlvinPatch]:
+    def get_patching_list(self):
         return [
             AlvinPatch(
                 package_name="apache-airflow",
                 function=_run_finished_callback,
-                supported_versions=[
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer",
-                ],
+                supported_versions=["2.2.3", "2.2.3+composer"],
                 destination_path="airflow.models.taskinstance.TaskInstance",
             ),
             AlvinPatch(
                 package_name="apache-airflow",
                 function=handle_failure,
                 supported_versions=["1.10.15"],
                 destination_path="airflow.models.taskinstance.TaskInstance",
             ),
             AlvinPatch(
                 package_name="apache-airflow",
                 function=handle_callback,
-                supported_versions=[
-                    "1.10.15",
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer",
-                ],
+                supported_versions=["1.10.15", "2.2.3+composer", "2.2.3"],
                 destination_path="airflow.models.dag.DAG",
             ),
             AlvinPatch(
                 package_name="apache-airflow",
                 function=pre_execute,
                 supported_versions=["1.10.15", "1.10.15+composer"],
                 destination_path="airflow.contrib.operators.bigquery_operator.BigQueryOperator",
@@ -102,166 +72,79 @@
                 function=get_hook,
                 supported_versions=["1.10.15", "1.10.15+composer"],
                 destination_path="airflow.contrib.operators.snowflake_operator.SnowflakeOperator",
             ),
             AlvinPatch(
                 package_name="apache-airflow",
                 function=_add_auth,
-                supported_versions=[
-                    "1.10.15",
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "1.10.15+composer",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer",
-                ],
+                supported_versions=["1.10.15", "1.10.15+composer", "2.2.3", "2.2.3+composer"],
                 destination_path="openlineage.client.OpenLineageClient",
             ),
             AlvinPatch(
                 package_name="apache-airflow",
                 function=get_or_create_openlineage_client,
-                supported_versions=[
-                    "1.10.15",
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "1.10.15+composer",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer",
-                ],
+                supported_versions=["1.10.15", "1.10.15+composer", "2.2.3", "2.2.3+composer"],
                 destination_path="openlineage.airflow.adapter.OpenLineageAdapter",
             ),
             AlvinPatch(
                 package_name="apache-airflow",
                 function=update_state,
-                supported_versions=["2.2.3", "2.2.5", "2.2.3+composer", "2.2.5+composer"],
-                destination_path="airflow.models.dagrun.DagRun",
-            ),
-            AlvinPatch(
-                package_name="apache-airflow",
-                function=update_state_214,
-                supported_versions=["2.1.4", "2.1.4+composer"],
+                supported_versions=["2.2.3", "2.2.3+composer"],
                 destination_path="airflow.models.dagrun.DagRun",
             ),
             AlvinPatch(
                 package_name="apache-airflow",
                 function=update_state_legacy,
-                supported_versions=[
-                    "1.10.15",
-                    "1.10.15+composer",
-                    "2.1.4+composer",
-                ],
+                supported_versions=["1.10.15", "1.10.15+composer"],
                 destination_path="airflow.models.dagrun.DagRun",
-            ),
-            AlvinPatch(
-                package_name="apache-airflow",
-                function=get_all_dagmodels,
-                supported_versions=[
-                    "1.10.15",
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "1.10.15+composer",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer"
-                ],
-                destination_path="airflow.models.dag.DagModel",
-            ),
-        ]
+            )
+            ]
 
     def get_target_packages(self):
-        return ["apache-airflow"]
+        return ['apache-airflow']
 
     def get_target_pipelines(self):
         return [
             AlvinPipelineCreator(
                 package_name="apache-airflow",
                 function=create_alvin_dag_current,
-                supported_versions=["2.1.4", "2.2.3", "2.2.5"],
+                supported_versions=["2.2.3"]
             ),
             AlvinPipelineCreator(
                 package_name="apache-airflow",
                 function=create_alvin_dag_google_composer,
-                supported_versions=["2.1.4+composer", "2.2.3+composer", "2.2.5+composer"],
+                supported_versions=["2.2.3+composer"]
             ),
             AlvinPipelineCreator(
                 package_name="apache-airflow",
                 function=create_alvin_dag_legacy,
-                supported_versions=["1.10.15"],
-            ),
+                supported_versions=["1.10.15"]
+            )
         ]
 
     def get_lineage_config(self):
         return [
-            AlvinLineageConfig(
-                package_name="apache-airflow",
-                env_name="OPENLINEAGE_EXTRACTOR_BigQueryExecuteQueryOperator",
-                env_value="alvin_integration.producers.airflow.lineage.extractors.bigquery.AlvinBigQueryExtractor",
-                supported_versions=[
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer",
-                ],
-            ),
-            AlvinLineageConfig(
-                package_name="apache-airflow",
-                env_name="OPENLINEAGE_EXTRACTOR_BigQueryInsertJobOperator",
-                env_value="alvin_integration.producers.airflow.lineage.extractors.bigquery.AlvinBigQueryExtractor",
-                supported_versions=[
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer"
-                ],
-            ),
-            # We have some customers that still use the BigQueryOperator on Airflow V2
-            # also what is interesting is that the AlvinBigQueryExtractor in Airflow V2 uses similar
-            # attributes as the BigQueryInsertJobOperator, like gcp_conn_id instead of bigquery_conn_id
-            # so we have to use the AlvinBigQueryExtractor instead of the AlvinBigQueryLegacyExtractor one.
-            AlvinLineageConfig(
-                package_name="apache-airflow",
-                env_name="OPENLINEAGE_EXTRACTOR_BigQueryOperator",
-                env_value="alvin_integration.producers.airflow.lineage.extractors.bigquery.AlvinBigQueryExtractor",
-                supported_versions=[
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer"
-                ],
-            ),
-            AlvinLineageConfig(
-                package_name="apache-airflow",
-                env_name="OPENLINEAGE_EXTRACTOR_BigQueryOperator",
-                env_value="alvin_integration.producers.airflow.lineage.extractors.bigquery.AlvinBigQueryLegacyExtractor",
-                supported_versions=["1.10.15", "1.10.15+composer"],
-            ),
-            AlvinLineageConfig(
-                package_name="apache-airflow",
-                env_name="OPENLINEAGE_EXTRACTOR_SnowflakeOperator",
-                env_value="alvin_integration.producers.airflow.lineage.extractors.snowflake.AlvinSnowflakeLegacyExtractor",
-                supported_versions=["1.10.15", "1.10.15+composer"],
-            ),
-            AlvinLineageConfig(
-                package_name="apache-airflow",
-                env_name="OPENLINEAGE_EXTRACTOR_SnowflakeOperator",
-                env_value="alvin_integration.producers.airflow.lineage.extractors.snowflake.AlvinSnowflakeExtractor",
-                supported_versions=[
-                    "2.1.4",
-                    "2.2.3",
-                    "2.2.5",
-                    "2.1.4+composer",
-                    "2.2.3+composer",
-                    "2.2.5+composer"
-                ],
-            ),
-        ]
+                AlvinLineageConfig(
+                    package_name="apache-airflow",
+                    env_name="OPENLINEAGE_EXTRACTOR_BigQueryExecuteQueryOperator",
+                    env_value="alvin_integration.producers.airflow.lineage.extractors.bigquery.AlvinBigQueryExtractor",
+                    supported_versions=["2.2.3", "2.2.3+composer"],
+                ),
+                AlvinLineageConfig(
+                    package_name="apache-airflow",
+                    env_name="OPENLINEAGE_EXTRACTOR_BigQueryOperator",
+                    env_value="alvin_integration.producers.airflow.lineage.extractors.bigquery.AlvinBigQueryLegacyExtractor",
+                    supported_versions=["1.10.15", "1.10.15+composer"],
+                ),
+                AlvinLineageConfig(
+                    package_name="apache-airflow",
+                    env_name="OPENLINEAGE_EXTRACTOR_SnowflakeOperator",
+                    env_value="alvin_integration.producers.airflow.lineage.extractors.snowflake.AlvinSnowflakeLegacyExtractor",
+                    supported_versions=["1.10.15", "1.10.15+composer"],
+                ),
+                AlvinLineageConfig(
+                    package_name="apache-airflow",
+                    env_name="OPENLINEAGE_EXTRACTOR_SnowflakeOperator",
+                    env_value="alvin_integration.producers.airflow.lineage.extractors.snowflake.AlvinSnowflakeExtractor",
+                    supported_versions=["2.2.3", "2.2.3+composer"],
+                ),
+            ]
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/extractors/mixins.py` & `alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/extractors/mixins.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,67 +1,60 @@
 import os
 from dataclasses import asdict
-from importlib.metadata import version
 from typing import Optional
-
-from alvin_integration.helper import log_verbose
-from openlineage.airflow.extractors.base import TaskMetadata
-
-from alvin_integration.constants import ALVIN_PACKAGE_NAME
+from openlineage.airflow.extractors.base import (
+    TaskMetadata
+)
 from alvin_integration.models import AlvinAirflowTaskExecution
-
+from importlib.metadata import version
 
 class AlvinAirflowExtractorMixin:
+
     def build_facet(self, task_instance):
         raise NotImplementedError
 
     def build_task_metadata(self, task_instance):
         raise NotImplementedError
 
     def get_airflow_run_id(self, task_instance):
         raise NotImplementedError
 
     def get_connection_id(self):
         raise NotImplementedError
 
     def get_alvin_package_version(self):
-        return version(ALVIN_PACKAGE_NAME)
+        return version('alvin_integration')
 
     def get_alvin_platform_id(self):
-        return os.getenv("ALVIN_PLATFORM_ID")
+        return os.getenv('ALVIN_PLATFORM_ID')
 
     def extract_on_complete(self, task_instance) -> Optional[TaskMetadata]:
-
         if not task_instance:
             return self.extract()
 
         alvin_facet = self.build_facet(task_instance)
 
         task_metadata = self.extract()
 
         if not task_metadata:
             task_metadata = self.build_task_metadata(task_instance)
 
-        log_verbose(f"Alvin Facet: {asdict(alvin_facet)}")
-
         task_metadata.job_facets.update(asdict(alvin_facet))
 
         return task_metadata
 
     def get_execution_details(self, task_instance):
         return AlvinAirflowTaskExecution(
             task_id=task_instance.task_id,
             dag_id=task_instance.dag_id,
             run_id=self.get_airflow_run_id(task_instance),
             start_date=task_instance.start_date.isoformat(),
-            end_date=task_instance.end_date.isoformat()
-            if task_instance.end_date
-            else None,
+            end_date=task_instance.end_date.isoformat() if task_instance.end_date else None,
             duration=task_instance.duration,
             try_number=task_instance.try_number,
             pool=task_instance.pool,
             operator=task_instance.operator,
             state=task_instance.state,
             max_tries=task_instance.max_tries,
             platform_id=self.get_alvin_platform_id(),
-            alvin_package_version=self.get_alvin_package_version(),
+            alvin_package_version=self.get_alvin_package_version()
         )
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/lineage/extractors/snowflake.py` & `alvin_integration-1.0.0b0/alvin_integration/producers/airflow/lineage/extractors/snowflake.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 import logging
-
-from alvin_integration.helper import log_verbose
-from openlineage.airflow.extractors.base import TaskMetadata
 from openlineage.airflow.extractors.snowflake_extractor import SnowflakeExtractor
+from openlineage.common.sql import SqlMeta, SqlParser
+from openlineage.common.dataset import Source, Dataset
 from openlineage.airflow.utils import (
-    get_connection,
     get_normalized_postgres_connection_uri,
-    safe_import_airflow,
+    get_connection, safe_import_airflow
+)
+from openlineage.airflow.extractors.base import (
+    TaskMetadata
 )
 from openlineage.client.facet import SqlJobFacet
-from openlineage.common.dataset import Dataset, Source
-from openlineage.common.sql import SqlMeta, SqlParser
-
 from alvin_integration.models import AlvinFacet, AlvinSnowflakeLineageDetails
-from alvin_integration.producers.airflow.lineage.extractors.mixins import (
-    AlvinAirflowExtractorMixin,
-)
+from alvin_integration.producers.airflow.lineage.extractors.mixins import AlvinAirflowExtractorMixin
+
 
 logger = logging.getLogger(__name__)
 
 
 class AlvinSnowflakeBaseExtractor(AlvinAirflowExtractorMixin, SnowflakeExtractor):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
@@ -31,15 +28,15 @@
         return self.operator.snowflake_conn_id if self.operator else None
 
     def build_facet(self, task_instance):
         return AlvinFacet(
             alvin=AlvinSnowflakeLineageDetails(
                 query_ids=self._get_query_ids(),
                 execution=self.get_execution_details(task_instance),
-                connection_id=self.get_connection_id(),
+                connection_id=self.get_connection_id()
             )
         )
 
     def _get_database(self) -> str:
         return self._get_hook().database
 
     def _get_authority(self) -> str:
@@ -53,73 +50,77 @@
     def _get_hook(self):
         return self.operator.get_db_hook()
 
     def _get_query_ids(self):
         return self.operator.query_ids
 
     def get_airflow_run_id(self, task_instance):
-        return task_instance.get_dagrun().run_id
+        return task_instance.run_id
 
 
 class AlvinSnowflakeLegacyExtractor(AlvinSnowflakeBaseExtractor):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
-        log_verbose("AlvinSnowflakeLegacyExtractor")
+        print('AlvinSnowflakeLegacyExtractor')
 
     def _get_hook(self):
         return self.operator.get_hook()
 
     def extract(self) -> TaskMetadata:
 
         sql_meta: SqlMeta = SqlParser.parse(self.operator.sql, self.default_schema)
 
         self.conn = get_connection(self._conn_id())
 
         source = Source(
             scheme=self._get_scheme(),
             authority=self._get_authority(),
-            connection_url=self._get_connection_uri(),
+            connection_url=self._get_connection_uri()
         )
 
         database = self.operator.database
         if not database:
             database = self._get_database()
 
         inputs = [
             Dataset.from_table(
                 source=source,
                 table_name=in_table_schema.table_name.name,
                 schema_name=in_table_schema.schema_name,
-                database_name=database,
+                database_name=database
+            ) for in_table_schema in self._get_table_schemas(
+                sql_meta.in_tables
             )
-            for in_table_schema in self._get_table_schemas(sql_meta.in_tables)
         ]
         outputs = [
             Dataset.from_table_schema(
-                source=source, table_schema=out_table_schema, database_name=database
+                source=source,
+                table_schema=out_table_schema,
+                database_name=database
+            ) for out_table_schema in self._get_table_schemas(
+                sql_meta.out_tables
             )
-            for out_table_schema in self._get_table_schemas(sql_meta.out_tables)
         ]
         query_ids = self._get_query_ids()
 
         return TaskMetadata(
             name=f"{self.operator.dag_id}.{self.operator.task_id}",
             inputs=[ds.to_openlineage_dataset() for ds in inputs],
             outputs=[ds.to_openlineage_dataset() for ds in outputs],
             job_facets={
-                "sql": SqlJobFacet(self.operator.sql),
-                "queries_ids": query_ids if query_ids else [],
-            },
+                'sql': SqlJobFacet(self.operator.sql),
+                'queries_ids': query_ids if query_ids else []
+            }
         )
 
     def _get_query_ids(self):
         hook = self.operator.get_hook()
-        log_verbose(hook)
-        if hasattr(hook, "query_ids"):
-            log_verbose(f"Query ids found: {hook.query_ids}")
+        print(hook)
+        if hasattr(hook, 'query_ids'):
+            print(f'Query ids found: {hook.query_ids}')
             return hook.query_ids
         else:
-            log_verbose(f"Query ids not found")
+            print(f'Query ids not found')
             return []
 
     def get_airflow_run_id(self, task_instance):
-        return task_instance.get_dagrun().run_id
+        return task_instance.get_dagrun().run_id
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/patch/functions.py` & `alvin_integration-1.0.0b0/alvin_integration/producers/airflow/patch/functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,125 +1,62 @@
 import airflow
 
-
 def _run_finished_callback(self, error=None):
     """
     Alvin patched version of _run_finished_callback from TaskInstance.
 
     This method will inject the call
     to alvin_callback in case the task has failed.
     """
-
-    import logging
-    import traceback
-
-    from airflow.utils.state import State
-
-    from alvin_integration.helper import AlvinLoggerAdapter
     from alvin_integration.producers.airflow.lineage.backend import alvin_callback
-
-    log = AlvinLoggerAdapter(logging.getLogger(__name__), {})
-
-    context = None
-
-    try:
-        # call unpatched function
-        # see for details
-        # https://airflow.apache.org/docs/apache-airflow/2.1.0/_api/airflow/models/taskinstance/index.html#airflow.models.taskinstance.TaskInstance._run_finished_callback
-        if self.state == State.FAILED:
-            task = self.task
-            if task.on_failure_callback is not None:
-                context = self.get_template_context()
-                context["exception"] = error
-                task.on_failure_callback(context)
-        elif self.state == State.SUCCESS:
-            task = self.task
-            if task.on_success_callback is not None:
-                context = self.get_template_context()
-                task.on_success_callback(context)
-        elif self.state == State.UP_FOR_RETRY:
-            task = self.task
-            if task.on_retry_callback is not None:
-                context = self.get_template_context()
-                context["exception"] = error
-                task.on_retry_callback(context)
-    except Exception:
-        log.error(f"Default Callback Error: {traceback.format_exc()}")
-
-    if not context:
-        context = self.get_template_context()
+    context = self.get_template_context()
 
     alvin_callback(context=context, operator=self.task)
 
-def get_all_dagmodels(self, session=None):
-    from airflow.models.dag import DagModel
-    from airflow.utils.session import provide_session
-    
-
-    @provide_session
-    def get_session(session):
-        return session
-
-    if not session:
-        session = get_session()
-
-    return session.query(DagModel).all()
 
 def handle_failure(
-    self,
-    error,
-    test_mode=None,
-    context=None,
-    force_fail=False,
-    session=None,  # noqa
+    self, error, test_mode=None, context=None, force_fail=False, session=None,  # noqa
 ):
     """
     Alvin patched version of handle_failure from TaskInstance.
 
     This method will inject the call
     to alvin_callback in case the task has failed.
     """
-    import logging
-
-    from alvin_integration.helper import AlvinLoggerAdapter
     from alvin_integration.producers.airflow.lineage.backend import alvin_callback
-
-    log = AlvinLoggerAdapter(logging.getLogger(__name__), {})
-
     @airflow.utils.db.provide_session
     def get_session(session):
         return session
 
     if not session:
         session = get_session()
-    from airflow.models.log import Log
-    from airflow.models.taskfail import TaskFail
-    from airflow.settings import Stats
-    from airflow.utils import timezone
     from airflow.utils.state import State
-
+    from airflow.utils import timezone
+    from airflow.settings import Stats
+    from airflow.models.taskfail import TaskFail
+    from airflow.models.log import Log
     if test_mode is None:
         test_mode = self.test_mode
     if context is None:
         context = self.get_template_context()
 
-    log.exception(error)
+    self.log.exception(error)
     task = self.task
     self.end_date = timezone.utcnow()
     self.set_duration()
-    Stats.incr("operator_failures_{}".format(task.__class__.__name__), 1, 1)
-    Stats.incr("ti_failures")
+    Stats.incr('operator_failures_{}'.format(task.__class__.__name__), 1, 1)
+    Stats.incr('ti_failures')
     if not test_mode:
         session.add(Log(State.FAILED, self))
 
     # Log failure duration
     session.add(TaskFail(task, self.execution_date, self.start_date, self.end_date))
 
     if context is not None:
-        context["exception"] = error
+        context['exception'] = error
 
     # Set state correctly and figure out how to log it,
     # what callback to call if any, and how to decide whether to email
 
     # Since this function is called only when the TaskInstance state is running,
     # try_number contains the current try_number (not the next). We
     # only mark task instance as FAILED if the next task instance
@@ -135,37 +72,37 @@
         callback = task.on_failure_callback
     else:
         self.state = State.UP_FOR_RETRY
         log_message = "Marking task as UP_FOR_RETRY."
         email_for_state = task.email_on_retry
         callback = task.on_retry_callback
 
-    log.info(
-        "%s dag_id=%s, task_id=%s, execution_date=%s, start_date=%s, end_date=%s",
+    self.log.info(
+        '%s dag_id=%s, task_id=%s, execution_date=%s, start_date=%s, end_date=%s',
         log_message,
         self.dag_id,
         self.task_id,
-        self._safe_date("execution_date", "%Y%m%dT%H%M%S"),
-        self._safe_date("start_date", "%Y%m%dT%H%M%S"),
-        self._safe_date("end_date", "%Y%m%dT%H%M%S"),
+        self._safe_date('execution_date', '%Y%m%dT%H%M%S'),
+        self._safe_date('start_date', '%Y%m%dT%H%M%S'),
+        self._safe_date('end_date', '%Y%m%dT%H%M%S')
     )
     if email_for_state and task.email:
         try:
             self.email_alert(error)
         except Exception as e2:
-            log.error("Failed to send email to: %s", task.email)
-            log.exception(e2)
+            self.log.error('Failed to send email to: %s', task.email)
+            self.log.exception(e2)
 
     # Handling callbacks pessimistically
     if callback:
         try:
             callback(context)
         except Exception as e3:
-            log.error("Failed at executing callback")
-            log.exception(e3)
+            self.log.error("Failed at executing callback")
+            self.log.exception(e3)
 
     if not test_mode:
         session.merge(self)
     session.commit()
 
     alvin_callback(context=context, operator=self.task, is_airflow_legacy=True)  # noqa
 
@@ -173,21 +110,15 @@
 def handle_callback(self, dagrun, success=True, reason=None, session=None):
     """
     Alvin patched version of handle_callback from DAG.
 
     This method will inject the call
     to alvin_callback in case the task has failed.
     """
-    import logging
-
-    from alvin_integration.helper import AlvinLoggerAdapter
     from alvin_integration.producers.airflow.lineage.backend import alvin_callback
-
-    log = AlvinLoggerAdapter(logging.getLogger(__name__), {})
-
     task_instance_list = dagrun.get_task_instances()
 
     if not success:
         is_airlfow_legacy = True
 
         for ti in task_instance_list:
             ti.task = self.get_task(ti.task_id)
@@ -197,15 +128,15 @@
                 operator=ti.task,
                 is_airflow_legacy=is_airlfow_legacy,  # noqa
             )
 
     callback = self.on_success_callback if success else self.on_failure_callback  # noqa
 
     if callback:
-        log.info("Executing dag callback function: {}".format(callback))
+        self.log.info("Executing dag callback function: {}".format(callback))
         task_instance_list = dagrun.get_task_instances()
         ti = task_instance_list[-1]  # get first TaskInstance of DagRun
         ti.task = self.get_task(ti.task_id)
         context = ti.get_template_context(session=session)
         context.update({"reason": reason})
         callback(context)
 
@@ -240,17 +171,15 @@
 
     This method will create crate a Google Client using the
     reusing the Airflow Google connection.
     """
     from google.cloud.bigquery import Client
 
     return Client(
-        project=project_id,
-        location=location,
-        credentials=self._get_credentials(),
+        project=project_id, location=location, credentials=self._get_credentials(),
     )
 
 
 def run(self, sql, autocommit=False, parameters=None):
     """
     Runs a command or a list of commands. Pass a list of sql
     statements to the sql parameter to get them to execute
@@ -260,137 +189,117 @@
     :type sql: str or list
     :param autocommit: What to set the connection's autocommit setting to
         before executing the query.
     :type autocommit: bool
     :param parameters: The parameters to render the SQL query with.
     :type parameters: mapping or iterable
     """
-    import logging
-    import sys
     from contextlib import closing
-
     from past.builtins import basestring
-
-    from alvin_integration.helper import AlvinLoggerAdapter
-
-    log = AlvinLoggerAdapter(logging.getLogger(__name__), {})
+    import sys
 
     self.query_ids = []
 
     if isinstance(sql, basestring):
         sql = [sql]
 
     with closing(self.get_conn()) as conn:
         if self.supports_autocommit:
             self.set_autocommit(conn, autocommit)
 
         with closing(conn.cursor()) as cur:
             for s in sql:
                 if sys.version_info[0] < 3:
-                    s = s.encode("utf-8")
+                    s = s.encode('utf-8')
                 if parameters is not None:
-                    log.info("{} with parameters {}".format(s, parameters))
+                    self.log.info("{} with parameters {}".format(s, parameters))
                     cur.execute(s, parameters)
                 else:
-                    log.info(s)
+                    self.log.info(s)
                     cur.execute(s)
                 query_id = cur.sfqid
-                log.info("Rows affected: %s", cur.rowcount)
-                log.info("Snowflake query id: %s", query_id)
+                self.log.info("Rows affected: %s", cur.rowcount)
+                self.log.info("Snowflake query id: %s", query_id)
                 self.query_ids.append(query_id)
 
         # If autocommit was set to False for db that supports autocommit,
         # or if db does not supports autocommit, we do a manual commit.
         if not self.get_autocommit(conn):
             conn.commit()
 
 
 def get_hook(self):
     from airflow.contrib.hooks.snowflake_hook import SnowflakeHook
-
-    if not hasattr(self, "hook"):
-        self.hook = SnowflakeHook(
-            snowflake_conn_id=self.snowflake_conn_id,
-            warehouse=self.warehouse,
-            database=self.database,
-            role=self.role,
-            schema=self.schema,
-            authenticator=self.authenticator,
-        )
+    if not hasattr(self, 'hook'):
+        self.hook = SnowflakeHook(snowflake_conn_id=self.snowflake_conn_id,
+                             warehouse=self.warehouse, database=self.database,
+                             role=self.role, schema=self.schema, authenticator=self.authenticator)
     return self.hook
 
 
 def _add_auth(self, api_key: str):
-    if "alvin" in api_key:
-        alvin_api_key = api_key.split("-alvin-")
-        self.session.headers.update({"X-API-KEY": f"{alvin_api_key[1]}"})
+    if 'alvin' in api_key:
+        alvin_api_key = api_key.split('-alvin-')
+        self.session.headers.update({
+            "X-API-KEY": f"{alvin_api_key[1]}"
+        })
     else:
-        self.session.headers.update({"Authorization": f"Bearer {api_key}"})
+        self.session.headers.update({
+            "Authorization": f"Bearer {api_key}"
+        })
 
 
 def get_or_create_openlineage_client(self):
-    import logging
-    import os
-
     from openlineage.client import OpenLineageClient, OpenLineageClientOptions
+    import os, logging
 
-    from alvin_integration.helper import AlvinLoggerAdapter
-
-    log = AlvinLoggerAdapter(logging.getLogger(__name__), {})
+    log = logging.getLogger(__name__)
 
     if not self._client:
-        alvin_url = os.getenv("ALVIN_URL")
-        alvin_api_key = os.getenv("ALVIN_API_KEY")
+        alvin_url = os.getenv('ALVIN_URL')
+        alvin_api_key = os.getenv('ALVIN_API_KEY')
         if alvin_url:
             log.info(f"Sending lineage events to Alvin Backend: {alvin_url}")
-            self._client = OpenLineageClient(
-                alvin_url,
-                OpenLineageClientOptions(api_key=f"key-alvin-{alvin_api_key}"),
-            )
+            self._client = OpenLineageClient(alvin_url, OpenLineageClientOptions(
+                api_key=f'key-alvin-{alvin_api_key}'
+            ))
             return self._client
         # Backcomp with Marquez integration
-        marquez_url = os.getenv("MARQUEZ_URL")
-        marquez_api_key = os.getenv("MARQUEZ_API_KEY")
+        marquez_url = os.getenv('MARQUEZ_URL')
+        marquez_api_key = os.getenv('MARQUEZ_API_KEY')
 
         if marquez_url:
             log.info(f"Sending lineage events to {marquez_url}")
-            self._client = OpenLineageClient(
-                marquez_url, OpenLineageClientOptions(api_key=marquez_api_key)
-            )
+            self._client = OpenLineageClient(marquez_url, OpenLineageClientOptions(
+                api_key=marquez_api_key
+            ))
         else:
             self._client = OpenLineageClient.from_environment()
     return self._client
 
 
-def update_state(self, session=None, execute_callbacks=True):
+def update_state(
+    self, session=None, execute_callbacks=True
+):
     """
     Determines the overall state of the DagRun based on the state
     of its TaskInstances.
     :param session: Sqlalchemy ORM Session
     :type session: Session
     :param execute_callbacks: Should dag callbacks (success/failure, SLA etc) be invoked
         directly (default: true) or recorded as a pending request in the ``callback`` property
     :type execute_callbacks: bool
     :return: Tuple containing tis that can be scheduled in the current loop & `callback` that
         needs to be executed
     """
-    import logging
+    from airflow.utils import callback_requests, timezone
     from typing import Optional
-
     from airflow.stats import Stats
-    from airflow.utils import callback_requests, timezone
     from airflow.utils.state import DagRunState, State, TaskInstanceState
-
-    from alvin_integration.helper import AlvinLoggerAdapter
-    from alvin_integration.producers.airflow.lineage.backend import (
-        alvin_dag_run_extractor,
-    )
-
-    log = AlvinLoggerAdapter(logging.getLogger(__name__), {})
-
+    from alvin_integration.producers.airflow.lineage.backend import alvin_callback, alvin_dag_run_extractor
     # Callback to execute in case of Task Failures
     callback: Optional[callback_requests.DagCallbackRequest] = None
 
     @airflow.utils.session.provide_session
     def get_session(session):
         return session
 
@@ -406,106 +315,91 @@
         tis = info.tis
         schedulable_tis = info.schedulable_tis
         changed_tis = info.changed_tis
         finished_tasks = info.finished_tasks
         unfinished_tasks = info.unfinished_tasks
 
         none_depends_on_past = all(not t.task.depends_on_past for t in unfinished_tasks)
-        none_task_concurrency = all(
-            t.task.max_active_tis_per_dag is None for t in unfinished_tasks
-        )
+        none_task_concurrency = all(t.task.max_active_tis_per_dag is None for t in unfinished_tasks)
         none_deferred = all(t.state != State.DEFERRED for t in unfinished_tasks)
 
-        if (
-            unfinished_tasks
-            and none_depends_on_past
-            and none_task_concurrency
-            and none_deferred
-        ):
+        if unfinished_tasks and none_depends_on_past and none_task_concurrency and none_deferred:
             # small speed up
             are_runnable_tasks = (
                 schedulable_tis
                 or self._are_premature_tis(unfinished_tasks, finished_tasks, session)
                 or changed_tis
             )
 
     leaf_task_ids = {t.task_id for t in dag.leaves}
     leaf_tis = [ti for ti in tis if ti.task_id in leaf_task_ids]
 
     # if all roots finished and at least one failed, the run failed
-    if not unfinished_tasks and any(
-        leaf_ti.state in State.failed_states for leaf_ti in leaf_tis
-    ):
-        log.error("Marking run %s failed", self)
+    if not unfinished_tasks and any(leaf_ti.state in State.failed_states for leaf_ti in leaf_tis):
+        self.log.error('Marking run %s failed', self)
         self.set_state(State.FAILED)
         if execute_callbacks:
-            dag.handle_callback(
-                self, success=False, reason="task_failure", session=session
-            )
+            dag.handle_callback(self, success=False, reason='task_failure', session=session)
         elif dag.has_on_failure_callback:
             callback = callback_requests.DagCallbackRequest(
                 full_filepath=dag.fileloc,
                 dag_id=self.dag_id,
                 run_id=self.run_id,
                 is_failure_callback=True,
-                msg="task_failure",
+                msg='task_failure',
             )
 
     # if all leaves succeeded and no unfinished tasks, the run succeeded
-    elif not unfinished_tasks and all(
-        leaf_ti.state in State.success_states for leaf_ti in leaf_tis
-    ):
-        log.info("Marking run %s successful", self)
+    elif not unfinished_tasks and all(leaf_ti.state in State.success_states for leaf_ti in leaf_tis):
+        self.log.info('Marking run %s successful', self)
         self.set_state(State.SUCCESS)
         if execute_callbacks:
-            dag.handle_callback(self, success=True, reason="success", session=session)
+            dag.handle_callback(self, success=True, reason='success', session=session)
         elif dag.has_on_success_callback:
             callback = callback_requests.DagCallbackRequest(
                 full_filepath=dag.fileloc,
                 dag_id=self.dag_id,
                 run_id=self.run_id,
                 is_failure_callback=False,
-                msg="success",
+                msg='success',
             )
 
     # if *all tasks* are deadlocked, the run failed
     elif (
         unfinished_tasks
         and none_depends_on_past
         and none_task_concurrency
         and none_deferred
         and not are_runnable_tasks
     ):
-        log.error("Deadlock; marking run %s failed", self)
+        self.log.error('Deadlock; marking run %s failed', self)
         self.set_state(State.FAILED)
         if execute_callbacks:
-            dag.handle_callback(
-                self, success=False, reason="all_tasks_deadlocked", session=session
-            )
+            dag.handle_callback(self, success=False, reason='all_tasks_deadlocked', session=session)
         elif dag.has_on_failure_callback:
             callback = callback_requests.DagCallbackRequest(
                 full_filepath=dag.fileloc,
                 dag_id=self.dag_id,
                 run_id=self.run_id,
                 is_failure_callback=True,
-                msg="all_tasks_deadlocked",
+                msg='all_tasks_deadlocked',
             )
 
     # finally, if the roots aren't done, the dag is still running
     else:
         self.set_state(State.RUNNING)
 
     if self._state == State.FAILED or self._state == State.SUCCESS:
         msg = (
             "Alvin DagRun Finished: dag_id=%s, execution_date=%s, run_id=%s, "
             "run_start_date=%s, run_end_date=%s, run_duration=%s, "
             "state=%s, external_trigger=%s, run_type=%s, "
             "data_interval_start=%s, data_interval_end=%s, dag_hash=%s"
         )
-        log.info(
+        self.log.info(
             msg,
             self.dag_id,
             self.execution_date,
             self.run_id,
             self.start_date,
             self.end_date,
             (self.end_date - self.start_date).total_seconds()
@@ -515,14 +409,16 @@
             self.external_trigger,
             self.run_type,
             self.data_interval_start,
             self.data_interval_end,
             self.dag_hash,
         )
 
-    alvin_dag_run_extractor(dag_run=self)
+    alvin_dag_run_extractor(
+       dag_run=self
+    )
     self._emit_true_scheduling_delay_stats_for_finished_state(finished_tasks)
     self._emit_duration_stats_for_finished_state()
 
     session.merge(self)
 
     return schedulable_tis, callback
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/patch/functions_legacy.py` & `alvin_integration-1.0.0b0/alvin_integration/producers/airflow/patch/functions_legacy.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,118 +4,92 @@
 def update_state(self, session=None):
     """
     Determines the overall state of the DagRun based on the state
     of its TaskInstances.
     :return: ready_tis: the tis that can be scheduled in the current loop
     :rtype ready_tis: list[airflow.models.TaskInstance]
     """
-    import logging
-
-    from airflow.settings import Stats
-    from airflow.ti_deps.dep_context import SCHEDULEABLE_STATES
-    from airflow.utils import timezone
     from airflow.utils.state import State
-
-    from alvin_integration.helper import AlvinLoggerAdapter
-    from alvin_integration.producers.airflow.lineage.backend import (
-        alvin_dag_run_extractor,
-    )
-
-    log = AlvinLoggerAdapter(logging.getLogger(__name__), {})
+    from airflow.utils import timezone
+    from airflow.ti_deps.dep_context import SCHEDULEABLE_STATES
+    from alvin_integration.producers.airflow.lineage.backend import alvin_dag_run_extractor
+    from airflow.settings import Stats
 
     @airflow.utils.db.provide_session
     def get_session(session):
         return session
 
     if not session:
         session = get_session()
 
     dag = self.get_dag()
     ready_tis = []
-    tis = [
-        ti
-        for ti in self.get_task_instances(
-            session=session, state=State.task_states + (State.SHUTDOWN,)
-        )
-    ]
-    log.debug("number of tis tasks for %s: %s task(s)", self, len(tis))
+    tis = [ti for ti in self.get_task_instances(session=session,
+                                                state=State.task_states + (State.SHUTDOWN,))]
+    self.log.debug("number of tis tasks for %s: %s task(s)", self, len(tis))
     for ti in list(tis):
         ti.task = dag.get_task(ti.task_id)
 
     start_dttm = timezone.utcnow()
     unfinished_tasks = [t for t in tis if t.state in State.unfinished()]
-    finished_tasks = [
-        t for t in tis if t.state in State.finished() + [State.UPSTREAM_FAILED]
-    ]
+    finished_tasks = [t for t in tis if t.state in State.finished() + [State.UPSTREAM_FAILED]]
     none_depends_on_past = all(not t.task.depends_on_past for t in unfinished_tasks)
-    none_task_concurrency = all(
-        t.task.task_concurrency is None for t in unfinished_tasks
-    )
+    none_task_concurrency = all(t.task.task_concurrency is None
+                                for t in unfinished_tasks)
     # small speed up
     if unfinished_tasks:
-        scheduleable_tasks = [
-            ut for ut in unfinished_tasks if ut.state in SCHEDULEABLE_STATES
-        ]
-        log.debug(
+        scheduleable_tasks = [ut for ut in unfinished_tasks if ut.state in SCHEDULEABLE_STATES]
+        self.log.debug(
             "number of scheduleable tasks for %s: %s task(s)",
-            self,
-            len(scheduleable_tasks),
-        )
-        ready_tis, changed_tis = self._get_ready_tis(
-            scheduleable_tasks, finished_tasks, session
-        )
-        log.debug("ready tis length for %s: %s task(s)", self, len(ready_tis))
+            self, len(scheduleable_tasks))
+        ready_tis, changed_tis = self._get_ready_tis(scheduleable_tasks, finished_tasks, session)
+        self.log.debug("ready tis length for %s: %s task(s)", self, len(ready_tis))
         if none_depends_on_past and none_task_concurrency:
             # small speed up
-            are_runnable_tasks = (
-                ready_tis
-                or self._are_premature_tis(unfinished_tasks, finished_tasks, session)
-                or changed_tis
-            )
+            are_runnable_tasks = ready_tis or self._are_premature_tis(
+                unfinished_tasks, finished_tasks, session) or changed_tis
 
-    duration = timezone.utcnow() - start_dttm
+    duration = (timezone.utcnow() - start_dttm)
     Stats.timing("dagrun.dependency-check.{}".format(self.dag_id), duration)
 
     leaf_task_ids = {t.task_id for t in dag.leaves}
     leaf_tis = [ti for ti in tis if ti.task_id in leaf_task_ids]
 
     # if all roots finished and at least one failed, the run failed
     if not unfinished_tasks and any(
-        leaf_ti.state in {State.FAILED, State.UPSTREAM_FAILED} for leaf_ti in leaf_tis
+            leaf_ti.state in {State.FAILED, State.UPSTREAM_FAILED} for leaf_ti in leaf_tis
     ):
-        log.info("Marking run %s failed", self)
+        self.log.info('Marking run %s failed', self)
         self.set_state(State.FAILED)
-        dag.handle_callback(self, success=False, reason="task_failure", session=session)
+        dag.handle_callback(self, success=False, reason='task_failure',
+                            session=session)
 
     # if all leafs succeeded and no unfinished tasks, the run succeeded
     elif not unfinished_tasks and all(
-        leaf_ti.state in {State.SUCCESS, State.SKIPPED} for leaf_ti in leaf_tis
+            leaf_ti.state in {State.SUCCESS, State.SKIPPED} for leaf_ti in leaf_tis
     ):
-        log.info("Marking run %s successful", self)
+        self.log.info('Marking run %s successful', self)
         self.set_state(State.SUCCESS)
-        dag.handle_callback(self, success=True, reason="success", session=session)
+        dag.handle_callback(self, success=True, reason='success', session=session)
 
     # if *all tasks* are deadlocked, the run failed
-    elif (
-        unfinished_tasks
-        and none_depends_on_past
-        and none_task_concurrency
-        and not are_runnable_tasks
-    ):
-        log.info("Deadlock; marking run %s failed", self)
+    elif (unfinished_tasks and none_depends_on_past and
+          none_task_concurrency and not are_runnable_tasks):
+        self.log.info('Deadlock; marking run %s failed', self)
         self.set_state(State.FAILED)
-        dag.handle_callback(
-            self, success=False, reason="all_tasks_deadlocked", session=session
-        )
+        dag.handle_callback(self, success=False, reason='all_tasks_deadlocked',
+                            session=session)
 
     # finally, if the roots aren't done, the dag is still running
     else:
         self.set_state(State.RUNNING)
 
     self._emit_true_scheduling_delay_stats_for_finished_state(finished_tasks)
     self._emit_duration_stats_for_finished_state()
-    alvin_dag_run_extractor(dag_run=self)
+    alvin_dag_run_extractor(
+        dag_run=self
+    )
     # todo: determine we want to use with_for_update to make sure to lock the run
     session.merge(self)
     session.commit()
 
-    return ready_tis
+    return ready_tis
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/pipeline/__init__.py` & `alvin_integration-1.0.0b0/alvin_integration/producers/airflow/pipeline/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,43 @@
-import inspect
 import os
 import sys
-
 from airflow import settings
-from alvin_integration.helper import log_verbose
+
+import inspect
 
 
 def create_alvin_dag_current():
     from alvin_integration.producers.airflow.pipeline import dag_metadata_current
-
-    create_alvin_dag("alvin_metadata_dag.py", dag_metadata_current)
+    create_alvin_dag('alvin_metadata_dag.py', dag_metadata_current)
 
 
 def create_alvin_dag_legacy():
     from alvin_integration.producers.airflow.pipeline import dag_metadata_legacy
-
-    create_alvin_dag("alvin_metadata_dag.py", dag_metadata_legacy)
+    create_alvin_dag('alvin_metadata_dag.py', dag_metadata_legacy)
 
 
 def create_alvin_dag(file_name, dag_module):
 
-    log_verbose("Creating Alvin DAGs.....", True)
+    print('Creating Alvin DAGs.....')
     dag_folder = settings.DAGS_FOLDER
     dag_source_code = inspect.getsource(sys.modules[dag_module.__name__])
-    with open(os.path.join(dag_folder, file_name), "w") as file:
+    with open(os.path.join(dag_folder, file_name), 'w') as file:
         file.write(dag_source_code)
 
 
 def create_alvin_dag_google_composer():
-    log_verbose(f"Importing dag metadata dependencies.....")
-
-    from google.cloud import storage
-
-    from alvin_integration.producers.airflow.config import GOOGLE_COMPOSER_BUCKET
+    print(f'Importing dag metadata dependencies.....')
     from alvin_integration.producers.airflow.pipeline import dag_metadata_current
+    from alvin_integration.producers.airflow.config import GOOGLE_COMPOSER_BUCKET
+    from gcloud import storage
 
-    log_verbose(
-        f"Creating Alvin DAGs on Google Composer path {GOOGLE_COMPOSER_BUCKET}....."
-    )
+    print(f'Creating Alvin DAGs on Google Composer path {GOOGLE_COMPOSER_BUCKET}.....')
 
     dag_source_code = inspect.getsource(sys.modules[dag_metadata_current.__name__])
 
     client = storage.Client()
 
     bucket = client.get_bucket(GOOGLE_COMPOSER_BUCKET)
 
-    blob = bucket.blob("dags/alvin_metadata_dag.py")
+    blob = bucket.blob('dags/alvin_metadata_dag.py')
 
     blob.upload_from_string(dag_source_code)
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/pipeline/dag_metadata_current.py` & `alvin_integration-1.0.0b0/alvin_integration/producers/airflow/pipeline/dag_metadata_legacy.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,31 @@
-from datetime import datetime, timedelta
-
 from airflow.models import DAG
-from airflow.operators.python import PythonOperator
-from airflow.utils.session import provide_session
-
+from airflow.operators.python_operator import PythonOperator
+from datetime import datetime, timedelta
+from airflow.utils import db
 from alvin_integration.producers.airflow.pipeline.extractor import extract_dag_metadata
 
 seven_days_ago = datetime.combine(
     datetime.today() - timedelta(1), datetime.min.time()
 )  # noqa
 
 args = {
     "owner": "airflow",
     "start_date": seven_days_ago,
 }
 
 
-@provide_session
-def extract_metadata(session):
+@db.provide_session
+def extract_metadata(session, **kwargs):
     """Extract metadata from DAG and send to Alvin Backend API."""
     extract_dag_metadata(session)
 
 
 alvin_metadata_extractor = DAG(
-    dag_id="alvin_metadata_extractor",
-    default_args=args,
-    schedule_interval="@hourly",
-    catchup=False,
+    dag_id="alvin_metadata_extractor", default_args=args, schedule_interval="@hourly", catchup=False
 )  # noqa
 
 task_success_one = PythonOperator(
     task_id="dag_metadata_extractor",
     provide_context=True,
     python_callable=extract_metadata,
     dag=alvin_metadata_extractor,
```

### Comparing `alvin_integration-0.19.0rc0/alvin_integration/producers/airflow/pipeline/dag_metadata_legacy.py` & `alvin_integration-1.0.0b0/alvin_integration/producers/airflow/pipeline/dag_metadata_current.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,32 @@
-from datetime import datetime, timedelta
-
 from airflow.models import DAG
-from airflow.operators.python_operator import PythonOperator
-from airflow.utils import db
-
+from airflow.operators.python import PythonOperator
+from datetime import datetime, timedelta
+from airflow.utils.session import provide_session
 from alvin_integration.producers.airflow.pipeline.extractor import extract_dag_metadata
 
+
 seven_days_ago = datetime.combine(
     datetime.today() - timedelta(1), datetime.min.time()
 )  # noqa
 
 args = {
     "owner": "airflow",
     "start_date": seven_days_ago,
 }
 
 
-@db.provide_session
-def extract_metadata(session, **kwargs):
+@provide_session
+def extract_metadata(session):
     """Extract metadata from DAG and send to Alvin Backend API."""
     extract_dag_metadata(session)
 
 
 alvin_metadata_extractor = DAG(
-    dag_id="alvin_metadata_extractor",
-    default_args=args,
-    schedule_interval="@hourly",
-    catchup=False,
+    dag_id="alvin_metadata_extractor", default_args=args, schedule_interval="@hourly", catchup=False
 )  # noqa
 
 task_success_one = PythonOperator(
     task_id="dag_metadata_extractor",
     provide_context=True,
     python_callable=extract_metadata,
     dag=alvin_metadata_extractor,
```

### Comparing `alvin_integration-0.19.0rc0/pyproject.toml` & `alvin_integration-1.0.0b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,33 @@
 [tool.poetry]
-name = "alvin_integration"
+name = "alvin_airflow"
 version = "0.1.0"
 description = "Package for Alvin implementation of the Airflow Integration."
-authors = ["Alvin <tech@alvin.ai>"]
+authors = ["thcidale0808 <thiago@alvin.ai>"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 docker = "^5.0.3"
 gorilla = "^0.4.0"
-openlineage-airflow = { version = "0.6.1", optional = true }
-dbt-core = { version = "1.2.0", optional = true }
-dbt-bigquery = { version = "1.2.0", optional = true }
+openlineage-airflow = "^0.6.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.0.1"
 flake8 = "^4.0.1"
 black = "^22.1.0"
 isort = "^5.10.1"
 bandit = "^1.7.4"
 
-[tool.poetry.extras]
-airflow = ["openlineage-airflow"]
-dbt = ["dbt-core", "dbt-bigquery"]
-
 [tool.pytest.ini_options]
 filterwarnings = [
     "ignore::DeprecationWarning:.*backports.*:",
     "ignore::DeprecationWarning:.*future.*:",
     "ignore::DeprecationWarning:.*past.*:",
     "ignore::DeprecationWarning:.*pendulum.*:",
 ]
 
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.semantic_release]
-version_variable = 'setup.py:__base_version__'
-tag_commit=false
-patch_without_tag=true
+version_variable = "setup.py:__base_version__"
```

