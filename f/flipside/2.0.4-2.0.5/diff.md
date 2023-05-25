# Comparing `tmp/flipside-2.0.4.tar.gz` & `tmp/flipside-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipside-2.0.4.tar", last modified: Mon May  8 14:19:38 2023, max compression
+gzip compressed data, was "flipside-2.0.5.tar", last modified: Thu May 25 23:48:35 2023, max compression
```

## Comparing `flipside-2.0.4.tar` & `flipside-2.0.5.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.071953 flipside-2.0.4/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 flipside-2.0.4/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 flipside-2.0.4/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-08 14:19:38.072028 flipside-2.0.4/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 flipside-2.0.4/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-08 14:18:06.000000 flipside-2.0.4/VERSION
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.057876 flipside-2.0.4/flipside/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.059495 flipside-2.0.4/flipside/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2982 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.059664 flipside-2.0.4/flipside/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.060182 flipside-2.0.4/flipside/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.061309 flipside-2.0.4/flipside/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.062166 flipside-2.0.4/flipside/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.063619 flipside-2.0.4/flipside/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.063824 flipside-2.0.4/flipside/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.064035 flipside-2.0.4/flipside/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.064322 flipside-2.0.4/flipside/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.064582 flipside-2.0.4/flipside/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.064822 flipside-2.0.4/flipside/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.065062 flipside-2.0.4/flipside/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-08 14:19:37.000000 flipside-2.0.4/flipside/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.058570 flipside-2.0.4/flipside.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-08 14:19:38.000000 flipside-2.0.4/flipside.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-08 14:19:38.000000 flipside-2.0.4/flipside.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-08 14:19:38.000000 flipside-2.0.4/flipside.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-08 14:19:38.000000 flipside-2.0.4/flipside.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-08 14:19:38.000000 flipside-2.0.4/flipside.egg-info/top_level.txt
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 flipside-2.0.4/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 flipside-2.0.4/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-08 14:19:38.072558 flipside-2.0.4/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 flipside-2.0.4/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.055453 flipside-2.0.4/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.065909 flipside-2.0.4/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 flipside-2.0.4/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-02 18:10:35.000000 flipside-2.0.4/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 flipside-2.0.4/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 flipside-2.0.4/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 flipside-2.0.4/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 flipside-2.0.4/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.066015 flipside-2.0.4/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 flipside-2.0.4/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.066531 flipside-2.0.4/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 flipside-2.0.4/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 flipside-2.0.4/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 flipside-2.0.4/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3570 2023-05-02 18:10:35.000000 flipside-2.0.4/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.067489 flipside-2.0.4/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.068659 flipside-2.0.4/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.070348 flipside-2.0.4/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:18:06.000000 flipside-2.0.4/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1031 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 flipside-2.0.4/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.070610 flipside-2.0.4/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.070719 flipside-2.0.4/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.071054 flipside-2.0.4/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.071279 flipside-2.0.4/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.071515 flipside-2.0.4/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 flipside-2.0.4/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-08 14:19:38.071795 flipside-2.0.4/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.4/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 flipside-2.0.4/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.104070 flipside-2.0.5/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 flipside-2.0.5/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 flipside-2.0.5/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-25 23:48:35.104171 flipside-2.0.5/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 flipside-2.0.5/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-25 23:47:03.000000 flipside-2.0.5/VERSION
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.090803 flipside-2.0.5/flipside/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.092750 flipside-2.0.5/flipside/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2982 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.092874 flipside-2.0.5/flipside/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.093362 flipside-2.0.5/flipside/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.094148 flipside-2.0.5/flipside/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.094930 flipside-2.0.5/flipside/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.096226 flipside-2.0.5/flipside/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.096418 flipside-2.0.5/flipside/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.096534 flipside-2.0.5/flipside/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.096819 flipside-2.0.5/flipside/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.097023 flipside-2.0.5/flipside/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.097268 flipside-2.0.5/flipside/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.097483 flipside-2.0.5/flipside/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.091799 flipside-2.0.5/flipside.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/top_level.txt
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 flipside-2.0.5/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 flipside-2.0.5/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-25 23:48:35.104442 flipside-2.0.5/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 flipside-2.0.5/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.088416 flipside-2.0.5/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.098382 flipside-2.0.5/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-09 02:05:09.000000 flipside-2.0.5/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.098500 flipside-2.0.5/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 flipside-2.0.5/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.098968 flipside-2.0.5/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 flipside-2.0.5/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 flipside-2.0.5/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 flipside-2.0.5/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:47:03.000000 flipside-2.0.5/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.099743 flipside-2.0.5/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.100533 flipside-2.0.5/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.102584 flipside-2.0.5/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:18:06.000000 flipside-2.0.5/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:47:03.000000 flipside-2.0.5/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.102781 flipside-2.0.5/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.102908 flipside-2.0.5/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.103214 flipside-2.0.5/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.103441 flipside-2.0.5/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.103685 flipside-2.0.5/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.103924 flipside-2.0.5/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 flipside-2.0.5/src/utils/sleep.py
```

### Comparing `flipside-2.0.4/LICENSE.txt` & `flipside-2.0.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/PKG-INFO` & `flipside-2.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipside
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

### Comparing `flipside-2.0.4/README.md` & `flipside-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/errors/api_error.py` & `flipside-2.0.5/flipside/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/errors/query_run_errors.py` & `flipside-2.0.5/flipside/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/flipside.py` & `flipside-2.0.5/flipside/flipside.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/integrations/query_integration/compass_query_integration.py` & `flipside-2.0.5/flipside/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/integrations/query_integration/query_result_set_builder.py` & `flipside-2.0.5/flipside/integrations/query_integration/query_result_set_builder.py`

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

### Comparing `flipside-2.0.4/flipside/models/compass/cancel_query_run.py` & `flipside-2.0.5/flipside/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/compass/core/query_run.py` & `flipside-2.0.5/flipside/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/compass/create_query_run.py` & `flipside-2.0.5/flipside/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/compass/get_query_run.py` & `flipside-2.0.5/flipside/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/compass/get_query_run_results.py` & `flipside-2.0.5/flipside/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/compass/get_sql_statement.py` & `flipside-2.0.5/flipside/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/compass/query_results.py` & `flipside-2.0.5/flipside/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/query.py` & `flipside-2.0.5/flipside/models/query.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/query_defaults.py` & `flipside-2.0.5/flipside/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/query_result_set.py` & `flipside-2.0.5/flipside/models/query_result_set.py`

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

### Comparing `flipside-2.0.4/flipside/models/query_run_stats.py` & `flipside-2.0.5/flipside/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/models/query_status.py` & `flipside-2.0.5/flipside/models/query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/rpc.py` & `flipside-2.0.5/flipside/rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/tests/integrations/query_integration/test_query_compass_integration.py` & `flipside-2.0.5/flipside/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/tests/integrations/query_integration/test_query_result_set_builder.py` & `flipside-2.0.5/flipside/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/tests/models/test_query_status.py` & `flipside-2.0.5/flipside/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/tests/test_rpc.py` & `flipside-2.0.5/flipside/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/tests/utils/test_sleep.py` & `flipside-2.0.5/flipside/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside/utils/sleep.py` & `flipside-2.0.5/flipside/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/flipside.egg-info/PKG-INFO` & `flipside-2.0.5/flipside.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipside
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

### Comparing `flipside-2.0.4/flipside.egg-info/SOURCES.txt` & `flipside-2.0.5/flipside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/setup.py` & `flipside-2.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/errors/api_error.py` & `flipside-2.0.5/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/errors/query_run_errors.py` & `flipside-2.0.5/src/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/integrations/query_integration/compass_query_integration.py` & `flipside-2.0.5/src/integrations/query_integration/compass_query_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/integrations/query_integration/query_result_set_builder.py` & `flipside-2.0.5/src/integrations/query_integration/query_result_set_builder.py`

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

### Comparing `flipside-2.0.4/src/models/compass/cancel_query_run.py` & `flipside-2.0.5/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/compass/core/query_run.py` & `flipside-2.0.5/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/compass/create_query_run.py` & `flipside-2.0.5/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/compass/get_query_run.py` & `flipside-2.0.5/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/compass/get_query_run_results.py` & `flipside-2.0.5/src/models/compass/get_query_run_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/compass/get_sql_statement.py` & `flipside-2.0.5/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/compass/query_results.py` & `flipside-2.0.5/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/query.py` & `flipside-2.0.5/src/models/query.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/query_defaults.py` & `flipside-2.0.5/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/query_result_set.py` & `flipside-2.0.5/src/models/query_result_set.py`

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

### Comparing `flipside-2.0.4/src/models/query_run_stats.py` & `flipside-2.0.5/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/models/query_status.py` & `flipside-2.0.5/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/tests/integrations/query_integration/test_query_compass_integration.py` & `flipside-2.0.5/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `flipside-2.0.5/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/tests/models/test_query_status.py` & `flipside-2.0.5/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/tests/test_rpc.py` & `flipside-2.0.5/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/tests/utils/test_sleep.py` & `flipside-2.0.5/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.4/src/utils/sleep.py` & `flipside-2.0.5/src/utils/sleep.py`

 * *Files identical despite different names*

