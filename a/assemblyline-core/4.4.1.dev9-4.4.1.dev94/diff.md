# Comparing `tmp/assemblyline-core-4.4.1.dev9.tar.gz` & `tmp/assemblyline-core-4.4.1.dev94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "assemblyline-core-4.4.1.dev9.tar", last modified: Fri Mar 24 16:14:11 2023, max compression
+gzip compressed data, was "assemblyline-core-4.4.1.dev94.tar", last modified: Thu May 25 21:44:22 2023, max compression
```

## Comparing `assemblyline-core-4.4.1.dev9.tar` & `assemblyline-core-4.4.1.dev94.tar`

### file list

```diff
@@ -1,101 +1,101 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.302348 assemblyline-core-4.4.1.dev9/
--rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/LICENCE.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1680 2023-03-24 16:14:11.302348 assemblyline-core-4.4.1.dev9/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      860 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.290348 assemblyline-core-4.4.1.dev9/assemblyline_core/
--rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-03-24 16:14:10.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/VERSION
--rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.290348 assemblyline-core-4.4.1.dev9/assemblyline_core/alerter/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/alerter/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15689 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/alerter/processing.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/alerter/run_alerter.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.290348 assemblyline-core-4.4.1.dev9/assemblyline_core/archiver/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/archiver/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6167 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/archiver/run_archiver.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.290348 assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      122 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    16929 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/client.py
--rw-r--r--   0 vsts      (1001) docker     (122)    79585 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6401 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/schedules.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/timeout.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.290348 assemblyline-core-4.4.1.dev9/assemblyline_core/expiry/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/expiry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13558 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/expiry/run_expiry.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.298348 assemblyline-core-4.4.1.dev9/assemblyline_core/ingester/
--rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/ingester/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/ingester/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/ingester/constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35888 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/ingester/ingester.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.298348 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    30681 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/es_metrics.py
--rw-r--r--   0 vsts      (1001) docker     (122)    13019 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/heartbeat_formatter.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7559 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/helper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    17144 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/metrics_server.py
--rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/run_heartbeat_manager.py
--rw-r--r--   0 vsts      (1001) docker     (122)      250 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/run_metrics_aggregator.py
--rw-r--r--   0 vsts      (1001) docker     (122)      274 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/run_statistics_aggregator.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.298348 assemblyline-core-4.4.1.dev9/assemblyline_core/plumber/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/plumber/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6434 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/plumber/run_plumber.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.298348 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12345 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.298348 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/creator/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/creator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2168 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/creator/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4743 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/creator/run_worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.298348 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/loader/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/loader/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3533 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/loader/run.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/loader/run_worker.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2577 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/replay/replay.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2498 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/safelist_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.298348 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1858 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/collection.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.302348 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/controllers/
--rw-r--r--   0 vsts      (1001) docker     (122)       90 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    24018 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/controllers/docker_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2174 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/controllers/interface.py
--rw-r--r--   0 vsts      (1001) docker     (122)    52980 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/controllers/kubernetes_ctl.py
--rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/run_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    47769 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/scaler_server.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11969 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/server_base.py
--rw-r--r--   0 vsts      (1001) docker     (122)    10353 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/submission_client.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21921 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/tasking_client.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.302348 assemblyline-core-4.4.1.dev9/assemblyline_core/updater/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/updater/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8093 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/updater/helper.py
--rw-r--r--   0 vsts      (1001) docker     (122)    32095 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/updater/run_updater.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.302348 assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5628 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/crawler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/department_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/safelist.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/stream_map.py
--rw-r--r--   0 vsts      (1001) docker     (122)    29142 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/worker.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.302348 assemblyline-core-4.4.1.dev9/assemblyline_core/workflow/
--rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9532 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/assemblyline_core/workflow/run_workflow.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.290348 assemblyline-core-4.4.1.dev9/assemblyline_core.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1680 2023-03-24 16:14:11.000000 assemblyline-core-4.4.1.dev9/assemblyline_core.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     2975 2023-03-24 16:14:11.000000 assemblyline-core-4.4.1.dev9/assemblyline_core.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-03-24 16:14:11.000000 assemblyline-core-4.4.1.dev9/assemblyline_core.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       85 2023-03-24 16:14:11.000000 assemblyline-core-4.4.1.dev9/assemblyline_core.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-03-24 16:14:11.000000 assemblyline-core-4.4.1.dev9/assemblyline_core.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-03-24 16:14:11.322348 assemblyline-core-4.4.1.dev9/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1941 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-03-24 16:14:11.302348 assemblyline-core-4.4.1.dev9/test/
--rw-r--r--   0 vsts      (1001) docker     (122)     5768 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/test/test_alerter.py
--rw-r--r--   0 vsts      (1001) docker     (122)    14866 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_dispatcher.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2043 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_expiry.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_plumber.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6995 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_replay.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2006 2023-03-24 16:13:56.000000 assemblyline-core-4.4.1.dev9/test/test_scaler.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5313 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_scheduler.py
--rw-r--r--   0 vsts      (1001) docker     (122)    38477 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_simulation.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_vacuum.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6776 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_worker_ingest.py
--rw-r--r--   0 vsts      (1001) docker     (122)     4780 2023-03-24 16:13:58.000000 assemblyline-core-4.4.1.dev9/test/test_worker_submit.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.720460 assemblyline-core-4.4.1.dev94/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1396 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/LICENCE.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-25 21:44:22.720460 assemblyline-core-4.4.1.dev94/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      860 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.664459 assemblyline-core-4.4.1.dev94/assemblyline_core/
+-rw-r--r--   0 vsts      (1001) docker     (122)       12 2023-05-25 21:44:21.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/VERSION
+-rw-r--r--   0 vsts      (1001) docker     (122)       49 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.668459 assemblyline-core-4.4.1.dev94/assemblyline_core/alerter/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/alerter/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15689 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/alerter/processing.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4871 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/alerter/run_alerter.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.668459 assemblyline-core-4.4.1.dev94/assemblyline_core/archiver/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/archiver/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8210 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/archiver/run_archiver.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.676459 assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      122 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16929 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/client.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    83163 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7289 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/schedules.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2050 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/timeout.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.676459 assemblyline-core-4.4.1.dev94/assemblyline_core/expiry/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/expiry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13558 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/expiry/run_expiry.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.676459 assemblyline-core-4.4.1.dev94/assemblyline_core/ingester/
+-rw-r--r--   0 vsts      (1001) docker     (122)       54 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/ingester/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/ingester/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      182 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/ingester/constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35958 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/ingester/ingester.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.684459 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    30681 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/es_metrics.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    13019 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/heartbeat_formatter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7559 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    17144 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/metrics_server.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      256 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/run_heartbeat_manager.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      250 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/run_metrics_aggregator.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      274 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/run_statistics_aggregator.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.684459 assemblyline-core-4.4.1.dev94/assemblyline_core/plumber/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/plumber/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6434 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/plumber/run_plumber.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.684459 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12345 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.688459 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/creator/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/creator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2168 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/creator/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4743 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/creator/run_worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.688459 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/loader/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/loader/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3533 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/loader/run.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2999 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/loader/run_worker.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2577 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/replay/replay.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2498 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/safelist_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.692459 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1858 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/collection.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.700459 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (122)       90 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    24018 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/controllers/docker_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2174 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/controllers/interface.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    53877 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/controllers/kubernetes_ctl.py
+-rw-r--r--   0 vsts      (1001) docker     (122)      160 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/run_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    48567 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/scaler_server.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12219 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/server_base.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    10353 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/submission_client.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    22003 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/tasking_client.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.700459 assemblyline-core-4.4.1.dev94/assemblyline_core/updater/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/updater/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8093 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/updater/helper.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    32152 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/updater/run_updater.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.708459 assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5628 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/crawler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2675 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/department_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3478 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/safelist.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3136 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/stream_map.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    29284 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/worker.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.708459 assemblyline-core-4.4.1.dev94/assemblyline_core/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9532 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/assemblyline_core/workflow/run_workflow.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.664459 assemblyline-core-4.4.1.dev94/assemblyline_core.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1681 2023-05-25 21:44:22.000000 assemblyline-core-4.4.1.dev94/assemblyline_core.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     2975 2023-05-25 21:44:22.000000 assemblyline-core-4.4.1.dev94/assemblyline_core.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-05-25 21:44:22.000000 assemblyline-core-4.4.1.dev94/assemblyline_core.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       66 2023-05-25 21:44:22.000000 assemblyline-core-4.4.1.dev94/assemblyline_core.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       18 2023-05-25 21:44:22.000000 assemblyline-core-4.4.1.dev94/assemblyline_core.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       70 2023-05-25 21:44:22.720460 assemblyline-core-4.4.1.dev94/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1870 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-05-25 21:44:22.720460 assemblyline-core-4.4.1.dev94/test/
+-rw-r--r--   0 vsts      (1001) docker     (122)     5768 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/test/test_alerter.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    15228 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_dispatcher.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2043 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_expiry.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2506 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_plumber.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6995 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_replay.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2006 2023-05-25 21:44:06.000000 assemblyline-core-4.4.1.dev94/test/test_scaler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5313 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_scheduler.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    38685 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_simulation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4419 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_vacuum.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6792 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_worker_ingest.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4780 2023-05-25 21:44:07.000000 assemblyline-core-4.4.1.dev94/test/test_worker_submit.py
```

### Comparing `assemblyline-core-4.4.1.dev9/LICENCE.md` & `assemblyline-core-4.4.1.dev94/LICENCE.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/PKG-INFO` & `assemblyline-core-4.4.1.dev94/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.4.1.dev9
+Version: 4.4.1.dev94
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-core-4.4.1.dev9/README.md` & `assemblyline-core-4.4.1.dev94/README.md`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/alerter/processing.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/alerter/processing.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/alerter/run_alerter.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/alerter/run_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/client.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/dispatcher.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,34 +12,36 @@
 import dataclasses
 
 import elasticapm
 
 from assemblyline.common import isotime
 from assemblyline.common.constants import make_watcher_list_name, SUBMISSION_QUEUE, \
     DISPATCH_RUNNING_TASK_HASH, SCALER_TIMEOUT_QUEUE, DISPATCH_TASK_HASH
-from assemblyline.common.forge import get_service_queue, get_apm_client
+from assemblyline.common.forge import get_service_queue, get_apm_client, get_datastore, get_classification
 from assemblyline.common.isotime import now_as_iso
 from assemblyline.common.metrics import MetricsFactory
 from assemblyline.common.postprocess import ActionWorker
+from assemblyline.odm.messages.changes import ServiceChange, Operation
 from assemblyline.odm.messages.dispatcher_heartbeat import Metrics
 from assemblyline.odm.messages.service_heartbeat import Metrics as ServiceMetrics
 from assemblyline.odm.messages.dispatching import WatchQueueMessage, CreateWatch, DispatcherCommandMessage, \
     CREATE_WATCH, LIST_OUTSTANDING, UPDATE_BAD_SID, ListOutstanding
 from assemblyline.odm.messages.submission import SubmissionMessage, from_datastore_submission
 from assemblyline.odm.messages.task import FileInfo, Task as ServiceTask
 from assemblyline.odm.models.error import Error
+from assemblyline.odm.models.result import Result
 from assemblyline.odm.models.service import Service
 from assemblyline.odm.models.submission import Submission
-from assemblyline.odm.models.result import Result
+from assemblyline.odm.models.user import User
 from assemblyline.remote.datatypes.exporting_counter import export_metrics_once
+from assemblyline.remote.datatypes.events import EventWatcher
 from assemblyline.remote.datatypes.hash import Hash
-from assemblyline.remote.datatypes.set import Set
 from assemblyline.remote.datatypes.queues.comms import CommsQueue
 from assemblyline.remote.datatypes.queues.named import NamedQueue
-from assemblyline.remote.datatypes.set import ExpiringSet
+from assemblyline.remote.datatypes.set import ExpiringSet, Set
 from assemblyline.remote.datatypes.user_quota_tracker import UserQuotaTracker
 from assemblyline_core.server_base import ThreadedCoreBase
 from assemblyline_core.alerter.run_alerter import ALERT_QUEUE_NAME
 
 
 if TYPE_CHECKING:
     from assemblyline.odm.models.file import File
@@ -104,14 +106,15 @@
 
 class SubmissionTask:
     """Dispatcher internal model for submissions"""
 
     def __init__(self, submission, completed_queue, scheduler, results=None,
                  file_infos=None, file_tree=None, errors: Optional[Iterable[str]] = None):
         self.submission: Submission = Submission(submission)
+        self.submitter: User = get_datastore().user.get(self.submission.params.submitter)
 
         self.completed_queue = None
         if completed_queue:
             self.completed_queue = str(completed_queue)
 
         self.file_info: dict[str, Optional[FileInfo]] = {}
         self.file_names: dict[str, str] = {}
@@ -119,14 +122,15 @@
         self.file_tags: dict[str, dict[str, dict[str, Any]]] = defaultdict(dict)
         self.file_depth: dict[str, int] = {}
         self.file_temporary_data: dict[str, dict] = defaultdict(dict)
         self.extra_errors: list[str] = []
         self.active_files: set[str] = set()
         self.dropped_files: set[str] = set()
         self.dynamic_recursion_bypass: set[str] = set()
+        self.service_logs: dict[tuple[str, str], list[str]] = defaultdict(list)
 
         # mapping from file hash to a set of services that shouldn't be run on
         # any children (recursively) of that file
         self._forbidden_services: dict[str, set[str]] = {}
         self._parent_map: dict[str, set[str]] = {}
 
         self.service_results: dict[tuple[str, str], ResultSummary] = {}
@@ -179,15 +183,15 @@
 
         if errors is not None:
             for e in errors:
                 sha256, service, _ = e.split('.', 2)
                 self.service_errors[(sha256, service)] = e
 
     @property
-    def sid(self):
+    def sid(self) -> str:
         return self.submission.sid
 
     def forbid_for_children(self, sha256: str, service_name: str):
         """Mark that children of a given file should not be routed to a service."""
         try:
             self._forbidden_services[sha256].add(service_name)
         except KeyError:
@@ -284,16 +288,16 @@
 
         #
         # # Build some utility classes
         self.scheduler = Scheduler(self.datastore, self.config, self.redis)
         self.running_tasks = Hash(DISPATCH_RUNNING_TASK_HASH, host=self.redis)
         self.scaler_timeout_queue = NamedQueue(SCALER_TIMEOUT_QUEUE, host=self.redis_persist)
 
-        # self.classification_engine = forge.get_classification()
-        #
+        self.classification_engine = get_classification()
+
         # Output. Duplicate our input traffic into this queue so it may be cloned by other systems
         self.traffic_queue = CommsQueue('submissions', self.redis)
         self.quota_tracker = UserQuotaTracker('submissions', timeout=60 * 60, host=self.redis_persist)
         self.submission_queue = NamedQueue(SUBMISSION_QUEUE, self.redis)
 
         # Table to track the running dispatchers
         self.dispatchers_directory: Hash[int] = Hash(DISPATCH_DIRECTORY, host=self.redis_persist)
@@ -343,38 +347,71 @@
         self.postprocess_worker = ActionWorker(cache=False, config=self.config, datastore=self.datastore,
                                                redis_persist=self.redis_persist)
 
         # Update bad sid list
         self.redis_bad_sids = Set(BAD_SID_HASH, host=self.redis_persist)
         self.bad_sids: set[str] = set(self.redis_bad_sids.members())
 
+        # Event Watchers
+        self.service_change_watcher = EventWatcher(self.redis, deserializer=ServiceChange.deserialize)
+        self.service_change_watcher.register('changes.services.*', self._handle_service_change_event)
+
+
     def stop(self):
         super().stop()
+        self.service_change_watcher.stop()
         self.postprocess_worker.stop()
 
     def interrupt_handler(self, signum, stack_frame):
         self.log.info("Instance caught signal. Beginning to drain work.")
         self.finalizing_start = time.time()
         self._shutdown_timeout = AL_SHUTDOWN_QUIT
         self.finalizing.set()
         self.dispatchers_directory_finalize.set(self.instance_id, int(time.time()))
 
+    def _handle_status_change(self, status: Optional[bool]):
+        super()._handle_status_change(status)
+
+        # If we may have lost redis connection check all of our submissions
+        if status is None:
+            for sid in self.tasks.keys():
+                _q = self.find_process_queue(sid)
+                _q.put(DispatchAction(kind=Action.check_submission, sid=sid))
+
+    def _handle_service_change_event(self, data: ServiceChange):
+        if data.operation == Operation.Removed:
+            # Remove all current instances of service from scheduler cache
+            [service_set.remove(data.name) for service_set in self.scheduler.c12n_services.values()
+             if data.name in service_set]
+        else:
+            # If Added/Modifed, pull the service information and modify cache
+            service: Service = self.datastore.get_service_with_delta(data.name)
+            for c12n, service_set in self.scheduler.c12n_services.items():
+                if self.classification_engine.is_accessible(c12n, service.classification):
+                    # Classification group is allowed to use this service
+                    service_set.add(service.name)
+                else:
+                    # Classification group isn't allowed to use this service
+                    if service.name in service_set:
+                        service_set.remove(service.name)
+
     def process_queue_index(self, key: str) -> int:
         return sum(ord(_x) for _x in key) % RESULT_THREADS
 
     def find_process_queue(self, key: str):
         return self.process_queues[self.process_queue_index(key)]
 
     def service_worker_factory(self, index: int):
         def service_worker():
             return self.service_worker(index)
         return service_worker
 
     def try_run(self):
         self.log.info(f'Using dispatcher id {self.instance_id}')
+        self.service_change_watcher.start()
         threads = {
             # Pull in new submissions
             'Pull Submissions': self.pull_submissions,
             # pull start messages
             'Pull Service Start': self.pull_service_starts,
             # pull result messages
             'Pull Service Result': self.pull_service_results,
@@ -523,23 +560,68 @@
                 self.log.warning(f"[{sid}] could not process initialization data: {err}")
 
         self.tasks[sid] = task
         self._submission_timeouts.set(task.sid, SUBMISSION_TOTAL_TIMEOUT, None)
 
         task.file_depth[sha256] = 0
         task.file_names[sha256] = submission.files[0].name or sha256
+
         # Initialize ancestry chain by identifying the root file
-        task.file_temporary_data[sha256]['ancestry'] = [[dict(type=self.datastore.file.get(sha256).type,
-                                                              parent_relation="ROOT",
-                                                              sha256=sha256)]]
+        file_info = self.get_fileinfo(task, sha256)
+        file_type = file_info.type if file_info else 'NOT_FOUND'
+        task.file_temporary_data[sha256]['ancestry'] = [[dict(type=file_type, parent_relation="ROOT", sha256=sha256)]]
+
+        # Start the file dispatching
         task.active_files.add(sha256)
         action = DispatchAction(kind=Action.dispatch_file, sid=sid, sha=sha256)
         self.find_process_queue(sid).put(action)
 
     @elasticapm.capture_span(span_type='dispatcher')
+    def get_fileinfo(self, task: SubmissionTask, sha256: str) -> Optional[FileInfo]:
+        # First try to get the info from local cache
+        file_info = task.file_info.get(sha256, None)
+        if file_info:
+            return file_info
+
+        # get the info from datastore
+        filestore_info: Optional[File] = self.datastore.file.get(sha256)
+
+        if filestore_info is None:
+            # Store an error and mark this file as unprocessable
+            task.dropped_files.add(sha256)
+            self._dispatching_error(task, Error({
+                'archive_ts': None,
+                'expiry_ts': task.submission.expiry_ts,
+                'response': {
+                    'message': f"Couldn't find file info for {sha256} in submission {task.sid}",
+                    'service_name': 'Dispatcher',
+                    'service_tool_version': '4.0',
+                    'service_version': '4.0',
+                    'status': 'FAIL_NONRECOVERABLE'
+                },
+                'sha256': sha256,
+                'type': 'UNKNOWN'
+            }))
+            task.file_info[sha256] = None
+            task.file_schedules[sha256] = []
+            return None
+        else:
+            # Translate the file info format
+            file_info = task.file_info[sha256] = FileInfo(dict(
+                magic=filestore_info.magic,
+                md5=filestore_info.md5,
+                mime=filestore_info.mime,
+                sha1=filestore_info.sha1,
+                sha256=filestore_info.sha256,
+                size=filestore_info.size,
+                type=filestore_info.type,
+            ))
+        return file_info
+
+    @elasticapm.capture_span(span_type='dispatcher')
     def dispatch_file(self, task: SubmissionTask, sha256: str) -> bool:
         """
         Dispatch to any outstanding services for the given file.
         If nothing can be dispatched, check if the submission is finished.
 
         :param task: Submission task object.
         :param sha256: hash of the file to check.
@@ -550,57 +632,30 @@
         sid = submission.sid
         if self.apm_client:
             elasticapm.label(sid=sid, sha256=sha256)
 
         file_depth: int = task.file_depth[sha256]
         # If its the first time we've seen this file, we won't have a schedule for it
         if sha256 not in task.file_schedules:
-            with elasticapm.capture_span('build_schedule'):
-                # We are processing this file, load the file info, and build the schedule
-                filestore_info: Optional[File] = self.datastore.file.get(sha256)
-
-                if filestore_info is None:
-                    task.dropped_files.add(sha256)
-                    self._dispatching_error(task, Error({
-                        'archive_ts': None,
-                        'expiry_ts': task.submission.expiry_ts,
-                        'response': {
-                            'message': f"Couldn't find file info for {sha256} in submission {sid}",
-                            'service_name': 'Dispatcher',
-                            'service_tool_version': '4.0',
-                            'service_version': '4.0',
-                            'status': 'FAIL_NONRECOVERABLE'
-                        },
-                        'sha256': sha256,
-                        'type': 'UNKNOWN'
-                    }))
-                    task.file_info[sha256] = None
-                    task.file_schedules[sha256] = []
-                    return False
-                else:
-                    file_info = task.file_info[sha256] = FileInfo(dict(
-                        magic=filestore_info.magic,
-                        md5=filestore_info.md5,
-                        mime=filestore_info.mime,
-                        sha1=filestore_info.sha1,
-                        sha256=filestore_info.sha256,
-                        size=filestore_info.size,
-                        type=filestore_info.type,
-                    ))
-
-                    forbidden_services = None
+            # We are processing this file, load the file info, and build the schedule
+            file_info = self.get_fileinfo(task, sha256)
+            if file_info is None:
+                return False
 
-                    # If Dynamic Recursion Prevention is in effect and the file is not part of the bypass list,
-                    # Find the list of services this file is forbidden from being sent to.
-                    ignore_drp = submission.params.ignore_dynamic_recursion_prevention
-                    if not ignore_drp and sha256 not in task.dynamic_recursion_bypass:
-                        forbidden_services = task.find_recursion_excluded_services(sha256)
+            forbidden_services = None
 
-                    task.file_schedules[sha256] = self.scheduler.build_schedule(submission, file_info.type,
-                                                                                file_depth, forbidden_services)
+            # If Dynamic Recursion Prevention is in effect and the file is not part of the bypass list,
+            # Find the list of services this file is forbidden from being sent to.
+            ignore_drp = submission.params.ignore_dynamic_recursion_prevention
+            if not ignore_drp and sha256 not in task.dynamic_recursion_bypass:
+                forbidden_services = task.find_recursion_excluded_services(sha256)
+
+            task.file_schedules[sha256] = self.scheduler.build_schedule(submission, file_info.type,
+                                                                        file_depth, forbidden_services,
+                                                                        task.submitter.classification.value)
 
         file_info = task.file_info[sha256]
         schedule: list = list(task.file_schedules[sha256])
         deep_scan, ignore_filtering = submission.params.deep_scan, submission.params.ignore_filtering
 
         # Go through each round of the schedule removing complete/failed services
         # Break when we find a stage that still needs processing
@@ -713,16 +768,17 @@
                         priority=submission.params.priority,
                         safelist_config=self.config.services.safelist
                     ))
                     service_task.metadata['dispatcher__'] = self.instance_id
 
                     # Its a new task, send it to the service
                     queue_key = service_queue.push(service_task.priority, service_task.as_primitives())
-                    task.queue_keys[(sha256, service_name)] = queue_key
+                    task.queue_keys[key] = queue_key
                     sent.append(service_name)
+                    task.service_logs[key].append(f'Submitted to queue at {now_as_iso()}')
 
             if sent or enqueued or running:
                 # If we have confirmed that we are waiting, or have taken an action, log that.
                 self.log.info(f"[{sid}] File {sha256} sent to: {sent} "
                               f"already in queue for: {enqueued} "
                               f"running on: {running}")
                 return False
@@ -973,21 +1029,26 @@
         # Count the submission as 'complete' either way
         self.counter.increment('submissions_completed')
 
     def retry_error(self, task: SubmissionTask, sha256, service_name):
         self.log.warning(f"[{task.submission.sid}/{sha256}] "
                          f"{service_name} marking task failed: TASK PREEMPTED ")
 
+        # Pull out any details to include in error message
+        error_details = '\n'.join(task.service_logs[(sha256, service_name)])
+        if error_details:
+            error_details = '\n\n' + error_details
+
         ttl = task.submission.params.ttl
         error = Error(dict(
             archive_ts=None,
             created='NOW',
             expiry_ts=now_as_iso(ttl * 24 * 60 * 60) if ttl else None,
             response=dict(
-                message='The number of retries has passed the limit.',
+                message='The number of retries has passed the limit.' + error_details,
                 service_name=service_name,
                 service_version='0',
                 status='FAIL_NONRECOVERABLE',
             ),
             sha256=sha256, type="TASK PRE-EMPTED",
         ))
 
@@ -1071,14 +1132,16 @@
                     key = (message.sha, message.service_name)
                     if task.queue_keys.pop(key, None) is not None:
                         # If this task is already finished (result message processed before start
                         # message) we can skip setting a timeout
                         if key in task.service_errors or key in task.service_results:
                             continue
                         self.set_timeout(task, message.sha, message.service_name, message.worker_id)
+                        task.service_logs[(message.sha, message.service_name)].append(
+                            f'Popped from queue and running at {now_as_iso()} on worker {message.worker_id}')
 
             elif kind == Action.result:
                 self.queue_ready_signals[self.process_queue_index(message.sid)].release()
                 with apm_span(self.apm_client, "dispatcher_results"):
                     task = self.tasks.get(message.sid)
                     if not task:
                         self.log.warning(f'[{message.sid}] Result returned for finished task.')
@@ -1099,15 +1162,22 @@
 
                         # If we didn't finish the submission here, wait another 20 minutes
                         if message.sid in self.tasks:
                             self._submission_timeouts.set(message.sid, SUBMISSION_TOTAL_TIMEOUT, None)
 
             elif kind == Action.service_timeout:
                 task = self.tasks.get(message.sid)
+
+                if not message.sha or not message.service_name:
+                    self.log.warning(f'[{message.sid}] Service timeout missing data.')
+                    continue
+
                 if task:
+                    task.service_logs[(message.sha, message.service_name)].append(
+                        f'Service timeout at {now_as_iso()} on worker {message.worker_id}')
                     self.timeout_service(task, message.sha, message.service_name, message.worker_id)
 
             elif kind == Action.dispatch_file:
                 task = self.tasks.get(message.sid)
                 if task:
                     self.dispatch_file(task, message.sha)
 
@@ -1148,14 +1218,15 @@
             return
 
         # Add SHA256s of files that allowed to run regardless of Dynamic Recursion Prevention
         task.dynamic_recursion_bypass = task.dynamic_recursion_bypass.union(set(dynamic_recursion_bypass))
 
         # Immediately remove timeout so we don't cancel now
         self.clear_timeout(task, sha256, service_name)
+        task.service_logs.pop((sha256, service_name), None)
 
         # Don't process duplicates
         if (sha256, service_name) in task.service_results:
             return
 
         # Let the logs know we have received a result for this task
         if summary.drop:
@@ -1245,16 +1316,18 @@
                         }))
                         continue
 
                     dispatched += 1
                     task.active_files.add(extracted_sha256)
                     parent_ancestry = parent_data['ancestry']
                     existing_ancestry = task.file_temporary_data.get(extracted_sha256, {}).get('ancestry', [])
-                    current_ancestry_node = dict(type=self.datastore.file.get(extracted_sha256).type,
-                                                 parent_relation=parent_relation, sha256=extracted_sha256)
+                    file_info = self.get_fileinfo(task, extracted_sha256)
+                    file_type = file_info.type if file_info else 'NOT_FOUND'
+                    current_ancestry_node = dict(type=file_type, parent_relation=parent_relation,
+                                                 sha256=extracted_sha256)
 
                     task.file_temporary_data[extracted_sha256] = dict(parent_data)
                     task.file_temporary_data[extracted_sha256]['ancestry'] = existing_ancestry
                     [task.file_temporary_data[extracted_sha256]['ancestry'].append(ancestry + [current_ancestry_node])
                      for ancestry in parent_ancestry]
                     self.find_process_queue(sid).put(DispatchAction(kind=Action.dispatch_file, sid=sid,
                                                                     sha=extracted_sha256))
@@ -1292,19 +1365,23 @@
         task.extra_errors.append(error_key)
         self.error_queue.put((error_key, error))
         msg = {'status': 'FAIL', 'cache_key': error_key}
         for w in self._watcher_list(task.submission.sid).members():
             NamedQueue(w).push(msg)
 
     @elasticapm.capture_span(span_type='dispatcher')
-    def process_service_error(self, task: SubmissionTask, error_key, error):
+    def process_service_error(self, task: SubmissionTask, error_key, error: Error):
         self.log.info(f'[{task.submission.sid}] Error from service {error.response.service_name} on {error.sha256}')
         self.clear_timeout(task, error.sha256, error.response.service_name)
+        key = (error.sha256, error.response.service_name)
         if error.response.status == "FAIL_NONRECOVERABLE":
-            task.service_errors[(error.sha256, error.response.service_name)] = error_key
+            task.service_errors[key] = error_key
+            task.service_logs.pop(key, None)
+        else:
+            task.service_logs[key].append(f"Service error: {error.response.message}")
         self.dispatch_file(task, error.sha256)
 
     def pull_service_starts(self):
         start_queue = self.start_queue
         cpu_mark = time.process_time()
         time_mark = time.time()
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/schedules.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/schedules.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,41 +1,48 @@
 from __future__ import annotations
-from typing import Dict, Optional, cast
+from typing import Dict, Optional, Set, cast
 
 import logging
 import os
 import re
 
-from assemblyline.common.forge import CachedObject
+from assemblyline.common.forge import CachedObject, get_classification
 from assemblyline.datastore.helper import AssemblylineDatastore
 from assemblyline.odm.models.config import Config
 from assemblyline.odm.models.service import Service
 from assemblyline.odm.models.submission import Submission
 from assemblyline_core.server_base import get_service_stage_hash, ServiceStage
 
 
 # If you are doing development and you want the system to route jobs ignoring the service setup/teardown
 # set an environment variable SKIP_SERVICE_SETUP to true for all dispatcher containers
 SKIP_SERVICE_SETUP = os.environ.get('SKIP_SERVICE_SETUP', 'false').lower() in ['true', '1']
 
+Classification = get_classification()
 
 class Scheduler:
     """This object encapsulates building the schedule for a given file type for a submission."""
 
     def __init__(self, datastore: AssemblylineDatastore, config: Config, redis):
         self.datastore = datastore
         self.config = config
-        self._services: dict[str, Service] = {}
+        self._services: Dict[str, Service] = {}
         self.services = cast(Dict[str, Service], CachedObject(self._get_services))
         self.service_stage = get_service_stage_hash(redis)
+        self.c12n_services: Dict[str, Set[str]] = {}
 
     def build_schedule(self, submission: Submission, file_type: str, file_depth: int = 0,
-                       runtime_excluded: Optional[list[str]] = None) -> list[dict[str, Service]]:
+                       runtime_excluded: Optional[list[str]] = None,
+                       submitter_c12n: str = Classification.UNRESTRICTED) -> list[dict[str, Service]]:
+        # Get the set of all services currently enabled on the system
         all_services = dict(self.services)
 
+        # Retrieve a list of services that the classfication group is allowed to submit to
+        accessible = self.get_accessible_services(submitter_c12n)
+
         # Load the selected and excluded services by category
         excluded = self.expand_categories(submission.params.services.excluded)
         runtime_excluded = self.expand_categories(runtime_excluded or [])
         if not submission.params.services.selected:
             selected = [s for s in all_services.keys()]
         else:
             selected = self.expand_categories(submission.params.services.selected)
@@ -51,15 +58,15 @@
                 not self.config.services.safelist.enforce_safelist_service \
                 and not (submission.params.deep_scan or submission.params.ignore_filtering):
             # Alter schedule to remove Safelist, if scheduled to run
             selected.remove("Safelist")
 
         # Add all selected, accepted, and not rejected services to the schedule
         schedule: list[dict[str, Service]] = [{} for _ in self.config.services.stages]
-        services = list(set(selected) - set(excluded) - set(runtime_excluded))
+        services = list(set(selected).intersection(accessible) - set(excluded) - set(runtime_excluded))
         selected = []
         skipped = []
         for name in services:
             service = all_services.get(name, None)
 
             if not service:
                 skipped.append(name)
@@ -115,14 +122,22 @@
         for service in self.services.values():
             try:
                 all_categories[service.category].append(service.name)
             except KeyError:
                 all_categories[service.category] = [service.name]
         return all_categories
 
+    def get_accessible_services(self, user_c12n: str) -> Set[str]:
+        if not self.c12n_services.get(user_c12n):
+            # Cache services that are accessible to a classification group
+            self.c12n_services[user_c12n] = {_ for _, service in dict(self.services).items()
+                                             if Classification.is_accessible(user_c12n, service.classification)}
+
+        return self.c12n_services[user_c12n]
+
     def stage_index(self, stage):
         return self.config.services.stages.index(stage)
 
     def _get_services(self):
         old, self._services = self._services, {}
         stages = self.service_stage.items()
         services: list[Service] = self.datastore.list_all_services(full=True)
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/dispatching/timeout.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/dispatching/timeout.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/expiry/run_expiry.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/expiry/run_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/ingester/ingester.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/ingester/ingester.py`

 * *Files 1% similar despite different names*

```diff
@@ -526,15 +526,16 @@
             self._notify_drop(task)
             self.counter.increment('skipped')
             self.log.error(f"[{task.ingest_id} :: {task.sha256}] {task.failure}")
             return
 
         # Set the groups from the user, if they aren't already set
         if not task.params.groups:
-            task.params.groups = self.get_groups_from_user(task.params.submitter)
+            task.params.groups = [g for g in self.get_groups_from_user(
+                task.params.submitter) if g in str(task.params.classification)]
 
         # Check if this file is already being processed
         self.stamp_filescore_key(task)
         pprevious, previous, score = None, None, None
         if not param.ignore_cache:
             pprevious, previous, score, _ = self.check(task, count_miss=False)
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/es_metrics.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/es_metrics.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/heartbeat_formatter.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/heartbeat_formatter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/helper.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/metrics/metrics_server.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/metrics/metrics_server.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/plumber/run_plumber.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/plumber/run_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/replay/client.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/replay/client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/replay/creator/run.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/replay/creator/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/replay/creator/run_worker.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/replay/creator/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/replay/loader/run.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/replay/loader/run.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/replay/loader/run_worker.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/replay/loader/run_worker.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/replay/replay.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/replay/replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/safelist_client.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/safelist_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/collection.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/collection.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/controllers/docker_ctl.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/controllers/docker_ctl.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/controllers/interface.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/controllers/interface.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/controllers/kubernetes_ctl.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/controllers/kubernetes_ctl.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,17 @@
     if string.endswith('m'):
         return float(string[:-1])/1000.0
 
     raise ValueError('Un-parsable CPU string: ' + string)
 
 
 class KubernetesController(ControllerInterface):
-    def __init__(self, logger, namespace, prefix, priority, cpu_reservation, labels=None,
-                 log_level="INFO", core_env={}, default_service_account=None):
+    def __init__(self, logger, namespace: str, prefix: str, priority: str, dependency_priority: str,
+                 cpu_reservation: float, labels=None, log_level="INFO", core_env={},
+                 default_service_account=None):
         # Try loading a kubernetes connection from either the fact that we are running
         # inside of a cluster, or have a config file that tells us how
         try:
             config.load_incluster_config()
         except config.config_exception.ConfigException:
             # Load the configuration once to initialize the defaults
             config.load_kube_config()
@@ -184,14 +185,15 @@
 
             # Load again with our settings set
             config.load_kube_config(client_configuration=cfg)
 
         self.running: bool = True
         self.prefix: str = prefix.lower()
         self.priority: str = priority
+        self.dependency_priority: str = dependency_priority
         self.cpu_reservation: float = max(0.0, min(cpu_reservation, 1.0))
         self.logger = logger
         self.log_level: str = log_level
         self._labels: dict[str, str] = labels or {}
         self.apps_api = client.AppsV1Api()
         self.api = client.CoreV1Api()
         self.net_api = client.NetworkingV1Api()
@@ -331,28 +333,51 @@
         return _function
 
     def _monitor_node_pool(self):
         self._node_pool_max_cpu = 0
         self._node_pool_max_ram = 0
         self.node_count = 0
         watch = TypelessWatch()
+        ready_nodes: dict[str, tuple[float, float]] = {}
 
         for event in watch.stream(func=self.api.list_node, timeout_seconds=WATCH_TIMEOUT,
                                   _request_timeout=WATCH_API_TIMEOUT):
             if not self.running:
                 break
 
-            if event['type'] == "ADDED":
-                self._node_pool_max_cpu += parse_cpu(event['raw_object']['status']['allocatable']['cpu'])
-                self._node_pool_max_ram += parse_memory(event['raw_object']['status']['allocatable']['memory'])
-                self.node_count += 1
+            name: str = event['raw_object']['metadata']['name']
+
+            if event['type'] in ["ADDED", "MODIFIED"]:
+                # Check for node ready condition
+                ready = False
+                for condition in event['raw_object']['status']['conditions']:
+                    if condition['type'] == 'Ready':
+                        ready = condition['status'] == 'True'
+                        break
+
+                if ready:
+                    cpu = parse_cpu(event['raw_object']['status']['allocatable']['cpu'])
+                    ram = parse_memory(event['raw_object']['status']['allocatable']['memory'])
+                    ready_nodes[name] = (cpu, ram)
+                else:
+                    ready_nodes.pop(name, None)
+
             elif event['type'] == "DELETED":
-                self._node_pool_max_cpu -= parse_cpu(event['raw_object']['status']['allocatable']['cpu'])
-                self._node_pool_max_ram -= parse_memory(event['raw_object']['status']['allocatable']['memory'])
-                self.node_count -= 1
+                # Remove deleted nodes
+                ready_nodes.pop(name, None)
+
+            # Update the totals
+            self.node_count = len(ready_nodes)
+            max_cpu = 0
+            max_ram = 0
+            for cpu, ram in ready_nodes.values():
+                max_cpu += cpu
+                max_ram += ram
+            self._node_pool_max_cpu = max_cpu
+            self._node_pool_max_ram = max_ram
 
     def _monitor_pods(self):
         watch = TypelessWatch()
         containers = {}
         log_cache = CacheDict(cache_len=8000)
         namespaced_containers = {}
         self._pod_used_cpu = 0
@@ -579,15 +604,15 @@
             liveness_probe=health_probe,
             readiness_probe=health_probe
         )]
 
     def _create_deployment(self, service_name: str, deployment_name: str, docker_config: DockerConfig,
                            shutdown_seconds: int, scale: int, labels: dict[str, str] = None,
                            volumes: list[V1Volume] = None, mounts: list[V1VolumeMount] = None,
-                           core_mounts: bool = False, change_key: str = '',
+                           core_mounts: bool = False, change_key: str = '', high_priority: bool = False,
                            deployment_strategy: V1DeploymentStrategy = V1DeploymentStrategy()):
         # Build a cache key to check for changes, just trying to only patch what changed
         # will still potentially result in a lot of restarts due to different kubernetes
         # systems returning differently formatted data
         lbls = sorted((labels or {}).items())
         svc_env = sorted(self._service_limited_env[service_name].items())
         change_key = str(f"n={deployment_name}{change_key}dc={docker_config}ss={shutdown_seconds}"
@@ -690,15 +715,15 @@
             ))
 
         pod = V1PodSpec(
             init_containers=init_containers,
             volumes=all_volumes,
             containers=self._create_containers(service_name, deployment_name, docker_config,
                                                all_mounts, core_container=core_mounts),
-            priority_class_name=self.priority,
+            priority_class_name=self.dependency_priority if high_priority else self.priority,
             termination_grace_period_seconds=shutdown_seconds,
             security_context=V1PodSecurityContext(fs_group=1000),
             service_account_name=service_account,
         )
 
         if use_pull_secret:
             pod.image_pull_secrets = [V1LocalObjectReference(name=pull_secret_name)]
@@ -910,15 +935,15 @@
             if error.status != 404:
                 raise
 
         # Setup the deployment itself
         labels['container'] = container_name
         spec.container.environment.append({'name': 'AL_INSTANCE_KEY', 'value': instance_key})
         self._create_deployment(service_name, deployment_name, spec.container,
-                                30, 1, labels, volumes=volumes, mounts=mounts,
+                                30, 1, labels, volumes=volumes, mounts=mounts, high_priority=True,
                                 core_mounts=spec.run_as_core, change_key=change_key,
                                 deployment_strategy=deployment_strategy)
 
         # Setup a service to direct to the deployment
         try:
             service = self.api.read_namespaced_service(deployment_name, self.namespace)
             service.metadata.labels = labels
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/scaler/scaler_server.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/scaler/scaler_server.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,14 +257,15 @@
                          redis=redis, redis_persist=redis_persist)
 
         self.scaler_timeout_queue = NamedQueue(SCALER_TIMEOUT_QUEUE, host=self.redis_persist)
         self.error_count_lock = threading.Lock()
         self.error_count: dict[str, list[float]] = {}
         self.status_table = ExpiringHash(SERVICE_STATE_HASH, host=self.redis, ttl=30*60)
         self.service_event_sender = EventSender('changes.services', host=self.redis)
+        self.service_watcher_wakeup = threading.Event()
         self.service_change_watcher = EventWatcher(self.redis, deserializer=ServiceChange.deserialize)
         self.service_change_watcher.register('changes.services.*', self._handle_service_change_event)
 
         core_env: dict[str, str] = {}
         # If we have privileged services, we must be able to pass the necessary environment variables for them to
         # function properly.
         for secret in re.findall(r'\${\w+}', open('/etc/assemblyline/config.yml', 'r').read()) + ['UI_SERVER']:
@@ -286,14 +287,15 @@
         if self.config.core.scaler.additional_labels:
             labels.update({k: v for k, v in (_l.split("=") for _l in self.config.core.scaler.additional_labels)})
 
         if KUBERNETES_AL_CONFIG:
             self.log.info(f"Loading Kubernetes cluster interface on namespace: {NAMESPACE}")
             self.controller = KubernetesController(logger=self.log, prefix='alsvc_', labels=labels,
                                                    namespace=NAMESPACE, priority='al-service-priority',
+                                                   dependency_priority='al-core-priority',
                                                    cpu_reservation=self.config.services.cpu_reservation,
                                                    log_level=self.config.logging.log_level,
                                                    core_env=core_env,
                                                    default_service_account=self.config.services.service_account)
 
             # Add global configuration for privileged services
             self.controller.add_config_mount(KUBERNETES_AL_CONFIG, config_map=KUBERNETES_AL_CONFIG, key="config",
@@ -418,51 +420,64 @@
             'Import Metrics': self.sync_metrics,
             'Export Metrics': self.export_metrics,
         })
 
     def stop(self):
         super().stop()
         self.service_change_watcher.stop()
+        self.service_watcher_wakeup.set()
         self.controller.stop()
 
-    def _handle_service_change_event(self, data: ServiceChange):
-        if data.operation == Operation.Removed:
-            self.log.info(f'Service appears to be deleted, removing {data.name}')
-            stage = self.get_service_stage(data.name)
-            self.stop_service(data.name, stage)
-        elif data.operation == Operation.Incompatible:
-            return
+    def _handle_service_change_event(self, data: Optional[ServiceChange]):
+        if data is None:
+            self.service_watcher_wakeup.set()
         else:
-            service = self.datastore.get_service_with_delta(data.name)
-            if not service:
-                self.log.warning(f'Received change event for non-existent service: {data.name}. Ignoring..')
+            if data.operation == Operation.Removed:
+                self.log.info(f'Service appears to be deleted, removing {data.name}')
+                stage = self.get_service_stage(data.name)
+                self.stop_service(data.name, stage)
+            elif data.operation == Operation.Incompatible:
                 return
-            self._sync_service(service)
+            else:
+                service = self.datastore.get_service_with_delta(data.name)
+                if not service:
+                    self.log.warning(f'Received change event for non-existent service: {data.name}. Ignoring..')
+                    return
+                self._sync_service(service)
 
     def sync_services(self):
         while self.running:
             with apm_span(self.apm_client, 'sync_services'):
+                self.log.info('Synchronizing service configuration')
                 with self.profiles_lock:
                     current_services = set(self.profiles.keys())
                 discovered_services: list[str] = []
 
                 # Get all the service data
                 for service in self.datastore.list_all_services(full=True):
                     self._sync_service(service)
                     discovered_services.append(service.name)
 
                 # Find any services we have running, that are no longer in the database and remove them
                 for stray_service in current_services - set(discovered_services):
                     self.log.info(f'Service appears to be deleted, removing stray {stray_service}')
                     stage = self.get_service_stage(stray_service)
                     self.stop_service(stray_service, stage)
+                self.log.info('Finish synchronizing service configuration')
 
-            self.sleep(SERVICE_SYNC_INTERVAL)
+            # Wait for the interval or until someone wakes us up
+            self.service_watcher_wakeup.wait(timeout=SERVICE_SYNC_INTERVAL)
+            self.service_watcher_wakeup.clear()
 
     def _sync_service(self, service: Service):
+        """
+        Synchronize the state of the service in the database with the orchestration environment.
+
+        :param service: Service data from the database.
+        """
         name = service.name
         stage = self.get_service_stage(service.name)
         default_settings = self.config.core.scaler.service_defaults
         image_variables: defaultdict[str, str] = defaultdict(str)
         image_variables.update(self.config.services.image_variables)
 
         def prepare_container(docker_config: DockerConfig) -> DockerConfig:
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/server_base.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/server_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,17 +232,22 @@
         self.service_info = typing.cast(typing.Dict[str, Service], forge.CachedObject(self._get_services))
         self._service_stage_hash = get_service_stage_hash(self.redis)
 
     def _get_services(self):
         # noinspection PyUnresolvedReferences
         return {x.name: x for x in self.datastore.list_all_services(full=True)}
 
-    def _handle_status_change(self, status: bool):
-        self.log.info(f"Status change detected: {status}")
-        self.active = status
+    def _handle_status_change(self, status: Optional[bool]):
+        if status is None:
+            self.log.info("Refreshing status")
+            component = self.__class__.__name__.lower()
+            self.active = Hash('system', self.redis_persist).get(f'{component}.active')
+        else:
+            self.log.info(f"Status change detected: {status}")
+            self.active = status
 
     def get_service_stage(self, service_name: str, default=ServiceStage.Off) -> ServiceStage:
         return ServiceStage(self._service_stage_hash.get(service_name) or default)
 
 
 class ThreadedCoreBase(CoreBase):
     def __init__(self, component_name: str, logger: Optional[logging.Logger] = None,
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/submission_client.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/submission_client.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/tasking_client.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/tasking_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import concurrent.futures
 import logging
 import time
-from typing import Any, Dict
+from typing import Any, Dict, Optional
 
 import elasticapm
 
 from assemblyline.common import forge
 from assemblyline.common.constants import SERVICE_STATE_HASH, ServiceStatus
 from assemblyline.common.dict_utils import flatten, unflatten
 from assemblyline.common.heuristics import HeuristicHandler, InvalidHeuristicException
@@ -65,16 +65,19 @@
                 self.cleanup = False
             else:
                 self.cleanup = True
             self.identify = identify or forge.get_identify(config=self.config, datastore=self.datastore, use_cache=True)
             self.event_listener.register('changes.heuristics', self.reload_heuristics)
             self.event_listener.start()
 
-    def reload_heuristics(self, data: dict):
-        service_name = data.get('service_name')
+    def reload_heuristics(self, data: Optional[dict]):
+        service_name = None
+        if data is not None:
+            service_name = data.get('service_name')
+
         if service_name:
             self.heuristics.update({h.heur_id: h for h in self.datastore.list_service_heuristics(service_name)})
         else:
             self.heuristics = {h.heur_id: h for h in self.datastore.list_all_heuristics()}
 
     def __enter__(self):
         return self
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/updater/helper.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/updater/helper.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/updater/run_updater.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/updater/run_updater.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 import os
 import re
 import time
 import uuid
 
 from concurrent.futures import ThreadPoolExecutor
-from typing import Any, List
+from typing import Any, List, Optional
 
 import docker
 
 from kubernetes.client import V1Job, V1ObjectMeta, V1JobSpec, V1PodTemplateSpec, V1PodSpec, V1Volume, \
     V1VolumeMount, V1EnvVar, V1Container, V1ResourceRequirements, \
     V1ConfigMapVolumeSource, V1Secret, V1SecretVolumeSource, V1LocalObjectReference
 from kubernetes import client, config
@@ -450,17 +450,18 @@
                                                         log_level=self.config.logging.log_level,
                                                         default_service_account=self.config.services.service_account)
             # Add all additional mounts to privileged services
             self.mounts = self.config.core.scaler.service_defaults.mounts
         else:
             self.controller = DockerUpdateInterface(logger=self.log, log_level=self.config.logging.log_level)
 
-    def _handle_service_change_event(self, data: ServiceChange):
-        if data.operation == Operation.Incompatible:
-            self.incompatible_services.add(data.name)
+    def _handle_service_change_event(self, data: Optional[ServiceChange]):
+        if data is not None:
+            if data.operation == Operation.Incompatible:
+                self.incompatible_services.add(data.name)
 
     def container_installs(self):
         """Go through the list of services and check what are the latest tags for it"""
         while self.running:
             self.log.info("[CI] Installing all services marked for install...")
 
             # Install function for services
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/crawler.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/crawler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/department_map.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/department_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/safelist.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/safelist.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/stream_map.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/stream_map.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/vacuum/worker.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/vacuum/worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 from typing import Optional, Any
 from multiprocessing import Lock, Event
 import threading
 
 import elasticapm
 import arrow
 
-from assemblyline.common.forge import CachedObject, get_classification, get_config, get_datastore, get_filestore, get_apm_client
+from assemblyline.common.forge import CachedObject, get_classification, get_config, get_datastore, get_filestore, \
+    get_apm_client
 from assemblyline.common.codec import decode_file
 from assemblyline.common.dict_utils import flatten
 from assemblyline.common.log import init_logging
 from assemblyline.common.metrics import MetricsFactory
 from assemblyline.datastore.helper import AssemblylineDatastore
 from assemblyline.common import identify
 from assemblyline.common.isotime import now_as_iso
@@ -408,15 +409,15 @@
                 s_params.update({
                     'classification': active_cc,
                     'ttl': 60,
                 })
                 s_params['services']['resubmit'] = ['Dynamic Analysis']
 
                 if 'groups' not in s_params:
-                    s_params['groups'] = user['groups']
+                    s_params['groups'] = [g for g in user['groups'] if g in active_cc]
 
                 # Override final parameters
                 s_params.update({
                     'generate_alert': True,
                     'max_extracted': 100,  # config.core.ingester.default_max_extracted,
                     'max_supplementary': 100,  # config.core.ingester.default_max_supplementary,
                     'priority': 100,
@@ -552,15 +553,15 @@
 
     @elasticapm.capture_span(span_type=APM_SPAN_TYPE)
     def process_file(self, meta_path: str):
         flush_file = False
         try:
             with self.timed('load_json'):
                 if not os.path.exists(meta_path):
-                    logger.warning("File %s was not found..." % meta_path)
+                    logger.info("File %s not found. Probably already processed." % meta_path)
                     self.counter.increment('skipped')
                     return
 
                 if not os.path.getsize(meta_path):
                     raise EmptyMetaException("Metadata file '%s' is empty." % meta_path)
 
                 with open(meta_path, 'rb') as fh:
@@ -613,25 +614,26 @@
         except (NotJSONException, InvalidMessageException) as nje:
             logger.warning(str(nje) + " " + meta_path)
             self.counter.increment('skipped')
         except Exception as e:
             self.counter.increment('errors')
             logger.exception("%s: %s" % (e.__class__.__name__, str(e)))
         finally:
-            with self.timed('cleanup_meta'):
-                try:
-                    if flush_file:
-                        os.unlink(meta_path)
-                    else:
-                        os.rename(meta_path, meta_path + '.bad')
-                except Exception as error:
-                    logger.exception(f"Exception caught deleting file: {meta_path} {error}")
-                finally:
-                    if os.path.exists(meta_path):
-                        logger.warning("File '%s' could not be deleted by vacuum worker" % meta_path)
+            if os.path.exists(meta_path):
+                with self.timed('cleanup_meta'):
+                    try:
+                        if flush_file:
+                            os.unlink(meta_path)
+                        else:
+                            os.rename(meta_path, meta_path + '.bad')
+                    except Exception as error:
+                        logger.exception(f"Exception caught deleting file: {meta_path} {error}")
+                    finally:
+                        if os.path.exists(meta_path):
+                            logger.warning("File '%s' could not be deleted by vacuum worker" % meta_path)
 
     def run(self):
         logger.info('Waiting for files...')
         while not stop_event.is_set():
             heartbeat(self.config)
 
             if self.ingest_queue.length() > 100000:
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core/workflow/run_workflow.py` & `assemblyline-core-4.4.1.dev94/assemblyline_core/workflow/run_workflow.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core.egg-info/PKG-INFO` & `assemblyline-core-4.4.1.dev94/assemblyline_core.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: assemblyline-core
-Version: 4.4.1.dev9
+Version: 4.4.1.dev94
 Summary: Assemblyline 4 - Core components
 Home-page: https://github.com/CybercentreCanada/assemblyline-core/
 Author: CCCS Assemblyline development team
 Author-email: assemblyline@cyber.gc.ca
 License: MIT
 Keywords: assemblyline automated malware analysis gc canada cse-cst cse cst cyber cccs
 Platform: UNKNOWN
```

### Comparing `assemblyline-core-4.4.1.dev9/assemblyline_core.egg-info/SOURCES.txt` & `assemblyline-core-4.4.1.dev94/assemblyline_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/setup.py` & `assemblyline-core-4.4.1.dev94/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,20 +40,17 @@
         'assemblyline',
         'docker',
         'kubernetes',
     ],
     extras_require={
         'test': [
             'pytest',
-            'pytest-cov',
-            'codecov',
             'assemblyline_client'
         ]
     },
     tests_require=[
         'pytest',
-        'pytest-cov',
     ],
     package_data={
         '': ["*classification.yml", "*.magic", "VERSION"]
     }
 )
```

### Comparing `assemblyline-core-4.4.1.dev9/test/test_alerter.py` & `assemblyline-core-4.4.1.dev94/test/test_alerter.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/test/test_dispatcher.py` & `assemblyline-core-4.4.1.dev94/test/test_dispatcher.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import json
 import pytest
 
 from assemblyline.common.forge import get_service_queue, get_classification
 from assemblyline.odm.models.error import Error
 from assemblyline.odm.models.file import File
 from assemblyline.odm.models.result import Result
+from assemblyline.odm.models.user import User
 from assemblyline.odm.randomizer import random_model_obj, random_minimal_obj, get_random_hash
 from assemblyline.odm import models
 from assemblyline.common.metrics import MetricsFactory
 
 from assemblyline_core.dispatching.client import DispatchClient
 from assemblyline_core.dispatching.dispatcher import Dispatcher, Submission
 from assemblyline_core.dispatching.schedules import Scheduler as RealScheduler
@@ -110,26 +111,30 @@
 @mock.patch('assemblyline_core.dispatching.dispatcher.MetricsFactory', new=mock.MagicMock(spec=MetricsFactory))
 def test_simple(clean_redis, clean_datastore):
     ds = clean_datastore
     redis = clean_redis
 
     def service_queue(name): return get_service_queue(name, redis)
 
-    file = random_model_obj(File)
+    file: File = random_model_obj(File)
     file_hash = file.sha256
     file.type = 'unknown'
     ds.file.save(file_hash, file)
 
+    user: User = random_model_obj(User)
+    ds.user.save(user.uname, user)
+
     sub: Submission = random_model_obj(models.submission.Submission)
     sub.sid = sid = 'first-submission'
     sub.params.ignore_cache = False
     sub.params.max_extracted = 5
     sub.to_be_deleted = False
     sub.params.classification = get_classification().UNRESTRICTED
     sub.params.initial_data = json.dumps({'cats': 'big'})
+    sub.params.submitter = user.uname
     sub.files = [dict(sha256=file_hash, name='file')]
 
     disp = Dispatcher(ds, redis, redis)
     disp.running = ToggleTrue()
     client = DispatchClient(ds, redis, redis)
     client.dispatcher_data_age = time.time()
     client.dispatcher_data.append(disp.instance_id)
@@ -224,24 +229,27 @@
     ds = clean_datastore
 
     # def service_queue(name): return get_service_queue(name, redis)
 
     # Setup the fake datastore
     file_hash = get_random_hash(64)
     second_file_hash = get_random_hash(64)
+    user: User = random_model_obj(User)
+    ds.user.save(user.uname, user)
 
     for fh in [file_hash, second_file_hash]:
         obj = random_model_obj(models.file.File)
         obj.sha256 = fh
         ds.file.save(fh, obj)
 
     # Inject the fake submission
     submission = random_model_obj(models.submission.Submission)
     submission.to_be_deleted = False
     submission.files = [dict(name='./file', sha256=file_hash)]
+    submission.params.submitter = user.uname
     sid = submission.sid = 'first-submission'
 
     disp = Dispatcher(ds, redis, redis)
     disp.running = ToggleTrue()
     client = DispatchClient(ds, redis, redis)
     client.dispatcher_data_age = time.time()
     client.dispatcher_data.append(disp.instance_id)
@@ -287,14 +295,17 @@
 
     # def service_queue(name): return get_service_queue(name, redis)
 
     # Setup the fake datastore
     file_hash = get_random_hash(64)
     second_file_hash = get_random_hash(64)
 
+    user: User = random_model_obj(User)
+    ds.user.save(user.uname, user)
+
     for fh in [file_hash, second_file_hash]:
         obj = random_model_obj(models.file.File)
         obj.sha256 = fh
         ds.file.save(fh, obj)
 
     # Inject the fake submission
     submission = random_model_obj(models.submission.Submission)
```

### Comparing `assemblyline-core-4.4.1.dev9/test/test_expiry.py` & `assemblyline-core-4.4.1.dev94/test/test_expiry.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/test/test_plumber.py` & `assemblyline-core-4.4.1.dev94/test/test_plumber.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/test/test_replay.py` & `assemblyline-core-4.4.1.dev94/test/test_replay.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/test/test_scaler.py` & `assemblyline-core-4.4.1.dev94/test/test_scaler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/test/test_scheduler.py` & `assemblyline-core-4.4.1.dev94/test/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/test/test_simulation.py` & `assemblyline-core-4.4.1.dev94/test/test_simulation.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 from assemblyline.common.uid import get_random_id
 from assemblyline.datastore.helper import AssemblylineDatastore
 from assemblyline.odm.models.config import Config
 from assemblyline.odm.models.error import Error
 from assemblyline.odm.models.result import Result
 from assemblyline.odm.models.service_delta import ServiceDelta
 from assemblyline.odm.models.submission import Submission
+from assemblyline.odm.models.user import User
+from assemblyline.odm.randomizer import random_model_obj
 from assemblyline.odm.messages.submission import Submission as SubmissionInput
 from assemblyline.remote.datatypes.queues.named import NamedQueue
 
 import assemblyline_core
 from assemblyline_core.plumber.run_plumber import Plumber
 from assemblyline_core.dispatching import dispatcher
 from assemblyline_core.dispatching.client import DispatchClient
@@ -231,16 +233,21 @@
             'name': svc,
             'version': '0',
             'enabled': True
         }))
         stages.set(svc, ServiceStage.Running)
         services.append(MockService(svc, ds, redis, filestore))
 
+    user = random_model_obj(User)
+    user.uname = "user"
+    ds.user.save("user", user)
+
     ds.service.commit()
     ds.service_delta.commit()
+    ds.user.commit()
 
     listed_services = ds.list_all_services(full=True)
     assert len(listed_services) == 4
 
     ingester = Ingester(datastore=ds, redis=redis, persistent_redis=redis, config=config)
 
     fields = CoreSession(config, ingester)
@@ -1005,15 +1012,15 @@
         service_delta = core.ds.service_delta.get('pre')
         service_delta['enabled'] = True
         core.ds.service_delta.save('pre', service_delta)
 
 
 def test_filter(core: CoreSession, metrics):
     from assemblyline.common.postprocess import SubmissionFilter, PostprocessAction
-    filter_string = "params.submitter: /f.*l/"
+    filter_string = "params.submitter: user"
     core.dispatcher.postprocess_worker.actions['test_process'] = \
         SubmissionFilter(filter_string), PostprocessAction({
             'enabled': True,
             'raise_alert': True,
             'filter': filter_string,
         })
 
@@ -1021,15 +1028,15 @@
         sha, size = ready_extract(core, ready_body(core)[0])
 
         core.ingest_queue.push(SubmissionInput(dict(
             metadata={},
             params=dict(
                 description="file abc123",
                 services=dict(selected=''),
-                submitter='frengl',
+                submitter='user',
                 groups=['user'],
                 max_extracted=10000,
                 generate_alert=True,
             ),
             notification=dict(
                 queue='text-filter',
                 threshold=0
@@ -1093,15 +1100,15 @@
         })
 
         core.ingest_queue.push(SubmissionInput(dict(
             metadata={},
             params=dict(
                 description="file abc123",
                 services=dict(selected=''),
-                submitter='frengl',
+                submitter='user',
                 groups=['user'],
                 max_extracted=10000,
                 generate_alert=True,
             ),
             notification=dict(
                 queue='tag-filter',
                 threshold=0
```

### Comparing `assemblyline-core-4.4.1.dev9/test/test_vacuum.py` & `assemblyline-core-4.4.1.dev94/test/test_vacuum.py`

 * *Files identical despite different names*

### Comparing `assemblyline-core-4.4.1.dev9/test/test_worker_ingest.py` & `assemblyline-core-4.4.1.dev94/test/test_worker_ingest.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 
     # Send a message that is fine, but has an illegal metadata field
     in_queue.push(make_message(dict(
         metadata={
             'tobig': 'a' * (ingester.config.submission.max_metadata_length + 2),
             'small': '100'
         }
-    ), params={'submitter': 'user', 'groups': []}))
+    ), params={'submitter': 'user', 'groups': custom_user_groups}))
 
     # Process those ok message
     ingester.running.counter = 1
     ingester.handle_ingest()
 
     # The only task that makes it through though fit these parameters
     task = ingester.unique_queue.pop()
```

### Comparing `assemblyline-core-4.4.1.dev9/test/test_worker_submit.py` & `assemblyline-core-4.4.1.dev94/test/test_worker_submit.py`

 * *Files identical despite different names*

