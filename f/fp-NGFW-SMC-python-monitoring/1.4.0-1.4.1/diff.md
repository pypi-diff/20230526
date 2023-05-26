# Comparing `tmp/fp-NGFW-SMC-python-monitoring-1.4.0.tar.gz` & `tmp/fp-NGFW-SMC-python-monitoring-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fp-NGFW-SMC-python-monitoring-1.4.0.tar", last modified: Thu Jun 10 15:38:50 2021, max compression
+gzip compressed data, was "fp-NGFW-SMC-python-monitoring-1.4.1.tar", last modified: Fri May 26 09:34:53 2023, max compression
```

## Comparing `fp-NGFW-SMC-python-monitoring-1.4.0.tar` & `fp-NGFW-SMC-python-monitoring-1.4.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7334 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-monitoring-1.4.0/README.rst
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1064 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-monitoring-1.4.0/HISTORY.rst
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       18 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-monitoring-1.4.0/version.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/fp_NGFW_SMC_python_monitoring.egg-info/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       21 2021-06-10 15:38:49.000000 fp-NGFW-SMC-python-monitoring-1.4.0/fp_NGFW_SMC_python_monitoring.egg-info/top_level.txt
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        1 2021-06-10 15:38:49.000000 fp-NGFW-SMC-python-monitoring-1.4.0/fp_NGFW_SMC_python_monitoring.egg-info/dependency_links.txt
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1212 2021-06-10 15:38:49.000000 fp-NGFW-SMC-python-monitoring-1.4.0/fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       51 2021-06-10 15:38:49.000000 fp-NGFW-SMC-python-monitoring-1.4.0/fp_NGFW_SMC_python_monitoring.egg-info/requires.txt
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    11297 2021-06-10 15:38:49.000000 fp-NGFW-SMC-python-monitoring-1.4.0/fp_NGFW_SMC_python_monitoring.egg-info/PKG-INFO
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        1 2021-06-10 15:38:45.000000 fp-NGFW-SMC-python-monitoring-1.4.0/fp_NGFW_SMC_python_monitoring.egg-info/not-zip-safe
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    11297 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/PKG-INFO
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       42 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-monitoring-1.4.0/MANIFEST.in
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)       67 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/setup.cfg
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     1510 2021-06-10 15:06:04.000000 fp-NGFW-SMC-python-monitoring-1.4.0/setup.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/tests/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     6524 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/tests/test_queries.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    16154 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/tests/test_filters.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     9071 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/tests/docker_smc_bootstrap.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-monitoring-1.4.0/tests/__init__.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/pubsub/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4832 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/pubsub/subscribers.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)        0 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/pubsub/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     8422 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/wsocket.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    13376 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/query.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    21654 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/constants.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     7801 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/formatters.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)    11439 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/filters.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5862 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/calendar.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5493 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/values.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     6890 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/formats.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      201 2020-01-21 17:33:45.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      123 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/__init__.py
-drwxrwxr-x   0 vdsouza   (1000) vdsouza   (1000)        0 2021-06-10 15:38:50.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     8169 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/logs.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4652 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/routes.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     6301 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/vpns.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5501 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/alerts.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     3611 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/sslvpn.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     5016 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/connections.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4018 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/users.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     4684 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/neighbors.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)      259 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/__init__.py
--rw-rw-r--   0 vdsouza   (1000) vdsouza   (1000)     8039 2021-05-13 14:34:13.000000 fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/blacklist.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       40 2023-05-25 13:16:11.000000 fp-NGFW-SMC-python-monitoring-1.4.1/MANIFEST.in
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9361 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/PKG-INFO
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7334 2022-10-19 07:17:48.000000 fp-NGFW-SMC-python-monitoring-1.4.1/README.rst
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.523753 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9361 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/PKG-INFO
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     1238 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)        1 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/dependency_links.txt
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)        1 2023-05-26 09:31:55.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/not-zip-safe
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       51 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/requires.txt
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       21 2023-05-26 09:34:53.000000 fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/top_level.txt
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       67 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/setup.cfg
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     2065 2023-05-25 13:34:06.000000 fp-NGFW-SMC-python-monitoring-1.4.1/setup.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.523753 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      678 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/__init__.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      756 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/__init__.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6416 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/calendar.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    23470 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/constants.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    11993 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/filters.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7444 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/formats.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     8355 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/formatters.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    14473 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/query.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6974 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/values.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      814 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/__init__.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6055 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/alerts.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9936 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/blacklist.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9653 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/block_list.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     6303 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/connections.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     8723 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/logs.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5976 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/neighbors.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5938 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/routes.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     4899 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/sslvpn.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5306 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/users.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7588 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/vpns.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      554 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/__init__.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     5355 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/subscribers.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    10017 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/wsocket.py
+drwxrwxr-x   0 lvalero   (1000) lvalero   (1000)        0 2023-05-26 09:34:53.527753 fp-NGFW-SMC-python-monitoring-1.4.1/tests/
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)      554 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/tests/__init__.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     9625 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/tests/docker_smc_bootstrap.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)    16709 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/tests/test_filters.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)     7079 2023-05-25 12:54:03.000000 fp-NGFW-SMC-python-monitoring-1.4.1/tests/test_queries.py
+-rw-rw-r--   0 lvalero   (1000) lvalero   (1000)       18 2023-05-26 09:31:29.000000 fp-NGFW-SMC-python-monitoring-1.4.1/version.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/README.rst` & `fp-NGFW-SMC-python-monitoring-1.4.1/README.rst`

 * *Files identical despite different names*

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt` & `fp-NGFW-SMC-python-monitoring-1.4.1/fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-HISTORY.rst
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
 version.py
 fp_NGFW_SMC_python_monitoring.egg-info/PKG-INFO
 fp_NGFW_SMC_python_monitoring.egg-info/SOURCES.txt
@@ -19,14 +18,15 @@
 smc_monitoring/models/formats.py
 smc_monitoring/models/formatters.py
 smc_monitoring/models/query.py
 smc_monitoring/models/values.py
 smc_monitoring/monitors/__init__.py
 smc_monitoring/monitors/alerts.py
 smc_monitoring/monitors/blacklist.py
+smc_monitoring/monitors/block_list.py
 smc_monitoring/monitors/connections.py
 smc_monitoring/monitors/logs.py
 smc_monitoring/monitors/neighbors.py
 smc_monitoring/monitors/routes.py
 smc_monitoring/monitors/sslvpn.py
 smc_monitoring/monitors/users.py
 smc_monitoring/monitors/vpns.py
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/tests/test_queries.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/tests/test_queries.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
+
 import unittest
 from smc_monitoring.monitors.logs import LogQuery
 from smc_monitoring.models.formats import TextFormat, DetailedFormat, RawFormat, CombinedFormat
 from smc_monitoring.models.constants import LogField
 from smc_monitoring.models.calendar import datetime_to_ms, datetime_from_ms, TimeFormat
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/tests/test_filters.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/tests/test_filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
+
 import unittest
 from pprint import pprint
 from smc_monitoring.monitors.logs import LogQuery
 from smc_monitoring.models.values import (
     FieldValue,
     IPValue,
     ServiceValue,
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/tests/docker_smc_bootstrap.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/tests/docker_smc_bootstrap.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Used to bootstrap the SMC into a docker container. Provides a clean installed version
 with pre-existing license with SMC API enabled. All ports are forwarded from the native
 docker host to the private SMC address, including Web Start.
 
 In this configuration, docker is installed on CentOS7 (which uses systemd)
 To enable docker remote API. http://sudoall.com/docker-remote-api-on-centos/
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/pubsub/subscribers.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/pubsub/subscribers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,19 @@
-"""
-Created on Sep 24, 2017
-"""
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
+
 from smc.base.model import Element
 from smc_monitoring.wsocket import SMCSocketProtocol
 
 
 EVENT_ACTIONS = set(["create",
                      "update",
                      "delete",
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/wsocket.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/wsocket.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,29 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
+
 import os
 import ssl
 import json
 import select
 import logging
 import threading
 import time
 from pprint import pformat
 from smc import session
+from smc.compat import PYTHON_v3_9
 
 import websocket
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -47,21 +60,22 @@
 class SMCSocketProtocol(websocket.WebSocket):
     """
     SMCSocketProtocol manages the web socket connection between this
     client and the SMC. It provides the interface to monitor the query
     results and yield them back to the caller as a context manager.
     """
 
-    def __init__(self, query, query_timeout=None, sock_timeout=3, **kw):
+    def __init__(self, query, query_timeout=None, sock_timeout=3, inactivity_timeout=None, **kw):
         """
         Initialize the web socket.
 
         :param Query query: Query type from `smc_monitoring.monitors`
         :param int query_timeout: length of time to wait on recieving web
-            socket results.
+            socket results (total query time).
+        :param int inactivity_timeout: length of time before exiting if no new entry.
         :param int sock_timeout: length of time to wait on a select call
             before trying to receive data. For LogQueries, this should be
             short, i.e. 1 second. For other queries the default is 3 sec.
         :param int max_recv: for queries that are not 'live', set
             this to supply a max number of receive iterations.
         :param kw: supported keyword args:
             cert_reqs: ssl.CERT_NONE|ssl.CERT_REQUIRED|ssl.CERT_OPTIONAL
@@ -69,15 +83,15 @@
             enable_multithread: True|False (Default: True)
 
         .. note:: The keyword args are not required unless you want to override
             default settings. If SSL is used for the SMC session, the settings
             for verifying the server with the root CA is based on whether the
             'verify' setting has been provided with a path to the root CA file.
         """
-        if not session.session or not session.session.cookies:
+        if not session.session:
             raise SessionNotFound(
                 "No SMC session found. You must first "
                 "obtain an SMC session through session.login before making "
                 "a web socket connection."
             )
 
         sslopt = {}
@@ -111,26 +125,36 @@
             kw.update(enable_multithread=True)
 
         # Max number of receives, configurable for batching
         self.max_recv = kw.pop("max_recv", 0)
 
         super(SMCSocketProtocol, self).__init__(sslopt=sslopt, **kw)
         self.query_timeout = query_timeout
+        self.inactivity_timeout = inactivity_timeout
         self.query = query
         self.fetch_id = None
         # Inner thread used to keep socket select alive
         self.thread = None
         self.event = threading.Event()
         self.sock_timeout = sock_timeout
 
     def __enter__(self):
-        self.connect(
-            url=session.web_socket_url +
-            self.query.location,
-            cookie=session.session_id)
+        if session.session_id is None:
+            sock = session.sock
+            if sock is None:
+                # Need to obtain new socket
+                session.refresh()
+            self.connect(
+                url=session.web_socket_url + self.query.location,
+                socket=session.sock)
+        else:
+            self.connect(
+                url=session.web_socket_url + self.query.location,
+                cookie=session.session_id)
+
         if self.connected:
             self.settimeout(self.sock_timeout)
             self.on_open()
         return self
 
     def __exit__(self, exctype, value, traceback):
         if exctype in (SystemExit, GeneratorExit):
@@ -182,34 +206,36 @@
         has a timeout, the SMC will not reply with a message more
         than every two minutes.
         """
         try:
             itr = 0
             if self.connected and self.query_timeout:
                 start = time.time()
+                inactivity_start = time.time()
             while self.connected:
-
-                r, w, e = select.select((self.sock,), (), (), 10.0)
+                r, w, e = select.select((self.sock,), (), (), self.sock_timeout)
 
                 if r:
+                    if self.inactivity_timeout:
+                        inactivity_start = time.time()
                     message = json.loads(self.recv())
 
                     if "fetch" in message:
                         self.fetch_id = message["fetch"]
 
                     if "failure" in message:
                         raise InvalidFetch(message["failure"])
 
                     if "records" in message:
                         if "added" in message["records"]:
                             num = len(message["records"]["added"])
                         else:
                             num = len(message["records"])
 
-                        logger.debug("Query returned %s records.", num)
+                        logger.info("Query returned %s records.", num)
                         if self.max_recv:
                             itr += 1
 
                     if "end" in message:
                         logger.debug(
                             "Received end message: %s" %
                             message["end"])
@@ -219,15 +245,21 @@
                     yield message
                     if self.max_recv and self.max_recv <= itr:
                         break
 
                 if self.query_timeout:
                     progress = time.time()
                     if self.query_timeout < int(progress - start):
-                        logger.info("Socket recieve timeout")
+                        logger.info("Socket receive query timeout")
+                        break
+
+                if self.inactivity_timeout:
+                    progress = time.time()
+                    if self.inactivity_timeout < int(progress - inactivity_start):
+                        logger.info("Socket receive inactivity timeout")
                         break
 
         except (Exception, KeyboardInterrupt, SystemExit, FetchAborted) as e:
             logger.info(
                 "Caught exception in receive: %s -> %s",
                 type(e),
                 str(e))
@@ -238,11 +270,12 @@
             if self.connected:
                 if self.fetch_id:
                     self.send(json.dumps({"abort": self.fetch_id}))
                 self.close()
 
             if self.thread:
                 self.event.set()
-                while self.thread.isAlive():
+                while (not PYTHON_v3_9 and self.thread.isAlive()) or \
+                      (PYTHON_v3_9 and self.thread.is_alive()):
                     self.event.wait(1)
 
             logger.info("Closed web socket connection normally.")
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/query.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/query.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 A Query is the top level object used to construct parameters to make queries
 to the SMC.
 
 Query is the parent class for all monitors in package :py:mod:`smc_monitoring.monitors`
 
 Each monitor type will have it's own predefined set of log fields that are considered
@@ -285,14 +296,17 @@
         This fetch should be used if you want to return only the result records
         returned from the query in raw dict format. Any other dict key/values
         from the raw query are ignored.
 
         :param int max_recv: max number of socket receive calls before
             returning from this query. If you want to wait longer for
             results before returning, increase max_iterations (default: 0)
+        :param int query_timeout: length of time to wait on recieving web
+            socket results (total query time).
+        :param int inactivity_timeout: length of time before exiting if no new entry.
         :return: list of query results
         :rtype: list(dict)
         """
         self.sockopt.update(kw)
         with SMCSocketProtocol(self, **self.sockopt) as protocol:
             for result in protocol.receive():
                 if "records" in result and result["records"].get("added"):
@@ -302,14 +316,19 @@
         """
         Fetch and return in the specified format. Output format is a formatter
         class in :py:mod:`smc_monitoring.models.formatters`. This fetch type will
         be a single shot fetch unless providing max_recv keyword with a value
         greater than the default of 1. Keyword arguments available are kw in
         :meth:`.fetch_raw`.
 
+        :param int query_timeout: length of time to wait on recieving web
+            socket results (total query time).
+        :param int inactivity_timeout: length of time before exiting if no new entry.
+        :param int max_recv: for queries that are not 'live', set
+            this to supply a max number of receive iterations.
         :param formatter: Formatter type for data representation. Any type
             in :py:mod:`smc_monitoring.models.formatters`.
         :return: generator returning data in specified format
 
         .. note:: You can provide your own formatter class,
             see :py:mod:`smc_monitoring.models.formatters` for more info.
         """
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/constants.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/constants.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Constants used within :py:mod:`smc_monitoring.models.values.Value` values to simplify
 referencing log viewer data.
 """
 
 
 class LogField:
@@ -115,14 +126,30 @@
     BLACKLISTENTRYSOURCEPORT = 123  #: Blacklist entry source port
     BLACKLISTENTRYSOURCEPORTRANGE = 124  #: Blacklist entry source port range end
     BLACKLISTENTRYDESTINATIONPORT = 125  #: Blacklist entry destination port
     #: Blacklist entry destination port range end
     BLACKLISTENTRYDESTINATIONPORTRANGE = 126
     BLACKLISTENTRYDURATION = 127  #: Blacklist entry duration
     BLACKLISTER = 128  #: Blacklister
+    # BLOCK_LIST renaming
+    BLOCK_LISTENTRYID = 117  #: None
+    BLOCK_LISTENTRYSOURCEIP = 118  #: block_list entry source IP address
+    BLOCK_LISTENTRYSOURCEIPMASK = 119  #: block_list entry source IP address mask
+    BLOCK_LISTENTRYDESTINATIONIP = 120  #: block_list entry destination IP address
+    #: block_list entry destination IP address mask
+    BLOCK_LISTENTRYDESTINATIONIPMASK = 121
+    BLOCK_LISTENTRYPROTOCOL = 122  #: block_list entry IP protocol
+    BLOCK_LISTENTRYSOURCEPORT = 123  #: block_list entry source port
+    BLOCK_LISTENTRYSOURCEPORTRANGE = 124  #: block_list entry source port range end
+    BLOCK_LISTENTRYDESTINATIONPORT = 125  #: block_list entry destination port
+    #: block_list entry destination port range end
+    BLOCK_LISTENTRYDESTINATIONPORTRANGE = 126
+    BLOCK_LISTENTRYDURATION = 127  #: block_list entry duration
+    BLOCK_LISTER = 128  #: block_lister
+
     QOSCLASS = 129  #: QoS Class
     DSCPMARK = 130  #: DSCP Mark
     QOSPRIORITY = 131  #: QoS Priority
     SERVICEKEY = 132  #: Service primary key, used in service resolving
     AUTHMETHOD = 133  #: Authentication Method element
     IPSAPPID = 134  #: Network application detected in the connection
     #: TLS Match detected in the connection. Note that a single connection
@@ -150,14 +177,20 @@
     ROUTEBGPPATH = 167  #: Active BGP path
     POTENTIALLYDUPLICATERESPONSE = 170  #: Potentially duplicate correlation response
     #: Blacklist entry source IP address prefix length
     BLACKLISTENTRYSOURCEIPPREFIXLEN = 172
     BLACKLISTENTRYDESTINATIONIPPREFIXLEN = (
         173  #: Blacklist entry destination IP address prefix length
     )
+    # BLOCK_LIST renaming
+    #: block_list entry source IP address prefix length
+    BLOCK_LISTENTRYSOURCEIPPREFIXLEN = 172
+    BLOCK_LISTENTRYDESTINATIONIPPREFIXLEN = (
+        173  #: block_list entry destination IP address prefix length
+    )
     SFPINGRESS = 900  #: SFP_INGRESS
     IKEDHGROUP = 901  #: Diffie-Hellman Group
     RWPHTTPREFERRER = 832  #: HTTP Referrer
     NODESTATUS = 300  #: Node status
     NODEVERSION = 301  #: Node version
     #: Session monitoring event code (1 = new, 2 = update, 3 = remove, 4 = all sessions sent)
     SESSIONEVENT = 302
@@ -218,14 +251,16 @@
     NUMLOGEVENTS = 363  #: Number of log events
     NUMLOGRESPONSES = 364  #: Number of log responses performed by this engine
     NUMALERTRESPONSES = 365  #: Number of alert responses performed by this engine
     NUMRECORDRESPONSES = 366  #: Number of record responses performed by this engine
     NUMRESETRESPONSES = 367  #: Number of reset responses performed by this engine
     NUMDISCARDRESPONSES = 368  #: Number of discard responses performed by this engine
     NUMBLACKLISTRESPONSES = 369  #: Number of blacklist responses performed by this engine
+    # BLACKLIST renaming
+    NUMBLOCK_LISTRESPONSES = 369  #: Number of block_list responses performed by this engine
     SENSORINTERFACEKEY = 370  #: Sensor interface key
     SENSORTRAFFIC = 372  #: Sensor traffic
     SENSORTRAFFICPROCESSEDPACKETS = 373  #: Processed Packets
     SENSORTRAFFICPROCESSEDBYTES = 374  #: Processed Bytes
     SENSORTRAFFICLOSTPACKETS = 375  #: Lost Packets
     SENSORTRAFFICINSPECTEDPACKETS = 376  #: Inspected Packets
     SENSORTRAFFICSTATSOFPACKETS = 377  #: Stats Of Packets
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/formatters.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/formatters.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Custom formats used to return data in different formats.
 These are used from the query itself when calling the fetch_as_format()
 method.
 For example, returning a LogQuery as a table::
 
     query = LogQuery(fetch_size=200)
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/filters.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/filters.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Filters are used by queries to refine how results are returned.
 
 QueryFilter is the top level 'interface' for all filter types. The ``filter``
 attribute of a QueryFilter provides access to the compiled query string used
 to build the filter. Each QueryFilter also has an ``update_filter`` method
 that can be used to swap new filters in and out of an existing query.
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/calendar.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/calendar.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Time formats are optionally used in a LogQuery to specify custom ranges for
 which to search 'stored' log events.
 
 When adding a time format to a query, the ``start_time`` and ``end_time`` values
 need to be in milliseconds. The engine logs are stored in UTC time but in order
 to display the client side dates properly, you should set a timezone on the
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/values.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/values.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Values are used to provide searchable input for filters.
 Each value format is specific to the data type added to the filter. For example,
 an IPValue specifies IP's or network values that can be added to a filter from
 :py:mod:`smc_monitoring.models.filters`.
 
 Each constructor can be initialized in the following ways:
@@ -172,12 +183,42 @@
 
     def __init__(self, *values):
         value = [{"type": "string", "value": value} for value in values]
         super(StringValue, self).__init__(value)
 
 
 class NumberValue(Value):
-    pass
+    """
+    Number value match.
+
+    Search for port in source fields::
+
+    query = LogQuery(fetch_size=10)
+    query.add_in_filter(FieldValue(LogField.SPORT), [NumberValue(7000, 7001)])
+
+    :param value: number definitions
+    :type value: list or int
+    """
+
+    def __init__(self, *values):
+        value = [{"type": "number", "value": value} for value in values]
+        super(NumberValue, self).__init__(value)
 
 
 class TranslatedValue(Value):
-    pass
+    """
+    Internal SMC filter format value match.
+    To use with "translated" filter
+
+    Search for port in destination fields::
+
+    query = LogQuery(fetch_size=10)
+    query_filter = QueryFilter("translated")
+    query_filter.update_filter(TranslatedValue("$Dport == 22 OR $Dport == 25").value)
+    query.update_filter(query_filter)
+
+    :param value: specifies a string in the internal SMC filter format.
+    :type value: str
+    """
+
+    def __init__(self, value):
+        super(TranslatedValue, self).__init__(value)
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/models/formats.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/models/formats.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Field formats represent a way to control the format of the returned data.
 By modifying a field format, you can control field level settings such as
 wther to resolve IP's via DNS, how to display field names and values and
 which fields to return in the query.
 
 Each log format will return a different view type The most common and default
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/logs.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/logs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 LogQuery provides an interface to the SMC Log Viewer to retrieve data
 in real time or by batch.
 
 There are a variety of settings you can configure on a query such as whether
 to execute a real time query versus a stored log fetch, time frame for the
 query, fetch size quantity, returned format style, specify which fields to
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/routes.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/routes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Query the current routing table entries.
 
 Create a query to obtain all connections for a given engine::
 
     query = RoutingQuery('sg_vm')
 
@@ -62,38 +73,56 @@
         super(RoutingQuery, self).__init__("ROUTING", target, **kw)
 
     def fetch_as_element(self, **kw):
         """
         Fetch the results and return as a RoutingView element. The original
         query is not modified.
 
+        :param int query_timeout: length of time to wait on recieving web
+            socket results (total query time).
+        :param int inactivity_timeout: length of time before exiting if no new entry.
+        :param int max_recv: for queries that are not 'live', set
+            this to supply a max number of receive iterations.
         :return: generator of elements
         :rtype: :class:`.RoutingView`
         """
         clone = self.copy()
         clone.format.field_format("id")
         for custom_field in ["field_ids", "field_names"]:
             clone.format.data.pop(custom_field, None)
 
         for list_of_results in clone.fetch_raw(**kw):
             for entry in list_of_results:
+                first_fetch = entry.get("first_fetch")
+                first_fetch = first_fetch if first_fetch else False
+                entry.update({"first_fetch": first_fetch})
                 yield RoutingView(**entry)
 
 
 class RoutingView(object):
     """
     A Routing View represents an entry in the current routing table.
     This is the result of making a :class:`.RoutingQuery` and using
     :meth:`~RoutingQuery.fetch_as_element`.
     """
 
     def __init__(self, **data):
         self.rt = data
 
     @property
+    def first_fetch(self):
+        """
+        first fetch
+        True means entry is part of initial data at first fetch
+
+        :rtype: bool
+        """
+        return self.rt.get("first_fetch")
+
+    @property
     def timestamp(self):
         """
         Timestamp of this connection. It is recommended to set the timezone
         on the query to view this timestamp in the systems local time.
         For example::
 
             query.format.timezone('CST')
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/vpns.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/alerts.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,254 +1,228 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
-Get all active VPN SA's.
+ActiveAlert Query provides the ability to view current alert entries from the
+alert log viewer.
+When creating the query, you must specify a target which speifies the SMC domain
+for which to retrieve the alerts.
 
-Create a query to obtain all connections for a given engine::
-
-    query = VPNSAQuery('sg_vm')
-
-Add a timezone to the query::
+A basic alert query using a local timezone example::
 
+    query = ActiveAlertQuery('Shared Domain')
     query.format.timezone('CST')
 
-Execute query and return raw results::
-
-    for records in query.fetch_batch():
-        ...
-
-Execute query and return as a :class:`.VPNSecurityAssoc` element::
+You can also use standard filters to specify a more exact match, for example, showing
+alerts with a severity of CRITICAL::
 
-    for records in query.fetch_as_element():
-        ...
-
-Delete a VPN SA::
-
-    query = VPNSAQuery('sg_vm')
-    for sa in query.fetch_as_element():
-        sa.delete()
-
-.. seealso:: :class:`smc_monitoring.models.filters` for more information on creating filters
+    query.add_in_filter(
+        FieldValue(LogField.ALERTSEVERITY), [ConstantValue(Alerts.CRITICAL)])
 
 """
+
 from smc_monitoring.models.query import Query
 from smc_monitoring.models.constants import LogField
-from smc.base.model import prepared_request
-from smc.api.exceptions import DeleteElementFailed
 
 
-class VPNSAQuery(Query):
+class ActiveAlertQuery(Query):
     """
-    Show all current VPN SA's on the specified target.
+    Active Alert Query is an interface to the alert log viewer in Log Server.
+    This query type provides the ability to fetch and filter on active
+    alerts.
 
-    :ivar list field_ids: field IDs are the default fields for this entry type
-        and are constants found in :class:`smc_monitoring.models.constants.LogField`
+    You can create a new query specifying a valid timezone abbreviation::
 
-    :param str target: name of target engine/cluster
+        query = ActiveAlertQuery('Shared Domain', timezone='CST')
+
+    Or alternatively no timezone::
+
+        query = ActiveAlertQuery('DomainFoo')
+
+    :param str target: domain for which to filter alerts. Default: 'Shared Domain'
+    :param str timezone: timezone for timestamps, i.e. 'CST', etc
     """
 
     location = "/monitoring/session/socket"
     field_ids = [
         LogField.TIMESTAMP,
+        LogField.ALERTSEVERITY,
+        LogField.ACTION,
         LogField.NODEID,
-        LogField.VPNID,
-        LogField.SECURITYGATEWAY,
-        LogField.PEERSECURITYGATEWAY,
-        LogField.IKECOOKIE,
-        LogField.ENDPOINT,
-        LogField.PEERENDPOINT,
-        LogField.SACLASS,
-        LogField.CIPHERALG,
-        LogField.NEGOTIATIONROLE,
-        LogField.SRCADDRS,
-        LogField.DSTADDRS,
+        LogField.SRC,
+        LogField.DST,
+        LogField.SERVICE,
         LogField.PROTOCOL,
-        LogField.NUMBYTESSENT,
-        LogField.NUMBYTESRECEIVED,
-        LogField.EXPIRATIONTIME,
+        LogField.SPORT,
+        LogField.DPORT,
+        LogField.SITUATION,
+        LogField.VULNERABILITYREFERENCES,
     ]
 
-    def __init__(self, target, **kw):
-        super(VPNSAQuery, self).__init__("VPN_SA", target, **kw)
+    def __init__(self, target="Shared Domain", timezone=None):
+        super(ActiveAlertQuery, self).__init__("ACTIVE_ALERTS", target)
+        if timezone is not None:
+            self.format.set_resolving(timezone=timezone)
 
     def fetch_as_element(self, **kw):
         """
-        Fetch the results and return as a VPNSecurityAssoc element.
-        The original query is not modified.
+        Fetch the results and return as a User element. The original
+        query is not modified.
 
-        :return: generator of elements
-        :rtype: :class:`~VPNSecurityAssoc`
+        :return: generator returning element instances
+        :rtype: Alert
         """
         clone = self.copy()
         clone.format.field_format("id")
         for custom_field in ["field_ids", "field_names"]:
             clone.format.data.pop(custom_field, None)
 
         for list_of_results in clone.fetch_raw(**kw):
             for entry in list_of_results:
-                yield VPNSecurityAssoc(**entry)
+                yield Alert(**entry)
 
 
-class VPNSecurityAssoc(object):
+class Alert(object):
     """
-    A VPN Security Association represents a currently connected VPN
-    endpoint. This is the result of making a :class:`.VPNSAQuery` and
-    using :meth:`~VPNSAQuery.fetch_as_element`.
+    Alert definition returned from specified domain.
+    This is the result of making a :class:`.ActiveAlertQuery` and using
+    :meth:`~ActiveAlertQuery.fetch_as_element`.
     """
 
     def __init__(self, **data):
-        self.vpn = data
-
-    @property
-    def href(self):
-        return self.vpn.get("vpn_sa_href")
-
-    def delete(self):
-        return prepared_request(DeleteElementFailed, href=self.href).delete()
+        self.alert = data
 
     @property
     def timestamp(self):
         """
         Timestamp of this connection. It is recommended to set the timezone
         on the query to view this timestamp in the systems local time.
         For example::
 
             query.format.timezone('CST')
 
+        :return timestamp in string format
         :rtype: str
         """
-        return self.vpn.get(str(LogField.TIMESTAMP))
+        return self.alert.get(str(LogField.TIMESTAMP))
 
     @property
     def engine(self):
         """
-        The engine/cluster for this VPN
-
-        :rtype: str
-        """
-        return self.vpn.get(str(LogField.NODEID))
-
-    @property
-    def local_gateway(self):
-        """
-        Local gateway for this VPN.
-
-        :rtype: str
-        """
-        return self.vpn.get(str(LogField.SECURITYGATEWAY))
-
-    @property
-    def peer_gateway(self):
-        """
-        Peer gateway for this VPN.
+        The engine/cluster for this state table entry
 
+        :return: engine or cluster for this entry
         :rtype: str
         """
-        return self.vpn.get(str(LogField.PEERSECURITYGATEWAY))
+        return self.alert.get(str(LogField.NODEID))
 
     @property
-    def local_endpoint(self):
+    def severity(self):
         """
-        Local endpoint (IP address) for this VPN tunnel.
+        Severity for this alert
 
         :rtype: str
         """
-        return self.vpn.get(str(LogField.ENDPOINT))
+        return self.alert.get(str(LogField.ALERTSEVERITY))
 
     @property
-    def peer_endpoint(self):
+    def action(self):
         """
-        Peer endpoint element and IP Address for this tunnel.
+        Action performed for the alert
 
         :rtype: str
         """
-        return self.vpn.get(str(LogField.PEERENDPOINT))
+        return self.alert.get(str(LogField.ACTION))
 
     @property
-    def local_networks(self):
+    def source(self):
         """
-        Local protected networks
+        Source IP for the alert
 
         :rtype: str
         """
-        return self.vpn.get(str(LogField.SRCADDRS))
+        return self.alert.get(str(LogField.SRC))
 
     @property
-    def peer_networks(self):
+    def destination(self):
         """
-        Remote protected networks
+        Destination IP for the alert
 
         :rtype: str
         """
-        return self.vpn.get(str(LogField.DSTADDRS))
-
-    @property
-    def vpn_id(self):
-        return self.vpn.get(str(LogField.VPNID))
+        return self.alert.get(str(LogField.DST))
 
     @property
-    def sa_type(self):
+    def service(self):
         """
-        SA Type for this VPN tunnel. Each VPN tunnel will typically have
-        at least two entries, one for IPSEC and another for IKE.
+        Service associated with alert
 
         :rtype: str
         """
-        return self.vpn.get(str(LogField.SACLASS))
+        return self.alert.get(str(LogField.SERVICE))
 
     @property
     def protocol(self):
         """
-        WHich protocol is associated with this tunnel entry.
+        Protocol for alert
 
-        :return: IP protocol for tunnel, i.e. ESP/UDP
         :rtype: str
         """
-        return self.vpn.get(str(LogField.PROTOCOL))
+        return self.alert.get(str(LogField.PROTOCOL))
 
     @property
-    def negotiation_role(self):
+    def source_port(self):
         """
-        Role for this tunnel entry.
+        Source port for alert
 
-        :return: Negotiation role, i.e. Initiator, Responder, etc.
-        :rtype: str
+        :rtype: int
         """
-        return self.vpn.get(str(LogField.NEGOTIATIONROLE))
+        return int(self.alert.get(str(LogField.SPORT)))
 
     @property
-    def bytes_sent(self):
+    def destination_port(self):
         """
-        Number of bytes sent.
+        Destination port for alert
 
         :rtype: int
         """
-        return int(self.vpn.get(str(LogField.NUMBYTESSENT), 0))
+        return int(self.alert.get(str(LogField.DPORT)))
 
     @property
-    def bytes_received(self):
+    def situation(self):
         """
-        Number of bytes received.
+        Situation defined for this alert
 
-        :rtype: int
+        :rtype: str
         """
-        return int(self.vpn.get(str(LogField.NUMBYTESRECEIVED), 0))
+        return self.alert.get(str(LogField.SITUATION))
 
     @property
-    def expiration(self):
+    def vulnerability_refs(self):
         """
-        Expiration time for this tunnel Security Association
+        Comma seperated string listing any vulnerability references for
+        the alert, if any.
 
         :rtype: str
         """
-        return self.vpn.get(str(LogField.EXPIRATIONTIME))
+        return self.alert.get(str(LogField.VULNERABILITYREFERENCES))
 
     def __str__(self):
-        return "{}(local={},peer={},localip={},peerip={},satype={})".format(
+        return "{}(severity={},src={},dst={},action={},situation={})".format(
             self.__class__.__name__,
-            self.local_gateway,
-            self.peer_gateway,
-            self.local_endpoint,
-            self.peer_endpoint,
-            self.sa_type,
+            self.severity,
+            self.source,
+            self.destination,
+            self.action,
+            self.situation,
         )
 
     def __repr__(self):
         return str(self)
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/alerts.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/connections.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,217 +1,230 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
-ActiveAlert Query provides the ability to view current alert entries from the
-alert log viewer.
-When creating the query, you must specify a target which speifies the SMC domain
-for which to retrieve the alerts.
+A connection query returns all currently connected sessions on the
+given target.
 
-A basic alert query using a local timezone example::
+Create a query to obtain all connections for a given engine::
+
+    query = ConnectionQuery('sg_vm')
+
+Add a timezone to the query::
 
-    query = ActiveAlertQuery('Shared Domain')
     query.format.timezone('CST')
 
-You can also use standard filters to specify a more exact match, for example, showing
-alerts with a severity of CRITICAL::
+Add a filter to only get connections if the source address is 172.18.1.252::
 
-    query.add_in_filter(
-        FieldValue(LogField.ALERTSEVERITY), [ConstantValue(Alerts.CRITICAL)])
+    query.add_in_filter(FieldValue(LogField.SRC), [IPValue('172.18.1.252')])
 
-"""
+Only connections that match a specific service::
 
-from smc_monitoring.models.query import Query
-from smc_monitoring.models.constants import LogField
+    query.add_in_filter(FieldValue(LogField.SERVICE), [ServiceValue('TCP/443', 'UDP/53')])
 
+Execute query and return raw results::
 
-class ActiveAlertQuery(Query):
-    """
-    Active Alert Query is an interface to the alert log viewer in Log Server.
-    This query type provides the ability to fetch and filter on active
-    alerts.
+    for records in query.fetch_raw():
+        ...
 
-    You can create a new query specifying a valid timezone abbreviation::
+Execute query and return as an :class:`.Connection` element::
 
-        query = ActiveAlertQuery('Shared Domain', timezone='CST')
+    for records in query.fetch_as_element():
+        ...
 
-    Or alternatively no timezone::
+Retrieving live streaming results::
 
-        query = ActiveAlertQuery('DomainFoo')
+    for records in query.fetch_live():
+        ...
+
+.. seealso:: :class:`smc_monitoring.models.filters` for more information on creating filters
+
+"""
+from smc_monitoring.models.query import Query
+from smc_monitoring.models.constants import LogField
 
-    :param str target: domain for which to filter alerts. Default: 'Shared Domain'
-    :param str timezone: timezone for timestamps, i.e. 'CST', etc
+
+class ConnectionQuery(Query):
+    """
+    Show all current connections on the specified target.
+
+    :ivar list field_ids: field IDs are the default fields for this entry type
+        and are constants found in :class:`smc_monitoring.models.constants.LogField`
+
+    :param str target: name of target engine/cluster
     """
 
     location = "/monitoring/session/socket"
     field_ids = [
         LogField.TIMESTAMP,
-        LogField.ALERTSEVERITY,
-        LogField.ACTION,
         LogField.NODEID,
         LogField.SRC,
+        LogField.SPORT,
+        LogField.SRCZONE,
         LogField.DST,
+        LogField.DPORT,
+        LogField.DSTZONE,
         LogField.SERVICE,
+        LogField.IPSAPPID,
         LogField.PROTOCOL,
-        LogField.SPORT,
-        LogField.DPORT,
-        LogField.SITUATION,
-        LogField.VULNERABILITYREFERENCES,
+        LogField.STATE,
     ]
 
-    def __init__(self, target="Shared Domain", timezone=None):
-        super(ActiveAlertQuery, self).__init__("ACTIVE_ALERTS", target)
-        if timezone is not None:
-            self.format.set_resolving(timezone=timezone)
+    def __init__(self, target, **kw):
+        super(ConnectionQuery, self).__init__("CONNECTIONS", target, **kw)
 
     def fetch_as_element(self, **kw):
         """
-        Fetch the results and return as a User element. The original
+        Fetch the results and return as a Connection element. The original
         query is not modified.
 
-        :return: generator returning element instances
-        :rtype: Alert
+        :param int query_timeout: length of time to wait on recieving web
+            socket results (total query time).
+        :param int inactivity_timeout: length of time before exiting if no new entry.
+        :param int max_recv: for queries that are not 'live', set
+            this to supply a max number of receive iterations.
+        :return: generator of elements
+        :rtype: :class:`.Connection`
         """
         clone = self.copy()
         clone.format.field_format("id")
         for custom_field in ["field_ids", "field_names"]:
             clone.format.data.pop(custom_field, None)
 
         for list_of_results in clone.fetch_raw(**kw):
             for entry in list_of_results:
-                yield Alert(**entry)
+                first_fetch = entry.get("first_fetch")
+                first_fetch = first_fetch if first_fetch else False
+                entry.update({"first_fetch": first_fetch})
+                yield Connection(**entry)
 
 
-class Alert(object):
+class Connection(object):
     """
-    Alert definition returned from specified domain.
-    This is the result of making a :class:`.ActiveAlertQuery` and using
-    :meth:`~ActiveAlertQuery.fetch_as_element`.
+    Connection represents a state table entry. This is the result of
+    making a :class:`~ConnectionQuery` and using
+    :meth:`~ConnectionQuery.fetch_as_element`.
     """
 
     def __init__(self, **data):
-        self.alert = data
+        self.cxn = data
+
+    @property
+    def first_fetch(self):
+        """
+        first fetch
+        True means entry is part of initial data at first fetch
+
+        :rtype: bool
+        """
+        return self.cnx.get("first_fetch")
 
     @property
     def timestamp(self):
         """
         Timestamp of this connection. It is recommended to set the timezone
         on the query to view this timestamp in the systems local time.
         For example::
 
             query.format.timezone('CST')
 
-        :return timestamp in string format
+        :return: timestamp in string format
         :rtype: str
         """
-        return self.alert.get(str(LogField.TIMESTAMP))
+        return self.cxn.get(str(LogField.TIMESTAMP))
 
     @property
     def engine(self):
         """
         The engine/cluster for this state table entry
 
         :return: engine or cluster for this entry
         :rtype: str
         """
-        return self.alert.get(str(LogField.NODEID))
+        return self.cxn.get(str(LogField.NODEID))
 
     @property
-    def severity(self):
+    def source_addr(self):
         """
-        Severity for this alert
+        Source address for this entry
 
         :rtype: str
         """
-        return self.alert.get(str(LogField.ALERTSEVERITY))
+        return self.cxn.get(str(LogField.SRC))
 
     @property
-    def action(self):
+    def dest_addr(self):
         """
-        Action performed for the alert
+        Destination address for this entry
 
         :rtype: str
         """
-        return self.alert.get(str(LogField.ACTION))
-
-    @property
-    def source(self):
-        """
-        Source IP for the alert
-
-        :rtype: str
-        """
-        return self.alert.get(str(LogField.SRC))
-
-    @property
-    def destination(self):
-        """
-        Destination IP for the alert
-
-        :rtype: str
-        """
-        return self.alert.get(str(LogField.DST))
+        return self.cxn.get(str(LogField.DST))
 
     @property
     def service(self):
         """
-        Service associated with alert
+        Service for this entry
 
+        :return: service (HTTP/HTTPS, etc)
         :rtype: str
         """
-        return self.alert.get(str(LogField.SERVICE))
+        return self.cxn.get(str(LogField.SERVICE))
 
     @property
     def protocol(self):
         """
-        Protocol for alert
+        Protocol for this entry
 
+        :return: protocol (UDP/TCP/ICMP, etc)
         :rtype: str
         """
-        return self.alert.get(str(LogField.PROTOCOL))
+        return self.cxn.get(str(LogField.PROTOCOL), "ANY")
 
     @property
     def source_port(self):
         """
-        Source port for alert
+        Source port for the entry.
 
         :rtype: int
         """
-        return int(self.alert.get(str(LogField.SPORT)))
+        return int(self.cxn.get(str(LogField.SPORT), 0))
 
     @property
-    def destination_port(self):
+    def dest_port(self):
         """
-        Destination port for alert
+        Destination port for the entry.
 
         :rtype: int
         """
-        return int(self.alert.get(str(LogField.DPORT)))
-
-    @property
-    def situation(self):
-        """
-        Situation defined for this alert
-
-        :rtype: str
-        """
-        return self.alert.get(str(LogField.SITUATION))
+        return int(self.cxn.get(str(LogField.DPORT), 0))
 
     @property
-    def vulnerability_refs(self):
+    def state(self):
         """
-        Comma seperated string listing any vulnerability references for
-        the alert, if any.
+        State of the connection.
 
+        :return: state, i.e. UDP established, TCP established, etc.
         :rtype: str
         """
-        return self.alert.get(str(LogField.VULNERABILITYREFERENCES))
+        return self.cxn.get(str(LogField.STATE))
 
     def __str__(self):
-        return "{}(severity={},src={},dst={},action={},situation={})".format(
+        return "{}(src={},dst={},proto={},dst_port={},state={})".format(
             self.__class__.__name__,
-            self.severity,
-            self.source,
-            self.destination,
-            self.action,
-            self.situation,
+            self.source_addr,
+            self.dest_addr,
+            self.protocol,
+            self.dest_port,
+            self.state,
         )
 
     def __repr__(self):
         return str(self)
```

### Comparing `fp-NGFW-SMC-python-monitoring-1.4.0/smc_monitoring/monitors/blacklist.py` & `fp-NGFW-SMC-python-monitoring-1.4.1/smc_monitoring/monitors/blacklist.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+#  Licensed under the Apache License, Version 2.0 (the "License"); you may
+#  not use this file except in compliance with the License. You may obtain
+#  a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
+#  WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
+#  License for the specific language governing permissions and limitations
+#  under the License.
 """
 Blacklist Query provides the ability to view current blacklist entries in the
 SMC by target. Target is defined as the cluster or engine. Retrieved results
 will have a reference to the entry and hence be possible to remove the entry.
 ::
 
     query = BlacklistQuery('sg_vm')
@@ -40,16 +51,18 @@
 
 .. seealso:: :class:`smc_monitoring.models.filters` for more information on creating filters
 
 """
 from smc_monitoring.models.query import Query
 from smc_monitoring.models.formats import TextFormat, CombinedFormat, DetailedFormat
 from smc_monitoring.models.constants import LogField
+from smc_monitoring.monitors.block_list import BlockListQuery
 from smc.base.model import prepared_request
 from smc.api.exceptions import DeleteElementFailed
+from smc.compat import is_api_version_less_than, is_smc_version_less_than
 
 
 class BlacklistQuery(Query):
     """
     Query existing blacklist entries for a given cluster/engine.
     It is generally recommended to set your local timezone when making a
     query to convert the timestamp into a relevant format.
@@ -74,21 +87,30 @@
         LogField.NODEID,
         LogField.SENDERDOMAIN,
         LogField.BLACKLISTENTRYID,
     ]
 
     def __init__(self, target, timezone=None, **kw):
 
-        super(BlacklistQuery, self).__init__("BLACKLIST", target, **kw)
+        if is_smc_version_less_than("7.0"):
+            super(BlacklistQuery, self).__init__("BLACKLIST", target, **kw)
+        else:
+            super(BlacklistQuery, self).__init__("BLOCK_LIST", target, **kw)
+
         if timezone is not None:
             self.format.set_resolving(timezone=timezone)
 
     def fetch_as_element(self, **kw):
         """
         Fetch the blacklist and return as an instance of Element.
+        :param int query_timeout: length of time to wait on recieving web
+            socket results (total query time).
+        :param int inactivity_timeout: length of time before exiting if no new entry.
+        :param int max_recv: for queries that are not 'live', set
+            this to supply a max number of receive iterations.
 
         :return: generator returning element instances
         :rtype: BlacklistEntry
         """
         clone = self.copy()
         # Replace all filters with a combined filter
         bldata = TextFormat(field_format="name")
@@ -103,14 +125,17 @@
         combined = CombinedFormat(bldata=bldata, blid=blid)
         clone.update_format(combined)
 
         for list_of_results in clone.fetch_raw(**kw):
             for entry in list_of_results:
                 data = entry.get("bldata")
                 data.update(**entry.get("blid"))
+                first_fetch = entry.get("first_fetch")
+                first_fetch = first_fetch if first_fetch else False
+                data.update({"first_fetch": first_fetch})
                 yield BlacklistEntry(**data)
 
 
 class BlacklistEntry(object):
     """
     A blacklist entry represents an entry in the engines kernel table
     indicating that a source/destination/port/protocol mapping is currently
@@ -133,14 +158,34 @@
         within the Management Client.
 
         :rtype: str
         """
         return self.blacklist.get("Blacklist Entry ID")
 
     @property
+    def blacklist_entry_key(self):
+        """
+        Blacklist entry Key.
+        Needed to remove the entry
+
+        :rtype: str
+        """
+        return self.blacklist.get("BlacklistEntryId")
+
+    @property
+    def first_fetch(self):
+        """
+        first fetch
+        True means entry is part of initial data at first fetch
+
+        :rtype: bool
+        """
+        return self.blacklist.get("first_fetch")
+
+    @property
     def timestamp(self):
         """
         Timestamp when this blacklist entry was added.
 
         :rtype: str
         """
         return self.blacklist.get("Timestamp")
@@ -158,15 +203,19 @@
     def href(self):
         """
         The href for this blacklist entry. This is the reference to the
         entry for deleting the entry.
 
         :rtype: str
         """
-        return self.blacklist.get("blacklist_href")
+        if is_api_version_less_than("7.0"):
+            ref = "blacklist_href"
+        else:
+            ref = "block_list_href"
+        return self.blacklist.get(ref)
 
     @property
     def source(self):
         """
         Source address/netmask for this blacklist entry.
 
         :rtype: str
```

