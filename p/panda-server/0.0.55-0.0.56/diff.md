# Comparing `tmp/panda-server-0.0.55.tar.gz` & `tmp/panda-server-0.0.56.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panda-server-0.0.55.tar", last modified: Wed May 24 13:38:53 2023, max compression
+gzip compressed data, was "panda-server-0.0.56.tar", last modified: Fri May 26 06:58:10 2023, max compression
```

## Comparing `panda-server-0.0.55.tar` & `panda-server-0.0.56.tar`

### file list

```diff
@@ -1,224 +1,224 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.810153 panda-server-0.0.55/
--rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-05-24 13:38:42.000000 panda-server-0.0.55/ChangeLog.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-24 13:38:42.000000 panda-server-0.0.55/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 13:38:42.000000 panda-server-0.0.55/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 13:38:53.810153 panda-server-0.0.55/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-24 13:38:42.000000 panda-server-0.0.55/PandaPkgInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 13:38:42.000000 panda-server-0.0.55/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.786152 panda-server-0.0.55/panda_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-24 13:38:53.000000 panda-server-0.0.55/panda_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-24 13:38:53.000000 panda-server-0.0.55/panda_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:38:53.000000 panda-server-0.0.55/panda_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 13:38:53.000000 panda-server-0.0.55/panda_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-24 13:38:53.000000 panda-server-0.0.55/panda_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-24 13:38:53.000000 panda-server-0.0.55/panda_server.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.786152 panda-server-0.0.55/pandaserver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.786152 panda-server-0.0.55/pandaserver/brokerage/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/brokerage/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/brokerage/SiteMapper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/brokerage/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/brokerage/broker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.786152 panda-server-0.0.55/pandaserver/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/config/config_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/config/daemon_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7167 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/config/panda_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.786152 panda-server-0.0.55/pandaserver/configurator/
--rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/configurator/Carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/configurator/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/configurator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/configurator/aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.786152 panda-server-0.0.55/pandaserver/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/master.py
--rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/master_systemd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.790152 panda-server-0.0.55/pandaserver/daemons/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/add_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/add_sub.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/carbon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/copyArchive.py
--rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/datasetManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/dummy_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/evpPD2P.py
--rw-r--r--   0 runner    (1001) docker     (123)    41977 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/metric_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/panda_activeusers_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/pilotStreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/process_workflow_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/recover_lost_files_daemon.py
--rw-r--r--   0 runner    (1001) docker     (123)    15074 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/task_evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/tmpwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/scripts/worker_synchronization.py
--rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/daemons/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.794153 panda-server-0.0.55/pandaserver/dataservice/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/Activator.py
--rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/AdderAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/AdderDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    40601 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/AdderGen.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/AdderPluginBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/AdderResult.py
--rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/AdderSimplePlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/Closer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/CloserAtlasPlugin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/DDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/DDMHandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/DataService.py
--rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/DataServiceUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/DynDataDistributer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/EventPicker.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/Finisher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18450 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/Notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/ProcessLimiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/RecoverLostFilesCore.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/Setupper.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   113605 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/SetupperAtlasPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/SetupperDummyPlugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/SetupperPluginBase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/eventLookupClientEI.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/dataservice/forkSetupper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.794153 panda-server-0.0.55/pandaserver/jobdispatcher/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/jobdispatcher/DispatcherUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/jobdispatcher/ErrorCode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/jobdispatcher/JobDispatcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/jobdispatcher/Protocol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/jobdispatcher/Watcher.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/jobdispatcher/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.794153 panda-server-0.0.55/pandaserver/proxycache/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/proxycache/DBMSql.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/proxycache/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/proxycache/panda_activeusers_query.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/proxycache/panda_proxy_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.794153 panda-server-0.0.55/pandaserver/server/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/server/.gacl
--rwxr-xr-x   0 runner    (1001) docker     (123)    22444 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/server/panda.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.794153 panda-server-0.0.55/pandaserver/srvcore/
--rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/srvcore/CoreUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/srvcore/MailUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/srvcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/srvcore/oidc_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/srvcore/srv_msg_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.802153 panda-server-0.0.55/pandaserver/taskbuffer/
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/CloudSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/CloudTaskSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/ConBridge.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/DBProxyPool.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/DatasetSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/DdmSpec.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/EiDBProxy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/ErrorCode.py
--rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/EventServiceUtils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/FileSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/GlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/HarvesterMetricsSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/Initializer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/JobSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/JobUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/NucleusSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)  1232528 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/OraDBProxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/PanDAMsgProcessor.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/PandaDBSchemaInfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/PrioUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/ProcessGroups.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/ResourceSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/SQLDumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/SiteSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/SupErrors.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   138224 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/TaskBuffer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/TaskBufferInterface.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/Utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/WorkerSpec.py
--rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/WrappedCursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/WrappedPickle.py
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/WrappedPostgresConn.py
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/retryModule.py
--rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/taskbuffer/workflow_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.806153 panda-server-0.0.55/pandaserver/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/SchemaChecker.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.806153 panda-server-0.0.55/pandaserver/test/alice/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/banUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/boostPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/boostUser.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/callbackDDM.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/finishJob.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/finishTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/frontier_retagging.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/getJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1860 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/killJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/killJobLowPrio.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/killJobsInTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/killProdJobs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/killTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/killTaskJEDI.py
--rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/killUser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.806153 panda-server-0.0.55/pandaserver/test/lsst/
--rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/lsst/lsstSubmit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/lsst/lsstSubmitMERGEtest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/lsst/lsstSubmitPhosim332.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/reassignJobs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/reassignSite.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/reassignTask.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/reassignWaiting.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/recoverLostFiles.py
--rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/reloadInputDS.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/sendCommandToJob.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/setDebugMode.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/setPriority.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testEvgen.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testEvgen17.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testG4sim.py
--rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testG4sim17.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testGetCriteriaForGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testGlobalShares.py
--rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testJobFlowATLAS.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testReco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testSimulReco14.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testSiteMap.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testUpdateWorkerPilotStatus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/test/testutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.806153 panda-server-0.0.55/pandaserver/userinterface/
--rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/userinterface/Client.py
--rw-r--r--   0 runner    (1001) docker     (123)    89624 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/userinterface/UserIF.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/userinterface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.810153 panda-server-0.0.55/pandaserver/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/pcwl_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/pcwl_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/psnakemake_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.810153 panda-server-0.0.55/pandaserver/workflow/snakeparser/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/snakeparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/snakeparser/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/snakeparser/log.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/snakeparser/names.py
--rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/snakeparser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/snakeparser/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-05-24 13:38:42.000000 panda-server-0.0.55/pandaserver/workflow/workflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-24 13:38:53.810153 panda-server-0.0.55/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)    12531 2023-05-24 13:38:42.000000 panda-server-0.0.55/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.810153 panda-server-0.0.55/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/conda_meta.yaml.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.810153 panda-server-0.0.55/templates/init.d/
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/init.d/panda_daemon.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/init.d/panda_httpd.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/init.d/panda_server.exe.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.810153 panda-server-0.0.55/templates/logrotate.d/
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/logrotate.d/panda_server.logrotate.template
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/panda_server-httpd.conf.rpmnew.template
--rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/panda_server-makeSlsXml.exe.template
--rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/panda_server-vomsrenew.exe.template
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/panda_server.cfg.rpmnew.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.810153 panda-server-0.0.55/templates/sysconfig/
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/sysconfig/panda_server.sysconfig.rpmnew.template
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/sysconfig/panda_server_env.systemd.rpmnew.template
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 13:38:53.810153 panda-server-0.0.55/templates/systemd/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/systemd/panda.service.template
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/systemd/panda_daemon.service.template
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-24 13:38:42.000000 panda-server-0.0.55/templates/systemd/panda_httpd.service.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.467751 panda-server-0.0.56/
+-rw-r--r--   0 runner    (1001) docker     (123)    81051 2023-05-26 06:57:57.000000 panda-server-0.0.56/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-26 06:57:57.000000 panda-server-0.0.56/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 06:57:57.000000 panda-server-0.0.56/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 06:58:10.467751 panda-server-0.0.56/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-26 06:57:57.000000 panda-server-0.0.56/PandaPkgInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-26 06:57:57.000000 panda-server-0.0.56/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.443751 panda-server-0.0.56/panda_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-26 06:58:10.000000 panda-server-0.0.56/panda_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-05-26 06:58:10.000000 panda-server-0.0.56/panda_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:58:10.000000 panda-server-0.0.56/panda_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 06:58:10.000000 panda-server-0.0.56/panda_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-26 06:58:10.000000 panda-server-0.0.56/panda_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-26 06:58:10.000000 panda-server-0.0.56/panda_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.443751 panda-server-0.0.56/pandaserver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.443751 panda-server-0.0.56/pandaserver/brokerage/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/brokerage/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16197 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/brokerage/SiteMapper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/brokerage/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    80940 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/brokerage/broker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.443751 panda-server-0.0.56/pandaserver/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/config/config_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/config/daemon_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7167 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/config/panda_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.443751 panda-server-0.0.56/pandaserver/configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)     2448 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/configurator/Carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35264 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/configurator/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/configurator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/configurator/aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.443751 panda-server-0.0.56/pandaserver/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/master.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/master_systemd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.447751 panda-server-0.0.56/pandaserver/daemons/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7893 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/add_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12972 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/add_sub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/carbon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2726 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64166 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/copyArchive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54562 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/datasetManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/dummy_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5767 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/evpPD2P.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41977 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/metric_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/panda_activeusers_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/pilotStreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4919 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/process_workflow_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4701 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/recover_lost_files_daemon.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15682 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/task_evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/tmpwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/scripts/worker_synchronization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25399 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/daemons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.451751 panda-server-0.0.56/pandaserver/dataservice/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1604 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/Activator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53929 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/AdderAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/AdderDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40601 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/AdderGen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/AdderPluginBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/AdderResult.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5906 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/AdderSimplePlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    17541 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/Closer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1544 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/CloserAtlasPlugin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27051 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/DDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1988 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/DDMHandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2634 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/DataService.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/DataServiceUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57671 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/DynDataDistributer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      412 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/EventPicker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11067 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/Finisher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18450 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/Notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/ProcessLimiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/RecoverLostFilesCore.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8488 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/Setupper.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   113605 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/SetupperAtlasPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/SetupperDummyPlugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/SetupperPluginBase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/eventLookupClientEI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2101 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/dataservice/forkSetupper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.451751 panda-server-0.0.56/pandaserver/jobdispatcher/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/jobdispatcher/DispatcherUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      263 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/jobdispatcher/ErrorCode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58936 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/jobdispatcher/JobDispatcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16316 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/jobdispatcher/Protocol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8959 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/jobdispatcher/Watcher.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/jobdispatcher/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.451751 panda-server-0.0.56/pandaserver/proxycache/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2898 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/proxycache/DBMSql.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/proxycache/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1539 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/proxycache/panda_activeusers_query.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9479 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/proxycache/panda_proxy_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.451751 panda-server-0.0.56/pandaserver/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/server/.gacl
+-rwxr-xr-x   0 runner    (1001) docker     (123)    22444 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/server/panda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.451751 panda-server-0.0.56/pandaserver/srvcore/
+-rw-r--r--   0 runner    (1001) docker     (123)     5103 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/srvcore/CoreUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4037 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/srvcore/MailUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/srvcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/srvcore/oidc_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/srvcore/srv_msg_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.459751 panda-server-0.0.56/pandaserver/taskbuffer/
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/CloudSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/CloudTaskSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18890 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/ConBridge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2132 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/DBProxyPool.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3002 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/DatasetSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4028 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/DdmSpec.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4647 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/EiDBProxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/ErrorCode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10721 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/EventServiceUtils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7836 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/FileSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7014 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/GlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/HarvesterMetricsSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/Initializer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25903 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/JobSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/JobUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3913 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/NucleusSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1232654 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/OraDBProxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/PanDAMsgProcessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/PandaDBSchemaInfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/PrioUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/ProcessGroups.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/ResourceSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/SQLDumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6859 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/SiteSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/SupErrors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   138224 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/TaskBuffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/TaskBufferInterface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19209 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3906 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/WorkerSpec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17662 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/WrappedCursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3224 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/WrappedPickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/WrappedPostgresConn.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13789 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/retryModule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12573 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/taskbuffer/workflow_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.463751 panda-server-0.0.56/pandaserver/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/SchemaChecker.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.463751 panda-server-0.0.56/pandaserver/test/alice/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/alice/titan_testScript_ec2_alice_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/alice/titan_testScript_ec2_alice_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1010 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/banUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      623 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/boostPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1051 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/boostUser.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      789 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/callbackDDM.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10377 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/finishJob.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/finishTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6951 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/frontier_retagging.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1314 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/getJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1922 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/killJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2952 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/killJobLowPrio.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1625 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/killJobsInTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      555 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/killProdJobs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2417 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/killTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      239 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/killTaskJEDI.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2372 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/killUser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.463751 panda-server-0.0.56/pandaserver/test/lsst/
+-rw-r--r--   0 runner    (1001) docker     (123)     5693 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/lsst/lsstSubmit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/lsst/lsstSubmitMERGEtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/lsst/lsstSubmitPhosim332.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/reassignJobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/reassignSite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/reassignTask.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1023 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/reassignWaiting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/recoverLostFiles.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/reloadInputDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/sendCommandToJob.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      898 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/setDebugMode.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      806 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/setPriority.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1834 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testEvgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1808 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testEvgen17.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2574 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testG4sim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2704 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testG4sim17.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testGetCriteriaForGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testGlobalShares.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11962 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testJobFlowATLAS.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3739 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testReco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testSimulReco14.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      551 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testSiteMap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testUpdateWorkerPilotStatus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1334 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/test/testutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.463751 panda-server-0.0.56/pandaserver/userinterface/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81389 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/userinterface/Client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89624 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/userinterface/UserIF.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/userinterface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.463751 panda-server-0.0.56/pandaserver/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/pcwl_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14264 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/pcwl_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/psnakemake_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.467751 panda-server-0.0.56/pandaserver/workflow/snakeparser/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/snakeparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/snakeparser/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/snakeparser/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/snakeparser/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13754 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/snakeparser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/snakeparser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35878 2023-05-26 06:57:57.000000 panda-server-0.0.56/pandaserver/workflow/workflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-26 06:58:10.467751 panda-server-0.0.56/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12531 2023-05-26 06:57:57.000000 panda-server-0.0.56/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.467751 panda-server-0.0.56/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/conda_meta.yaml.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.467751 panda-server-0.0.56/templates/init.d/
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/init.d/panda_daemon.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/init.d/panda_httpd.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1547 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/init.d/panda_server.exe.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.467751 panda-server-0.0.56/templates/logrotate.d/
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/logrotate.d/panda_server.logrotate.template
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/panda_server-httpd-FastCGI.conf.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/panda_server-httpd.conf.rpmnew.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13906 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/panda_server-makeSlsXml.exe.template
+-rwxr-xr-x   0 runner    (1001) docker     (123)      745 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/panda_server-vomsrenew.exe.template
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/panda_server.cfg.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.467751 panda-server-0.0.56/templates/sysconfig/
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/sysconfig/panda_server.sysconfig.rpmnew.template
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/sysconfig/panda_server_env.systemd.rpmnew.template
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 06:58:10.467751 panda-server-0.0.56/templates/systemd/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/systemd/panda.service.template
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/systemd/panda_daemon.service.template
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-26 06:57:57.000000 panda-server-0.0.56/templates/systemd/panda_httpd.service.template
```

### Comparing `panda-server-0.0.55/ChangeLog.txt` & `panda-server-0.0.56/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/LICENSE.txt` & `panda-server-0.0.56/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/panda_server.egg-info/SOURCES.txt` & `panda-server-0.0.56/panda_server.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/brokerage/SiteMapper.py` & `panda-server-0.0.56/pandaserver/brokerage/SiteMapper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/brokerage/broker.py` & `panda-server-0.0.56/pandaserver/brokerage/broker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/config/daemon_config.py` & `panda-server-0.0.56/pandaserver/config/daemon_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/config/panda_config.py` & `panda-server-0.0.56/pandaserver/config/panda_config.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/configurator/Carbon.py` & `panda-server-0.0.56/pandaserver/configurator/Carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/configurator/Configurator.py` & `panda-server-0.0.56/pandaserver/configurator/Configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/configurator/aux.py` & `panda-server-0.0.56/pandaserver/configurator/aux.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/master.py` & `panda-server-0.0.56/pandaserver/daemons/master.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/master_systemd.py` & `panda-server-0.0.56/pandaserver/daemons/master_systemd.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/add_main.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/add_main.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/add_sub.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/add_sub.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/carbon.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/carbon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/configurator.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/configurator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/copyArchive.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/copyArchive.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/datasetManager.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/datasetManager.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/dummy_test.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/dummy_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/evpPD2P.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/evpPD2P.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/metric_collector.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/metric_collector.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/panda_activeusers_query.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/pilotStreaming.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/pilotStreaming.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/process_workflow_files_daemon.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/process_workflow_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/recover_lost_files_daemon.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/recover_lost_files_daemon.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/task_evaluator.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/task_evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -232,14 +232,20 @@
             varMap = {}
             active_tasks_list = self.tbuf.querySQL(sql_get_active_tasks, varMap)
             taskID_list = [ task[0] for task in active_tasks_list ]
             n_tot_tasks = len(active_tasks_list)
             tmp_log.debug('got total {0} tasks'.format(n_tot_tasks))
             # counter
             cc = 0
+            n_tasks_dict = {
+                    2: 0,
+                    1: 0,
+                    0: 0,
+                    -1: 0,
+                }
             # loop over tasks
             for taskID, user, gshare in active_tasks_list:
                 # initialize
                 task_class = 1
                 n_files_total = 0
                 n_files_finished = 0
                 n_files_failed = 0
@@ -256,37 +262,41 @@
                     n_files_total = ds_info.get('nFiles', 0)
                     n_files_finished = ds_info.get('nFilesFinished', 0)
                     n_files_failed = ds_info.get('nFilesFailed', 0)
                     if n_files_total > 0:
                         pct_finished = n_files_finished*100/n_files_total
                         pct_failed = n_files_failed*100/n_files_total
                 # classify
-                # parameters
-                progress_to_boost_A = self.tbuf.getConfigValue('analy_eval', 'PROGRESS_TO_BOOST_A')
-                if progress_to_boost_A is None:
-                    progress_to_boost_A = 90
-                progress_to_boost_B = self.tbuf.getConfigValue('analy_eval', 'PROGRESS_TO_BOOST_B')
-                if progress_to_boost_B is None:
-                    progress_to_boost_B = 95
-                # check usage of the user
-                usage_dict = ue_dict.get(user)
-                if usage_dict is None:
-                    continue
-                if usage_dict['rem_slots_A'] <= 0:
-                    if usage_dict['rem_slots_B'] <= 0:
-                        task_class = -1
-                    else:
-                        task_class = 0
-                # boost for nearly done tasks
-                if task_class == 1 and pct_finished >= progress_to_boost_A:
-                    # almost done A-tasks, to boost
-                    task_class = 2
-                elif task_class == 0 and pct_finished >= progress_to_boost_B:
-                    # almost done B-tasks, to boost
+                if gshare == 'Express Analysis':
+                    # Express Analysis tasks always in class S
                     task_class = 2
+                else:
+                    # parameters
+                    progress_to_boost_A = self.tbuf.getConfigValue('analy_eval', 'PROGRESS_TO_BOOST_A')
+                    if progress_to_boost_A is None:
+                        progress_to_boost_A = 90
+                    progress_to_boost_B = self.tbuf.getConfigValue('analy_eval', 'PROGRESS_TO_BOOST_B')
+                    if progress_to_boost_B is None:
+                        progress_to_boost_B = 95
+                    # check usage of the user
+                    usage_dict = ue_dict.get(user)
+                    if usage_dict is None:
+                        continue
+                    if usage_dict['rem_slots_A'] <= 0:
+                        if usage_dict['rem_slots_B'] <= 0:
+                            task_class = -1
+                        else:
+                            task_class = 0
+                    # boost for nearly done tasks
+                    if task_class == 1 and pct_finished >= progress_to_boost_A:
+                        # almost done A-tasks, to boost
+                        task_class = 2
+                    elif task_class == 0 and pct_finished >= progress_to_boost_B:
+                        # almost done B-tasks, to boost
+                        task_class = 2
                 # fill in task class
                 task_dict[taskID] = {
                         'task_id': taskID,
                         'user': user,
                         'gshare': gshare,
                         'n_files_total': n_files_total,
                         'n_files_finished': n_files_finished,
@@ -294,16 +304,18 @@
                         'pct_finished': pct_finished,
                         'pct_failed': pct_failed,
                         'class': task_class,
                     }
                 # counter
                 cc += 1
                 if cc % 5000 == 0:
-                    tmp_log.debug('evaluated {0:9d} tasks'.format(cc))
-            tmp_log.debug('evaluated {0:9d} tasks in total'.format(cc))
+                    tmp_log.debug('evaluated {0:6d} tasks'.format(cc))
+                n_tasks_dict[task_class] += 1
+            tmp_log.debug('evaluated {tot:6d} tasks in total (S:{nS}, A:{nA}, B:{nB}, C:{nC})'.format(
+                            tot=cc, nS=n_tasks_dict[2], nA=n_tasks_dict[1], nB=n_tasks_dict[0], nC=n_tasks_dict[-1]))
             # return
             # tmp_log.debug('{}'.format(str([ v for v in task_dict.values() if v['class'] != 1 ])[:3000]))
             tmp_log.debug('done')
             return task_dict
         except Exception:
             tmp_log.error(traceback.format_exc())
```

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/tmpwatch.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/tmpwatch.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/scripts/worker_synchronization.py` & `panda-server-0.0.56/pandaserver/daemons/scripts/worker_synchronization.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/daemons/utils.py` & `panda-server-0.0.56/pandaserver/daemons/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/Activator.py` & `panda-server-0.0.56/pandaserver/dataservice/Activator.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/AdderAtlasPlugin.py` & `panda-server-0.0.56/pandaserver/dataservice/AdderAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/AdderGen.py` & `panda-server-0.0.56/pandaserver/dataservice/AdderGen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/AdderResult.py` & `panda-server-0.0.56/pandaserver/dataservice/AdderResult.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/AdderSimplePlugin.py` & `panda-server-0.0.56/pandaserver/dataservice/AdderSimplePlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/Closer.py` & `panda-server-0.0.56/pandaserver/dataservice/Closer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/CloserAtlasPlugin.py` & `panda-server-0.0.56/pandaserver/dataservice/CloserAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/DDM.py` & `panda-server-0.0.56/pandaserver/dataservice/DDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/DDMHandler.py` & `panda-server-0.0.56/pandaserver/dataservice/DDMHandler.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/DataService.py` & `panda-server-0.0.56/pandaserver/dataservice/DataService.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/DataServiceUtils.py` & `panda-server-0.0.56/pandaserver/dataservice/DataServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/DynDataDistributer.py` & `panda-server-0.0.56/pandaserver/dataservice/DynDataDistributer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/EventPicker.py` & `panda-server-0.0.56/pandaserver/dataservice/EventPicker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/Finisher.py` & `panda-server-0.0.56/pandaserver/dataservice/Finisher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/Notifier.py` & `panda-server-0.0.56/pandaserver/dataservice/Notifier.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/ProcessLimiter.py` & `panda-server-0.0.56/pandaserver/dataservice/ProcessLimiter.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/RecoverLostFilesCore.py` & `panda-server-0.0.56/pandaserver/dataservice/RecoverLostFilesCore.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/Setupper.py` & `panda-server-0.0.56/pandaserver/dataservice/Setupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/SetupperAtlasPlugin.py` & `panda-server-0.0.56/pandaserver/dataservice/SetupperAtlasPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/SetupperDummyPlugin.py` & `panda-server-0.0.56/pandaserver/dataservice/SetupperDummyPlugin.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/SetupperPluginBase.py` & `panda-server-0.0.56/pandaserver/dataservice/SetupperPluginBase.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/eventLookupClientEI.py` & `panda-server-0.0.56/pandaserver/dataservice/eventLookupClientEI.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/dataservice/forkSetupper.py` & `panda-server-0.0.56/pandaserver/dataservice/forkSetupper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/jobdispatcher/DispatcherUtils.py` & `panda-server-0.0.56/pandaserver/jobdispatcher/DispatcherUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/jobdispatcher/JobDispatcher.py` & `panda-server-0.0.56/pandaserver/jobdispatcher/JobDispatcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/jobdispatcher/Protocol.py` & `panda-server-0.0.56/pandaserver/jobdispatcher/Protocol.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/jobdispatcher/Watcher.py` & `panda-server-0.0.56/pandaserver/jobdispatcher/Watcher.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/proxycache/DBMSql.py` & `panda-server-0.0.56/pandaserver/proxycache/DBMSql.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/proxycache/panda_activeusers_query.py` & `panda-server-0.0.56/pandaserver/proxycache/panda_activeusers_query.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/proxycache/panda_proxy_cache.py` & `panda-server-0.0.56/pandaserver/proxycache/panda_proxy_cache.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/server/panda.py` & `panda-server-0.0.56/pandaserver/server/panda.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/srvcore/CoreUtils.py` & `panda-server-0.0.56/pandaserver/srvcore/CoreUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/srvcore/MailUtils.py` & `panda-server-0.0.56/pandaserver/srvcore/MailUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/srvcore/oidc_utils.py` & `panda-server-0.0.56/pandaserver/srvcore/oidc_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/srvcore/srv_msg_utils.py` & `panda-server-0.0.56/pandaserver/srvcore/srv_msg_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/CloudSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/CloudSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/CloudTaskSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/CloudTaskSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/ConBridge.py` & `panda-server-0.0.56/pandaserver/taskbuffer/ConBridge.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/DBProxyPool.py` & `panda-server-0.0.56/pandaserver/taskbuffer/DBProxyPool.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/DatasetSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/DatasetSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/DdmSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/DdmSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/EiDBProxy.py` & `panda-server-0.0.56/pandaserver/taskbuffer/EiDBProxy.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/ErrorCode.py` & `panda-server-0.0.56/pandaserver/taskbuffer/ErrorCode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/EventServiceUtils.py` & `panda-server-0.0.56/pandaserver/taskbuffer/EventServiceUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/FileSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/FileSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/GlobalShares.py` & `panda-server-0.0.56/pandaserver/taskbuffer/GlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/HarvesterMetricsSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/HarvesterMetricsSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/Initializer.py` & `panda-server-0.0.56/pandaserver/taskbuffer/Initializer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/JobSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/JobSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/JobUtils.py` & `panda-server-0.0.56/pandaserver/taskbuffer/JobUtils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/NucleusSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/NucleusSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/OraDBProxy.py` & `panda-server-0.0.56/pandaserver/taskbuffer/OraDBProxy.py`

 * *Files 0% similar despite different names*

```diff
@@ -4393,14 +4393,15 @@
         # 10 : fast rebrokerage in overloaded PQ
         # 50 : kill by JEDI
         # 51 : reassigned by JEDI
         # 52 : force kill by JEDI
         # 55 : killed since task is (almost) done
         # 60 : workload was terminated by the pilot without actual work
         # 91 : kill user jobs with prod role
+        # 99 : force kill user jobs with prod role
         comment = ' /* DBProxy.killJob */'
         methodName = comment.split(' ')[-2].split('.')[-1]
         methodName += ' <PandaID={0}>'.format(pandaID)
         tmpLog = LogWrapper(_logger,methodName)
         tmpLog.debug("code=%s role=%s user=%s wg=%s opts=%s" % (code,prodManager,user,wgProdRole,killOpts))
         timeStart = datetime.datetime.utcnow()
         # check PandaID
@@ -4476,15 +4477,15 @@
                         if tmpGroupProdRole == '':
                             continue
                         if re.search('(^|_)'+tmpGroupProdRole+'$',workingGroup,re.I) is not None:
                             validGroupProdRole = True
                             break
                 if prodManager:
                     if res[1] in ['user','panda'] and (code not in ['2','4','7','8','9','50','51','52','91',
-                                                                    '10']):
+                                                                    '10', '99']):
                         tmpLog.debug("ignored -> prod proxy tried to kill analysis job type=%s" % res[1])
                         break
                     tmpLog.debug("using prod role")
                 elif validGroupProdRole:
                     # WGs with prod role
                     tmpLog.debug("using group prod role for workingGroup=%s" % workingGroup)
                     pass
@@ -4500,15 +4501,15 @@
                     eventService in [EventServiceUtils.jumboJobFlagNumber, EventServiceUtils.coJumboJobFlagNumber]
                 useEventServiceMerge = EventServiceUtils.isEventServiceMergeSH(specialHandling)
                 # update
                 varMap = {}
                 varMap[':PandaID'] = pandaID
                 varMap[':commandToPilot'] = 'tobekilled'
                 varMap[':taskBufferErrorDiag'] = 'killed by %s' % user
-                if code in ['2', '9', '10', '52', '51', '60']:
+                if code in ['2', '9', '10', '52', '51', '60', '99']:
                     # ignore commandToPilot for force kill
                     self.cur.execute((sql1F+comment) % table, varMap)
                 elif useEventService or jobStatusInDB in ['merging']:
                     # use force kill for event service or merging
                     self.cur.execute((sql1F+comment) % table, varMap)
                 else:
                     self.cur.execute((sql1+comment) % table, varMap)
@@ -4516,15 +4517,16 @@
                 if retU == 0:
                     continue
                 # set flag
                 flagCommand = True
                 # select
                 varMap = {}
                 varMap[':PandaID'] = pandaID
-                if (userProdSourceLabel in ['managed','test',None] or 'test' in userProdSourceLabel) and code in ['9','52']:
+                if ((userProdSourceLabel in ['managed', 'test', None] or 'test' in userProdSourceLabel)
+                        and code in ['9', '52']) or (prodManager and code == '99'):
                     # use dummy for force kill
                     varMap[':jobStatus'] = 'dummy'
                 elif useEventService or jobStatusInDB in ['merging']:
                     # use dummy for force kill
                     varMap[':jobStatus'] = 'dummy'
                 else:
                     varMap[':jobStatus'] = 'running'
```

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/PrioUtil.py` & `panda-server-0.0.56/pandaserver/taskbuffer/PrioUtil.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/ProcessGroups.py` & `panda-server-0.0.56/pandaserver/taskbuffer/ProcessGroups.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/ResourceSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/ResourceSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/SQLDumper.py` & `panda-server-0.0.56/pandaserver/taskbuffer/SQLDumper.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/SiteSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/SiteSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/TaskBuffer.py` & `panda-server-0.0.56/pandaserver/taskbuffer/TaskBuffer.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/TaskBufferInterface.py` & `panda-server-0.0.56/pandaserver/taskbuffer/TaskBufferInterface.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/Utils.py` & `panda-server-0.0.56/pandaserver/taskbuffer/Utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/WorkerSpec.py` & `panda-server-0.0.56/pandaserver/taskbuffer/WorkerSpec.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/WrappedCursor.py` & `panda-server-0.0.56/pandaserver/taskbuffer/WrappedCursor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/WrappedPickle.py` & `panda-server-0.0.56/pandaserver/taskbuffer/WrappedPickle.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/retryModule.py` & `panda-server-0.0.56/pandaserver/taskbuffer/retryModule.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/taskbuffer/workflow_processor.py` & `panda-server-0.0.56/pandaserver/taskbuffer/workflow_processor.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/SchemaChecker.py` & `panda-server-0.0.56/pandaserver/test/SchemaChecker.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/alice/titan_testScript_ec2_alice_1.py` & `panda-server-0.0.56/pandaserver/test/alice/titan_testScript_ec2_alice_1.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/alice/titan_testScript_ec2_alice_2.py` & `panda-server-0.0.56/pandaserver/test/alice/titan_testScript_ec2_alice_2.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/banUser.py` & `panda-server-0.0.56/pandaserver/test/banUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/boostPrio.py` & `panda-server-0.0.56/pandaserver/test/boostPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/boostUser.py` & `panda-server-0.0.56/pandaserver/test/boostUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/callbackDDM.py` & `panda-server-0.0.56/pandaserver/test/callbackDDM.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/finishJob.py` & `panda-server-0.0.56/pandaserver/test/finishJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/frontier_retagging.py` & `panda-server-0.0.56/pandaserver/test/frontier_retagging.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/getJobs.py` & `panda-server-0.0.56/pandaserver/test/getJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/killJob.py` & `panda-server-0.0.56/pandaserver/test/killJob.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,15 +20,18 @@
 
 aSrvID = None
 
 codeV = None
 useMailAsIDV = False
 
 if options.forceKill:
-    codeV = 9
+    if options.killUserJobs:
+        codeV = 99
+    else:
+        codeV = 9
 elif options.killUserJobs:
     codeV = 91
 else:
     try:
         codeV = int(options.codeV)
     except Exception:
         pass
```

### Comparing `panda-server-0.0.55/pandaserver/test/killJobLowPrio.py` & `panda-server-0.0.56/pandaserver/test/killJobLowPrio.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/killJobsInTask.py` & `panda-server-0.0.56/pandaserver/test/killJobsInTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/killProdJobs.py` & `panda-server-0.0.56/pandaserver/test/killProdJobs.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/killTask.py` & `panda-server-0.0.56/pandaserver/test/killTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/killUser.py` & `panda-server-0.0.56/pandaserver/test/killUser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/lsst/lsstSubmit.py` & `panda-server-0.0.56/pandaserver/test/lsst/lsstSubmit.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/lsst/lsstSubmitMERGEtest.py` & `panda-server-0.0.56/pandaserver/test/lsst/lsstSubmitMERGEtest.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/lsst/lsstSubmitPhosim332.py` & `panda-server-0.0.56/pandaserver/test/lsst/lsstSubmitPhosim332.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/reassignSite.py` & `panda-server-0.0.56/pandaserver/test/reassignSite.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/reassignTask.py` & `panda-server-0.0.56/pandaserver/test/reassignTask.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/reassignWaiting.py` & `panda-server-0.0.56/pandaserver/test/reassignWaiting.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/reloadInputDS.py` & `panda-server-0.0.56/pandaserver/test/reloadInputDS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/sendCommandToJob.py` & `panda-server-0.0.56/pandaserver/test/sendCommandToJob.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/setDebugMode.py` & `panda-server-0.0.56/pandaserver/test/setDebugMode.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/setPriority.py` & `panda-server-0.0.56/pandaserver/test/setPriority.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testEvgen.py` & `panda-server-0.0.56/pandaserver/test/testEvgen.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testEvgen17.py` & `panda-server-0.0.56/pandaserver/test/testEvgen17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testG4sim.py` & `panda-server-0.0.56/pandaserver/test/testG4sim.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testG4sim17.py` & `panda-server-0.0.56/pandaserver/test/testG4sim17.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testGetCriteriaForGlobalShares.py` & `panda-server-0.0.56/pandaserver/test/testGetCriteriaForGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testGlobalShares.py` & `panda-server-0.0.56/pandaserver/test/testGlobalShares.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testJobFlowATLAS.py` & `panda-server-0.0.56/pandaserver/test/testJobFlowATLAS.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testReco.py` & `panda-server-0.0.56/pandaserver/test/testReco.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testSimulReco14.py` & `panda-server-0.0.56/pandaserver/test/testSimulReco14.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testSiteMap.py` & `panda-server-0.0.56/pandaserver/test/testSiteMap.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/test/testutils.py` & `panda-server-0.0.56/pandaserver/test/testutils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/userinterface/Client.py` & `panda-server-0.0.56/pandaserver/userinterface/Client.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/userinterface/UserIF.py` & `panda-server-0.0.56/pandaserver/userinterface/UserIF.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/workflow/pcwl_test.py` & `panda-server-0.0.56/pandaserver/workflow/pcwl_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/workflow/pcwl_utils.py` & `panda-server-0.0.56/pandaserver/workflow/pcwl_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/workflow/psnakemake_test.py` & `panda-server-0.0.56/pandaserver/workflow/psnakemake_test.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/workflow/snakeparser/extensions.py` & `panda-server-0.0.56/pandaserver/workflow/snakeparser/extensions.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/workflow/snakeparser/log.py` & `panda-server-0.0.56/pandaserver/workflow/snakeparser/log.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/workflow/snakeparser/parser.py` & `panda-server-0.0.56/pandaserver/workflow/snakeparser/parser.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/workflow/snakeparser/utils.py` & `panda-server-0.0.56/pandaserver/workflow/snakeparser/utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/pandaserver/workflow/workflow_utils.py` & `panda-server-0.0.56/pandaserver/workflow/workflow_utils.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/setup.py` & `panda-server-0.0.56/setup.py`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/conda_meta.yaml.template` & `panda-server-0.0.56/templates/conda_meta.yaml.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/init.d/panda_daemon.exe.template` & `panda-server-0.0.56/templates/init.d/panda_daemon.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/init.d/panda_httpd.exe.template` & `panda-server-0.0.56/templates/init.d/panda_httpd.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/init.d/panda_server.exe.template` & `panda-server-0.0.56/templates/init.d/panda_server.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/logrotate.d/panda_server.logrotate.template` & `panda-server-0.0.56/templates/logrotate.d/panda_server.logrotate.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/panda_server-httpd-FastCGI.conf.rpmnew.template` & `panda-server-0.0.56/templates/panda_server-httpd-FastCGI.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/panda_server-httpd.conf.rpmnew.template` & `panda-server-0.0.56/templates/panda_server-httpd.conf.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/panda_server-makeSlsXml.exe.template` & `panda-server-0.0.56/templates/panda_server-makeSlsXml.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/panda_server-vomsrenew.exe.template` & `panda-server-0.0.56/templates/panda_server-vomsrenew.exe.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/panda_server.cfg.rpmnew.template` & `panda-server-0.0.56/templates/panda_server.cfg.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/sysconfig/panda_server.sysconfig.rpmnew.template` & `panda-server-0.0.56/templates/sysconfig/panda_server.sysconfig.rpmnew.template`

 * *Files identical despite different names*

### Comparing `panda-server-0.0.55/templates/sysconfig/panda_server_env.systemd.rpmnew.template` & `panda-server-0.0.56/templates/sysconfig/panda_server_env.systemd.rpmnew.template`

 * *Files identical despite different names*

