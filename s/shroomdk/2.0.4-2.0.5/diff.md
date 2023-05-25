# Comparing `tmp/shroomdk-2.0.4.tar.gz` & `tmp/shroomdk-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shroomdk-2.0.4.tar", last modified: Mon May  8 14:20:04 2023, max compression
+gzip compressed data, was "shroomdk-2.0.5.tar", last modified: Thu May 25 23:48:59 2023, max compression
```

## Comparing `shroomdk-2.0.4.tar` & `shroomdk-2.0.5.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.609377 shroomdk-2.0.4/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.4/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.4/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-08 14:20:04.609459 shroomdk-2.0.4/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.4/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-08 14:18:06.000000 shroomdk-2.0.4/VERSION
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.4/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.4/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-08 14:20:04.610061 shroomdk-2.0.4/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.4/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.574897 shroomdk-2.0.4/shroomdk/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.576531 shroomdk-2.0.4/shroomdk/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2982 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.576749 shroomdk-2.0.4/shroomdk/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.577286 shroomdk-2.0.4/shroomdk/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.578474 shroomdk-2.0.4/shroomdk/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.579245 shroomdk-2.0.4/shroomdk/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.580480 shroomdk-2.0.4/shroomdk/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.580664 shroomdk-2.0.4/shroomdk/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.580794 shroomdk-2.0.4/shroomdk/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.581100 shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.581292 shroomdk-2.0.4/shroomdk/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.582352 shroomdk-2.0.4/shroomdk/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.583202 shroomdk-2.0.4/shroomdk/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.575633 shroomdk-2.0.4/shroomdk.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-08 14:20:04.000000 shroomdk-2.0.4/shroomdk.egg-info/top_level.txt
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.572122 shroomdk-2.0.4/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.584210 shroomdk-2.0.4/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.584329 shroomdk-2.0.4/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.585143 shroomdk-2.0.4/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.586716 shroomdk-2.0.4/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.594529 shroomdk-2.0.4/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.606954 shroomdk-2.0.4/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:18:06.000000 shroomdk-2.0.4/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.607497 shroomdk-2.0.4/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.607885 shroomdk-2.0.4/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.608473 shroomdk-2.0.4/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.608766 shroomdk-2.0.4/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.609018 shroomdk-2.0.4/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:20:04.609259 shroomdk-2.0.4/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.4/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.634222 shroomdk-2.0.5/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 shroomdk-2.0.5/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 shroomdk-2.0.5/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-25 23:48:59.634309 shroomdk-2.0.5/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 shroomdk-2.0.5/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-25 23:47:03.000000 shroomdk-2.0.5/VERSION
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 shroomdk-2.0.5/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 shroomdk-2.0.5/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-25 23:48:59.634830 shroomdk-2.0.5/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 shroomdk-2.0.5/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.621820 shroomdk-2.0.5/shroomdk/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.623085 shroomdk-2.0.5/shroomdk/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2982 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.623205 shroomdk-2.0.5/shroomdk/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.624755 shroomdk-2.0.5/shroomdk/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.625603 shroomdk-2.0.5/shroomdk/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.626373 shroomdk-2.0.5/shroomdk/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.627664 shroomdk-2.0.5/shroomdk/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.627853 shroomdk-2.0.5/shroomdk/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.627963 shroomdk-2.0.5/shroomdk/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.628261 shroomdk-2.0.5/shroomdk/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.628454 shroomdk-2.0.5/shroomdk/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.628661 shroomdk-2.0.5/shroomdk/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.628851 shroomdk-2.0.5/shroomdk/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.622400 shroomdk-2.0.5/shroomdk.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-25 23:48:59.000000 shroomdk-2.0.5/shroomdk.egg-info/top_level.txt
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.619660 shroomdk-2.0.5/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.629502 shroomdk-2.0.5/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-09 02:05:09.000000 shroomdk-2.0.5/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.629612 shroomdk-2.0.5/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.630065 shroomdk-2.0.5/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:47:03.000000 shroomdk-2.0.5/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.630832 shroomdk-2.0.5/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.631615 shroomdk-2.0.5/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.632918 shroomdk-2.0.5/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:18:06.000000 shroomdk-2.0.5/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:47:03.000000 shroomdk-2.0.5/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.633112 shroomdk-2.0.5/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.633229 shroomdk-2.0.5/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.633515 shroomdk-2.0.5/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.633708 shroomdk-2.0.5/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.633903 shroomdk-2.0.5/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:59.634103 shroomdk-2.0.5/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 shroomdk-2.0.5/src/utils/sleep.py
```

### Comparing `shroomdk-2.0.4/LICENSE.txt` & `shroomdk-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/PKG-INFO` & `shroomdk-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.4
+Version: 2.0.5
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shroomdk-2.0.4/README.md` & `shroomdk-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/setup.py` & `shroomdk-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/errors/api_error.py` & `shroomdk-2.0.5/shroomdk/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/errors/query_run_errors.py` & `shroomdk-2.0.5/shroomdk/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/flipside.py` & `shroomdk-2.0.5/shroomdk/flipside.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.5/shroomdk/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.5/shroomdk/integrations/query_integration/query_result_set_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,30 @@
         self.sqlStatementId = query_run.sqlStatementId
         self.dataSourceId = query_run.dataSourceId
         self.errorName = query_run.errorName
         self.errorMessage = query_run.errorMessage
         self.errorData = query_run.errorData
         self.dataSourceQueryId = query_run.dataSourceQueryId
         self.dataSourceSessionId = query_run.dataSourceSessionId
+        self.page = query_result.page
         self.path = query_run.path
 
         self.run_stats = self.compute_run_stats(query_run)
         self.records = self.create_records()
 
     def build(self) -> QueryResultSet:
         return QueryResultSet(
             query_id=self.query_id,
             status=self.status,
             columns=self.columns,
             column_types=self.column_types,
             rows=self.rows,
             run_stats=self.run_stats,
             records=self.records,
+            page=self.page,
             error=None,
         )
 
     def compute_run_stats(self, query_run: QueryRun) -> QueryRunStats:
         if (
             not query_run.startedAt
             or not query_run.endedAt
```

### Comparing `shroomdk-2.0.4/shroomdk/models/compass/cancel_query_run.py` & `shroomdk-2.0.5/shroomdk/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/compass/core/query_run.py` & `shroomdk-2.0.5/shroomdk/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/compass/create_query_run.py` & `shroomdk-2.0.5/shroomdk/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/compass/get_query_run.py` & `shroomdk-2.0.5/shroomdk/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/compass/get_query_run_results.py` & `shroomdk-2.0.5/shroomdk/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/compass/get_sql_statement.py` & `shroomdk-2.0.5/shroomdk/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/compass/query_results.py` & `shroomdk-2.0.5/shroomdk/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/query.py` & `shroomdk-2.0.5/shroomdk/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/query_defaults.py` & `shroomdk-2.0.5/shroomdk/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/query_result_set.py` & `shroomdk-2.0.5/shroomdk/models/query_result_set.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, List, Union
 
 from pydantic import BaseModel, Field
 
+from .compass.core.page_stats import PageStats
 from .query_run_stats import QueryRunStats
 
 
 class QueryResultSet(BaseModel):
     query_id: Union[str, None] = Field(None, description="The server id of the query")
 
     status: str = Field(
@@ -21,8 +22,11 @@
     run_stats: Union[QueryRunStats, None] = Field(
         None,
         description="Summary stats on the query run (i.e. the number of rows returned, the elapsed time, etc)",
     )
     records: Union[List[Any], None] = Field(
         None, description="The results of the query transformed as an array of objects"
     )
+    page: Union[PageStats, None] = Field(
+        None, description="Summary of page stats for this query result set"
+    )
     error: Any
```

### Comparing `shroomdk-2.0.4/shroomdk/models/query_run_stats.py` & `shroomdk-2.0.5/shroomdk/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/models/query_status.py` & `shroomdk-2.0.5/shroomdk/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/rpc.py` & `shroomdk-2.0.5/shroomdk/rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.5/shroomdk/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.5/shroomdk/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/tests/models/test_query_status.py` & `shroomdk-2.0.5/shroomdk/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/tests/test_rpc.py` & `shroomdk-2.0.5/shroomdk/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/tests/utils/test_sleep.py` & `shroomdk-2.0.5/shroomdk/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk/utils/sleep.py` & `shroomdk-2.0.5/shroomdk/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/shroomdk.egg-info/PKG-INFO` & `shroomdk-2.0.5/shroomdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shroomdk
-Version: 2.0.4
+Version: 2.0.5
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `shroomdk-2.0.4/shroomdk.egg-info/SOURCES.txt` & `shroomdk-2.0.5/shroomdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/errors/api_error.py` & `shroomdk-2.0.5/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/errors/query_run_errors.py` & `shroomdk-2.0.5/src/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/integrations/query_integration/compass_query_integration.py` & `shroomdk-2.0.5/src/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/integrations/query_integration/query_result_set_builder.py` & `shroomdk-2.0.5/src/integrations/query_integration/query_result_set_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,28 +17,30 @@
         self.sqlStatementId = query_run.sqlStatementId
         self.dataSourceId = query_run.dataSourceId
         self.errorName = query_run.errorName
         self.errorMessage = query_run.errorMessage
         self.errorData = query_run.errorData
         self.dataSourceQueryId = query_run.dataSourceQueryId
         self.dataSourceSessionId = query_run.dataSourceSessionId
+        self.page = query_result.page
         self.path = query_run.path
 
         self.run_stats = self.compute_run_stats(query_run)
         self.records = self.create_records()
 
     def build(self) -> QueryResultSet:
         return QueryResultSet(
             query_id=self.query_id,
             status=self.status,
             columns=self.columns,
             column_types=self.column_types,
             rows=self.rows,
             run_stats=self.run_stats,
             records=self.records,
+            page=self.page,
             error=None,
         )
 
     def compute_run_stats(self, query_run: QueryRun) -> QueryRunStats:
         if (
             not query_run.startedAt
             or not query_run.endedAt
```

### Comparing `shroomdk-2.0.4/src/models/compass/cancel_query_run.py` & `shroomdk-2.0.5/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/compass/core/query_run.py` & `shroomdk-2.0.5/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/compass/create_query_run.py` & `shroomdk-2.0.5/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/compass/get_query_run.py` & `shroomdk-2.0.5/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/compass/get_query_run_results.py` & `shroomdk-2.0.5/src/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/compass/get_sql_statement.py` & `shroomdk-2.0.5/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/compass/query_results.py` & `shroomdk-2.0.5/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/query.py` & `shroomdk-2.0.5/src/models/query.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/query_defaults.py` & `shroomdk-2.0.5/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/query_result_set.py` & `shroomdk-2.0.5/src/models/query_result_set.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import Any, List, Union
 
 from pydantic import BaseModel, Field
 
+from .compass.core.page_stats import PageStats
 from .query_run_stats import QueryRunStats
 
 
 class QueryResultSet(BaseModel):
     query_id: Union[str, None] = Field(None, description="The server id of the query")
 
     status: str = Field(
@@ -21,8 +22,11 @@
     run_stats: Union[QueryRunStats, None] = Field(
         None,
         description="Summary stats on the query run (i.e. the number of rows returned, the elapsed time, etc)",
     )
     records: Union[List[Any], None] = Field(
         None, description="The results of the query transformed as an array of objects"
     )
+    page: Union[PageStats, None] = Field(
+        None, description="Summary of page stats for this query result set"
+    )
     error: Any
```

### Comparing `shroomdk-2.0.4/src/models/query_run_stats.py` & `shroomdk-2.0.5/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/models/query_status.py` & `shroomdk-2.0.5/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/tests/integrations/query_integration/test_query_compass_integration.py` & `shroomdk-2.0.5/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `shroomdk-2.0.5/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/tests/models/test_query_status.py` & `shroomdk-2.0.5/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/tests/test_rpc.py` & `shroomdk-2.0.5/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/tests/utils/test_sleep.py` & `shroomdk-2.0.5/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `shroomdk-2.0.4/src/utils/sleep.py` & `shroomdk-2.0.5/src/utils/sleep.py`

 * *Files identical despite different names*

