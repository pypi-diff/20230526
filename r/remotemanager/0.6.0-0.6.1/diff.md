# Comparing `tmp/remotemanager-0.6.0.tar.gz` & `tmp/remotemanager-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remotemanager-0.6.0.tar", last modified: Thu May 25 10:21:17 2023, max compression
+gzip compressed data, was "remotemanager-0.6.1.tar", last modified: Fri May 26 07:15:24 2023, max compression
```

## Comparing `remotemanager-0.6.0.tar` & `remotemanager-0.6.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.631509 remotemanager-0.6.0/
--rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-18 14:24:27.000000 remotemanager-0.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1278 2023-05-25 10:21:17.631509 remotemanager-0.6.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 12:43:02.000000 remotemanager-0.6.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)     1351 2023-05-24 13:40:04.000000 remotemanager-0.6.0/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.623509 remotemanager-0.6.0/remotemanager/
--rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-24 13:40:04.000000 remotemanager-0.6.0/remotemanager/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.627509 remotemanager-0.6.0/remotemanager/connection/
--rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/connection/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14968 2023-05-24 13:40:04.000000 remotemanager-0.6.0/remotemanager/connection/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.627509 remotemanager-0.6.0/remotemanager/connection/computers/
--rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/connection/computers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    12341 2023-05-24 13:40:04.000000 remotemanager-0.6.0/remotemanager/connection/computers/base.py
--rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:40:04.000000 remotemanager-0.6.0/remotemanager/connection/computers/example.py
--rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:40:04.000000 remotemanager-0.6.0/remotemanager/connection/computers/options.py
--rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:32:25.000000 remotemanager-0.6.0/remotemanager/connection/computers/parsers.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:04.000000 remotemanager-0.6.0/remotemanager/connection/detect_locale_error.py
--rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/connection/testing_object.py
--rw-rw-rw-   0 root         (0) root         (0)    23588 2023-05-24 14:43:56.000000 remotemanager-0.6.0/remotemanager/connection/url.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.627509 remotemanager-0.6.0/remotemanager/dataset/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/dataset/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    48903 2023-05-25 09:38:01.000000 remotemanager-0.6.0/remotemanager/dataset/dataset.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/dataset/dependency.py
--rw-rw-rw-   0 root         (0) root         (0)    22556 2023-05-25 09:38:01.000000 remotemanager-0.6.0/remotemanager/dataset/runner.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.627509 remotemanager-0.6.0/remotemanager/jupyter/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 14:24:27.000000 remotemanager-0.6.0/remotemanager/jupyter/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-24 14:43:56.000000 remotemanager-0.6.0/remotemanager/jupyter/magic.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.627509 remotemanager-0.6.0/remotemanager/logging/
--rw-rw-rw-   0 root         (0) root         (0)     4043 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/logging/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6496 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/logging/log.py
--rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-18 14:24:27.000000 remotemanager-0.6.0/remotemanager/logging/quiet.py
--rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/logging/utils.py
--rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/logging/verbosity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.631509 remotemanager-0.6.0/remotemanager/serialisation/
--rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/serialisation/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/serialisation/serial.py
--rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-18 14:24:27.000000 remotemanager-0.6.0/remotemanager/serialisation/serialdill.py
--rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-18 14:24:27.000000 remotemanager-0.6.0/remotemanager/serialisation/serialjson.py
--rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/serialisation/serialjsonpickle.py
--rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/serialisation/serialyaml.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.631509 remotemanager-0.6.0/remotemanager/storage/
--rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/storage/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/storage/database.py
--rw-rw-rw-   0 root         (0) root         (0)     4901 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/storage/function.py
--rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/storage/remotefunction.py
--rw-rw-rw-   0 root         (0) root         (0)    11768 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/storage/sendablemixin.py
--rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/storage/trackedfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.631509 remotemanager-0.6.0/remotemanager/transport/
--rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/transport/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/transport/cp.py
--rw-rw-rw-   0 root         (0) root         (0)     2251 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/transport/rsync.py
--rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/transport/scp.py
--rw-rw-rw-   0 root         (0) root         (0)     9230 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/transport/transport.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.631509 remotemanager-0.6.0/remotemanager/utils/
--rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/utils/flags.py
--rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 10:04:17.000000 remotemanager-0.6.0/remotemanager/utils/uuid.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 09:35:30.000000 remotemanager-0.6.0/remotemanager/utils/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-25 10:21:17.623509 remotemanager-0.6.0/remotemanager.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1278 2023-05-25 10:21:17.000000 remotemanager-0.6.0/remotemanager.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1788 2023-05-25 10:21:17.000000 remotemanager-0.6.0/remotemanager.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-25 10:21:17.000000 remotemanager-0.6.0/remotemanager.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      154 2023-05-25 10:21:17.000000 remotemanager-0.6.0/remotemanager.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-05-25 10:21:17.000000 remotemanager-0.6.0/remotemanager.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-25 10:21:17.631509 remotemanager-0.6.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-18 14:24:27.000000 remotemanager-0.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1067 2023-04-20 09:36:43.000000 remotemanager-0.6.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-05-26 07:15:24.321536 remotemanager-0.6.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      864 2023-05-15 13:29:14.000000 remotemanager-0.6.1/README.md
+-rw-rw-rw-   0 root         (0) root         (0)     1367 2023-05-26 07:15:10.000000 remotemanager-0.6.1/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/
+-rw-rw-rw-   0 root         (0) root         (0)      481 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/connection/
+-rw-rw-rw-   0 root         (0) root         (0)       64 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/connection/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    15152 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/connection/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/connection/computers/
+-rw-rw-rw-   0 root         (0) root         (0)      137 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/connection/computers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    12341 2023-05-24 13:40:42.000000 remotemanager-0.6.1/remotemanager/connection/computers/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     1613 2023-05-24 13:40:42.000000 remotemanager-0.6.1/remotemanager/connection/computers/example.py
+-rw-rw-rw-   0 root         (0) root         (0)     2970 2023-05-24 13:40:42.000000 remotemanager-0.6.1/remotemanager/connection/computers/options.py
+-rw-rw-rw-   0 root         (0) root         (0)     1503 2023-05-25 07:31:16.000000 remotemanager-0.6.1/remotemanager/connection/computers/parsers.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2023-05-24 13:40:42.000000 remotemanager-0.6.1/remotemanager/connection/detect_locale_error.py
+-rw-rw-rw-   0 root         (0) root         (0)     6672 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/connection/testing_object.py
+-rw-rw-rw-   0 root         (0) root         (0)    24726 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/connection/url.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/dataset/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/dataset/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    48903 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/dataset/dataset.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/dataset/dependency.py
+-rw-rw-rw-   0 root         (0) root         (0)    22556 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/dataset/runner.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/jupyter/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-20 09:36:43.000000 remotemanager-0.6.1/remotemanager/jupyter/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4873 2023-05-22 10:40:03.000000 remotemanager-0.6.1/remotemanager/jupyter/magic.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager/logging/
+-rw-rw-rw-   0 root         (0) root         (0)     4043 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/logging/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6496 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/logging/log.py
+-rw-rw-rw-   0 root         (0) root         (0)      266 2023-04-20 09:36:43.000000 remotemanager-0.6.1/remotemanager/logging/quiet.py
+-rw-rw-rw-   0 root         (0) root         (0)     1943 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/logging/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     2262 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/logging/verbosity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/remotemanager/serialisation/
+-rw-rw-rw-   0 root         (0) root         (0)      497 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/serialisation/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4038 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/serialisation/serial.py
+-rw-rw-rw-   0 root         (0) root         (0)      402 2023-04-20 09:36:43.000000 remotemanager-0.6.1/remotemanager/serialisation/serialdill.py
+-rw-rw-rw-   0 root         (0) root         (0)      427 2023-04-20 09:36:43.000000 remotemanager-0.6.1/remotemanager/serialisation/serialjson.py
+-rw-rw-rw-   0 root         (0) root         (0)     1609 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/serialisation/serialjsonpickle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1000 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/serialisation/serialyaml.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/remotemanager/storage/
+-rw-rw-rw-   0 root         (0) root         (0)      164 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5351 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/database.py
+-rw-rw-rw-   0 root         (0) root         (0)     4901 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/function.py
+-rw-rw-rw-   0 root         (0) root         (0)     1053 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/remotefunction.py
+-rw-rw-rw-   0 root         (0) root         (0)    12263 2023-05-25 13:31:29.000000 remotemanager-0.6.1/remotemanager/storage/sendablemixin.py
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/storage/trackedfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/remotemanager/transport/
+-rw-rw-rw-   0 root         (0) root         (0)      181 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      541 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/cp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2251 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/rsync.py
+-rw-rw-rw-   0 root         (0) root         (0)     3202 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/scp.py
+-rw-rw-rw-   0 root         (0) root         (0)     9230 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/transport/transport.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.321536 remotemanager-0.6.1/remotemanager/utils/
+-rw-rw-rw-   0 root         (0) root         (0)     3860 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4505 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/utils/flags.py
+-rw-rw-rw-   0 root         (0) root         (0)      149 2023-04-21 12:27:38.000000 remotemanager-0.6.1/remotemanager/utils/uuid.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-04-27 10:20:11.000000 remotemanager-0.6.1/remotemanager/utils/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-26 07:15:24.317536 remotemanager-0.6.1/remotemanager.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1278 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1788 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      163 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-05-26 07:15:24.000000 remotemanager-0.6.1/remotemanager.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-26 07:15:24.321536 remotemanager-0.6.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-04-20 09:36:43.000000 remotemanager-0.6.1/setup.py
```

### Comparing `remotemanager-0.6.0/LICENSE` & `remotemanager-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/PKG-INFO` & `remotemanager-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.0
+Version: 0.6.1
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.0/README.md` & `remotemanager-0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/pyproject.toml` & `remotemanager-0.6.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 classifiers = [
     "Programming Language :: Python :: 3.9",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     'pyyaml',
     'numpy',
+    'requests',
 ]
 dynamic = ['version']
 
 [project.optional-dependencies]
 dill = ["dill"]
 jsonpickle = ["jsonpickle"]
 all = ["dill", "jsonpickle"]
@@ -41,15 +42,15 @@
 [tool.pytest.ini_options]
 addopts = "--nbval --cov=remotemanager --cov-report term-missing --cov-append --nbval-sanitize-with ./tests/uuid_sanitise.cfg"
 
 [tool.coverage.report]
 omit = ["remotemanager/connection/computers/*"]
 
 [tool.bumpver]
-current_version = "0.6.0"
+current_version = "0.6.1"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "[clean] bump version {old_version} -> {new_version}"
 commit = true
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `remotemanager-0.6.0/remotemanager/connection/cmd.py` & `remotemanager-0.6.1/remotemanager/connection/cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 import subprocess
 import getpass
 import time
 import warnings
 
 from remotemanager.connection.detect_locale_error import detect_locale_error
-from remotemanager.storage.sendablemixin import SendableMixin
+from remotemanager.storage.sendablemixin import SendableMixin, Unloaded
 from remotemanager.logging import LoggingMixin
 
 
 def _process_redirect_file(file) -> [str, None]:
     if file is not None:
         return os.path.abspath(file)
     return None
@@ -126,14 +126,18 @@
     def is_redirected(self) -> bool:
         """
         True if the cmd is redirected to a file
         """
         return any([self._redirect["stdout"], self._redirect["stderr"]])
 
     def _get_return_attr(self, attr: str) -> [str, None]:
+        if isinstance(self._subprocess, Unloaded):
+            self._logger.warning(f"broken subprocess, getting attr _{attr}")
+            return getattr(self, f"_{attr}")
+
         poll = self._subprocess.poll()
         self._logger.info(f"cmd poll returned {poll}")
         if poll is None or poll < 0:
             self._logger.info("Falling back to communicate()")
             return self.communicate()[attr]
 
         self._logger.info(f"attempting to access the subprocess {attr} attr")
```

### Comparing `remotemanager-0.6.0/remotemanager/connection/computers/base.py` & `remotemanager-0.6.1/remotemanager/connection/computers/base.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/connection/computers/example.py` & `remotemanager-0.6.1/remotemanager/connection/computers/example.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/connection/computers/options.py` & `remotemanager-0.6.1/remotemanager/connection/computers/options.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/connection/computers/parsers.py` & `remotemanager-0.6.1/remotemanager/connection/computers/parsers.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/connection/testing_object.py` & `remotemanager-0.6.1/remotemanager/connection/testing_object.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/connection/url.py` & `remotemanager-0.6.1/remotemanager/connection/url.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 URL base class for connecting to remote systems
 """
 import logging
 import os
 import time
 import typing
+from collections import deque
 
 from remotemanager.connection.testing_object import ConnectionTest
 from remotemanager.logging.utils import format_iterable
 from remotemanager.connection.cmd import CMD
 from remotemanager.storage.sendablemixin import SendableMixin
 from remotemanager.utils import ensure_list
 from remotemanager.logging import LoggingMixin
@@ -40,14 +41,16 @@
         raise_errors (bool):
             set false to ignore errors by default in cmd calls
         passfile (str):
             absolute path to password file for sshpass calls
         envpass (str):
             environment variable containing absolute path to password file for
             sshpass calls
+        cmd_history_depth (int):
+            number of cmd calls to store history for
         kwargs:
             any extra args that may end up here from a Dataset or Computer are
             discarded
     """
 
     _localhost = "localhost"
 
@@ -66,14 +69,15 @@
         python: str = None,
         submitter: str = None,
         shell: str = None,
         raise_errors: bool = True,
         keyfile: str = None,
         passfile: str = None,
         envpass: str = None,
+        cmd_history_depth: int = 10,
         **kwargs,
     ):
 
         self._verbose = Verbosity(verbose)
 
         if host is None:
             host = URL._localhost
@@ -81,14 +85,17 @@
 
         self.timeout = timeout
         self.max_timeouts = max_timeouts
         self._python = python
         self._submitter = submitter
         self._shell = shell
 
+        self._cmd_history_depth = cmd_history_depth
+        self._cmd_history = deque(maxlen=self._cmd_history_depth)
+
         # explicit path takes precedent over environment variable
         if passfile is None and envpass is not None:
             passfile = os.environ[envpass]
 
         if "ignore_errors" in kwargs:
             raise_errors = not kwargs.pop("ignore_errors")
 
@@ -447,17 +454,52 @@
             timeout=timeout,
             max_timeouts=max_timeouts,
             raise_errors=raise_errors,
         )
         thiscmd.exec()
         if not local:
             self._callcount += 1
+
+        self._cmd_history.append(thiscmd)
+
         return thiscmd
 
     @property
+    def cmd_history(self):
+        return self._cmd_history
+
+    @property
+    def cmd_history_depth(self):
+        return self._cmd_history_depth
+
+    @cmd_history_depth.setter
+    def cmd_history_depth(self, newdepth: int):
+        """
+        Updates the history depth, and creates a new dequeue populated with as many of
+        the existing cmds as possible
+
+        Args:
+            newdepth (int):
+                new depth to capture
+        Returns:
+
+        """
+        self._logger.info(
+            f"updating history depth from {self.cmd_history_depth} " f"to {newdepth}"
+        )
+        self._cmd_history_depth = newdepth
+
+        newqueue = deque(maxlen=self.cmd_history_depth)
+
+        for item in self.cmd_history:
+            newqueue.append(item)
+
+        self._cmd_history = newqueue
+
+    @property
     def utils(self):
         """
         Handle for the URLUtils module
         """
         if self.is_missing("_urlutils"):
             self._urlutils = URLUtils(self)
         return self._urlutils
```

### Comparing `remotemanager-0.6.0/remotemanager/dataset/dataset.py` & `remotemanager-0.6.1/remotemanager/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/dataset/dependency.py` & `remotemanager-0.6.1/remotemanager/dataset/dependency.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/dataset/runner.py` & `remotemanager-0.6.1/remotemanager/dataset/runner.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/jupyter/magic.py` & `remotemanager-0.6.1/remotemanager/jupyter/magic.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/logging/__init__.py` & `remotemanager-0.6.1/remotemanager/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/logging/log.py` & `remotemanager-0.6.1/remotemanager/logging/log.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/logging/utils.py` & `remotemanager-0.6.1/remotemanager/logging/utils.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/logging/verbosity.py` & `remotemanager-0.6.1/remotemanager/logging/verbosity.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/serialisation/serial.py` & `remotemanager-0.6.1/remotemanager/serialisation/serial.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/serialisation/serialjsonpickle.py` & `remotemanager-0.6.1/remotemanager/serialisation/serialjsonpickle.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/serialisation/serialyaml.py` & `remotemanager-0.6.1/remotemanager/serialisation/serialyaml.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/storage/database.py` & `remotemanager-0.6.1/remotemanager/storage/database.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/storage/function.py` & `remotemanager-0.6.1/remotemanager/storage/function.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/storage/remotefunction.py` & `remotemanager-0.6.1/remotemanager/storage/remotefunction.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/storage/sendablemixin.py` & `remotemanager-0.6.1/remotemanager/storage/sendablemixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import collections.abc
 import importlib
 import logging
 import os.path
+from collections import deque
 
 import yaml
 
 CLASS_STORAGE_KEY = "~serialisedclass~"
 TUPLE_STORAGE_KEY = "~serialisedtuple~"
 SET_STORAGE_KEY = "~serialisedset~"
+DEQUE_STORAGE_KEY = "~serialiseddeque"
 SERIALISED_STORAGE_KEY = "~serialisedobject~"
 
 _logger = logging.getLogger(__name__)
 
 
 class SendableMixin:
     """
@@ -252,14 +254,18 @@
             # tuple-type
             return [TUPLE_STORAGE_KEY] + [self.serialise(v) for v in obj]
 
         elif isinstance(obj, set):
             # set-type
             return [SET_STORAGE_KEY] + [self.serialise(v) for v in obj]
 
+        elif isinstance(obj, deque):
+            # collections deque
+            return [DEQUE_STORAGE_KEY, obj.maxlen] + [self.serialise(v) for v in obj]
+
         if basic_available(obj):
             return obj
 
         try:
             return [SERIALISED_STORAGE_KEY, self.serialiser.dumps(obj)]
         except AttributeError:
             pass
@@ -315,17 +321,21 @@
             # dict type
             return {self.unserialise(k): self.unserialise(v) for k, v in obj.items()}
 
         # coming from the yaml file, output should _only_ be list
         elif isinstance(obj, list):
             try:
                 if obj[0] == TUPLE_STORAGE_KEY:
-                    return tuple(obj[1:])
+                    return tuple([self.unserialise(o) for o in obj[1:]])
                 elif obj[0] == SET_STORAGE_KEY:
-                    return set(obj[1:])
+                    return set([self.unserialise(o) for o in obj[1:]])
+                elif obj[0] == DEQUE_STORAGE_KEY:
+                    maxlen = obj[1]
+                    dqobj = obj[2:]
+                    return deque([self.unserialise(o) for o in dqobj], maxlen=maxlen)
             except IndexError:
                 return [self.unserialise(v) for v in obj]
 
         if basic_available(obj):
             return obj
 
         return obj
```

### Comparing `remotemanager-0.6.0/remotemanager/storage/trackedfile.py` & `remotemanager-0.6.1/remotemanager/storage/trackedfile.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/transport/cp.py` & `remotemanager-0.6.1/remotemanager/transport/cp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/transport/rsync.py` & `remotemanager-0.6.1/remotemanager/transport/rsync.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/transport/scp.py` & `remotemanager-0.6.1/remotemanager/transport/scp.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/transport/transport.py` & `remotemanager-0.6.1/remotemanager/transport/transport.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/utils/__init__.py` & `remotemanager-0.6.1/remotemanager/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/utils/flags.py` & `remotemanager-0.6.1/remotemanager/utils/flags.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager/utils/version.py` & `remotemanager-0.6.1/remotemanager/utils/version.py`

 * *Files identical despite different names*

### Comparing `remotemanager-0.6.0/remotemanager.egg-info/PKG-INFO` & `remotemanager-0.6.1/remotemanager.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: remotemanager
-Version: 0.6.0
+Version: 0.6.1
 Summary: remote run management tool
 Author-email: Louis Beal <louis.j.beal@gmail.com>
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dill
```

### Comparing `remotemanager-0.6.0/remotemanager.egg-info/SOURCES.txt` & `remotemanager-0.6.1/remotemanager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

