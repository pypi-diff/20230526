# Comparing `tmp/flipside-2.0.5.tar.gz` & `tmp/flipside-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flipside-2.0.5.tar", last modified: Thu May 25 23:48:35 2023, max compression
+gzip compressed data, was "flipside-2.0.7.tar", last modified: Fri May 26 02:51:31 2023, max compression
```

## Comparing `flipside-2.0.5.tar` & `flipside-2.0.7.tar`

### file list

```diff
@@ -1,144 +1,144 @@
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.104070 flipside-2.0.5/
--rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 flipside-2.0.5/LICENSE.txt
--rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 flipside-2.0.5/MANIFEST.in
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-25 23:48:35.104171 flipside-2.0.5/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 flipside-2.0.5/README.md
--rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-25 23:47:03.000000 flipside-2.0.5/VERSION
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.090803 flipside-2.0.5/flipside/
--rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.092750 flipside-2.0.5/flipside/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/errors/server_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2982 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/flipside.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.092874 flipside-2.0.5/flipside/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.093362 flipside-2.0.5/flipside/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.094148 flipside-2.0.5/flipside/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.094930 flipside-2.0.5/flipside/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.096226 flipside-2.0.5/flipside/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/models/sleep_config.py
--rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/rpc.py
--rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/shroomdk.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.096418 flipside-2.0.5/flipside/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.096534 flipside-2.0.5/flipside/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.096819 flipside-2.0.5/flipside/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.097023 flipside-2.0.5/flipside/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.097268 flipside-2.0.5/flipside/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.097483 flipside-2.0.5/flipside/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-25 23:48:34.000000 flipside-2.0.5/flipside/utils/sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.091799 flipside-2.0.5/flipside.egg-info/
--rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/PKG-INFO
--rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/SOURCES.txt
--rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/dependency_links.txt
--rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/requires.txt
--rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-25 23:48:35.000000 flipside-2.0.5/flipside.egg-info/top_level.txt
--rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 flipside-2.0.5/requirements-dev.txt
--rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 flipside-2.0.5/requirements.txt
--rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-25 23:48:35.104442 flipside-2.0.5/setup.cfg
--rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 flipside-2.0.5/setup.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.088416 flipside-2.0.5/src/
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.098382 flipside-2.0.5/src/errors/
--rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-09 02:05:09.000000 flipside-2.0.5/src/errors/api_error.py
--rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/base_error.py
--rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/query_run_errors.py
--rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/sdk_error.py
--rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 flipside-2.0.5/src/errors/server_error.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.098500 flipside-2.0.5/src/integrations/
--rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 flipside-2.0.5/src/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.098968 flipside-2.0.5/src/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 flipside-2.0.5/src/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     9884 2023-05-02 18:10:35.000000 flipside-2.0.5/src/integrations/query_integration/compass_query_integration.py
--rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 flipside-2.0.5/src/integrations/query_integration/defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:47:03.000000 flipside-2.0.5/src/integrations/query_integration/query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.099743 flipside-2.0.5/src/models/
--rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.100533 flipside-2.0.5/src/models/compass/
--rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/cancel_query_run.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.102584 flipside-2.0.5/src/models/compass/core/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/column_metadata.py
--rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/page.py
--rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/page_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/query_request.py
--rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/query_run.py
--rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/result_format.py
--rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/rpc_error.py
--rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/rpc_request.py
--rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/rpc_response.py
--rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/core/tags.py
--rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/create_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/get_query_run.py
--rw-r--r--   0 jim        (501) staff       (20)     2104 2023-05-08 14:18:06.000000 flipside-2.0.5/src/models/compass/get_query_run_results.py
--rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/get_sql_statement.py
--rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/compass/query_results.py
--rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/query.py
--rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/query_defaults.py
--rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:47:03.000000 flipside-2.0.5/src/models/query_result_set.py
--rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/query_run_stats.py
--rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/query_status.py
--rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 flipside-2.0.5/src/models/sleep_config.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.102781 flipside-2.0.5/src/tests/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.102908 flipside-2.0.5/src/tests/integrations/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/integrations/__init__.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.103214 flipside-2.0.5/src/tests/integrations/query_integration/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/integrations/query_integration/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/integrations/query_integration/test_query_compass_integration.py
--rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/integrations/query_integration/test_query_result_set_builder.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.103441 flipside-2.0.5/src/tests/models/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/models/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/models/test_query_status.py
--rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/test_rpc.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.103685 flipside-2.0.5/src/tests/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 flipside-2.0.5/src/tests/utils/test_sleep.py
-drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-25 23:48:35.103924 flipside-2.0.5/src/utils/
--rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.5/src/utils/__init__.py
--rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 flipside-2.0.5/src/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.405232 flipside-2.0.7/
+-rw-r--r--   0 jim        (501) staff       (20)     1073 2022-07-25 21:42:15.000000 flipside-2.0.7/LICENSE.txt
+-rw-r--r--   0 jim        (501) staff       (20)       69 2022-07-25 21:42:15.000000 flipside-2.0.7/MANIFEST.in
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-26 02:51:31.405314 flipside-2.0.7/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)      709 2023-05-02 18:18:58.000000 flipside-2.0.7/README.md
+-rw-r--r--   0 jim        (501) staff       (20)        5 2023-05-26 02:49:25.000000 flipside-2.0.7/VERSION
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.390730 flipside-2.0.7/flipside/
+-rw-r--r--   0 jim        (501) staff       (20)      147 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.392270 flipside-2.0.7/flipside/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/errors/server_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2982 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/flipside.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.392410 flipside-2.0.7/flipside/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.392892 flipside-2.0.7/flipside/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9851 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.393749 flipside-2.0.7/flipside/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.394528 flipside-2.0.7/flipside/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.395918 flipside-2.0.7/flipside/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2231 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/models/sleep_config.py
+-rw-r--r--   0 jim        (501) staff       (20)     5898 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/rpc.py
+-rw-r--r--   0 jim        (501) staff       (20)       68 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/shroomdk.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.396184 flipside-2.0.7/flipside/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.396350 flipside-2.0.7/flipside/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.396917 flipside-2.0.7/flipside/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.397219 flipside-2.0.7/flipside/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.397487 flipside-2.0.7/flipside/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.397756 flipside-2.0.7/flipside/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside/utils/sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.391442 flipside-2.0.7/flipside.egg-info/
+-rw-r--r--   0 jim        (501) staff       (20)     1510 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside.egg-info/PKG-INFO
+-rw-r--r--   0 jim        (501) staff       (20)     4101 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside.egg-info/SOURCES.txt
+-rw-r--r--   0 jim        (501) staff       (20)        1 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside.egg-info/dependency_links.txt
+-rw-r--r--   0 jim        (501) staff       (20)       34 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside.egg-info/requires.txt
+-rw-r--r--   0 jim        (501) staff       (20)       13 2023-05-26 02:51:31.000000 flipside-2.0.7/flipside.egg-info/top_level.txt
+-rw-r--r--   0 jim        (501) staff       (20)       30 2022-07-25 21:42:15.000000 flipside-2.0.7/requirements-dev.txt
+-rw-r--r--   0 jim        (501) staff       (20)       33 2023-05-02 18:10:35.000000 flipside-2.0.7/requirements.txt
+-rw-r--r--   0 jim        (501) staff       (20)       79 2023-05-26 02:51:31.405578 flipside-2.0.7/setup.cfg
+-rw-r--r--   0 jim        (501) staff       (20)     1557 2023-05-02 18:10:35.000000 flipside-2.0.7/setup.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.388743 flipside-2.0.7/src/
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.398587 flipside-2.0.7/src/errors/
+-rw-r--r--   0 jim        (501) staff       (20)      336 2023-05-02 18:10:35.000000 flipside-2.0.7/src/errors/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1583 2023-05-09 02:05:09.000000 flipside-2.0.7/src/errors/api_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      121 2023-05-02 18:10:35.000000 flipside-2.0.7/src/errors/base_error.py
+-rw-r--r--   0 jim        (501) staff       (20)     2077 2023-05-02 18:10:35.000000 flipside-2.0.7/src/errors/query_run_errors.py
+-rw-r--r--   0 jim        (501) staff       (20)      262 2023-05-02 18:10:35.000000 flipside-2.0.7/src/errors/sdk_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      361 2023-05-02 18:10:35.000000 flipside-2.0.7/src/errors/server_error.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.398715 flipside-2.0.7/src/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)       69 2023-05-02 18:10:35.000000 flipside-2.0.7/src/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.399276 flipside-2.0.7/src/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)       77 2023-05-02 18:10:35.000000 flipside-2.0.7/src/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     9851 2023-05-26 02:49:25.000000 flipside-2.0.7/src/integrations/query_integration/compass_query_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)      237 2023-05-02 18:10:35.000000 flipside-2.0.7/src/integrations/query_integration/defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     3636 2023-05-25 23:47:03.000000 flipside-2.0.7/src/integrations/query_integration/query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.400594 flipside-2.0.7/src/models/
+-rw-r--r--   0 jim        (501) staff       (20)      365 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.401648 flipside-2.0.7/src/models/compass/
+-rw-r--r--   0 jim        (501) staff       (20)       50 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      571 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/cancel_query_run.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.403590 flipside-2.0.7/src/models/compass/core/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      187 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/column_metadata.py
+-rw-r--r--   0 jim        (501) staff       (20)      117 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/page.py
+-rw-r--r--   0 jim        (501) staff       (20)      183 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/page_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      358 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/query_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      807 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)       89 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/result_format.py
+-rw-r--r--   0 jim        (501) staff       (20)      149 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/rpc_error.py
+-rw-r--r--   0 jim        (501) staff       (20)      198 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/rpc_request.py
+-rw-r--r--   0 jim        (501) staff       (20)      252 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/rpc_response.py
+-rw-r--r--   0 jim        (501) staff       (20)      340 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      221 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/core/tags.py
+-rw-r--r--   0 jim        (501) staff       (20)      845 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/create_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)      639 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/get_query_run.py
+-rw-r--r--   0 jim        (501) staff       (20)     2231 2023-05-26 02:49:25.000000 flipside-2.0.7/src/models/compass/get_query_run_results.py
+-rw-r--r--   0 jim        (501) staff       (20)      582 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/get_sql_statement.py
+-rw-r--r--   0 jim        (501) staff       (20)      852 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/compass/query_results.py
+-rw-r--r--   0 jim        (501) staff       (20)     1422 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/query.py
+-rw-r--r--   0 jim        (501) staff       (20)      836 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/query_defaults.py
+-rw-r--r--   0 jim        (501) staff       (20)     1202 2023-05-25 23:47:03.000000 flipside-2.0.7/src/models/query_result_set.py
+-rw-r--r--   0 jim        (501) staff       (20)     1658 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/query_run_stats.py
+-rw-r--r--   0 jim        (501) staff       (20)      544 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)      194 2023-05-02 18:10:35.000000 flipside-2.0.7/src/models/sleep_config.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.403784 flipside-2.0.7/src/tests/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.403903 flipside-2.0.7/src/tests/integrations/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/integrations/__init__.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.404193 flipside-2.0.7/src/tests/integrations/query_integration/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/integrations/query_integration/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     8712 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/integrations/query_integration/test_query_compass_integration.py
+-rw-r--r--   0 jim        (501) staff       (20)     3438 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/integrations/query_integration/test_query_result_set_builder.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.404607 flipside-2.0.7/src/tests/models/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/models/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)      931 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/models/test_query_status.py
+-rw-r--r--   0 jim        (501) staff       (20)     5218 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/test_rpc.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.404896 flipside-2.0.7/src/tests/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     2242 2023-05-02 18:10:35.000000 flipside-2.0.7/src/tests/utils/test_sleep.py
+drwxr-xr-x   0 jim        (501) staff       (20)        0 2023-05-26 02:51:31.405121 flipside-2.0.7/src/utils/
+-rw-r--r--   0 jim        (501) staff       (20)        0 2023-05-02 18:10:35.000000 flipside-2.0.7/src/utils/__init__.py
+-rw-r--r--   0 jim        (501) staff       (20)     1966 2023-05-02 18:10:35.000000 flipside-2.0.7/src/utils/sleep.py
```

### Comparing `flipside-2.0.5/LICENSE.txt` & `flipside-2.0.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/PKG-INFO` & `flipside-2.0.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipside
-Version: 2.0.5
+Version: 2.0.7
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flipside-2.0.5/README.md` & `flipside-2.0.7/README.md`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/errors/api_error.py` & `flipside-2.0.7/flipside/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/errors/query_run_errors.py` & `flipside-2.0.7/flipside/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/flipside.py` & `flipside-2.0.7/flipside/flipside.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/integrations/query_integration/compass_query_integration.py` & `flipside-2.0.7/flipside/integrations/query_integration/compass_query_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,27 +155,27 @@
         self,
         query_run_id: str,
         page_number: int = 1,
         page_size: int = 100000,
         filters: Optional[Union[List[Filter], None]] = [],
         sort_by: Optional[Union[List[SortBy], None]] = [],
     ) -> GetQueryRunResultsRpcResult:
-        query_results_resp = self.rpc.get_query_result(
-            GetQueryRunResultsRpcParams(
-                queryRunId=query_run_id,
-                format=ResultFormat.csv,
-                page=Page(
-                    number=page_number,
-                    size=page_size,
-                ),
-                filters=filters,
-                sortBy=sort_by,
-            )
+        params = GetQueryRunResultsRpcParams(
+            queryRunId=query_run_id,
+            format=ResultFormat.csv,
+            page=Page(
+                number=page_number,
+                size=page_size,
+            ),
+            filters=filters,
+            sortBy=sort_by,
         )
 
+        query_results_resp = self.rpc.get_query_result(params)
+
         if query_results_resp.error:
             raise get_exception_by_error_code(
                 error_code=query_results_resp.error.code
                 if query_results_resp.error
                 else None,
                 message=query_results_resp.error.message
                 if query_results_resp.error
```

### Comparing `flipside-2.0.5/flipside/integrations/query_integration/query_result_set_builder.py` & `flipside-2.0.7/flipside/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/compass/cancel_query_run.py` & `flipside-2.0.7/flipside/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/compass/core/query_run.py` & `flipside-2.0.7/flipside/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/compass/create_query_run.py` & `flipside-2.0.7/flipside/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/compass/get_query_run.py` & `flipside-2.0.7/flipside/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/compass/get_query_run_results.py` & `flipside-2.0.7/flipside/models/compass/get_query_run_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,30 +9,33 @@
 from .core.rpc_request import RpcRequest
 from .core.rpc_response import RpcResponse
 
 
 # Request
 class Filter(BaseModel):
     column: str
-    eq: Optional[str] = None
-    neq: Optional[str] = None
-    gt: Optional[str] = None
-    gte: Optional[str] = None
-    lt: Optional[str] = None
-    lte: Optional[str] = None
-    like: Optional[str] = None
-    in_: Optional[List[str]] = None
-    notIn: Optional[List[str]] = None
+    eq: Optional[Any] = None
+    neq: Optional[Any] = None
+    gt: Optional[Any] = None
+    gte: Optional[Any] = None
+    lt: Optional[Any] = None
+    lte: Optional[Any] = None
+    like: Optional[Any] = None
+    in_: Optional[List[Any]] = None
+    notIn: Optional[List[Any]] = None
 
     class Config:
         fields = {"in_": "in"}
 
     def dict(self, *args, **kwargs) -> dict:
         kwargs.setdefault("exclude_none", True)  # Exclude keys with None values
-        return super().dict(*args, **kwargs)
+        result = super().dict(*args, **kwargs)
+        if "in_" in result:
+            result["in"] = result.pop("in_")  # convert 'in_' back to 'in'
+        return result
 
 
 class SortBy(BaseModel):
     column: str
     direction: str
```

### Comparing `flipside-2.0.5/flipside/models/compass/get_sql_statement.py` & `flipside-2.0.7/flipside/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/compass/query_results.py` & `flipside-2.0.7/flipside/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/query.py` & `flipside-2.0.7/flipside/models/query.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/query_defaults.py` & `flipside-2.0.7/flipside/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/query_result_set.py` & `flipside-2.0.7/flipside/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/query_run_stats.py` & `flipside-2.0.7/flipside/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/models/query_status.py` & `flipside-2.0.7/flipside/models/query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/rpc.py` & `flipside-2.0.7/flipside/rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/tests/integrations/query_integration/test_query_compass_integration.py` & `flipside-2.0.7/flipside/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/tests/integrations/query_integration/test_query_result_set_builder.py` & `flipside-2.0.7/flipside/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/tests/models/test_query_status.py` & `flipside-2.0.7/flipside/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/tests/test_rpc.py` & `flipside-2.0.7/flipside/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/tests/utils/test_sleep.py` & `flipside-2.0.7/flipside/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside/utils/sleep.py` & `flipside-2.0.7/flipside/utils/sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/flipside.egg-info/PKG-INFO` & `flipside-2.0.7/flipside.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flipside
-Version: 2.0.5
+Version: 2.0.7
 Summary: SDK by Flipside Crypto: Query the most reliable & comprehensive blockchain data in crypto
 Home-page: https://github.com/FlipsideCrypto/sdk/python
 Author: dev@flipsidecrypto.com
 Author-email: dev@flipsidecrypto.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `flipside-2.0.5/flipside.egg-info/SOURCES.txt` & `flipside-2.0.7/flipside.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/setup.py` & `flipside-2.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/errors/api_error.py` & `flipside-2.0.7/src/errors/api_error.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/errors/query_run_errors.py` & `flipside-2.0.7/src/errors/query_run_errors.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/integrations/query_integration/compass_query_integration.py` & `flipside-2.0.7/src/integrations/query_integration/compass_query_integration.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,27 +155,27 @@
         self,
         query_run_id: str,
         page_number: int = 1,
         page_size: int = 100000,
         filters: Optional[Union[List[Filter], None]] = [],
         sort_by: Optional[Union[List[SortBy], None]] = [],
     ) -> GetQueryRunResultsRpcResult:
-        query_results_resp = self.rpc.get_query_result(
-            GetQueryRunResultsRpcParams(
-                queryRunId=query_run_id,
-                format=ResultFormat.csv,
-                page=Page(
-                    number=page_number,
-                    size=page_size,
-                ),
-                filters=filters,
-                sortBy=sort_by,
-            )
+        params = GetQueryRunResultsRpcParams(
+            queryRunId=query_run_id,
+            format=ResultFormat.csv,
+            page=Page(
+                number=page_number,
+                size=page_size,
+            ),
+            filters=filters,
+            sortBy=sort_by,
         )
 
+        query_results_resp = self.rpc.get_query_result(params)
+
         if query_results_resp.error:
             raise get_exception_by_error_code(
                 error_code=query_results_resp.error.code
                 if query_results_resp.error
                 else None,
                 message=query_results_resp.error.message
                 if query_results_resp.error
```

### Comparing `flipside-2.0.5/src/integrations/query_integration/query_result_set_builder.py` & `flipside-2.0.7/src/integrations/query_integration/query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/compass/cancel_query_run.py` & `flipside-2.0.7/src/models/compass/cancel_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/compass/core/query_run.py` & `flipside-2.0.7/src/models/compass/core/query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/compass/create_query_run.py` & `flipside-2.0.7/src/models/compass/create_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/compass/get_query_run.py` & `flipside-2.0.7/src/models/compass/get_query_run.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/compass/get_query_run_results.py` & `flipside-2.0.7/src/models/compass/get_query_run_results.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,30 +9,33 @@
 from .core.rpc_request import RpcRequest
 from .core.rpc_response import RpcResponse
 
 
 # Request
 class Filter(BaseModel):
     column: str
-    eq: Optional[str] = None
-    neq: Optional[str] = None
-    gt: Optional[str] = None
-    gte: Optional[str] = None
-    lt: Optional[str] = None
-    lte: Optional[str] = None
-    like: Optional[str] = None
-    in_: Optional[List[str]] = None
-    notIn: Optional[List[str]] = None
+    eq: Optional[Any] = None
+    neq: Optional[Any] = None
+    gt: Optional[Any] = None
+    gte: Optional[Any] = None
+    lt: Optional[Any] = None
+    lte: Optional[Any] = None
+    like: Optional[Any] = None
+    in_: Optional[List[Any]] = None
+    notIn: Optional[List[Any]] = None
 
     class Config:
         fields = {"in_": "in"}
 
     def dict(self, *args, **kwargs) -> dict:
         kwargs.setdefault("exclude_none", True)  # Exclude keys with None values
-        return super().dict(*args, **kwargs)
+        result = super().dict(*args, **kwargs)
+        if "in_" in result:
+            result["in"] = result.pop("in_")  # convert 'in_' back to 'in'
+        return result
 
 
 class SortBy(BaseModel):
     column: str
     direction: str
```

### Comparing `flipside-2.0.5/src/models/compass/get_sql_statement.py` & `flipside-2.0.7/src/models/compass/get_sql_statement.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/compass/query_results.py` & `flipside-2.0.7/src/models/compass/query_results.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/query.py` & `flipside-2.0.7/src/models/query.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/query_defaults.py` & `flipside-2.0.7/src/models/query_defaults.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/query_result_set.py` & `flipside-2.0.7/src/models/query_result_set.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/query_run_stats.py` & `flipside-2.0.7/src/models/query_run_stats.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/models/query_status.py` & `flipside-2.0.7/src/models/query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/tests/integrations/query_integration/test_query_compass_integration.py` & `flipside-2.0.7/src/tests/integrations/query_integration/test_query_compass_integration.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/tests/integrations/query_integration/test_query_result_set_builder.py` & `flipside-2.0.7/src/tests/integrations/query_integration/test_query_result_set_builder.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/tests/models/test_query_status.py` & `flipside-2.0.7/src/tests/models/test_query_status.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/tests/test_rpc.py` & `flipside-2.0.7/src/tests/test_rpc.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/tests/utils/test_sleep.py` & `flipside-2.0.7/src/tests/utils/test_sleep.py`

 * *Files identical despite different names*

### Comparing `flipside-2.0.5/src/utils/sleep.py` & `flipside-2.0.7/src/utils/sleep.py`

 * *Files identical despite different names*

