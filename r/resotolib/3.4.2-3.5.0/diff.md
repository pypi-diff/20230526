# Comparing `tmp/resotolib-3.4.2.tar.gz` & `tmp/resotolib-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.4.2.tar", last modified: Wed May 10 12:25:37 2023, max compression
+gzip compressed data, was "resotolib-3.5.0.tar", last modified: Fri May 26 18:24:17 2023, max compression
```

## Comparing `resotolib-3.4.2.tar` & `resotolib-3.5.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-10 12:22:37.000000 resotolib-3.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-10 12:25:37.406532 resotolib-3.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-10 12:22:37.000000 resotolib-3.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-10 12:22:37.000000 resotolib-3.4.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-10 12:22:37.000000 resotolib-3.4.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/periodic.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40989 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    16788 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.402532 resotolib-3.4.2/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    26757 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.402532 resotolib-3.4.2/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6471 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/log/logstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    22777 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.402532 resotolib-3.4.2/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.402532 resotolib-3.4.2/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    11471 2023-05-10 12:22:37.000000 resotolib-3.4.2/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.398532 resotolib-3.4.2/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-10 12:25:37.000000 resotolib-3.4.2/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-10 12:25:37.406532 resotolib-3.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-10 12:22:37.000000 resotolib-3.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/test/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/asynchronous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/test/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/asynchronous/web/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 12:25:37.406532 resotolib-3.4.2/test/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/custom_command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/model_check_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/model_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/progress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/core/tasks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/durations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/json_bender_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/parse_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2750 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-10 12:22:37.000000 resotolib-3.4.2/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-26 18:21:38.000000 resotolib-3.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-26 18:24:17.649375 resotolib-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-05-26 18:21:38.000000 resotolib-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-26 18:21:38.000000 resotolib-3.5.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-26 18:21:38.000000 resotolib-3.5.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.641375 resotolib-3.5.0/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.641375 resotolib-3.5.0/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/periodic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.641375 resotolib-3.5.0/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4134 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8971 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41019 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17649 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9787 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13827 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6884 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6215 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16850 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8301 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5426 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5831 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    26773 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7072 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33805 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23264 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.645375 resotolib-3.5.0/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    11813 2023-05-26 18:21:38.000000 resotolib-3.5.0/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.641375 resotolib-3.5.0/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-26 18:24:17.000000 resotolib-3.5.0/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-26 18:24:17.649375 resotolib-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-05-26 18:21:38.000000 resotolib-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/test/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1871 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/asynchronous/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/test/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/asynchronous/web/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:17.649375 resotolib-3.5.0/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/custom_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/model_check_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/model_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/progress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/core/tasks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/durations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/json_bender_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/parse_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15731 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3269 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-26 18:21:38.000000 resotolib-3.5.0/test/test_x509.py
```

### Comparing `resotolib-3.4.2/PKG-INFO` & `resotolib-3.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotolib-3.4.2/README.md` & `resotolib-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/args.py` & `resotolib-3.5.0/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/asynchronous/periodic.py` & `resotolib-3.5.0/resotolib/asynchronous/periodic.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/asynchronous/web/runner.py` & `resotolib-3.5.0/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.5.0/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/baseplugin.py` & `resotolib-3.5.0/resotolib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/baseresources.py` & `resotolib-3.5.0/resotolib/baseresources.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 from copy import deepcopy
 from datetime import datetime, timezone, timedelta
 from enum import Enum
 from functools import wraps, cached_property
 from typing import Dict, Iterator, List, ClassVar, Optional, TypedDict, Any, TypeVar, Type, Callable, Set, Tuple
 
 import jsons
-from attrs import define, field, resolve_types, Factory
+from attr import resolve_types
+from attrs import define, field, Factory
 from prometheus_client import Counter, Summary
 
 from resotolib.json import from_json as _from_json, to_json as _to_json
 from resotolib.logger import log
 from resotolib.types import Json
 from resotolib.utils import make_valid_timestamp, utc_str
 
@@ -390,29 +391,29 @@
     @metrics_resource_cleanup.time()  # type: ignore
     @unless_protected
     def cleanup(self, graph: Optional[Any] = None) -> bool:
         if self.phantom:
             raise RuntimeError(f"Can't cleanup phantom resource {self.rtdname}")
 
         if self.cleaned:
-            log.debug(f"Resource {self.rtdname} has already been cleaned up")
+            log.info(f"Resource {self.rtdname} has already been cleaned up")
             return True
 
         self._changes.add("cleaned")
         if graph is None:
             graph = self._graph
 
         account = self.account(graph)
         region = self.region(graph)
         if not isinstance(account, BaseAccount) or not isinstance(region, BaseRegion):
             raise RuntimeError(f"Could not determine account or region for cleanup of {self.rtdname}")
 
         log_suffix = f" in account {account.dname} region {region.name}"
         self.log("Trying to clean up")
-        log.debug(f"Trying to clean up {self.rtdname}{log_suffix}")
+        log.info(f"Trying to clean up {self.rtdname}{log_suffix}")
         try:
             if deleted := self.delete(graph):
                 self._cleaned = True
                 self.log("Successfully cleaned up")
                 log.info(f"Successfully cleaned up {self.rtdname}{log_suffix}")
         except Exception as e:
             self.log("An error occurred during clean up", exception=e)
@@ -1215,8 +1216,8 @@
 class UnknownLocation(BaseResource):
     kind: ClassVar[str] = "unknown_location"
 
     def delete(self, graph: Any) -> bool:
         return False
 
 
-resolve_types(BaseResource)
+resolve_types(BaseResource)  # type: ignore
```

### Comparing `resotolib-3.4.2/resotolib/config.py` & `resotolib-3.5.0/resotolib/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/__init__.py` & `resotolib-3.5.0/resotolib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/actions.py` & `resotolib-3.5.0/resotolib/core/actions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/ca.py` & `resotolib-3.5.0/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/config.py` & `resotolib-3.5.0/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/custom_command.py` & `resotolib-3.5.0/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/events.py` & `resotolib-3.5.0/resotolib/core/events.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/model_check.py` & `resotolib-3.5.0/resotolib/core/model_check.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
 
     # List of all plugin classes that need to be imported.
     model_classes = {
         *dynamic_import("resoto_plugin_aws.collector.all_resources"),
         *dynamic_import("resoto_plugin_digitalocean.resources.DigitalOceanResource"),
         *dynamic_import("resoto_plugin_dockerhub.resources.DockerHubResource"),
         *dynamic_import("resoto_plugin_example_collector.ExampleResource"),
-        *dynamic_import("resoto_plugin_gcp.gcp_resources.GCPResource"),
+        *dynamic_import("resoto_plugin_gcp.resources.base.GcpResource"),
         *dynamic_import("resoto_plugin_github.resources.GithubResource"),
         *dynamic_import("resoto_plugin_k8s.resources.KubernetesResource"),
         *dynamic_import("resoto_plugin_onelogin.OneLoginResource"),
         *dynamic_import("resoto_plugin_onprem.resources.OnpremResource"),
         *dynamic_import("resoto_plugin_posthog.resources.PosthogResource"),
         *dynamic_import("resoto_plugin_random.resources.RandomResource"),
         *dynamic_import("resoto_plugin_scarf.resources.ScarfResource"),
```

### Comparing `resotolib-3.4.2/resotolib/core/model_export.py` & `resotolib-3.5.0/resotolib/core/model_export.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         elif is_dict(clazz):
             key_type, value_type = dict_types(to_check)
             check(key_type)
             check(value_type)
         elif is_collection(clazz):
             check(type_arg(to_check))
         elif attrs.has(clazz):
-            resolve_types(clazz)
+            resolve_types(clazz)  # type: ignore
             all_classes.add(clazz)
             for mro_clazz in clazz.mro()[1:]:
                 check(mro_clazz)
             if walk_subclasses:
                 for subclass in clazz.__subclasses__():
                     check(subclass)
             for field in attrs.fields(clazz):
@@ -205,15 +205,15 @@
         ]
 
         # required = not is_optional(field.type)
         return [json(name, kind, required, desc, meta)] + synthetics
 
     for cls in classes:
         if attrs.has(cls):
-            resolve_types(cls)  # make sure all string based types are resolved correctly
+            resolve_types(cls)  # type: ignore # make sure all string based types are resolved correctly
     model: List[Json] = []
     all_classes = transitive_classes(classes, walk_subclasses)
 
     # type edge_type -> list of types
     successors: Dict[str, Dict[str, List[str]]] = defaultdict(lambda: defaultdict(list))
 
     for clazz in all_classes:
@@ -266,15 +266,15 @@
                 raise AttributeError(f"Enumeration {clazz} does not use string as values!")
 
         enum_values = [literal_name(literal) for literal in clazz]
         model.append({"fqn": model_name(clazz), "runtime_kind": "string", "enum": enum_values})
 
     for cls in all_classes:
         if attrs.has(cls):
-            resolve_types(cls)  # make sure all string based types are resolved correctly
+            resolve_types(cls)  # type: ignore # make sure all string based types are resolved correctly
             export_data_class(cls)
         elif is_enum(cls):
             export_enum(cls)
         else:
             raise AttributeError(f"Don't know how to handle: {cls}")
     return model
 
@@ -338,15 +338,15 @@
     return node_dict
 
 
 @lru_cache(maxsize=None)
 def locate_python_type(python_type: str) -> Any:
     cls: Type[Any] = locate(python_type)  # type: ignore
     if attrs.has(cls):
-        attrs.resolve_types(cls)
+        attrs.resolve_types(cls)  # type: ignore
     return cls
 
 
 converter = cattrs.Converter()
 
 
 def convert_datetime(value: datetime) -> datetime:
```

### Comparing `resotolib-3.4.2/resotolib/core/progress.py` & `resotolib-3.5.0/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/search.py` & `resotolib-3.5.0/resotolib/core/search.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/core/tasks.py` & `resotolib-3.5.0/resotolib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/durations.py` & `resotolib-3.5.0/resotolib/durations.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/event.py` & `resotolib-3.5.0/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/graph/__init__.py` & `resotolib-3.5.0/resotolib/graph/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -377,15 +377,15 @@
 
     def export_iterator(self) -> GraphExportIterator:
         return GraphExportIterator(self)
 
 
 @lru_cache(maxsize=4096)  # Only resolve types once per type
 def resolve_type(clazz: Type[Any]) -> None:
-    resolve_types(clazz)
+    resolve_types(clazz)  # type: ignore
 
 
 def validate_dataclass(node: BaseResource) -> None:
     resolve_type(type(node))  # make sure all type annotations are resolved
     for field in fields(type(node)):
         value = getattr(node, field.name)
         try:
```

### Comparing `resotolib-3.4.2/resotolib/graph/graph_extensions.py` & `resotolib-3.5.0/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/json.py` & `resotolib-3.5.0/resotolib/json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/json_bender.py` & `resotolib-3.5.0/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/jwt.py` & `resotolib-3.5.0/resotolib/jwt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 import os
 import jwt
 import base64
 import hashlib
 import time
+
+from cryptography.hazmat.primitives import serialization
+from jwt.utils import base64url_encode
+
 from resotolib.args import ArgumentParser
-from resotolib.x509 import x5t_s256
+from resotolib.x509 import x5t_s256, x5t
 from typing import Any, Optional, Tuple, Dict, Mapping, Union, cast
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey, RSAPublicKey
 from cryptography.x509.base import Certificate
 
 from resotolib.types import Json
 
 
@@ -50,29 +54,29 @@
     headers: Dict[str, str],
     cert: Optional[Certificate] = None,
 ) -> str:
     """Encodes a payload into a JWT either using an RSA private key."""
     headers.update({"alg": "RS256"})
     if cert is not None:
         headers.update({"x5t#S256": x5t_s256(cert)})
-    return jwt.encode(payload, private_key, algorithm="RS256", headers=headers)  # type: ignore
+    return jwt.encode(payload, private_key, algorithm="RS256", headers=headers)
 
 
 def encode_jwt_psk(
     payload: Dict[str, Any],
     psk: str,
     headers: Dict[str, str],
 ) -> str:
     """Encodes a payload into a JWT and signs using a key derived from a pre-shared-key.
     Stores the key's salt in the JWT headers.
     """
     key, salt = key_from_psk(psk)
     salt_encoded = base64.standard_b64encode(salt).decode("utf-8")
     headers.update({"alg": "HS256", "salt": salt_encoded})
-    return jwt.encode(payload, key, algorithm="HS256", headers=headers)  # type: ignore
+    return jwt.encode(payload, key, algorithm="HS256", headers=headers)
 
 
 def decode_jwt(
     encoded_jwt: str, psk_or_cert: Union[str, Certificate, RSAPublicKey], options: Optional[Dict[str, Any]] = None
 ) -> Json:
     """Decode a JWT using a key derived from a pre-shared-key and a salt stored
     in the JWT headers or an RSA public key.
@@ -152,14 +156,35 @@
         or authorization_header[len(scheme) : len(scheme) + 1] != " "
     ):
         return None
     encoded_jwt = authorization_header[len(scheme) + 1 :]
     return decode_jwt(encoded_jwt, psk_or_cert, options)
 
 
+def create_jwk_dict(cert: Certificate) -> Json:
+    pub_key = cert.public_key()
+    if not isinstance(pub_key, RSAPublicKey):
+        raise ValueError(f"Unsupported public key type: {type(pub_key)}")
+    pem_data = cert.public_bytes(serialization.Encoding.PEM)
+    pem_contents = pem_data.split(b"\n")[1:-2]  # Remove header and footer lines
+    x5t_256 = x5t_s256(cert)
+    pub_num = pub_key.public_numbers()
+    return {
+        "kty": "RSA",
+        "alg": cert.signature_algorithm_oid._name,
+        "n": base64url_encode(pub_num.n.to_bytes((pub_num.n.bit_length() + 7) // 8, "big")).decode("utf-8"),
+        "e": base64url_encode(pub_num.e.to_bytes((pub_num.e.bit_length() + 7) // 8, "big")).decode("utf-8"),
+        "use": "sig",
+        "kid": x5t_256,
+        "x5t": x5t(cert),
+        "x5t#S256": x5t_256,
+        "x5c": [b"".join(pem_contents).decode("utf-8")],
+    }
+
+
 def add_args(arg_parser: ArgumentParser) -> None:
     arg_parser.add_argument(
         "--psk",
         help="Pre-shared key",
         type=lambda x: x if len(x) > 0 else None,
         default=None,
         dest="psk",
```

### Comparing `resotolib-3.4.2/resotolib/lock.py` & `resotolib-3.5.0/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/logger.py` & `resotolib-3.5.0/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/parse_util.py` & `resotolib-3.5.0/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/proc.py` & `resotolib-3.5.0/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/tree.py` & `resotolib-3.5.0/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/utils.py` & `resotolib-3.5.0/resotolib/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+import sys
+import select
 import hashlib
 import os
 import random
 import re
 import socket
 import string
 import time
 from argparse import ArgumentParser
+from contextlib import closing
 from copy import deepcopy
 from datetime import date, datetime, timezone, timedelta
 from functools import wraps, cached_property
 from tarfile import TarFile, TarInfo
 from typing import Dict, List, Tuple, Optional, NoReturn, Any, Mapping, Union, Callable, cast, Iterator, TypeVar
 from zoneinfo import ZoneInfo
 
@@ -608,7 +611,20 @@
     if isinstance(to_be_cleaned, dict):
         reference = cast(Dict[str, JsonElement], reference)
 
         return {k: drop_deleted_attributes(v, reference[k]) for k, v in to_be_cleaned.items() if k in reference}
 
     # should never happen if mypy is happy
     raise ValueError(f"Unexpected type {type(to_be_cleaned)}")
+
+
+def get_free_port() -> int:
+    with closing(socket.socket(socket.AF_INET, socket.SOCK_STREAM)) as tcp:
+        tcp.bind(("", 0))
+        tcp.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
+        return tcp.getsockname()[1]  # type: ignore
+
+
+def stdin_generator() -> Iterator[str]:
+    if select.select([sys.stdin], [], [], 0.0)[0]:
+        for line in iter(sys.stdin.readline, ""):
+            yield line.rstrip("\r\n")
```

### Comparing `resotolib-3.4.2/resotolib/web/__init__.py` & `resotolib-3.5.0/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/metrics.py` & `resotolib-3.5.0/resotolib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.5.0/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.5.0/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.5.0/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/static/favicon-16x16.png` & `resotolib-3.5.0/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/static/favicon-32x32.png` & `resotolib-3.5.0/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/static/index.html` & `resotolib-3.5.0/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/static/mstile-150x150.png` & `resotolib-3.5.0/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/web/static/picnic.min.css` & `resotolib-3.5.0/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/resotolib/x509.py` & `resotolib-3.5.0/resotolib/x509.py`

 * *Files 8% similar despite different names*

```diff
@@ -126,34 +126,36 @@
 def sign_csr(
     csr: CertificateSigningRequest,
     ca_key: RSAPrivateKey,
     ca_cert: Certificate,
     days_valid: int = 365,
     server_auth: bool = True,
     client_auth: bool = True,
+    key_usages: Optional[Dict[str, bool]] = None,
 ) -> Certificate:
+    usage = key_usages or {}
     crt_build = (
         x509.CertificateBuilder()
         .subject_name(csr.subject)
         .issuer_name(ca_cert.subject)
         .public_key(csr.public_key())
         .serial_number(x509.random_serial_number())
         .not_valid_before(datetime.now(tz=timezone.utc))
         .not_valid_after(datetime.now(tz=timezone.utc) + timedelta(days=days_valid))
         .add_extension(
             x509.KeyUsage(
-                digital_signature=True,  # Server/client certs are allowed for
-                key_encipherment=True,  # signatures and encrypting traffic.
-                key_cert_sign=False,
-                key_agreement=False,
-                content_commitment=False,
-                data_encipherment=False,
-                crl_sign=False,
-                encipher_only=False,
-                decipher_only=False,
+                digital_signature=usage.get("digital_signature", True),  # Server/client certs are allowed for
+                key_encipherment=usage.get("key_encipherment", True),  # signatures and encrypting traffic.
+                key_cert_sign=usage.get("key_cert_sign", False),
+                key_agreement=usage.get("key_agreement", False),
+                content_commitment=usage.get("content_commitment", False),
+                data_encipherment=usage.get("data_encipherment", False),
+                crl_sign=usage.get("crl_sign", False),
+                encipher_only=usage.get("encipher_only", False),
+                decipher_only=usage.get("decipher_only", False),
             ),
             critical=True,
         )
     )
     if server_auth or client_auth:
         key_usage = []
         if server_auth:
```

### Comparing `resotolib-3.4.2/resotolib.egg-info/PKG-INFO` & `resotolib-3.5.0/resotolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.4.2
+Version: 3.5.0
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotolib-3.4.2/resotolib.egg-info/SOURCES.txt` & `resotolib-3.5.0/resotolib.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -47,15 +47,14 @@
 resotolib/core/model_export.py
 resotolib/core/progress.py
 resotolib/core/search.py
 resotolib/core/tasks.py
 resotolib/graph/__init__.py
 resotolib/graph/graph_extensions.py
 resotolib/log/__init__.py
-resotolib/log/logstream.py
 resotolib/web/__init__.py
 resotolib/web/metrics.py
 resotolib/web/static/android-chrome-192x192.png
 resotolib/web/static/android-chrome-512x512.png
 resotolib/web/static/apple-touch-icon.png
 resotolib/web/static/browserconfig.xml
 resotolib/web/static/favicon-16x16.png
@@ -79,14 +78,15 @@
 test/test_logging.py
 test/test_plugin.py
 test/test_tree.py
 test/test_utils.py
 test/test_web.py
 test/test_x509.py
 test/asynchronous/__init__.py
+test/asynchronous/test_utils.py
 test/asynchronous/web/__init__.py
 test/asynchronous/web/test_auth.py
 test/core/__init__.py
 test/core/custom_command_test.py
 test/core/model_check_test.py
 test/core/model_export_test.py
 test/core/progress_test.py
```

### Comparing `resotolib-3.4.2/setup.py` & `resotolib-3.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/asynchronous/web/test_auth.py` & `resotolib-3.5.0/test/asynchronous/web/test_auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 import asyncio
+from datetime import timedelta
 from typing import Any
 
 import pytest
 from aiohttp.test_utils import TestClient
 from multidict import CIMultiDict
 from pytest import mark
 from aiohttp.web import Application, Request, Response
-from resotolib.asynchronous.web.auth import check_jwt, jwt_from_context
+from resotolib.asynchronous.web.auth import check_auth, jwt_from_context
 from resotolib.jwt import encode_jwt
 
 # noinspection PyUnresolvedReferences
 from aiohttp.pytest_plugin import aiohttp_client
 
 
 @pytest.fixture
@@ -23,36 +24,28 @@
     async def hello(_: Request) -> Response:
         jwt = await jwt_from_context()
         # make sure, the context variable is set
         assert jwt["foo"] == "bla"
         assert "exp" in jwt
         return Response(text="Hello, world")
 
-    app = Application(middlewares=[check_jwt("test", set())])
+    app = Application(middlewares=[check_auth("test", timedelta(minutes=5), set())])
     app.router.add_get("/", hello)
     return app
 
 
 @mark.asyncio
 async def test_correct_psk(aiohttp_client: Any, app_with_auth: Application) -> None:
     client: TestClient = await aiohttp_client(app_with_auth)
     jwt = encode_jwt({"foo": "bla"}, "test")
     resp = await client.get("/", headers=CIMultiDict({"Authorization": f"Bearer {jwt}"}))
     assert resp.status == 200
 
 
 @mark.asyncio
-async def test_correct_psk_as_cookie(aiohttp_client: Any, app_with_auth: Application) -> None:
-    client: TestClient = await aiohttp_client(app_with_auth)
-    jwt = encode_jwt({"foo": "bla"}, "test")
-    resp = await client.get("/", cookies=CIMultiDict({"resoto_authorization": f"Bearer {jwt}"}))
-    assert resp.status == 200
-
-
-@mark.asyncio
 async def test_wrong_psk(aiohttp_client: Any, app_with_auth: Application) -> None:
     client: TestClient = await aiohttp_client(app_with_auth)
     jwt = encode_jwt({"foo": "bla"}, "wrong!")
     resp = await client.get("/", headers=CIMultiDict({"Authorization": f"Bearer {jwt}"}))
     assert resp.status == 401
```

### Comparing `resotolib-3.4.2/test/core/custom_command_test.py` & `resotolib-3.5.0/test/core/custom_command_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/core/model_check_test.py` & `resotolib-3.5.0/test/core/model_check_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/core/model_export_test.py` & `resotolib-3.5.0/test/core/model_export_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/core/progress_test.py` & `resotolib-3.5.0/test/core/progress_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/core/tasks_test.py` & `resotolib-3.5.0/test/core/tasks_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/durations_test.py` & `resotolib-3.5.0/test/durations_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/json_bender_test.py` & `resotolib-3.5.0/test/json_bender_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/parse_util_test.py` & `resotolib-3.5.0/test/parse_util_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_args.py` & `resotolib-3.5.0/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_baseresources.py` & `resotolib-3.5.0/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_config.py` & `resotolib-3.5.0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_graph.py` & `resotolib-3.5.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_graph_extensions.py` & `resotolib-3.5.0/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_json.py` & `resotolib-3.5.0/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_jwt.py` & `resotolib-3.5.0/test/test_jwt.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import datetime
 from resotolib.jwt import (
     decode_jwt_from_header_value,
     decode_jwt_from_headers,
     encode_jwt,
     decode_jwt,
     encode_jwt_to_headers,
+    create_jwk_dict,
 )
 from jwt import (
     InvalidSignatureError,
     ExpiredSignatureError,
     ImmatureSignatureError,
     MissingRequiredClaimError,
     get_unverified_header,
@@ -71,7 +72,24 @@
     jwt = encode_jwt(payload, cert_key, expire_in=-1)
     assert cert_is_signed_by_ca(cert_crt, ca_cert)
     assert decode_jwt(jwt, cert_crt) == payload
 
     jwt = encode_jwt(payload, cert_key, cert=cert_crt)
     assert decode_jwt(jwt, cert_crt).get("Hello") == "World"
     assert get_unverified_header(jwt).get("x5t#S256") == x5t_s256(cert_crt)
+
+
+def test_jwk() -> None:
+    ca_key, ca_cert = bootstrap_ca()
+    cert_key = gen_rsa_key()
+    cert_crt = sign_csr(gen_csr(cert_key), ca_key, ca_cert)
+    cert_cwk = create_jwk_dict(cert_crt)
+    # has 9 entries
+    assert len(cert_cwk) == 9
+    # creating the jwk from the same cert, creates the same key data
+    assert cert_cwk == create_jwk_dict(cert_crt)
+    # check on specific values
+    assert cert_cwk["alg"] == "sha256WithRSAEncryption"
+    assert cert_cwk["kty"] == "RSA"
+    assert cert_cwk["use"] == "sig"
+    assert cert_cwk["x5t#S256"] == x5t_s256(cert_crt)
+    assert cert_cwk["kid"] == cert_cwk["x5t#S256"]
```

### Comparing `resotolib-3.4.2/test/test_plugin.py` & `resotolib-3.5.0/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_tree.py` & `resotolib-3.5.0/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.4.2/test/test_utils.py` & `resotolib-3.5.0/test/test_utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,17 +17,21 @@
     get_local_tzinfo,
     utc_str,
     replace_env_vars,
     merge_json_elements,
     drop_deleted_attributes,
 )
 from resotolib.baseresources import BaseResource
+from resotolib.utils import stdin_generator
 from attrs import define
 from typing import ClassVar
 import pytest
+import sys
+import tempfile
+from contextlib import contextmanager
 
 
 class Writer(threading.Thread):
     def __init__(self, buffer_, rw_lock, init_sleep_time, sleep_time, to_write):
         """
         @param buffer_: common buffer_ shared by the readers and writers
         @type buffer_: list
@@ -427,7 +431,34 @@
             "bar": ["bar"],
         },
         "baz": [1, 2, 3],
         "foobar": {
             "foo": "foo",
         },
     }
+
+
+@contextmanager
+def replace_stdin(input_data: str):
+    with tempfile.TemporaryFile(mode="w+t") as temp_file:
+        temp_file.write(input_data)
+        temp_file.seek(0)
+        original_stdin = sys.stdin
+        sys.stdin = temp_file
+        try:
+            yield
+        finally:
+            sys.stdin = original_stdin
+
+
+@pytest.mark.parametrize(
+    "input_data, expected_output",
+    [
+        ("line1\nline2\nline3", ["line1", "line2", "line3"]),
+        ("line1\r\nline2\r\nline3", ["line1", "line2", "line3"]),
+        ("", []),
+    ],
+)
+def test_sync_stdin_generator(input_data, expected_output):
+    with replace_stdin(input_data):
+        output = list(stdin_generator())
+    assert output == expected_output
```

### Comparing `resotolib-3.4.2/test/test_web.py` & `resotolib-3.5.0/test/test_web.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,25 @@
-import socket
-import requests
-import time
 import os
 import tempfile
+import time
+
+import cherrypy
+import requests
+
+from resotolib.utils import get_free_port
+from resotolib.web import WebServer
+from resotolib.web.metrics import WebApp
 from resotolib.x509 import (
     gen_rsa_key,
     gen_csr,
     bootstrap_ca,
     sign_csr,
     write_cert_to_file,
     write_key_to_file,
 )
-from resotolib.web import WebServer
-from resotolib.web.metrics import WebApp
-import cherrypy
-
-
-def get_free_port() -> int:
-    tcp = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-    tcp.bind(("", 0))
-    _, free_port = tcp.getsockname()
-    tcp.close()
-    return free_port
 
 
 def test_web():
     # Find a free local port to reuse when we bind the web server.
     # This is so that multiple builds/tests can run in parallel
     # on the same CI agent.
     # todo: race between closing socket and reusing free port in WebServer
@@ -87,8 +81,7 @@
         endpoint = f"https://localhost:{free_port}"
         r = requests.get(f"{endpoint}/health", verify=ca_cert_path)
         assert r.text == "ok\r\n"
         web_server.shutdown()
         while web_server.is_alive():
             print("Waiting for web server to shutdown")
             time.sleep(1)
-        cherrypy.engine
```

### Comparing `resotolib-3.4.2/test/test_x509.py` & `resotolib-3.5.0/test/test_x509.py`

 * *Files identical despite different names*

