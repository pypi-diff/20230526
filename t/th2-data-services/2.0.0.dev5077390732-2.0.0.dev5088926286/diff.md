# Comparing `tmp/th2_data_services-2.0.0.dev5077390732.tar.gz` & `tmp/th2_data_services-2.0.0.dev5088926286.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/th2_data_services-2.0.0.dev5077390732.tar", last modified: Thu May 25 07:45:38 2023, max compression
+gzip compressed data, was "dist/th2_data_services-2.0.0.dev5088926286.tar", last modified: Fri May 26 08:43:12 2023, max compression
```

## Comparing `th2_data_services-2.0.0.dev5077390732.tar` & `th2_data_services-2.0.0.dev5088926286.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/
--rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)   510907 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-25 07:45:26.000000 th2_data_services-2.0.0.dev5077390732/package_info.json
--rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/config/
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/config/config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30846 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/
--rw-r--r--   0 runner    (1001) docker     (122)      806 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/etc_driver.py
--rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/event_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/parent_event_tree_collection.py
--rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/adapter.py
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/data_source.py
--rw-r--r--   0 runner    (1001) docker     (122)      706 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/source_api.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/struct.py
--rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/stub_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/utils/converter.py
--rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/utils/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/
--rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/_json.py
--rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/_types.py
--rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/aggregation_classes.py
--rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/az_tree.py
--rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/categorizers.py
--rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/category.py
--rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (122)      908 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/decode_error_handler.py
--rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/display.py
--rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/event_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/select.py
--rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/totals.py
--rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/experimental.py
--rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/json_tree.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/message_utils/
--rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/message_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/message_utils/frequencies.py
--rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/message_utils/message_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/misc_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/perfect_table.py
--rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/script_report_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/sse_client.py
--rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/time.py
--rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/total_category_calculator.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/viewer_structs/
--rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/viewer_structs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-05-25 07:44:34.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/viewer_structs/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)   614698 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-25 07:45:38.000000 th2_data_services-2.0.0.dev5077390732/th2_data_services.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/
+-rw-r--r--   0 runner    (1001) docker     (122)       68 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23148 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-26 08:42:52.000000 th2_data_services-2.0.0.dev5088926286/package_info.json
+-rw-r--r--   0 runner    (1001) docker     (122)      269 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2427 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1213 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30846 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/
+-rw-r--r--   0 runner    (1001) docker     (122)      806 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2146 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/etc_driver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16045 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/event_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)    25893 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2497 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2501 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/parent_event_tree_collection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1680 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1100 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1056 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (122)      706 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/source_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/struct.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2255 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/stub_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3023 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/utils/converter.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2705 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/utils/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)     3360 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      643 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15883 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/aggregation_classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)      894 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/az_tree.py
+-rw-r--r--   0 runner    (1001) docker     (122)      742 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/categorizers.py
+-rw-r--r--   0 runner    (1001) docker     (122)      935 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/category.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3296 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (122)      908 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/decode_error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2604 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      725 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11551 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/display.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7107 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/event_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5291 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12089 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/select.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6805 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/totals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1819 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15216 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/json_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/message_utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      663 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/message_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1014 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/message_utils/frequencies.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14456 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/message_utils/message_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15739 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/misc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10508 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/perfect_table.py
+-rw-r--r--   0 runner    (1001) docker     (122)    33801 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/script_report_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3531 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/sse_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5285 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/time.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6538 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/total_category_calculator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/viewer_structs/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/viewer_structs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6185 2023-05-26 08:41:27.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/viewer_structs/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    28243 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      575 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       18 2023-05-26 08:43:12.000000 th2_data_services-2.0.0.dev5088926286/th2_data_services.egg-info/top_level.txt
```

### Comparing `th2_data_services-2.0.0.dev5077390732/setup.py` & `th2_data_services-2.0.0.dev5088926286/setup.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/config/__init__.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/config/config.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/config/config.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/data.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/data.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/__init__.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/etc_driver.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/etc_driver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/event_tree.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/event_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/event_tree_collection.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/exceptions.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/event_tree/parent_event_tree_collection.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/event_tree/parent_event_tree_collection.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/exceptions.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/exceptions.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/__init__.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/adapter.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/adapter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/command.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/command.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/data_source.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/data_source.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/source_api.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/source_api.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/struct.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/struct.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/stub_builder.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/stub_builder.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/utils/__init__.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/utils/converter.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/utils/converter.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/interfaces/utils/resolver.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/interfaces/utils/resolver.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/_json.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/_json.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/_types.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/_types.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/aggregation_classes.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/aggregation_classes.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/az_tree.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/az_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/categorizers.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/categorizers.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/category.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/category.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/converters.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/converters.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/decode_error_handler.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/decode_error_handler.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/display.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/__init__.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/display.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/display.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/event_utils.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/event_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/frequencies.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/select.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/select.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/event_utils/totals.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/event_utils/totals.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/experimental.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/experimental.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/json_tree.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/json_tree.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/message_utils/__init__.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/message_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/message_utils/frequencies.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/message_utils/frequencies.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/message_utils/message_utils.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/message_utils/message_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/misc_utils.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/misc_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/perfect_table.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/perfect_table.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/script_report_utils.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/script_report_utils.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/sse_client.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/sse_client.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/time.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/time.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/total_category_calculator.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/total_category_calculator.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/viewer_structs/__init__.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/viewer_structs/__init__.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services/utils/viewer_structs/verification.py` & `th2_data_services-2.0.0.dev5088926286/th2_data_services/utils/viewer_structs/verification.py`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services.egg-info/SOURCES.txt` & `th2_data_services-2.0.0.dev5088926286/th2_data_services.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `th2_data_services-2.0.0.dev5077390732/th2_data_services.egg-info/requires.txt` & `th2_data_services-2.0.0.dev5088926286/th2_data_services.egg-info/requires.txt`

 * *Files identical despite different names*

